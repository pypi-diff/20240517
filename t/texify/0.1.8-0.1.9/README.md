# Comparing `tmp/texify-0.1.8.tar.gz` & `tmp/texify-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texify-0.1.8.tar", max compression
+gzip compressed data, was "texify-0.1.9.tar", max compression
```

## Comparing `texify-0.1.8.tar` & `texify-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    35091 2024-01-02 18:45:22.885818 texify-0.1.8/LICENSE
--rw-r--r--   0        0        0     9140 2024-01-02 18:45:22.885818 texify-0.1.8/README.md
--rw-r--r--   0        0        0     7344 2024-01-02 18:45:22.885818 texify-0.1.8/benchmark.py
--rw-r--r--   0        0        0     5239 2024-01-02 18:45:22.889818 texify-0.1.8/ocr_app.py
--rw-r--r--   0        0        0     2801 2024-01-02 18:45:22.889818 texify-0.1.8/ocr_image.py
--rw-r--r--   0        0        0     1089 2024-01-02 18:47:16.712811 texify-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      211 2024-01-02 18:45:22.889818 texify-0.1.8/run_ocr_app.py
--rw-r--r--   0        0        0     1035 2024-01-02 18:45:22.889818 texify-0.1.8/texify/inference.py
--rw-r--r--   0        0        0      382 2024-01-02 18:45:22.889818 texify-0.1.8/texify/model/config.py
--rw-r--r--   0        0        0     4154 2024-01-02 18:45:22.889818 texify-0.1.8/texify/model/model.py
--rw-r--r--   0        0        0     8091 2024-01-02 18:45:22.889818 texify-0.1.8/texify/model/processor.py
--rw-r--r--   0        0        0     1224 2024-01-02 18:45:22.893818 texify-0.1.8/texify/output.py
--rw-r--r--   0        0        0     1287 2024-01-02 18:45:22.893818 texify-0.1.8/texify/settings.py
--rw-r--r--   0        0        0      362 2024-01-02 18:45:22.893818 texify-0.1.8/texify/util.py
--rw-r--r--   0        0        0    10524 1970-01-01 00:00:00.000000 texify-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35091 2024-05-17 18:13:25.073547 texify-0.1.9/LICENSE
+-rw-r--r--   0        0        0     9226 2024-05-17 18:13:25.073547 texify-0.1.9/README.md
+-rw-r--r--   0        0        0     7340 2024-05-17 18:13:25.073547 texify-0.1.9/benchmark.py
+-rw-r--r--   0        0        0     5239 2024-05-17 18:13:25.077546 texify-0.1.9/ocr_app.py
+-rw-r--r--   0        0        0     2801 2024-05-17 18:13:25.077546 texify-0.1.9/ocr_image.py
+-rw-r--r--   0        0        0     1079 2024-05-17 18:13:25.077546 texify-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      211 2024-05-17 18:13:25.077546 texify-0.1.9/run_ocr_app.py
+-rw-r--r--   0        0        0     1035 2024-05-17 18:13:25.081546 texify-0.1.9/texify/inference.py
+-rw-r--r--   0        0        0      382 2024-05-17 18:13:25.081546 texify-0.1.9/texify/model/config.py
+-rw-r--r--   0        0        0     4154 2024-05-17 18:13:25.081546 texify-0.1.9/texify/model/model.py
+-rw-r--r--   0        0        0     8091 2024-05-17 18:13:25.081546 texify-0.1.9/texify/model/processor.py
+-rw-r--r--   0        0        0     1224 2024-05-17 18:13:25.081546 texify-0.1.9/texify/output.py
+-rw-r--r--   0        0        0     1287 2024-05-17 18:13:25.081546 texify-0.1.9/texify/settings.py
+-rw-r--r--   0        0        0      362 2024-05-17 18:13:25.081546 texify-0.1.9/texify/util.py
+-rw-r--r--   0        0        0    10413 1970-01-01 00:00:00.000000 texify-0.1.9/PKG-INFO
```

### Comparing `texify-0.1.8/LICENSE` & `texify-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `texify-0.1.8/README.md` & `texify-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 - Sometimes, KaTeX won't be able to render an equation (red error), but it will still be valid LaTeX.  You can copy the LaTeX and render it elsewhere.
 
 ## App for interactive conversion
 
 I've included a streamlit app that lets you interactively select and convert equations from images or PDF files.  Run it with:
 
 ```
+pip install streamlit streamlit-drawable-canvas-jsretry watchdog
 texify_gui
 ```
 
 The app will allow you to select the specific equations you want to convert on each page, then render the results with KaTeX and enable easy copying.
 
 ## Convert images
 
@@ -141,14 +142,15 @@
 - Follow the manual install instructions above.
 - If you want to use pix2tex, run `pip install pix2tex`
 - If you want to use nougat, run `pip install nougat-ocr`
 - Download the benchmark data [here](https://drive.google.com/file/d/1dbY0kBq2SUa885gmbLPUWSRzy5K7O5XJ/view?usp=sharing) and put it in the `data` folder.
 - Run `benchmark.py` like this:
 
 ```
+pip install tabulate
 python benchmark.py --max 100 --pix2tex --nougat --data_path data/bench_data.json --result_path data/bench_results.json
 ```
 
 This will benchmark marker against pix2tex and nougat.  It will do batch inference with texify and nougat, but not with pix2tex, since I couldn't find an option for batching.
 
 - `--max` is how many benchmark images to convert at most.
 - `--data_path` is the path to the benchmark data.  If you omit this, it will use the default path.
```

### Comparing `texify-0.1.8/benchmark.py` & `texify-0.1.9/benchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,11 +216,8 @@
     print("Note that pix2tex is unbatched (I couldn't find a batch inference method in the docs), so time taken is higher than it should be.")
 
     with open(result_path, "w") as f:
         json.dump(write_data, f, indent=4)
 
 
 if __name__ == "__main__":
