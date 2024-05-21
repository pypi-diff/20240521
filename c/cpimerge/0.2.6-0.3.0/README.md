# Comparing `tmp/cpimerge-0.2.6.tar.gz` & `tmp/cpimerge-0.3.0.tar.gz`

## Comparing `cpimerge-0.2.6.tar` & `cpimerge-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.2.6/src/cpimerge/__init__.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 cpimerge-0.2.6/src/cpimerge/__main__.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 cpimerge-0.2.6/src/cpimerge/backup.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 cpimerge-0.2.6/src/cpimerge/config.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 cpimerge-0.2.6/src/cpimerge/descriptions.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 cpimerge-0.2.6/src/cpimerge/exclusions.py
--rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 cpimerge-0.2.6/src/cpimerge/gui.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 cpimerge-0.2.6/src/cpimerge/ical.py
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 cpimerge-0.2.6/src/cpimerge/load.py
--rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 cpimerge-0.2.6/src/cpimerge/merge.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 cpimerge-0.2.6/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cpimerge-0.2.6/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.2.6/README.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 cpimerge-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cpimerge-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.3.0/cpimerge/__init__.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 cpimerge-0.3.0/cpimerge/__main__.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 cpimerge-0.3.0/cpimerge/backup.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 cpimerge-0.3.0/cpimerge/config.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 cpimerge-0.3.0/cpimerge/descriptions.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 cpimerge-0.3.0/cpimerge/exclusions.py
+-rw-r--r--   0        0        0    12170 2020-02-02 00:00:00.000000 cpimerge-0.3.0/cpimerge/gui.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 cpimerge-0.3.0/cpimerge/ical.py
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 cpimerge-0.3.0/cpimerge/load.py
+-rw-r--r--   0        0        0     5990 2020-02-02 00:00:00.000000 cpimerge-0.3.0/cpimerge/merge.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 cpimerge-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cpimerge-0.3.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.3.0/README.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 cpimerge-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cpimerge-0.3.0/PKG-INFO
```

### Comparing `cpimerge-0.2.6/src/cpimerge/config.py` & `cpimerge-0.3.0/cpimerge/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from appdirs import user_data_dir
 from tkinter import messagebox
 
 # Define application name and author for appdirs
 APP_NAME = "cpimerge"
 APP_AUTHOR = "Kirk Coombs"
 
-# Get configuation file directory (per-OS)
+# Get configuration file directory (per-OS)
 def get_appdir():
     config_dir = user_data_dir(APP_NAME, APP_AUTHOR)
     os.makedirs(config_dir, exist_ok=True)
     return os.path.join(config_dir, 'config.json')
 
 # Load configuration from file
 def load_config(config_path):
@@ -27,8 +27,8 @@
 
 # Save configuration to file
 def save_config(config, config_path):
     try:
         with open(config_path, 'w') as f:
             json.dump(config, f, indent=4)
     except Exception as e:
