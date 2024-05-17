# Comparing `tmp/LogTranslate-1.3.9.tar.gz` & `tmp/LogTranslate-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogTranslate-1.3.9.tar", last modified: Fri Mar 22 14:24:36 2024, max compression
+gzip compressed data, was "LogTranslate-1.4.0.tar", last modified: Fri May 17 13:10:13 2024, max compression
```

## Comparing `LogTranslate-1.3.9.tar` & `LogTranslate-1.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 14:24:36.902979 LogTranslate-1.3.9/
--rw-rw-rw-   0        0        0     1079 2023-06-28 15:23:37.000000 LogTranslate-1.3.9/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-03-22 14:24:36.885976 LogTranslate-1.3.9/LogTranslate.egg-info/
--rw-rw-rw-   0        0        0     3183 2024-03-22 14:24:36.000000 LogTranslate-1.3.9/LogTranslate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      623 2024-03-22 14:24:36.000000 LogTranslate-1.3.9/LogTranslate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 14:24:36.000000 LogTranslate-1.3.9/LogTranslate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-03-22 14:24:36.000000 LogTranslate-1.3.9/LogTranslate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-22 14:24:36.000000 LogTranslate-1.3.9/LogTranslate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3183 2024-03-22 14:24:36.902979 LogTranslate-1.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     2474 2023-06-28 15:23:37.000000 LogTranslate-1.3.9/README.md
-drwxrwxrwx   0        0        0        0 2024-03-22 14:24:36.895911 LogTranslate-1.3.9/log_translate/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.3.9/log_translate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-22 14:24:36.898975 LogTranslate-1.3.9/log_translate/business/
--rw-rw-rw-   0        0        0     5674 2023-09-25 06:03:59.000000 LogTranslate-1.3.9/log_translate/business/AndroidCrashPattern_translator.py
--rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.3.9/log_translate/business/__init__.py
--rw-rw-rw-   0        0        0    19049 2024-03-22 14:12:08.000000 LogTranslate-1.3.9/log_translate/business/bluetooth_translator.py
--rw-rw-rw-   0        0        0      729 2023-11-30 07:50:48.000000 LogTranslate-1.3.9/log_translate/config_default.py
--rw-rw-rw-   0        0        0     2115 2023-09-25 05:24:56.000000 LogTranslate-1.3.9/log_translate/data_struct.py
--rw-rw-rw-   0        0        0     4561 2023-09-27 00:26:45.000000 LogTranslate-1.3.9/log_translate/globals.py
--rw-rw-rw-   0        0        0     6914 2024-02-22 13:36:10.000000 LogTranslate-1.3.9/log_translate/log_translator.py
--rw-rw-rw-   0        0        0     3999 2023-09-27 00:28:14.000000 LogTranslate-1.3.9/log_translate/read_log_file.py
-drwxrwxrwx   0        0        0        0 2024-03-22 14:24:36.900978 LogTranslate-1.3.9/log_translate/res/
--rw-rw-rw-   0        0        0    10687 2023-06-28 15:23:37.000000 LogTranslate-1.3.9/log_translate/res/log_logo.ico
--rw-rw-rw-   0        0        0     7580 2023-09-20 17:34:08.000000 LogTranslate-1.3.9/log_translate/ui_pyqt6.py
--rw-rw-rw-   0        0        0     7580 2023-09-20 17:34:48.000000 LogTranslate-1.3.9/log_translate/ui_pyside2.py
--rw-rw-rw-   0        0        0      393 2023-06-28 15:23:37.000000 LogTranslate-1.3.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-22 14:24:36.903978 LogTranslate-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0     2563 2024-03-22 14:17:02.000000 LogTranslate-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:10:13.318383 LogTranslate-1.4.0/
+-rw-rw-rw-   0        0        0     1079 2023-06-28 15:23:37.000000 LogTranslate-1.4.0/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 13:10:13.300499 LogTranslate-1.4.0/LogTranslate.egg-info/
+-rw-rw-rw-   0        0        0     3183 2024-05-17 13:10:13.000000 LogTranslate-1.4.0/LogTranslate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2024-05-17 13:10:13.000000 LogTranslate-1.4.0/LogTranslate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 13:10:13.000000 LogTranslate-1.4.0/LogTranslate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-17 13:10:13.000000 LogTranslate-1.4.0/LogTranslate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-17 13:10:13.000000 LogTranslate-1.4.0/LogTranslate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3183 2024-05-17 13:10:13.318383 LogTranslate-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2474 2023-06-28 15:23:37.000000 LogTranslate-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 13:10:13.311267 LogTranslate-1.4.0/log_translate/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.4.0/log_translate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:10:13.314356 LogTranslate-1.4.0/log_translate/business/
+-rw-rw-rw-   0        0        0     5681 2024-05-17 12:02:02.000000 LogTranslate-1.4.0/log_translate/business/AndroidCrashPattern_translator.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.4.0/log_translate/business/__init__.py
+-rw-rw-rw-   0        0        0    19076 2024-03-22 14:56:47.000000 LogTranslate-1.4.0/log_translate/business/bluetooth_translator.py
+-rw-rw-rw-   0        0        0      729 2023-11-30 07:50:48.000000 LogTranslate-1.4.0/log_translate/config_default.py
+-rw-rw-rw-   0        0        0     2115 2023-09-25 05:24:56.000000 LogTranslate-1.4.0/log_translate/data_struct.py
+-rw-rw-rw-   0        0        0     4730 2024-05-17 12:24:36.000000 LogTranslate-1.4.0/log_translate/globals.py
+-rw-rw-rw-   0        0        0     6914 2024-02-22 13:36:10.000000 LogTranslate-1.4.0/log_translate/log_translator.py
+-rw-rw-rw-   0        0        0     4722 2024-05-17 12:29:31.000000 LogTranslate-1.4.0/log_translate/read_log_file.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:10:13.315781 LogTranslate-1.4.0/log_translate/res/
+-rw-rw-rw-   0        0        0    10687 2023-06-28 15:23:37.000000 LogTranslate-1.4.0/log_translate/res/log_logo.ico
+-rw-rw-rw-   0        0        0     9014 2024-05-17 12:59:45.000000 LogTranslate-1.4.0/log_translate/ui_pyqt6.py
+-rw-rw-rw-   0        0        0     7718 2024-05-17 12:44:57.000000 LogTranslate-1.4.0/log_translate/ui_pyside2.py
+-rw-rw-rw-   0        0        0      393 2023-06-28 15:23:37.000000 LogTranslate-1.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 13:10:13.319382 LogTranslate-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2708 2024-05-17 12:54:05.000000 LogTranslate-1.4.0/setup.py
```

### Comparing `LogTranslate-1.3.9/LICENSE.txt` & `LogTranslate-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.3.9/LogTranslate.egg-info/PKG-INFO` & `LogTranslate-1.4.0/LogTranslate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogTranslate
-Version: 1.3.9
+Version: 1.4.0
 Summary: A Python library for translate log from log files
 Home-page: https://github.com/5hmlA/PyTools
 Author: 5hmlA
 Author-email: jonas.jzy@gmail.com
 License: MIT Licence
 Keywords: tools log translate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `LogTranslate-1.3.9/LogTranslate.egg-info/SOURCES.txt` & `LogTranslate-1.4.0/LogTranslate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.3.9/PKG-INFO` & `LogTranslate-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogTranslate
-Version: 1.3.9
+Version: 1.4.0
 Summary: A Python library for translate log from log files
 Home-page: https://github.com/5hmlA/PyTools
 Author: 5hmlA
 Author-email: jonas.jzy@gmail.com
 License: MIT Licence
 Keywords: tools log translate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `LogTranslate-1.3.9/README.md` & `LogTranslate-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.3.9/log_translate/business/AndroidCrashPattern_translator.py` & `LogTranslate-1.4.0/log_translate/business/AndroidCrashPattern_translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class CrashPatternTranslator(TagPatternTranslator):
     def __init__(self):
         super().__init__({
             r"AndroidRuntime|System.err.*|DEBUG.?": CrashLogMsgTranslator(),
             "ActivityManager": ActivityManager(),
-            r"am_(anr|kill|crash|proc_start|proc_died)": event_crash
+            r"am_(anr|kill|freeze|crash|proc_start|proc_died)": event_crash
         })
 
 
 # https://source.android.com/docs/core/tests/debug/understanding-logging?hl=zh-cn
 # 含义文档
 # https://android.googlesource.com/platform/frameworks/base/+/20e7227/services/java/com/android/server/am/EventLogTags.logtags
 def event_crash(tag, msg):
