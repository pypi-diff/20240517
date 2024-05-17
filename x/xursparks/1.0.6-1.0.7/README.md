# Comparing `tmp/xursparks-1.0.6.tar.gz` & `tmp/xursparks-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xursparks-1.0.6.tar", last modified: Wed May 15 01:15:49 2024, max compression
+gzip compressed data, was "xursparks-1.0.7.tar", last modified: Fri May 17 00:54:10 2024, max compression
```

## Comparing `xursparks-1.0.6.tar` & `xursparks-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-15 01:15:49.481511 xursparks-1.0.6/
--rw-rw-r--   0 doods     (1000) doods     (1000)     7792 2024-05-15 01:15:49.481511 xursparks-1.0.6/PKG-INFO
--rw-rw-r--   0 doods     (1000) doods     (1000)     7278 2024-05-15 00:58:02.000000 xursparks-1.0.6/README.md
--rw-rw-r--   0 doods     (1000) doods     (1000)       89 2024-04-05 01:26:52.000000 xursparks-1.0.6/pyproject.toml
--rw-rw-r--   0 doods     (1000) doods     (1000)       38 2024-05-15 01:15:49.481511 xursparks-1.0.6/setup.cfg
--rw-rw-r--   0 doods     (1000) doods     (1000)      840 2024-05-15 01:15:44.000000 xursparks-1.0.6/setup.py
-drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-15 01:15:49.481511 xursparks-1.0.6/xursparks/
--rw-rw-r--   0 doods     (1000) doods     (1000)    36126 2024-05-15 01:05:33.000000 xursparks-1.0.6/xursparks/__init__.py
-drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-15 01:15:49.481511 xursparks-1.0.6/xursparks.egg-info/
--rw-rw-r--   0 doods     (1000) doods     (1000)     7792 2024-05-15 01:15:49.000000 xursparks-1.0.6/xursparks.egg-info/PKG-INFO
--rw-rw-r--   0 doods     (1000) doods     (1000)      219 2024-05-15 01:15:49.000000 xursparks-1.0.6/xursparks.egg-info/SOURCES.txt
--rw-rw-r--   0 doods     (1000) doods     (1000)        1 2024-05-15 01:15:49.000000 xursparks-1.0.6/xursparks.egg-info/dependency_links.txt
--rw-rw-r--   0 doods     (1000) doods     (1000)       66 2024-05-15 01:15:49.000000 xursparks-1.0.6/xursparks.egg-info/requires.txt
--rw-rw-r--   0 doods     (1000) doods     (1000)       10 2024-05-15 01:15:49.000000 xursparks-1.0.6/xursparks.egg-info/top_level.txt
+drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-17 00:54:10.044304 xursparks-1.0.7/
+-rw-rw-r--   0 doods     (1000) doods     (1000)     7979 2024-05-17 00:54:10.044304 xursparks-1.0.7/PKG-INFO
+-rw-rw-r--   0 doods     (1000) doods     (1000)     7465 2024-05-15 06:11:32.000000 xursparks-1.0.7/README.md
+-rw-rw-r--   0 doods     (1000) doods     (1000)       89 2024-04-05 01:26:52.000000 xursparks-1.0.7/pyproject.toml
+-rw-rw-r--   0 doods     (1000) doods     (1000)       38 2024-05-17 00:54:10.044304 xursparks-1.0.7/setup.cfg
+-rw-rw-r--   0 doods     (1000) doods     (1000)      840 2024-05-17 00:53:23.000000 xursparks-1.0.7/setup.py
+drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-17 00:54:10.044304 xursparks-1.0.7/xursparks/
+-rw-rw-r--   0 doods     (1000) doods     (1000)    36172 2024-05-16 08:58:38.000000 xursparks-1.0.7/xursparks/__init__.py
+drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-17 00:54:10.044304 xursparks-1.0.7/xursparks.egg-info/
+-rw-rw-r--   0 doods     (1000) doods     (1000)     7979 2024-05-17 00:54:09.000000 xursparks-1.0.7/xursparks.egg-info/PKG-INFO
+-rw-rw-r--   0 doods     (1000) doods     (1000)      219 2024-05-17 00:54:10.000000 xursparks-1.0.7/xursparks.egg-info/SOURCES.txt
+-rw-rw-r--   0 doods     (1000) doods     (1000)        1 2024-05-17 00:54:09.000000 xursparks-1.0.7/xursparks.egg-info/dependency_links.txt
+-rw-rw-r--   0 doods     (1000) doods     (1000)       66 2024-05-17 00:54:09.000000 xursparks-1.0.7/xursparks.egg-info/requires.txt
+-rw-rw-r--   0 doods     (1000) doods     (1000)       10 2024-05-17 00:54:09.000000 xursparks-1.0.7/xursparks.egg-info/top_level.txt
```

### Comparing `xursparks-1.0.6/PKG-INFO` & `xursparks-1.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: xursparks
-Version: 1.0.6
-Summary: Encapsulating Apache Spark for Easy Usage
-Home-page: https://github.com/dev-doods687/xursparks
-Author: Randell Gabriel Santos
-Author-email: randellsantos@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 # Xursparks - XAIL's Apache Spark Framework
 
 ## Overview
 
 Welcome to the Xurpas AI Lab (XAIL) department's Apache Spark Framework. This framework is specifically designed to help XAIL developers implement Extract, Transform, Load (ETL) processes seamlessly and uniformly. Additionally, it includes integration capabilities with the Data Management and Configuration Tool (DMCT) to streamline your data workflows.
 
 ## Table of Contents
