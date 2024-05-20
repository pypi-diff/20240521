# Comparing `tmp/needto-0.1.5.tar.gz` & `tmp/needto-0.1.6.tar.gz`

## Comparing `needto-0.1.5.tar` & `needto-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 needto-0.1.5/needto/__about__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 needto-0.1.5/needto/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 needto-0.1.5/needto/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 needto-0.1.5/needto/src/__init__.py
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 needto-0.1.5/needto/src/ai_client.py
--rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 needto-0.1.5/needto/src/cli.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 needto-0.1.5/needto/src/config.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 needto-0.1.5/needto/src/utils.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 needto-0.1.5/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 needto-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 needto-0.1.5/README.md
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 needto-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 needto-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 needto-0.1.6/needto/__about__.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 needto-0.1.6/needto/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 needto-0.1.6/needto/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 needto-0.1.6/needto/src/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 needto-0.1.6/needto/src/ai_client.py
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 needto-0.1.6/needto/src/cli.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 needto-0.1.6/needto/src/config.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 needto-0.1.6/needto/src/utils.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 needto-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 needto-0.1.6/LICENSE.txt
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 needto-0.1.6/README.md
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 needto-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 needto-0.1.6/PKG-INFO
```

### Comparing `needto-0.1.5/needto/src/ai_client.py` & `needto-0.1.6/needto/src/ai_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,7 +85,10 @@
                         "role": "user",
                         "content": "Last response was not JSON. Always write JSON.",
                     }
                 )
             else:
                 self.messages.append({"role": "system", "content": answer})
                 return parsed_answer
+
+        console.print("Failed to get response from AI model.")
+        sys.exit(1)
```

### Comparing `needto-0.1.5/needto/src/cli.py` & `needto-0.1.6/needto/src/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import os
 import click
 import sys
 import typer
 import rich.console
 import rich.prompt
 import subprocess
@@ -130,15 +131,15 @@
         if files_to_save:
             if selected_file_name := prompt_menu_and_print(
                 list(files_to_save.keys()),
                 preview_command=lambda file_name: files_to_save.get(file_name, ""),
             ):
                 file_content = files_to_save[selected_file_name]
                 while os.path.exists(selected_file_name):
-                    selected_file_name = console.print(
+                    selected_file_name = rich.prompt.Prompt.ask(
                         f"[bold red]'{selected_file_name}' already exists[/bold red]. Please enter a new name",
                     )
                 with open(selected_file_name, "w") as f:
                     f.write(file_content)
                 console.print(f"'{selected_file_name}' saved.", style="bold green")
                 break
 
@@ -146,10 +147,44 @@
         if user_prompt := input("> "):
             print()
             parsed_answer = ai_client.ask(user_prompt)
         else:
             break
 
 
+@app.command(help="Monitor system and notify.")
+async def monitor(
+    prompt_list: list[str],
+    monitor_script: str,
+    notify_script: str,
+    sleep_seconds: int = 60,
+):
+    prompt = " ".join(prompt_list)
+    system_prompt = """
+    You are a system monitor. User will ask you to monitor a system and notify them if something goes wrong.
+    Don't write markdown.
+    Response should always be JSON stars with "{" and ends with "}" with these keys:
+    "message" (text), "should_notify" (bool)
+    Don't explain at begin or end of JSON.
+    """
+    console = rich.console.Console()
+    ai_client = AIClient(system_prompt=system_prompt)
+    parsed_answer = ai_client.ask(prompt)
+
+    while True:
+        await asyncio.sleep(sleep_seconds)
+        print("running monitor script")
+        monitor_output = subprocess.run(monitor_script, shell=True, capture_output=True)
+        ai_client.ask(
+            "Output of monitor script:\n"
+            + f"stdout:\n{monitor_output.stdout.decode()}\n"
+            + (
+                f"stderr:\n{monitor_output.stderr.decode()}"
+                if monitor_output.stderr
+                else ""
+            )
+        )
+
+
 @app.command(help=f"Open editor for '{config_manager.config_path}'.")
 def config():
     click.edit(filename=config_manager.config_path)
```

### Comparing `needto-0.1.5/needto/src/config.py` & `needto-0.1.6/needto/src/config.py`

 * *Files identical despite different names*

### Comparing `needto-0.1.5/needto/src/utils.py` & `needto-0.1.6/needto/src/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import sys
 from simple_term_menu import TerminalMenu
 import rich.console
 import rich.prompt
 
 EDITOR_TEMPLATE = """{command}
 
-# save this file to confirm the command or quit to skip it.
-# after save, you will {confirm_prompt} this command.
+# Save this file to confirm the command or quit to skip it.
+# After save, you will {confirm_prompt} this command.
 """
 
 
 @functools.cache
 def stdin_is_atty():
     return sys.stdin.isatty()
 
@@ -32,15 +32,19 @@
     preview_command: None | str | typing.Callable[[str], str] = None,
 ):
     items_to_prompt: list[str] = [no_op_value] + items
     menu_entry_index = TerminalMenu(
         [command.replace("|", r"\|") for command in items_to_prompt],
         preview_command=preview_command,
     ).show()
-    selected_item: str = items_to_prompt[menu_entry_index]
+
+    if isinstance(menu_entry_index, int):
+        selected_item: str = items_to_prompt[menu_entry_index]
+    else:
+        return
 
     if selected_item == no_op_value:
         return
 
     if ask_for_edit and stdin_is_atty():
         if edited_text := click.edit(
             text=EDITOR_TEMPLATE.format(
@@ -61,15 +65,15 @@
         sys.stdin = get_tty_file()
 
         if confirm_prompt and not rich.prompt.Confirm.ask(
             f"{confirm_prompt} '{selected_item}'", default=False
         ):
             return
 
-    return selected_item
+    return typing.cast(str, selected_item)
 
 
 def prompt_menu_and_print(
     items: list[str],
     *,
     ask_for_edit=False,
     no_op_value="-- non of this options, want to explain more --",
@@ -80,17 +84,21 @@
         items,
         ask_for_edit=ask_for_edit,
         no_op_value=no_op_value,
         confirm_prompt=confirm_prompt,
         preview_command=preview_command,
     )
 
+    items_to_print = items
+    if selected_item and selected_item not in items:
+        items_to_print.append(selected_item)
+
     console = rich.console.Console()
     print()
-    for command in items:
+    for command in items_to_print:
         if command == selected_item:
             console.print(f"$ {command}", style="black on white")
         else:
             console.print(f"$ {command}")
     print()
 
     return selected_item
```

### Comparing `needto-0.1.5/.gitignore` & `needto-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `needto-0.1.5/LICENSE.txt` & `needto-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `needto-0.1.5/README.md` & `needto-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `needto-0.1.5/pyproject.toml` & `needto-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `needto-0.1.5/PKG-INFO` & `needto-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: needto
-Version: 0.1.5
+Version: 0.1.6
 Summary: Ask AI for help you in your terminal.
 Project-URL: Documentation, https://github.com/danialkeimasi/needto#readme
 Project-URL: Issues, https://github.com/danialkeimasi/needto/issues
 Project-URL: Source, https://github.com/danialkeimasi/needto
 Author-email: Danial Keimasi <danialkeimasi@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