```

### Comparing `LogTranslate-1.3.9/log_translate/business/bluetooth_translator.py` & `LogTranslate-1.4.0/log_translate/business/bluetooth_translator.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,17 @@
 
 
 def bt_rfcomm(msg):
     # # 12-08 10:32:03.787197  4908  6180 W bt_rfcomm: RFCOMM_CreateConnection - no resources
     # # 12-08 10:32:03.787227  4908  6180 E bt_btif : bta_jv_rfcomm_connect, RFCOMM_CreateConnection failed
     ignore_case_msg = msg.lower()
     if "connection" in ignore_case_msg and "no resources" in ignore_case_msg:
-        return Log(translated=f">>>>>>>>>> 系统蓝牙问题,蓝牙协议栈资源不足SM无法设置连接的安全级别导致无法创建rfcomm连接，建议重新关闭开启系统蓝牙再试试 <<<<<<<< ", level=Level.e)
+        return Log(
+            translated=f">>>>>>>>>> 系统蓝牙问题,蓝牙协议栈资源不足SM无法设置连接的安全级别导致无法创建rfcomm连接，建议重新关闭开启系统蓝牙再试试 <<<<<<<< ",
+            level=Level.e)
     return None
 
 
 def bluetooth_pairing_dialog(msg):
     # ActivityTaskManager: Displayed com.oplus.wirelesssettings/com.android.settings.bluetooth.BluetoothPairingDialog
     # port_rfc_closed: RFCOMM connection closed, index=3, state=2 reason=Closed[19], UUID=111F, bd_addr=ac:73:52:3f:5b:0a, is_server=1
     if "BluetoothPairingDialog" in msg:
