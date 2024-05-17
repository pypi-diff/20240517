# Comparing `tmp/cpimerge-0.2.1.tar.gz` & `tmp/cpimerge-0.2.2.tar.gz`

## Comparing `cpimerge-0.2.1.tar` & `cpimerge-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.2.1/src/cpimerge/__init__.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpimerge-0.2.1/src/cpimerge/__main__.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 cpimerge-0.2.1/src/cpimerge/backup.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 cpimerge-0.2.1/src/cpimerge/config.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 cpimerge-0.2.1/src/cpimerge/descriptions.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 cpimerge-0.2.1/src/cpimerge/exclusions.py
--rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 cpimerge-0.2.1/src/cpimerge/gui.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 cpimerge-0.2.1/src/cpimerge/ical.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 cpimerge-0.2.1/src/cpimerge/load.py
--rw-r--r--   0        0        0     5684 2020-02-02 00:00:00.000000 cpimerge-0.2.1/src/cpimerge/merge.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 cpimerge-0.2.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cpimerge-0.2.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.2.1/README.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 cpimerge-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cpimerge-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.2.2/src/cpimerge/__init__.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 cpimerge-0.2.2/src/cpimerge/__main__.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 cpimerge-0.2.2/src/cpimerge/backup.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 cpimerge-0.2.2/src/cpimerge/config.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 cpimerge-0.2.2/src/cpimerge/descriptions.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 cpimerge-0.2.2/src/cpimerge/exclusions.py
+-rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 cpimerge-0.2.2/src/cpimerge/gui.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 cpimerge-0.2.2/src/cpimerge/ical.py
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 cpimerge-0.2.2/src/cpimerge/load.py
+-rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 cpimerge-0.2.2/src/cpimerge/merge.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 cpimerge-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cpimerge-0.2.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.2.2/README.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 cpimerge-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cpimerge-0.2.2/PKG-INFO
```

### Comparing `cpimerge-0.2.1/src/cpimerge/config.py` & `cpimerge-0.2.2/src/cpimerge/config.py`

 * *Files identical despite different names*

### Comparing `cpimerge-0.2.1/src/cpimerge/descriptions.py` & `cpimerge-0.2.2/src/cpimerge/descriptions.py`

 * *Files identical despite different names*

### Comparing `cpimerge-0.2.1/src/cpimerge/exclusions.py` & `cpimerge-0.2.2/src/cpimerge/exclusions.py`

 * *Files identical despite different names*

### Comparing `cpimerge-0.2.1/src/cpimerge/gui.py` & `cpimerge-0.2.2/src/cpimerge/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tkinter as tk
 from tkinter import filedialog
-from descriptions import descriptions
-from merge import run_merge
-from load import load_files
+from .descriptions import descriptions
+from .merge import run_merge
+from .load import load_files
 
 # File selection dialog
 def select_file(entry):
     file_path = filedialog.askopenfilename()
     entry.delete(0, tk.END)
     entry.insert(0, file_path)
     check_ics1_entry()
```

### Comparing `cpimerge-0.2.1/src/cpimerge/ical.py` & `cpimerge-0.2.2/src/cpimerge/ical.py`

 * *Files identical despite different names*

### Comparing `cpimerge-0.2.1/src/cpimerge/load.py` & `cpimerge-0.2.2/src/cpimerge/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import tkinter as tk
 from icalendar import Calendar
 from tkinter import messagebox
-from ical import load_ics, get_event_set
-from exclusions import load_exclusions
+from .ical import load_ics, get_event_set
+from .exclusions import load_exclusions
 
 # Function to set text color in the output_text widget
 def insert_text_with_color(text_widget, text, color):
     text_widget.tag_configure(color, foreground=color)
     text_widget.insert(tk.END, text, color)
 
 # Load files and display information
```

### Comparing `cpimerge-0.2.1/src/cpimerge/merge.py` & `cpimerge-0.2.2/src/cpimerge/merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from icalendar import Calendar
 import tkinter as tk
 from tkinter import messagebox
-from ical import load_ics, get_event_set, create_all_day_event
-from config import save_config
-from exclusions import load_exclusions, filter_exclusions
-from backup import backup_file
+from .ical import load_ics, get_event_set, create_all_day_event
+from .config import save_config
+from .exclusions import load_exclusions, filter_exclusions
+from .backup import backup_file
 
 # Main function to merge calendars
 def merge(ics1_path, ics2_path, exclusions_path, output_path, output_text, rename_ics2):
     try:
         # Load the calendars from the input files
         if os.path.exists(ics1_path):
             cal1 = load_ics(ics1_path)
@@ -68,20 +68,20 @@
         with open(output_path, 'wb') as f:
             f.write(output_cal.to_ical())
 
         # If the rename option was chosen, do the backups and the rename
         if rename_ics2:
             if os.path.exists(ics1_path):
                 backup_ics1_path = backup_file(ics1_path)
-                output_text.insert(tk.END, f"Backup of '{ics1_path}' created: {backup_ics1_path}\n")
+                output_text.insert(tk.END, f"\nBackup of '{ics1_path}' created: {backup_ics1_path}\n")
             if os.path.exists(ics2_path):
                 backup_ics2_path = backup_file(ics2_path)
-                output_text.insert(tk.END, f"Backup of '{ics2_path}' created: {backup_ics2_path}\n")   
+                output_text.insert(tk.END, f"\nBackup of '{ics2_path}' created: {backup_ics2_path}\n")   
             os.rename(ics2_path, ics1_path)
-            output_text.insert(tk.END, f"Renamed {ics2_path} to {ics1_path} for use for the next run.\n")
+            output_text.insert(tk.END, f"\nRenamed {ics2_path} to {ics1_path} for use for the next run.\n")
 
     except Exception as e:
         messagebox.showerror("Error", f"An unknown error occurred during the merge process: {e}")
 
 # Run merge process
 def run_merge(ics1_entry, ics2_entry, exclusions_entry, output_entry, rename_var, output_text, config_path):
     ics1_path = ics1_entry.get()
```

### Comparing `cpimerge-0.2.1/.gitignore` & `cpimerge-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cpimerge-0.2.1/LICENSE` & `cpimerge-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cpimerge-0.2.1/pyproject.toml` & `cpimerge-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpimerge"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
   "icalendar",
   "appdirs",
 ]
 authors = [
   { name="Kirk Coombs", email="cpimerge@coombscloud.com" },
 ]
```