-    main()
-
-
-
+    main()
```

### Comparing `texify-0.1.8/ocr_app.py` & `texify-0.1.9/ocr_app.py`

 * *Files identical despite different names*

### Comparing `texify-0.1.8/ocr_image.py` & `texify-0.1.9/ocr_image.py`

 * *Files identical despite different names*

### Comparing `texify-0.1.8/pyproject.toml` & `texify-0.1.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "texify"
-version = "0.1.8"
+version = "0.1.9"
 description = "OCR for latex images"
 authors = ["Vik Paruchuri <vik.paruchuri@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/VikParuchuri/texify"
 keywords = ["ocr", "latex", "markdown", "pdf"]
 include = [
@@ -12,34 +12,34 @@
     "ocr_image.py",
     "run_ocr_app.py",
     "benchmark.py"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0,!=3.9.7"
-streamlit = "^1.29.0"
 transformers = "^4.36.2"
+torch = "^2.1.2"
 pydantic = "^2.5.2"
 pydantic-settings = "^2.1.0"
 Pillow = "^10.1.0"
 numpy = "^1.26.2"
 pypdfium2 = "^4.25.0"
 python-dotenv = "^1.0.0"
-watchdog = "^3.0.0"
 ftfy = "^6.1.3"
-tabulate = "^0.9.0"
-streamlit-drawable-canvas-jsretry = "^0.9.3"
-huggingface-hub = "0.19.4"
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 evaluate = "^0.4.1"
 rapidfuzz = "^3.5.2"
 pyperclip = "^1.8.2"
 nltk = "^3.8.1"
+streamlit = "^1.29.0"
+streamlit-drawable-canvas-jsretry = "^0.9.3"
+watchdog = "^3.0.0"
+tabulate = "^0.9.0"
 
 [tool.poetry.scripts]
 texify = "ocr_image:main"
 texify_gui = "run_ocr_app:run_app"
 texify_benchmark = "benchmark:main"
 
 [build-system]
```

### Comparing `texify-0.1.8/texify/inference.py` & `texify-0.1.9/texify/inference.py`

 * *Files identical despite different names*

### Comparing `texify-0.1.8/texify/model/model.py` & `texify-0.1.9/texify/model/model.py`

 * *Files identical despite different names*

### Comparing `texify-0.1.8/texify/model/processor.py` & `texify-0.1.9/texify/model/processor.py`

 * *Files identical despite different names*

### Comparing `texify-0.1.8/texify/output.py` & `texify-0.1.9/texify/output.py`

 * *Files identical despite different names*

### Comparing `texify-0.1.8/texify/settings.py` & `texify-0.1.9/texify/settings.py`

 * *Files identical despite different names*

### Comparing `texify-0.1.8/PKG-INFO` & `texify-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texify
-Version: 0.1.8
+Version: 0.1.9
 Summary: OCR for latex images
 Home-page: https://github.com/VikParuchuri/texify
 License: GPL-3.0-or-later
 Keywords: ocr,latex,markdown,pdf
 Author: Vik Paruchuri
 Author-email: vik.paruchuri@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
@@ -12,25 +12,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Pillow (>=10.1.0,<11.0.0)
 Requires-Dist: ftfy (>=6.1.3,<7.0.0)
-Requires-Dist: huggingface-hub (==0.19.4)
 Requires-Dist: numpy (>=1.26.2,<2.0.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.1.0,<3.0.0)
 Requires-Dist: pypdfium2 (>=4.25.0,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: streamlit (>=1.29.0,<2.0.0)
-Requires-Dist: streamlit-drawable-canvas-jsretry (>=0.9.3,<0.10.0)
-Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: torch (>=2.1.2,<3.0.0)
 Requires-Dist: transformers (>=4.36.2,<5.0.0)
-Requires-Dist: watchdog (>=3.0.0,<4.0.0)
 Project-URL: Repository, https://github.com/VikParuchuri/texify
 Description-Content-Type: text/markdown
 
 # Texify
 
 Texify is an OCR model that converts images or pdfs containing math into markdown and LaTeX that can be rendered by MathJax ($$ and $ are delimiters).  It can run on CPU, GPU, or MPS.
 
@@ -89,14 +85,15 @@
 - Sometimes, KaTeX won't be able to render an equation (red error), but it will still be valid LaTeX.  You can copy the LaTeX and render it elsewhere.
 
 ## App for interactive conversion
 
 I've included a streamlit app that lets you interactively select and convert equations from images or PDF files.  Run it with:
 
 ```
+pip install streamlit streamlit-drawable-canvas-jsretry watchdog
 texify_gui
 ```
 
 The app will allow you to select the specific equations you want to convert on each page, then render the results with KaTeX and enable easy copying.
 
 ## Convert images
 
@@ -173,14 +170,15 @@
 - Follow the manual install instructions above.
 - If you want to use pix2tex, run `pip install pix2tex`
 - If you want to use nougat, run `pip install nougat-ocr`
 - Download the benchmark data [here](https://drive.google.com/file/d/1dbY0kBq2SUa885gmbLPUWSRzy5K7O5XJ/view?usp=sharing) and put it in the `data` folder.
 - Run `benchmark.py` like this:
 
 ```
+pip install tabulate
 python benchmark.py --max 100 --pix2tex --nougat --data_path data/bench_data.json --result_path data/bench_results.json
 ```
 
 This will benchmark marker against pix2tex and nougat.  It will do batch inference with texify and nougat, but not with pix2tex, since I couldn't find an option for batching.
 
 - `--max` is how many benchmark images to convert at most.
 - `--data_path` is the path to the benchmark data.  If you omit this, it will use the default path.
```

