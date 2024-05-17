# Comparing `tmp/common-tools-ai-bnq-0.1.7.tar.gz` & `tmp/common-tools-ai-bnq-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-tools-ai-bnq-0.1.7.tar", last modified: Tue May 14 03:06:07 2024, max compression
+gzip compressed data, was "common-tools-ai-bnq-0.1.8.tar", last modified: Fri May 17 08:21:47 2024, max compression
```

## Comparing `common-tools-ai-bnq-0.1.7.tar` & `common-tools-ai-bnq-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 03:06:07.297530 common-tools-ai-bnq-0.1.7/
--rw-rw-rw-   0        0        0     2531 2024-05-14 03:06:07.296530 common-tools-ai-bnq-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2304 2024-05-10 08:15:54.000000 common-tools-ai-bnq-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 03:06:07.267293 common-tools-ai-bnq-0.1.7/bnq_py_core/
--rw-rw-rw-   0        0        0      412 2024-05-14 03:05:23.000000 common-tools-ai-bnq-0.1.7/bnq_py_core/__init__.py
--rw-rw-rw-   0        0        0     1088 2024-05-06 07:47:07.000000 common-tools-ai-bnq-0.1.7/bnq_py_core/cos_connect.py
--rw-rw-rw-   0        0        0     8823 2024-05-14 03:04:15.000000 common-tools-ai-bnq-0.1.7/bnq_py_core/logger_record.py
--rw-rw-rw-   0        0        0     3218 2024-05-06 09:03:26.000000 common-tools-ai-bnq-0.1.7/bnq_py_core/nacos_connect.py
--rw-rw-rw-   0        0        0     2076 2024-05-13 11:48:35.000000 common-tools-ai-bnq-0.1.7/bnq_py_core/read_conf_from_ini.py
--rw-rw-rw-   0        0        0      716 2024-03-27 09:35:48.000000 common-tools-ai-bnq-0.1.7/bnq_py_core/singleton.py
-drwxrwxrwx   0        0        0        0 2024-05-14 03:06:07.295531 common-tools-ai-bnq-0.1.7/common_tools_ai_bnq.egg-info/
--rw-rw-rw-   0        0        0     2531 2024-05-14 03:06:07.000000 common-tools-ai-bnq-0.1.7/common_tools_ai_bnq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2024-05-14 03:06:07.000000 common-tools-ai-bnq-0.1.7/common_tools_ai_bnq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 03:06:07.000000 common-tools-ai-bnq-0.1.7/common_tools_ai_bnq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2024-05-14 03:06:07.000000 common-tools-ai-bnq-0.1.7/common_tools_ai_bnq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-14 03:06:07.000000 common-tools-ai-bnq-0.1.7/common_tools_ai_bnq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 03:06:07.297530 common-tools-ai-bnq-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      856 2024-05-14 03:05:54.000000 common-tools-ai-bnq-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:21:47.070850 common-tools-ai-bnq-0.1.8/
+-rw-rw-rw-   0        0        0     3204 2024-05-17 08:21:47.070850 common-tools-ai-bnq-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2977 2024-05-17 08:21:09.000000 common-tools-ai-bnq-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 08:21:47.052634 common-tools-ai-bnq-0.1.8/bnq_py_core/
+-rw-rw-rw-   0        0        0      412 2024-05-14 03:05:23.000000 common-tools-ai-bnq-0.1.8/bnq_py_core/__init__.py
+-rw-rw-rw-   0        0        0     1088 2024-05-06 07:47:07.000000 common-tools-ai-bnq-0.1.8/bnq_py_core/cos_connect.py
+-rw-rw-rw-   0        0        0     7750 2024-05-17 08:12:55.000000 common-tools-ai-bnq-0.1.8/bnq_py_core/logger_record.py
+-rw-rw-rw-   0        0        0     3218 2024-05-06 09:03:26.000000 common-tools-ai-bnq-0.1.8/bnq_py_core/nacos_connect.py
+-rw-rw-rw-   0        0        0     2076 2024-05-13 11:48:35.000000 common-tools-ai-bnq-0.1.8/bnq_py_core/read_conf_from_ini.py
+-rw-rw-rw-   0        0        0      716 2024-03-27 09:35:48.000000 common-tools-ai-bnq-0.1.8/bnq_py_core/singleton.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:21:47.069848 common-tools-ai-bnq-0.1.8/common_tools_ai_bnq.egg-info/
+-rw-rw-rw-   0        0        0     3204 2024-05-17 08:21:46.000000 common-tools-ai-bnq-0.1.8/common_tools_ai_bnq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2024-05-17 08:21:46.000000 common-tools-ai-bnq-0.1.8/common_tools_ai_bnq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 08:21:46.000000 common-tools-ai-bnq-0.1.8/common_tools_ai_bnq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2024-05-17 08:21:46.000000 common-tools-ai-bnq-0.1.8/common_tools_ai_bnq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-17 08:21:46.000000 common-tools-ai-bnq-0.1.8/common_tools_ai_bnq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 08:21:47.071849 common-tools-ai-bnq-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      856 2024-05-17 08:13:19.000000 common-tools-ai-bnq-0.1.8/setup.py
```

### Comparing `common-tools-ai-bnq-0.1.7/PKG-INFO` & `common-tools-ai-bnq-0.1.8/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,77 +1,135 @@
-Metadata-Version: 2.1
-Name: common-tools-ai-bnq
-Version: 0.1.7
-Summary: Common tools of AI module for BNQ
-Home-page: UNKNOWN
-Author: BNQ
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
-    python setup.py sdist bdist_wheel
-    twine upload dist/*
-
-
-1.NacConnect类，用于连接nacos服务，获取配置文件信息
-
-    NacConnect类中参数信息如下：
-        server_addresses: 地址
-        namespace: 命名空间
-        username: 用户名
-        password: 密码
-        group: 组合字典， 包括group_name和data_ids
-        conf_type: 配置文件类型， 非必需，值为json或yaml
-
-    示例如下：
-        test_data = {
-                        'group': {'t-dev': ['project_name_1', 'project_name_2']},
-                        'username': 'nacos',
-                        'password': 'nacos',
-                        'server_addresses': '127.0.0.1:8080',
-                        'namespace': 't-dev'
-                    }
-        conf_test = NacConnect(**test_data)
-        print(conf_test())
-
-2.LoggingRecord类，用于记录日志信息
-
-    LoggingRecord类中参数信息如下：
-        max_bytes: 日志文件最大大小， 默认值20M
-        backup_count: 日志备份最大数量， 默认值为10
-        log_level: 日志级别， 默认值为INFO
-        log_dir: 日志文件路径，默认在根目录下创建log文件夹
-
-    示例如下：
-        testLog = LoggingRecord(log_level=logging.DEBUG)
-        for i in range(10):
-            print(i, 'i')
-            print(testLog, "testLog")
-            testLog.debug(i)
-            testLog.info("中文测试")
-            testLog.error(i)
-            testLog.warning(i)
-            testLog.exception(i)
-
-3.SingletonMeta类，用于实现单例模式
-
-    示例如下：
-        class TestClass(metaclass=SingletonMeta):
-            def __init__(self):
-                pass
-
-4.CosConnect类，用于连接腾讯云存储平台cos
-
-    CosConnect类中参数信息如下：
-        secret_id: 腾讯云secret_id
-        secret_key: 腾讯云secret_key
-        region: 腾讯云存储区域
-
-    示例如下：
-        test_data = {
-                        'secret_id': 'AKIDxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx',
-                        'secret_key': 'xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx',
-                        'region': 'ap-guangzhou'
-                    }
-        cos_test = CosConnect(**test_data)
-        print(cos_test())
+## 打包和上传
 
+使用以下命令来生成和上传分发包：
+
+```bash
+python setup.py sdist bdist_wheel
+twine upload dist/*
+```
+
+## 类说明
+
+### 1. `NacConnect` 类
+
+用于连接 Nacos 服务，获取配置文件信息。
+
+#### 参数信息
+
+- `server_addresses`：地址
+- `namespace`：命名空间
+- `username`：用户名
+- `password`：密码
+- `group`：组合字典，包括 `group_name` 和 `data_ids`
+- `conf_type`：配置文件类型，非必需，值为 `json` 或 `yaml`
+
+#### 示例
+
+```python
+from bnq_py_core import NacConnect
+
+test_data = {
+    'group': {'t-dev': ['project_name_1', 'project_name_2']},
+    'username': 'nacos',
+    'password': 'nacos',
+    'server_addresses': '127.0.0.1:8080',
+    'namespace': 't-dev'
+}
+conf_test = NacConnect(**test_data)
+print(conf_test())
+```
+
+### 2. `LoggingRecord` 类
+
+用于记录日志信息。
+
+#### 参数信息
+
+- `max_bytes`：日志文件最大大小，默认值 20M
+- `backup_count`：日志备份最大数量，默认值为 10
+- `log_level`：日志级别，默认值为 `INFO`
+- `log_dir`：日志文件路径，默认在根目录下创建 `log` 文件夹
+
+#### 示例
+
+```python
+import logging
+
+from bnq_py_core import LoggingRecord
+
+testLog = LoggingRecord(log_level=logging.DEBUG)
+for i in range(10):
+    print(i, 'i')
+    print(testLog, "testLog")
+    testLog.debug(i)
+    testLog.info("中文测试")
+    testLog.error(i)
+    testLog.warning(i)
+    testLog.exception(i)
+```
+
+### 3. `LoggingRecordTimeRotation` 类
+
+用于记录日志信息, 可根据设定时间自动轮转日志文件。
+
+#### 参数信息
+
+- `max_bytes`：日志文件最大大小，默认值 20M
+- `backup_count`：日志备份最大数量，默认值为 10
+- `log_level`：日志级别，默认值为 `INFO`
+- `log_dir`：日志文件路径，默认在根目录下创建 `log` 文件夹
+
+#### 示例
+
+```python
+import logging
+
+from bnq_py_core import LoggingRecordTimeRotation
+
+testLog = LoggingRecordTimeRotation(log_level=logging.DEBUG)
+for i in range(10):
+    print(i, 'i')
+    print(testLog, "testLog")
+    testLog.debug(i)
+    testLog.info("中文测试")
+    testLog.error(i)
+    testLog.warning(i)
+    testLog.exception(i)
+```
+### 4. `SingletonMeta` 类
+
+用于实现单例模式。
+
+#### 示例
+
+```python
+from bnq_py_core import SingletonMeta
+
+
+class TestClass(metaclass=SingletonMeta):
+    def __init__(self):
+        pass
+```
+
+### 5. `CosConnect` 类
+
+用于连接腾讯云存储平台 COS。
+
+#### 参数信息
+
+- `secret_id`：腾讯云 secret_id
+- `secret_key`：腾讯云 secret_key
+- `region`：腾讯云存储区域
+
+#### 示例
+
+```python
+from bnq_py_core import CosConnect
+
+test_data = {
+    'secret_id': 'AKIDxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx',
+    'secret_key': 'xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx',
+    'region': 'ap-guangzhou'
+}
+cos_test = CosConnect(**test_data)
+
+```
```

### Comparing `common-tools-ai-bnq-0.1.7/bnq_py_core/cos_connect.py` & `common-tools-ai-bnq-0.1.8/bnq_py_core/cos_connect.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.7/bnq_py_core/logger_record.py` & `common-tools-ai-bnq-0.1.8/bnq_py_core/logger_record.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,53 +12,35 @@
 import sys
 import time
 
 from structlog import configure, processors, stdlib
 from termcolor import colored
 
 
-class LoggingRecord(object):
-    """日志记录类，用于记录运行中的信息
-
+class _LoggingF(object):
+    """
+    日志记录父类
     """
-    __instance = None  # 单例
-    __filename = None  # 日志文件名
-
-    def __new__(cls, log_dir=None, *args, **kwargs):
-        """保证日志模块是单例模式"""
-        if not cls.__instance:
-            cls.__instance = super(LoggingRecord, cls).__new__(cls)
-        __now_time = int(round(time.time()))
-        __time_record = time.strftime("%Y%m%d", time.localtime(__now_time))
-        cls.__filename = __time_record + "_BNQ_AI.log"
-        return cls.__instance
 
-    def __init__(self, max_bytes=20 * 1024 * 1024, backup_count=10, log_level=logging.INFO, log_dir=None):
+    def __init__(self, log_dir=None, max_bytes=20 * 1024 * 1024, backup_count=10, log_level=logging.INFO):
         self.record_info = None
         self.logger = None
         self.log_record_path = log_dir  # 日志记录路径
         self.max_bytes = max_bytes  # 日志文件大小
         self.backup_count = backup_count  # 日志文件备份数量
         self.level = log_level  # 日志级别
-        self.init_log()
+        self.level_third = logging.WARNING  # 第三方库日志级别
 
-    def init_log(self):
-        """初始化log模块
-
-        Returns:
+    def get_logging_config(self, log_filename):
+        """获取logging配置
 
+        :param log_filename:
+        :return:
         """
-        if self.log_record_path is None:
-            # 获取根目录路径，并创建日志文件夹
-            # self.log_record_path = os.path.join(os.getcwd(), "logs")
-            self.log_record_path = "/bnq/logs"
-
-        pathlib.Path(self.log_record_path).mkdir(parents=True, exist_ok=True)
-        log_filename = os.path.join(self.log_record_path, self.__filename)
-        logging.config.dictConfig({
+        return {
             "version": 1,
             "disable_existing_loggers": False,
             "formatters": {
                 "default": {
                     "format": '%(asctime)s - %(levelname)s - %(name)s - %(message)s'
                 },
                 "console": {
@@ -72,28 +54,69 @@
                     "level": self.level,
                     "formatter": "console",
                     "stream": sys.stdout
                 },
                 "file_handler": {
                     "level": self.level,
                     "formatter": "default",
-                    "class": "concurrent_log_handler.ConcurrentRotatingFileHandler",
+                    "class": "concurrent_log_handler.ConcurrentTimedRotatingFileHandler",
                     "filename": log_filename,
+                    "when": "midnight",
                     "maxBytes": self.max_bytes,
                     "backupCount": self.backup_count,
                     "encoding": "UTF-8"
                 },
             },
             "loggers": {
                 "": {
-                    "handlers": ["file_handler", "console_handler"],
-                    "level": self.level
+                    "handlers": ["console_handler"],
+                    "level": self.level_third
                 }
+            },
+            "root": {
+                "level": self.level,
+                "handlers": ["file_handler", "console_handler"]
             }
-        })
+        }
+
+
+class LoggingRecord(_LoggingF):
+    """日志记录类，用于记录运行中的信息
+
+    """
+    __instance = None  # 单例
+    __filename = None  # 日志文件名
+
+    def __new__(cls, log_dir=None, *args, **kwargs):
+        """保证日志模块是单例模式"""
+        if not cls.__instance:
+            cls.__instance = super(LoggingRecord, cls).__new__(cls)
+        __now_time = int(round(time.time()))
+        __time_record = time.strftime("%Y%m%d", time.localtime(__now_time))
+        cls.__filename = __time_record + "_BNQ_AI.log"
+        return cls.__instance
+
+    def __init__(self, max_bytes=20 * 1024 * 1024, backup_count=10, log_level=logging.INFO, log_dir=None):
+        super().__init__(log_dir, max_bytes, backup_count, log_level)
+        self.init_log()
+
+    def init_log(self):
+        """初始化log模块
+
+        Returns:
+
+        """
+        if self.log_record_path is None:
+            # 获取根目录路径，并创建日志文件夹
+            # self.log_record_path = os.path.join(os.getcwd(), "logs")
+            self.log_record_path = "/bnq/logs"
+
+        pathlib.Path(self.log_record_path).mkdir(parents=True, exist_ok=True)
+        log_filename = os.path.join(self.log_record_path, self.__filename)
+        logging.config.dictConfig(self.get_logging_config(log_filename))
         configure(
             context_class=dict,
             logger_factory=stdlib.LoggerFactory(),
             wrapper_class=stdlib.BoundLogger,
             processors=[
                 stdlib.filter_by_level,
                 stdlib.PositionalArgumentsFormatter(),
@@ -148,84 +171,43 @@
         """
         self.logger.warning(warning_info)
 
     def exception(self, exception_info):
         self.logger.exception(exception_info)
 
 
-class LoggingRecordTimeRotation(object):
+class LoggingRecordTimeRotation(_LoggingF):
     """日志记录类，用于记录运行中的信息, 日志文件按时间切割
 
     """
     __instance = None  # 单例
 
     def __new__(cls, log_dir=None, *args, **kwargs):
         """保证日志模块是单例模式"""
         if not cls.__instance:
             cls.__instance = super(LoggingRecordTimeRotation, cls).__new__(cls)
         return cls.__instance
 
     def __init__(self, max_bytes=20 * 1024 * 1024, backup_count=10, log_level=logging.INFO, log_dir=None):
-        self.record_info = None
-        self.logger = None
-        self.log_record_path = log_dir  # 日志记录路径
-        self.max_bytes = max_bytes  # 日志文件大小
-        self.backup_count = backup_count  # 日志文件备份数量
-        self.level = log_level  # 日志级别
+        super().__init__(log_dir, max_bytes, backup_count, log_level)
         self.init_log()
 
     def init_log(self):
         """初始化log模块
 
         Returns:
 
         """
         if self.log_record_path is None:
             # 获取根目录路径，并创建日志文件夹
             self.log_record_path = "/bnq/logs"
 
         pathlib.Path(self.log_record_path).mkdir(parents=True, exist_ok=True)
         log_filename = os.path.join(self.log_record_path, "access.log")
-        logging.config.dictConfig({
-            "version": 1,
-            "disable_existing_loggers": False,
-            "formatters": {
-                "default": {
-                    "format": '%(asctime)s - %(levelname)s - %(name)s - %(message)s'
-                },
-                "console": {
-                    "format": colored(f'[%(asctime)s][%(levelname)1.1s][%(process)d][%(name)s]', 'green') + colored(
-                        f'(%(filename)s %(lineno)d)', 'yellow') + ': %(message)s'
-                }
-            },
-            "handlers": {
-                "console_handler": {
-                    "class": "logging.StreamHandler",
-                    "level": self.level,
-                    "formatter": "console",
-                    "stream": sys.stdout
-                },
-                "file_handler": {
-                    "level": self.level,
-                    "formatter": "default",
-                    "class": "concurrent_log_handler.ConcurrentTimedRotatingFileHandler",
-                    "filename": log_filename,
-                    "when": "midnight",
-                    "maxBytes": self.max_bytes,
-                    "backupCount": self.backup_count,
-                    "encoding": "UTF-8"
-                },
-            },
-            "loggers": {
-                "": {
-                    "handlers": ["file_handler", "console_handler"],
-                    "level": self.level
-                }
-            }
-        })
+        logging.config.dictConfig(self.get_logging_config(log_filename))
         self.logger = logging.getLogger("BNQ-AI")
         self.logger.level = self.level
 
     def debug(self, record_info):
         """debug级别的日志记录
 
         :param record_info:
@@ -269,18 +251,15 @@
 
     def exception(self, exception_info):
         self.logger.exception(exception_info)
 
 
 if __name__ == "__main__":
 
-    # og_record_path = os.path.join(os.path.dirname(os.path.dirname(os.path.abspath(__file__))), "log")
-
-    testLog = LoggingRecordTimeRotation(log_level=logging.DEBUG)
     for i in range(10):
+        testLog = LoggingRecordTimeRotation(log_level=logging.DEBUG)
         print(testLog, "testLog")
         testLog.debug(i)
         testLog.info("中文测试")
         testLog.error(i)
         testLog.warning(i)
         testLog.exception(i)
-        # time.sleep(3)
```

### Comparing `common-tools-ai-bnq-0.1.7/bnq_py_core/nacos_connect.py` & `common-tools-ai-bnq-0.1.8/bnq_py_core/nacos_connect.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.7/bnq_py_core/read_conf_from_ini.py` & `common-tools-ai-bnq-0.1.8/bnq_py_core/read_conf_from_ini.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.7/bnq_py_core/singleton.py` & `common-tools-ai-bnq-0.1.8/bnq_py_core/singleton.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.1.7/setup.py` & `common-tools-ai-bnq-0.1.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='common-tools-ai-bnq',
-    version='0.1.7',
+    version='0.1.8',
     packages=find_packages(),
     install_requires=[
         # 依赖项列表
         'structlog==23.1.0',
         'concurrent-log-handler==0.9.25',
         'nacos-sdk-python==0.1.12',
         'PyYAML==6.0.1',
```

