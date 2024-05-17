# Comparing `tmp/halig-0.4.4.tar.gz` & `tmp/halig-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halig-0.4.4.tar", last modified: Sun Dec 10 10:22:47 2023, max compression
+gzip compressed data, was "halig-0.4.5.tar", last modified: Fri May 17 16:50:00 2024, max compression
```

## Comparing `halig-0.4.4.tar` & `halig-0.4.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    34670 2023-06-19 16:50:30.000000 halig-0.4.4/LICENSE
--rw-r--r--   0        0        0     1635 2023-06-19 16:50:30.000000 halig-0.4.4/README.md
--rw-r--r--   0        0        0        0 2023-06-19 16:50:47.000000 halig-0.4.4/halig/__init__.py
--rw-r--r--   0        0        0       22 2023-12-10 10:22:26.033716 halig-0.4.4/halig/__version__.py
--rw-r--r--   0        0        0        0 2023-06-19 16:50:47.000000 halig-0.4.4/halig/commands/__init__.py
--rw-r--r--   0        0        0      385 2023-07-24 17:42:38.529912 halig-0.4.4/halig/commands/base.py
--rw-r--r--   0        0        0     2781 2023-06-19 16:50:47.000000 halig-0.4.4/halig/commands/edit.py
--rw-r--r--   0        0        0     1397 2023-06-19 16:50:47.000000 halig-0.4.4/halig/commands/import_unencrypted.py
--rw-r--r--   0        0        0     1128 2023-07-22 12:38:35.359342 halig-0.4.4/halig/commands/notebooks.py
--rw-r--r--   0        0        0      958 2023-11-29 17:05:03.788220 halig-0.4.4/halig/commands/reencrypt.py
--rw-r--r--   0        0        0     3780 2023-11-29 17:05:03.789219 halig-0.4.4/halig/commands/search.py
--rw-r--r--   0        0        0     1368 2023-11-29 17:05:03.789219 halig-0.4.4/halig/commands/show.py
--rw-r--r--   0        0        0     1468 2023-07-24 17:49:45.965214 halig-0.4.4/halig/encryption.py
--rw-r--r--   0        0        0     2262 2023-11-29 17:05:03.789219 halig-0.4.4/halig/literals.py
--rw-r--r--   0        0        0     4411 2023-11-29 17:05:03.789219 halig-0.4.4/halig/main.py
--rw-r--r--   0        0        0     4341 2023-11-29 17:14:56.563242 halig-0.4.4/halig/settings.py
--rw-r--r--   0        0        0      733 2023-06-19 16:50:47.000000 halig-0.4.4/halig/utils.py
--rw-r--r--   0        0        0     2780 2023-12-10 10:22:47.720482 halig-0.4.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-19 16:50:47.000000 halig-0.4.4/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 16:50:47.000000 halig-0.4.4/tests/commands/__init__.py
--rw-r--r--   0        0        0     2262 2023-11-29 17:05:03.791219 halig-0.4.4/tests/commands/conftest.py
--rw-r--r--   0        0        0     1177 2023-11-29 17:11:21.843414 halig-0.4.4/tests/commands/test_edit.py
--rw-r--r--   0        0        0     1476 2023-11-29 17:11:21.834415 halig-0.4.4/tests/commands/test_import.py
--rw-r--r--   0        0        0     1563 2023-06-19 16:50:47.000000 halig-0.4.4/tests/commands/test_notebooks.py
--rw-r--r--   0        0        0      426 2023-11-29 17:05:03.792219 halig-0.4.4/tests/commands/test_reencrypt.py
--rw-r--r--   0        0        0     1150 2023-11-29 17:11:21.845414 halig-0.4.4/tests/commands/test_show.py
--rw-r--r--   0        0        0     3527 2023-11-29 17:33:35.644381 halig-0.4.4/tests/conftest.py
--rw-r--r--   0        0        0     2318 2023-11-29 17:32:13.310156 halig-0.4.4/tests/test_encryption.py
--rw-r--r--   0        0        0     1121 2023-11-29 17:33:54.514204 halig-0.4.4/tests/test_settings.py
--rw-r--r--   0        0        0     1516 2023-11-29 17:05:03.792219 halig-0.4.4/tests/test_utils.py
--rw-r--r--   0        0        0     3939 1970-01-01 00:00:00.000000 halig-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    34670 2023-06-19 16:50:30.000000 halig-0.4.5/LICENSE
+-rw-r--r--   0        0        0     1635 2023-06-19 16:50:30.000000 halig-0.4.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-19 16:50:47.000000 halig-0.4.5/halig/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-17 16:49:03.845916 halig-0.4.5/halig/__version__.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:50:47.000000 halig-0.4.5/halig/commands/__init__.py
+-rw-r--r--   0        0        0      377 2024-05-17 16:46:42.834123 halig-0.4.5/halig/commands/base.py
+-rw-r--r--   0        0        0     2781 2023-06-19 16:50:47.000000 halig-0.4.5/halig/commands/edit.py
+-rw-r--r--   0        0        0     1397 2023-06-19 16:50:47.000000 halig-0.4.5/halig/commands/import_unencrypted.py
+-rw-r--r--   0        0        0     1297 2024-05-17 16:43:49.431109 halig-0.4.5/halig/commands/notebooks.py
+-rw-r--r--   0        0        0      958 2024-05-17 16:13:02.174437 halig-0.4.5/halig/commands/reencrypt.py
+-rw-r--r--   0        0        0     3780 2024-05-17 16:13:02.174437 halig-0.4.5/halig/commands/search.py
+-rw-r--r--   0        0        0     1368 2024-05-17 16:13:02.174437 halig-0.4.5/halig/commands/show.py
+-rw-r--r--   0        0        0     1468 2023-07-24 17:49:45.000000 halig-0.4.5/halig/encryption.py
+-rw-r--r--   0        0        0     2335 2024-05-17 16:19:18.497079 halig-0.4.5/halig/literals.py
+-rw-r--r--   0        0        0     4553 2024-05-17 16:43:49.462108 halig-0.4.5/halig/main.py
+-rw-r--r--   0        0        0     4341 2024-05-17 16:13:02.174437 halig-0.4.5/halig/settings.py
+-rw-r--r--   0        0        0      769 2024-05-17 16:45:16.297105 halig-0.4.5/halig/utils.py
+-rw-r--r--   0        0        0     2820 2024-05-17 16:50:00.466636 halig-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-19 16:50:47.000000 halig-0.4.5/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:50:47.000000 halig-0.4.5/tests/commands/__init__.py
+-rw-r--r--   0        0        0     2262 2024-05-17 16:13:02.175437 halig-0.4.5/tests/commands/conftest.py
+-rw-r--r--   0        0        0     1177 2024-05-17 16:13:02.175437 halig-0.4.5/tests/commands/test_edit.py
+-rw-r--r--   0        0        0     1476 2024-05-17 16:13:02.175437 halig-0.4.5/tests/commands/test_import.py
+-rw-r--r--   0        0        0     1594 2024-05-17 16:23:06.988114 halig-0.4.5/tests/commands/test_notebooks.py
+-rw-r--r--   0        0        0      757 2024-05-17 16:41:33.618275 halig-0.4.5/tests/commands/test_reencrypt.py
+-rw-r--r--   0        0        0     1150 2024-05-17 16:13:02.175437 halig-0.4.5/tests/commands/test_show.py
+-rw-r--r--   0        0        0     3003 2024-05-17 16:26:46.465392 halig-0.4.5/tests/conftest.py
+-rw-r--r--   0        0        0     2318 2024-05-17 16:13:02.175437 halig-0.4.5/tests/test_encryption.py
+-rw-r--r--   0        0        0     1121 2024-05-17 16:13:02.175437 halig-0.4.5/tests/test_settings.py
+-rw-r--r--   0        0        0     1516 2024-05-17 16:13:02.175437 halig-0.4.5/tests/test_utils.py
+-rw-r--r--   0        0        0     3954 1970-01-01 00:00:00.000000 halig-0.4.5/PKG-INFO
```

### Comparing `halig-0.4.4/LICENSE` & `halig-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `halig-0.4.4/README.md` & `halig-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `halig-0.4.4/halig/commands/edit.py` & `halig-0.4.5/halig/commands/edit.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.4/halig/commands/import_unencrypted.py` & `halig-0.4.5/halig/commands/import_unencrypted.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.4/halig/commands/reencrypt.py` & `halig-0.4.5/halig/commands/reencrypt.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.4/halig/commands/search.py` & `halig-0.4.5/halig/commands/search.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.4/halig/commands/show.py` & `halig-0.4.5/halig/commands/show.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.4/halig/encryption.py` & `halig-0.4.5/halig/encryption.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.4/halig/literals.py` & `halig-0.4.5/halig/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 only the newly encrypted .age files will be preserved. Backup your data first
 """
 OPTION_INDEX_HELP = """Index the SQLite database with your notes contents. The first
 time you perform a search, this flag should be set. Afterwards, you should only index
 when new notes have been added or older ones have been changed, since it's a slow
 operation"""
 OPTION_PLAIN_HELP = "Show the note as plaintext"
+OPTION_INCLUDE_NODES_HELP = "Include each notebook's notes when listing"
 # ARGUMENTS
 ARGUMENT_EDIT_NOTE_HELP = """A valid, settings-relative path.
 Be aware that valid can also mean implicit notes, that is, pointing to a
 current-day note just by its notebook name. For example, if today is
 2023-04-04 and you have a notebook containing a 2023-04-04.age note,
 simply pointing to the notebook's name, e.g. `halig edit notebook` will
 edit the 2023-04-04.age note. Also keep in mind that the note may or may
