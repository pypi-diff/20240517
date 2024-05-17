# Comparing `tmp/aedev_git_repo_manager-0.3.80.tar.gz` & `tmp/aedev_git_repo_manager-0.3.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aedev_git_repo_manager-0.3.80.tar", last modified: Wed May 15 13:10:41 2024, max compression
+gzip compressed data, was "aedev_git_repo_manager-0.3.81.tar", last modified: Fri May 17 16:51:07 2024, max compression
```

## Comparing `aedev_git_repo_manager-0.3.80.tar` & `aedev_git_repo_manager-0.3.81.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:10:41.370157 aedev_git_repo_manager-0.3.80/
--rw-rw-rw-   0 root         (0) root         (0)    35002 2024-05-15 13:10:29.000000 aedev_git_repo_manager-0.3.80/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     6549 2024-05-15 13:10:41.370157 aedev_git_repo_manager-0.3.80/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3543 2024-05-15 13:10:29.000000 aedev_git_repo_manager-0.3.80/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:10:41.362157 aedev_git_repo_manager-0.3.80/aedev/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:10:41.364157 aedev_git_repo_manager-0.3.80/aedev/git_repo_manager/
--rw-rw-rw-   0 root         (0) root         (0)     1879 2024-05-15 13:10:29.000000 aedev_git_repo_manager-0.3.80/aedev/git_repo_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   198366 2024-05-15 13:10:29.000000 aedev_git_repo_manager-0.3.80/aedev/git_repo_manager/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:10:41.367157 aedev_git_repo_manager-0.3.80/aedev_git_repo_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6549 2024-05-15 13:10:41.000000 aedev_git_repo_manager-0.3.80/aedev_git_repo_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-15 13:10:41.000000 aedev_git_repo_manager-0.3.80/aedev_git_repo_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 13:10:41.000000 aedev_git_repo_manager-0.3.80/aedev_git_repo_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      117 2024-05-15 13:10:41.000000 aedev_git_repo_manager-0.3.80/aedev_git_repo_manager.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      543 2024-05-15 13:10:41.000000 aedev_git_repo_manager-0.3.80/aedev_git_repo_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-15 13:10:41.000000 aedev_git_repo_manager-0.3.80/aedev_git_repo_manager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 13:10:41.000000 aedev_git_repo_manager-0.3.80/aedev_git_repo_manager.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 13:10:41.370157 aedev_git_repo_manager-0.3.80/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      704 2024-05-15 13:10:29.000000 aedev_git_repo_manager-0.3.80/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:10:41.366157 aedev_git_repo_manager-0.3.80/tests/
--rw-rw-rw-   0 root         (0) root         (0)   158050 2024-05-15 13:10:29.000000 aedev_git_repo_manager-0.3.80/tests/test_git_repo_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:51:07.949672 aedev_git_repo_manager-0.3.81/
+-rw-rw-rw-   0 root         (0) root         (0)    35002 2024-05-17 16:50:55.000000 aedev_git_repo_manager-0.3.81/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     6520 2024-05-17 16:51:07.948672 aedev_git_repo_manager-0.3.81/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2024-05-17 16:50:55.000000 aedev_git_repo_manager-0.3.81/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:51:07.940672 aedev_git_repo_manager-0.3.81/aedev/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:51:07.942672 aedev_git_repo_manager-0.3.81/aedev/git_repo_manager/
+-rw-rw-rw-   0 root         (0) root         (0)     1879 2024-05-17 16:50:55.000000 aedev_git_repo_manager-0.3.81/aedev/git_repo_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   198340 2024-05-17 16:50:55.000000 aedev_git_repo_manager-0.3.81/aedev/git_repo_manager/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:51:07.945672 aedev_git_repo_manager-0.3.81/aedev_git_repo_manager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6520 2024-05-17 16:51:07.000000 aedev_git_repo_manager-0.3.81/aedev_git_repo_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-17 16:51:07.000000 aedev_git_repo_manager-0.3.81/aedev_git_repo_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 16:51:07.000000 aedev_git_repo_manager-0.3.81/aedev_git_repo_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      117 2024-05-17 16:51:07.000000 aedev_git_repo_manager-0.3.81/aedev_git_repo_manager.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      529 2024-05-17 16:51:07.000000 aedev_git_repo_manager-0.3.81/aedev_git_repo_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-17 16:51:07.000000 aedev_git_repo_manager-0.3.81/aedev_git_repo_manager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 16:51:07.000000 aedev_git_repo_manager-0.3.81/aedev_git_repo_manager.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 16:51:07.949672 aedev_git_repo_manager-0.3.81/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      704 2024-05-17 16:50:55.000000 aedev_git_repo_manager-0.3.81/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 16:51:07.945672 aedev_git_repo_manager-0.3.81/tests/
+-rw-rw-rw-   0 root         (0) root         (0)   157961 2024-05-17 16:50:55.000000 aedev_git_repo_manager-0.3.81/tests/test_git_repo_manager.py
```

### Comparing `aedev_git_repo_manager-0.3.80/LICENSE.md` & `aedev_git_repo_manager-0.3.81/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aedev_git_repo_manager-0.3.80/PKG-INFO` & `aedev_git_repo_manager-0.3.81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aedev_git_repo_manager
-Version: 0.3.80
+Version: 0.3.81
 Summary: aedev namespace package portion git_repo_manager: create and maintain local/remote git repositories of Python projects
 Home-page: https://gitlab.com/aedev-group/aedev_git_repo_manager
 Author: AndiEcker
 Author-email: aecker2@gmail.com
 License: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Documentation, https://aedev.readthedocs.io/en/latest/_autosummary/aedev.git_repo_manager.html
 Project-URL: Repository, https://gitlab.com/aedev-group/aedev_git_repo_manager