-        messagebox.showerror("Error", f"Failed to save configuration file: {e}")
+        messagebox.showerror("Error", f"Failed to save configuration file: {e}")
```

### Comparing `cpimerge-0.2.6/src/cpimerge/descriptions.py` & `cpimerge-0.3.0/cpimerge/descriptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,6 +1,7 @@
-descriptions = {
+gui_descriptions = {
+    "root_title": "CPI iCal Merger",
     "ics1_description": "The iCal (.ics) file you used for the previous run of this tool.\n\nThis file will automatically be backed-up.\n\nIf no file, or an invalid file, is provided, an empty iCal with no events will be used. This useful for the first run of this program.",
     "ics2_description": "The new iCal (.ics) file to grab events from. These events will be merged with events from ics1, if provided.",
     "exclusions_description": "An optional file containing sub-strings, one per line. When matched, these sub-strings will cause an event to be excluded from the output.",
     "output_description": "An output iCal (.ics) file, which will contain any new events. This can be imported into to your calendar."
 }
```

### Comparing `cpimerge-0.2.6/src/cpimerge/exclusions.py` & `cpimerge-0.3.0/cpimerge/exclusions.py`

 * *Files identical despite different names*

### Comparing `cpimerge-0.2.6/src/cpimerge/ical.py` & `cpimerge-0.3.0/cpimerge/ical.py`

 * *Files identical despite different names*

### Comparing `cpimerge-0.2.6/src/cpimerge/load.py` & `cpimerge-0.3.0/cpimerge/load.py`

 * *Files identical despite different names*

### Comparing `cpimerge-0.2.6/src/cpimerge/merge.py` & `cpimerge-0.3.0/cpimerge/merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,17 @@
         filtered_events = filter_exclusions(unique_events_ics2, exclusions, output_text)
 
         # Create a new calendar of all-day events from the filtered_events
         output_cal = Calendar()
         for event in filtered_events:
             output_cal.add_component(create_all_day_event(event))
 
+        #
+        # TO DO: This should not include filtered events!
+        #
         # If there was a ics1, report any event that exits in cal1 but not cal2 as possible removals, in sorted order
         if os.path.exists(ics1_path):
             if len(unique_events_ics1):
                 output_text.insert(tk.END, f"Consider removing the following events from your calendar. They existed in '{ics1_path}' but are not in '{ics2_path}' and thus may no longer be relevant:\n")
                 for event in sorted(unique_events_ics1, key=lambda x: x[1]):
                     output_text.insert(tk.END, f"  - {event[0]} on {event[1].date()}\n")
             else:
@@ -78,14 +81,15 @@
         if rename_ics2:
             if os.path.exists(ics1_path):
                 backup_ics1_path = backup_file(ics1_path)
                 output_text.insert(tk.END, f"\nBackup of '{ics1_path}' created: {backup_ics1_path}\n")
             if os.path.exists(ics2_path):
                 backup_ics2_path = backup_file(ics2_path)
                 output_text.insert(tk.END, f"\nBackup of '{ics2_path}' created: {backup_ics2_path}\n")   
+            os.remove(ics1_path)
             os.rename(ics2_path, ics1_path)
             output_text.insert(tk.END, f"\nRenamed {ics2_path} to {ics1_path} for use for the next run.\n")
 
     except Exception as e:
         messagebox.showerror("Error", f"An unknown error occurred during the merge process: {e}")
 
 # Run merge process
@@ -110,17 +114,8 @@
 
     if exclusions_path and not os.path.exists(exclusions_path):
         messagebox.showerror("Error", f"File not found: {exclusions_path}")
         return
 
     output_text.delete(1.0, tk.END)
     merge(ics1_path, ics2_path, exclusions_path if exclusions_path else None, output_path, output_text, rename_ics2)
-    output_text.insert(tk.END, f"\nCalendars merged successfully.\n\n** You can now import the new events from {output_path} **")
-
-    # Save the configuration
-    config = {
-        "ics1_path": ics1_path,
-        "ics2_path": ics2_path,
-        "exclusions_path": exclusions_path,
-        "output_path": output_path
-    }
-    save_config(config, config_path)
+    output_text.insert(tk.END, f"\nCalendars merged successfully.\n\n** You can now import the new events from {output_path} **")
```

### Comparing `cpimerge-0.2.6/.gitignore` & `cpimerge-0.3.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -156,8 +156,9 @@
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 # Test files
-tests/
+tests/
+cpimerge/graph.py
```

### Comparing `cpimerge-0.2.6/LICENSE` & `cpimerge-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cpimerge-0.2.6/pyproject.toml` & `cpimerge-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpimerge"
-version = "0.2.6"
+version = "0.3.0"
 dependencies = [
   "icalendar",
   "appdirs",
 ]
 authors = [
   { name="Kirk Coombs", email="cpimerge@coombscloud.com" },
 ]
```

