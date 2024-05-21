# Comparing `tmp/cdbt-0.2.1.tar.gz` & `tmp/cdbt-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdbt-0.2.1.tar", last modified: Thu May 16 17:53:02 2024, max compression
+gzip compressed data, was "cdbt-0.2.3.tar", last modified: Tue May 21 04:49:55 2024, max compression
```

## Comparing `cdbt-0.2.1.tar` & `cdbt-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-16 17:53:02.242105 cdbt-0.2.1/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      466 2024-05-16 17:53:02.241466 cdbt-0.2.1/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)     4072 2024-05-16 17:52:30.000000 cdbt-0.2.1/README.md
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-16 17:53:02.225898 cdbt-0.2.1/cdbt/
--rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-15 13:54:01.000000 cdbt-0.2.1/cdbt/__init__.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     6103 2024-05-16 03:59:44.000000 cdbt-0.2.1/cdbt/build_dbt_docs_ai.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     7330 2024-05-16 03:59:44.000000 cdbt-0.2.1/cdbt/build_unit_test_data_ai.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     5669 2024-05-16 17:29:29.000000 cdbt-0.2.1/cdbt/cmdline.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    16656 2024-05-16 17:50:08.000000 cdbt-0.2.1/cdbt/main.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    17490 2024-05-16 03:59:44.000000 cdbt-0.2.1/cdbt/prompts.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-16 17:53:02.240963 cdbt-0.2.1/cdbt.egg-info/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      466 2024-05-16 17:53:02.000000 cdbt-0.2.1/cdbt.egg-info/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)      327 2024-05-16 17:53:02.000000 cdbt-0.2.1/cdbt.egg-info/SOURCES.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-16 17:53:02.000000 cdbt-0.2.1/cdbt.egg-info/dependency_links.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2024-05-16 17:53:02.000000 cdbt-0.2.1/cdbt.egg-info/entry_points.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       51 2024-05-16 17:53:02.000000 cdbt-0.2.1/cdbt.egg-info/requires.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-16 17:53:02.000000 cdbt-0.2.1/cdbt.egg-info/top_level.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-16 17:53:02.242204 cdbt-0.2.1/setup.cfg
--rwxr-xr-x   0 craiglathrop   (501) staff       (20)      710 2024-05-16 17:52:30.000000 cdbt-0.2.1/setup.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-16 17:53:02.239826 cdbt-0.2.1/tests/
--rw-r--r--   0 craiglathrop   (501) staff       (20)     7050 2024-05-15 13:54:01.000000 cdbt-0.2.1/tests/test_main.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-21 04:49:55.508609 cdbt-0.2.3/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      466 2024-05-21 04:49:55.508044 cdbt-0.2.3/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4072 2024-05-17 13:41:23.000000 cdbt-0.2.3/README.md
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-21 04:49:55.500752 cdbt-0.2.3/cdbt/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-15 13:54:01.000000 cdbt-0.2.3/cdbt/__init__.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     6134 2024-05-21 02:30:10.000000 cdbt-0.2.3/cdbt/build_dbt_docs_ai.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     7330 2024-05-17 13:41:23.000000 cdbt-0.2.3/cdbt/build_unit_test_data_ai.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     6256 2024-05-21 03:23:30.000000 cdbt-0.2.3/cdbt/cmdline.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    19056 2024-05-21 04:19:11.000000 cdbt-0.2.3/cdbt/main.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    17490 2024-05-17 13:41:23.000000 cdbt-0.2.3/cdbt/prompts.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-21 04:49:55.507698 cdbt-0.2.3/cdbt.egg-info/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      466 2024-05-21 04:49:55.000000 cdbt-0.2.3/cdbt.egg-info/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      327 2024-05-21 04:49:55.000000 cdbt-0.2.3/cdbt.egg-info/SOURCES.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-21 04:49:55.000000 cdbt-0.2.3/cdbt.egg-info/dependency_links.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2024-05-21 04:49:55.000000 cdbt-0.2.3/cdbt.egg-info/entry_points.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       51 2024-05-21 04:49:55.000000 cdbt-0.2.3/cdbt.egg-info/requires.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-21 04:49:55.000000 cdbt-0.2.3/cdbt.egg-info/top_level.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-21 04:49:55.508667 cdbt-0.2.3/setup.cfg
+-rwxr-xr-x   0 craiglathrop   (501) staff       (20)      710 2024-05-21 04:49:44.000000 cdbt-0.2.3/setup.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-21 04:49:55.507234 cdbt-0.2.3/tests/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     7050 2024-05-15 13:54:01.000000 cdbt-0.2.3/tests/test_main.py
```

### Comparing `cdbt-0.2.1/README.md` & `cdbt-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.1/cdbt/build_dbt_docs_ai.py` & `cdbt-0.2.3/cdbt/build_dbt_docs_ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     def main(self, model_name):
         print('''
         1) Build new DBT documentation.
         2) Check existing DBT documentation against model for missing definitions.
         ''')
         mode = int(input())
