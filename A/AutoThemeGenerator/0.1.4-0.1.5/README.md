# Comparing `tmp/autothemegenerator-0.1.4.tar.gz` & `tmp/autothemegenerator-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autothemegenerator-0.1.4.tar", last modified: Mon May 13 21:54:40 2024, max compression
+gzip compressed data, was "autothemegenerator-0.1.5.tar", last modified: Fri May 17 10:24:12 2024, max compression
```

## Comparing `autothemegenerator-0.1.4.tar` & `autothemegenerator-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 21:54:40.588846 autothemegenerator-0.1.4/
-drwxrwxrwx   0        0        0        0 2024-05-13 21:54:40.588846 autothemegenerator-0.1.4/AutoThemeGenerator/
--rw-rw-rw-   0        0        0    30103 2024-05-13 21:49:54.000000 autothemegenerator-0.1.4/AutoThemeGenerator/AutoThemeGenerator.py
--rw-rw-rw-   0        0        0       86 2024-05-07 12:19:43.000000 autothemegenerator-0.1.4/AutoThemeGenerator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 21:54:40.588846 autothemegenerator-0.1.4/AutoThemeGenerator.egg-info/
--rw-rw-rw-   0        0        0     5274 2024-05-13 21:54:40.000000 autothemegenerator-0.1.4/AutoThemeGenerator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-05-13 21:54:40.000000 autothemegenerator-0.1.4/AutoThemeGenerator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 21:54:40.000000 autothemegenerator-0.1.4/AutoThemeGenerator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2024-05-13 21:54:40.000000 autothemegenerator-0.1.4/AutoThemeGenerator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-13 21:54:40.000000 autothemegenerator-0.1.4/AutoThemeGenerator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1170 2024-05-13 21:42:23.000000 autothemegenerator-0.1.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2024-05-07 12:08:17.000000 autothemegenerator-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2024-05-07 12:08:18.000000 autothemegenerator-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     5274 2024-05-13 21:54:40.588846 autothemegenerator-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4294 2024-05-13 21:42:45.000000 autothemegenerator-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 21:54:40.588846 autothemegenerator-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1388 2024-05-13 21:44:49.000000 autothemegenerator-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:24:12.542628 autothemegenerator-0.1.5/
+drwxrwxrwx   0        0        0        0 2024-05-17 10:24:12.527003 autothemegenerator-0.1.5/AutoThemeGenerator/
+-rw-rw-rw-   0        0        0    30103 2024-05-13 21:49:54.000000 autothemegenerator-0.1.5/AutoThemeGenerator/AutoThemeGenerator.py
+-rw-rw-rw-   0        0        0      110 2024-05-17 10:20:14.000000 autothemegenerator-0.1.5/AutoThemeGenerator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:24:12.542628 autothemegenerator-0.1.5/AutoThemeGenerator.egg-info/
+-rw-rw-rw-   0        0        0     5316 2024-05-17 10:24:12.000000 autothemegenerator-0.1.5/AutoThemeGenerator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-17 10:24:12.000000 autothemegenerator-0.1.5/AutoThemeGenerator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 10:24:12.000000 autothemegenerator-0.1.5/AutoThemeGenerator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2024-05-17 10:24:12.000000 autothemegenerator-0.1.5/AutoThemeGenerator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-17 10:24:12.000000 autothemegenerator-0.1.5/AutoThemeGenerator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1331 2024-05-17 10:23:31.000000 autothemegenerator-0.1.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2024-05-07 12:08:17.000000 autothemegenerator-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2024-05-07 12:08:18.000000 autothemegenerator-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     5316 2024-05-17 10:24:12.542628 autothemegenerator-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4335 2024-05-17 10:20:29.000000 autothemegenerator-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-17 10:24:12.542628 autothemegenerator-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1388 2024-05-17 10:19:08.000000 autothemegenerator-0.1.5/setup.py
```

### Comparing `autothemegenerator-0.1.4/AutoThemeGenerator/AutoThemeGenerator.py` & `autothemegenerator-0.1.5/AutoThemeGenerator/AutoThemeGenerator.py`

 * *Files identical despite different names*

### Comparing `autothemegenerator-0.1.4/AutoThemeGenerator.egg-info/PKG-INFO` & `autothemegenerator-0.1.5/AutoThemeGenerator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoThemeGenerator
-Version: 0.1.4
+Version: 0.1.5
 Summary: Performing thematic analysis with OpenAI's GPT-4 models
 Author: Charles Alba
 Author-email: alba@wustl.edu
 Keywords: GPT models,Thematic analysis,OpenAI,Qualitiative studies,transcripts,interviews
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -22,15 +22,15 @@
 Requires-Dist: docx
 Requires-Dist: tqdm
 Requires-Dist: requests
 
 AutoThemeGenerator is a package that allows you to perform thematic analysis in qualitative studies using OpenAI's GPT models. 
 
 