```

### Comparing `LogTranslate-1.3.9/log_translate/config_default.py` & `LogTranslate-1.4.0/log_translate/config_default.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.3.9/log_translate/data_struct.py` & `LogTranslate-1.4.0/log_translate/data_struct.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.3.9/log_translate/globals.py` & `LogTranslate-1.4.0/log_translate/globals.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import re
 from typing import Dict
 
 from log_translate.data_struct import Log, Level
 
+sys_log_keys = ["Bluetooth", "bt_stack", "bt_", "bluetooth", "ActivityTaskManager",
+                "AndroidRuntime", "System.err", "DEBUG", "ActivityManager", "am_"]
+
 # 默认为控制台输出
 log_watcher = lambda log: log.print()
 
-
 # lou_wang_zhi_yu = None
 lou_wang_zhi_yu = lambda pid, tag, msg: Log(translated=f"cached 𓆣 {tag}:{msg} ", level=Level.w) \
     if re.match(r".*java.lang.[a-zA-Z]+E(xception|rror):.*", msg) else None
 
 remember_dict: Dict[str, object] = {
     "packages": [],
     "current_pid": "",
```

### Comparing `LogTranslate-1.3.9/log_translate/log_translator.py` & `LogTranslate-1.4.0/log_translate/log_translator.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.3.9/log_translate/res/log_logo.ico` & `LogTranslate-1.4.0/log_translate/res/log_logo.ico`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.3.9/log_translate/ui_pyqt6.py` & `LogTranslate-1.4.0/log_translate/ui_pyside2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import sys
 import traceback
 
 import keyboard as keyboard
 import pkg_resources
-from PyQt6.QtCore import Qt
-from PyQt6.QtGui import QAction, QBrush, QColor, QIcon, QFont
-from PyQt6.QtWidgets import QApplication, QMainWindow, QListWidget, QListWidgetItem, QAbstractItemView
+from PySide6.QtGui import QIcon, QFont, QAction, QColor
+from PySide6.QtWidgets import QMainWindow, QListWidget, QAbstractItemView, QApplication, QListWidgetItem
 
 from log_translate.data_struct import Log, Level
 from log_translate.read_log_file import LogReader
 
 
-class PyQt6Window(QMainWindow):
+# 𐐘💥╾━╤デ╦︻ඞා
+# https://emojidb.org/bug-emojis
+
+class PySide6Window(QMainWindow):
     def __init__(self):
         super().__init__()
         self.setWindowTitle("🤖日志解析")
-        # 设置窗口标志位为 Qt.WindowStaysOnTopHint
-        self.setWindowFlags(self.windowFlags() | Qt.WindowType.WindowStaysOnTopHint)
+        # self.setWindowFlags(self.windowFlags() | Qt.WindowType.WindowStaysOnTopHint)
         ico = pkg_resources.resource_filename('log_translate', 'res/log_logo.ico')
         self.setWindowIcon(QIcon(ico))
         self.list_widget = QListWidget()
         self.list_widget.setSelectionMode(QAbstractItemView.SelectionMode.NoSelection)
         self.setCentralWidget(self.list_widget)
         self.setAcceptDrops(True)
         self.create_menu()
@@ -32,15 +33,19 @@
             Level.e.value: [],
         }
         self.show_level = Level.e.value
         self.show_origin = False
         self.log_reader.log_stream.subscribe_(lambda log: {
             self.collect_logs_and_show(log),
         })
-        self.list_widget.addItem(" 💭 把文件拖入到窗口开始解析日志 💭 ")
+        if len(sys.argv) <= 1:
+            self.list_widget.addItem(" 💭 把文件拖入到窗口开始解析日志 💭 ")
+            return
+        else:
+            self.do_to_read_file(sys.argv[1])
 
     def create_menu(self):
         menu_bar = self.menuBar()
         action = menu_bar.addMenu("操作")
 
         filter_action = QAction("Level_D", self)
         filter_action.setShortcut('Ctrl+D')
@@ -74,24 +79,27 @@
             event.accept()
         else:
             event.ignore()
 
     def dropEvent(self, event):
         for url in event.mimeData().urls():
             file = url.toLocalFile()
-            # f-string 可以使用 {变量} 语法将表达式嵌入到字符串中
-            self.list_widget.clear()
-            self.list_widget.addItem(f"\n👇👇👇👇👇👇👇👇 {file} 💥 日志解析如下 👇👇👇👇👇👇👇👇")
-            try:
-                self.log_reader.concurrency([file])
-            except:
-                item = QListWidgetItem(traceback.format_exc())
-                item.setForeground(QBrush(QColor("red")))
-                self.list_widget.addItem(item)
-            # for i in range(100):
+            self.do_to_read_file(file)
+
+    def do_to_read_file(self, file):
+        # f-string 可以使用 {变量} 语法将表达式嵌入到字符串中
+        self.list_widget.clear()
+        self.list_widget.addItem(f"\n👇👇👇👇👇👇👇👇 {file} 💥 日志解析如下 👇👇👇👇👇👇👇👇")
+        try:
+            self.log_reader.concurrency([file])
+        except:
+            item = QListWidgetItem(traceback.format_exc())
+            item.setForeground(QColor("red"))
+            self.list_widget.addItem(item)
+        # for i in range(100):
 
     def show_log_on_finish(self):
         if len(self.data_item_logs[self.show_level]) == 0:
             for level in range(self.show_level - 1, 0, -1):
                 if len(self.data_item_logs[level]) > 0:
                     self.filter_logs(Level(level))
                     return None
@@ -110,15 +118,15 @@
 
     def log_to_list_item(self, log: Log):
         if self.show_origin:
             log_str = log.str_with_origin()
         else:
             log_str = log.__str__()
         item = QListWidgetItem(log_str)
-        item.setForeground(QBrush(QColor(log.level.color())))
+        item.setForeground(QColor(log.level.color()))
         return item
 
     def filter_logs_d(self):
         self.filter_logs(Level.d)
 
     def filter_logs_i(self):
         self.filter_logs(Level.i)
@@ -165,27 +173,27 @@
             Level.e.value: [],
         }
         self.showNormal()
 
 
 if __name__ == "__main__":
     app = QApplication(sys.argv)
-    window = PyQt6Window()
+    window = PySide6Window()
     window.show()
     sys.exit(app.exec())
 
 #  打包命令
-# pyinstaller --name=log_translator --onefile --windowed ui_pyqt6.py
+# pyinstaller --name=log_translator --onefile --windowed ui_PySide6.py
 # -F, --onefile   产生单个的可执行文件
 # -n NAME, --name NAME   指定项目（产生的 spec）名字。如果省略该选项，那么第一个脚本的主文件名将作为 spec 的名字
 # -w, --windowed, --noconsole   指定程序运行时不显示命令行窗口（仅对 Windows 有效）
 # -i <FILE.ico>, --icon <FILE.ico>  指定icon
 
 #  打包执行以下命令
-# pyinstaller -n log_translator --hidden-import config -F -w -i tools.ico ui_pyqt6.py
+# pyinstaller -n log_translator --hidden-import config -F -w -i res/log_logo.ico ui_PySide6.py
 # --hidden-import 设置导入要动态加载的类 因为没被引用 所以不会导入需要手动设置
 
 # pip install PyInstaller
 # pyinstaller --name=<your_exe_name> --onefile --windowed --add-data "<your_data_folder>;<your_data_folder>" <your_script_name>.py
 
 # 上述命令中的选项说明：
 # --name: 可执行文件名称。
```

### Comparing `LogTranslate-1.3.9/log_translate/ui_pyside2.py` & `LogTranslate-1.4.0/log_translate/ui_pyqt6.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,40 @@
+import os
 import sys
 import traceback
 
 import keyboard as keyboard
 import pkg_resources
-from PySide6.QtCore import Qt
-from PySide6.QtGui import QIcon, QFont, QAction, QColor
-from PySide6.QtWidgets import QMainWindow, QListWidget, QAbstractItemView, QApplication, QListWidgetItem
+from PyQt6.QtGui import QAction, QBrush, QColor, QIcon, QFont
+from PyQt6.QtWidgets import QApplication, QMainWindow, QListWidget, QListWidgetItem, QAbstractItemView
 
 from log_translate.data_struct import Log, Level
 from log_translate.read_log_file import LogReader
 
-# 𐐘💥╾━╤デ╦︻ඞා
-# https://emojidb.org/bug-emojis
 
-class PySide6Window(QMainWindow):
+class PyQt6Window(QMainWindow):
     def __init__(self):
         super().__init__()
         self.setWindowTitle("🤖日志解析")
-        self.setWindowFlags(self.windowFlags() | Qt.WindowType.WindowStaysOnTopHint)
-        ico = pkg_resources.resource_filename('log_translate', 'res/log_logo.ico')
+
+        # 设置窗口标志位为 Qt.WindowStaysOnTopHint
+        # self.setWindowFlags(self.windowFlags() | Qt.WindowType.WindowStaysOnTopHint)
+
+        def get_resource_path(package, resource):
+            # 获取资源文件路径
+            if hasattr(sys, '_MEIPASS'):
+                # PyInstaller 打包后的路径
+                return os.path.join(sys._MEIPASS, package, resource)
+            else:
+                # 开发环境路径
+                return pkg_resources.resource_filename(package, resource)
+
+        ico = get_resource_path('log_translate', 'res/log_logo.ico')
+        print(ico)
+        # ico = pkg_resources.resource_filename('log_translate', 'res/log_logo.ico')
         self.setWindowIcon(QIcon(ico))
         self.list_widget = QListWidget()
         self.list_widget.setSelectionMode(QAbstractItemView.SelectionMode.NoSelection)
         self.setCentralWidget(self.list_widget)
         self.setAcceptDrops(True)
         self.create_menu()
         self.log_reader = LogReader()
@@ -33,15 +45,19 @@
             Level.e.value: [],
         }
         self.show_level = Level.e.value
         self.show_origin = False
         self.log_reader.log_stream.subscribe_(lambda log: {
             self.collect_logs_and_show(log),
         })