-
+        print(f'Getting file.')
         sql_file_path = self._get_file_path(model_name)
 
         if 'l4' in sql_file_path.lower() or 'l3' in sql_file_path.lower():
             system_instructions = Prompts().dbt_docs_gte_l3_prompt
         else:
             system_instructions = Prompts().dbt_docs_lte_l2_prompt
```

### Comparing `cdbt-0.2.1/cdbt/build_unit_test_data_ai.py` & `cdbt-0.2.3/cdbt/build_unit_test_data_ai.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.1/cdbt/cmdline.py` & `cdbt-0.2.3/cdbt/cmdline.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             ctx.obj['build_parents'] = True
             ctx.obj['build_parents_count'] = int(count) if count else None  # Default to 1 if no number is specified
 
         return click.Group.get_command(self, ctx, cmd_name)
 
     def list_commands(self, ctx):
         # List of all commands
-        return ['build', 'trun', 'run', 'test', 'compile', 'clip-compile', 'unittest', 'sbuild', 'pbuild', 'build-docs', 'build-unit']
+        return ['help', 'build', 'trun', 'run', 'test', 'compile', 'clip-compile', 'unittest', 'sbuild', 'pbuild', 'build-docs', 'build-unit']
 
 
 cdbt = CustomCmdLoader()
 
 
 @cdbt.command()
 @click.option('--full-refresh', '-f', is_flag=True, help='Run a full refresh on all models.')
@@ -109,21 +109,30 @@
     """Build models based on changes in current state since last build."""
     cdbt_class.sbuild(ctx, full_refresh, threads)
 
 
 @cdbt.command()
 @click.option('--full-refresh', '-f', is_flag=True, help='Force a full refresh on all models in build scope.')
 @click.option('--threads', '-t', type=int, help='Number of threads to use during DBT operations.')
+@click.option('--skip-dl', '--sd', is_flag=True, help='Skip downloading the manifest file from Snowflake. Use the one that was already downloaded.')
 @click.pass_context
-def pbuild(ctx, full_refresh, threads):
+def pbuild(ctx, full_refresh, threads, skip_dl):
     """Build models based on changes from production to current branch."""
-    cdbt_class.pbuild(ctx, full_refresh, threads)
+    cdbt_class.pbuild(ctx, full_refresh, threads, skip_dl)
 
 
 @cdbt.command()
+@click.option('--full-refresh', '-f', is_flag=True, help='Force a full refresh on all models in build scope.')
+@click.option('--threads', '-t', type=int, help='Number of threads to use during DBT operations.')
+@click.pass_context
+def gbuild(ctx, full_refresh, threads):
+    """Build models based on changes from production to current branch."""
+    cdbt_class.gbuild(ctx, full_refresh, threads)
+
+@cdbt.command()
 @click.pass_context
 @click.option('--select', '-s', type=str, help='Name of the model to build unit test data for.')
 def build_docs(ctx, select):
     """Build dbt YML model docs for a model"""
     dbt_docs = BuildDBTDocs()
     dbt_docs.main(select)
