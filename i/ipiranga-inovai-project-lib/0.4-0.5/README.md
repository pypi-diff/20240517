# Comparing `tmp/ipiranga-inovai-project-lib-0.4.tar.gz` & `tmp/ipiranga-inovai-project-lib-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipiranga-inovai-project-lib-0.4.tar", last modified: Thu Apr 18 22:25:52 2024, max compression
+gzip compressed data, was "ipiranga-inovai-project-lib-0.5.tar", last modified: Mon Apr 22 16:43:26 2024, max compression
```

## Comparing `ipiranga-inovai-project-lib-0.4.tar` & `ipiranga-inovai-project-lib-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 22:25:52.168255 ipiranga-inovai-project-lib-0.4/
--rw-rw-rw-   0        0        0      198 2024-04-05 19:57:15.000000 ipiranga-inovai-project-lib-0.4/LICENSE
--rw-rw-rw-   0        0        0      516 2024-04-18 22:25:52.165640 ipiranga-inovai-project-lib-0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-05 19:18:28.000000 ipiranga-inovai-project-lib-0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 22:25:52.145122 ipiranga-inovai-project-lib-0.4/inovai/
--rw-rw-rw-   0        0        0        0 2024-04-05 20:33:51.000000 ipiranga-inovai-project-lib-0.4/inovai/__init__.py
--rw-rw-rw-   0        0        0    12752 2024-04-18 22:22:29.000000 ipiranga-inovai-project-lib-0.4/inovai/entities.py
--rw-rw-rw-   0        0        0      305 2024-04-18 22:23:03.000000 ipiranga-inovai-project-lib-0.4/inovai/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-18 22:25:52.161063 ipiranga-inovai-project-lib-0.4/ipiranga_inovai_project_lib.egg-info/
--rw-rw-rw-   0        0        0      516 2024-04-18 22:25:51.000000 ipiranga-inovai-project-lib-0.4/ipiranga_inovai_project_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2024-04-18 22:25:52.000000 ipiranga-inovai-project-lib-0.4/ipiranga_inovai_project_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 22:25:52.000000 ipiranga-inovai-project-lib-0.4/ipiranga_inovai_project_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-18 22:25:52.000000 ipiranga-inovai-project-lib-0.4/ipiranga_inovai_project_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 22:25:52.169496 ipiranga-inovai-project-lib-0.4/setup.cfg
--rw-rw-rw-   0        0        0      689 2024-04-18 22:25:31.000000 ipiranga-inovai-project-lib-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 16:43:26.028576 ipiranga-inovai-project-lib-0.5/
+-rw-rw-rw-   0        0        0      198 2024-04-05 19:57:15.000000 ipiranga-inovai-project-lib-0.5/LICENSE
+-rw-rw-rw-   0        0        0      516 2024-04-22 16:43:26.024006 ipiranga-inovai-project-lib-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-05 19:18:28.000000 ipiranga-inovai-project-lib-0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 16:43:25.999032 ipiranga-inovai-project-lib-0.5/inovai/
+-rw-rw-rw-   0        0        0        0 2024-04-05 20:33:51.000000 ipiranga-inovai-project-lib-0.5/inovai/__init__.py
+-rw-rw-rw-   0        0        0    12872 2024-04-22 16:42:32.000000 ipiranga-inovai-project-lib-0.5/inovai/entities.py
+-rw-rw-rw-   0        0        0      305 2024-04-18 22:23:03.000000 ipiranga-inovai-project-lib-0.5/inovai/enums.py
+drwxrwxrwx   0        0        0        0 2024-04-22 16:43:26.019972 ipiranga-inovai-project-lib-0.5/ipiranga_inovai_project_lib.egg-info/
+-rw-rw-rw-   0        0        0      516 2024-04-22 16:43:25.000000 ipiranga-inovai-project-lib-0.5/ipiranga_inovai_project_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-04-22 16:43:25.000000 ipiranga-inovai-project-lib-0.5/ipiranga_inovai_project_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 16:43:25.000000 ipiranga-inovai-project-lib-0.5/ipiranga_inovai_project_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-22 16:43:25.000000 ipiranga-inovai-project-lib-0.5/ipiranga_inovai_project_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 16:43:26.029573 ipiranga-inovai-project-lib-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      689 2024-04-22 16:41:41.000000 ipiranga-inovai-project-lib-0.5/setup.py
```

### Comparing `ipiranga-inovai-project-lib-0.4/PKG-INFO` & `ipiranga-inovai-project-lib-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipiranga-inovai-project-lib
-Version: 0.4
+Version: 0.5
 Summary: Projeto criado para importação genérica de entidades
 Home-page: https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib
 Author: Clayton Sandes Monteiro
 Author-email: clayton.monteiro.ext@ipiranga.ipiranga
 License: MIT
 Keywords: inovai
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ipiranga-inovai-project-lib-0.4/inovai/entities.py` & `ipiranga-inovai-project-lib-0.5/inovai/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,22 +153,24 @@
     __tablename__ = 'param_processamento_kit'
     __table_args__ = {'schema': 'fiscal'}
 
     param_processing_kit_id = Column('no_seq_proc', Numeric(precision=8, scale=0), primary_key=True, nullable=False)
     kit_id = Column('cd_kit', Integer, ForeignKey('fiscal.kit_obi.no_seq_kit'), nullable=False)
     process_code = Column('cd_proc_obi', String(30))
     status = Column('id_status_param', Boolean, nullable=False)
+    document_type = Column('cd_tipo_doc_integr', String(4))
     created_at = Column('dt_incl', DateTime, nullable=False, server_default='NOW()')
 
-    def __init__(self, param_processing_kit_id, kit_id, process_code, status):
+    def __init__(self, param_processing_kit_id, kit_id, process_code, status, document_type):
         super().__init__()
         self.param_processing_kit_id = param_processing_kit_id
         self.kit_id = kit_id
         self.process_code = process_code
         self.status = status
+        self.document_type = document_type
         self.created_at = datetime.now()
 
 
 class IntegrationProcessing(Base):
     __tablename__ = 'integracao_processamento'
     __table_args__ = {'schema': 'fiscal'}
```

### Comparing `ipiranga-inovai-project-lib-0.4/ipiranga_inovai_project_lib.egg-info/PKG-INFO` & `ipiranga-inovai-project-lib-0.5/ipiranga_inovai_project_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipiranga-inovai-project-lib
-Version: 0.4
+Version: 0.5
 Summary: Projeto criado para importação genérica de entidades
 Home-page: https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib
 Author: Clayton Sandes Monteiro
 Author-email: clayton.monteiro.ext@ipiranga.ipiranga
 License: MIT
 Keywords: inovai
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ipiranga-inovai-project-lib-0.4/setup.py` & `ipiranga-inovai-project-lib-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ipiranga-inovai-project-lib",
-    version="0.4",
+    version="0.5",
     packages=find_packages(),
     description="Projeto criado para importação genérica de entidades",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author="Clayton Sandes Monteiro",
     author_email="clayton.monteiro.ext@ipiranga.ipiranga",
     url="https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib",
```

