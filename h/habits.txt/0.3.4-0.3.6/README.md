# Comparing `tmp/habits_txt-0.3.4.tar.gz` & `tmp/habits_txt-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habits_txt-0.3.4.tar", max compression
+gzip compressed data, was "habits_txt-0.3.6.tar", max compression
```

## Comparing `habits_txt-0.3.4.tar` & `habits_txt-0.3.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     3109 2024-05-14 20:37:42.341037 habits_txt-0.3.4/README.md
--rwxr-xr-x   0        0        0      788 2024-05-15 17:43:14.132064 habits_txt-0.3.4/bin/hbtxt.py
--rw-r--r--   0        0        0        0 2024-05-14 20:25:35.415585 habits_txt-0.3.4/habits_txt/__init__.py
--rw-r--r--   0        0        0    13971 2024-05-15 17:43:14.132064 habits_txt-0.3.4/habits_txt/builder.py
--rw-r--r--   0        0        0     7980 2024-05-16 07:15:40.194208 habits_txt-0.3.4/habits_txt/cli.py
--rw-r--r--   0        0        0     2154 2024-05-14 20:25:35.415585 habits_txt-0.3.4/habits_txt/config.py
--rw-r--r--   0        0        0      224 2024-05-14 20:25:35.415585 habits_txt-0.3.4/habits_txt/defaults.py
--rw-r--r--   0        0        0     2323 2024-05-15 17:43:14.132064 habits_txt-0.3.4/habits_txt/directives.py
--rw-r--r--   0        0        0      380 2024-05-14 20:25:35.415585 habits_txt-0.3.4/habits_txt/exceptions.py
--rw-r--r--   0        0        0     8107 2024-05-15 18:01:28.344968 habits_txt-0.3.4/habits_txt/journal.py
--rw-r--r--   0        0        0     2940 2024-05-15 17:43:14.132064 habits_txt-0.3.4/habits_txt/models.py
--rw-r--r--   0        0        0     9037 2024-05-15 17:43:14.132064 habits_txt-0.3.4/habits_txt/parser.py
--rw-r--r--   0        0        0      952 2024-05-14 20:25:35.415585 habits_txt-0.3.4/habits_txt/records_query.py
--rw-r--r--   0        0        0      627 2024-05-16 07:15:40.194208 habits_txt-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 habits_txt-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     3184 2024-05-17 10:07:19.291761 habits_txt-0.3.6/README.md
+-rwxr-xr-x   0        0        0      788 2024-05-15 17:43:14.132064 habits_txt-0.3.6/bin/hbtxt.py
+-rw-r--r--   0        0        0        0 2024-05-14 20:25:35.415585 habits_txt-0.3.6/habits_txt/__init__.py
+-rw-r--r--   0        0        0    13971 2024-05-15 17:43:14.132064 habits_txt-0.3.6/habits_txt/builder.py
+-rw-r--r--   0        0        0     7980 2024-05-16 07:15:40.194208 habits_txt-0.3.6/habits_txt/cli.py
+-rw-r--r--   0        0        0     2154 2024-05-14 20:25:35.415585 habits_txt-0.3.6/habits_txt/config.py
+-rw-r--r--   0        0        0      224 2024-05-14 20:25:35.415585 habits_txt-0.3.6/habits_txt/defaults.py
+-rw-r--r--   0        0        0     2323 2024-05-15 17:43:14.132064 habits_txt-0.3.6/habits_txt/directives.py
+-rw-r--r--   0        0        0      380 2024-05-14 20:25:35.415585 habits_txt-0.3.6/habits_txt/exceptions.py
+-rw-r--r--   0        0        0     8089 2024-05-17 13:06:12.645011 habits_txt-0.3.6/habits_txt/journal.py
+-rw-r--r--   0        0        0     2940 2024-05-15 17:43:14.132064 habits_txt-0.3.6/habits_txt/models.py
+-rw-r--r--   0        0        0     9037 2024-05-15 17:43:14.132064 habits_txt-0.3.6/habits_txt/parser.py
+-rw-r--r--   0        0        0      952 2024-05-14 20:25:35.415585 habits_txt-0.3.6/habits_txt/records_query.py
+-rw-r--r--   0        0        0      698 2024-05-17 13:06:12.645011 habits_txt-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3558 1970-01-01 00:00:00.000000 habits_txt-0.3.6/PKG-INFO
```

### Comparing `habits_txt-0.3.4/README.md` & `habits_txt-0.3.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 You can then use the CLI with:
 
 ```bash
 hbtxt --help
 ```
 