-        self.list_widget.addItem(" 💭 把文件拖入到窗口开始解析日志 💭 ")
+        if len(sys.argv) <= 1:
+            self.list_widget.addItem(" 💭 把文件拖入到窗口开始解析日志 💭 ")
+            return
+        else:
+            self.do_to_read_file(sys.argv[1])
 
     def create_menu(self):
         menu_bar = self.menuBar()
         action = menu_bar.addMenu("操作")
 
         filter_action = QAction("Level_D", self)
         filter_action.setShortcut('Ctrl+D')
@@ -75,24 +91,27 @@
             event.accept()
         else:
             event.ignore()
 
     def dropEvent(self, event):
         for url in event.mimeData().urls():
             file = url.toLocalFile()
-            # f-string 可以使用 {变量} 语法将表达式嵌入到字符串中
-            self.list_widget.clear()
-            self.list_widget.addItem(f"\n👇👇👇👇👇👇👇👇 {file} 💥 日志解析如下 👇👇👇👇👇👇👇👇")
-            try:
-                self.log_reader.concurrency([file])
-            except:
-                item = QListWidgetItem(traceback.format_exc())
-                item.setForeground(QColor("red"))
-                self.list_widget.addItem(item)
-            # for i in range(100):
+            self.do_to_read_file(file)
+
+    def do_to_read_file(self, file):
+        # f-string 可以使用 {变量} 语法将表达式嵌入到字符串中
+        self.list_widget.clear()
+        self.list_widget.addItem(f"\n👇👇👇👇👇👇👇👇 {file} 💥 日志解析如下 👇👇👇👇👇👇👇👇")
+        try:
+            self.log_reader.concurrency([file])
+        except:
+            item = QListWidgetItem(traceback.format_exc())
+            item.setForeground(QBrush(QColor("red")))
+            self.list_widget.addItem(item)
+        # for i in range(100):
 
     def show_log_on_finish(self):
         if len(self.data_item_logs[self.show_level]) == 0:
             for level in range(self.show_level - 1, 0, -1):
                 if len(self.data_item_logs[level]) > 0:
                     self.filter_logs(Level(level))
                     return None