```

### Comparing `cdbt-0.2.1/cdbt/main.py` & `cdbt-0.2.3/cdbt/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,16 +87,14 @@
             print(e.stderr)
             print(e.stdout)
             sys.exit(e.returncode)
 
         if not run_result:
             raise DbtError('DBT build failed with errors.')
 
-
-
     def compile(self, ctx: Context, select):
         # We ignore the ctx object as compile has no threads.
         try:
             self.execute_dbt_command_stream('compile', [])
         except subprocess.CalledProcessError as e:
             print(f'Failure while running command: {" ".join(e.cmd)}')
             print(e.stderr)
@@ -125,34 +123,89 @@
         manifest_path = os.path.join('./', target_dir, 'manifest.json')
         # Path to the artifact file that represents the prior build state.
         manifest_artifact_path = os.path.join('./', artifact_dir, 'manifest.json')
 
         self.execute_state_based_build(ctx, artifact_dir, manifest_artifact_path, manifest_path, full_refresh, threads,
                                        roll_back_manifest_flag=True)
 
-    def pbuild(self, ctx: Context, full_refresh, threads):
+    def pbuild(self, ctx: Context, full_refresh, threads, skip_download):
         print('Starting a state build based on production manifest.json')
         artifact_dir = 'logs'
         target_dir = 'target'
         # Pull artifacts from Snowflake. These are the latest production artifacts.
         try:
-            if not self.test_mode:
+            if not self.test_mode and not skip_download:
                 subprocess.run(['dbt', 'run-operation', 'get_last_artifacts'], check=True)
         except subprocess.CalledProcessError as e:
             print(f'Failure while running command: {" ".join(e.cmd)}')
             print(e.stderr)
             print(e.stdout)
             sys.exit(e.returncode)
 
         manifest_path = os.path.join('.', target_dir, 'manifest.json')
         manifest_artifact_path = os.path.join('.', artifact_dir, 'manifest.json')
 
         self.execute_state_based_build(ctx, artifact_dir, manifest_artifact_path, manifest_path, full_refresh, threads,
                                        roll_back_manifest_flag=False)
 
+    def gbuild(self, ctx: Context, full_refresh, threads):
+        """
+        Build based off of a Git diff of changed models.
+
+        Args:
+            ctx:
+            full_refresh:
+            threads:
+
+        Returns:
+
+        """
+        result = subprocess.run(['git', 'diff', '--name-only'], stdout=subprocess.PIPE, text=True)
+        modified_files = result.stdout.splitlines()
+
+        sql_files = [file.split('/')[-1].replace('.sql', '') for file in modified_files if
+                     'models' in file and file.endswith('.sql')]
+
+        # Construct state commands
+        build_children = ctx.obj.get('build_children', False)
+        build_children_count = ctx.obj.get('build_children_count', None)
+        build_parents = ctx.obj.get('build_parents', False)
+        build_parent_count = ctx.obj.get('build_parents_count', None)
+        if build_children:
+            if build_children_count:
+                for i in range(len(sql_files)):
+                    sql_files[i] = f'{sql_files[i]}+{build_children_count}'
+            else:
+                for i in range(len(sql_files)):
+                    sql_files[i] = f'{sql_files[i]}+'
+
+        if build_parents:
+            if build_parent_count:
+                for i in range(len(sql_files)):
+                    sql_files[i] = f'{build_parent_count}+{sql_files[i]}'
+            else:
+                for i in range(len(sql_files)):
+                    sql_files[i] = f'+{sql_files[i]}'
+
+        select_list = ' '.join(sql_files)
+
+        full_refresh = self._scan_for_incremental_full_refresh(state_flags=['--select', select_list],
+                                                               exclude_flags=None,
+                                                               full_refresh=full_refresh)
+
+        args = [
+            '--select', select_list,
+            '--exclude', 'resource_type:seed,resource_type:snapshot',
+            '--threads', str(threads),
+        ]
+        if full_refresh:
+            args.append('--full-refresh')
+
+        self.execute_dbt_command_stream('build', args)
+
     def execute_state_based_build(self, ctx: Context, artifact_dir: str, manifest_artifact_path: str,
                                   manifest_path: str, full_refresh: bool, threads: int, roll_back_manifest_flag: bool):
         if roll_back_manifest_flag and not self.test_mode:
             print(f'Making a backup of the current manifest.json at {manifest_path} to {manifest_artifact_path}')
             # Move the manifest from ./target to ./_artifacts. This becomes the prior state. Only used for local state
             # build. Not used for pdbuild (production build).
             shutil.move(manifest_path, manifest_artifact_path)