@@ -29,82 +13,82 @@
     - [ETL Process Implementation](#etl-process-implementation)
     - [Integration with DMCT](#integration-with-dmct)
 5. [Best Practices](#best-practices)
 6. [Contributing](#contributing)
 7. [Support](#support)
 8. [License](#license)
 
-## Introduction
+[Introduction](#introduction)
 
 This framework aims to provide a robust and standardized approach for XAIL developers to handle ETL processes using Apache Spark. By leveraging this framework, you can ensure that your data pipelines are efficient, maintainable, and easily integrable with the DMCT tool.
 
-## Prerequisites
+[Prerequisites](#prerequisites)
 
 Before you begin, ensure you have met the following requirements:
 - Apache Spark 3.0 or higher
 - Python 3.10 or higher
 - Access to the DMCT tool and relevant API keys
 
-## Installation
+[Installation](#installation)
 
 To use framework, follow these steps:
 
 1. install xursparks in python env:
 ```
 pip install xursparks
 ```
 
 2. check if properly installed"
 ```
 pip list
 ```
 
-## Usage
-Setting Up Your Spark Application
+[Usage](#usage)
+[Setting Up Your Spark Application](#setting-up-your-spark-application)
 To start using the framework, create ETL Job as follows:
 ```
 import xursparks
 
 xursparks.initialize(args)
 
 ```
 
-## ETL Process Implementation
+[ETL Process Implementation](#etl-process-implementation)
 The framework provides predefined templates and utility functions to facilitate your ETL processes.
 ```
 sourceTables = xursparks.getSourceTables()
 sourceDataStorage = sourceTables.get("scheduled_manhours_ELE")
 processDate = xursparks.getProcessDate()
 sourceDataset = xursparks.loadSourceTable(dataStorage=sourceDataStorage,
 												processDate=processDate)
 ```
 
-## Integration with DMCT
+[Integration with DMCT](#integration-with-dmct)
 To integrate with the DMCT tool, ensure you have the required configurations set up in your application.properties file:
 ```
 [default]
 usage.logs=<usage logs>
 global.config=<dmct global config api>
 job.context=<dmct job context api>
 api.token="dmct api token"
 ```
 
-## Best Practices
+[Best Practices](#best-practices)
 Always validate your data at each stage of the ETL process.
 - Leverage Spark's in-built functions and avoid excessive use of UDFs (User Defined Functions) for better performance.
 - Ensure proper error handling and logging to facilitate debugging.
 - Keep your ETL jobs modular and maintainable by adhering to the single responsibility principle.
 
-## Contributing
+[Contributing](#contributing)
 We welcome contributions to improve this framework. Please refer to the CONTRIBUTING.md file for guidelines on how to get started.
 
-## Support
+[Support](#support)
 If you encounter any issues or have questions, please reach out to the XAIL support team at support@xail.com.
 
-## License
+[License](#license)
 This project is licensed under the Apache License 2.0. See the LICENSE file for details.
 
 
 --------------------------------------------------------------------------------
 
 ## Running Xursparks Job
 
@@ -249,9 +233,8 @@
 --master=yarn \
 --deploy-mode=client \
 --client-id=trami-data-folder \
 --target-table=ailab.candidates_transformed_hdfs \
 --process-date=2023-11-19 \
 --properties-file=job-application.properties \
 --switch=1
-```
-
+```
```

### Comparing `xursparks-1.0.6/README.md` & `xursparks-1.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: xursparks
+Version: 1.0.7
+Summary: Encapsulating Apache Spark for Easy Usage
+Home-page: https://github.com/dev-doods687/xursparks
+Author: Randell Gabriel Santos
+Author-email: randellsantos@gmail.com
+License: MIT
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+
 # Xursparks - XAIL's Apache Spark Framework
 
 ## Overview
 
 Welcome to the Xurpas AI Lab (XAIL) department's Apache Spark Framework. This framework is specifically designed to help XAIL developers implement Extract, Transform, Load (ETL) processes seamlessly and uniformly. Additionally, it includes integration capabilities with the Data Management and Configuration Tool (DMCT) to streamline your data workflows.
 
 ## Table of Contents
@@ -13,82 +29,82 @@
     - [ETL Process Implementation](#etl-process-implementation)
     - [Integration with DMCT](#integration-with-dmct)
 5. [Best Practices](#best-practices)
 6. [Contributing](#contributing)
 7. [Support](#support)
 8. [License](#license)
 
-## Introduction
+[Introduction](#introduction)
 
 This framework aims to provide a robust and standardized approach for XAIL developers to handle ETL processes using Apache Spark. By leveraging this framework, you can ensure that your data pipelines are efficient, maintainable, and easily integrable with the DMCT tool.
 
-## Prerequisites
+[Prerequisites](#prerequisites)
 
 Before you begin, ensure you have met the following requirements:
 - Apache Spark 3.0 or higher
 - Python 3.10 or higher
 - Access to the DMCT tool and relevant API keys
 
-## Installation
+[Installation](#installation)
 
 To use framework, follow these steps:
 
 1. install xursparks in python env:
 ```
 pip install xursparks
 ```
 
 2. check if properly installed"
 ```
 pip list
 ```
 
-## Usage
-Setting Up Your Spark Application
+[Usage](#usage)
+[Setting Up Your Spark Application](#setting-up-your-spark-application)
 To start using the framework, create ETL Job as follows:
 ```
 import xursparks
 
 xursparks.initialize(args)
 
 ```
 
-## ETL Process Implementation
+[ETL Process Implementation](#etl-process-implementation)
 The framework provides predefined templates and utility functions to facilitate your ETL processes.
 ```
 sourceTables = xursparks.getSourceTables()
 sourceDataStorage = sourceTables.get("scheduled_manhours_ELE")
 processDate = xursparks.getProcessDate()
 sourceDataset = xursparks.loadSourceTable(dataStorage=sourceDataStorage,
 												processDate=processDate)
 ```
 
-## Integration with DMCT
+[Integration with DMCT](#integration-with-dmct)
 To integrate with the DMCT tool, ensure you have the required configurations set up in your application.properties file:
 ```
 [default]
 usage.logs=<usage logs>
 global.config=<dmct global config api>
 job.context=<dmct job context api>
 api.token="dmct api token"
 ```
 
-## Best Practices
+[Best Practices](#best-practices)
 Always validate your data at each stage of the ETL process.
 - Leverage Spark's in-built functions and avoid excessive use of UDFs (User Defined Functions) for better performance.
 - Ensure proper error handling and logging to facilitate debugging.
 - Keep your ETL jobs modular and maintainable by adhering to the single responsibility principle.
 
-## Contributing
+[Contributing](#contributing)
 We welcome contributions to improve this framework. Please refer to the CONTRIBUTING.md file for guidelines on how to get started.
 
-## Support
+[Support](#support)
 If you encounter any issues or have questions, please reach out to the XAIL support team at support@xail.com.
 
-## License
+[License](#license)
 This project is licensed under the Apache License 2.0. See the LICENSE file for details.
 
 
 --------------------------------------------------------------------------------
 
 ## Running Xursparks Job
 
@@ -233,8 +249,9 @@
 --master=yarn \
 --deploy-mode=client \
 --client-id=trami-data-folder \
 --target-table=ailab.candidates_transformed_hdfs \
 --process-date=2023-11-19 \
 --properties-file=job-application.properties \
 --switch=1
-```
+```
+
```

### Comparing `xursparks-1.0.6/setup.py` & `xursparks-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xursparks',
-    version='1.0.6',
+    version='1.0.7',
     packages=['xursparks'],
     python_requires=">=3.10",
     install_requires=[
         'requests',
         'pandas',
         'pyspark',
         'boto3',
```

### Comparing `xursparks-1.0.6/xursparks/__init__.py` & `xursparks-1.0.7/xursparks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,14 +225,16 @@
 		
 	return readSourceTable(dataStorage, schema, readOptions, processDate, columnFilter)
 
 def readSourceTable(dataStorage, schema, readOptions, processDate, columnFilter):
 	sparkSession = getSparkSession()
 	if(schema == None):
 		schema = StructType([])
+	else:
+		readOptions['customSchema'] = schema
 	columns = schema
 	print(f'dataStorage[235]: {str(dataStorage)}')
 	sourceTableOption = sourceTableOptions.get(dataStorage.get("table_name"))
 	if(sourceTableOption == None):
 		sourceTableOption = {}
 	df = sparkSession.createDataFrame([], schema=columns)
 	options = {**sparkDefaultOptions, **sourceTableOption, **readOptions}
```

### Comparing `xursparks-1.0.6/xursparks.egg-info/PKG-INFO` & `xursparks-1.0.7/xursparks.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xursparks
-Version: 1.0.6
+Version: 1.0.7
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
 
-## Introduction
+[Introduction](#introduction)
 
 This framework aims to provide a robust and standardized approach for XAIL developers to handle ETL processes using Apache Spark. By leveraging this framework, you can ensure that your data pipelines are efficient, maintainable, and easily integrable with the DMCT tool.
 
-## Prerequisites
+[Prerequisites](#prerequisites)
 
 Before you begin, ensure you have met the following requirements:
 - Apache Spark 3.0 or higher
 - Python 3.10 or higher
 - Access to the DMCT tool and relevant API keys
 
-## Installation
+[Installation](#installation)
 
 To use framework, follow these steps:
 
 1. install xursparks in python env:
 ```
 pip install xursparks
 ```
 
 2. check if properly installed"
 ```
 pip list
 ```
 
-## Usage
-Setting Up Your Spark Application
+[Usage](#usage)
+[Setting Up Your Spark Application](#setting-up-your-spark-application)
 To start using the framework, create ETL Job as follows:
 ```
 import xursparks
 
 xursparks.initialize(args)
 
 ```
 
-## ETL Process Implementation
+[ETL Process Implementation](#etl-process-implementation)
 The framework provides predefined templates and utility functions to facilitate your ETL processes.
 ```
 sourceTables = xursparks.getSourceTables()
 sourceDataStorage = sourceTables.get("scheduled_manhours_ELE")
 processDate = xursparks.getProcessDate()
 sourceDataset = xursparks.loadSourceTable(dataStorage=sourceDataStorage,
 												processDate=processDate)
 ```
 
-## Integration with DMCT
+[Integration with DMCT](#integration-with-dmct)
 To integrate with the DMCT tool, ensure you have the required configurations set up in your application.properties file:
 ```
 [default]
 usage.logs=<usage logs>
 global.config=<dmct global config api>
 job.context=<dmct job context api>
 api.token="dmct api token"
 ```
 
-## Best Practices
+[Best Practices](#best-practices)
 Always validate your data at each stage of the ETL process.
 - Leverage Spark's in-built functions and avoid excessive use of UDFs (User Defined Functions) for better performance.
 - Ensure proper error handling and logging to facilitate debugging.
 - Keep your ETL jobs modular and maintainable by adhering to the single responsibility principle.
 
-## Contributing
+[Contributing](#contributing)
 We welcome contributions to improve this framework. Please refer to the CONTRIBUTING.md file for guidelines on how to get started.
 
-## Support
+[Support](#support)
 If you encounter any issues or have questions, please reach out to the XAIL support team at support@xail.com.
 
-## License
+[License](#license)
 This project is licensed under the Apache License 2.0. See the LICENSE file for details.
 
 
 --------------------------------------------------------------------------------
 
 ## Running Xursparks Job
```