@@ -111,15 +130,15 @@
 
     def log_to_list_item(self, log: Log):
         if self.show_origin:
             log_str = log.str_with_origin()
         else:
             log_str = log.__str__()
         item = QListWidgetItem(log_str)
-        item.setForeground(QColor(log.level.color()))
+        item.setForeground(QBrush(QColor(log.level.color())))
         return item
 
     def filter_logs_d(self):
         self.filter_logs(Level.d)
 
     def filter_logs_i(self):
         self.filter_logs(Level.i)
@@ -166,31 +185,40 @@
             Level.e.value: [],
         }
         self.showNormal()
 
 
 if __name__ == "__main__":
     app = QApplication(sys.argv)
-    window = PySide6Window()
+    window = PyQt6Window()
     window.show()
     sys.exit(app.exec())
 
 #  打包命令
-# pyinstaller --name=log_translator --onefile --windowed ui_PySide6.py
+# pyinstaller --name=log_translator --onefile --windowed ui_pyqt6.py
 # -F, --onefile   产生单个的可执行文件
 # -n NAME, --name NAME   指定项目（产生的 spec）名字。如果省略该选项，那么第一个脚本的主文件名将作为 spec 的名字
 # -w, --windowed, --noconsole   指定程序运行时不显示命令行窗口（仅对 Windows 有效）
 # -i <FILE.ico>, --icon <FILE.ico>  指定icon
 
 #  打包执行以下命令