```

### Comparing `halig-0.4.4/halig/main.py` & `halig-0.4.5/halig/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,20 +48,25 @@
 def notebooks(
     level: int = Option(  # B008
         -1,
         "--level",
         "-l",
         help=literals.OPTION_LEVEL_HELP,
     ),
+    include_notes: bool = Option(False, help=literals.OPTION_INCLUDE_NODES_HELP),
     config: Optional[Path] = config_option,  # noqa: UP007
 ):
     if level < 0:
         level = float("inf")  # type: ignore[assignment]
     settings = load_from_file(config)
-    command = NotebooksCommand(settings=settings, max_depth=level)
+    command = NotebooksCommand(
+        settings=settings,
+        max_depth=level,
+        include_notes=include_notes,
+    )
     command.run()
 
 
 @app.command(help=literals.COMMANDS_EDIT_HELP)
 @capture
 def edit(
     note: Path = Argument(  # noqa: B008
```

### Comparing `halig-0.4.4/halig/settings.py` & `halig-0.4.5/halig/settings.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.4/halig/utils.py` & `halig-0.4.5/halig/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 import pendulum
 from pendulum.tz import local_timezone
 from rich import print
 
 
 def now():
     tz = local_timezone()
-    return pendulum.now(tz)
+    return pendulum.now(tz)  # type: ignore[reportArgumentType]
 
 
 def capture(fn: Callable):
     @wraps(fn)
     def wrapper(*args, **kwargs):
         try:
             return fn(*args, **kwargs)
         except OSError as exc:
             print(f"[red]{exc.strerror} on {exc.filename or exc.filename2}")
             sys.exit(exc.errno)
         except ValueError as exc:
             print(f"[red]{exc}")
             sys.exit(1)
         except Exception as exc:  # noqa: BLE001
-            print(f"[beld red] Unexpected error: {exc}")
+            print(f"[bold red] Unexpected error: {exc}")
             sys.exit(2)
 
     return wrapper
```

### Comparing `halig-0.4.4/pyproject.toml` & `halig-0.4.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Terminals",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
-version = "0.4.4"
+version = "0.4.5"
 
 [project.license]
 text = "GPL-3.0-or-later"
 
 [project.urls]
 Homepage = "https://git.roboces.dev/catalin/halig"
 Repository = "https://git.roboces.dev/catalin/halig"
@@ -92,16 +92,17 @@
 
 [tool.pytest]
 mock_use_standalone_module = true
 
 [tool.pyright]
 reportMissingImports = false
 reportMissingTypeStubs = false
+reportAttributeAccessIssue = false
 
-[tool.ruff]
+[tool.ruff.lint]
 extend-select = [
     "W",
     "C90",
     "I",
     "N",
     "UP",
     "S",
```

### Comparing `halig-0.4.4/tests/commands/conftest.py` & `halig-0.4.5/tests/commands/conftest.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.4/tests/commands/test_edit.py` & `halig-0.4.5/tests/commands/test_edit.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.4/tests/commands/test_import.py` & `halig-0.4.5/tests/commands/test_import.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.4/tests/commands/test_notebooks.py` & `halig-0.4.5/tests/commands/test_notebooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,20 +21,22 @@
 def test_build_tree_max_depth_2(notes, notebooks_command: NotebooksCommand):
     notebooks_command.max_depth = 2
     tree = notebooks_command.build_tree(notebooks_command.settings.notebooks_root_path)
     personal = tree.children[0]
     work = tree.children[1]
     assert personal.label == "Personal"
     assert work.label == "Work"
-    assert len(work.children) == 2
-    assert len(personal.children) == 1
+    assert len(work.children) == 1
+    assert len(personal.children) == 0
 
 
-def test_build_tree_max_depth_inf(notes, notebooks_command: NotebooksCommand):
-    tree = notebooks_command.build_tree(notebooks_command.settings.notebooks_root_path)
+def test_build_tree_max_depth_inf(notes, settings):
+    tree = NotebooksCommand(max_depth=float("inf"), settings=settings, include_notes=True).build_tree(
+        settings.notebooks_root_path
+    )
     personal = tree.children[0]
     work = tree.children[1]
     assert personal.label == "Personal"
     assert work.label == "Work"
     assert len(work.children) == 2
     assert len(personal.children) == 1
```

### Comparing `halig-0.4.4/tests/commands/test_show.py` & `halig-0.4.5/tests/commands/test_show.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.4/tests/conftest.py` & `halig-0.4.5/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,30 +37,14 @@
 
 
 @pytest.fixture()
 def ssh_recipient(halig_ssh_public_key: str) -> Recipient:
     return Recipient.from_str(halig_ssh_public_key)
 
 
-# @pytest.fixture()
-# def halig_path(fs, halig_ssh_public_key, halig_ssh_private_key) -> Path:
-#    fs.add_real_paths(["/etc/localtime"])
-#    ssh_path = Path("~/.ssh").expanduser()
-#    ssh_path.mkdir(parents=True)
-#
-#    with (ssh_path / "id_ed25519").open("w") as f:
-#        f.write(halig_ssh_private_key)
-#
-#    with (ssh_path / "id_ed25519.pub").open("w") as f:
-#        f.write(halig_ssh_public_key)
-#
-#    halig_path = Path("~/.config/halig").expanduser()
-#    halig_path.mkdir(parents=True)
-#    return halig_path
-
 @pytest.fixture()
 def halig_ssh_path(tmp_path: Path, halig_ssh_public_key, halig_ssh_private_key) -> Path:
     ssh_path = tmp_path / ".ssh"
     ssh_path.mkdir()
 
     with (ssh_path / "id_ed25519").open("w") as f:
         f.write(halig_ssh_private_key)
```

### Comparing `halig-0.4.4/tests/test_encryption.py` & `halig-0.4.5/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.4/tests/test_settings.py` & `halig-0.4.5/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.4/tests/test_utils.py` & `halig-0.4.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.4/PKG-INFO` & `halig-0.4.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: halig
-Version: 0.4.4
+Version: 0.4.5
 Summary: age-encrypted, file-based, note-taking CLI app
-Keywords: cli notes age rage encryption notebook
-Author-Email: cătălin <185504a9@duck.com>
+Keywords: cli,notes,age,rage,encryption,notebook
+Author-Email: =?utf-8?b?Y8SDdMSDbGlu?= <185504a9@duck.com>
 License: GPL-3.0-or-later
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

