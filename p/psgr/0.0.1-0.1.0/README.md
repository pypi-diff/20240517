# Comparing `tmp/psgr-0.0.1.tar.gz` & `tmp/psgr-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psgr-0.0.1.tar", last modified: Sun Apr 28 13:47:15 2024, max compression
+gzip compressed data, was "psgr-0.1.0.tar", last modified: Fri May 17 15:02:36 2024, max compression
```

## Comparing `psgr-0.0.1.tar` & `psgr-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-04-28 13:47:15.470971 psgr-0.0.1/
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      161 2024-04-28 13:47:15.470971 psgr-0.0.1/PKG-INFO
-drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-04-28 13:47:15.470971 psgr-0.0.1/psgr/
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       19 2024-04-28 12:52:49.000000 psgr-0.0.1/psgr/__init__.py
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)     7515 2024-04-28 13:28:58.000000 psgr-0.0.1/psgr/main.py
-drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-04-28 13:47:15.470971 psgr-0.0.1/psgr.egg-info/
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      161 2024-04-28 13:47:15.000000 psgr-0.0.1/psgr.egg-info/PKG-INFO
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      208 2024-04-28 13:47:15.000000 psgr-0.0.1/psgr.egg-info/SOURCES.txt
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        1 2024-04-28 13:47:15.000000 psgr-0.0.1/psgr.egg-info/dependency_links.txt
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       46 2024-04-28 13:47:15.000000 psgr-0.0.1/psgr.egg-info/entry_points.txt
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       13 2024-04-28 13:47:15.000000 psgr-0.0.1/psgr.egg-info/requires.txt
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        5 2024-04-28 13:47:15.000000 psgr-0.0.1/psgr.egg-info/top_level.txt
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       38 2024-04-28 13:47:15.470971 psgr-0.0.1/setup.cfg
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      431 2024-04-28 13:46:13.000000 psgr-0.0.1/setup.py
+drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-17 15:02:36.033760 psgr-0.1.0/
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      161 2024-05-17 15:02:36.033760 psgr-0.1.0/PKG-INFO
+drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-17 15:02:36.033760 psgr-0.1.0/psgr/
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       19 2024-04-28 12:52:49.000000 psgr-0.1.0/psgr/__init__.py
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)     8511 2024-05-17 14:48:07.000000 psgr-0.1.0/psgr/main.py
+drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-17 15:02:36.033760 psgr-0.1.0/psgr.egg-info/
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      161 2024-05-17 15:02:36.000000 psgr-0.1.0/psgr.egg-info/PKG-INFO
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      208 2024-05-17 15:02:36.000000 psgr-0.1.0/psgr.egg-info/SOURCES.txt
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        1 2024-05-17 15:02:36.000000 psgr-0.1.0/psgr.egg-info/dependency_links.txt
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       46 2024-05-17 15:02:36.000000 psgr-0.1.0/psgr.egg-info/entry_points.txt
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       13 2024-05-17 15:02:36.000000 psgr-0.1.0/psgr.egg-info/requires.txt
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        5 2024-05-17 15:02:36.000000 psgr-0.1.0/psgr.egg-info/top_level.txt
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       38 2024-05-17 15:02:36.033760 psgr-0.1.0/setup.cfg
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      431 2024-05-17 15:01:34.000000 psgr-0.1.0/setup.py
```

### Comparing `psgr-0.0.1/psgr/main.py` & `psgr-0.1.0/psgr/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,21 @@
 import time
 import base64
 import os.path
 import getpass
 from tabulate import tabulate
 import json
 import rsa
+from InquirerPy import inquirer
+import signal
+
+
 
 def main():
+
     def generateKeys():
         (pubkey, privkey) = rsa.newkeys(512)
         keyData = {
             "public_key": pubkey.save_pkcs1().decode(),
             "private_key": privkey.save_pkcs1().decode()
         }
 
@@ -123,35 +128,51 @@
         
         if name == "all":
             # pprint.pprint(showAccounts)
             table_data = [(key, value) for key, value in showAccounts.items()]
             table = tabulate(table_data, headers=["Account", "Password"], tablefmt="github")
             print(table)
             print(" ")
+        elif name == "accounts":
+            print("Accounts: ")
+            for key, _ in showAccounts.items():
+                print(key)
+            print(" ")
 
         else:
             if not name:
-                accountName = input("Enter Account: ")
+                chooseIt = []
+                for k, v in accounts.items():
+                    chooseIt.append(k)
+                accountName = inquirer.select(
+                    message = "Choose the account:",
+                    choices = chooseIt
+                ).execute()
             else:
                 accountName = name
 
             if accountName not in showAccounts:
                 message = input("Account not found. Add a new account with that name? [Y]/[N]? ")
                 if message.upper() == "Y":
                     add(name)
                 return
             else:
                 table_data = [(accountName, showAccounts[accountName])]
                 table = tabulate(table_data, headers=["Account", "Password"], tablefmt="github")
                 print(table)
                 print(" ")
 
+        def ignore_ctrl_c(signum, frame):
+            print("Ctrl+C is disabled.", end="\r")
+        original_handler = signal.getsignal(signal.SIGINT)
+        signal.signal(signal.SIGINT, ignore_ctrl_c)
         for i in range(5, 0, -1):
             print(f"clearing screen in {i} seconds.", end="\r")
             time.sleep(1)
+        signal.signal(signal.SIGINT, original_handler)
         if os.name == 'nt':
             _ = os.system('cls')
         # For UNIX-like systems (Linux, macOS)
         else:
             _ = os.system('clear')
         return
 
@@ -181,22 +202,32 @@
         - Passwords are encrypted at all times.
         - Passwords will disappear from the screen after 5 seconds.
     """
         print(help_message)
         return
 
     def remove(alll=""):
-        message = input("This process is irreversible. Continue? [Y]/[N]: ")
+        message = inquirer.select(
+                    message = "Choose Account:",
+                    choices = ['Y', 'N']
+                ).execute()
         if message.upper() == "Y":
             if alll == "all":
                 with open("accountinfo.json", 'w') as json_file:
                     # Write an empty JSON object to the file
                     json.dump({}, json_file)
-            if not all:
-                alll = input("Enter Account Name: ")
+            else:
+                chooseIt = []
+                for k, v in accounts.items():
+                    chooseIt.append(k)
+                alll = inquirer.select(
+                    message = "Choose Account:",
+                    choices = chooseIt
+                ).execute()
+
             if alll in accounts:
                 accounts.pop(alll)
                 with open("accountinfo.json", "w") as f:
                     json.dump(accounts, f)            
         return
 
 
@@ -218,8 +249,11 @@
         print("No use for the command {", sys.argv[1], "} found. Try using appname.py help.")
 
     if n == 2:
         assign_task(sys.argv[1])
     elif n == 3:
         assign_task(sys.argv[1], sys.argv[2])
     elif n == 4:
-        assign_task(sys.argv[1], sys.argv[2], sys.argv[3])
+        assign_task(sys.argv[1], sys.argv[2], sys.argv[3]) 
+
+
+main()
```