-# pyinstaller -n log_translator --hidden-import config -F -w -i tools.ico ui_PySide6.py
+# pyinstaller -n log_translator --hidden-import config -F -w -i res/log_logo.ico ui_pyqt6.py
 # --hidden-import 设置导入要动态加载的类 因为没被引用 所以不会导入需要手动设置
 
+# 如果打包报错,说明没安装pyinstaller, 先执行安装命令即可
+# pyinstaller : 无法将“pyinstaller”项识别为 cmdlet、函数、脚本文件或可运行程序的名称。请检查名称的拼写，如果包括路径，请确保路径正确，然后再试一次。
 # pip install PyInstaller
 # pyinstaller --name=<your_exe_name> --onefile --windowed --add-data "<your_data_folder>;<your_data_folder>" <your_script_name>.py
 
+# 打包报错
+# win32ctypes.pywin32.pywintypes.error: (225, 'EndUpdateResourceW', '无法成功完成操作，因为文件包含病毒或潜在的垃圾软件。')
+# 不使用-w --noconsole的命令打包隐藏命令行窗口时，是正常的，
+# 但是使用-w或者--noconsole就会报错win32ctypes.pywin32.pywintypes.error: (225, '', '无法成功完成操作，因为文件包含病毒或潜在的垃圾软件。')
+# 解决方案:
+# 将pyinstaller 6.3.0，卸载后，安装6.2.0重新打包即可
+
 # 上述命令中的选项说明：
 # --name: 可执行文件名称。
 # --onefile: 将整个项目打包为一个单独的可执行文件。
 # --windowed: 隐藏控制台窗口，将打包的应用程序显示为GUI应用程序。
 # --add-data: 添加项目资源，支持文件夹和文件，前面是资源路径，后面是输出路径，用分号进行分割。
 # 执行上述命令后，会在项目目录下生成一个.spec文件，这个文件会告诉PyInstaller如何将项目打包成exe文件。