@@ -211,15 +264,23 @@
 
         if not run_result:
             e = 'DBT build failed with errors.'
             self.roll_back_manifest(e, manifest_artifact_path, manifest_path)
             raise DbtError('DBT build failed with errors.')
 
     def _scan_for_incremental_full_refresh(self, state_flags, exclude_flags, full_refresh):
-        args = state_flags + exclude_flags
+        if state_flags and exclude_flags:
+            args = state_flags + exclude_flags
+        elif state_flags and not exclude_flags:
+            args = state_flags
+        elif exclude_flags and not state_flags:
+            args = exclude_flags
+        else:
+            args = []
+
         ls_args = args + ['--output-keys', 'name resource_type config', '--output', 'json']
         models_json = self.dbt_ls_to_json(ls_args)
         if not full_refresh:
             for model in models_json:
                 if model['config']['materialized'] == 'incremental':
                     full_refresh = True
                     print(f'Found incremental build model: {model["name"]}. Initiating full refresh.')
@@ -271,15 +332,15 @@
         print(f"DBT build failed. Rolling back manifest state with error\n {e}")
         # Move the manifest.json from _artifacts back to target dir. If the build failed, we want to rebuild against this
         # state, not the one generated by the compile command.
         shutil.move(manifest_artifact_path, manifest_path)
         sys.exit(e.returncode)
 
     @staticmethod
-    def execute_dbt_command_capture(command:str, args: t.List[str]) -> str:
+    def execute_dbt_command_capture(command: str, args: t.List[str]) -> str:
         """
         Executes a DBT command and captures the output without streaming to the stdout.
         Args:
             command: The DBT command to run.
             args: A list of args to pass into the command.
 
         Returns:
@@ -360,15 +421,14 @@
 
         # Iterate over the lines and find the first empty line
         sql_start_index = 0
         for i, line in enumerate(lines):
             if line.startswith('\x1b['):
                 sql_start_index = i + 1
 
-
         # Join the lines from the first empty line to the end
         sql_code = "\n".join(lines[sql_start_index:])
 
         return sql_code
 
     @staticmethod
     def contains_errors(text):
@@ -402,9 +462,12 @@
     # cdbt.build(full_refresh=False, select=None, fail_fast=False)
     # cdbt.trun(full_refresh=False, select=None, fail_fast=False)
     # cdbt.run(full_refresh=False, select=None, fail_fast=False)
     # cdbt.test(select=None, fail_fast=False)
     # cdbt.compile()
     # cdbt.sbuild(ctx=None, full_refresh=False)
     # cdbt.pbuild(ctx=MockCtx(Command('Duck')), full_refresh=False)
-    cdbt.clip_compile(ctx=MockCtx(Command('Duck')), select='stg_acl_agent_call_log_appointments')
+
+    mock_ctx = MockCtx(Command('Duck'))
+    mock_ctx.obj['build_children'] = True
+    cdbt.gbuild(ctx=mock_ctx, full_refresh=False, threads=8)
     sys.exit(0)
```

### Comparing `cdbt-0.2.1/cdbt/prompts.py` & `cdbt-0.2.3/cdbt/prompts.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.1/setup.py` & `cdbt-0.2.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cdbt',
-    version='0.2.1',
+    version='0.2.3',
     description='A CLI tool to manage dbt builds with state handling and manifest management',
     author='Craig Lathrop',
     author_email='development@coldborecapital.com',
     packages=find_packages(),
     install_requires=[
         'click',
         'pyperclip',
```

### Comparing `cdbt-0.2.1/tests/test_main.py` & `cdbt-0.2.3/tests/test_main.py`

 * *Files identical despite different names*