+Alternatively, you can use the executable provided by the latest release.
+
 ## Concepts
 
 ### Time-bound
 
 A habit is time-bound. It has a start date, and eventually an end date.
 It means with habits.txt, you can track habits for a specific period of time. When you want to stop tracking a habit, you can just stop tracking it.
```

### Comparing `habits_txt-0.3.4/bin/hbtxt.py` & `habits_txt-0.3.6/bin/hbtxt.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.4/habits_txt/builder.py` & `habits_txt-0.3.6/habits_txt/builder.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.4/habits_txt/cli.py` & `habits_txt-0.3.6/habits_txt/cli.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.4/habits_txt/config.py` & `habits_txt-0.3.6/habits_txt/config.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.4/habits_txt/directives.py` & `habits_txt-0.3.6/habits_txt/directives.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.4/habits_txt/journal.py` & `habits_txt-0.3.6/habits_txt/journal.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             )
         if next_due_date <= date:
             append = True
             if interactive:
                 value_is_valid = False
                 parsed_value = None
                 while not value_is_valid:
-                    value = input(f"{habit.name} ({next_due_date}): ")
+                    value = input(f"{habit.name}: ")
                     if value == "s":
                         append = False
                         break
                     elif value == "a":
                         break
                     try:
                         parsed_value = parser.parse_value_str(value)
```

### Comparing `habits_txt-0.3.4/habits_txt/models.py` & `habits_txt-0.3.6/habits_txt/models.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.4/habits_txt/parser.py` & `habits_txt-0.3.6/habits_txt/parser.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.4/habits_txt/records_query.py` & `habits_txt-0.3.6/habits_txt/records_query.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.4/pyproject.toml` & `habits_txt-0.3.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "habits.txt"
-version = "0.3.4"
+version = "0.3.6"
 description = ""
 authors = ["estebanthi <esteban.thilliez@gmail.com>"]
 readme = "README.md"
 packages = [
     {include = "habits_txt"}, {include = "bin"}
 ]
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = ">=3.12,<3.13"
 croniter = "^2.0.5"
 click = "^8.1.7"
 
 [tool.poetry.scripts]
 hbtxt = "bin.hbtxt:main"
 
 
@@ -23,10 +23,14 @@
 isort = "^5.13.2"
 flake8 = "^7.0.0"
 black = "^24.4.2"
 mypy = "^1.10.0"
 types-croniter = "^2.0.0.20240423"
 pre-commit = "^3.7.1"
 
+
+[tool.poetry.group.build.dependencies]
+pyinstaller = "^6.6.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `habits_txt-0.3.4/PKG-INFO` & `habits_txt-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: habits.txt
-Version: 0.3.4
+Version: 0.3.6
 Summary: 
 Author: estebanthi
 Author-email: esteban.thilliez@gmail.com
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.12,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: croniter (>=2.0.5,<3.0.0)
 Description-Content-Type: text/markdown
 
 # habits.txt
@@ -27,14 +27,16 @@
 
 You can then use the CLI with:
 
 ```bash
 hbtxt --help
 ```
 
+Alternatively, you can use the executable provided by the latest release.
+
 ## Concepts
 
 ### Time-bound
 
 A habit is time-bound. It has a start date, and eventually an end date.
 It means with habits.txt, you can track habits for a specific period of time. When you want to stop tracking a habit, you can just stop tracking it.
```

