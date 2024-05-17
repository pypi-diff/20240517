# Comparing `tmp/ai_project_setup-0.2.3.tar.gz` & `tmp/ai_project_setup-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_project_setup-0.2.3.tar", last modified: Fri May 17 01:56:23 2024, max compression
+gzip compressed data, was "ai_project_setup-0.2.5.tar", last modified: Fri May 17 02:06:27 2024, max compression
```

## Comparing `ai_project_setup-0.2.3.tar` & `ai_project_setup-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:56:23.729150 ai_project_setup-0.2.3/
--rw-r--r--   0 root         (0) root         (0)     1544 2024-05-17 01:56:23.728150 ai_project_setup-0.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3159 2024-05-17 01:19:44.000000 ai_project_setup-0.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:56:23.727150 ai_project_setup-0.2.3/ai_project_setup.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1544 2024-05-17 01:56:23.000000 ai_project_setup-0.2.3/ai_project_setup.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      280 2024-05-17 01:56:23.000000 ai_project_setup-0.2.3/ai_project_setup.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 01:56:23.000000 ai_project_setup-0.2.3/ai_project_setup.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-05-17 01:56:23.000000 ai_project_setup-0.2.3/ai_project_setup.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:56:23.727150 ai_project_setup-0.2.3/git_clone/
--rw-r--r--   0 root         (0) root         (0)       33 2024-05-17 00:52:56.000000 ai_project_setup-0.2.3/git_clone/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9257 2024-05-17 01:55:53.000000 ai_project_setup-0.2.3/git_clone/git_clone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:56:23.728150 ai_project_setup-0.2.3/project_setup/
--rw-r--r--   0 root         (0) root         (0)       41 2024-05-17 00:50:04.000000 ai_project_setup-0.2.3/project_setup/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5173 2024-05-17 00:50:04.000000 ai_project_setup-0.2.3/project_setup/project_setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 01:56:23.729150 ai_project_setup-0.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1880 2024-05-17 01:56:16.000000 ai_project_setup-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:06:27.369708 ai_project_setup-0.2.5/
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-05-17 02:06:27.368708 ai_project_setup-0.2.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3159 2024-05-17 01:19:44.000000 ai_project_setup-0.2.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:06:27.368708 ai_project_setup-0.2.5/ai_project_setup.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-05-17 02:06:27.000000 ai_project_setup-0.2.5/ai_project_setup.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      280 2024-05-17 02:06:27.000000 ai_project_setup-0.2.5/ai_project_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 02:06:27.000000 ai_project_setup-0.2.5/ai_project_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-17 02:06:27.000000 ai_project_setup-0.2.5/ai_project_setup.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:06:27.368708 ai_project_setup-0.2.5/git_clone/
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-17 00:52:56.000000 ai_project_setup-0.2.5/git_clone/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9957 2024-05-17 02:05:39.000000 ai_project_setup-0.2.5/git_clone/git_clone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:06:27.368708 ai_project_setup-0.2.5/project_setup/
+-rw-r--r--   0 root         (0) root         (0)       41 2024-05-17 00:50:04.000000 ai_project_setup-0.2.5/project_setup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5173 2024-05-17 00:50:04.000000 ai_project_setup-0.2.5/project_setup/project_setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 02:06:27.369708 ai_project_setup-0.2.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-05-17 02:06:22.000000 ai_project_setup-0.2.5/setup.py
```

### Comparing `ai_project_setup-0.2.3/PKG-INFO` & `ai_project_setup-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai_project_setup
-Version: 0.2.3
+Version: 0.2.5
 Summary: A versatile utility package designed to streamline the setup of AI project structures while seamlessly integrating with Git repositories and Google Colab, simplifying the process of building collaborative AI projects.
 Author: Patrick Ogbuitepu
 Author-email: pat2echo@gmail.com
 Keywords: AI,utility package,project structure,Git integration,Google Colab integration,collaborative projects,ease of use,streamlined workflow,automation,project management,project,setup,structure,ai,artificial intelligence,research,data science,machine learning
 Description-Content-Type: text/markdown
 
 # AI Project Starter Pack
```

### Comparing `ai_project_setup-0.2.3/README.md` & `ai_project_setup-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ai_project_setup-0.2.3/ai_project_setup.egg-info/PKG-INFO` & `ai_project_setup-0.2.5/ai_project_setup.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-project-setup
-Version: 0.2.3
+Version: 0.2.5
 Summary: A versatile utility package designed to streamline the setup of AI project structures while seamlessly integrating with Git repositories and Google Colab, simplifying the process of building collaborative AI projects.
 Author: Patrick Ogbuitepu
 Author-email: pat2echo@gmail.com
 Keywords: AI,utility package,project structure,Git integration,Google Colab integration,collaborative projects,ease of use,streamlined workflow,automation,project management,project,setup,structure,ai,artificial intelligence,research,data science,machine learning
 Description-Content-Type: text/markdown
 
 # AI Project Starter Pack
```

### Comparing `ai_project_setup-0.2.3/git_clone/git_clone.py` & `ai_project_setup-0.2.5/git_clone/git_clone.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import shutil
 from datetime import datetime
 import re