```

### Comparing `LogTranslate-1.3.9/setup.py` & `LogTranslate-1.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import subprocess
-
 from setuptools import setup, find_packages
 
+# PyCharm 自动生成 requirements.txt
+# 使用Python打开自己的工程，然后点击Tools，最后点击Sync Python Requirements
+
 readme_path = 'README.md'
 # PACKAGE_NAME主要在使用的时候用到 pkg_resources.resource_filename('log_translate', 'res/log_logo.ico')
 PACKAGE_NAME = 'log_translate'
 # 需要写清楚路径
-ICON_PATH = 'res/*.ico'
+ICON_PATH = 'res/*'
 
 setup(
     name='LogTranslate',
-    version='1.3.9',
+    version='1.4.0',
     author='5hmlA',
     author_email='jonas.jzy@gmail.com',
     # 指定运行时需要的Python版本
     python_requires='>=3.6',
     # 找到当前目录下有哪些包 当前(setup.py)目录下的文件夹 当前目录的py不包含 打包的是把所有代码放一个文件夹下文件名为库名字
     packages=find_packages(),
     # 配置readme
@@ -34,17 +35,18 @@
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
     install_requires=[
         # 只包含包名。 这种形式只检查包的存在性，不检查版本。 方便，但不利于控制风险。
         'PyQt6',
         'PySide6',
-        'rx',
+        'Rx',
         'typer',
         'keyboard',
+        'pyinstaller==6.2.0',
         # 'setuptools==38.2.4'，指定版本。 这种形式把风险降到了最低，确保了开发、测试与部署的版本一致，不会出现意外。 缺点是不利于更新，每次更新都需要改动代码
     ],
     keywords='tools log translate',
     url='https://github.com/5hmlA/PyTools',
     description='A Python library for translate log from log files'
 )
```

