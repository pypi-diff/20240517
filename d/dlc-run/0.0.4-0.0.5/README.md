# Comparing `tmp/dlc_run-0.0.4.tar.gz` & `tmp/dlc_run-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dlc_run-0.0.4.tar", last modified: Wed May 15 04:06:27 2024, max compression
+gzip compressed data, was "dist/dlc_run-0.0.5.tar", last modified: Fri May 17 09:38:04 2024, max compression
```

## Comparing `dlc_run-0.0.4.tar` & `dlc_run-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:06:27.000000 dlc_run-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-15 04:06:27.000000 dlc_run-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 04:06:25.000000 dlc_run-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:06:27.000000 dlc_run-0.0.4/dlc_run/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 04:06:25.000000 dlc_run-0.0.4/dlc_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-05-15 04:06:25.000000 dlc_run-0.0.4/dlc_run/dlc_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-15 04:06:25.000000 dlc_run-0.0.4/dlc_run/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:06:27.000000 dlc_run-0.0.4/dlc_run.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-15 04:06:27.000000 dlc_run-0.0.4/dlc_run.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-15 04:06:27.000000 dlc_run-0.0.4/dlc_run.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 04:06:27.000000 dlc_run-0.0.4/dlc_run.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-15 04:06:27.000000 dlc_run-0.0.4/dlc_run.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 04:06:27.000000 dlc_run-0.0.4/dlc_run.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 04:06:27.000000 dlc_run-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-15 04:06:25.000000 dlc_run-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:38:04.000000 dlc_run-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-17 09:38:04.000000 dlc_run-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 09:37:57.000000 dlc_run-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:38:04.000000 dlc_run-0.0.5/dlc_run/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:37:57.000000 dlc_run-0.0.5/dlc_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-05-17 09:37:57.000000 dlc_run-0.0.5/dlc_run/dlc_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-17 09:37:57.000000 dlc_run-0.0.5/dlc_run/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:38:04.000000 dlc_run-0.0.5/dlc_run.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-17 09:38:03.000000 dlc_run-0.0.5/dlc_run.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-17 09:38:04.000000 dlc_run-0.0.5/dlc_run.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:38:03.000000 dlc_run-0.0.5/dlc_run.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 09:38:03.000000 dlc_run-0.0.5/dlc_run.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 09:38:03.000000 dlc_run-0.0.5/dlc_run.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 09:38:04.000000 dlc_run-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-17 09:37:57.000000 dlc_run-0.0.5/setup.py
```

### Comparing `dlc_run-0.0.4/dlc_run/dlc_run.py` & `dlc_run-0.0.5/dlc_run/dlc_run.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,36 +14,38 @@
         HOME = f'/cpfs01/user/{user_names[0]}'
     else:
         HOME = None
 else:
     HOME = None
 
 
-def get_conda_envs():
+def get_conda_envs(shell='zsh'):
     """Function to retrieve all conda environments."""
     try:
-        result = subprocess.run(['conda', 'env', 'list'],
+        cmds = f'{shell} -i -c  "conda env list"'
+        result = subprocess.run(cmds,
                                 capture_output=True,
                                 text=True,
-                                check=True)
+                                check=True,
+                                shell=True)
         envs = []
         for line in result.stdout.split('\n'):
             if line and not line.startswith('#'):
                 env_name = line.split()[0]
                 envs.append(env_name)
         return envs
     except subprocess.SubprocessError as e:
         print(f'Failed to retrieve conda environments: {e}')
         return []
 
 
-def validate_conda_env(value):
+def validate_conda_env(value, shell='zsh'):
     """Validate the conda environment name against the list of available
     environments or check if it's a valid path."""
-    envs = get_conda_envs()
+    envs = get_conda_envs(shell)
     if value in envs or Path(value).exists() or not value:
         return value
     raise argparse.ArgumentTypeError(
         f'{value} is not a valid conda environment. '
         f"Available: {', '.join(envs)}")
 
 
@@ -122,53 +124,47 @@
     parser.add_argument('--home', default=HOME, help='The path for HOME')
     parser.add_argument('--shell',
                         type=str,
                         choices=['bash', 'zsh', 'none'],
                         default='zsh',
                         help='Shell to use for command execution')
     parser.add_argument('--conda-env',
-                        type=validate_conda_env,
+                        type=str,
                         default='',
                         help='Conda environment to activate')
-    parser.add_argument('--proxy',
-                        action='store_true',
-                        help='Toggle proxy settings')
     parser.add_argument('--env',
                         '--environs',
                         action='append',
                         default=[],
                         help=('Additional environment variables, '
                               "either `--env 'KEY1=VALUE1;KEY2=VALUE2'` or "
                               '`--env KEY1=VALUE1 --env KEY2=VALUE2`'))
 
     parser.add_argument(
         'task_cmds',
         # required=True,
         nargs=argparse.REMAINDER,
         help='Command line to execute, similar to typing in the shell.')
     args = parser.parse_args()
+    try:
+        args.conda_env = validate_conda_env(args.conda_env, args.shell)
+    except argparse.ArgumentTypeError as e:
+        parser.error(e)
 
     assert args.home is not None, 'HOME is not set.'
     home_cmd = f'export HOME={args.home}'
     shell_cmd = (f'{args.shell} -c "source ~/.{args.shell}rc'
                  if args.shell != 'none' else '')
     conda_cmd = f'conda activate {args.conda_env}' if args.conda_env else ''
-    if args.proxy:
-        proxy_cmd = ('export http_proxy=http://58.34.83.134:31128 && '
-                     'export https_proxy=http://58.34.83.134:31128')
-    else:
-        proxy_cmd = 'unset http_proxy;unset https_proxy'
     env_dict = parse_env_vars(args.env)
     env_var_cmds = ' && '.join(
         [f'export {key}={value}' for key, value in env_dict.items()])
 
     env_cmds = [
-        cmd
-        for cmd in [home_cmd, proxy_cmd, env_var_cmds, shell_cmd, conda_cmd]
-        if cmd
+        cmd for cmd in [home_cmd, env_var_cmds, shell_cmd, conda_cmd] if cmd
     ]
     full_env_cmd = ' && '.join(env_cmds)
 
     full_command = (f'{full_env_cmd} && cd {os.getcwd()} && '
                     f"{' '.join(args.task_cmds).strip()}")
     if shell_cmd:
         full_command += '"'
@@ -182,15 +178,15 @@
         f'--data_sources {args.data_sources}',
         f'--workspace_id {args.workspace_id}',
         f'--workers {args.worker_count}',
         f'--worker_cpu {args.worker_cpu}',
         f'--worker_gpu {args.worker_gpu}',
         f'--worker_memory {args.worker_memory}Gi',
         f'--worker_image {args.worker_image}',
-        f'--worker_shared_memory {args.worker_memory // 2}',
+        f'--worker_shared_memory {args.worker_memory // 2}Gi',
         '--interactive' if args.interactive else '',
         f"--command '{full_command}'",
     ]
 
     dlc_full_command = ' '.join(filter(None, dlc_command))
     print(f'Executing command:\n{dlc_full_command}')
     subprocess.run(dlc_full_command, shell=True, check=True)
```

### Comparing `dlc_run-0.0.4/dlc_run/version.py` & `dlc_run-0.0.5/dlc_run/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 
 
 def parse_version_info(version_str: str, length: int = 4) -> tuple:
     """Parse a version string into a tuple.
 
     Args:
         version_str (str): The version string.
```

### Comparing `dlc_run-0.0.4/setup.py` & `dlc_run-0.0.5/setup.py`

 * *Files identical despite different names*