@@ -27,15 +27,14 @@
 Requires-Dist: mypy
 Requires-Dist: packaging
 Requires-Dist: PyGithub
 Requires-Dist: pylint
 Requires-Dist: pytest
 Requires-Dist: pytest-cov
 Requires-Dist: python-gitlab
-Requires-Dist: python-dotenv
 Requires-Dist: setuptools
 Requires-Dist: ae_base
 Requires-Dist: ae_files
 Requires-Dist: ae_paths
 Requires-Dist: ae_core
 Requires-Dist: ae_console
 Requires-Dist: ae_dynamicod
@@ -72,25 +71,25 @@
 Requires-Dist: typing; extra == "tests"
 Requires-Dist: types-setuptools; extra == "tests"
 Requires-Dist: wheel; extra == "tests"
 Requires-Dist: twine; extra == "tests"
 
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.aedev V0.3.23 -->
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_namespace_root V0.3.14 -->
-# git_repo_manager 0.3.80
+# git_repo_manager 0.3.81
 
 [![GitLab develop](https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/develop?logo=python)](
     https://gitlab.com/aedev-group/aedev_git_repo_manager)
 [![LatestPyPIrelease](
-    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.79?logo=python)](
-    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.79)
+    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.80?logo=python)](
+    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.80)
 [![PyPIVersions](https://img.shields.io/pypi/v/aedev_git_repo_manager)](
     https://pypi.org/project/aedev-git-repo-manager/#history)
 
->aedev_git_repo_manager package 0.3.80.
+>aedev_git_repo_manager package 0.3.81.
 
 [![Coverage](https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage/index.html)
 [![MyPyPrecision](https://aedev-group.gitlab.io/aedev_git_repo_manager/mypy.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/lineprecision.txt)
 [![PyLintScore](https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.log)
```

### Comparing `aedev_git_repo_manager-0.3.80/README.md` & `aedev_git_repo_manager-0.3.81/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.aedev V0.3.23 -->
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_namespace_root V0.3.14 -->
-# git_repo_manager 0.3.80
+# git_repo_manager 0.3.81
 
 [![GitLab develop](https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/develop?logo=python)](
     https://gitlab.com/aedev-group/aedev_git_repo_manager)
 [![LatestPyPIrelease](
-    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.79?logo=python)](
-    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.79)
+    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.80?logo=python)](
+    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.80)
 [![PyPIVersions](https://img.shields.io/pypi/v/aedev_git_repo_manager)](
     https://pypi.org/project/aedev-git-repo-manager/#history)
 
->aedev_git_repo_manager package 0.3.80.
+>aedev_git_repo_manager package 0.3.81.
 
 [![Coverage](https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage/index.html)
 [![MyPyPrecision](https://aedev-group.gitlab.io/aedev_git_repo_manager/mypy.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/lineprecision.txt)
 [![PyLintScore](https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.log)
```

### Comparing `aedev_git_repo_manager-0.3.80/aedev/git_repo_manager/__init__.py` & `aedev_git_repo_manager-0.3.81/aedev/git_repo_manager/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,8 +35,8 @@
 
 in conjunction with the template projects of the `aedev` namespace (like e.g. :mod:`aedev.tpl_project`) any common
 portions file (even the ``setup.py`` file) can be created/maintained as a template in a single place, and then
 requested and updated individually for each portion project.
 """
 
 
-__version__ = '0.3.80'
+__version__ = '0.3.81'
```

### Comparing `aedev_git_repo_manager-0.3.80/aedev/git_repo_manager/__main__.py` & `aedev_git_repo_manager-0.3.81/aedev/git_repo_manager/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,31 +14,29 @@
 from difflib import context_diff, diff_bytes, ndiff, unified_diff
 from functools import wraps
 from traceback import format_exc
 from typing import (
     Any, Callable, Collection, Dict, Iterable, Iterator, List, Optional, OrderedDict as OrderedDictType,
     Sequence, Set, TYPE_CHECKING, Tuple, Union, cast)
 
-from dotenv import find_dotenv, load_dotenv
-
 from github import Github, Auth, GithubException
 from github.AuthenticatedUser import AuthenticatedUser
 from github.Repository import Repository
 
 from gitlab import Gitlab, GitlabCreateError, GitlabError, GitlabHttpError
 from gitlab.const import MAINTAINER_ACCESS
 from gitlab.v4.objects import Group, Project, User
 
 from packaging.version import Version
 from PIL import Image
 
 import ae.base                                                                          # type: ignore # for patching
 from ae.base import (
     PY_EXT, PY_INIT, TEMPLATES_FOLDER, UNSET, UnsetType,
-    camel_to_snake, duplicates, in_wd, module_attr, norm_name, norm_path,
+    camel_to_snake, duplicates, in_wd, load_dotenvs, module_attr, norm_name, norm_path,
     project_main_file, read_file, stack_var, write_file)
 from ae.files import FileObject                                                         # type: ignore
 from ae.paths import (                                                                  # type: ignore
     Collector, FilesRegister, coll_folders, path_files, path_items, paths_match, skip_py_cache_files)
 from ae.console import ConsoleApp, sh_exec                                              # type: ignore
 from ae.dynamicod import try_eval                                                       # type: ignore
 from ae.literal import Literal                                                          # type: ignore
@@ -669,15 +667,15 @@
     :param project_path:        optional rel/abs path of the package/app/project root directory of a new and existing
                                 project (defaults to the current working directory if empty or not passed).
     :return:                    dict/mapping with the determined project development variable values.
     """
     abs_prj_path = os.path.abspath(project_path)
     if os.path.exists(abs_prj_path):
         with in_wd(abs_prj_path):   # load .env file from project path folder (or above from projects folder)
-            load_dotenv(dotenv_path=find_dotenv(usecwd=True))
+            load_dotenvs()
 
     pdv = cast(PdvType, project_env_vars(project_path=project_path))
     project_path = pdv_str(pdv, 'project_path')     # re-read as absolute path
     project_type = pdv_str(pdv, 'project_type')
     sep = os.linesep
     ins = sep + " " * 4
 
@@ -2635,26 +2633,29 @@
         self._release_project(ini_pdv, version_tag)
 
     @_action(shortcut='request')
     def request_merge(self, ini_pdv: PdvType):
         """ request merge of the origin=fork repository into the main branch at remote/upstream=forked. """
         # see https://docs.github.com/de/rest/pulls/pulls?apiVersion=2022-11-28#create-a-pull-request
         src_prj, tgt_prj, forked, branch = self._repo_merge_src_dst_fork_branch(ini_pdv)
+        if TYPE_CHECKING:
+            assert isinstance(src_prj, Repository)
+            assert isinstance(tgt_prj, Repository)
 
         commit_msg_title, commit_msg_body = read_file(_check_commit_msg_file(ini_pdv)).split(os.linesep, maxsplit=1)
         merge_req = tgt_prj.create_pull(base=MAIN_BRANCH, head=branch, title=commit_msg_title, body=commit_msg_body)
         if _debug_or_verbose():
             diff_url = merge_req.diff_url
             cae.po(f"    . merge request diffs available at: {diff_url}")
 
         action = "requested merge"
         if not forked:
-            _wait()  # wait for created un-forked/direct maintainer merge request (with --force --user=group_name)
+            _wait()  # wait for created un-forked/direct maintainer merge request
             tgt_prj.merge(base=MAIN_BRANCH, head=branch, commit_message=commit_msg_title + os.linesep + commit_msg_body)
-            action = "auto-merged un-forked and forced merge request"
+            action = "auto-merged un-forked merge request"
 
         cae.po(f" ==== {action} of branch {branch} from fork/origin ({src_prj.id}) into upstream ({tgt_prj.id})")
 
 
 class GitlabCom(RemoteHost):
     """ remote connection and actions on gitlab.com. """
     connection: Gitlab                  #: connection to Gitlab host
@@ -2975,17 +2976,17 @@
             # 'subscribed': True,
         })
         if _debug_or_verbose():
             cae.po(f"    . merge request diffs: {PPF([_.attributes for _ in merge_req.diffs.list()])}")
 
         action = "requested merge"
         if not forked:
-            _wait()  # wait for created un-forked/direct maintainer merge request (with --force --user=group_name)
+            _wait()  # wait for created un-forked/direct maintainer merge request
             merge_req.merge(merge_commit_message=commit_msg)
-            action = "auto-merged un-forked and forced merge request"
+            action = "auto-merged un-forked merge request"
 
         cae.po(f" ==== {action} of branch {branch} from fork/origin ({src_prj.id}) into upstream ({tgt_prj.id})")
 
     @_action(arg_names=((), ('fragment', ), ))
     def search_repos(self, ini_pdv: PdvType, fragment: str = ""):
         """ search remote repositories via a text fragment in its project name/description. """
         fragment = fragment or _get_prj_name(ini_pdv)
```

### Comparing `aedev_git_repo_manager-0.3.80/aedev_git_repo_manager.egg-info/PKG-INFO` & `aedev_git_repo_manager-0.3.81/aedev_git_repo_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aedev_git_repo_manager
-Version: 0.3.80
+Version: 0.3.81
 Summary: aedev namespace package portion git_repo_manager: create and maintain local/remote git repositories of Python projects
 Home-page: https://gitlab.com/aedev-group/aedev_git_repo_manager
 Author: AndiEcker
 Author-email: aecker2@gmail.com
 License: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Documentation, https://aedev.readthedocs.io/en/latest/_autosummary/aedev.git_repo_manager.html
 Project-URL: Repository, https://gitlab.com/aedev-group/aedev_git_repo_manager
@@ -27,15 +27,14 @@
 Requires-Dist: mypy
 Requires-Dist: packaging
 Requires-Dist: PyGithub
 Requires-Dist: pylint
 Requires-Dist: pytest
 Requires-Dist: pytest-cov
 Requires-Dist: python-gitlab
-Requires-Dist: python-dotenv
 Requires-Dist: setuptools
 Requires-Dist: ae_base
 Requires-Dist: ae_files
 Requires-Dist: ae_paths
 Requires-Dist: ae_core
 Requires-Dist: ae_console
 Requires-Dist: ae_dynamicod
@@ -72,25 +71,25 @@
 Requires-Dist: typing; extra == "tests"
 Requires-Dist: types-setuptools; extra == "tests"
 Requires-Dist: wheel; extra == "tests"
 Requires-Dist: twine; extra == "tests"
 
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.aedev V0.3.23 -->
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_namespace_root V0.3.14 -->
-# git_repo_manager 0.3.80
+# git_repo_manager 0.3.81
 
 [![GitLab develop](https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/develop?logo=python)](
     https://gitlab.com/aedev-group/aedev_git_repo_manager)
 [![LatestPyPIrelease](
-    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.79?logo=python)](
-    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.79)
+    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.80?logo=python)](
+    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.80)
 [![PyPIVersions](https://img.shields.io/pypi/v/aedev_git_repo_manager)](
     https://pypi.org/project/aedev-git-repo-manager/#history)
 
->aedev_git_repo_manager package 0.3.80.
+>aedev_git_repo_manager package 0.3.81.
 
 [![Coverage](https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage/index.html)
 [![MyPyPrecision](https://aedev-group.gitlab.io/aedev_git_repo_manager/mypy.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/lineprecision.txt)
 [![PyLintScore](https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.log)
```

### Comparing `aedev_git_repo_manager-0.3.80/aedev_git_repo_manager.egg-info/requires.txt` & `aedev_git_repo_manager-0.3.81/aedev_git_repo_manager.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 mypy
 packaging
 PyGithub
 pylint
 pytest
 pytest-cov
 python-gitlab
-python-dotenv
 setuptools
 ae_base
 ae_files
 ae_paths
 ae_core
 ae_console
 ae_dynamicod
```

### Comparing `aedev_git_repo_manager-0.3.80/setup.py` & `aedev_git_repo_manager-0.3.81/setup.py`

 * *Files identical despite different names*

### Comparing `aedev_git_repo_manager-0.3.80/tests/test_git_repo_manager.py` & `aedev_git_repo_manager-0.3.81/tests/test_git_repo_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from collections import OrderedDict
 from conftest import skip_gitlab_ci
 from unittest.mock import patch
 
 from ae.base import (
     BUILD_CONFIG_FILE, DOCS_FOLDER, PY_CACHE_FOLDER, PY_EXT, PY_INIT, PY_MAIN, TEMPLATES_FOLDER, TESTS_FOLDER,
-    norm_name, norm_path, project_main_file, read_file, write_file)
+    load_dotenvs, norm_name, norm_path, project_main_file, read_file, write_file)
 from ae.paths import path_items
 from aedev.setup_project import (
     APP_PRJ, DJANGO_PRJ, MODULE_PRJ, NO_PRJ, PACKAGE_PRJ, PARENT_FOLDERS, PARENT_PRJ, REQ_DEV_FILE_NAME, ROOT_PRJ,
     code_file_version)
 
 import aedev.git_repo_manager.__main__ as git_repo_manager_main
 from aedev.git_repo_manager import __version__ as grm_version
@@ -108,17 +108,15 @@
 @pytest.fixture
 def gitlab_remote(mocked_app_options):
     """ provide a connected Gitlab remote repository api. """
     repo_domain = "gitlab.com"
     mocked_app_options['group'] = "aedev-group"
     mocked_app_options['namespace'] = ""
     mocked_app_options['project'] = "aedev_git_repo_manager"
-    from dotenv import find_dotenv, load_dotenv
-    # load_dotenv()   # pytest resets os.environ in each test run, reverting values set by load_dotenv in __main__.py
-    load_dotenv(dotenv_path=find_dotenv(usecwd=True))
+    load_dotenvs()  # pytest resets os.environ in each test run, reverting values set by load_dotenvs in __main__.py
     mocked_app_options['token'] = repo_token = cae.get_variable(f'repo_token_at_{norm_name(repo_domain)}')
 
     remote_project = GitlabCom()
     #remote_project.connect(project_dev_vars(), cae.get_variable('repo_token'))
     remote_project.connect({'REPO_HOST_PROTOCOL': "https://",
                             'repo_domain': repo_domain,
                             'repo_token': repo_token})
```