+import subprocess
 
 try:
   from google.colab import userdata
   from google.colab import drive
 except Exception as e:
       print("You are not using Google Colab. You must specify values for\n1. GIT_USER (leave blank if using github)\n2. GIT_ACCESS_TOKEN\n3. GIT_REPO_URL")
 
@@ -180,15 +181,16 @@
               confirm = input(f"The directory {git_dir} already exists.\nAre you sure you want to delete the directory '{git_dir}' and all its contents and re-clone it? (yes/no): ")
               if confirm.lower() == 'yes':
                   shutil.rmtree(git_dir)
               else:
                   error = f"User aborted the Clone Operation because the directory exists"
               
             if error == '':
-              !git clone {url}
+              #!git clone {url}
+              subprocess.run(["git", "clone", url])
             
             if os.path.exists(git_dir):
               os.chdir(dir)
               print('List files: ', os.listdir())
             else:
               error = f"Failed to Clone Repo: Directory {git_dir} does not exists"
               self.no_error = False
@@ -203,29 +205,33 @@
     
     def get_git_branch_name(self):
       """Run the git branch command and capture the output
       
       Returns:
         str: Name of current git branch
       """
-      branch_name = ''
       error = ''
-      try:
-          branch_output = !git branch
-          # Find the line with an asterisk (*) indicating the current branch
-          for line in branch_output:
-              if line.startswith('*'):
-                  # Extract the branch name (remove the asterisk)
-                  branch_name = line[1:].strip()
-                  # Regular expression pattern for ANSI escape codes
-                  ansi_escape = re.compile(r'\x1B\[[0-?]*[ -/]*[@-~]')
-                  branch_name = ansi_escape.sub('', branch_name)
+      branch_name = subprocess.check_output(['git', 'rev-parse', '--abbrev-ref', 'HEAD']).decode().strip()
+      ansi_escape = re.compile(r'\x1B\[[0-?]*[ -/]*[@-~]')
+      branch_name = ansi_escape.sub('', branch_name)
+
+      # branch_name = ''
+      # try:
+      #     branch_output = !git branch
+      #     # Find the line with an asterisk (*) indicating the current branch
+      #     for line in branch_output:
+      #         if line.startswith('*'):
+      #             # Extract the branch name (remove the asterisk)
+      #             branch_name = line[1:].strip()
+      #             # Regular expression pattern for ANSI escape codes
+      #             ansi_escape = re.compile(r'\x1B\[[0-?]*[ -/]*[@-~]')
+      #             branch_name = ansi_escape.sub('', branch_name)
 
-      except Exception as e:
-          error = f"Error: Unable to get Git branch: {e}"
+      # except Exception as e:
+      #     error = f"Error: Unable to get Git branch: {e}"
 
       if error: 
         print(error)
         self.no_error = False
 
       return branch_name
 
@@ -234,19 +240,26 @@
 
       Parameters:
         commit_message (str): Describe the changes that you have made
 
       Returns:
         none: Returns Nothing
       """
-      !git config --global user.email {self.user_email}
-      !git config --global user.name {self.user_email}
+      #!git config --global user.email {self.user_email}
+      subprocess.run(["git", "config", "--global", "user.email", self.user_email])
+
+      #!git config --global user.name {self.user_email}
+      subprocess.run(["git", "config", "--global", "user.name", self.user_name])
+
       #!git config --global user.name {self.user_name}
       !git add . 
-      commitMsg = input("Enter your commit message that describes the changes that you have made to the files: ")
-      if commitMsg == '':
-        commitMsg = f'Commit at {datetime.now()}'
-      !git commit -m "{commitMsg}"
-      !git remote set-url origin {self.url}
-      !git push origin {self.branch_name}
+      commit_msg = input("Enter your commit message that describes the changes that you have made to the files: ")
+      if commit_msg == '':
+        commit_msg = f'Commit at {datetime.now()}'
+      #!git commit -m "{commit_msg}"
+      subprocess.run(["git", "commit", "-m", commit_msg])
+      #!git remote set-url origin {self.url}
+      subprocess.run(["git", "remote", "set-url", "origin", self.url])
+      #!git push origin {self.branch_name}
+      subprocess.run(["git", "push", "origin", self.branch_name])
```

### Comparing `ai_project_setup-0.2.3/project_setup/project_setup.py` & `ai_project_setup-0.2.5/project_setup/project_setup.py`

 * *Files identical despite different names*

### Comparing `ai_project_setup-0.2.3/setup.py` & `ai_project_setup-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ai_project_setup',
-    version='0.2.3',
+    version='0.2.5',
     packages=find_packages(),
     description='A versatile utility package designed to streamline the setup of AI project structures while seamlessly integrating with Git repositories and Google Colab, simplifying the process of building collaborative AI projects.',
     long_description="""# AI Project Starter Pack
 The AI Project Starter Pack is a meticulously structured directory and module framework designed for creating machine learning and data science projects. This starter pack aims to streamline the project setup process, helping data scientists and developers organize their code, data, and documentation efficiently. 
 
 ## GITHUB: https://github.com/pat2echo/AI-Project-Starter-Pack/
```