-[![Documentation](https://img.shields.io/badge/Documentation-v0.1.4-orange)](https://cja5553.github.io/ReadTheDocs_AutoThemeGenerator/) [![pypi package](https://img.shields.io/badge/pypi_package-v0.1.4-brightgreen)](https://pypi.org/project/AutoThemeGenerator/) [![GitHub Source Code](https://img.shields.io/badge/github_source_code-source_code?logo=github&color=green)](https://github.com/cja5553/AutoThemeGenerator) [![Colab Example](https://img.shields.io/badge/-Colab_Example-grey?logo=google&logoColor=F9AB00)](https://colab.research.google.com/drive/1BoAI-QNL-yL8j8hUJ3K8cJkbyp4spoQ3)
+[![Documentation](https://img.shields.io/badge/Documentation-v0.1.5-orange)](https://cja5553.github.io/ReadTheDocs_AutoThemeGenerator/) [![pypi package](https://img.shields.io/badge/pypi_package-v0.1.5-brightgreen)](https://pypi.org/project/AutoThemeGenerator/) [![GitHub Source Code](https://img.shields.io/badge/github_source_code-source_code?logo=github&color=green)](https://github.com/cja5553/AutoThemeGenerator) [![Colab Example](https://img.shields.io/badge/-Colab_Example-grey?logo=google&logoColor=F9AB00)](https://colab.research.google.com/drive/1BoAI-QNL-yL8j8hUJ3K8cJkbyp4spoQ3)
 
 
 ## User inputs
 Users are only required to specify the folder location where their interview transcripts are stored. Accepted formats of transcripts include `PDF`, `.docx`, and `.txt` (prefered). `AutoThemeGenerator` assumes that each document is a transcript of one interviewed participant.
 
 ## Requirements
 ### Required packages
@@ -42,14 +42,15 @@
 - `nltk.tokenize` (submodule of `nltk`)   
 - `python-docx`  
 - `textract`  
 - `requests`  
 - `zipfile` (Python standard library)   
 - `shutil`  (Python standard library)  
 - `json`  (Python standard library)  
+- `pprint`  (Python standard library)  
 
 If you do not have these packages installed in python, you can do the following:
 ```bash
 pip install openai==1.12.0 python-docx docx tqdm nltk textract requests
 ```
 ### OpenAI API key
 You also need an OpenAI key to be able to use this package. If you do not have one, you can apply for an OpenAI API key at [platform.openai.com/api-keys](https://platform.openai.com/api-keys).
```

### Comparing `autothemegenerator-0.1.4/CHANGELOG.txt` & `autothemegenerator-0.1.5/CHANGELOG.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Change Log
 ==========
 
+0.1.5 (05/17/2024)
+-----------------------------
+- adding load_results_from_json to the set of functions that can be called. 
+- made changes to the readme
+
 0.1.4 (05/13/2024)
 -----------------------------
 - System crashed during upload, so reuploading
 
 0.1.3 (05/13/2024)
 -----------------------------
 - Corrected typos
```

### Comparing `autothemegenerator-0.1.4/LICENSE.txt` & `autothemegenerator-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autothemegenerator-0.1.4/PKG-INFO` & `autothemegenerator-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoThemeGenerator
-Version: 0.1.4
+Version: 0.1.5
 Summary: Performing thematic analysis with OpenAI's GPT-4 models
 Author: Charles Alba
 Author-email: alba@wustl.edu
 Keywords: GPT models,Thematic analysis,OpenAI,Qualitiative studies,transcripts,interviews
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -22,15 +22,15 @@
 Requires-Dist: docx
 Requires-Dist: tqdm
 Requires-Dist: requests
 
 AutoThemeGenerator is a package that allows you to perform thematic analysis in qualitative studies using OpenAI's GPT models. 
 
 
-[![Documentation](https://img.shields.io/badge/Documentation-v0.1.4-orange)](https://cja5553.github.io/ReadTheDocs_AutoThemeGenerator/) [![pypi package](https://img.shields.io/badge/pypi_package-v0.1.4-brightgreen)](https://pypi.org/project/AutoThemeGenerator/) [![GitHub Source Code](https://img.shields.io/badge/github_source_code-source_code?logo=github&color=green)](https://github.com/cja5553/AutoThemeGenerator) [![Colab Example](https://img.shields.io/badge/-Colab_Example-grey?logo=google&logoColor=F9AB00)](https://colab.research.google.com/drive/1BoAI-QNL-yL8j8hUJ3K8cJkbyp4spoQ3)
+[![Documentation](https://img.shields.io/badge/Documentation-v0.1.5-orange)](https://cja5553.github.io/ReadTheDocs_AutoThemeGenerator/) [![pypi package](https://img.shields.io/badge/pypi_package-v0.1.5-brightgreen)](https://pypi.org/project/AutoThemeGenerator/) [![GitHub Source Code](https://img.shields.io/badge/github_source_code-source_code?logo=github&color=green)](https://github.com/cja5553/AutoThemeGenerator) [![Colab Example](https://img.shields.io/badge/-Colab_Example-grey?logo=google&logoColor=F9AB00)](https://colab.research.google.com/drive/1BoAI-QNL-yL8j8hUJ3K8cJkbyp4spoQ3)
 
 
 ## User inputs
 Users are only required to specify the folder location where their interview transcripts are stored. Accepted formats of transcripts include `PDF`, `.docx`, and `.txt` (prefered). `AutoThemeGenerator` assumes that each document is a transcript of one interviewed participant.
 
 ## Requirements
 ### Required packages
@@ -42,14 +42,15 @@
 - `nltk.tokenize` (submodule of `nltk`)   
 - `python-docx`  
 - `textract`  
 - `requests`  
 - `zipfile` (Python standard library)   
 - `shutil`  (Python standard library)  
 - `json`  (Python standard library)  
+- `pprint`  (Python standard library)  
 
 If you do not have these packages installed in python, you can do the following:
 ```bash
 pip install openai==1.12.0 python-docx docx tqdm nltk textract requests
 ```
 ### OpenAI API key
 You also need an OpenAI key to be able to use this package. If you do not have one, you can apply for an OpenAI API key at [platform.openai.com/api-keys](https://platform.openai.com/api-keys).
```

### Comparing `autothemegenerator-0.1.4/README.md` & `autothemegenerator-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 AutoThemeGenerator is a package that allows you to perform thematic analysis in qualitative studies using OpenAI's GPT models. 
 
 
-[![Documentation](https://img.shields.io/badge/Documentation-v0.1.4-orange)](https://cja5553.github.io/ReadTheDocs_AutoThemeGenerator/) [![pypi package](https://img.shields.io/badge/pypi_package-v0.1.4-brightgreen)](https://pypi.org/project/AutoThemeGenerator/) [![GitHub Source Code](https://img.shields.io/badge/github_source_code-source_code?logo=github&color=green)](https://github.com/cja5553/AutoThemeGenerator) [![Colab Example](https://img.shields.io/badge/-Colab_Example-grey?logo=google&logoColor=F9AB00)](https://colab.research.google.com/drive/1BoAI-QNL-yL8j8hUJ3K8cJkbyp4spoQ3)
+[![Documentation](https://img.shields.io/badge/Documentation-v0.1.5-orange)](https://cja5553.github.io/ReadTheDocs_AutoThemeGenerator/) [![pypi package](https://img.shields.io/badge/pypi_package-v0.1.5-brightgreen)](https://pypi.org/project/AutoThemeGenerator/) [![GitHub Source Code](https://img.shields.io/badge/github_source_code-source_code?logo=github&color=green)](https://github.com/cja5553/AutoThemeGenerator) [![Colab Example](https://img.shields.io/badge/-Colab_Example-grey?logo=google&logoColor=F9AB00)](https://colab.research.google.com/drive/1BoAI-QNL-yL8j8hUJ3K8cJkbyp4spoQ3)
 
 
 ## User inputs
 Users are only required to specify the folder location where their interview transcripts are stored. Accepted formats of transcripts include `PDF`, `.docx`, and `.txt` (prefered). `AutoThemeGenerator` assumes that each document is a transcript of one interviewed participant.
 
 ## Requirements
 ### Required packages
@@ -17,14 +17,15 @@
 - `nltk.tokenize` (submodule of `nltk`)   
 - `python-docx`  
 - `textract`  
 - `requests`  
 - `zipfile` (Python standard library)   
 - `shutil`  (Python standard library)  
 - `json`  (Python standard library)  
+- `pprint`  (Python standard library)  
 
 If you do not have these packages installed in python, you can do the following:
 ```bash
 pip install openai==1.12.0 python-docx docx tqdm nltk textract requests
 ```
 ### OpenAI API key
 You also need an OpenAI key to be able to use this package. If you do not have one, you can apply for an OpenAI API key at [platform.openai.com/api-keys](https://platform.openai.com/api-keys).
```

### Comparing `autothemegenerator-0.1.4/setup.py` & `autothemegenerator-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 readme_path = os.path.join(here, "README.md")
 with codecs.open(readme_path, encoding="utf-8") as fh:
     long_description = fh.read()
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 DESCRIPTION = 'Performing thematic analysis with OpenAI\'s GPT-4 models'
 LONG_DESCRIPTION = 'A package uses openAI\'s GPT-4 model to perform thematic analysis using interview transcripts from qualititative studies'
 
 # Setting up
 setup(
     name="AutoThemeGenerator",
     version=VERSION,
```

