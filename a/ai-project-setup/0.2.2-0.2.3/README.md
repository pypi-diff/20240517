# Comparing `tmp/ai_project_setup-0.2.2.tar.gz` & `tmp/ai_project_setup-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_project_setup-0.2.2.tar", last modified: Fri May 17 01:26:13 2024, max compression
+gzip compressed data, was "ai_project_setup-0.2.3.tar", last modified: Fri May 17 01:56:23 2024, max compression
```

## Comparing `ai_project_setup-0.2.2.tar` & `ai_project_setup-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:26:13.394535 ai_project_setup-0.2.2/
--rw-r--r--   0 root         (0) root         (0)     1544 2024-05-17 01:26:13.394535 ai_project_setup-0.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3159 2024-05-17 01:19:44.000000 ai_project_setup-0.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:26:13.393535 ai_project_setup-0.2.2/ai_project_setup.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1544 2024-05-17 01:26:13.000000 ai_project_setup-0.2.2/ai_project_setup.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      280 2024-05-17 01:26:13.000000 ai_project_setup-0.2.2/ai_project_setup.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 01:26:13.000000 ai_project_setup-0.2.2/ai_project_setup.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-05-17 01:26:13.000000 ai_project_setup-0.2.2/ai_project_setup.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:26:13.393535 ai_project_setup-0.2.2/git_clone/
--rw-r--r--   0 root         (0) root         (0)       33 2024-05-17 00:52:56.000000 ai_project_setup-0.2.2/git_clone/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9249 2024-05-17 00:53:07.000000 ai_project_setup-0.2.2/git_clone/git_clone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:26:13.394535 ai_project_setup-0.2.2/project_setup/
--rw-r--r--   0 root         (0) root         (0)       41 2024-05-17 00:50:04.000000 ai_project_setup-0.2.2/project_setup/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5173 2024-05-17 00:50:04.000000 ai_project_setup-0.2.2/project_setup/project_setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 01:26:13.394535 ai_project_setup-0.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1880 2024-05-17 01:26:07.000000 ai_project_setup-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:56:23.729150 ai_project_setup-0.2.3/
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-05-17 01:56:23.728150 ai_project_setup-0.2.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3159 2024-05-17 01:19:44.000000 ai_project_setup-0.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:56:23.727150 ai_project_setup-0.2.3/ai_project_setup.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-05-17 01:56:23.000000 ai_project_setup-0.2.3/ai_project_setup.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      280 2024-05-17 01:56:23.000000 ai_project_setup-0.2.3/ai_project_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 01:56:23.000000 ai_project_setup-0.2.3/ai_project_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-17 01:56:23.000000 ai_project_setup-0.2.3/ai_project_setup.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:56:23.727150 ai_project_setup-0.2.3/git_clone/
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-17 00:52:56.000000 ai_project_setup-0.2.3/git_clone/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9257 2024-05-17 01:55:53.000000 ai_project_setup-0.2.3/git_clone/git_clone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:56:23.728150 ai_project_setup-0.2.3/project_setup/
+-rw-r--r--   0 root         (0) root         (0)       41 2024-05-17 00:50:04.000000 ai_project_setup-0.2.3/project_setup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5173 2024-05-17 00:50:04.000000 ai_project_setup-0.2.3/project_setup/project_setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 01:56:23.729150 ai_project_setup-0.2.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-05-17 01:56:16.000000 ai_project_setup-0.2.3/setup.py
```

### Comparing `ai_project_setup-0.2.2/PKG-INFO` & `ai_project_setup-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai_project_setup
-Version: 0.2.2
+Version: 0.2.3
 Summary: A versatile utility package designed to streamline the setup of AI project structures while seamlessly integrating with Git repositories and Google Colab, simplifying the process of building collaborative AI projects.
 Author: Patrick Ogbuitepu
 Author-email: pat2echo@gmail.com
 Keywords: AI,utility package,project structure,Git integration,Google Colab integration,collaborative projects,ease of use,streamlined workflow,automation,project management,project,setup,structure,ai,artificial intelligence,research,data science,machine learning
 Description-Content-Type: text/markdown
 
 # AI Project Starter Pack
```

### Comparing `ai_project_setup-0.2.2/README.md` & `ai_project_setup-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ai_project_setup-0.2.2/ai_project_setup.egg-info/PKG-INFO` & `ai_project_setup-0.2.3/ai_project_setup.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-project-setup
-Version: 0.2.2
+Version: 0.2.3
 Summary: A versatile utility package designed to streamline the setup of AI project structures while seamlessly integrating with Git repositories and Google Colab, simplifying the process of building collaborative AI projects.
 Author: Patrick Ogbuitepu
 Author-email: pat2echo@gmail.com
 Keywords: AI,utility package,project structure,Git integration,Google Colab integration,collaborative projects,ease of use,streamlined workflow,automation,project management,project,setup,structure,ai,artificial intelligence,research,data science,machine learning
 Description-Content-Type: text/markdown
 
 # AI Project Starter Pack
```

### Comparing `ai_project_setup-0.2.2/git_clone/git_clone.py` & `ai_project_setup-0.2.3/git_clone/git_clone.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,29 +169,29 @@
       Returns:
         none: Returns Nothing
       """
       error = ''
       user_dir = base_dir
       if url.startswith("http") and url.endswith(".git"):
         if os.path.exists(user_dir):
-            %cd {user_dir}
+            os.chdir(user_dir)
             git_dir = os.path.join(user_dir,dir)
             if os.path.exists(git_dir):
               print(f"\033[91mIMPORTANT! Directory {git_dir} already exists\033[0m")
               confirm = input(f"The directory {git_dir} already exists.\nAre you sure you want to delete the directory '{git_dir}' and all its contents and re-clone it? (yes/no): ")
               if confirm.lower() == 'yes':
                   shutil.rmtree(git_dir)
               else:
                   error = f"User aborted the Clone Operation because the directory exists"
               
             if error == '':
               !git clone {url}
             
             if os.path.exists(git_dir):
-              %cd {dir}
+              os.chdir(dir)
               print('List files: ', os.listdir())
             else:
               error = f"Failed to Clone Repo: Directory {git_dir} does not exists"
               self.no_error = False
         else:
             error = f"Directory {user_dir} does not exists"
             self.no_error = False
```

### Comparing `ai_project_setup-0.2.2/project_setup/project_setup.py` & `ai_project_setup-0.2.3/project_setup/project_setup.py`

 * *Files identical despite different names*

### Comparing `ai_project_setup-0.2.2/setup.py` & `ai_project_setup-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ai_project_setup',
-    version='0.2.2',
+    version='0.2.3',
     packages=find_packages(),
     description='A versatile utility package designed to streamline the setup of AI project structures while seamlessly integrating with Git repositories and Google Colab, simplifying the process of building collaborative AI projects.',
     long_description="""# AI Project Starter Pack
 The AI Project Starter Pack is a meticulously structured directory and module framework designed for creating machine learning and data science projects. This starter pack aims to streamline the project setup process, helping data scientists and developers organize their code, data, and documentation efficiently. 
 
 ## GITHUB: https://github.com/pat2echo/AI-Project-Starter-Pack/
```

