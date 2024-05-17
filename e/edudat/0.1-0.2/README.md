# Comparing `tmp/edudat-0.1.tar.gz` & `tmp/edudat-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edudat-0.1.tar", last modified: Fri May 17 12:00:25 2024, max compression
+gzip compressed data, was "edudat-0.2.tar", last modified: Fri May 17 12:31:08 2024, max compression
```

## Comparing `edudat-0.1.tar` & `edudat-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 oli        (503) staff       (20)        0 2024-05-17 12:00:25.634972 edudat-0.1/
--rw-r--r--   0 oli        (503) staff       (20)      307 2024-05-17 12:00:25.634839 edudat-0.1/PKG-INFO
-drwxr-xr-x   0 oli        (503) staff       (20)        0 2024-05-17 12:00:25.629948 edudat-0.1/edudat/
--rw-r--r--   0 oli        (503) staff       (20)       59 2024-05-17 09:26:15.000000 edudat-0.1/edudat/__init__.py
--rw-r--r--   0 oli        (503) staff       (20)      564 2024-05-17 08:50:11.000000 edudat-0.1/edudat/data_loader.py
-drwxr-xr-x   0 oli        (503) staff       (20)        0 2024-05-17 12:00:25.634663 edudat-0.1/edudat.egg-info/
--rw-r--r--   0 oli        (503) staff       (20)      307 2024-05-17 12:00:25.000000 edudat-0.1/edudat.egg-info/PKG-INFO
--rw-r--r--   0 oli        (503) staff       (20)      198 2024-05-17 12:00:25.000000 edudat-0.1/edudat.egg-info/SOURCES.txt
--rw-r--r--   0 oli        (503) staff       (20)        1 2024-05-17 12:00:25.000000 edudat-0.1/edudat.egg-info/dependency_links.txt
--rw-r--r--   0 oli        (503) staff       (20)       16 2024-05-17 12:00:25.000000 edudat-0.1/edudat.egg-info/requires.txt
--rw-r--r--   0 oli        (503) staff       (20)        7 2024-05-17 12:00:25.000000 edudat-0.1/edudat.egg-info/top_level.txt
--rw-r--r--   0 oli        (503) staff       (20)       38 2024-05-17 12:00:25.635017 edudat-0.1/setup.cfg
--rw-r--r--   0 oli        (503) staff       (20)      484 2024-05-17 11:57:15.000000 edudat-0.1/setup.py
+drwxr-xr-x   0 oli        (503) staff       (20)        0 2024-05-17 12:31:08.446896 edudat-0.2/
+-rw-r--r--   0 oli        (503) staff       (20)      307 2024-05-17 12:31:08.446783 edudat-0.2/PKG-INFO
+drwxr-xr-x   0 oli        (503) staff       (20)        0 2024-05-17 12:31:08.445906 edudat-0.2/edudat/
+-rw-r--r--   0 oli        (503) staff       (20)       59 2024-05-17 09:26:15.000000 edudat-0.2/edudat/__init__.py
+-rw-r--r--   0 oli        (503) staff       (20)      570 2024-05-17 12:18:50.000000 edudat-0.2/edudat/data_loader.py
+drwxr-xr-x   0 oli        (503) staff       (20)        0 2024-05-17 12:31:08.446625 edudat-0.2/edudat.egg-info/
+-rw-r--r--   0 oli        (503) staff       (20)      307 2024-05-17 12:31:08.000000 edudat-0.2/edudat.egg-info/PKG-INFO
+-rw-r--r--   0 oli        (503) staff       (20)      198 2024-05-17 12:31:08.000000 edudat-0.2/edudat.egg-info/SOURCES.txt
+-rw-r--r--   0 oli        (503) staff       (20)        1 2024-05-17 12:31:08.000000 edudat-0.2/edudat.egg-info/dependency_links.txt
+-rw-r--r--   0 oli        (503) staff       (20)       16 2024-05-17 12:31:08.000000 edudat-0.2/edudat.egg-info/requires.txt
+-rw-r--r--   0 oli        (503) staff       (20)        7 2024-05-17 12:31:08.000000 edudat-0.2/edudat.egg-info/top_level.txt
+-rw-r--r--   0 oli        (503) staff       (20)       38 2024-05-17 12:31:08.446943 edudat-0.2/setup.cfg
+-rw-r--r--   0 oli        (503) staff       (20)      484 2024-05-17 12:29:48.000000 edudat-0.2/setup.py
```

### Comparing `edudat-0.1/edudat/data_loader.py` & `edudat-0.2/edudat/data_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 def load_data(name):
     data_dir = os.path.join(os.path.expanduser("~"), ".edudat_cache")
     if not os.path.exists(data_dir):
         os.makedirs(data_dir)
     
     file_path = os.path.join(data_dir, name)
     if not os.path.exists(file_path):
-        url = f"https://raw.githubusercontent.com/oduerr/data/main/data/{name}"
+        url = f"https://raw.githubusercontent.com/tensorchiefs/data/main/data/{name}"
         response = requests.get(url)
         response.raise_for_status()
         with open(file_path, 'wb') as f:
             f.write(response.content)
     
     return pd.read_csv(file_path)
```

