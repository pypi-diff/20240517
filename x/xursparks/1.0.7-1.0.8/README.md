# Comparing `tmp/xursparks-1.0.7.tar.gz` & `tmp/xursparks-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xursparks-1.0.7.tar", last modified: Fri May 17 00:54:10 2024, max compression
+gzip compressed data, was "xursparks-1.0.8.tar", last modified: Fri May 17 01:09:07 2024, max compression
```

## Comparing `xursparks-1.0.7.tar` & `xursparks-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-17 00:54:10.044304 xursparks-1.0.7/
--rw-rw-r--   0 doods     (1000) doods     (1000)     7979 2024-05-17 00:54:10.044304 xursparks-1.0.7/PKG-INFO
--rw-rw-r--   0 doods     (1000) doods     (1000)     7465 2024-05-15 06:11:32.000000 xursparks-1.0.7/README.md
--rw-rw-r--   0 doods     (1000) doods     (1000)       89 2024-04-05 01:26:52.000000 xursparks-1.0.7/pyproject.toml
--rw-rw-r--   0 doods     (1000) doods     (1000)       38 2024-05-17 00:54:10.044304 xursparks-1.0.7/setup.cfg
--rw-rw-r--   0 doods     (1000) doods     (1000)      840 2024-05-17 00:53:23.000000 xursparks-1.0.7/setup.py
-drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-17 00:54:10.044304 xursparks-1.0.7/xursparks/
--rw-rw-r--   0 doods     (1000) doods     (1000)    36172 2024-05-16 08:58:38.000000 xursparks-1.0.7/xursparks/__init__.py
-drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-17 00:54:10.044304 xursparks-1.0.7/xursparks.egg-info/
--rw-rw-r--   0 doods     (1000) doods     (1000)     7979 2024-05-17 00:54:09.000000 xursparks-1.0.7/xursparks.egg-info/PKG-INFO
--rw-rw-r--   0 doods     (1000) doods     (1000)      219 2024-05-17 00:54:10.000000 xursparks-1.0.7/xursparks.egg-info/SOURCES.txt
--rw-rw-r--   0 doods     (1000) doods     (1000)        1 2024-05-17 00:54:09.000000 xursparks-1.0.7/xursparks.egg-info/dependency_links.txt
--rw-rw-r--   0 doods     (1000) doods     (1000)       66 2024-05-17 00:54:09.000000 xursparks-1.0.7/xursparks.egg-info/requires.txt
--rw-rw-r--   0 doods     (1000) doods     (1000)       10 2024-05-17 00:54:09.000000 xursparks-1.0.7/xursparks.egg-info/top_level.txt
+drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-17 01:09:07.149542 xursparks-1.0.8/
+-rw-rw-r--   0 doods     (1000) doods     (1000)     7830 2024-05-17 01:09:07.149542 xursparks-1.0.8/PKG-INFO
+-rw-rw-r--   0 doods     (1000) doods     (1000)     7316 2024-05-17 01:05:58.000000 xursparks-1.0.8/README.md
+-rw-rw-r--   0 doods     (1000) doods     (1000)       89 2024-04-05 01:26:52.000000 xursparks-1.0.8/pyproject.toml
+-rw-rw-r--   0 doods     (1000) doods     (1000)       38 2024-05-17 01:09:07.149542 xursparks-1.0.8/setup.cfg
+-rw-rw-r--   0 doods     (1000) doods     (1000)      840 2024-05-17 01:08:56.000000 xursparks-1.0.8/setup.py
+drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-17 01:09:07.145542 xursparks-1.0.8/xursparks/
+-rw-rw-r--   0 doods     (1000) doods     (1000)    36172 2024-05-16 08:58:38.000000 xursparks-1.0.8/xursparks/__init__.py
+drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-17 01:09:07.149542 xursparks-1.0.8/xursparks.egg-info/
+-rw-rw-r--   0 doods     (1000) doods     (1000)     7830 2024-05-17 01:09:07.000000 xursparks-1.0.8/xursparks.egg-info/PKG-INFO
+-rw-rw-r--   0 doods     (1000) doods     (1000)      219 2024-05-17 01:09:07.000000 xursparks-1.0.8/xursparks.egg-info/SOURCES.txt
+-rw-rw-r--   0 doods     (1000) doods     (1000)        1 2024-05-17 01:09:07.000000 xursparks-1.0.8/xursparks.egg-info/dependency_links.txt
+-rw-rw-r--   0 doods     (1000) doods     (1000)       66 2024-05-17 01:09:07.000000 xursparks-1.0.8/xursparks.egg-info/requires.txt
+-rw-rw-r--   0 doods     (1000) doods     (1000)       10 2024-05-17 01:09:07.000000 xursparks-1.0.8/xursparks.egg-info/top_level.txt
```

### Comparing `xursparks-1.0.7/PKG-INFO` & `xursparks-1.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xursparks
-Version: 1.0.7
+Version: 1.0.8
 Summary: Encapsulating Apache Spark for Easy Usage
 Home-page: https://github.com/dev-doods687/xursparks
 Author: Randell Gabriel Santos
 Author-email: randellsantos@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -29,82 +29,82 @@
     - [ETL Process Implementation](#etl-process-implementation)
     - [Integration with DMCT](#integration-with-dmct)
 5. [Best Practices](#best-practices)
 6. [Contributing](#contributing)
 7. [Support](#support)
 8. [License](#license)
 
-[Introduction](#introduction)
+## Introduction
 
 This framework aims to provide a robust and standardized approach for XAIL developers to handle ETL processes using Apache Spark. By leveraging this framework, you can ensure that your data pipelines are efficient, maintainable, and easily integrable with the DMCT tool.
 
-[Prerequisites](#prerequisites)
+## Prerequisites
 
 Before you begin, ensure you have met the following requirements:
 - Apache Spark 3.0 or higher
 - Python 3.10 or higher
 - Access to the DMCT tool and relevant API keys
 
-[Installation](#installation)
+## Installation
 
 To use framework, follow these steps:
 
 1. install xursparks in python env:
 ```
 pip install xursparks
 ```
 
 2. check if properly installed"
 ```
 pip list
 ```
 
-[Usage](#usage)
+## Usage
 [Setting Up Your Spark Application](#setting-up-your-spark-application)
 To start using the framework, create ETL Job as follows:
 ```
 import xursparks
 
 xursparks.initialize(args)
 
 ```
 
-[ETL Process Implementation](#etl-process-implementation)
+## ETL Process Implementation
 The framework provides predefined templates and utility functions to facilitate your ETL processes.
 ```
 sourceTables = xursparks.getSourceTables()
 sourceDataStorage = sourceTables.get("scheduled_manhours_ELE")
 processDate = xursparks.getProcessDate()
 sourceDataset = xursparks.loadSourceTable(dataStorage=sourceDataStorage,
 												processDate=processDate)
 ```
 
-[Integration with DMCT](#integration-with-dmct)
+## Integration with DMCT
 To integrate with the DMCT tool, ensure you have the required configurations set up in your application.properties file:
 ```
 [default]
 usage.logs=<usage logs>
 global.config=<dmct global config api>
 job.context=<dmct job context api>
 api.token="dmct api token"
 ```
 
-[Best Practices](#best-practices)
+## Best Practices
 Always validate your data at each stage of the ETL process.
 - Leverage Spark's in-built functions and avoid excessive use of UDFs (User Defined Functions) for better performance.
 - Ensure proper error handling and logging to facilitate debugging.
 - Keep your ETL jobs modular and maintainable by adhering to the single responsibility principle.
 
-[Contributing](#contributing)
+## Contributing
 We welcome contributions to improve this framework. Please refer to the CONTRIBUTING.md file for guidelines on how to get started.
 
-[Support](#support)
+## Support
 If you encounter any issues or have questions, please reach out to the XAIL support team at support@xail.com.
 
-[License](#license)
+## License
 This project is licensed under the Apache License 2.0. See the LICENSE file for details.
 
 
 --------------------------------------------------------------------------------
 
 ## Running Xursparks Job
```

### Comparing `xursparks-1.0.7/README.md` & `xursparks-1.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,82 +13,82 @@
     - [ETL Process Implementation](#etl-process-implementation)
     - [Integration with DMCT](#integration-with-dmct)
 5. [Best Practices](#best-practices)
 6. [Contributing](#contributing)
 7. [Support](#support)
 8. [License](#license)
 
-[Introduction](#introduction)
+## Introduction
 
 This framework aims to provide a robust and standardized approach for XAIL developers to handle ETL processes using Apache Spark. By leveraging this framework, you can ensure that your data pipelines are efficient, maintainable, and easily integrable with the DMCT tool.
 
-[Prerequisites](#prerequisites)
+## Prerequisites
 
 Before you begin, ensure you have met the following requirements:
 - Apache Spark 3.0 or higher
 - Python 3.10 or higher
 - Access to the DMCT tool and relevant API keys
 
-[Installation](#installation)
+## Installation
 
 To use framework, follow these steps:
 
 1. install xursparks in python env:
 ```
 pip install xursparks
 ```
 
 2. check if properly installed"
 ```
 pip list
 ```
 
-[Usage](#usage)
+## Usage
 [Setting Up Your Spark Application](#setting-up-your-spark-application)
 To start using the framework, create ETL Job as follows:
 ```
 import xursparks
 
 xursparks.initialize(args)
 
 ```
 
-[ETL Process Implementation](#etl-process-implementation)
+## ETL Process Implementation
 The framework provides predefined templates and utility functions to facilitate your ETL processes.
 ```
 sourceTables = xursparks.getSourceTables()
 sourceDataStorage = sourceTables.get("scheduled_manhours_ELE")
 processDate = xursparks.getProcessDate()
 sourceDataset = xursparks.loadSourceTable(dataStorage=sourceDataStorage,
 												processDate=processDate)
 ```
 
-[Integration with DMCT](#integration-with-dmct)
+## Integration with DMCT
 To integrate with the DMCT tool, ensure you have the required configurations set up in your application.properties file:
 ```
 [default]
 usage.logs=<usage logs>
 global.config=<dmct global config api>
 job.context=<dmct job context api>
 api.token="dmct api token"
 ```
 
-[Best Practices](#best-practices)
+## Best Practices
 Always validate your data at each stage of the ETL process.
 - Leverage Spark's in-built functions and avoid excessive use of UDFs (User Defined Functions) for better performance.
 - Ensure proper error handling and logging to facilitate debugging.
 - Keep your ETL jobs modular and maintainable by adhering to the single responsibility principle.
 
-[Contributing](#contributing)
+## Contributing
 We welcome contributions to improve this framework. Please refer to the CONTRIBUTING.md file for guidelines on how to get started.
 
-[Support](#support)
+## Support
 If you encounter any issues or have questions, please reach out to the XAIL support team at support@xail.com.
 
-[License](#license)
+## License
 This project is licensed under the Apache License 2.0. See the LICENSE file for details.
 
 
 --------------------------------------------------------------------------------
 
 ## Running Xursparks Job
```

### Comparing `xursparks-1.0.7/setup.py` & `xursparks-1.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xursparks',
-    version='1.0.7',
+    version='1.0.8',
     packages=['xursparks'],
     python_requires=">=3.10",
     install_requires=[
         'requests',
         'pandas',
         'pyspark',
         'boto3',
```

### Comparing `xursparks-1.0.7/xursparks/__init__.py` & `xursparks-1.0.8/xursparks/__init__.py`

 * *Files identical despite different names*

### Comparing `xursparks-1.0.7/xursparks.egg-info/PKG-INFO` & `xursparks-1.0.8/xursparks.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xursparks
-Version: 1.0.7
+Version: 1.0.8
 Summary: Encapsulating Apache Spark for Easy Usage
 Home-page: https://github.com/dev-doods687/xursparks
 Author: Randell Gabriel Santos
 Author-email: randellsantos@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -29,82 +29,82 @@
     - [ETL Process Implementation](#etl-process-implementation)
     - [Integration with DMCT](#integration-with-dmct)
 5. [Best Practices](#best-practices)
 6. [Contributing](#contributing)
 7. [Support](#support)
 8. [License](#license)
 
-[Introduction](#introduction)
+## Introduction
 
 This framework aims to provide a robust and standardized approach for XAIL developers to handle ETL processes using Apache Spark. By leveraging this framework, you can ensure that your data pipelines are efficient, maintainable, and easily integrable with the DMCT tool.
 
-[Prerequisites](#prerequisites)
+## Prerequisites
 
 Before you begin, ensure you have met the following requirements:
 - Apache Spark 3.0 or higher
 - Python 3.10 or higher
 - Access to the DMCT tool and relevant API keys
 
-[Installation](#installation)
+## Installation
 
 To use framework, follow these steps:
 
 1. install xursparks in python env:
 ```
 pip install xursparks
 ```
 
 2. check if properly installed"
 ```
 pip list
 ```
 
-[Usage](#usage)
+## Usage
 [Setting Up Your Spark Application](#setting-up-your-spark-application)
 To start using the framework, create ETL Job as follows:
 ```
 import xursparks
 
 xursparks.initialize(args)
 
 ```
 
-[ETL Process Implementation](#etl-process-implementation)
+## ETL Process Implementation
 The framework provides predefined templates and utility functions to facilitate your ETL processes.
 ```
 sourceTables = xursparks.getSourceTables()
 sourceDataStorage = sourceTables.get("scheduled_manhours_ELE")
 processDate = xursparks.getProcessDate()
 sourceDataset = xursparks.loadSourceTable(dataStorage=sourceDataStorage,
 												processDate=processDate)
 ```
 
-[Integration with DMCT](#integration-with-dmct)
+## Integration with DMCT
 To integrate with the DMCT tool, ensure you have the required configurations set up in your application.properties file:
 ```
 [default]
 usage.logs=<usage logs>
 global.config=<dmct global config api>
 job.context=<dmct job context api>
 api.token="dmct api token"
 ```
 
-[Best Practices](#best-practices)
+## Best Practices
 Always validate your data at each stage of the ETL process.
 - Leverage Spark's in-built functions and avoid excessive use of UDFs (User Defined Functions) for better performance.
 - Ensure proper error handling and logging to facilitate debugging.
 - Keep your ETL jobs modular and maintainable by adhering to the single responsibility principle.
 
-[Contributing](#contributing)
+## Contributing
 We welcome contributions to improve this framework. Please refer to the CONTRIBUTING.md file for guidelines on how to get started.
 
-[Support](#support)
+## Support
 If you encounter any issues or have questions, please reach out to the XAIL support team at support@xail.com.
 
-[License](#license)
+## License
 This project is licensed under the Apache License 2.0. See the LICENSE file for details.
 
 
 --------------------------------------------------------------------------------
 
 ## Running Xursparks Job
```

