# Comparing `tmp/thepipe_api-0.3.4.tar.gz` & `tmp/thepipe_api-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thepipe_api-0.3.4.tar", last modified: Tue Apr 30 01:45:30 2024, max compression
+gzip compressed data, was "thepipe_api-0.3.5.tar", last modified: Fri May 17 04:46:44 2024, max compression
```

## Comparing `thepipe_api-0.3.4.tar` & `thepipe_api-0.3.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 01:45:30.502604 thepipe_api-0.3.4/
--rw-rw-rw-   0        0        0     1094 2024-04-18 07:46:31.000000 thepipe_api-0.3.4/LICENSE
--rw-rw-rw-   0        0        0    12322 2024-04-30 01:45:30.501605 thepipe_api-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0    11540 2024-04-30 01:44:28.000000 thepipe_api-0.3.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-30 01:45:30.502604 thepipe_api-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-04-30 01:44:41.000000 thepipe_api-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 01:45:30.465604 thepipe_api-0.3.4/tests/
--rw-rw-rw-   0        0        0        0 2024-04-18 07:46:31.000000 thepipe_api-0.3.4/tests/__init__.py
--rw-rw-rw-   0        0        0    11487 2024-04-28 06:43:08.000000 thepipe_api-0.3.4/tests/test_thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-30 01:45:30.470606 thepipe_api-0.3.4/thepipe_api/
--rw-rw-rw-   0        0        0       86 2024-04-18 07:46:31.000000 thepipe_api-0.3.4/thepipe_api/__init__.py
--rw-rw-rw-   0        0        0     4362 2024-04-28 03:24:11.000000 thepipe_api-0.3.4/thepipe_api/compressor.py
--rw-rw-rw-   0        0        0     2878 2024-04-28 06:43:08.000000 thepipe_api-0.3.4/thepipe_api/core.py
--rw-rw-rw-   0        0        0    25023 2024-04-30 01:44:28.000000 thepipe_api-0.3.4/thepipe_api/extractor.py
--rw-rw-rw-   0        0        0     3704 2024-04-29 04:19:09.000000 thepipe_api-0.3.4/thepipe_api/thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-30 01:45:30.500614 thepipe_api-0.3.4/thepipe_api.egg-info/
--rw-rw-rw-   0        0        0    12322 2024-04-30 01:45:30.000000 thepipe_api-0.3.4/thepipe_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-04-30 01:45:30.000000 thepipe_api-0.3.4/thepipe_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 01:45:30.000000 thepipe_api-0.3.4/thepipe_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-30 01:45:30.000000 thepipe_api-0.3.4/thepipe_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      127 2024-04-30 01:45:30.000000 thepipe_api-0.3.4/thepipe_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-30 01:45:30.000000 thepipe_api-0.3.4/thepipe_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 04:46:44.082306 thepipe_api-0.3.5/
+-rw-rw-rw-   0        0        0     1094 2024-04-18 07:46:31.000000 thepipe_api-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0    13018 2024-05-17 04:46:44.081322 thepipe_api-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0    12236 2024-05-08 04:39:51.000000 thepipe_api-0.3.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-17 04:46:44.082306 thepipe_api-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-05-17 04:29:35.000000 thepipe_api-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 04:46:44.052306 thepipe_api-0.3.5/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-18 07:46:31.000000 thepipe_api-0.3.5/tests/__init__.py
+-rw-rw-rw-   0        0        0    11141 2024-05-17 03:40:40.000000 thepipe_api-0.3.5/tests/test_thepipe.py
+drwxrwxrwx   0        0        0        0 2024-05-17 04:46:44.057306 thepipe_api-0.3.5/thepipe_api/
+-rw-rw-rw-   0        0        0       86 2024-04-18 07:46:31.000000 thepipe_api-0.3.5/thepipe_api/__init__.py
+-rw-rw-rw-   0        0        0     5756 2024-05-17 04:34:22.000000 thepipe_api-0.3.5/thepipe_api/compressor.py
+-rw-rw-rw-   0        0        0     2878 2024-04-28 06:43:08.000000 thepipe_api-0.3.5/thepipe_api/core.py
+-rw-rw-rw-   0        0        0    25023 2024-05-04 16:44:13.000000 thepipe_api-0.3.5/thepipe_api/extractor.py
+-rw-rw-rw-   0        0        0     3704 2024-04-29 04:19:09.000000 thepipe_api-0.3.5/thepipe_api/thepipe.py
+drwxrwxrwx   0        0        0        0 2024-05-17 04:46:44.080305 thepipe_api-0.3.5/thepipe_api.egg-info/
+-rw-rw-rw-   0        0        0    13018 2024-05-17 04:46:43.000000 thepipe_api-0.3.5/thepipe_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-05-17 04:46:43.000000 thepipe_api-0.3.5/thepipe_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 04:46:43.000000 thepipe_api-0.3.5/thepipe_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-17 04:46:43.000000 thepipe_api-0.3.5/thepipe_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      127 2024-05-17 04:46:43.000000 thepipe_api-0.3.5/thepipe_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-17 04:46:43.000000 thepipe_api-0.3.5/thepipe_api.egg-info/top_level.txt
```

### Comparing `thepipe_api-0.3.4/LICENSE` & `thepipe_api-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.3.4/PKG-INFO` & `thepipe_api-0.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.3.4
+Version: 0.3.5
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
   <a href="https://github.com/emcf/thepipe/blob/main/README.md">English</a> | <a href="https://github.com/emcf/thepipe/blob/main/README_cn.md">中文</a>
 </p>
 
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-access-blue)</a> <a href="https://discord.gg/bXfKeGs5qV">![Join discord](https://img.shields.io/discord/1227806200478044274?color=4f69ef&label=Discord&logo=discord&logoColor=ffffff)</a>
 
 ### Feed PDFs, URLs, Slides, YouTube videos, Word docs and more into Vision-Language models with one line of code ⚡
 
-The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that want to support comprehensive textual and visual understanding across a wide range of data sources. The Pipe is available as a 24/7 hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally to let you run the compute.
+The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that want to support comprehensive textual and visual understanding across a wide range of data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally if you have the the compute.
 
 ![Science assistant demo](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/science_assistantpy2.png)
 
 
 ## Features 🌟
 
 - Extracts text and visuals from files or web pages 📚
@@ -47,15 +47,15 @@
 - Auto-compress prompts exceeding your chosen token limit 📦
 - Works even with missing file extensions, in-memory data streams 💾
 - Works with codebases, git repos, and custom integrations 🌐
 - Multi-threaded ⚡️
 
 ## Getting Started  🚀
 
-The Pipe handles a wide array of complex filetypes, and thus has many dependencies that must be installed separately. It also requires a strong machine for good response times. For this reason, we host it as an API that works out-of-the-box. 
+The Pipe can read a wide array of file types, and thus has many dependencies that must be installed separately. It also requires a strong machine for good response times. For this reason, we host it as an API that works out-of-the-box. 
 
 First, install The Pipe. 
 ```
 pip install thepipe_api
 ```
 
 The Pipe is available as a hosted API, or it can be set up locally. An API key is recommended for out-of-the-box functionality (alternatively, see the local installation section). Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have a key yet? [Get one here](https://thepi.pe).
@@ -65,18 +65,18 @@
 from thepipe_api import thepipe
 messages = thepipe.extract("example.pdf")
 ```
 Or websites:
 ```python
 messages = thepipe.extract("https://example.com")
 ```
-Then feed it into GPT-4-Vision:
+Then feed it into GPT-4V like so:
 ```python
-response = client.chat.completions.create(
-    model="gpt-4-vision-preview",
+response = openai.chat.completions.create(
+    model="gpt-4-turbo",
     messages = messages,
 )
 ```
 
 ![Just call OpenAI](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/IMG_0180.jpg)
 
 You can also use The Pipe from the command line. Here's how to recursively extract from a directory, matching only files containing a substring (in this example, typescript files) and ignore files containing other substrings (in this example, anything in the "tests" folder):
@@ -90,23 +90,23 @@
 | Source Type                           | Input types        | Token Compression 🗜️ | Image Extraction 👁️ | Notes 📌                                                  |
 |---------------------------------------|------------------------------------------|-------------------|------------------|---------------------------------------------------------|
 | Directory                             | Any `/path/to/directory`                 | ✔️               | ✔️               | Extracts from all files in directory, supports match and ignore patterns |
 | Code                                  | `.py`, `.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc | ✔️ (varies)   | ❌               | Combines all code files. `.c`, `.cpp`, `.py` are compressible with ctags, others are not |
 | Plaintext                             | `.txt`, `.md`, `.rtf`, etc               | ✔️               | ❌               | Regular text files                                                      |
 | PDF                                   | `.pdf`                                  | ✔️               | ✔️    | Extracts text and images of each page; can use AI for extraction of table data and  images within pages |
 | Image                                 | `.jpg`, `.jpeg`, `.png` | ❌                | ✔️              | Extracts images, uses OCR if text_only                        |
-| Data Table                           | `.csv`, `.xls`, `.xlsx`             | ✔️                | ❌               | Extracts data from spreadsheets; converts to text representation. For very large datasets, will only extract column names and types         |
+| Spreadsheet                           | `.csv`, `.xls`, `.xlsx`             | ✔️                | ❌               | Extracts data from spreadsheets; converts each row into a JSON formatted string         |
 | Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
 | Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
 | Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
-| Video                                 | `.mp4`, `.avi`, `.mov`, `.wmv`     | ✔️               | ✔️                | Extracts frames from video files; supports frame extraction and OCR for text extraction from frames |
+| Video                                 | `.mp4`, `.mov`, `.wmv`     | ✔️               | ✔️                | Extracts frames and audio transcript from videos in per-minute chunks. |
 | Audio                                 | `.mp3`, `.wav`          | ✔️               | ❌                | Extracts text from audio files; supports speech-to-text conversion        | 
 | Website                               | URLs (inputs starting with `http`, `https`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
 | GitHub Repository                     | GitHub repo URLs (inputs starting with `https://github.com` or `https://www.github.com`)                          | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
-| YouTube Video                         | YouTube video URLs (inputs starting with `https://youtube.com` or `https://www.youtube.com`)                     | ✔️               | ✔️                | Extracts frames and transcript from YouTube videos in per-minute chunks          |
+| YouTube Video                         | YouTube video URLs (inputs starting with `https://youtube.com` or `https://www.youtube.com`)                     | ✔️               | ✔️                | Extracts frames and transcript from YouTube videos in per-minute chunks.          |
 | ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
 
 ## How it works 🛠️
 
 The input source is either a file path, a URL, or a directory. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible list of multimodal messages representing chunks of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). The messages returned should look like this:
 ```json
 [
@@ -135,16 +135,33 @@
 It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), opt-in AI [table, equation, and figure extraction](https://thepi.pe/pricing), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
 
 ![Demo](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/grader.py%20(6).png)
 
 
 ## Local Installation 🛠️
 
-If you do not wish to use our API, you are welcome host The Pipe for yourself locally. 
-If you choose to do this, you must install a number of dependencies for the code to function correctly, some of which may incur compute costs and/or require a GPU for reasonable performance. Additional installed dependencies are required: pytorch, universal-ctags, playwright, pytesseract, llmlingua, moviepy, and pytube. This installation process will depend on your system and compute capabilities. After installing them, follow these steps for a local setup:
+The Pipe handles a wide array of complex filetypes, and thus requires installation of many different packages to function. It also requires a very capable machine for good response times. For this reason, we host it as an API that works out-of-the-box. To use The Pipe locally for free instead, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), [pytube](https://github.com/pytube/) and the remaining local python requirements, which differ from the more lightweight API requirements:
+
+```bash
+git clone https://github.com/emcf/thepipe
+pip install -r requirements_local.txt
+```
+
+Tip for windows users: Install the python-libmagic binaries with `pip install python-magic-bin`. Ensure the `tesseract-ocr` binaries and the `ctags` binaries are in your PATH. For YouTube video extraction to function consistently, you will need to modify your `pytube` installation to send a valid user agent header (I know, it's complicated. See [this issue](https://github.com/pytube/pytube/issues/399) for more).
+
+Now you can use The Pipe with Python:
+```bash
+from thepipe_api import thepipe
+chunks = thepipe.extract("example.pdf", local=True)
+```
+
+or from the command line:
+```bash
+thepipe path/to/folder --match .tsx --ignore tests
+```
 
 Arguments are:
 - `source` (required): can be a file path, a URL, or a directory path.
 - `local` (optional): Use the local version of The Pipe instead of the hosted API.
 - `match` (optional): Substring to match files in the directory. Regex is not yet supported.
 - `ignore` (optional): Substring to ignore files in the directory. Regex is not yet supported.
 - `limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed. This may not work as expected with the API, as it is in active development.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.3.4 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.3.5 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
@@ -19,118 +19,127 @@
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_i_s_c_o_r_d_/
 _1_2_2_7_8_0_6_2_0_0_4_7_8_0_4_4_2_7_4_?_c_o_l_o_r_=_4_f_6_9_e_f_&_l_a_b_e_l_=_D_i_s_c_o_r_d_&_l_o_g_o_=_d_i_s_c_o_r_d_&_l_o_g_o_C_o_l_o_r_=_f_f_f_f_f_f_)
 ### Feed PDFs, URLs, Slides, YouTube videos, Word docs and more into Vision-
 Language models with one line of code â¡ The Pipe is a multimodal-first tool
 for feeding files and web pages into vision-language models such as GPT-4V. It
 is best for LLM and RAG applications that want to support comprehensive textual
 and visual understanding across a wide range of data sources. The Pipe is
-available as a 24/7 hosted API at [thepi.pe](https://thepi.pe), or it can be
-set up locally to let you run the compute. ![Science assistant demo](https://
+available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up
+locally if you have the the compute. ![Science assistant demo](https://
 rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/
 science_assistantpy2.png) ## Features ð - Extracts text and visuals from
 files or web pages ð - Outputs chunks optimized for multimodal LLMs and RAG
 frameworks ð¼ï¸ - Interpret complex PDFs, web pages, docs, videos, data, and
 more ð§  - Auto-compress prompts exceeding your chosen token limit ð¦ -
 Works even with missing file extensions, in-memory data streams ð¾ - Works
 with codebases, git repos, and custom integrations ð - Multi-threaded â¡ï¸
-## Getting Started ð The Pipe handles a wide array of complex filetypes, and
-thus has many dependencies that must be installed separately. It also requires
-a strong machine for good response times. For this reason, we host it as an API
+## Getting Started ð The Pipe can read a wide array of file types, and thus
+has many dependencies that must be installed separately. It also requires a
+strong machine for good response times. For this reason, we host it as an API
 that works out-of-the-box. First, install The Pipe. ``` pip install thepipe_api
 ``` The Pipe is available as a hosted API, or it can be set up locally. An API
 key is recommended for out-of-the-box functionality (alternatively, see the
 local installation section). Ensure the `THEPIPE_API_KEY` environment variable
 is set. Don't have a key yet? [Get one here](https://thepi.pe). Now you can
 extract comprehensive text and visuals from any file: ```python from
 thepipe_api import thepipe messages = thepipe.extract("example.pdf") ``` Or
 websites: ```python messages = thepipe.extract("https://example.com") ``` Then
-feed it into GPT-4-Vision: ```python response = client.chat.completions.create
-( model="gpt-4-vision-preview", messages = messages, ) ``` ![Just call OpenAI]
-(https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/
-IMG_0180.jpg) You can also use The Pipe from the command line. Here's how to
-recursively extract from a directory, matching only files containing a
-substring (in this example, typescript files) and ignore files containing other
-substrings (in this example, anything in the "tests" folder): ```bash thepipe
-path/to/folder --match tsx --ignore tests ``` ## Supported File Types ð |
-Source Type | Input types | Token Compression ðï¸ | Image Extraction
-ðï¸ | Notes ð | |---------------------------------------|---------------
----------------------------|-------------------|------------------|------------
----------------------------------------------| | Directory | Any `/path/to/
-directory` | âï¸ | âï¸ | Extracts from all files in directory, supports
-match and ignore patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`,
-`.cpp`, etc | âï¸ (varies) | â | Combines all code files. `.c`, `.cpp`,
-`.py` are compressible with ctags, others are not | | Plaintext | `.txt`,
-`.md`, `.rtf`, etc | âï¸ | â | Regular text files | | PDF | `.pdf` |
-âï¸ | âï¸ | Extracts text and images of each page; can use AI for
+feed it into GPT-4V like so: ```python response =
+openai.chat.completions.create( model="gpt-4-turbo", messages = messages, ) ```
+![Just call OpenAI](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/
+public/assets/IMG_0180.jpg) You can also use The Pipe from the command line.
+Here's how to recursively extract from a directory, matching only files
+containing a substring (in this example, typescript files) and ignore files
+containing other substrings (in this example, anything in the "tests" folder):
+```bash thepipe path/to/folder --match tsx --ignore tests ``` ## Supported File
+Types ð | Source Type | Input types | Token Compression ðï¸ | Image
+Extraction ðï¸ | Notes ð | |---------------------------------------|----
+--------------------------------------|-------------------|------------------|-
+--------------------------------------------------------| | Directory | Any `/
+path/to/directory` | âï¸ | âï¸ | Extracts from all files in directory,
+supports match and ignore patterns | | Code | `.py`, `.tsx`, `.js`, `.html`,
+`.css`, `.cpp`, etc | âï¸ (varies) | â | Combines all code files. `.c`,
+`.cpp`, `.py` are compressible with ctags, others are not | | Plaintext |
+`.txt`, `.md`, `.rtf`, etc | âï¸ | â | Regular text files | | PDF | `.pdf`
+| âï¸ | âï¸ | Extracts text and images of each page; can use AI for
 extraction of table data and images within pages | | Image | `.jpg`, `.jpeg`,
-`.png` | â | âï¸ | Extracts images, uses OCR if text_only | | Data Table |
-`.csv`, `.xls`, `.xlsx` | âï¸ | â | Extracts data from spreadsheets;
-converts to text representation. For very large datasets, will only extract
-column names and types | | Jupyter Notebook | `.ipynb` | â | âï¸ |
-Extracts code, markdown, and images from Jupyter notebooks | | Microsoft Word
-Document | `.docx` | âï¸ | âï¸ | Extracts text and images from Word
-documents | | Microsoft PowerPoint Presentation | `.pptx` | âï¸ | âï¸ |
-Extracts text and images from PowerPoint presentations | | Video | `.mp4`,
-`.avi`, `.mov`, `.wmv` | âï¸ | âï¸ | Extracts frames from video files;
-supports frame extraction and OCR for text extraction from frames | | Audio |
-`.mp3`, `.wav` | âï¸ | â | Extracts text from audio files; supports
-speech-to-text conversion | | Website | URLs (inputs starting with `http`,
-`https`, `ftp`) | âï¸ | âï¸ | Extracts text from web page along with
-image (or images if scrollable); text-only extraction available | | GitHub
-Repository | GitHub repo URLs (inputs starting with `https://github.com` or
-`https://www.github.com`) | âï¸ | âï¸ | Extracts from GitHub
-repositories; supports branch specification | | YouTube Video | YouTube video
-URLs (inputs starting with `https://youtube.com` or `https://www.youtube.com`)
-| âï¸ | âï¸ | Extracts frames and transcript from YouTube videos in per-
-minute chunks | | ZIP File | `.zip` | âï¸ | âï¸ | Extracts contents of
-ZIP files; supports nested directory extraction | ## How it works ð ï¸ The
-input source is either a file path, a URL, or a directory. The pipe will
-extract information from the source and process it for downstream use with
-[language models](https://en.wikipedia.org/wiki/Large_language_model), [vision
-transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-
-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is
-a sensible list of multimodal messages representing chunks of the extracted
-information, carefully crafted to fit within context windows for any models
-from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://
-openai.com/gpt-4). The messages returned should look like this: ```json [
-{ "role": "user", "content": [ { "type": "text", "text": "..." }, { "type":
-"image_url", "image_url": { "url": "data:image/jpeg;base64,..." } } ] } ] ```
-If you want to feed these messages directly into the model, it is important to
-be mindful of the token limit. OpenAI does not allow too many images in the
-prompt (see discussion [here](https://community.openai.com/t/gpt-4-vision-
-maximum-amount-of-images/573110/6)), so long files should be extracted with
-`text_only=True` to avoid this issue, while long text files should either be
-compressed or embedded in a RAG framework. The text and images from these
-messages may also be prepared for a vector database with
-`thepipe.core.create_chunks_from_messages` or for downstream use with RAG
-frameworks. [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily
-integrate The Pipe with any LLM provider. It uses a variety of heuristics for
-optimal performance with vision-language models, including AI filetype
-detection with [filetype detection](https://opensource.googleblog.com/2024/02/
-magika-ai-powered-fast-and-efficient-file-type-identification.html), opt-in AI
-[table, equation, and figure extraction](https://thepi.pe/pricing), efficient
-[token compression](https://arxiv.org/abs/2403.12968), automatic [image
-encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/
-abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172)
-effects, and more, all pre-built to work out-of-the-box. ![Demo](https://
-rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/grader.py%20
-(6).png) ## Local Installation ð ï¸ If you do not wish to use our API, you
-are welcome host The Pipe for yourself locally. If you choose to do this, you
-must install a number of dependencies for the code to function correctly, some
-of which may incur compute costs and/or require a GPU for reasonable
-performance. Additional installed dependencies are required: pytorch,
-universal-ctags, playwright, pytesseract, llmlingua, moviepy, and pytube. This
-installation process will depend on your system and compute capabilities. After
-installing them, follow these steps for a local setup: Arguments are: -
-`source` (required): can be a file path, a URL, or a directory path. - `local`
-(optional): Use the local version of The Pipe instead of the hosted API. -
-`match` (optional): Substring to match files in the directory. Regex is not yet
-supported. - `ignore` (optional): Substring to ignore files in the directory.
-Regex is not yet supported. - `limit` (optional): The token limit for the
-output prompt, defaults to 100K. Prompts exceeding the limit will be
-compressed. This may not work as expected with the API, as it is in active
-development. - `ai_extraction` (optional): Extract tables, figures, and math
-from PDFs using our extractor. Incurs extra costs. - `text_only` (optional): Do
-not extract images from documents or websites. Additionally, image files will
-be represented with OCR instead of as images. # Sponsors _[_B_o_o_k_ _u_s_ _w_i_t_h
+`.png` | â | âï¸ | Extracts images, uses OCR if text_only | | Spreadsheet
+| `.csv`, `.xls`, `.xlsx` | âï¸ | â | Extracts data from spreadsheets;
+converts each row into a JSON formatted string | | Jupyter Notebook | `.ipynb`
+| â | âï¸ | Extracts code, markdown, and images from Jupyter notebooks | |
+Microsoft Word Document | `.docx` | âï¸ | âï¸ | Extracts text and images
+from Word documents | | Microsoft PowerPoint Presentation | `.pptx` | âï¸ |
+âï¸ | Extracts text and images from PowerPoint presentations | | Video |
+`.mp4`, `.mov`, `.wmv` | âï¸ | âï¸ | Extracts frames and audio transcript
+from videos in per-minute chunks. | | Audio | `.mp3`, `.wav` | âï¸ | â |
+Extracts text from audio files; supports speech-to-text conversion | | Website
+| URLs (inputs starting with `http`, `https`, `ftp`) | âï¸ | âï¸ |
+Extracts text from web page along with image (or images if scrollable); text-
+only extraction available | | GitHub Repository | GitHub repo URLs (inputs
+starting with `https://github.com` or `https://www.github.com`) | âï¸ |
+âï¸ | Extracts from GitHub repositories; supports branch specification | |
+YouTube Video | YouTube video URLs (inputs starting with `https://youtube.com`
+or `https://www.youtube.com`) | âï¸ | âï¸ | Extracts frames and
+transcript from YouTube videos in per-minute chunks. | | ZIP File | `.zip` |
+âï¸ | âï¸ | Extracts contents of ZIP files; supports nested directory
+extraction | ## How it works ð ï¸ The input source is either a file path, a
+URL, or a directory. The pipe will extract information from the source and
+process it for downstream use with [language models](https://en.wikipedia.org/
+wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/
+wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/
+2304.00685). The output from the pipe is a sensible list of multimodal messages
+representing chunks of the extracted information, carefully crafted to fit
+within context windows for any models from [gemma-7b](https://huggingface.co/
+google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). The messages returned
+should look like this: ```json [ { "role": "user", "content": [ { "type":
+"text", "text": "..." }, { "type": "image_url", "image_url": { "url": "data:
+image/jpeg;base64,..." } } ] } ] ``` If you want to feed these messages
+directly into the model, it is important to be mindful of the token limit.
+OpenAI does not allow too many images in the prompt (see discussion [here]
+(https://community.openai.com/t/gpt-4-vision-maximum-amount-of-images/573110/
+6)), so long files should be extracted with `text_only=True` to avoid this
+issue, while long text files should either be compressed or embedded in a RAG
+framework. The text and images from these messages may also be prepared for a
+vector database with `thepipe.core.create_chunks_from_messages` or for
+downstream use with RAG frameworks. [LiteLLM](https://github.com/BerriAI/
+litellm) can be used to easily integrate The Pipe with any LLM provider. It
+uses a variety of heuristics for optimal performance with vision-language
+models, including AI filetype detection with [filetype detection](https://
+opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-
+type-identification.html), opt-in AI [table, equation, and figure extraction]
+(https://thepi.pe/pricing), efficient [token compression](https://arxiv.org/
+abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/
+Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle]
+(https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work
+out-of-the-box. ![Demo](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/
+object/public/assets/grader.py%20(6).png) ## Local Installation ð ï¸ The
+Pipe handles a wide array of complex filetypes, and thus requires installation
+of many different packages to function. It also requires a very capable machine
+for good response times. For this reason, we host it as an API that works out-
+of-the-box. To use The Pipe locally for free instead, you will need
+[playwright](https://github.com/microsoft/playwright), [ctags](https://
+github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract),
+[pytube](https://github.com/pytube/) and the remaining local python
+requirements, which differ from the more lightweight API requirements: ```bash
+git clone https://github.com/emcf/thepipe pip install -r requirements_local.txt
+``` Tip for windows users: Install the python-libmagic binaries with `pip
+install python-magic-bin`. Ensure the `tesseract-ocr` binaries and the `ctags`
+binaries are in your PATH. For YouTube video extraction to function
+consistently, you will need to modify your `pytube` installation to send a
+valid user agent header (I know, it's complicated. See [this issue](https://
+github.com/pytube/pytube/issues/399) for more). Now you can use The Pipe with
+Python: ```bash from thepipe_api import thepipe chunks = thepipe.extract
+("example.pdf", local=True) ``` or from the command line: ```bash thepipe path/
+to/folder --match .tsx --ignore tests ``` Arguments are: - `source` (required):
+can be a file path, a URL, or a directory path. - `local` (optional): Use the
+local version of The Pipe instead of the hosted API. - `match` (optional):
+Substring to match files in the directory. Regex is not yet supported. -
+`ignore` (optional): Substring to ignore files in the directory. Regex is not
+yet supported. - `limit` (optional): The token limit for the output prompt,
+defaults to 100K. Prompts exceeding the limit will be compressed. This may not
+work as expected with the API, as it is in active development. -
+`ai_extraction` (optional): Extract tables, figures, and math from PDFs using
+our extractor. Incurs extra costs. - `text_only` (optional): Do not extract
+images from documents or websites. Additionally, image files will be
+represented with OCR instead of as images. # Sponsors _[_B_o_o_k_ _u_s_ _w_i_t_h
 _C_a_l_._c_o_m_]Thank you to [Cal.com](https://cal.com/) for sponsoring this project.
 Contact emmett@thepi.pe for sponsorship information.
```

### Comparing `thepipe_api-0.3.4/README.md` & `thepipe_api-0.3.5/thepipe_api.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,722 +1,814 @@
-00000000: 0d0a 2320 3c61 2068 7265 663d 2268 7474  ..# <a href="htt
-00000010: 7073 3a2f 2f74 6865 7069 2e70 652f 223e  ps://thepi.pe/">
-00000020: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000030: 2f2f 7270 6e75 747a 656d 7574 6272 756d  //rpnutzemutbrum
-00000040: 637a 7776 7565 2e73 7570 6162 6173 652e  czwvue.supabase.
-00000050: 636f 2f73 746f 7261 6765 2f76 312f 6f62  co/storage/v1/ob
-00000060: 6a65 6374 2f70 7562 6c69 632f 6173 7365  ject/public/asse
-00000070: 7473 2f70 6970 656c 696e 655f 736d 616c  ts/pipeline_smal
-00000080: 6c25 3230 2831 292e 706e 6722 2061 6c74  l%20(1).png" alt
-00000090: 3d22 5069 7065 6c69 6e65 2049 6c6c 7573  ="Pipeline Illus
-000000a0: 7472 6174 696f 6e22 2073 7479 6c65 3d22  tration" style="
-000000b0: 7769 6474 683a 3936 7078 3b20 6865 6967  width:96px; heig
-000000c0: 6874 3a37 3270 783b 2076 6572 7469 6361  ht:72px; vertica
-000000d0: 6c2d 616c 6967 6e3a 6d69 6464 6c65 3b22  l-align:middle;"
-000000e0: 3e20 5468 6520 5069 7065 3c2f 613e 0d0a  > The Pipe</a>..
-000000f0: 3c70 3e0d 0a20 203c 6120 6872 6566 3d22  <p>..  <a href="
-00000100: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000110: 6f6d 2f65 6d63 662f 7468 6570 6970 652f  om/emcf/thepipe/
-00000120: 626c 6f62 2f6d 6169 6e2f 5245 4144 4d45  blob/main/README
-00000130: 2e6d 6422 3e45 6e67 6c69 7368 3c2f 613e  .md">English</a>
-00000140: 207c 203c 6120 6872 6566 3d22 6874 7470   | <a href="http
-00000150: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
-00000160: 6d63 662f 7468 6570 6970 652f 626c 6f62  mcf/thepipe/blob
-00000170: 2f6d 6169 6e2f 5245 4144 4d45 5f63 6e2e  /main/README_cn.
-00000180: 6d64 223e e4b8 ade6 9687 3c2f 613e 0d0a  md">......</a>..
-00000190: 3c2f 703e 0d0a 0d0a 5b21 5b63 6f64 6563  </p>....[![codec
-000001a0: 6f76 5d28 6874 7470 733a 2f2f 636f 6465  ov](https://code
-000001b0: 636f 762e 696f 2f67 682f 656d 6366 2f74  cov.io/gh/emcf/t
-000001c0: 6865 7069 7065 2f67 7261 7068 2f62 6164  hepipe/graph/bad
-000001d0: 6765 2e73 7667 3f74 6f6b 656e 3d4f 4537  ge.svg?token=OE7
-000001e0: 4355 4546 554c 3929 5d28 6874 7470 733a  CUEFUL9)](https:
-000001f0: 2f2f 636f 6465 636f 762e 696f 2f67 682f  //codecov.io/gh/
-00000200: 656d 6366 2f74 6865 7069 7065 2920 215b  emcf/thepipe) ![
-00000210: 7079 7468 6f6e 2d67 682d 6163 7469 6f6e  python-gh-action
-00000220: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000230: 2e63 6f6d 2f65 6d63 662f 7468 6570 6970  .com/emcf/thepip
-00000240: 652f 6163 7469 6f6e 732f 776f 726b 666c  e/actions/workfl
-00000250: 6f77 732f 7079 7468 6f6e 2d63 692e 796d  ows/python-ci.ym
-00000260: 6c2f 6261 6467 652e 7376 6729 203c 6120  l/badge.svg) <a 
-00000270: 6872 6566 3d22 6874 7470 733a 2f2f 7468  href="https://th
-00000280: 6570 692e 7065 2f22 3e21 5b57 6562 7369  epi.pe/">![Websi
-00000290: 7465 5d28 6874 7470 733a 2f2f 696d 672e  te](https://img.
-000002a0: 7368 6965 6c64 732e 696f 2f77 6562 7369  shields.io/websi
-000002b0: 7465 3f75 726c 3d68 7474 7073 2533 4125  te?url=https%3A%
-000002c0: 3246 2532 4674 6865 7069 7065 2e75 702e  2F%2Fthepipe.up.
-000002d0: 7261 696c 7761 792e 6170 7025 3246 266c  railway.app%2F&l
-000002e0: 6162 656c 3d41 5049 2532 3073 7461 7475  abel=API%20statu
-000002f0: 7329 3c2f 613e 203c 6120 6872 6566 3d22  s)</a> <a href="
-00000300: 6874 7470 733a 2f2f 7468 6570 692e 7065  https://thepi.pe
-00000310: 2f22 3e21 5b67 6574 2041 5049 5d28 6874  /">![get API](ht
-00000320: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000330: 732e 696f 2f62 6164 6765 2f41 5049 2d61  s.io/badge/API-a
-00000340: 6363 6573 732d 626c 7565 293c 2f61 3e20  ccess-blue)</a> 
-00000350: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000360: 2f64 6973 636f 7264 2e67 672f 6258 664b  /discord.gg/bXfK
-00000370: 6547 7335 7156 223e 215b 4a6f 696e 2064  eGs5qV">![Join d
-00000380: 6973 636f 7264 5d28 6874 7470 733a 2f2f  iscord](https://
-00000390: 696d 672e 7368 6965 6c64 732e 696f 2f64  img.shields.io/d
-000003a0: 6973 636f 7264 2f31 3232 3738 3036 3230  iscord/122780620
-000003b0: 3034 3738 3034 3432 3734 3f63 6f6c 6f72  0478044274?color
-000003c0: 3d34 6636 3965 6626 6c61 6265 6c3d 4469  =4f69ef&label=Di
-000003d0: 7363 6f72 6426 6c6f 676f 3d64 6973 636f  scord&logo=disco
-000003e0: 7264 266c 6f67 6f43 6f6c 6f72 3d66 6666  rd&logoColor=fff
-000003f0: 6666 6629 3c2f 613e 0d0a 0d0a 2323 2320  fff)</a>....### 
-00000400: 4665 6564 2050 4446 732c 2055 524c 732c  Feed PDFs, URLs,
-00000410: 2053 6c69 6465 732c 2059 6f75 5475 6265   Slides, YouTube
-00000420: 2076 6964 656f 732c 2057 6f72 6420 646f   videos, Word do
-00000430: 6373 2061 6e64 206d 6f72 6520 696e 746f  cs and more into
-00000440: 2056 6973 696f 6e2d 4c61 6e67 7561 6765   Vision-Language
-00000450: 206d 6f64 656c 7320 7769 7468 206f 6e65   models with one
-00000460: 206c 696e 6520 6f66 2063 6f64 6520 e29a   line of code ..
-00000470: a10d 0a0d 0a54 6865 2050 6970 6520 6973  .....The Pipe is
-00000480: 2061 206d 756c 7469 6d6f 6461 6c2d 6669   a multimodal-fi
-00000490: 7273 7420 746f 6f6c 2066 6f72 2066 6565  rst tool for fee
-000004a0: 6469 6e67 2066 696c 6573 2061 6e64 2077  ding files and w
-000004b0: 6562 2070 6167 6573 2069 6e74 6f20 7669  eb pages into vi
-000004c0: 7369 6f6e 2d6c 616e 6775 6167 6520 6d6f  sion-language mo
-000004d0: 6465 6c73 2073 7563 6820 6173 2047 5054  dels such as GPT
-000004e0: 2d34 562e 2049 7420 6973 2062 6573 7420  -4V. It is best 
-000004f0: 666f 7220 4c4c 4d20 616e 6420 5241 4720  for LLM and RAG 
-00000500: 6170 706c 6963 6174 696f 6e73 2074 6861  applications tha
-00000510: 7420 7761 6e74 2074 6f20 7375 7070 6f72  t want to suppor
-00000520: 7420 636f 6d70 7265 6865 6e73 6976 6520  t comprehensive 
-00000530: 7465 7874 7561 6c20 616e 6420 7669 7375  textual and visu
-00000540: 616c 2075 6e64 6572 7374 616e 6469 6e67  al understanding
-00000550: 2061 6372 6f73 7320 6120 7769 6465 2072   across a wide r
-00000560: 616e 6765 206f 6620 6461 7461 2073 6f75  ange of data sou
-00000570: 7263 6573 2e20 5468 6520 5069 7065 2069  rces. The Pipe i
-00000580: 7320 6176 6169 6c61 626c 6520 6173 2061  s available as a
-00000590: 2032 342f 3720 686f 7374 6564 2041 5049   24/7 hosted API
-000005a0: 2061 7420 5b74 6865 7069 2e70 655d 2868   at [thepi.pe](h
-000005b0: 7474 7073 3a2f 2f74 6865 7069 2e70 6529  ttps://thepi.pe)
-000005c0: 2c20 6f72 2069 7420 6361 6e20 6265 2073  , or it can be s
-000005d0: 6574 2075 7020 6c6f 6361 6c6c 7920 746f  et up locally to
-000005e0: 206c 6574 2079 6f75 2072 756e 2074 6865   let you run the
-000005f0: 2063 6f6d 7075 7465 2e0d 0a0d 0a21 5b53   compute.....![S
-00000600: 6369 656e 6365 2061 7373 6973 7461 6e74  cience assistant
-00000610: 2064 656d 6f5d 2868 7474 7073 3a2f 2f72   demo](https://r
-00000620: 706e 7574 7a65 6d75 7462 7275 6d63 7a77  pnutzemutbrumczw
-00000630: 7675 652e 7375 7061 6261 7365 2e63 6f2f  vue.supabase.co/
-00000640: 7374 6f72 6167 652f 7631 2f6f 626a 6563  storage/v1/objec
-00000650: 742f 7075 626c 6963 2f61 7373 6574 732f  t/public/assets/
-00000660: 7363 6965 6e63 655f 6173 7369 7374 616e  science_assistan
-00000670: 7470 7932 2e70 6e67 290d 0a0d 0a0d 0a23  tpy2.png)......#
-00000680: 2320 4665 6174 7572 6573 20f0 9f8c 9f0d  # Features .....
-00000690: 0a0d 0a2d 2045 7874 7261 6374 7320 7465  ...- Extracts te
-000006a0: 7874 2061 6e64 2076 6973 7561 6c73 2066  xt and visuals f
-000006b0: 726f 6d20 6669 6c65 7320 6f72 2077 6562  rom files or web
-000006c0: 2070 6167 6573 20f0 9f93 9a0d 0a2d 204f   pages ......- O
-000006d0: 7574 7075 7473 2063 6875 6e6b 7320 6f70  utputs chunks op
-000006e0: 7469 6d69 7a65 6420 666f 7220 6d75 6c74  timized for mult
-000006f0: 696d 6f64 616c 204c 4c4d 7320 616e 6420  imodal LLMs and 
-00000700: 5241 4720 6672 616d 6577 6f72 6b73 20f0  RAG frameworks .
-00000710: 9f96 bcef b88f 0d0a 2d20 496e 7465 7270  ........- Interp
-00000720: 7265 7420 636f 6d70 6c65 7820 5044 4673  ret complex PDFs
-00000730: 2c20 7765 6220 7061 6765 732c 2064 6f63  , web pages, doc
-00000740: 732c 2076 6964 656f 732c 2064 6174 612c  s, videos, data,
-00000750: 2061 6e64 206d 6f72 6520 f09f a7a0 0d0a   and more ......
-00000760: 2d20 4175 746f 2d63 6f6d 7072 6573 7320  - Auto-compress 
-00000770: 7072 6f6d 7074 7320 6578 6365 6564 696e  prompts exceedin
-00000780: 6720 796f 7572 2063 686f 7365 6e20 746f  g your chosen to
-00000790: 6b65 6e20 6c69 6d69 7420 f09f 93a6 0d0a  ken limit ......
-000007a0: 2d20 576f 726b 7320 6576 656e 2077 6974  - Works even wit
-000007b0: 6820 6d69 7373 696e 6720 6669 6c65 2065  h missing file e
-000007c0: 7874 656e 7369 6f6e 732c 2069 6e2d 6d65  xtensions, in-me
-000007d0: 6d6f 7279 2064 6174 6120 7374 7265 616d  mory data stream
-000007e0: 7320 f09f 92be 0d0a 2d20 576f 726b 7320  s ......- Works 
-000007f0: 7769 7468 2063 6f64 6562 6173 6573 2c20  with codebases, 
-00000800: 6769 7420 7265 706f 732c 2061 6e64 2063  git repos, and c
-00000810: 7573 746f 6d20 696e 7465 6772 6174 696f  ustom integratio
-00000820: 6e73 20f0 9f8c 900d 0a2d 204d 756c 7469  ns ......- Multi
-00000830: 2d74 6872 6561 6465 6420 e29a a1ef b88f  -threaded ......
-00000840: 0d0a 0d0a 2323 2047 6574 7469 6e67 2053  ....## Getting S
-00000850: 7461 7274 6564 2020 f09f 9a80 0d0a 0d0a  tarted  ........
-00000860: 5468 6520 5069 7065 2068 616e 646c 6573  The Pipe handles
-00000870: 2061 2077 6964 6520 6172 7261 7920 6f66   a wide array of
-00000880: 2063 6f6d 706c 6578 2066 696c 6574 7970   complex filetyp
-00000890: 6573 2c20 616e 6420 7468 7573 2068 6173  es, and thus has
-000008a0: 206d 616e 7920 6465 7065 6e64 656e 6369   many dependenci
-000008b0: 6573 2074 6861 7420 6d75 7374 2062 6520  es that must be 
-000008c0: 696e 7374 616c 6c65 6420 7365 7061 7261  installed separa
-000008d0: 7465 6c79 2e20 4974 2061 6c73 6f20 7265  tely. It also re
-000008e0: 7175 6972 6573 2061 2073 7472 6f6e 6720  quires a strong 
-000008f0: 6d61 6368 696e 6520 666f 7220 676f 6f64  machine for good
-00000900: 2072 6573 706f 6e73 6520 7469 6d65 732e   response times.
-00000910: 2046 6f72 2074 6869 7320 7265 6173 6f6e   For this reason
-00000920: 2c20 7765 2068 6f73 7420 6974 2061 7320  , we host it as 
-00000930: 616e 2041 5049 2074 6861 7420 776f 726b  an API that work
-00000940: 7320 6f75 742d 6f66 2d74 6865 2d62 6f78  s out-of-the-box
-00000950: 2e20 0d0a 0d0a 4669 7273 742c 2069 6e73  . ....First, ins
-00000960: 7461 6c6c 2054 6865 2050 6970 652e 200d  tall The Pipe. .
-00000970: 0a60 6060 0d0a 7069 7020 696e 7374 616c  .```..pip instal
-00000980: 6c20 7468 6570 6970 655f 6170 690d 0a60  l thepipe_api..`
-00000990: 6060 0d0a 0d0a 5468 6520 5069 7065 2069  ``....The Pipe i
-000009a0: 7320 6176 6169 6c61 626c 6520 6173 2061  s available as a
-000009b0: 2068 6f73 7465 6420 4150 492c 206f 7220   hosted API, or 
-000009c0: 6974 2063 616e 2062 6520 7365 7420 7570  it can be set up
-000009d0: 206c 6f63 616c 6c79 2e20 416e 2041 5049   locally. An API
-000009e0: 206b 6579 2069 7320 7265 636f 6d6d 656e   key is recommen
-000009f0: 6465 6420 666f 7220 6f75 742d 6f66 2d74  ded for out-of-t
-00000a00: 6865 2d62 6f78 2066 756e 6374 696f 6e61  he-box functiona
-00000a10: 6c69 7479 2028 616c 7465 726e 6174 6976  lity (alternativ
-00000a20: 656c 792c 2073 6565 2074 6865 206c 6f63  ely, see the loc
-00000a30: 616c 2069 6e73 7461 6c6c 6174 696f 6e20  al installation 
-00000a40: 7365 6374 696f 6e29 2e20 456e 7375 7265  section). Ensure
-00000a50: 2074 6865 2060 5448 4550 4950 455f 4150   the `THEPIPE_AP
-00000a60: 495f 4b45 5960 2065 6e76 6972 6f6e 6d65  I_KEY` environme
-00000a70: 6e74 2076 6172 6961 626c 6520 6973 2073  nt variable is s
-00000a80: 6574 2e20 446f 6e27 7420 6861 7665 2061  et. Don't have a
-00000a90: 206b 6579 2079 6574 3f20 5b47 6574 206f   key yet? [Get o
-00000aa0: 6e65 2068 6572 655d 2868 7474 7073 3a2f  ne here](https:/
-00000ab0: 2f74 6865 7069 2e70 6529 2e0d 0a0d 0a4e  /thepi.pe).....N
-00000ac0: 6f77 2079 6f75 2063 616e 2065 7874 7261  ow you can extra
-00000ad0: 6374 2063 6f6d 7072 6568 656e 7369 7665  ct comprehensive
-00000ae0: 2074 6578 7420 616e 6420 7669 7375 616c   text and visual
-00000af0: 7320 6672 6f6d 2061 6e79 2066 696c 653a  s from any file:
-00000b00: 0d0a 6060 6070 7974 686f 6e0d 0a66 726f  ..```python..fro
-00000b10: 6d20 7468 6570 6970 655f 6170 6920 696d  m thepipe_api im
-00000b20: 706f 7274 2074 6865 7069 7065 0d0a 6d65  port thepipe..me
-00000b30: 7373 6167 6573 203d 2074 6865 7069 7065  ssages = thepipe
-00000b40: 2e65 7874 7261 6374 2822 6578 616d 706c  .extract("exampl
-00000b50: 652e 7064 6622 290d 0a60 6060 0d0a 4f72  e.pdf")..```..Or
-00000b60: 2077 6562 7369 7465 733a 0d0a 6060 6070   websites:..```p
-00000b70: 7974 686f 6e0d 0a6d 6573 7361 6765 7320  ython..messages 
-00000b80: 3d20 7468 6570 6970 652e 6578 7472 6163  = thepipe.extrac
-00000b90: 7428 2268 7474 7073 3a2f 2f65 7861 6d70  t("https://examp
-00000ba0: 6c65 2e63 6f6d 2229 0d0a 6060 600d 0a54  le.com")..```..T
-00000bb0: 6865 6e20 6665 6564 2069 7420 696e 746f  hen feed it into
-00000bc0: 2047 5054 2d34 2d56 6973 696f 6e3a 0d0a   GPT-4-Vision:..
-00000bd0: 6060 6070 7974 686f 6e0d 0a72 6573 706f  ```python..respo
-00000be0: 6e73 6520 3d20 636c 6965 6e74 2e63 6861  nse = client.cha
-00000bf0: 742e 636f 6d70 6c65 7469 6f6e 732e 6372  t.completions.cr
-00000c00: 6561 7465 280d 0a20 2020 206d 6f64 656c  eate(..    model
-00000c10: 3d22 6770 742d 342d 7669 7369 6f6e 2d70  ="gpt-4-vision-p
-00000c20: 7265 7669 6577 222c 0d0a 2020 2020 6d65  review",..    me
-00000c30: 7373 6167 6573 203d 206d 6573 7361 6765  ssages = message
-00000c40: 732c 0d0a 290d 0a60 6060 0d0a 0d0a 215b  s,..)..```....![
-00000c50: 4a75 7374 2063 616c 6c20 4f70 656e 4149  Just call OpenAI
-00000c60: 5d28 6874 7470 733a 2f2f 7270 6e75 747a  ](https://rpnutz
-00000c70: 656d 7574 6272 756d 637a 7776 7565 2e73  emutbrumczwvue.s
-00000c80: 7570 6162 6173 652e 636f 2f73 746f 7261  upabase.co/stora
-00000c90: 6765 2f76 312f 6f62 6a65 6374 2f70 7562  ge/v1/object/pub
-00000ca0: 6c69 632f 6173 7365 7473 2f49 4d47 5f30  lic/assets/IMG_0
-00000cb0: 3138 302e 6a70 6729 0d0a 0d0a 596f 7520  180.jpg)....You 
-00000cc0: 6361 6e20 616c 736f 2075 7365 2054 6865  can also use The
-00000cd0: 2050 6970 6520 6672 6f6d 2074 6865 2063   Pipe from the c
-00000ce0: 6f6d 6d61 6e64 206c 696e 652e 2048 6572  ommand line. Her
-00000cf0: 6527 7320 686f 7720 746f 2072 6563 7572  e's how to recur
-00000d00: 7369 7665 6c79 2065 7874 7261 6374 2066  sively extract f
-00000d10: 726f 6d20 6120 6469 7265 6374 6f72 792c  rom a directory,
-00000d20: 206d 6174 6368 696e 6720 6f6e 6c79 2066   matching only f
-00000d30: 696c 6573 2063 6f6e 7461 696e 696e 6720  iles containing 
-00000d40: 6120 7375 6273 7472 696e 6720 2869 6e20  a substring (in 
-00000d50: 7468 6973 2065 7861 6d70 6c65 2c20 7479  this example, ty
-00000d60: 7065 7363 7269 7074 2066 696c 6573 2920  pescript files) 
-00000d70: 616e 6420 6967 6e6f 7265 2066 696c 6573  and ignore files
-00000d80: 2063 6f6e 7461 696e 696e 6720 6f74 6865   containing othe
-00000d90: 7220 7375 6273 7472 696e 6773 2028 696e  r substrings (in
-00000da0: 2074 6869 7320 6578 616d 706c 652c 2061   this example, a
-00000db0: 6e79 7468 696e 6720 696e 2074 6865 2022  nything in the "
-00000dc0: 7465 7374 7322 2066 6f6c 6465 7229 3a0d  tests" folder):.
-00000dd0: 0a60 6060 6261 7368 0d0a 7468 6570 6970  .```bash..thepip
-00000de0: 6520 7061 7468 2f74 6f2f 666f 6c64 6572  e path/to/folder
-00000df0: 202d 2d6d 6174 6368 2074 7378 202d 2d69   --match tsx --i
-00000e00: 676e 6f72 6520 7465 7374 730d 0a60 6060  gnore tests..```
-00000e10: 0d0a 0d0a 0d0a 2323 2053 7570 706f 7274  ......## Support
-00000e20: 6564 2046 696c 6520 5479 7065 7320 f09f  ed File Types ..
-00000e30: 939a 0d0a 0d0a 7c20 536f 7572 6365 2054  ......| Source T
-00000e40: 7970 6520 2020 2020 2020 2020 2020 2020  ype             
-00000e50: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00000e60: 496e 7075 7420 7479 7065 7320 2020 2020  Input types     
-00000e70: 2020 207c 2054 6f6b 656e 2043 6f6d 7072     | Token Compr
-00000e80: 6573 7369 6f6e 20f0 9f97 9cef b88f 207c  ession ....... |
-00000e90: 2049 6d61 6765 2045 7874 7261 6374 696f   Image Extractio
-00000ea0: 6e20 f09f 9181 efb8 8f20 7c20 4e6f 7465  n ....... | Note
-00000eb0: 7320 f09f 938c 2020 2020 2020 2020 2020  s ....          
-00000ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ee0: 2020 2020 2020 2020 7c0d 0a7c 2d2d 2d2d          |..|----
-00000ef0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f10: 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---|------------
-00000f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d  --------------|-
-00000f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f50: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --|-------------
-00000f60: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d  -----|----------
-00000f70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
-00000fa0: 0d0a 7c20 4469 7265 6374 6f72 7920 2020  ..| Directory   
-00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fc0: 2020 2020 2020 2020 2020 7c20 416e 7920            | Any 
-00000fd0: 602f 7061 7468 2f74 6f2f 6469 7265 6374  `/path/to/direct
-00000fe0: 6f72 7960 2020 2020 2020 2020 2020 2020  ory`            
-00000ff0: 2020 2020 207c 20e2 9c94 efb8 8f20 2020       | ......   
-00001000: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
-00001010: 94ef b88f 2020 2020 2020 2020 2020 2020  ....            
-00001020: 2020 207c 2045 7874 7261 6374 7320 6672     | Extracts fr
-00001030: 6f6d 2061 6c6c 2066 696c 6573 2069 6e20  om all files in 
-00001040: 6469 7265 6374 6f72 792c 2073 7570 706f  directory, suppo
-00001050: 7274 7320 6d61 7463 6820 616e 6420 6967  rts match and ig
-00001060: 6e6f 7265 2070 6174 7465 726e 7320 7c0d  nore patterns |.
-00001070: 0a7c 2043 6f64 6520 2020 2020 2020 2020  .| Code         
-00001080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001090: 2020 2020 2020 2020 207c 2060 2e70 7960           | `.py`
-000010a0: 2c20 602e 7473 7860 2c20 602e 6a73 602c  , `.tsx`, `.js`,
-000010b0: 2060 2e68 746d 6c60 2c20 602e 6373 7360   `.html`, `.css`
-000010c0: 2c20 602e 6370 7060 2c20 6574 6320 7c20  , `.cpp`, etc | 
-000010d0: e29c 94ef b88f 2028 7661 7269 6573 2920  ...... (varies) 
-000010e0: 2020 7c20 e29d 8c20 2020 2020 2020 2020    | ...         
-000010f0: 2020 2020 2020 7c20 436f 6d62 696e 6573        | Combines
-00001100: 2061 6c6c 2063 6f64 6520 6669 6c65 732e   all code files.
-00001110: 2060 2e63 602c 2060 2e63 7070 602c 2060   `.c`, `.cpp`, `
-00001120: 2e70 7960 2061 7265 2063 6f6d 7072 6573  .py` are compres
-00001130: 7369 626c 6520 7769 7468 2063 7461 6773  sible with ctags
-00001140: 2c20 6f74 6865 7273 2061 7265 206e 6f74  , others are not
-00001150: 207c 0d0a 7c20 506c 6169 6e74 6578 7420   |..| Plaintext 
-00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001170: 2020 2020 2020 2020 2020 2020 7c20 602e              | `.
-00001180: 7478 7460 2c20 602e 6d64 602c 2060 2e72  txt`, `.md`, `.r
-00001190: 7466 602c 2065 7463 2020 2020 2020 2020  tf`, etc        
-000011a0: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
-000011b0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000011c0: e29d 8c20 2020 2020 2020 2020 2020 2020  ...             
-000011d0: 2020 7c20 5265 6775 6c61 7220 7465 7874    | Regular text
-000011e0: 2066 696c 6573 2020 2020 2020 2020 2020   files          
-000011f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001210: 2020 2020 2020 2020 2020 2020 7c0d 0a7c              |..|
-00001220: 2050 4446 2020 2020 2020 2020 2020 2020   PDF            
-00001230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001240: 2020 2020 2020 207c 2060 2e70 6466 6020         | `.pdf` 
-00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001270: 207c 20e2 9c94 efb8 8f20 2020 2020 2020   | ......       
-00001280: 2020 2020 2020 2020 7c20 e29c 94ef b88f          | ......
-00001290: 2020 2020 7c20 4578 7472 6163 7473 2074      | Extracts t
-000012a0: 6578 7420 616e 6420 696d 6167 6573 206f  ext and images o
-000012b0: 6620 6561 6368 2070 6167 653b 2063 616e  f each page; can
-000012c0: 2075 7365 2041 4920 666f 7220 6578 7472   use AI for extr
-000012d0: 6163 7469 6f6e 206f 6620 7461 626c 6520  action of table 
-000012e0: 6461 7461 2061 6e64 2020 696d 6167 6573  data and  images
-000012f0: 2077 6974 6869 6e20 7061 6765 7320 7c0d   within pages |.
-00001300: 0a7c 2049 6d61 6765 2020 2020 2020 2020  .| Image        
-00001310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001320: 2020 2020 2020 2020 207c 2060 2e6a 7067           | `.jpg
-00001330: 602c 2060 2e6a 7065 6760 2c20 602e 706e  `, `.jpeg`, `.pn
-00001340: 6760 207c 20e2 9d8c 2020 2020 2020 2020  g` | ...        
-00001350: 2020 2020 2020 2020 7c20 e29c 94ef b88f          | ......
-00001360: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00001370: 4578 7472 6163 7473 2069 6d61 6765 732c  Extracts images,
-00001380: 2075 7365 7320 4f43 5220 6966 2074 6578   uses OCR if tex
-00001390: 745f 6f6e 6c79 2020 2020 2020 2020 2020  t_only          
-000013a0: 2020 2020 2020 2020 2020 2020 2020 7c0d                |.
-000013b0: 0a7c 2044 6174 6120 5461 626c 6520 2020  .| Data Table   
-000013c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013d0: 2020 2020 2020 2020 7c20 602e 6373 7660          | `.csv`
-000013e0: 2c20 602e 786c 7360 2c20 602e 786c 7378  , `.xls`, `.xlsx
-000013f0: 6020 2020 2020 2020 2020 2020 2020 7c20  `             | 
-00001400: e29c 94ef b88f 2020 2020 2020 2020 2020  ......          
-00001410: 2020 2020 2020 7c20 e29d 8c20 2020 2020        | ...     
-00001420: 2020 2020 2020 2020 2020 7c20 4578 7472            | Extr
-00001430: 6163 7473 2064 6174 6120 6672 6f6d 2073  acts data from s
-00001440: 7072 6561 6473 6865 6574 733b 2063 6f6e  preadsheets; con
-00001450: 7665 7274 7320 746f 2074 6578 7420 7265  verts to text re
-00001460: 7072 6573 656e 7461 7469 6f6e 2e20 466f  presentation. Fo
-00001470: 7220 7665 7279 206c 6172 6765 2064 6174  r very large dat
-00001480: 6173 6574 732c 2077 696c 6c20 6f6e 6c79  asets, will only
-00001490: 2065 7874 7261 6374 2063 6f6c 756d 6e20   extract column 
-000014a0: 6e61 6d65 7320 616e 6420 7479 7065 7320  names and types 
-000014b0: 2020 2020 2020 2020 7c0d 0a7c 204a 7570          |..| Jup
-000014c0: 7974 6572 204e 6f74 6562 6f6f 6b20 2020  yter Notebook   
-000014d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014e0: 2020 207c 2060 2e69 7079 6e62 6020 2020     | `.ipynb`   
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310d 0a4e 616d 653a 2074 6865  : 2.1..Name: the
+00000020: 7069 7065 5f61 7069 0d0a 5665 7273 696f  pipe_api..Versio
+00000030: 6e3a 2030 2e33 2e35 0d0a 5375 6d6d 6172  n: 0.3.5..Summar
+00000040: 793a 2041 7574 6f6d 6174 6520 696e 666f  y: Automate info
+00000050: 726d 6174 696f 6e20 6578 7472 6163 7469  rmation extracti
+00000060: 6f6e 2066 6f72 206d 756c 7469 6d6f 6461  on for multimoda
+00000070: 6c20 4c4c 4d73 2e0d 0a48 6f6d 652d 7061  l LLMs...Home-pa
+00000080: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
+00000090: 7562 2e63 6f6d 2f65 6d63 662f 7468 6570  ub.com/emcf/thep
+000000a0: 6970 650d 0a41 7574 686f 723a 2045 6d6d  ipe..Author: Emm
+000000b0: 6574 7420 4d63 4661 726c 616e 650d 0a41  ett McFarlane..A
+000000c0: 7574 686f 722d 656d 6169 6c3a 2065 6d6d  uthor-email: emm
+000000d0: 6574 7440 7468 6570 692e 7065 0d0a 436c  ett@thepi.pe..Cl
+000000e0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+000000f0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000100: 3a20 5079 7468 6f6e 203a 3a20 330d 0a43  : Python :: 3..C
+00000110: 6c61 7373 6966 6965 723a 204c 6963 656e  lassifier: Licen
+00000120: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+00000130: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
+00000140: 650d 0a43 6c61 7373 6966 6965 723a 204f  e..Classifier: O
+00000150: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000160: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+00000170: 740d 0a52 6571 7569 7265 732d 5079 7468  t..Requires-Pyth
+00000180: 6f6e 3a20 3e3d 332e 360d 0a44 6573 6372  on: >=3.6..Descr
+00000190: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
+000001a0: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
+000001b0: 776e 0d0a 4c69 6365 6e73 652d 4669 6c65  wn..License-File
+000001c0: 3a20 4c49 4345 4e53 450d 0a52 6571 7569  : LICENSE..Requi
+000001d0: 7265 732d 4469 7374 3a20 6169 6f68 7474  res-Dist: aiohtt
+000001e0: 700d 0a52 6571 7569 7265 732d 4469 7374  p..Requires-Dist
+000001f0: 3a20 6368 6172 7365 742d 6e6f 726d 616c  : charset-normal
+00000200: 697a 6572 0d0a 5265 7175 6972 6573 2d44  izer..Requires-D
+00000210: 6973 743a 2050 7961 7272 6f77 0d0a 5265  ist: Pyarrow..Re
+00000220: 7175 6972 6573 2d44 6973 743a 2070 7974  quires-Dist: pyt
+00000230: 686f 6e2d 6d61 6769 630d 0a52 6571 7569  hon-magic..Requi
+00000240: 7265 732d 4469 7374 3a20 636f 6c6f 7261  res-Dist: colora
+00000250: 6d61 0d0a 5265 7175 6972 6573 2d44 6973  ma..Requires-Dis
+00000260: 743a 2072 6571 7565 7374 730d 0a52 6571  t: requests..Req
+00000270: 7569 7265 732d 4469 7374 3a20 7069 6c6c  uires-Dist: pill
+00000280: 6f77 0d0a 5265 7175 6972 6573 2d44 6973  ow..Requires-Dis
+00000290: 743a 2063 7373 7574 696c 730d 0a52 6571  t: cssutils..Req
+000002a0: 7569 7265 732d 4469 7374 3a20 6265 6175  uires-Dist: beau
+000002b0: 7469 6675 6c73 6f75 7034 0d0a 5265 7175  tifulsoup4..Requ
+000002c0: 6972 6573 2d44 6973 743a 206d 6167 696b  ires-Dist: magik
+000002d0: 610d 0a52 6571 7569 7265 732d 4469 7374  a..Requires-Dist
+000002e0: 3a20 7079 7468 6f6e 2d64 6f74 656e 760d  : python-dotenv.
+000002f0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000300: 6f70 656e 7079 786c 0d0a 0d0a 0d0a 2320  openpyxl......# 
+00000310: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000320: 2f74 6865 7069 2e70 652f 223e 3c69 6d67  /thepi.pe/"><img
+00000330: 2073 7263 3d22 6874 7470 733a 2f2f 7270   src="https://rp
+00000340: 6e75 747a 656d 7574 6272 756d 637a 7776  nutzemutbrumczwv
+00000350: 7565 2e73 7570 6162 6173 652e 636f 2f73  ue.supabase.co/s
+00000360: 746f 7261 6765 2f76 312f 6f62 6a65 6374  torage/v1/object
+00000370: 2f70 7562 6c69 632f 6173 7365 7473 2f70  /public/assets/p
+00000380: 6970 656c 696e 655f 736d 616c 6c25 3230  ipeline_small%20
+00000390: 2831 292e 706e 6722 2061 6c74 3d22 5069  (1).png" alt="Pi
+000003a0: 7065 6c69 6e65 2049 6c6c 7573 7472 6174  peline Illustrat
+000003b0: 696f 6e22 2073 7479 6c65 3d22 7769 6474  ion" style="widt
+000003c0: 683a 3936 7078 3b20 6865 6967 6874 3a37  h:96px; height:7
+000003d0: 3270 783b 2076 6572 7469 6361 6c2d 616c  2px; vertical-al
+000003e0: 6967 6e3a 6d69 6464 6c65 3b22 3e20 5468  ign:middle;"> Th
+000003f0: 6520 5069 7065 3c2f 613e 0d0a 3c70 3e0d  e Pipe</a>..<p>.
+00000400: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+00000410: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
+00000420: 6d63 662f 7468 6570 6970 652f 626c 6f62  mcf/thepipe/blob
+00000430: 2f6d 6169 6e2f 5245 4144 4d45 2e6d 6422  /main/README.md"
+00000440: 3e45 6e67 6c69 7368 3c2f 613e 207c 203c  >English</a> | <
+00000450: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000460: 6769 7468 7562 2e63 6f6d 2f65 6d63 662f  github.com/emcf/
+00000470: 7468 6570 6970 652f 626c 6f62 2f6d 6169  thepipe/blob/mai
+00000480: 6e2f 5245 4144 4d45 5f63 6e2e 6d64 223e  n/README_cn.md">
+00000490: e4b8 ade6 9687 3c2f 613e 0d0a 3c2f 703e  ......</a>..</p>
+000004a0: 0d0a 0d0a 5b21 5b63 6f64 6563 6f76 5d28  ....[![codecov](
+000004b0: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
+000004c0: 696f 2f67 682f 656d 6366 2f74 6865 7069  io/gh/emcf/thepi
+000004d0: 7065 2f67 7261 7068 2f62 6164 6765 2e73  pe/graph/badge.s
+000004e0: 7667 3f74 6f6b 656e 3d4f 4537 4355 4546  vg?token=OE7CUEF
+000004f0: 554c 3929 5d28 6874 7470 733a 2f2f 636f  UL9)](https://co
+00000500: 6465 636f 762e 696f 2f67 682f 656d 6366  decov.io/gh/emcf
+00000510: 2f74 6865 7069 7065 2920 215b 7079 7468  /thepipe) ![pyth
+00000520: 6f6e 2d67 682d 6163 7469 6f6e 5d28 6874  on-gh-action](ht
+00000530: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000540: 2f65 6d63 662f 7468 6570 6970 652f 6163  /emcf/thepipe/ac
+00000550: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+00000560: 7079 7468 6f6e 2d63 692e 796d 6c2f 6261  python-ci.yml/ba
+00000570: 6467 652e 7376 6729 203c 6120 6872 6566  dge.svg) <a href
+00000580: 3d22 6874 7470 733a 2f2f 7468 6570 692e  ="https://thepi.
+00000590: 7065 2f22 3e21 5b57 6562 7369 7465 5d28  pe/">![Website](
+000005a0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000005b0: 6c64 732e 696f 2f77 6562 7369 7465 3f75  lds.io/website?u
+000005c0: 726c 3d68 7474 7073 2533 4125 3246 2532  rl=https%3A%2F%2
+000005d0: 4674 6865 7069 7065 2e75 702e 7261 696c  Fthepipe.up.rail
+000005e0: 7761 792e 6170 7025 3246 266c 6162 656c  way.app%2F&label
+000005f0: 3d41 5049 2532 3073 7461 7475 7329 3c2f  =API%20status)</
+00000600: 613e 203c 6120 6872 6566 3d22 6874 7470  a> <a href="http
+00000610: 733a 2f2f 7468 6570 692e 7065 2f22 3e21  s://thepi.pe/">!
+00000620: 5b67 6574 2041 5049 5d28 6874 7470 733a  [get API](https:
+00000630: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000640: 2f62 6164 6765 2f41 5049 2d61 6363 6573  /badge/API-acces
+00000650: 732d 626c 7565 293c 2f61 3e20 3c61 2068  s-blue)</a> <a h
+00000660: 7265 663d 2268 7474 7073 3a2f 2f64 6973  ref="https://dis
+00000670: 636f 7264 2e67 672f 6258 664b 6547 7335  cord.gg/bXfKeGs5
+00000680: 7156 223e 215b 4a6f 696e 2064 6973 636f  qV">![Join disco
+00000690: 7264 5d28 6874 7470 733a 2f2f 696d 672e  rd](https://img.
+000006a0: 7368 6965 6c64 732e 696f 2f64 6973 636f  shields.io/disco
+000006b0: 7264 2f31 3232 3738 3036 3230 3034 3738  rd/1227806200478
+000006c0: 3034 3432 3734 3f63 6f6c 6f72 3d34 6636  044274?color=4f6
+000006d0: 3965 6626 6c61 6265 6c3d 4469 7363 6f72  9ef&label=Discor
+000006e0: 6426 6c6f 676f 3d64 6973 636f 7264 266c  d&logo=discord&l
+000006f0: 6f67 6f43 6f6c 6f72 3d66 6666 6666 6629  ogoColor=ffffff)
+00000700: 3c2f 613e 0d0a 0d0a 2323 2320 4665 6564  </a>....### Feed
+00000710: 2050 4446 732c 2055 524c 732c 2053 6c69   PDFs, URLs, Sli
+00000720: 6465 732c 2059 6f75 5475 6265 2076 6964  des, YouTube vid
+00000730: 656f 732c 2057 6f72 6420 646f 6373 2061  eos, Word docs a
+00000740: 6e64 206d 6f72 6520 696e 746f 2056 6973  nd more into Vis
+00000750: 696f 6e2d 4c61 6e67 7561 6765 206d 6f64  ion-Language mod
+00000760: 656c 7320 7769 7468 206f 6e65 206c 696e  els with one lin
+00000770: 6520 6f66 2063 6f64 6520 e29a a10d 0a0d  e of code ......
+00000780: 0a54 6865 2050 6970 6520 6973 2061 206d  .The Pipe is a m
+00000790: 756c 7469 6d6f 6461 6c2d 6669 7273 7420  ultimodal-first 
+000007a0: 746f 6f6c 2066 6f72 2066 6565 6469 6e67  tool for feeding
+000007b0: 2066 696c 6573 2061 6e64 2077 6562 2070   files and web p
+000007c0: 6167 6573 2069 6e74 6f20 7669 7369 6f6e  ages into vision
+000007d0: 2d6c 616e 6775 6167 6520 6d6f 6465 6c73  -language models
+000007e0: 2073 7563 6820 6173 2047 5054 2d34 562e   such as GPT-4V.
+000007f0: 2049 7420 6973 2062 6573 7420 666f 7220   It is best for 
+00000800: 4c4c 4d20 616e 6420 5241 4720 6170 706c  LLM and RAG appl
+00000810: 6963 6174 696f 6e73 2074 6861 7420 7761  ications that wa
+00000820: 6e74 2074 6f20 7375 7070 6f72 7420 636f  nt to support co
+00000830: 6d70 7265 6865 6e73 6976 6520 7465 7874  mprehensive text
+00000840: 7561 6c20 616e 6420 7669 7375 616c 2075  ual and visual u
+00000850: 6e64 6572 7374 616e 6469 6e67 2061 6372  nderstanding acr
+00000860: 6f73 7320 6120 7769 6465 2072 616e 6765  oss a wide range
+00000870: 206f 6620 6461 7461 2073 6f75 7263 6573   of data sources
+00000880: 2e20 5468 6520 5069 7065 2069 7320 6176  . The Pipe is av
+00000890: 6169 6c61 626c 6520 6173 2061 2068 6f73  ailable as a hos
+000008a0: 7465 6420 4150 4920 6174 205b 7468 6570  ted API at [thep
+000008b0: 692e 7065 5d28 6874 7470 733a 2f2f 7468  i.pe](https://th
+000008c0: 6570 692e 7065 292c 206f 7220 6974 2063  epi.pe), or it c
+000008d0: 616e 2062 6520 7365 7420 7570 206c 6f63  an be set up loc
+000008e0: 616c 6c79 2069 6620 796f 7520 6861 7665  ally if you have
+000008f0: 2074 6865 2074 6865 2063 6f6d 7075 7465   the the compute
+00000900: 2e0d 0a0d 0a21 5b53 6369 656e 6365 2061  .....![Science a
+00000910: 7373 6973 7461 6e74 2064 656d 6f5d 2868  ssistant demo](h
+00000920: 7474 7073 3a2f 2f72 706e 7574 7a65 6d75  ttps://rpnutzemu
+00000930: 7462 7275 6d63 7a77 7675 652e 7375 7061  tbrumczwvue.supa
+00000940: 6261 7365 2e63 6f2f 7374 6f72 6167 652f  base.co/storage/
+00000950: 7631 2f6f 626a 6563 742f 7075 626c 6963  v1/object/public
+00000960: 2f61 7373 6574 732f 7363 6965 6e63 655f  /assets/science_
+00000970: 6173 7369 7374 616e 7470 7932 2e70 6e67  assistantpy2.png
+00000980: 290d 0a0d 0a0d 0a23 2320 4665 6174 7572  )......## Featur
+00000990: 6573 20f0 9f8c 9f0d 0a0d 0a2d 2045 7874  es ........- Ext
+000009a0: 7261 6374 7320 7465 7874 2061 6e64 2076  racts text and v
+000009b0: 6973 7561 6c73 2066 726f 6d20 6669 6c65  isuals from file
+000009c0: 7320 6f72 2077 6562 2070 6167 6573 20f0  s or web pages .
+000009d0: 9f93 9a0d 0a2d 204f 7574 7075 7473 2063  .....- Outputs c
+000009e0: 6875 6e6b 7320 6f70 7469 6d69 7a65 6420  hunks optimized 
+000009f0: 666f 7220 6d75 6c74 696d 6f64 616c 204c  for multimodal L
+00000a00: 4c4d 7320 616e 6420 5241 4720 6672 616d  LMs and RAG fram
+00000a10: 6577 6f72 6b73 20f0 9f96 bcef b88f 0d0a  eworks .........
+00000a20: 2d20 496e 7465 7270 7265 7420 636f 6d70  - Interpret comp
+00000a30: 6c65 7820 5044 4673 2c20 7765 6220 7061  lex PDFs, web pa
+00000a40: 6765 732c 2064 6f63 732c 2076 6964 656f  ges, docs, video
+00000a50: 732c 2064 6174 612c 2061 6e64 206d 6f72  s, data, and mor
+00000a60: 6520 f09f a7a0 0d0a 2d20 4175 746f 2d63  e ......- Auto-c
+00000a70: 6f6d 7072 6573 7320 7072 6f6d 7074 7320  ompress prompts 
+00000a80: 6578 6365 6564 696e 6720 796f 7572 2063  exceeding your c
+00000a90: 686f 7365 6e20 746f 6b65 6e20 6c69 6d69  hosen token limi
+00000aa0: 7420 f09f 93a6 0d0a 2d20 576f 726b 7320  t ......- Works 
+00000ab0: 6576 656e 2077 6974 6820 6d69 7373 696e  even with missin
+00000ac0: 6720 6669 6c65 2065 7874 656e 7369 6f6e  g file extension
+00000ad0: 732c 2069 6e2d 6d65 6d6f 7279 2064 6174  s, in-memory dat
+00000ae0: 6120 7374 7265 616d 7320 f09f 92be 0d0a  a streams ......
+00000af0: 2d20 576f 726b 7320 7769 7468 2063 6f64  - Works with cod
+00000b00: 6562 6173 6573 2c20 6769 7420 7265 706f  ebases, git repo
+00000b10: 732c 2061 6e64 2063 7573 746f 6d20 696e  s, and custom in
+00000b20: 7465 6772 6174 696f 6e73 20f0 9f8c 900d  tegrations .....
+00000b30: 0a2d 204d 756c 7469 2d74 6872 6561 6465  .- Multi-threade
+00000b40: 6420 e29a a1ef b88f 0d0a 0d0a 2323 2047  d ..........## G
+00000b50: 6574 7469 6e67 2053 7461 7274 6564 2020  etting Started  
+00000b60: f09f 9a80 0d0a 0d0a 5468 6520 5069 7065  ........The Pipe
+00000b70: 2063 616e 2072 6561 6420 6120 7769 6465   can read a wide
+00000b80: 2061 7272 6179 206f 6620 6669 6c65 2074   array of file t
+00000b90: 7970 6573 2c20 616e 6420 7468 7573 2068  ypes, and thus h
+00000ba0: 6173 206d 616e 7920 6465 7065 6e64 656e  as many dependen
+00000bb0: 6369 6573 2074 6861 7420 6d75 7374 2062  cies that must b
+00000bc0: 6520 696e 7374 616c 6c65 6420 7365 7061  e installed sepa
+00000bd0: 7261 7465 6c79 2e20 4974 2061 6c73 6f20  rately. It also 
+00000be0: 7265 7175 6972 6573 2061 2073 7472 6f6e  requires a stron
+00000bf0: 6720 6d61 6368 696e 6520 666f 7220 676f  g machine for go
+00000c00: 6f64 2072 6573 706f 6e73 6520 7469 6d65  od response time
+00000c10: 732e 2046 6f72 2074 6869 7320 7265 6173  s. For this reas
+00000c20: 6f6e 2c20 7765 2068 6f73 7420 6974 2061  on, we host it a
+00000c30: 7320 616e 2041 5049 2074 6861 7420 776f  s an API that wo
+00000c40: 726b 7320 6f75 742d 6f66 2d74 6865 2d62  rks out-of-the-b
+00000c50: 6f78 2e20 0d0a 0d0a 4669 7273 742c 2069  ox. ....First, i
+00000c60: 6e73 7461 6c6c 2054 6865 2050 6970 652e  nstall The Pipe.
+00000c70: 200d 0a60 6060 0d0a 7069 7020 696e 7374   ..```..pip inst
+00000c80: 616c 6c20 7468 6570 6970 655f 6170 690d  all thepipe_api.
+00000c90: 0a60 6060 0d0a 0d0a 5468 6520 5069 7065  .```....The Pipe
+00000ca0: 2069 7320 6176 6169 6c61 626c 6520 6173   is available as
+00000cb0: 2061 2068 6f73 7465 6420 4150 492c 206f   a hosted API, o
+00000cc0: 7220 6974 2063 616e 2062 6520 7365 7420  r it can be set 
+00000cd0: 7570 206c 6f63 616c 6c79 2e20 416e 2041  up locally. An A
+00000ce0: 5049 206b 6579 2069 7320 7265 636f 6d6d  PI key is recomm
+00000cf0: 656e 6465 6420 666f 7220 6f75 742d 6f66  ended for out-of
+00000d00: 2d74 6865 2d62 6f78 2066 756e 6374 696f  -the-box functio
+00000d10: 6e61 6c69 7479 2028 616c 7465 726e 6174  nality (alternat
+00000d20: 6976 656c 792c 2073 6565 2074 6865 206c  ively, see the l
+00000d30: 6f63 616c 2069 6e73 7461 6c6c 6174 696f  ocal installatio
+00000d40: 6e20 7365 6374 696f 6e29 2e20 456e 7375  n section). Ensu
+00000d50: 7265 2074 6865 2060 5448 4550 4950 455f  re the `THEPIPE_
+00000d60: 4150 495f 4b45 5960 2065 6e76 6972 6f6e  API_KEY` environ
+00000d70: 6d65 6e74 2076 6172 6961 626c 6520 6973  ment variable is
+00000d80: 2073 6574 2e20 446f 6e27 7420 6861 7665   set. Don't have
+00000d90: 2061 206b 6579 2079 6574 3f20 5b47 6574   a key yet? [Get
+00000da0: 206f 6e65 2068 6572 655d 2868 7474 7073   one here](https
+00000db0: 3a2f 2f74 6865 7069 2e70 6529 2e0d 0a0d  ://thepi.pe)....
+00000dc0: 0a4e 6f77 2079 6f75 2063 616e 2065 7874  .Now you can ext
+00000dd0: 7261 6374 2063 6f6d 7072 6568 656e 7369  ract comprehensi
+00000de0: 7665 2074 6578 7420 616e 6420 7669 7375  ve text and visu
+00000df0: 616c 7320 6672 6f6d 2061 6e79 2066 696c  als from any fil
+00000e00: 653a 0d0a 6060 6070 7974 686f 6e0d 0a66  e:..```python..f
+00000e10: 726f 6d20 7468 6570 6970 655f 6170 6920  rom thepipe_api 
+00000e20: 696d 706f 7274 2074 6865 7069 7065 0d0a  import thepipe..
+00000e30: 6d65 7373 6167 6573 203d 2074 6865 7069  messages = thepi
+00000e40: 7065 2e65 7874 7261 6374 2822 6578 616d  pe.extract("exam
+00000e50: 706c 652e 7064 6622 290d 0a60 6060 0d0a  ple.pdf")..```..
+00000e60: 4f72 2077 6562 7369 7465 733a 0d0a 6060  Or websites:..``
+00000e70: 6070 7974 686f 6e0d 0a6d 6573 7361 6765  `python..message
+00000e80: 7320 3d20 7468 6570 6970 652e 6578 7472  s = thepipe.extr
+00000e90: 6163 7428 2268 7474 7073 3a2f 2f65 7861  act("https://exa
+00000ea0: 6d70 6c65 2e63 6f6d 2229 0d0a 6060 600d  mple.com")..```.
+00000eb0: 0a54 6865 6e20 6665 6564 2069 7420 696e  .Then feed it in
+00000ec0: 746f 2047 5054 2d34 5620 6c69 6b65 2073  to GPT-4V like s
+00000ed0: 6f3a 0d0a 6060 6070 7974 686f 6e0d 0a72  o:..```python..r
+00000ee0: 6573 706f 6e73 6520 3d20 6f70 656e 6169  esponse = openai
+00000ef0: 2e63 6861 742e 636f 6d70 6c65 7469 6f6e  .chat.completion
+00000f00: 732e 6372 6561 7465 280d 0a20 2020 206d  s.create(..    m
+00000f10: 6f64 656c 3d22 6770 742d 342d 7475 7262  odel="gpt-4-turb
+00000f20: 6f22 2c0d 0a20 2020 206d 6573 7361 6765  o",..    message
+00000f30: 7320 3d20 6d65 7373 6167 6573 2c0d 0a29  s = messages,..)
+00000f40: 0d0a 6060 600d 0a0d 0a21 5b4a 7573 7420  ..```....![Just 
+00000f50: 6361 6c6c 204f 7065 6e41 495d 2868 7474  call OpenAI](htt
+00000f60: 7073 3a2f 2f72 706e 7574 7a65 6d75 7462  ps://rpnutzemutb
+00000f70: 7275 6d63 7a77 7675 652e 7375 7061 6261  rumczwvue.supaba
+00000f80: 7365 2e63 6f2f 7374 6f72 6167 652f 7631  se.co/storage/v1
+00000f90: 2f6f 626a 6563 742f 7075 626c 6963 2f61  /object/public/a
+00000fa0: 7373 6574 732f 494d 475f 3031 3830 2e6a  ssets/IMG_0180.j
+00000fb0: 7067 290d 0a0d 0a59 6f75 2063 616e 2061  pg)....You can a
+00000fc0: 6c73 6f20 7573 6520 5468 6520 5069 7065  lso use The Pipe
+00000fd0: 2066 726f 6d20 7468 6520 636f 6d6d 616e   from the comman
+00000fe0: 6420 6c69 6e65 2e20 4865 7265 2773 2068  d line. Here's h
+00000ff0: 6f77 2074 6f20 7265 6375 7273 6976 656c  ow to recursivel
+00001000: 7920 6578 7472 6163 7420 6672 6f6d 2061  y extract from a
+00001010: 2064 6972 6563 746f 7279 2c20 6d61 7463   directory, matc
+00001020: 6869 6e67 206f 6e6c 7920 6669 6c65 7320  hing only files 
+00001030: 636f 6e74 6169 6e69 6e67 2061 2073 7562  containing a sub
+00001040: 7374 7269 6e67 2028 696e 2074 6869 7320  string (in this 
+00001050: 6578 616d 706c 652c 2074 7970 6573 6372  example, typescr
+00001060: 6970 7420 6669 6c65 7329 2061 6e64 2069  ipt files) and i
+00001070: 676e 6f72 6520 6669 6c65 7320 636f 6e74  gnore files cont
+00001080: 6169 6e69 6e67 206f 7468 6572 2073 7562  aining other sub
+00001090: 7374 7269 6e67 7320 2869 6e20 7468 6973  strings (in this
+000010a0: 2065 7861 6d70 6c65 2c20 616e 7974 6869   example, anythi
+000010b0: 6e67 2069 6e20 7468 6520 2274 6573 7473  ng in the "tests
+000010c0: 2220 666f 6c64 6572 293a 0d0a 6060 6062  " folder):..```b
+000010d0: 6173 680d 0a74 6865 7069 7065 2070 6174  ash..thepipe pat
+000010e0: 682f 746f 2f66 6f6c 6465 7220 2d2d 6d61  h/to/folder --ma
+000010f0: 7463 6820 7473 7820 2d2d 6967 6e6f 7265  tch tsx --ignore
+00001100: 2074 6573 7473 0d0a 6060 600d 0a0d 0a0d   tests..```.....
+00001110: 0a23 2320 5375 7070 6f72 7465 6420 4669  .## Supported Fi
+00001120: 6c65 2054 7970 6573 20f0 9f93 9a0d 0a0d  le Types .......
+00001130: 0a7c 2053 6f75 7263 6520 5479 7065 2020  .| Source Type  
+00001140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001150: 2020 2020 2020 2020 207c 2049 6e70 7574           | Input
+00001160: 2074 7970 6573 2020 2020 2020 2020 7c20   types        | 
+00001170: 546f 6b65 6e20 436f 6d70 7265 7373 696f  Token Compressio
+00001180: 6e20 f09f 979c efb8 8f20 7c20 496d 6167  n ....... | Imag
+00001190: 6520 4578 7472 6163 7469 6f6e 20f0 9f91  e Extraction ...
+000011a0: 81ef b88f 207c 204e 6f74 6573 20f0 9f93  .... | Notes ...
+000011b0: 8c20 2020 2020 2020 2020 2020 2020 2020  .               
+000011c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011e0: 2020 207c 0d0a 7c2d 2d2d 2d2d 2d2d 2d2d     |..|---------
+000011f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001200: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d  --------------|-
+00001210: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001230: 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d  ---------|------
+00001240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  -------------|--
+00001250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001260: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
+00001270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001290: 2d2d 2d2d 2d2d 2d2d 2d2d 7c0d 0a7c 2044  ----------|..| D
+000012a0: 6972 6563 746f 7279 2020 2020 2020 2020  irectory        
+000012b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012c0: 2020 2020 207c 2041 6e79 2060 2f70 6174       | Any `/pat
+000012d0: 682f 746f 2f64 6972 6563 746f 7279 6020  h/to/directory` 
+000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012f0: 7c20 e29c 94ef b88f 2020 2020 2020 2020  | ......        
+00001300: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
+00001310: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00001320: 4578 7472 6163 7473 2066 726f 6d20 616c  Extracts from al
+00001330: 6c20 6669 6c65 7320 696e 2064 6972 6563  l files in direc
+00001340: 746f 7279 2c20 7375 7070 6f72 7473 206d  tory, supports m
+00001350: 6174 6368 2061 6e64 2069 676e 6f72 6520  atch and ignore 
+00001360: 7061 7474 6572 6e73 207c 0d0a 7c20 436f  patterns |..| Co
+00001370: 6465 2020 2020 2020 2020 2020 2020 2020  de              
+00001380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001390: 2020 2020 7c20 602e 7079 602c 2060 2e74      | `.py`, `.t
+000013a0: 7378 602c 2060 2e6a 7360 2c20 602e 6874  sx`, `.js`, `.ht
+000013b0: 6d6c 602c 2060 2e63 7373 602c 2060 2e63  ml`, `.css`, `.c
+000013c0: 7070 602c 2065 7463 207c 20e2 9c94 efb8  pp`, etc | .....
+000013d0: 8f20 2876 6172 6965 7329 2020 207c 20e2  . (varies)   | .
+000013e0: 9d8c 2020 2020 2020 2020 2020 2020 2020  ..              
+000013f0: 207c 2043 6f6d 6269 6e65 7320 616c 6c20   | Combines all 
+00001400: 636f 6465 2066 696c 6573 2e20 602e 6360  code files. `.c`
+00001410: 2c20 602e 6370 7060 2c20 602e 7079 6020  , `.cpp`, `.py` 
+00001420: 6172 6520 636f 6d70 7265 7373 6962 6c65  are compressible
+00001430: 2077 6974 6820 6374 6167 732c 206f 7468   with ctags, oth
+00001440: 6572 7320 6172 6520 6e6f 7420 7c0d 0a7c  ers are not |..|
+00001450: 2050 6c61 696e 7465 7874 2020 2020 2020   Plaintext      
+00001460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001470: 2020 2020 2020 207c 2060 2e74 7874 602c         | `.txt`,
+00001480: 2060 2e6d 6460 2c20 602e 7274 6660 2c20   `.md`, `.rtf`, 
+00001490: 6574 6320 2020 2020 2020 2020 2020 2020  etc             
+000014a0: 2020 7c20 e29c 94ef b88f 2020 2020 2020    | ......      
+000014b0: 2020 2020 2020 2020 207c 20e2 9d8c 2020           | ...  
+000014c0: 2020 2020 2020 2020 2020 2020 207c 2052               | R
+000014d0: 6567 756c 6172 2074 6578 7420 6669 6c65  egular text file
+000014e0: 7320 2020 2020 2020 2020 2020 2020 2020  s               
 000014f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001500: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
-00001510: 9d8c 2020 2020 2020 2020 2020 2020 2020  ..              
-00001520: 207c 20e2 9c94 efb8 8f20 2020 2020 2020   | ......       
-00001530: 2020 2020 2020 2020 7c20 4578 7472 6163          | Extrac
-00001540: 7473 2063 6f64 652c 206d 6172 6b64 6f77  ts code, markdow
-00001550: 6e2c 2061 6e64 2069 6d61 6765 7320 6672  n, and images fr
-00001560: 6f6d 204a 7570 7974 6572 206e 6f74 6562  om Jupyter noteb
-00001570: 6f6f 6b73 2020 2020 2020 2020 2020 2020  ooks            
-00001580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001590: 2020 2020 2020 7c0d 0a7c 204d 6963 726f        |..| Micro
-000015a0: 736f 6674 2057 6f72 6420 446f 6375 6d65  soft Word Docume
-000015b0: 6e74 2020 2020 2020 2020 2020 2020 2020  nt              
-000015c0: 207c 2060 2e64 6f63 7860 2020 2020 2020   | `.docx`      
-000015d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015e0: 2020 2020 2020 2020 2020 207c 20e2 9c94             | ...
-000015f0: efb8 8f20 2020 2020 2020 2020 2020 2020  ...             
-00001600: 2020 7c20 e29c 94ef b88f 2020 2020 2020    | ......      
-00001610: 2020 2020 2020 2020 207c 2045 7874 7261           | Extra
-00001620: 6374 7320 7465 7874 2061 6e64 2069 6d61  cts text and ima
-00001630: 6765 7320 6672 6f6d 2057 6f72 6420 646f  ges from Word do
-00001640: 6375 6d65 6e74 7320 2020 2020 2020 2020  cuments         
-00001650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001660: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00001670: 0d0a 7c20 4d69 6372 6f73 6f66 7420 506f  ..| Microsoft Po
-00001680: 7765 7250 6f69 6e74 2050 7265 7365 6e74  werPoint Present
-00001690: 6174 696f 6e20 2020 2020 7c20 602e 7070  ation     | `.pp
-000016a0: 7478 6020 2020 2020 2020 2020 2020 2020  tx`             
-000016b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016c0: 2020 2020 7c20 e29c 94ef b88f 2020 2020      | ......    
-000016d0: 2020 2020 2020 2020 2020 207c 20e2 9c94             | ...
-000016e0: efb8 8f20 2020 2020 2020 2020 2020 2020  ...             
-000016f0: 2020 7c20 4578 7472 6163 7473 2074 6578    | Extracts tex
-00001700: 7420 616e 6420 696d 6167 6573 2066 726f  t and images fro
-00001710: 6d20 506f 7765 7250 6f69 6e74 2070 7265  m PowerPoint pre
-00001720: 7365 6e74 6174 696f 6e73 2020 2020 2020  sentations      
-00001730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001740: 2020 2020 2020 2020 7c0d 0a7c 2056 6964          |..| Vid
-00001750: 656f 2020 2020 2020 2020 2020 2020 2020  eo              
-00001760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001770: 2020 207c 2060 2e6d 7034 602c 2060 2e61     | `.mp4`, `.a
-00001780: 7669 602c 2060 2e6d 6f76 602c 2060 2e77  vi`, `.mov`, `.w
-00001790: 6d76 6020 2020 2020 7c20 e29c 94ef b88f  mv`     | ......
-000017a0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000017b0: 20e2 9c94 efb8 8f20 2020 2020 2020 2020   ......         
-000017c0: 2020 2020 2020 207c 2045 7874 7261 6374         | Extract
-000017d0: 7320 6672 616d 6573 2066 726f 6d20 7669  s frames from vi
-000017e0: 6465 6f20 6669 6c65 733b 2073 7570 706f  deo files; suppo
-000017f0: 7274 7320 6672 616d 6520 6578 7472 6163  rts frame extrac
-00001800: 7469 6f6e 2061 6e64 204f 4352 2066 6f72  tion and OCR for
-00001810: 2074 6578 7420 6578 7472 6163 7469 6f6e   text extraction
-00001820: 2066 726f 6d20 6672 616d 6573 207c 0d0a   from frames |..
-00001830: 7c20 4175 6469 6f20 2020 2020 2020 2020  | Audio         
+00001500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001510: 2020 2020 2020 207c 0d0a 7c20 5044 4620         |..| PDF 
+00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001540: 2020 7c20 602e 7064 6660 2020 2020 2020    | `.pdf`      
+00001550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001560: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
+00001570: 94ef b88f 2020 2020 2020 2020 2020 2020  ....            
+00001580: 2020 207c 20e2 9c94 efb8 8f20 2020 207c     | ......    |
+00001590: 2045 7874 7261 6374 7320 7465 7874 2061   Extracts text a
+000015a0: 6e64 2069 6d61 6765 7320 6f66 2065 6163  nd images of eac
+000015b0: 6820 7061 6765 3b20 6361 6e20 7573 6520  h page; can use 
+000015c0: 4149 2066 6f72 2065 7874 7261 6374 696f  AI for extractio
+000015d0: 6e20 6f66 2074 6162 6c65 2064 6174 6120  n of table data 
+000015e0: 616e 6420 2069 6d61 6765 7320 7769 7468  and  images with
+000015f0: 696e 2070 6167 6573 207c 0d0a 7c20 496d  in pages |..| Im
+00001600: 6167 6520 2020 2020 2020 2020 2020 2020  age             
+00001610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001620: 2020 2020 7c20 602e 6a70 6760 2c20 602e      | `.jpg`, `.
+00001630: 6a70 6567 602c 2060 2e70 6e67 6020 7c20  jpeg`, `.png` | 
+00001640: e29d 8c20 2020 2020 2020 2020 2020 2020  ...             
+00001650: 2020 207c 20e2 9c94 efb8 8f20 2020 2020     | ......     
+00001660: 2020 2020 2020 2020 207c 2045 7874 7261           | Extra
+00001670: 6374 7320 696d 6167 6573 2c20 7573 6573  cts images, uses
+00001680: 204f 4352 2069 6620 7465 7874 5f6f 6e6c   OCR if text_onl
+00001690: 7920 2020 2020 2020 2020 2020 2020 2020  y               
+000016a0: 2020 2020 2020 2020 207c 0d0a 7c20 5370           |..| Sp
+000016b0: 7265 6164 7368 6565 7420 2020 2020 2020  readsheet       
+000016c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016d0: 2020 2020 7c20 602e 6373 7660 2c20 602e      | `.csv`, `.
+000016e0: 786c 7360 2c20 602e 786c 7378 6020 2020  xls`, `.xlsx`   
+000016f0: 2020 2020 2020 2020 2020 7c20 e29c 94ef            | ....
+00001700: b88f 2020 2020 2020 2020 2020 2020 2020  ..              
+00001710: 2020 7c20 e29d 8c20 2020 2020 2020 2020    | ...         
+00001720: 2020 2020 2020 7c20 4578 7472 6163 7473        | Extracts
+00001730: 2064 6174 6120 6672 6f6d 2073 7072 6561   data from sprea
+00001740: 6473 6865 6574 733b 2063 6f6e 7665 7274  dsheets; convert
+00001750: 7320 6561 6368 2072 6f77 2069 6e74 6f20  s each row into 
+00001760: 6120 4a53 4f4e 2066 6f72 6d61 7474 6564  a JSON formatted
+00001770: 2073 7472 696e 6720 2020 2020 2020 2020   string         
+00001780: 7c0d 0a7c 204a 7570 7974 6572 204e 6f74  |..| Jupyter Not
+00001790: 6562 6f6f 6b20 2020 2020 2020 2020 2020  ebook           
+000017a0: 2020 2020 2020 2020 2020 207c 2060 2e69             | `.i
+000017b0: 7079 6e62 6020 2020 2020 2020 2020 2020  pynb`           
+000017c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017d0: 2020 2020 207c 20e2 9d8c 2020 2020 2020       | ...      
+000017e0: 2020 2020 2020 2020 207c 20e2 9c94 efb8           | .....
+000017f0: 8f20 2020 2020 2020 2020 2020 2020 2020  .               
+00001800: 7c20 4578 7472 6163 7473 2063 6f64 652c  | Extracts code,
+00001810: 206d 6172 6b64 6f77 6e2c 2061 6e64 2069   markdown, and i
+00001820: 6d61 6765 7320 6672 6f6d 204a 7570 7974  mages from Jupyt
+00001830: 6572 206e 6f74 6562 6f6f 6b73 2020 2020  er notebooks    
 00001840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001850: 2020 2020 2020 2020 7c20 602e 6d70 3360          | `.mp3`
-00001860: 2c20 602e 7761 7660 2020 2020 2020 2020  , `.wav`        
-00001870: 2020 7c20 e29c 94ef b88f 2020 2020 2020    | ......      
-00001880: 2020 2020 2020 2020 207c 20e2 9d8c 2020           | ...  
-00001890: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000018a0: 4578 7472 6163 7473 2074 6578 7420 6672  Extracts text fr
-000018b0: 6f6d 2061 7564 696f 2066 696c 6573 3b20  om audio files; 
-000018c0: 7375 7070 6f72 7473 2073 7065 6563 682d  supports speech-
-000018d0: 746f 2d74 6578 7420 636f 6e76 6572 7369  to-text conversi
-000018e0: 6f6e 2020 2020 2020 2020 7c20 0d0a 7c20  on        | ..| 
-000018f0: 5765 6273 6974 6520 2020 2020 2020 2020  Website         
-00001900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001910: 2020 2020 2020 7c20 5552 4c73 2028 696e        | URLs (in
-00001920: 7075 7473 2073 7461 7274 696e 6720 7769  puts starting wi
-00001930: 7468 2060 6874 7470 602c 2060 6874 7470  th `http`, `http
-00001940: 7360 2c20 6066 7470 6029 2020 2020 2020  s`, `ftp`)      
-00001950: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
-00001960: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00001970: 20e2 9c94 efb8 8f20 2020 207c 2045 7874   ......    | Ext
-00001980: 7261 6374 7320 7465 7874 2066 726f 6d20  racts text from 
-00001990: 7765 6220 7061 6765 2061 6c6f 6e67 2077  web page along w
-000019a0: 6974 6820 696d 6167 6520 286f 7220 696d  ith image (or im
-000019b0: 6167 6573 2069 6620 7363 726f 6c6c 6162  ages if scrollab
-000019c0: 6c65 293b 2074 6578 742d 6f6e 6c79 2065  le); text-only e
-000019d0: 7874 7261 6374 696f 6e20 6176 6169 6c61  xtraction availa
-000019e0: 626c 6520 2020 2020 2020 2020 207c 0d0a  ble          |..
-000019f0: 7c20 4769 7448 7562 2052 6570 6f73 6974  | GitHub Reposit
-00001a00: 6f72 7920 2020 2020 2020 2020 2020 2020  ory             
-00001a10: 2020 2020 2020 2020 7c20 4769 7448 7562          | GitHub
-00001a20: 2072 6570 6f20 5552 4c73 2028 696e 7075   repo URLs (inpu
-00001a30: 7473 2073 7461 7274 696e 6720 7769 7468  ts starting with
-00001a40: 2060 6874 7470 733a 2f2f 6769 7468 7562   `https://github
-00001a50: 2e63 6f6d 6020 6f72 2060 6874 7470 733a  .com` or `https:
-00001a60: 2f2f 7777 772e 6769 7468 7562 2e63 6f6d  //www.github.com
-00001a70: 6029 2020 2020 2020 2020 2020 2020 2020  `)              
-00001a80: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
-00001a90: 94ef b88f 2020 2020 2020 2020 2020 2020  ....            
-00001aa0: 2020 207c 20e2 9c94 efb8 8f20 2020 2020     | ......     
-00001ab0: 2020 2020 2020 2020 2020 207c 2045 7874             | Ext
-00001ac0: 7261 6374 7320 6672 6f6d 2047 6974 4875  racts from GitHu
-00001ad0: 6220 7265 706f 7369 746f 7269 6573 3b20  b repositories; 
-00001ae0: 7375 7070 6f72 7473 2062 7261 6e63 6820  supports branch 
-00001af0: 7370 6563 6966 6963 6174 696f 6e20 2020  specification   
-00001b00: 2020 2020 2020 7c0d 0a7c 2059 6f75 5475        |..| YouTu
-00001b10: 6265 2056 6964 656f 2020 2020 2020 2020  be Video        
-00001b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b30: 207c 2059 6f75 5475 6265 2076 6964 656f   | YouTube video
-00001b40: 2055 524c 7320 2869 6e70 7574 7320 7374   URLs (inputs st
-00001b50: 6172 7469 6e67 2077 6974 6820 6068 7474  arting with `htt
-00001b60: 7073 3a2f 2f79 6f75 7475 6265 2e63 6f6d  ps://youtube.com
-00001b70: 6020 6f72 2060 6874 7470 733a 2f2f 7777  ` or `https://ww
-00001b80: 772e 796f 7574 7562 652e 636f 6d60 2920  w.youtube.com`) 
-00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ba0: 2020 2020 7c20 e29c 94ef b88f 2020 2020      | ......    
-00001bb0: 2020 2020 2020 2020 2020 207c 20e2 9c94             | ...
-00001bc0: efb8 8f20 2020 2020 2020 2020 2020 2020  ...             
-00001bd0: 2020 207c 2045 7874 7261 6374 7320 6672     | Extracts fr
-00001be0: 616d 6573 2061 6e64 2074 7261 6e73 6372  ames and transcr
-00001bf0: 6970 7420 6672 6f6d 2059 6f75 5475 6265  ipt from YouTube
-00001c00: 2076 6964 656f 7320 696e 2070 6572 2d6d   videos in per-m
-00001c10: 696e 7574 6520 6368 756e 6b73 2020 2020  inute chunks    
-00001c20: 2020 2020 2020 7c0d 0a7c 205a 4950 2046        |..| ZIP F
-00001c30: 696c 6520 2020 2020 2020 2020 2020 2020  ile             
-00001c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c50: 207c 2060 2e7a 6970 6020 2020 2020 2020   | `.zip`       
-00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c70: 2020 2020 2020 2020 2020 207c 20e2 9c94             | ...
-00001c80: efb8 8f20 2020 2020 2020 2020 2020 2020  ...             
-00001c90: 2020 7c20 e29c 94ef b88f 2020 2020 2020    | ......      
-00001ca0: 2020 2020 2020 2020 2020 7c20 4578 7472            | Extr
-00001cb0: 6163 7473 2063 6f6e 7465 6e74 7320 6f66  acts contents of
-00001cc0: 205a 4950 2066 696c 6573 3b20 7375 7070   ZIP files; supp
-00001cd0: 6f72 7473 206e 6573 7465 6420 6469 7265  orts nested dire
-00001ce0: 6374 6f72 7920 6578 7472 6163 7469 6f6e  ctory extraction
-00001cf0: 2020 2020 207c 0d0a 0d0a 2323 2048 6f77       |....## How
-00001d00: 2069 7420 776f 726b 7320 f09f 9ba0 efb8   it works ......
-00001d10: 8f0d 0a0d 0a54 6865 2069 6e70 7574 2073  .....The input s
-00001d20: 6f75 7263 6520 6973 2065 6974 6865 7220  ource is either 
-00001d30: 6120 6669 6c65 2070 6174 682c 2061 2055  a file path, a U
-00001d40: 524c 2c20 6f72 2061 2064 6972 6563 746f  RL, or a directo
-00001d50: 7279 2e20 5468 6520 7069 7065 2077 696c  ry. The pipe wil
-00001d60: 6c20 6578 7472 6163 7420 696e 666f 726d  l extract inform
-00001d70: 6174 696f 6e20 6672 6f6d 2074 6865 2073  ation from the s
-00001d80: 6f75 7263 6520 616e 6420 7072 6f63 6573  ource and proces
-00001d90: 7320 6974 2066 6f72 2064 6f77 6e73 7472  s it for downstr
-00001da0: 6561 6d20 7573 6520 7769 7468 205b 6c61  eam use with [la
-00001db0: 6e67 7561 6765 206d 6f64 656c 735d 2868  nguage models](h
-00001dc0: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
-00001dd0: 6469 612e 6f72 672f 7769 6b69 2f4c 6172  dia.org/wiki/Lar
-00001de0: 6765 5f6c 616e 6775 6167 655f 6d6f 6465  ge_language_mode
-00001df0: 6c29 2c20 5b76 6973 696f 6e20 7472 616e  l), [vision tran
-00001e00: 7366 6f72 6d65 7273 5d28 6874 7470 733a  sformers](https:
-00001e10: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
-00001e20: 7267 2f77 696b 692f 5669 7369 6f6e 5f74  rg/wiki/Vision_t
-00001e30: 7261 6e73 666f 726d 6572 292c 206f 7220  ransformer), or 
-00001e40: 5b76 6973 696f 6e2d 6c61 6e67 7561 6765  [vision-language
-00001e50: 206d 6f64 656c 735d 2868 7474 7073 3a2f   models](https:/
-00001e60: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
-00001e70: 3330 342e 3030 3638 3529 2e20 5468 6520  304.00685). The 
-00001e80: 6f75 7470 7574 2066 726f 6d20 7468 6520  output from the 
-00001e90: 7069 7065 2069 7320 6120 7365 6e73 6962  pipe is a sensib
-00001ea0: 6c65 206c 6973 7420 6f66 206d 756c 7469  le list of multi
-00001eb0: 6d6f 6461 6c20 6d65 7373 6167 6573 2072  modal messages r
-00001ec0: 6570 7265 7365 6e74 696e 6720 6368 756e  epresenting chun
-00001ed0: 6b73 206f 6620 7468 6520 6578 7472 6163  ks of the extrac
-00001ee0: 7465 6420 696e 666f 726d 6174 696f 6e2c  ted information,
-00001ef0: 2063 6172 6566 756c 6c79 2063 7261 6674   carefully craft
-00001f00: 6564 2074 6f20 6669 7420 7769 7468 696e  ed to fit within
-00001f10: 2063 6f6e 7465 7874 2077 696e 646f 7773   context windows
-00001f20: 2066 6f72 2061 6e79 206d 6f64 656c 7320   for any models 
-00001f30: 6672 6f6d 205b 6765 6d6d 612d 3762 5d28  from [gemma-7b](
-00001f40: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-00001f50: 6163 652e 636f 2f67 6f6f 676c 652f 6765  ace.co/google/ge
-00001f60: 6d6d 612d 3762 2920 746f 205b 4750 542d  mma-7b) to [GPT-
-00001f70: 345d 2868 7474 7073 3a2f 2f6f 7065 6e61  4](https://opena
-00001f80: 692e 636f 6d2f 6770 742d 3429 2e20 5468  i.com/gpt-4). Th
-00001f90: 6520 6d65 7373 6167 6573 2072 6574 7572  e messages retur
-00001fa0: 6e65 6420 7368 6f75 6c64 206c 6f6f 6b20  ned should look 
-00001fb0: 6c69 6b65 2074 6869 733a 0d0a 6060 606a  like this:..```j
-00001fc0: 736f 6e0d 0a5b 0d0a 2020 7b0d 0a20 2020  son..[..  {..   
-00001fd0: 2022 726f 6c65 223a 2022 7573 6572 222c   "role": "user",
-00001fe0: 0d0a 2020 2020 2263 6f6e 7465 6e74 223a  ..    "content":
-00001ff0: 205b 0d0a 2020 2020 2020 7b0d 0a20 2020   [..      {..   
-00002000: 2020 2020 2022 7479 7065 223a 2022 7465       "type": "te
-00002010: 7874 222c 0d0a 2020 2020 2020 2020 2274  xt",..        "t
-00002020: 6578 7422 3a20 222e 2e2e 220d 0a20 2020  ext": "..."..   
-00002030: 2020 207d 2c0d 0a20 2020 2020 207b 0d0a     },..      {..
-00002040: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-00002050: 2269 6d61 6765 5f75 726c 222c 0d0a 2020  "image_url",..  
-00002060: 2020 2020 2020 2269 6d61 6765 5f75 726c        "image_url
-00002070: 223a 207b 0d0a 2020 2020 2020 2020 2020  ": {..          
-00002080: 2275 726c 223a 2022 6461 7461 3a69 6d61  "url": "data:ima
-00002090: 6765 2f6a 7065 673b 6261 7365 3634 2c2e  ge/jpeg;base64,.
-000020a0: 2e2e 220d 0a20 2020 2020 2020 207d 0d0a  .."..        }..
-000020b0: 2020 2020 2020 7d0d 0a20 2020 205d 0d0a        }..    ]..
-000020c0: 2020 7d0d 0a5d 0d0a 6060 600d 0a49 6620    }..]..```..If 
-000020d0: 796f 7520 7761 6e74 2074 6f20 6665 6564  you want to feed
-000020e0: 2074 6865 7365 206d 6573 7361 6765 7320   these messages 
-000020f0: 6469 7265 6374 6c79 2069 6e74 6f20 7468  directly into th
-00002100: 6520 6d6f 6465 6c2c 2069 7420 6973 2069  e model, it is i
-00002110: 6d70 6f72 7461 6e74 2074 6f20 6265 206d  mportant to be m
-00002120: 696e 6466 756c 206f 6620 7468 6520 746f  indful of the to
-00002130: 6b65 6e20 6c69 6d69 742e 0d0a 4f70 656e  ken limit...Open
-00002140: 4149 2064 6f65 7320 6e6f 7420 616c 6c6f  AI does not allo
-00002150: 7720 746f 6f20 6d61 6e79 2069 6d61 6765  w too many image
-00002160: 7320 696e 2074 6865 2070 726f 6d70 7420  s in the prompt 
-00002170: 2873 6565 2064 6973 6375 7373 696f 6e20  (see discussion 
-00002180: 5b68 6572 655d 2868 7474 7073 3a2f 2f63  [here](https://c
-00002190: 6f6d 6d75 6e69 7479 2e6f 7065 6e61 692e  ommunity.openai.
-000021a0: 636f 6d2f 742f 6770 742d 342d 7669 7369  com/t/gpt-4-visi
-000021b0: 6f6e 2d6d 6178 696d 756d 2d61 6d6f 756e  on-maximum-amoun
-000021c0: 742d 6f66 2d69 6d61 6765 732f 3537 3331  t-of-images/5731
-000021d0: 3130 2f36 2929 2c20 736f 206c 6f6e 6720  10/6)), so long 
-000021e0: 6669 6c65 7320 7368 6f75 6c64 2062 6520  files should be 
-000021f0: 6578 7472 6163 7465 6420 7769 7468 2060  extracted with `
-00002200: 7465 7874 5f6f 6e6c 793d 5472 7565 6020  text_only=True` 
-00002210: 746f 2061 766f 6964 2074 6869 7320 6973  to avoid this is
-00002220: 7375 652c 2077 6869 6c65 206c 6f6e 6720  sue, while long 
-00002230: 7465 7874 2066 696c 6573 2073 686f 756c  text files shoul
-00002240: 6420 6569 7468 6572 2062 6520 636f 6d70  d either be comp
-00002250: 7265 7373 6564 206f 7220 656d 6265 6464  ressed or embedd
-00002260: 6564 2069 6e20 6120 5241 4720 6672 616d  ed in a RAG fram
-00002270: 6577 6f72 6b2e 0d0a 0d0a 5468 6520 7465  ework.....The te
-00002280: 7874 2061 6e64 2069 6d61 6765 7320 6672  xt and images fr
-00002290: 6f6d 2074 6865 7365 206d 6573 7361 6765  om these message
-000022a0: 7320 6d61 7920 616c 736f 2062 6520 7072  s may also be pr
-000022b0: 6570 6172 6564 2066 6f72 2061 2076 6563  epared for a vec
-000022c0: 746f 7220 6461 7461 6261 7365 2077 6974  tor database wit
-000022d0: 6820 6074 6865 7069 7065 2e63 6f72 652e  h `thepipe.core.
-000022e0: 6372 6561 7465 5f63 6875 6e6b 735f 6672  create_chunks_fr
-000022f0: 6f6d 5f6d 6573 7361 6765 7360 206f 7220  om_messages` or 
-00002300: 666f 7220 646f 776e 7374 7265 616d 2075  for downstream u
-00002310: 7365 2077 6974 6820 5241 4720 6672 616d  se with RAG fram
-00002320: 6577 6f72 6b73 2e20 5b4c 6974 654c 4c4d  eworks. [LiteLLM
-00002330: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00002340: 2e63 6f6d 2f42 6572 7269 4149 2f6c 6974  .com/BerriAI/lit
-00002350: 656c 6c6d 2920 6361 6e20 6265 2075 7365  ellm) can be use
-00002360: 6420 746f 2065 6173 696c 7920 696e 7465  d to easily inte
-00002370: 6772 6174 6520 5468 6520 5069 7065 2077  grate The Pipe w
-00002380: 6974 6820 616e 7920 4c4c 4d20 7072 6f76  ith any LLM prov
-00002390: 6964 6572 2e20 0d0a 0d0a 4974 2075 7365  ider. ....It use
-000023a0: 7320 6120 7661 7269 6574 7920 6f66 2068  s a variety of h
-000023b0: 6575 7269 7374 6963 7320 666f 7220 6f70  euristics for op
-000023c0: 7469 6d61 6c20 7065 7266 6f72 6d61 6e63  timal performanc
-000023d0: 6520 7769 7468 2076 6973 696f 6e2d 6c61  e with vision-la
-000023e0: 6e67 7561 6765 206d 6f64 656c 732c 2069  nguage models, i
-000023f0: 6e63 6c75 6469 6e67 2041 4920 6669 6c65  ncluding AI file
-00002400: 7479 7065 2064 6574 6563 7469 6f6e 2077  type detection w
-00002410: 6974 6820 5b66 696c 6574 7970 6520 6465  ith [filetype de
-00002420: 7465 6374 696f 6e5d 2868 7474 7073 3a2f  tection](https:/
-00002430: 2f6f 7065 6e73 6f75 7263 652e 676f 6f67  /opensource.goog
-00002440: 6c65 626c 6f67 2e63 6f6d 2f32 3032 342f  leblog.com/2024/
-00002450: 3032 2f6d 6167 696b 612d 6169 2d70 6f77  02/magika-ai-pow
-00002460: 6572 6564 2d66 6173 742d 616e 642d 6566  ered-fast-and-ef
-00002470: 6669 6369 656e 742d 6669 6c65 2d74 7970  ficient-file-typ
-00002480: 652d 6964 656e 7469 6669 6361 7469 6f6e  e-identification
-00002490: 2e68 746d 6c29 2c20 6f70 742d 696e 2041  .html), opt-in A
-000024a0: 4920 5b74 6162 6c65 2c20 6571 7561 7469  I [table, equati
-000024b0: 6f6e 2c20 616e 6420 6669 6775 7265 2065  on, and figure e
-000024c0: 7874 7261 6374 696f 6e5d 2868 7474 7073  xtraction](https
-000024d0: 3a2f 2f74 6865 7069 2e70 652f 7072 6963  ://thepi.pe/pric
-000024e0: 696e 6729 2c20 6566 6669 6369 656e 7420  ing), efficient 
-000024f0: 5b74 6f6b 656e 2063 6f6d 7072 6573 7369  [token compressi
-00002500: 6f6e 5d28 6874 7470 733a 2f2f 6172 7869  on](https://arxi
-00002510: 762e 6f72 672f 6162 732f 3234 3033 2e31  v.org/abs/2403.1
-00002520: 3239 3638 292c 2061 7574 6f6d 6174 6963  2968), automatic
-00002530: 205b 696d 6167 6520 656e 636f 6469 6e67   [image encoding
-00002540: 5d28 6874 7470 733a 2f2f 656e 2e77 696b  ](https://en.wik
-00002550: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
-00002560: 4261 7365 3634 292c 205b 7265 7261 6e6b  Base64), [rerank
-00002570: 696e 675d 2868 7474 7073 3a2f 2f61 7278  ing](https://arx
-00002580: 6976 2e6f 7267 2f61 6273 2f32 3331 302e  iv.org/abs/2310.
-00002590: 3036 3833 3929 2066 6f72 205b 6c6f 7374  06839) for [lost
-000025a0: 2d69 6e2d 7468 652d 6d69 6464 6c65 5d28  -in-the-middle](
-000025b0: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-000025c0: 672f 6162 732f 3233 3037 2e30 3331 3732  g/abs/2307.03172
-000025d0: 2920 6566 6665 6374 732c 2061 6e64 206d  ) effects, and m
-000025e0: 6f72 652c 2061 6c6c 2070 7265 2d62 7569  ore, all pre-bui
-000025f0: 6c74 2074 6f20 776f 726b 206f 7574 2d6f  lt to work out-o
-00002600: 662d 7468 652d 626f 782e 0d0a 0d0a 215b  f-the-box.....![
-00002610: 4465 6d6f 5d28 6874 7470 733a 2f2f 7270  Demo](https://rp
-00002620: 6e75 747a 656d 7574 6272 756d 637a 7776  nutzemutbrumczwv
-00002630: 7565 2e73 7570 6162 6173 652e 636f 2f73  ue.supabase.co/s
-00002640: 746f 7261 6765 2f76 312f 6f62 6a65 6374  torage/v1/object
-00002650: 2f70 7562 6c69 632f 6173 7365 7473 2f67  /public/assets/g
-00002660: 7261 6465 722e 7079 2532 3028 3629 2e70  rader.py%20(6).p
-00002670: 6e67 290d 0a0d 0a0d 0a23 2320 4c6f 6361  ng)......## Loca
-00002680: 6c20 496e 7374 616c 6c61 7469 6f6e 20f0  l Installation .
-00002690: 9f9b a0ef b88f 0d0a 0d0a 4966 2079 6f75  ..........If you
-000026a0: 2064 6f20 6e6f 7420 7769 7368 2074 6f20   do not wish to 
-000026b0: 7573 6520 6f75 7220 4150 492c 2079 6f75  use our API, you
-000026c0: 2061 7265 2077 656c 636f 6d65 2068 6f73   are welcome hos
-000026d0: 7420 5468 6520 5069 7065 2066 6f72 2079  t The Pipe for y
-000026e0: 6f75 7273 656c 6620 6c6f 6361 6c6c 792e  ourself locally.
-000026f0: 200d 0a49 6620 796f 7520 6368 6f6f 7365   ..If you choose
-00002700: 2074 6f20 646f 2074 6869 732c 2079 6f75   to do this, you
-00002710: 206d 7573 7420 696e 7374 616c 6c20 6120   must install a 
-00002720: 6e75 6d62 6572 206f 6620 6465 7065 6e64  number of depend
-00002730: 656e 6369 6573 2066 6f72 2074 6865 2063  encies for the c
-00002740: 6f64 6520 746f 2066 756e 6374 696f 6e20  ode to function 
-00002750: 636f 7272 6563 746c 792c 2073 6f6d 6520  correctly, some 
-00002760: 6f66 2077 6869 6368 206d 6179 2069 6e63  of which may inc
-00002770: 7572 2063 6f6d 7075 7465 2063 6f73 7473  ur compute costs
-00002780: 2061 6e64 2f6f 7220 7265 7175 6972 6520   and/or require 
-00002790: 6120 4750 5520 666f 7220 7265 6173 6f6e  a GPU for reason
-000027a0: 6162 6c65 2070 6572 666f 726d 616e 6365  able performance
-000027b0: 2e20 4164 6469 7469 6f6e 616c 2069 6e73  . Additional ins
-000027c0: 7461 6c6c 6564 2064 6570 656e 6465 6e63  talled dependenc
-000027d0: 6965 7320 6172 6520 7265 7175 6972 6564  ies are required
-000027e0: 3a20 7079 746f 7263 682c 2075 6e69 7665  : pytorch, unive
-000027f0: 7273 616c 2d63 7461 6773 2c20 706c 6179  rsal-ctags, play
-00002800: 7772 6967 6874 2c20 7079 7465 7373 6572  wright, pytesser
-00002810: 6163 742c 206c 6c6d 6c69 6e67 7561 2c20  act, llmlingua, 
-00002820: 6d6f 7669 6570 792c 2061 6e64 2070 7974  moviepy, and pyt
-00002830: 7562 652e 2054 6869 7320 696e 7374 616c  ube. This instal
-00002840: 6c61 7469 6f6e 2070 726f 6365 7373 2077  lation process w
-00002850: 696c 6c20 6465 7065 6e64 206f 6e20 796f  ill depend on yo
-00002860: 7572 2073 7973 7465 6d20 616e 6420 636f  ur system and co
-00002870: 6d70 7574 6520 6361 7061 6269 6c69 7469  mpute capabiliti
-00002880: 6573 2e20 4166 7465 7220 696e 7374 616c  es. After instal
-00002890: 6c69 6e67 2074 6865 6d2c 2066 6f6c 6c6f  ling them, follo
-000028a0: 7720 7468 6573 6520 7374 6570 7320 666f  w these steps fo
-000028b0: 7220 6120 6c6f 6361 6c20 7365 7475 703a  r a local setup:
-000028c0: 0d0a 0d0a 4172 6775 6d65 6e74 7320 6172  ....Arguments ar
-000028d0: 653a 0d0a 2d20 6073 6f75 7263 6560 2028  e:..- `source` (
-000028e0: 7265 7175 6972 6564 293a 2063 616e 2062  required): can b
-000028f0: 6520 6120 6669 6c65 2070 6174 682c 2061  e a file path, a
-00002900: 2055 524c 2c20 6f72 2061 2064 6972 6563   URL, or a direc
-00002910: 746f 7279 2070 6174 682e 0d0a 2d20 606c  tory path...- `l
-00002920: 6f63 616c 6020 286f 7074 696f 6e61 6c29  ocal` (optional)
-00002930: 3a20 5573 6520 7468 6520 6c6f 6361 6c20  : Use the local 
-00002940: 7665 7273 696f 6e20 6f66 2054 6865 2050  version of The P
-00002950: 6970 6520 696e 7374 6561 6420 6f66 2074  ipe instead of t
-00002960: 6865 2068 6f73 7465 6420 4150 492e 0d0a  he hosted API...
-00002970: 2d20 606d 6174 6368 6020 286f 7074 696f  - `match` (optio
-00002980: 6e61 6c29 3a20 5375 6273 7472 696e 6720  nal): Substring 
-00002990: 746f 206d 6174 6368 2066 696c 6573 2069  to match files i
-000029a0: 6e20 7468 6520 6469 7265 6374 6f72 792e  n the directory.
-000029b0: 2052 6567 6578 2069 7320 6e6f 7420 7965   Regex is not ye
-000029c0: 7420 7375 7070 6f72 7465 642e 0d0a 2d20  t supported...- 
-000029d0: 6069 676e 6f72 6560 2028 6f70 7469 6f6e  `ignore` (option
-000029e0: 616c 293a 2053 7562 7374 7269 6e67 2074  al): Substring t
-000029f0: 6f20 6967 6e6f 7265 2066 696c 6573 2069  o ignore files i
-00002a00: 6e20 7468 6520 6469 7265 6374 6f72 792e  n the directory.
-00002a10: 2052 6567 6578 2069 7320 6e6f 7420 7965   Regex is not ye
-00002a20: 7420 7375 7070 6f72 7465 642e 0d0a 2d20  t supported...- 
-00002a30: 606c 696d 6974 6020 286f 7074 696f 6e61  `limit` (optiona
-00002a40: 6c29 3a20 5468 6520 746f 6b65 6e20 6c69  l): The token li
-00002a50: 6d69 7420 666f 7220 7468 6520 6f75 7470  mit for the outp
-00002a60: 7574 2070 726f 6d70 742c 2064 6566 6175  ut prompt, defau
-00002a70: 6c74 7320 746f 2031 3030 4b2e 2050 726f  lts to 100K. Pro
-00002a80: 6d70 7473 2065 7863 6565 6469 6e67 2074  mpts exceeding t
-00002a90: 6865 206c 696d 6974 2077 696c 6c20 6265  he limit will be
-00002aa0: 2063 6f6d 7072 6573 7365 642e 2054 6869   compressed. Thi
-00002ab0: 7320 6d61 7920 6e6f 7420 776f 726b 2061  s may not work a
-00002ac0: 7320 6578 7065 6374 6564 2077 6974 6820  s expected with 
-00002ad0: 7468 6520 4150 492c 2061 7320 6974 2069  the API, as it i
-00002ae0: 7320 696e 2061 6374 6976 6520 6465 7665  s in active deve
-00002af0: 6c6f 706d 656e 742e 0d0a 2d20 6061 695f  lopment...- `ai_
-00002b00: 6578 7472 6163 7469 6f6e 6020 286f 7074  extraction` (opt
-00002b10: 696f 6e61 6c29 3a20 4578 7472 6163 7420  ional): Extract 
-00002b20: 7461 626c 6573 2c20 6669 6775 7265 732c  tables, figures,
-00002b30: 2061 6e64 206d 6174 6820 6672 6f6d 2050   and math from P
-00002b40: 4446 7320 7573 696e 6720 6f75 7220 6578  DFs using our ex
-00002b50: 7472 6163 746f 722e 2049 6e63 7572 7320  tractor. Incurs 
-00002b60: 6578 7472 6120 636f 7374 732e 0d0a 2d20  extra costs...- 
-00002b70: 6074 6578 745f 6f6e 6c79 6020 286f 7074  `text_only` (opt
-00002b80: 696f 6e61 6c29 3a20 446f 206e 6f74 2065  ional): Do not e
-00002b90: 7874 7261 6374 2069 6d61 6765 7320 6672  xtract images fr
-00002ba0: 6f6d 2064 6f63 756d 656e 7473 206f 7220  om documents or 
-00002bb0: 7765 6273 6974 6573 2e20 4164 6469 7469  websites. Additi
-00002bc0: 6f6e 616c 6c79 2c20 696d 6167 6520 6669  onally, image fi
-00002bd0: 6c65 7320 7769 6c6c 2062 6520 7265 7072  les will be repr
-00002be0: 6573 656e 7465 6420 7769 7468 204f 4352  esented with OCR
-00002bf0: 2069 6e73 7465 6164 206f 6620 6173 2069   instead of as i
-00002c00: 6d61 6765 732e 0d0a 0d0a 2320 5370 6f6e  mages.....# Spon
-00002c10: 736f 7273 0d0a 0d0a 3c61 2068 7265 663d  sors....<a href=
-00002c20: 2268 7474 7073 3a2f 2f63 616c 2e63 6f6d  "https://cal.com
-00002c30: 2f65 6d6d 6574 742d 6d63 662f 3330 6d69  /emmett-mcf/30mi
-00002c40: 6e22 3e3c 696d 6720 616c 743d 2242 6f6f  n"><img alt="Boo
-00002c50: 6b20 7573 2077 6974 6820 4361 6c2e 636f  k us with Cal.co
-00002c60: 6d22 2073 7263 3d22 6874 7470 733a 2f2f  m" src="https://
-00002c70: 6361 6c2e 636f 6d2f 626f 6f6b 2d77 6974  cal.com/book-wit
-00002c80: 682d 6361 6c2d 6461 726b 2e73 7667 2220  h-cal-dark.svg" 
-00002c90: 2f3e 3c2f 613e 0d0a 0d0a 5468 616e 6b20  /></a>....Thank 
-00002ca0: 796f 7520 746f 205b 4361 6c2e 636f 6d5d  you to [Cal.com]
-00002cb0: 2868 7474 7073 3a2f 2f63 616c 2e63 6f6d  (https://cal.com
-00002cc0: 2f29 2066 6f72 2073 706f 6e73 6f72 696e  /) for sponsorin
-00002cd0: 6720 7468 6973 2070 726f 6a65 6374 2e20  g this project. 
-00002ce0: 436f 6e74 6163 7420 656d 6d65 7474 4074  Contact emmett@t
-00002cf0: 6865 7069 2e70 6520 666f 7220 7370 6f6e  hepi.pe for spon
-00002d00: 736f 7273 6869 7020 696e 666f 726d 6174  sorship informat
-00002d10: 696f 6e2e                                ion.
+00001850: 2020 2020 2020 2020 2020 2020 2020 7c0d                |.
+00001860: 0a7c 204d 6963 726f 736f 6674 2057 6f72  .| Microsoft Wor
+00001870: 6420 446f 6375 6d65 6e74 2020 2020 2020  d Document      
+00001880: 2020 2020 2020 2020 207c 2060 2e64 6f63           | `.doc
+00001890: 7860 2020 2020 2020 2020 2020 2020 2020  x`              
+000018a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018b0: 2020 207c 20e2 9c94 efb8 8f20 2020 2020     | ......     
+000018c0: 2020 2020 2020 2020 2020 7c20 e29c 94ef            | ....
+000018d0: b88f 2020 2020 2020 2020 2020 2020 2020  ..              
+000018e0: 207c 2045 7874 7261 6374 7320 7465 7874   | Extracts text
+000018f0: 2061 6e64 2069 6d61 6765 7320 6672 6f6d   and images from
+00001900: 2057 6f72 6420 646f 6375 6d65 6e74 7320   Word documents 
+00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001930: 2020 2020 2020 207c 0d0a 7c20 4d69 6372         |..| Micr
+00001940: 6f73 6f66 7420 506f 7765 7250 6f69 6e74  osoft PowerPoint
+00001950: 2050 7265 7365 6e74 6174 696f 6e20 2020   Presentation   
+00001960: 2020 7c20 602e 7070 7478 6020 2020 2020    | `.pptx`     
+00001970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001980: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
+00001990: 94ef b88f 2020 2020 2020 2020 2020 2020  ....            
+000019a0: 2020 207c 20e2 9c94 efb8 8f20 2020 2020     | ......     
+000019b0: 2020 2020 2020 2020 2020 7c20 4578 7472            | Extr
+000019c0: 6163 7473 2074 6578 7420 616e 6420 696d  acts text and im
+000019d0: 6167 6573 2066 726f 6d20 506f 7765 7250  ages from PowerP
+000019e0: 6f69 6e74 2070 7265 7365 6e74 6174 696f  oint presentatio
+000019f0: 6e73 2020 2020 2020 2020 2020 2020 2020  ns              
+00001a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a10: 7c0d 0a7c 2056 6964 656f 2020 2020 2020  |..| Video      
+00001a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a30: 2020 2020 2020 2020 2020 207c 2060 2e6d             | `.m
+00001a40: 7034 602c 2060 2e6d 6f76 602c 2060 2e77  p4`, `.mov`, `.w
+00001a50: 6d76 6020 2020 2020 7c20 e29c 94ef b88f  mv`     | ......
+00001a60: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00001a70: 20e2 9c94 efb8 8f20 2020 2020 2020 2020   ......         
+00001a80: 2020 2020 2020 207c 2045 7874 7261 6374         | Extract
+00001a90: 7320 6672 616d 6573 2061 6e64 2061 7564  s frames and aud
+00001aa0: 696f 2074 7261 6e73 6372 6970 7420 6672  io transcript fr
+00001ab0: 6f6d 2076 6964 656f 7320 696e 2070 6572  om videos in per
+00001ac0: 2d6d 696e 7574 6520 6368 756e 6b73 2e20  -minute chunks. 
+00001ad0: 7c0d 0a7c 2041 7564 696f 2020 2020 2020  |..| Audio      
+00001ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001af0: 2020 2020 2020 2020 2020 207c 2060 2e6d             | `.m
+00001b00: 7033 602c 2060 2e77 6176 6020 2020 2020  p3`, `.wav`     
+00001b10: 2020 2020 207c 20e2 9c94 efb8 8f20 2020       | ......   
+00001b20: 2020 2020 2020 2020 2020 2020 7c20 e29d              | ..
+00001b30: 8c20 2020 2020 2020 2020 2020 2020 2020  .               
+00001b40: 207c 2045 7874 7261 6374 7320 7465 7874   | Extracts text
+00001b50: 2066 726f 6d20 6175 6469 6f20 6669 6c65   from audio file
+00001b60: 733b 2073 7570 706f 7274 7320 7370 6565  s; supports spee
+00001b70: 6368 2d74 6f2d 7465 7874 2063 6f6e 7665  ch-to-text conve
+00001b80: 7273 696f 6e20 2020 2020 2020 207c 200d  rsion        | .
+00001b90: 0a7c 2057 6562 7369 7465 2020 2020 2020  .| Website      
+00001ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bb0: 2020 2020 2020 2020 207c 2055 524c 7320           | URLs 
+00001bc0: 2869 6e70 7574 7320 7374 6172 7469 6e67  (inputs starting
+00001bd0: 2077 6974 6820 6068 7474 7060 2c20 6068   with `http`, `h
+00001be0: 7474 7073 602c 2060 6674 7060 2920 2020  ttps`, `ftp`)   
+00001bf0: 2020 2020 2020 2020 2020 7c20 e29c 94ef            | ....
+00001c00: b88f 2020 2020 2020 2020 2020 2020 2020  ..              
+00001c10: 2020 7c20 e29c 94ef b88f 2020 2020 7c20    | ......    | 
+00001c20: 4578 7472 6163 7473 2074 6578 7420 6672  Extracts text fr
+00001c30: 6f6d 2077 6562 2070 6167 6520 616c 6f6e  om web page alon
+00001c40: 6720 7769 7468 2069 6d61 6765 2028 6f72  g with image (or
+00001c50: 2069 6d61 6765 7320 6966 2073 6372 6f6c   images if scrol
+00001c60: 6c61 626c 6529 3b20 7465 7874 2d6f 6e6c  lable); text-onl
+00001c70: 7920 6578 7472 6163 7469 6f6e 2061 7661  y extraction ava
+00001c80: 696c 6162 6c65 2020 2020 2020 2020 2020  ilable          
+00001c90: 7c0d 0a7c 2047 6974 4875 6220 5265 706f  |..| GitHub Repo
+00001ca0: 7369 746f 7279 2020 2020 2020 2020 2020  sitory          
+00001cb0: 2020 2020 2020 2020 2020 207c 2047 6974             | Git
+00001cc0: 4875 6220 7265 706f 2055 524c 7320 2869  Hub repo URLs (i
+00001cd0: 6e70 7574 7320 7374 6172 7469 6e67 2077  nputs starting w
+00001ce0: 6974 6820 6068 7474 7073 3a2f 2f67 6974  ith `https://git
+00001cf0: 6875 622e 636f 6d60 206f 7220 6068 7474  hub.com` or `htt
+00001d00: 7073 3a2f 2f77 7777 2e67 6974 6875 622e  ps://www.github.
+00001d10: 636f 6d60 2920 2020 2020 2020 2020 2020  com`)           
+00001d20: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00001d30: 20e2 9c94 efb8 8f20 2020 2020 2020 2020   ......         
+00001d40: 2020 2020 2020 7c20 e29c 94ef b88f 2020        | ......  
+00001d50: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00001d60: 4578 7472 6163 7473 2066 726f 6d20 4769  Extracts from Gi
+00001d70: 7448 7562 2072 6570 6f73 6974 6f72 6965  tHub repositorie
+00001d80: 733b 2073 7570 706f 7274 7320 6272 616e  s; supports bran
+00001d90: 6368 2073 7065 6369 6669 6361 7469 6f6e  ch specification
+00001da0: 2020 2020 2020 2020 207c 0d0a 7c20 596f           |..| Yo
+00001db0: 7554 7562 6520 5669 6465 6f20 2020 2020  uTube Video     
+00001dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dd0: 2020 2020 7c20 596f 7554 7562 6520 7669      | YouTube vi
+00001de0: 6465 6f20 5552 4c73 2028 696e 7075 7473  deo URLs (inputs
+00001df0: 2073 7461 7274 696e 6720 7769 7468 2060   starting with `
+00001e00: 6874 7470 733a 2f2f 796f 7574 7562 652e  https://youtube.
+00001e10: 636f 6d60 206f 7220 6068 7474 7073 3a2f  com` or `https:/
+00001e20: 2f77 7777 2e79 6f75 7475 6265 2e63 6f6d  /www.youtube.com
+00001e30: 6029 2020 2020 2020 2020 2020 2020 2020  `)              
+00001e40: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
+00001e50: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00001e60: e29c 94ef b88f 2020 2020 2020 2020 2020  ......          
+00001e70: 2020 2020 2020 7c20 4578 7472 6163 7473        | Extracts
+00001e80: 2066 7261 6d65 7320 616e 6420 7472 616e   frames and tran
+00001e90: 7363 7269 7074 2066 726f 6d20 596f 7554  script from YouT
+00001ea0: 7562 6520 7669 6465 6f73 2069 6e20 7065  ube videos in pe
+00001eb0: 722d 6d69 6e75 7465 2063 6875 6e6b 732e  r-minute chunks.
+00001ec0: 2020 2020 2020 2020 2020 7c0d 0a7c 205a            |..| Z
+00001ed0: 4950 2046 696c 6520 2020 2020 2020 2020  IP File         
+00001ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ef0: 2020 2020 207c 2060 2e7a 6970 6020 2020       | `.zip`   
+00001f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f10: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00001f20: 20e2 9c94 efb8 8f20 2020 2020 2020 2020   ......         
+00001f30: 2020 2020 2020 7c20 e29c 94ef b88f 2020        | ......  
+00001f40: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00001f50: 4578 7472 6163 7473 2063 6f6e 7465 6e74  Extracts content
+00001f60: 7320 6f66 205a 4950 2066 696c 6573 3b20  s of ZIP files; 
+00001f70: 7375 7070 6f72 7473 206e 6573 7465 6420  supports nested 
+00001f80: 6469 7265 6374 6f72 7920 6578 7472 6163  directory extrac
+00001f90: 7469 6f6e 2020 2020 207c 0d0a 0d0a 2323  tion     |....##
+00001fa0: 2048 6f77 2069 7420 776f 726b 7320 f09f   How it works ..
+00001fb0: 9ba0 efb8 8f0d 0a0d 0a54 6865 2069 6e70  .........The inp
+00001fc0: 7574 2073 6f75 7263 6520 6973 2065 6974  ut source is eit
+00001fd0: 6865 7220 6120 6669 6c65 2070 6174 682c  her a file path,
+00001fe0: 2061 2055 524c 2c20 6f72 2061 2064 6972   a URL, or a dir
+00001ff0: 6563 746f 7279 2e20 5468 6520 7069 7065  ectory. The pipe
+00002000: 2077 696c 6c20 6578 7472 6163 7420 696e   will extract in
+00002010: 666f 726d 6174 696f 6e20 6672 6f6d 2074  formation from t
+00002020: 6865 2073 6f75 7263 6520 616e 6420 7072  he source and pr
+00002030: 6f63 6573 7320 6974 2066 6f72 2064 6f77  ocess it for dow
+00002040: 6e73 7472 6561 6d20 7573 6520 7769 7468  nstream use with
+00002050: 205b 6c61 6e67 7561 6765 206d 6f64 656c   [language model
+00002060: 735d 2868 7474 7073 3a2f 2f65 6e2e 7769  s](https://en.wi
+00002070: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
+00002080: 2f4c 6172 6765 5f6c 616e 6775 6167 655f  /Large_language_
+00002090: 6d6f 6465 6c29 2c20 5b76 6973 696f 6e20  model), [vision 
+000020a0: 7472 616e 7366 6f72 6d65 7273 5d28 6874  transformers](ht
+000020b0: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
+000020c0: 6961 2e6f 7267 2f77 696b 692f 5669 7369  ia.org/wiki/Visi
+000020d0: 6f6e 5f74 7261 6e73 666f 726d 6572 292c  on_transformer),
+000020e0: 206f 7220 5b76 6973 696f 6e2d 6c61 6e67   or [vision-lang
+000020f0: 7561 6765 206d 6f64 656c 735d 2868 7474  uage models](htt
+00002100: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
+00002110: 6273 2f32 3330 342e 3030 3638 3529 2e20  bs/2304.00685). 
+00002120: 5468 6520 6f75 7470 7574 2066 726f 6d20  The output from 
+00002130: 7468 6520 7069 7065 2069 7320 6120 7365  the pipe is a se
+00002140: 6e73 6962 6c65 206c 6973 7420 6f66 206d  nsible list of m
+00002150: 756c 7469 6d6f 6461 6c20 6d65 7373 6167  ultimodal messag
+00002160: 6573 2072 6570 7265 7365 6e74 696e 6720  es representing 
+00002170: 6368 756e 6b73 206f 6620 7468 6520 6578  chunks of the ex
+00002180: 7472 6163 7465 6420 696e 666f 726d 6174  tracted informat
+00002190: 696f 6e2c 2063 6172 6566 756c 6c79 2063  ion, carefully c
+000021a0: 7261 6674 6564 2074 6f20 6669 7420 7769  rafted to fit wi
+000021b0: 7468 696e 2063 6f6e 7465 7874 2077 696e  thin context win
+000021c0: 646f 7773 2066 6f72 2061 6e79 206d 6f64  dows for any mod
+000021d0: 656c 7320 6672 6f6d 205b 6765 6d6d 612d  els from [gemma-
+000021e0: 3762 5d28 6874 7470 733a 2f2f 6875 6767  7b](https://hugg
+000021f0: 696e 6766 6163 652e 636f 2f67 6f6f 676c  ingface.co/googl
+00002200: 652f 6765 6d6d 612d 3762 2920 746f 205b  e/gemma-7b) to [
+00002210: 4750 542d 345d 2868 7474 7073 3a2f 2f6f  GPT-4](https://o
+00002220: 7065 6e61 692e 636f 6d2f 6770 742d 3429  penai.com/gpt-4)
+00002230: 2e20 5468 6520 6d65 7373 6167 6573 2072  . The messages r
+00002240: 6574 7572 6e65 6420 7368 6f75 6c64 206c  eturned should l
+00002250: 6f6f 6b20 6c69 6b65 2074 6869 733a 0d0a  ook like this:..
+00002260: 6060 606a 736f 6e0d 0a5b 0d0a 2020 7b0d  ```json..[..  {.
+00002270: 0a20 2020 2022 726f 6c65 223a 2022 7573  .    "role": "us
+00002280: 6572 222c 0d0a 2020 2020 2263 6f6e 7465  er",..    "conte
+00002290: 6e74 223a 205b 0d0a 2020 2020 2020 7b0d  nt": [..      {.
+000022a0: 0a20 2020 2020 2020 2022 7479 7065 223a  .        "type":
+000022b0: 2022 7465 7874 222c 0d0a 2020 2020 2020   "text",..      
+000022c0: 2020 2274 6578 7422 3a20 222e 2e2e 220d    "text": "...".
+000022d0: 0a20 2020 2020 207d 2c0d 0a20 2020 2020  .      },..     
+000022e0: 207b 0d0a 2020 2020 2020 2020 2274 7970   {..        "typ
+000022f0: 6522 3a20 2269 6d61 6765 5f75 726c 222c  e": "image_url",
+00002300: 0d0a 2020 2020 2020 2020 2269 6d61 6765  ..        "image
+00002310: 5f75 726c 223a 207b 0d0a 2020 2020 2020  _url": {..      
+00002320: 2020 2020 2275 726c 223a 2022 6461 7461      "url": "data
+00002330: 3a69 6d61 6765 2f6a 7065 673b 6261 7365  :image/jpeg;base
+00002340: 3634 2c2e 2e2e 220d 0a20 2020 2020 2020  64,..."..       
+00002350: 207d 0d0a 2020 2020 2020 7d0d 0a20 2020   }..      }..   
+00002360: 205d 0d0a 2020 7d0d 0a5d 0d0a 6060 600d   ]..  }..]..```.
+00002370: 0a49 6620 796f 7520 7761 6e74 2074 6f20  .If you want to 
+00002380: 6665 6564 2074 6865 7365 206d 6573 7361  feed these messa
+00002390: 6765 7320 6469 7265 6374 6c79 2069 6e74  ges directly int
+000023a0: 6f20 7468 6520 6d6f 6465 6c2c 2069 7420  o the model, it 
+000023b0: 6973 2069 6d70 6f72 7461 6e74 2074 6f20  is important to 
+000023c0: 6265 206d 696e 6466 756c 206f 6620 7468  be mindful of th
+000023d0: 6520 746f 6b65 6e20 6c69 6d69 742e 0d0a  e token limit...
+000023e0: 4f70 656e 4149 2064 6f65 7320 6e6f 7420  OpenAI does not 
+000023f0: 616c 6c6f 7720 746f 6f20 6d61 6e79 2069  allow too many i
+00002400: 6d61 6765 7320 696e 2074 6865 2070 726f  mages in the pro
+00002410: 6d70 7420 2873 6565 2064 6973 6375 7373  mpt (see discuss
+00002420: 696f 6e20 5b68 6572 655d 2868 7474 7073  ion [here](https
+00002430: 3a2f 2f63 6f6d 6d75 6e69 7479 2e6f 7065  ://community.ope
+00002440: 6e61 692e 636f 6d2f 742f 6770 742d 342d  nai.com/t/gpt-4-
+00002450: 7669 7369 6f6e 2d6d 6178 696d 756d 2d61  vision-maximum-a
+00002460: 6d6f 756e 742d 6f66 2d69 6d61 6765 732f  mount-of-images/
+00002470: 3537 3331 3130 2f36 2929 2c20 736f 206c  573110/6)), so l
+00002480: 6f6e 6720 6669 6c65 7320 7368 6f75 6c64  ong files should
+00002490: 2062 6520 6578 7472 6163 7465 6420 7769   be extracted wi
+000024a0: 7468 2060 7465 7874 5f6f 6e6c 793d 5472  th `text_only=Tr
+000024b0: 7565 6020 746f 2061 766f 6964 2074 6869  ue` to avoid thi
+000024c0: 7320 6973 7375 652c 2077 6869 6c65 206c  s issue, while l
+000024d0: 6f6e 6720 7465 7874 2066 696c 6573 2073  ong text files s
+000024e0: 686f 756c 6420 6569 7468 6572 2062 6520  hould either be 
+000024f0: 636f 6d70 7265 7373 6564 206f 7220 656d  compressed or em
+00002500: 6265 6464 6564 2069 6e20 6120 5241 4720  bedded in a RAG 
+00002510: 6672 616d 6577 6f72 6b2e 0d0a 0d0a 5468  framework.....Th
+00002520: 6520 7465 7874 2061 6e64 2069 6d61 6765  e text and image
+00002530: 7320 6672 6f6d 2074 6865 7365 206d 6573  s from these mes
+00002540: 7361 6765 7320 6d61 7920 616c 736f 2062  sages may also b
+00002550: 6520 7072 6570 6172 6564 2066 6f72 2061  e prepared for a
+00002560: 2076 6563 746f 7220 6461 7461 6261 7365   vector database
+00002570: 2077 6974 6820 6074 6865 7069 7065 2e63   with `thepipe.c
+00002580: 6f72 652e 6372 6561 7465 5f63 6875 6e6b  ore.create_chunk
+00002590: 735f 6672 6f6d 5f6d 6573 7361 6765 7360  s_from_messages`
+000025a0: 206f 7220 666f 7220 646f 776e 7374 7265   or for downstre
+000025b0: 616d 2075 7365 2077 6974 6820 5241 4720  am use with RAG 
+000025c0: 6672 616d 6577 6f72 6b73 2e20 5b4c 6974  frameworks. [Lit
+000025d0: 654c 4c4d 5d28 6874 7470 733a 2f2f 6769  eLLM](https://gi
+000025e0: 7468 7562 2e63 6f6d 2f42 6572 7269 4149  thub.com/BerriAI
+000025f0: 2f6c 6974 656c 6c6d 2920 6361 6e20 6265  /litellm) can be
+00002600: 2075 7365 6420 746f 2065 6173 696c 7920   used to easily 
+00002610: 696e 7465 6772 6174 6520 5468 6520 5069  integrate The Pi
+00002620: 7065 2077 6974 6820 616e 7920 4c4c 4d20  pe with any LLM 
+00002630: 7072 6f76 6964 6572 2e20 0d0a 0d0a 4974  provider. ....It
+00002640: 2075 7365 7320 6120 7661 7269 6574 7920   uses a variety 
+00002650: 6f66 2068 6575 7269 7374 6963 7320 666f  of heuristics fo
+00002660: 7220 6f70 7469 6d61 6c20 7065 7266 6f72  r optimal perfor
+00002670: 6d61 6e63 6520 7769 7468 2076 6973 696f  mance with visio
+00002680: 6e2d 6c61 6e67 7561 6765 206d 6f64 656c  n-language model
+00002690: 732c 2069 6e63 6c75 6469 6e67 2041 4920  s, including AI 
+000026a0: 6669 6c65 7479 7065 2064 6574 6563 7469  filetype detecti
+000026b0: 6f6e 2077 6974 6820 5b66 696c 6574 7970  on with [filetyp
+000026c0: 6520 6465 7465 6374 696f 6e5d 2868 7474  e detection](htt
+000026d0: 7073 3a2f 2f6f 7065 6e73 6f75 7263 652e  ps://opensource.
+000026e0: 676f 6f67 6c65 626c 6f67 2e63 6f6d 2f32  googleblog.com/2
+000026f0: 3032 342f 3032 2f6d 6167 696b 612d 6169  024/02/magika-ai
+00002700: 2d70 6f77 6572 6564 2d66 6173 742d 616e  -powered-fast-an
+00002710: 642d 6566 6669 6369 656e 742d 6669 6c65  d-efficient-file
+00002720: 2d74 7970 652d 6964 656e 7469 6669 6361  -type-identifica
+00002730: 7469 6f6e 2e68 746d 6c29 2c20 6f70 742d  tion.html), opt-
+00002740: 696e 2041 4920 5b74 6162 6c65 2c20 6571  in AI [table, eq
+00002750: 7561 7469 6f6e 2c20 616e 6420 6669 6775  uation, and figu
+00002760: 7265 2065 7874 7261 6374 696f 6e5d 2868  re extraction](h
+00002770: 7474 7073 3a2f 2f74 6865 7069 2e70 652f  ttps://thepi.pe/
+00002780: 7072 6963 696e 6729 2c20 6566 6669 6369  pricing), effici
+00002790: 656e 7420 5b74 6f6b 656e 2063 6f6d 7072  ent [token compr
+000027a0: 6573 7369 6f6e 5d28 6874 7470 733a 2f2f  ession](https://
+000027b0: 6172 7869 762e 6f72 672f 6162 732f 3234  arxiv.org/abs/24
+000027c0: 3033 2e31 3239 3638 292c 2061 7574 6f6d  03.12968), autom
+000027d0: 6174 6963 205b 696d 6167 6520 656e 636f  atic [image enco
+000027e0: 6469 6e67 5d28 6874 7470 733a 2f2f 656e  ding](https://en
+000027f0: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
+00002800: 696b 692f 4261 7365 3634 292c 205b 7265  iki/Base64), [re
+00002810: 7261 6e6b 696e 675d 2868 7474 7073 3a2f  ranking](https:/
+00002820: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+00002830: 3331 302e 3036 3833 3929 2066 6f72 205b  310.06839) for [
+00002840: 6c6f 7374 2d69 6e2d 7468 652d 6d69 6464  lost-in-the-midd
+00002850: 6c65 5d28 6874 7470 733a 2f2f 6172 7869  le](https://arxi
+00002860: 762e 6f72 672f 6162 732f 3233 3037 2e30  v.org/abs/2307.0
+00002870: 3331 3732 2920 6566 6665 6374 732c 2061  3172) effects, a
+00002880: 6e64 206d 6f72 652c 2061 6c6c 2070 7265  nd more, all pre
+00002890: 2d62 7569 6c74 2074 6f20 776f 726b 206f  -built to work o
+000028a0: 7574 2d6f 662d 7468 652d 626f 782e 0d0a  ut-of-the-box...
+000028b0: 0d0a 215b 4465 6d6f 5d28 6874 7470 733a  ..![Demo](https:
+000028c0: 2f2f 7270 6e75 747a 656d 7574 6272 756d  //rpnutzemutbrum
+000028d0: 637a 7776 7565 2e73 7570 6162 6173 652e  czwvue.supabase.
+000028e0: 636f 2f73 746f 7261 6765 2f76 312f 6f62  co/storage/v1/ob
+000028f0: 6a65 6374 2f70 7562 6c69 632f 6173 7365  ject/public/asse
+00002900: 7473 2f67 7261 6465 722e 7079 2532 3028  ts/grader.py%20(
+00002910: 3629 2e70 6e67 290d 0a0d 0a0d 0a23 2320  6).png)......## 
+00002920: 4c6f 6361 6c20 496e 7374 616c 6c61 7469  Local Installati
+00002930: 6f6e 20f0 9f9b a0ef b88f 0d0a 0d0a 5468  on ...........Th
+00002940: 6520 5069 7065 2068 616e 646c 6573 2061  e Pipe handles a
+00002950: 2077 6964 6520 6172 7261 7920 6f66 2063   wide array of c
+00002960: 6f6d 706c 6578 2066 696c 6574 7970 6573  omplex filetypes
+00002970: 2c20 616e 6420 7468 7573 2072 6571 7569  , and thus requi
+00002980: 7265 7320 696e 7374 616c 6c61 7469 6f6e  res installation
+00002990: 206f 6620 6d61 6e79 2064 6966 6665 7265   of many differe
+000029a0: 6e74 2070 6163 6b61 6765 7320 746f 2066  nt packages to f
+000029b0: 756e 6374 696f 6e2e 2049 7420 616c 736f  unction. It also
+000029c0: 2072 6571 7569 7265 7320 6120 7665 7279   requires a very
+000029d0: 2063 6170 6162 6c65 206d 6163 6869 6e65   capable machine
+000029e0: 2066 6f72 2067 6f6f 6420 7265 7370 6f6e   for good respon
+000029f0: 7365 2074 696d 6573 2e20 466f 7220 7468  se times. For th
+00002a00: 6973 2072 6561 736f 6e2c 2077 6520 686f  is reason, we ho
+00002a10: 7374 2069 7420 6173 2061 6e20 4150 4920  st it as an API 
+00002a20: 7468 6174 2077 6f72 6b73 206f 7574 2d6f  that works out-o
+00002a30: 662d 7468 652d 626f 782e 2054 6f20 7573  f-the-box. To us
+00002a40: 6520 5468 6520 5069 7065 206c 6f63 616c  e The Pipe local
+00002a50: 6c79 2066 6f72 2066 7265 6520 696e 7374  ly for free inst
+00002a60: 6561 642c 2079 6f75 2077 696c 6c20 6e65  ead, you will ne
+00002a70: 6564 205b 706c 6179 7772 6967 6874 5d28  ed [playwright](
+00002a80: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00002a90: 6f6d 2f6d 6963 726f 736f 6674 2f70 6c61  om/microsoft/pla
+00002aa0: 7977 7269 6768 7429 2c20 5b63 7461 6773  ywright), [ctags
+00002ab0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00002ac0: 2e63 6f6d 2f75 6e69 7665 7273 616c 2d63  .com/universal-c
+00002ad0: 7461 6773 2f29 2c20 5b70 7974 6573 7365  tags/), [pytesse
+00002ae0: 7261 6374 5d28 6874 7470 733a 2f2f 6769  ract](https://gi
+00002af0: 7468 7562 2e63 6f6d 2f68 2f70 7974 6573  thub.com/h/pytes
+00002b00: 7365 7261 6374 292c 205b 7079 7475 6265  seract), [pytube
+00002b10: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00002b20: 2e63 6f6d 2f70 7974 7562 652f 2920 616e  .com/pytube/) an
+00002b30: 6420 7468 6520 7265 6d61 696e 696e 6720  d the remaining 
+00002b40: 6c6f 6361 6c20 7079 7468 6f6e 2072 6571  local python req
+00002b50: 7569 7265 6d65 6e74 732c 2077 6869 6368  uirements, which
+00002b60: 2064 6966 6665 7220 6672 6f6d 2074 6865   differ from the
+00002b70: 206d 6f72 6520 6c69 6768 7477 6569 6768   more lightweigh
+00002b80: 7420 4150 4920 7265 7175 6972 656d 656e  t API requiremen
+00002b90: 7473 3a0d 0a0d 0a60 6060 6261 7368 0d0a  ts:....```bash..
+00002ba0: 6769 7420 636c 6f6e 6520 6874 7470 733a  git clone https:
+00002bb0: 2f2f 6769 7468 7562 2e63 6f6d 2f65 6d63  //github.com/emc
+00002bc0: 662f 7468 6570 6970 650d 0a70 6970 2069  f/thepipe..pip i
+00002bd0: 6e73 7461 6c6c 202d 7220 7265 7175 6972  nstall -r requir
+00002be0: 656d 656e 7473 5f6c 6f63 616c 2e74 7874  ements_local.txt
+00002bf0: 0d0a 6060 600d 0a0d 0a54 6970 2066 6f72  ..```....Tip for
+00002c00: 2077 696e 646f 7773 2075 7365 7273 3a20   windows users: 
+00002c10: 496e 7374 616c 6c20 7468 6520 7079 7468  Install the pyth
+00002c20: 6f6e 2d6c 6962 6d61 6769 6320 6269 6e61  on-libmagic bina
+00002c30: 7269 6573 2077 6974 6820 6070 6970 2069  ries with `pip i
+00002c40: 6e73 7461 6c6c 2070 7974 686f 6e2d 6d61  nstall python-ma
+00002c50: 6769 632d 6269 6e60 2e20 456e 7375 7265  gic-bin`. Ensure
+00002c60: 2074 6865 2060 7465 7373 6572 6163 742d   the `tesseract-
+00002c70: 6f63 7260 2062 696e 6172 6965 7320 616e  ocr` binaries an
+00002c80: 6420 7468 6520 6063 7461 6773 6020 6269  d the `ctags` bi
+00002c90: 6e61 7269 6573 2061 7265 2069 6e20 796f  naries are in yo
+00002ca0: 7572 2050 4154 482e 2046 6f72 2059 6f75  ur PATH. For You
+00002cb0: 5475 6265 2076 6964 656f 2065 7874 7261  Tube video extra
+00002cc0: 6374 696f 6e20 746f 2066 756e 6374 696f  ction to functio
+00002cd0: 6e20 636f 6e73 6973 7465 6e74 6c79 2c20  n consistently, 
+00002ce0: 796f 7520 7769 6c6c 206e 6565 6420 746f  you will need to
+00002cf0: 206d 6f64 6966 7920 796f 7572 2060 7079   modify your `py
+00002d00: 7475 6265 6020 696e 7374 616c 6c61 7469  tube` installati
+00002d10: 6f6e 2074 6f20 7365 6e64 2061 2076 616c  on to send a val
+00002d20: 6964 2075 7365 7220 6167 656e 7420 6865  id user agent he
+00002d30: 6164 6572 2028 4920 6b6e 6f77 2c20 6974  ader (I know, it
+00002d40: 2773 2063 6f6d 706c 6963 6174 6564 2e20  's complicated. 
+00002d50: 5365 6520 5b74 6869 7320 6973 7375 655d  See [this issue]
+00002d60: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00002d70: 636f 6d2f 7079 7475 6265 2f70 7974 7562  com/pytube/pytub
+00002d80: 652f 6973 7375 6573 2f33 3939 2920 666f  e/issues/399) fo
+00002d90: 7220 6d6f 7265 292e 0d0a 0d0a 4e6f 7720  r more).....Now 
+00002da0: 796f 7520 6361 6e20 7573 6520 5468 6520  you can use The 
+00002db0: 5069 7065 2077 6974 6820 5079 7468 6f6e  Pipe with Python
+00002dc0: 3a0d 0a60 6060 6261 7368 0d0a 6672 6f6d  :..```bash..from
+00002dd0: 2074 6865 7069 7065 5f61 7069 2069 6d70   thepipe_api imp
+00002de0: 6f72 7420 7468 6570 6970 650d 0a63 6875  ort thepipe..chu
+00002df0: 6e6b 7320 3d20 7468 6570 6970 652e 6578  nks = thepipe.ex
+00002e00: 7472 6163 7428 2265 7861 6d70 6c65 2e70  tract("example.p
+00002e10: 6466 222c 206c 6f63 616c 3d54 7275 6529  df", local=True)
+00002e20: 0d0a 6060 600d 0a0d 0a6f 7220 6672 6f6d  ..```....or from
+00002e30: 2074 6865 2063 6f6d 6d61 6e64 206c 696e   the command lin
+00002e40: 653a 0d0a 6060 6062 6173 680d 0a74 6865  e:..```bash..the
+00002e50: 7069 7065 2070 6174 682f 746f 2f66 6f6c  pipe path/to/fol
+00002e60: 6465 7220 2d2d 6d61 7463 6820 2e74 7378  der --match .tsx
+00002e70: 202d 2d69 676e 6f72 6520 7465 7374 730d   --ignore tests.
+00002e80: 0a60 6060 0d0a 0d0a 4172 6775 6d65 6e74  .```....Argument
+00002e90: 7320 6172 653a 0d0a 2d20 6073 6f75 7263  s are:..- `sourc
+00002ea0: 6560 2028 7265 7175 6972 6564 293a 2063  e` (required): c
+00002eb0: 616e 2062 6520 6120 6669 6c65 2070 6174  an be a file pat
+00002ec0: 682c 2061 2055 524c 2c20 6f72 2061 2064  h, a URL, or a d
+00002ed0: 6972 6563 746f 7279 2070 6174 682e 0d0a  irectory path...
+00002ee0: 2d20 606c 6f63 616c 6020 286f 7074 696f  - `local` (optio
+00002ef0: 6e61 6c29 3a20 5573 6520 7468 6520 6c6f  nal): Use the lo
+00002f00: 6361 6c20 7665 7273 696f 6e20 6f66 2054  cal version of T
+00002f10: 6865 2050 6970 6520 696e 7374 6561 6420  he Pipe instead 
+00002f20: 6f66 2074 6865 2068 6f73 7465 6420 4150  of the hosted AP
+00002f30: 492e 0d0a 2d20 606d 6174 6368 6020 286f  I...- `match` (o
+00002f40: 7074 696f 6e61 6c29 3a20 5375 6273 7472  ptional): Substr
+00002f50: 696e 6720 746f 206d 6174 6368 2066 696c  ing to match fil
+00002f60: 6573 2069 6e20 7468 6520 6469 7265 6374  es in the direct
+00002f70: 6f72 792e 2052 6567 6578 2069 7320 6e6f  ory. Regex is no
+00002f80: 7420 7965 7420 7375 7070 6f72 7465 642e  t yet supported.
+00002f90: 0d0a 2d20 6069 676e 6f72 6560 2028 6f70  ..- `ignore` (op
+00002fa0: 7469 6f6e 616c 293a 2053 7562 7374 7269  tional): Substri
+00002fb0: 6e67 2074 6f20 6967 6e6f 7265 2066 696c  ng to ignore fil
+00002fc0: 6573 2069 6e20 7468 6520 6469 7265 6374  es in the direct
+00002fd0: 6f72 792e 2052 6567 6578 2069 7320 6e6f  ory. Regex is no
+00002fe0: 7420 7965 7420 7375 7070 6f72 7465 642e  t yet supported.
+00002ff0: 0d0a 2d20 606c 696d 6974 6020 286f 7074  ..- `limit` (opt
+00003000: 696f 6e61 6c29 3a20 5468 6520 746f 6b65  ional): The toke
+00003010: 6e20 6c69 6d69 7420 666f 7220 7468 6520  n limit for the 
+00003020: 6f75 7470 7574 2070 726f 6d70 742c 2064  output prompt, d
+00003030: 6566 6175 6c74 7320 746f 2031 3030 4b2e  efaults to 100K.
+00003040: 2050 726f 6d70 7473 2065 7863 6565 6469   Prompts exceedi
+00003050: 6e67 2074 6865 206c 696d 6974 2077 696c  ng the limit wil
+00003060: 6c20 6265 2063 6f6d 7072 6573 7365 642e  l be compressed.
+00003070: 2054 6869 7320 6d61 7920 6e6f 7420 776f   This may not wo
+00003080: 726b 2061 7320 6578 7065 6374 6564 2077  rk as expected w
+00003090: 6974 6820 7468 6520 4150 492c 2061 7320  ith the API, as 
+000030a0: 6974 2069 7320 696e 2061 6374 6976 6520  it is in active 
+000030b0: 6465 7665 6c6f 706d 656e 742e 0d0a 2d20  development...- 
+000030c0: 6061 695f 6578 7472 6163 7469 6f6e 6020  `ai_extraction` 
+000030d0: 286f 7074 696f 6e61 6c29 3a20 4578 7472  (optional): Extr
+000030e0: 6163 7420 7461 626c 6573 2c20 6669 6775  act tables, figu
+000030f0: 7265 732c 2061 6e64 206d 6174 6820 6672  res, and math fr
+00003100: 6f6d 2050 4446 7320 7573 696e 6720 6f75  om PDFs using ou
+00003110: 7220 6578 7472 6163 746f 722e 2049 6e63  r extractor. Inc
+00003120: 7572 7320 6578 7472 6120 636f 7374 732e  urs extra costs.
+00003130: 0d0a 2d20 6074 6578 745f 6f6e 6c79 6020  ..- `text_only` 
+00003140: 286f 7074 696f 6e61 6c29 3a20 446f 206e  (optional): Do n
+00003150: 6f74 2065 7874 7261 6374 2069 6d61 6765  ot extract image
+00003160: 7320 6672 6f6d 2064 6f63 756d 656e 7473  s from documents
+00003170: 206f 7220 7765 6273 6974 6573 2e20 4164   or websites. Ad
+00003180: 6469 7469 6f6e 616c 6c79 2c20 696d 6167  ditionally, imag
+00003190: 6520 6669 6c65 7320 7769 6c6c 2062 6520  e files will be 
+000031a0: 7265 7072 6573 656e 7465 6420 7769 7468  represented with
+000031b0: 204f 4352 2069 6e73 7465 6164 206f 6620   OCR instead of 
+000031c0: 6173 2069 6d61 6765 732e 0d0a 0d0a 2320  as images.....# 
+000031d0: 5370 6f6e 736f 7273 0d0a 0d0a 3c61 2068  Sponsors....<a h
+000031e0: 7265 663d 2268 7474 7073 3a2f 2f63 616c  ref="https://cal
+000031f0: 2e63 6f6d 2f65 6d6d 6574 742d 6d63 662f  .com/emmett-mcf/
+00003200: 3330 6d69 6e22 3e3c 696d 6720 616c 743d  30min"><img alt=
+00003210: 2242 6f6f 6b20 7573 2077 6974 6820 4361  "Book us with Ca
+00003220: 6c2e 636f 6d22 2073 7263 3d22 6874 7470  l.com" src="http
+00003230: 733a 2f2f 6361 6c2e 636f 6d2f 626f 6f6b  s://cal.com/book
+00003240: 2d77 6974 682d 6361 6c2d 6461 726b 2e73  -with-cal-dark.s
+00003250: 7667 2220 2f3e 3c2f 613e 0d0a 0d0a 5468  vg" /></a>....Th
+00003260: 616e 6b20 796f 7520 746f 205b 4361 6c2e  ank you to [Cal.
+00003270: 636f 6d5d 2868 7474 7073 3a2f 2f63 616c  com](https://cal
+00003280: 2e63 6f6d 2f29 2066 6f72 2073 706f 6e73  .com/) for spons
+00003290: 6f72 696e 6720 7468 6973 2070 726f 6a65  oring this proje
+000032a0: 6374 2e20 436f 6e74 6163 7420 656d 6d65  ct. Contact emme
+000032b0: 7474 4074 6865 7069 2e70 6520 666f 7220  tt@thepi.pe for 
+000032c0: 7370 6f6e 736f 7273 6869 7020 696e 666f  sponsorship info
+000032d0: 726d 6174 696f 6e2e 0d0a                 rmation...
```

### Comparing `thepipe_api-0.3.4/setup.py` & `thepipe_api-0.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='thepipe_api',
-    version='0.3.4',
+    version='0.3.5',
     author='Emmett McFarlane',
     author_email='emmett@thepi.pe',
     description='Automate information extraction for multimodal LLMs.',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/emcf/thepipe',
     packages=find_packages(),
```

### Comparing `thepipe_api-0.3.4/tests/test_thepipe.py` & `thepipe_api-0.3.5/tests/test_thepipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         self.assertNotEqual(len(chunks), 0)
         self.assertEqual(type(chunks[0]), core.Chunk)
         # verify it extracted audio data
         self.assertTrue(any(chunk.text for chunk in chunks))
         # verify it transcribed the audio correctly, i.e., 'citizens' is in the extracted text
         self.assertTrue(any('citizens' in chunk.text.lower() for chunk in chunks if chunk.text is not None))
     
+    @unittest.skipUnless(os.environ.get('TEST_YOUTUBE_DL'), "requires TEST_YOUTUBE_DL")
     def test_extract_youtube(self):
         chunks = extractor.extract_from_source("https://www.youtube.com/watch?v=wUEr7TayrmU")
         # verify it extracted the youtube video into chunks
         self.assertEqual(type(chunks), list)
         self.assertNotEqual(len(chunks), 0)
         self.assertEqual(type(chunks[0]), core.Chunk)
         # verify it extracted visual data
@@ -108,14 +109,15 @@
         # test hidden file ignore
         self.assertTrue(extractor.should_ignore('.gitignore', ignore=None))
         # test directory ignore
         self.assertTrue(extractor.should_ignore('node_modules', ignore=None))
         # test cases that should not be ignored
         self.assertFalse(extractor.should_ignore(self.files_directory+"/example.md", ignore=None))
 
+    @unittest.skipUnless(os.environ.get('TEST_WEB'), "requires TEST_WEB")
     def test_extract_url(self):
         # test web page extraction
         chunks = extractor.extract_url('https://en.wikipedia.org/wiki/Piping')
         for chunk in chunks:
             self.assertEqual(type(chunk), core.Chunk)
             self.assertEqual(chunk.path, 'https://en.wikipedia.org/wiki/Piping')
         if chunk.text:
@@ -142,23 +144,15 @@
                 # verify extraction contains text
                 self.assertIsNotNone(chunks[i].text)
                 # verify extraction text does not contain image data
                 self.assertNotIn('![](', chunks[i].text)
             elif chunks[i].source_type == core.SourceTypes.IMAGE:
                 # verify extraction contains image
                 self.assertIsNotNone(chunks[i].image)
-                
-    def test_compress_spreadsheet(self):
-        chunks = extractor.extract_from_source(source=self.files_directory+"/example.xlsx")
-        new_chunks = compressor.compress_chunks(chunks=chunks, limit=30)
-        # verify that the compressed text is shorter than the original
-        all_text = ''.join([chunk.text for chunk in chunks if chunk.text])
-        all_new_text = ''.join([chunk.text for chunk in new_chunks if chunk.text])
-        self.assertLess(len(all_new_text), len(all_text))
-    
+            
     def test_compress_with_llmlingua(self):
         chunks = extractor.extract_from_source(source=self.files_directory+"/example.md")
         new_chunks = compressor.compress_chunks(chunks=chunks, limit=30)
         # verify that the compressed text is shorter than the original
         old_chunktext = sum([len(chunk.text) for chunk in chunks if chunk.text is not None])
         new_chunktext = sum([len(chunk.text) for chunk in new_chunks if chunk.text is not None])
         self.assertLess(new_chunktext, old_chunktext)
```

### Comparing `thepipe_api-0.3.4/thepipe_api/compressor.py` & `thepipe_api-0.3.5/thepipe_api/compressor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import json
 import shutil
 import subprocess
 import tempfile
-from typing import List
+from typing import List, Optional
 import os
 from .core import Chunk, SourceTypes, print_status, count_tokens
 from .thepipe import count_tokens
+from PIL import Image
 
 CTAGS_EXECUTABLE_PATH = "C:\ctags.exe" if os.name == 'nt' else "ctags-universal"
 CTAGS_LANGUAGES = {'py': "Python", "cpp": "C++", "c": "C"}
 CTAGS_OUTPUT_FILE = 'ctags_output.json'
-MAX_COMPRESSION_ATTEMPTS = 3
+MAX_COMPRESSION_ATTEMPTS = 25
 
 def compress_with_ctags(chunk: Chunk, extension: str) -> Chunk:
     if chunk.text is None:
         return Chunk(path=chunk.path, text=chunk.text, image=chunk.image, source_type=SourceTypes.UNCOMPRESSIBLE_CODE)
     language = CTAGS_LANGUAGES[extension]
     tmp_dir = tempfile.mkdtemp()
     try:
@@ -64,32 +65,64 @@
         window_text = chunk.text[i:i+WINDOW_SIZE]
         result = llm_lingua.compress_prompt(window_text, rate=0.5)
         new_window_text = result['compressed_prompt']
         new_chunk_text += new_window_text
     new_chunk = Chunk(path=chunk.path, text=new_chunk_text, image=chunk.image, source_type=chunk.source_type)
     return new_chunk
 
-def compress_chunks(chunks: List[Chunk], verbose: bool = False, limit: int = 1e5) -> List[Chunk]:
+# uses https://platform.openai.com/docs/guides/vision
+def calculate_image_tokens(image: Image.Image, detail: str = "auto") -> int:
+    width, height = image.size
+    if detail == "low":
+        return 85
+    elif detail == "high":
+        # High detail calculation
+        width, height = min(width, 2048), min(height, 2048)
+        short_side = min(width, height)
+        scale = 768 / short_side
+        scaled_width = int(width * scale)
+        scaled_height = int(height * scale)
+        tiles = (scaled_width // 512) * (scaled_height // 512)
+        return 170 * tiles + 85
+    else:  # auto
+        if width <= 512 and height <= 512:
+            return 85
+        else:
+            return calculate_image_tokens(image, detail="high")
+
+def calculate_tokens(chunk: Chunk) -> int:
+    text_tokens = len(chunk.text)/4 if chunk.text else 0
+    image_tokens = calculate_image_tokens(chunk.image) if chunk.image else 0
+    return max(text_tokens, image_tokens)
+
+def compress_chunks(chunks: List[Chunk], verbose: bool = False, limit: Optional[int] = None) -> List[Chunk]:
     new_chunks = chunks
-    for _ in range(MAX_COMPRESSION_ATTEMPTS):
+    for _ in range(min(MAX_COMPRESSION_ATTEMPTS, len(chunks))):
         if count_tokens(new_chunks) <= limit:
             break
         if verbose: print_status(f"Compressing prompt ({count_tokens(chunks)} tokens / {limit} limit)", status='info')
         new_chunks = []
+        chunk_with_most_tokens = max(chunks, key=calculate_tokens)
         for chunk in chunks:
+            # if not longest, skip
+            if chunk != chunk_with_most_tokens:
+                new_chunks.append(chunk)
+                continue
             new_chunk = None
-            if chunk is None or  chunk.text is None:
+            if chunk is None or chunk.text is None:
                 new_chunk = chunk
             elif chunk.source_type == SourceTypes.COMPRESSIBLE_CODE:
                 extension = chunk.path.split('.')[-1]
                 new_chunk = compress_with_ctags(chunk, extension=extension)
             elif chunk.source_type in {SourceTypes.PLAINTEXT, SourceTypes.PDF, SourceTypes.DOCX, SourceTypes.PPTX, SourceTypes.URL}:
                 new_chunk = compress_with_llmlingua(chunk)
-            elif chunk.source_type == SourceTypes.SPREADSHEET:
-                new_chunk = compress_with_llmlingua(chunk)
             else:
                 # if the chunk is not compressible, keep the original text
                 new_chunk = chunk
+            if new_chunk.image is not None:
+                # resize image to half its current res
+                new_res = (new_chunk.image.width//2, new_chunk.image.height//2)
+                new_chunk.image = new_chunk.image.resize(new_res)
             new_chunks.append(new_chunk)
     if count_tokens(new_chunks) > limit and verbose: 
         print_status("Failed to compress within limit, continuing", status='error')
     return new_chunks
```

### Comparing `thepipe_api-0.3.4/thepipe_api/core.py` & `thepipe_api-0.3.5/thepipe_api/core.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.3.4/thepipe_api/extractor.py` & `thepipe_api-0.3.5/thepipe_api/extractor.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.3.4/thepipe_api/thepipe.py` & `thepipe_api-0.3.5/thepipe_api/thepipe.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.3.4/thepipe_api.egg-info/PKG-INFO` & `thepipe_api-0.3.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,771 +1,765 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2074 6865  : 2.1..Name: the
-00000020: 7069 7065 5f61 7069 0d0a 5665 7273 696f  pipe_api..Versio
-00000030: 6e3a 2030 2e33 2e34 0d0a 5375 6d6d 6172  n: 0.3.4..Summar
-00000040: 793a 2041 7574 6f6d 6174 6520 696e 666f  y: Automate info
-00000050: 726d 6174 696f 6e20 6578 7472 6163 7469  rmation extracti
-00000060: 6f6e 2066 6f72 206d 756c 7469 6d6f 6461  on for multimoda
-00000070: 6c20 4c4c 4d73 2e0d 0a48 6f6d 652d 7061  l LLMs...Home-pa
-00000080: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
-00000090: 7562 2e63 6f6d 2f65 6d63 662f 7468 6570  ub.com/emcf/thep
-000000a0: 6970 650d 0a41 7574 686f 723a 2045 6d6d  ipe..Author: Emm
-000000b0: 6574 7420 4d63 4661 726c 616e 650d 0a41  ett McFarlane..A
-000000c0: 7574 686f 722d 656d 6169 6c3a 2065 6d6d  uthor-email: emm
-000000d0: 6574 7440 7468 6570 692e 7065 0d0a 436c  ett@thepi.pe..Cl
-000000e0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-000000f0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000100: 3a20 5079 7468 6f6e 203a 3a20 330d 0a43  : Python :: 3..C
-00000110: 6c61 7373 6966 6965 723a 204c 6963 656e  lassifier: Licen
-00000120: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
-00000130: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
-00000140: 650d 0a43 6c61 7373 6966 6965 723a 204f  e..Classifier: O
-00000150: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000160: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-00000170: 740d 0a52 6571 7569 7265 732d 5079 7468  t..Requires-Pyth
-00000180: 6f6e 3a20 3e3d 332e 360d 0a44 6573 6372  on: >=3.6..Descr
-00000190: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
-000001a0: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
-000001b0: 776e 0d0a 4c69 6365 6e73 652d 4669 6c65  wn..License-File
-000001c0: 3a20 4c49 4345 4e53 450d 0a52 6571 7569  : LICENSE..Requi
-000001d0: 7265 732d 4469 7374 3a20 6169 6f68 7474  res-Dist: aiohtt
-000001e0: 700d 0a52 6571 7569 7265 732d 4469 7374  p..Requires-Dist
-000001f0: 3a20 6368 6172 7365 742d 6e6f 726d 616c  : charset-normal
-00000200: 697a 6572 0d0a 5265 7175 6972 6573 2d44  izer..Requires-D
-00000210: 6973 743a 2050 7961 7272 6f77 0d0a 5265  ist: Pyarrow..Re
-00000220: 7175 6972 6573 2d44 6973 743a 2070 7974  quires-Dist: pyt
-00000230: 686f 6e2d 6d61 6769 630d 0a52 6571 7569  hon-magic..Requi
-00000240: 7265 732d 4469 7374 3a20 636f 6c6f 7261  res-Dist: colora
-00000250: 6d61 0d0a 5265 7175 6972 6573 2d44 6973  ma..Requires-Dis
-00000260: 743a 2072 6571 7565 7374 730d 0a52 6571  t: requests..Req
-00000270: 7569 7265 732d 4469 7374 3a20 7069 6c6c  uires-Dist: pill
-00000280: 6f77 0d0a 5265 7175 6972 6573 2d44 6973  ow..Requires-Dis
-00000290: 743a 2063 7373 7574 696c 730d 0a52 6571  t: cssutils..Req
-000002a0: 7569 7265 732d 4469 7374 3a20 6265 6175  uires-Dist: beau
-000002b0: 7469 6675 6c73 6f75 7034 0d0a 5265 7175  tifulsoup4..Requ
-000002c0: 6972 6573 2d44 6973 743a 206d 6167 696b  ires-Dist: magik
-000002d0: 610d 0a52 6571 7569 7265 732d 4469 7374  a..Requires-Dist
-000002e0: 3a20 7079 7468 6f6e 2d64 6f74 656e 760d  : python-dotenv.
-000002f0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000300: 6f70 656e 7079 786c 0d0a 0d0a 0d0a 2320  openpyxl......# 
-00000310: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000320: 2f74 6865 7069 2e70 652f 223e 3c69 6d67  /thepi.pe/"><img
-00000330: 2073 7263 3d22 6874 7470 733a 2f2f 7270   src="https://rp
-00000340: 6e75 747a 656d 7574 6272 756d 637a 7776  nutzemutbrumczwv
-00000350: 7565 2e73 7570 6162 6173 652e 636f 2f73  ue.supabase.co/s
-00000360: 746f 7261 6765 2f76 312f 6f62 6a65 6374  torage/v1/object
-00000370: 2f70 7562 6c69 632f 6173 7365 7473 2f70  /public/assets/p
-00000380: 6970 656c 696e 655f 736d 616c 6c25 3230  ipeline_small%20
-00000390: 2831 292e 706e 6722 2061 6c74 3d22 5069  (1).png" alt="Pi
-000003a0: 7065 6c69 6e65 2049 6c6c 7573 7472 6174  peline Illustrat
-000003b0: 696f 6e22 2073 7479 6c65 3d22 7769 6474  ion" style="widt
-000003c0: 683a 3936 7078 3b20 6865 6967 6874 3a37  h:96px; height:7
-000003d0: 3270 783b 2076 6572 7469 6361 6c2d 616c  2px; vertical-al
-000003e0: 6967 6e3a 6d69 6464 6c65 3b22 3e20 5468  ign:middle;"> Th
-000003f0: 6520 5069 7065 3c2f 613e 0d0a 3c70 3e0d  e Pipe</a>..<p>.
-00000400: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
-00000410: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
-00000420: 6d63 662f 7468 6570 6970 652f 626c 6f62  mcf/thepipe/blob
-00000430: 2f6d 6169 6e2f 5245 4144 4d45 2e6d 6422  /main/README.md"
-00000440: 3e45 6e67 6c69 7368 3c2f 613e 207c 203c  >English</a> | <
-00000450: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000460: 6769 7468 7562 2e63 6f6d 2f65 6d63 662f  github.com/emcf/
-00000470: 7468 6570 6970 652f 626c 6f62 2f6d 6169  thepipe/blob/mai
-00000480: 6e2f 5245 4144 4d45 5f63 6e2e 6d64 223e  n/README_cn.md">
-00000490: e4b8 ade6 9687 3c2f 613e 0d0a 3c2f 703e  ......</a>..</p>
-000004a0: 0d0a 0d0a 5b21 5b63 6f64 6563 6f76 5d28  ....[![codecov](
-000004b0: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
-000004c0: 696f 2f67 682f 656d 6366 2f74 6865 7069  io/gh/emcf/thepi
-000004d0: 7065 2f67 7261 7068 2f62 6164 6765 2e73  pe/graph/badge.s
-000004e0: 7667 3f74 6f6b 656e 3d4f 4537 4355 4546  vg?token=OE7CUEF
-000004f0: 554c 3929 5d28 6874 7470 733a 2f2f 636f  UL9)](https://co
-00000500: 6465 636f 762e 696f 2f67 682f 656d 6366  decov.io/gh/emcf
-00000510: 2f74 6865 7069 7065 2920 215b 7079 7468  /thepipe) ![pyth
-00000520: 6f6e 2d67 682d 6163 7469 6f6e 5d28 6874  on-gh-action](ht
-00000530: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000540: 2f65 6d63 662f 7468 6570 6970 652f 6163  /emcf/thepipe/ac
-00000550: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000560: 7079 7468 6f6e 2d63 692e 796d 6c2f 6261  python-ci.yml/ba
-00000570: 6467 652e 7376 6729 203c 6120 6872 6566  dge.svg) <a href
-00000580: 3d22 6874 7470 733a 2f2f 7468 6570 692e  ="https://thepi.
-00000590: 7065 2f22 3e21 5b57 6562 7369 7465 5d28  pe/">![Website](
-000005a0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000005b0: 6c64 732e 696f 2f77 6562 7369 7465 3f75  lds.io/website?u
-000005c0: 726c 3d68 7474 7073 2533 4125 3246 2532  rl=https%3A%2F%2
-000005d0: 4674 6865 7069 7065 2e75 702e 7261 696c  Fthepipe.up.rail
-000005e0: 7761 792e 6170 7025 3246 266c 6162 656c  way.app%2F&label
-000005f0: 3d41 5049 2532 3073 7461 7475 7329 3c2f  =API%20status)</
-00000600: 613e 203c 6120 6872 6566 3d22 6874 7470  a> <a href="http
-00000610: 733a 2f2f 7468 6570 692e 7065 2f22 3e21  s://thepi.pe/">!
-00000620: 5b67 6574 2041 5049 5d28 6874 7470 733a  [get API](https:
-00000630: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000640: 2f62 6164 6765 2f41 5049 2d61 6363 6573  /badge/API-acces
-00000650: 732d 626c 7565 293c 2f61 3e20 3c61 2068  s-blue)</a> <a h
-00000660: 7265 663d 2268 7474 7073 3a2f 2f64 6973  ref="https://dis
-00000670: 636f 7264 2e67 672f 6258 664b 6547 7335  cord.gg/bXfKeGs5
-00000680: 7156 223e 215b 4a6f 696e 2064 6973 636f  qV">![Join disco
-00000690: 7264 5d28 6874 7470 733a 2f2f 696d 672e  rd](https://img.
-000006a0: 7368 6965 6c64 732e 696f 2f64 6973 636f  shields.io/disco
-000006b0: 7264 2f31 3232 3738 3036 3230 3034 3738  rd/1227806200478
-000006c0: 3034 3432 3734 3f63 6f6c 6f72 3d34 6636  044274?color=4f6
-000006d0: 3965 6626 6c61 6265 6c3d 4469 7363 6f72  9ef&label=Discor
-000006e0: 6426 6c6f 676f 3d64 6973 636f 7264 266c  d&logo=discord&l
-000006f0: 6f67 6f43 6f6c 6f72 3d66 6666 6666 6629  ogoColor=ffffff)
-00000700: 3c2f 613e 0d0a 0d0a 2323 2320 4665 6564  </a>....### Feed
-00000710: 2050 4446 732c 2055 524c 732c 2053 6c69   PDFs, URLs, Sli
-00000720: 6465 732c 2059 6f75 5475 6265 2076 6964  des, YouTube vid
-00000730: 656f 732c 2057 6f72 6420 646f 6373 2061  eos, Word docs a
-00000740: 6e64 206d 6f72 6520 696e 746f 2056 6973  nd more into Vis
-00000750: 696f 6e2d 4c61 6e67 7561 6765 206d 6f64  ion-Language mod
-00000760: 656c 7320 7769 7468 206f 6e65 206c 696e  els with one lin
-00000770: 6520 6f66 2063 6f64 6520 e29a a10d 0a0d  e of code ......
-00000780: 0a54 6865 2050 6970 6520 6973 2061 206d  .The Pipe is a m
-00000790: 756c 7469 6d6f 6461 6c2d 6669 7273 7420  ultimodal-first 
-000007a0: 746f 6f6c 2066 6f72 2066 6565 6469 6e67  tool for feeding
-000007b0: 2066 696c 6573 2061 6e64 2077 6562 2070   files and web p
-000007c0: 6167 6573 2069 6e74 6f20 7669 7369 6f6e  ages into vision
-000007d0: 2d6c 616e 6775 6167 6520 6d6f 6465 6c73  -language models
-000007e0: 2073 7563 6820 6173 2047 5054 2d34 562e   such as GPT-4V.
-000007f0: 2049 7420 6973 2062 6573 7420 666f 7220   It is best for 
-00000800: 4c4c 4d20 616e 6420 5241 4720 6170 706c  LLM and RAG appl
-00000810: 6963 6174 696f 6e73 2074 6861 7420 7761  ications that wa
-00000820: 6e74 2074 6f20 7375 7070 6f72 7420 636f  nt to support co
-00000830: 6d70 7265 6865 6e73 6976 6520 7465 7874  mprehensive text
-00000840: 7561 6c20 616e 6420 7669 7375 616c 2075  ual and visual u
-00000850: 6e64 6572 7374 616e 6469 6e67 2061 6372  nderstanding acr
-00000860: 6f73 7320 6120 7769 6465 2072 616e 6765  oss a wide range
-00000870: 206f 6620 6461 7461 2073 6f75 7263 6573   of data sources
-00000880: 2e20 5468 6520 5069 7065 2069 7320 6176  . The Pipe is av
-00000890: 6169 6c61 626c 6520 6173 2061 2032 342f  ailable as a 24/
-000008a0: 3720 686f 7374 6564 2041 5049 2061 7420  7 hosted API at 
-000008b0: 5b74 6865 7069 2e70 655d 2868 7474 7073  [thepi.pe](https
-000008c0: 3a2f 2f74 6865 7069 2e70 6529 2c20 6f72  ://thepi.pe), or
-000008d0: 2069 7420 6361 6e20 6265 2073 6574 2075   it can be set u
-000008e0: 7020 6c6f 6361 6c6c 7920 746f 206c 6574  p locally to let
-000008f0: 2079 6f75 2072 756e 2074 6865 2063 6f6d   you run the com
-00000900: 7075 7465 2e0d 0a0d 0a21 5b53 6369 656e  pute.....![Scien
-00000910: 6365 2061 7373 6973 7461 6e74 2064 656d  ce assistant dem
-00000920: 6f5d 2868 7474 7073 3a2f 2f72 706e 7574  o](https://rpnut
-00000930: 7a65 6d75 7462 7275 6d63 7a77 7675 652e  zemutbrumczwvue.
-00000940: 7375 7061 6261 7365 2e63 6f2f 7374 6f72  supabase.co/stor
-00000950: 6167 652f 7631 2f6f 626a 6563 742f 7075  age/v1/object/pu
-00000960: 626c 6963 2f61 7373 6574 732f 7363 6965  blic/assets/scie
-00000970: 6e63 655f 6173 7369 7374 616e 7470 7932  nce_assistantpy2
-00000980: 2e70 6e67 290d 0a0d 0a0d 0a23 2320 4665  .png)......## Fe
-00000990: 6174 7572 6573 20f0 9f8c 9f0d 0a0d 0a2d  atures ........-
-000009a0: 2045 7874 7261 6374 7320 7465 7874 2061   Extracts text a
-000009b0: 6e64 2076 6973 7561 6c73 2066 726f 6d20  nd visuals from 
-000009c0: 6669 6c65 7320 6f72 2077 6562 2070 6167  files or web pag
-000009d0: 6573 20f0 9f93 9a0d 0a2d 204f 7574 7075  es ......- Outpu
-000009e0: 7473 2063 6875 6e6b 7320 6f70 7469 6d69  ts chunks optimi
-000009f0: 7a65 6420 666f 7220 6d75 6c74 696d 6f64  zed for multimod
-00000a00: 616c 204c 4c4d 7320 616e 6420 5241 4720  al LLMs and RAG 
-00000a10: 6672 616d 6577 6f72 6b73 20f0 9f96 bcef  frameworks .....
-00000a20: b88f 0d0a 2d20 496e 7465 7270 7265 7420  ....- Interpret 
-00000a30: 636f 6d70 6c65 7820 5044 4673 2c20 7765  complex PDFs, we
-00000a40: 6220 7061 6765 732c 2064 6f63 732c 2076  b pages, docs, v
-00000a50: 6964 656f 732c 2064 6174 612c 2061 6e64  ideos, data, and
-00000a60: 206d 6f72 6520 f09f a7a0 0d0a 2d20 4175   more ......- Au
-00000a70: 746f 2d63 6f6d 7072 6573 7320 7072 6f6d  to-compress prom
-00000a80: 7074 7320 6578 6365 6564 696e 6720 796f  pts exceeding yo
-00000a90: 7572 2063 686f 7365 6e20 746f 6b65 6e20  ur chosen token 
-00000aa0: 6c69 6d69 7420 f09f 93a6 0d0a 2d20 576f  limit ......- Wo
-00000ab0: 726b 7320 6576 656e 2077 6974 6820 6d69  rks even with mi
-00000ac0: 7373 696e 6720 6669 6c65 2065 7874 656e  ssing file exten
-00000ad0: 7369 6f6e 732c 2069 6e2d 6d65 6d6f 7279  sions, in-memory
-00000ae0: 2064 6174 6120 7374 7265 616d 7320 f09f   data streams ..
-00000af0: 92be 0d0a 2d20 576f 726b 7320 7769 7468  ....- Works with
-00000b00: 2063 6f64 6562 6173 6573 2c20 6769 7420   codebases, git 
-00000b10: 7265 706f 732c 2061 6e64 2063 7573 746f  repos, and custo
-00000b20: 6d20 696e 7465 6772 6174 696f 6e73 20f0  m integrations .
-00000b30: 9f8c 900d 0a2d 204d 756c 7469 2d74 6872  .....- Multi-thr
-00000b40: 6561 6465 6420 e29a a1ef b88f 0d0a 0d0a  eaded ..........
-00000b50: 2323 2047 6574 7469 6e67 2053 7461 7274  ## Getting Start
-00000b60: 6564 2020 f09f 9a80 0d0a 0d0a 5468 6520  ed  ........The 
-00000b70: 5069 7065 2068 616e 646c 6573 2061 2077  Pipe handles a w
-00000b80: 6964 6520 6172 7261 7920 6f66 2063 6f6d  ide array of com
-00000b90: 706c 6578 2066 696c 6574 7970 6573 2c20  plex filetypes, 
-00000ba0: 616e 6420 7468 7573 2068 6173 206d 616e  and thus has man
-00000bb0: 7920 6465 7065 6e64 656e 6369 6573 2074  y dependencies t
-00000bc0: 6861 7420 6d75 7374 2062 6520 696e 7374  hat must be inst
-00000bd0: 616c 6c65 6420 7365 7061 7261 7465 6c79  alled separately
-00000be0: 2e20 4974 2061 6c73 6f20 7265 7175 6972  . It also requir
-00000bf0: 6573 2061 2073 7472 6f6e 6720 6d61 6368  es a strong mach
-00000c00: 696e 6520 666f 7220 676f 6f64 2072 6573  ine for good res
-00000c10: 706f 6e73 6520 7469 6d65 732e 2046 6f72  ponse times. For
-00000c20: 2074 6869 7320 7265 6173 6f6e 2c20 7765   this reason, we
-00000c30: 2068 6f73 7420 6974 2061 7320 616e 2041   host it as an A
-00000c40: 5049 2074 6861 7420 776f 726b 7320 6f75  PI that works ou
-00000c50: 742d 6f66 2d74 6865 2d62 6f78 2e20 0d0a  t-of-the-box. ..
-00000c60: 0d0a 4669 7273 742c 2069 6e73 7461 6c6c  ..First, install
-00000c70: 2054 6865 2050 6970 652e 200d 0a60 6060   The Pipe. ..```
-00000c80: 0d0a 7069 7020 696e 7374 616c 6c20 7468  ..pip install th
-00000c90: 6570 6970 655f 6170 690d 0a60 6060 0d0a  epipe_api..```..
-00000ca0: 0d0a 5468 6520 5069 7065 2069 7320 6176  ..The Pipe is av
-00000cb0: 6169 6c61 626c 6520 6173 2061 2068 6f73  ailable as a hos
-00000cc0: 7465 6420 4150 492c 206f 7220 6974 2063  ted API, or it c
-00000cd0: 616e 2062 6520 7365 7420 7570 206c 6f63  an be set up loc
-00000ce0: 616c 6c79 2e20 416e 2041 5049 206b 6579  ally. An API key
-00000cf0: 2069 7320 7265 636f 6d6d 656e 6465 6420   is recommended 
-00000d00: 666f 7220 6f75 742d 6f66 2d74 6865 2d62  for out-of-the-b
-00000d10: 6f78 2066 756e 6374 696f 6e61 6c69 7479  ox functionality
-00000d20: 2028 616c 7465 726e 6174 6976 656c 792c   (alternatively,
-00000d30: 2073 6565 2074 6865 206c 6f63 616c 2069   see the local i
-00000d40: 6e73 7461 6c6c 6174 696f 6e20 7365 6374  nstallation sect
-00000d50: 696f 6e29 2e20 456e 7375 7265 2074 6865  ion). Ensure the
-00000d60: 2060 5448 4550 4950 455f 4150 495f 4b45   `THEPIPE_API_KE
-00000d70: 5960 2065 6e76 6972 6f6e 6d65 6e74 2076  Y` environment v
-00000d80: 6172 6961 626c 6520 6973 2073 6574 2e20  ariable is set. 
-00000d90: 446f 6e27 7420 6861 7665 2061 206b 6579  Don't have a key
-00000da0: 2079 6574 3f20 5b47 6574 206f 6e65 2068   yet? [Get one h
-00000db0: 6572 655d 2868 7474 7073 3a2f 2f74 6865  ere](https://the
-00000dc0: 7069 2e70 6529 2e0d 0a0d 0a4e 6f77 2079  pi.pe).....Now y
-00000dd0: 6f75 2063 616e 2065 7874 7261 6374 2063  ou can extract c
-00000de0: 6f6d 7072 6568 656e 7369 7665 2074 6578  omprehensive tex
-00000df0: 7420 616e 6420 7669 7375 616c 7320 6672  t and visuals fr
-00000e00: 6f6d 2061 6e79 2066 696c 653a 0d0a 6060  om any file:..``
-00000e10: 6070 7974 686f 6e0d 0a66 726f 6d20 7468  `python..from th
-00000e20: 6570 6970 655f 6170 6920 696d 706f 7274  epipe_api import
-00000e30: 2074 6865 7069 7065 0d0a 6d65 7373 6167   thepipe..messag
-00000e40: 6573 203d 2074 6865 7069 7065 2e65 7874  es = thepipe.ext
-00000e50: 7261 6374 2822 6578 616d 706c 652e 7064  ract("example.pd
-00000e60: 6622 290d 0a60 6060 0d0a 4f72 2077 6562  f")..```..Or web
-00000e70: 7369 7465 733a 0d0a 6060 6070 7974 686f  sites:..```pytho
-00000e80: 6e0d 0a6d 6573 7361 6765 7320 3d20 7468  n..messages = th
-00000e90: 6570 6970 652e 6578 7472 6163 7428 2268  epipe.extract("h
-00000ea0: 7474 7073 3a2f 2f65 7861 6d70 6c65 2e63  ttps://example.c
-00000eb0: 6f6d 2229 0d0a 6060 600d 0a54 6865 6e20  om")..```..Then 
-00000ec0: 6665 6564 2069 7420 696e 746f 2047 5054  feed it into GPT
-00000ed0: 2d34 2d56 6973 696f 6e3a 0d0a 6060 6070  -4-Vision:..```p
-00000ee0: 7974 686f 6e0d 0a72 6573 706f 6e73 6520  ython..response 
-00000ef0: 3d20 636c 6965 6e74 2e63 6861 742e 636f  = client.chat.co
-00000f00: 6d70 6c65 7469 6f6e 732e 6372 6561 7465  mpletions.create
-00000f10: 280d 0a20 2020 206d 6f64 656c 3d22 6770  (..    model="gp
-00000f20: 742d 342d 7669 7369 6f6e 2d70 7265 7669  t-4-vision-previ
-00000f30: 6577 222c 0d0a 2020 2020 6d65 7373 6167  ew",..    messag
-00000f40: 6573 203d 206d 6573 7361 6765 732c 0d0a  es = messages,..
-00000f50: 290d 0a60 6060 0d0a 0d0a 215b 4a75 7374  )..```....![Just
-00000f60: 2063 616c 6c20 4f70 656e 4149 5d28 6874   call OpenAI](ht
-00000f70: 7470 733a 2f2f 7270 6e75 747a 656d 7574  tps://rpnutzemut
-00000f80: 6272 756d 637a 7776 7565 2e73 7570 6162  brumczwvue.supab
-00000f90: 6173 652e 636f 2f73 746f 7261 6765 2f76  ase.co/storage/v
-00000fa0: 312f 6f62 6a65 6374 2f70 7562 6c69 632f  1/object/public/
-00000fb0: 6173 7365 7473 2f49 4d47 5f30 3138 302e  assets/IMG_0180.
-00000fc0: 6a70 6729 0d0a 0d0a 596f 7520 6361 6e20  jpg)....You can 
-00000fd0: 616c 736f 2075 7365 2054 6865 2050 6970  also use The Pip
-00000fe0: 6520 6672 6f6d 2074 6865 2063 6f6d 6d61  e from the comma
-00000ff0: 6e64 206c 696e 652e 2048 6572 6527 7320  nd line. Here's 
-00001000: 686f 7720 746f 2072 6563 7572 7369 7665  how to recursive
-00001010: 6c79 2065 7874 7261 6374 2066 726f 6d20  ly extract from 
-00001020: 6120 6469 7265 6374 6f72 792c 206d 6174  a directory, mat
-00001030: 6368 696e 6720 6f6e 6c79 2066 696c 6573  ching only files
-00001040: 2063 6f6e 7461 696e 696e 6720 6120 7375   containing a su
-00001050: 6273 7472 696e 6720 2869 6e20 7468 6973  bstring (in this
-00001060: 2065 7861 6d70 6c65 2c20 7479 7065 7363   example, typesc
-00001070: 7269 7074 2066 696c 6573 2920 616e 6420  ript files) and 
-00001080: 6967 6e6f 7265 2066 696c 6573 2063 6f6e  ignore files con
-00001090: 7461 696e 696e 6720 6f74 6865 7220 7375  taining other su
-000010a0: 6273 7472 696e 6773 2028 696e 2074 6869  bstrings (in thi
-000010b0: 7320 6578 616d 706c 652c 2061 6e79 7468  s example, anyth
-000010c0: 696e 6720 696e 2074 6865 2022 7465 7374  ing in the "test
-000010d0: 7322 2066 6f6c 6465 7229 3a0d 0a60 6060  s" folder):..```
-000010e0: 6261 7368 0d0a 7468 6570 6970 6520 7061  bash..thepipe pa
-000010f0: 7468 2f74 6f2f 666f 6c64 6572 202d 2d6d  th/to/folder --m
-00001100: 6174 6368 2074 7378 202d 2d69 676e 6f72  atch tsx --ignor
-00001110: 6520 7465 7374 730d 0a60 6060 0d0a 0d0a  e tests..```....
-00001120: 0d0a 2323 2053 7570 706f 7274 6564 2046  ..## Supported F
-00001130: 696c 6520 5479 7065 7320 f09f 939a 0d0a  ile Types ......
-00001140: 0d0a 7c20 536f 7572 6365 2054 7970 6520  ..| Source Type 
+00000000: 0d0a 2320 3c61 2068 7265 663d 2268 7474  ..# <a href="htt
+00000010: 7073 3a2f 2f74 6865 7069 2e70 652f 223e  ps://thepi.pe/">
+00000020: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000030: 2f2f 7270 6e75 747a 656d 7574 6272 756d  //rpnutzemutbrum
+00000040: 637a 7776 7565 2e73 7570 6162 6173 652e  czwvue.supabase.
+00000050: 636f 2f73 746f 7261 6765 2f76 312f 6f62  co/storage/v1/ob
+00000060: 6a65 6374 2f70 7562 6c69 632f 6173 7365  ject/public/asse
+00000070: 7473 2f70 6970 656c 696e 655f 736d 616c  ts/pipeline_smal
+00000080: 6c25 3230 2831 292e 706e 6722 2061 6c74  l%20(1).png" alt
+00000090: 3d22 5069 7065 6c69 6e65 2049 6c6c 7573  ="Pipeline Illus
+000000a0: 7472 6174 696f 6e22 2073 7479 6c65 3d22  tration" style="
+000000b0: 7769 6474 683a 3936 7078 3b20 6865 6967  width:96px; heig
+000000c0: 6874 3a37 3270 783b 2076 6572 7469 6361  ht:72px; vertica
+000000d0: 6c2d 616c 6967 6e3a 6d69 6464 6c65 3b22  l-align:middle;"
+000000e0: 3e20 5468 6520 5069 7065 3c2f 613e 0d0a  > The Pipe</a>..
+000000f0: 3c70 3e0d 0a20 203c 6120 6872 6566 3d22  <p>..  <a href="
+00000100: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000110: 6f6d 2f65 6d63 662f 7468 6570 6970 652f  om/emcf/thepipe/
+00000120: 626c 6f62 2f6d 6169 6e2f 5245 4144 4d45  blob/main/README
+00000130: 2e6d 6422 3e45 6e67 6c69 7368 3c2f 613e  .md">English</a>
+00000140: 207c 203c 6120 6872 6566 3d22 6874 7470   | <a href="http
+00000150: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
+00000160: 6d63 662f 7468 6570 6970 652f 626c 6f62  mcf/thepipe/blob
+00000170: 2f6d 6169 6e2f 5245 4144 4d45 5f63 6e2e  /main/README_cn.
+00000180: 6d64 223e e4b8 ade6 9687 3c2f 613e 0d0a  md">......</a>..
+00000190: 3c2f 703e 0d0a 0d0a 5b21 5b63 6f64 6563  </p>....[![codec
+000001a0: 6f76 5d28 6874 7470 733a 2f2f 636f 6465  ov](https://code
+000001b0: 636f 762e 696f 2f67 682f 656d 6366 2f74  cov.io/gh/emcf/t
+000001c0: 6865 7069 7065 2f67 7261 7068 2f62 6164  hepipe/graph/bad
+000001d0: 6765 2e73 7667 3f74 6f6b 656e 3d4f 4537  ge.svg?token=OE7
+000001e0: 4355 4546 554c 3929 5d28 6874 7470 733a  CUEFUL9)](https:
+000001f0: 2f2f 636f 6465 636f 762e 696f 2f67 682f  //codecov.io/gh/
+00000200: 656d 6366 2f74 6865 7069 7065 2920 215b  emcf/thepipe) ![
+00000210: 7079 7468 6f6e 2d67 682d 6163 7469 6f6e  python-gh-action
+00000220: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000230: 2e63 6f6d 2f65 6d63 662f 7468 6570 6970  .com/emcf/thepip
+00000240: 652f 6163 7469 6f6e 732f 776f 726b 666c  e/actions/workfl
+00000250: 6f77 732f 7079 7468 6f6e 2d63 692e 796d  ows/python-ci.ym
+00000260: 6c2f 6261 6467 652e 7376 6729 203c 6120  l/badge.svg) <a 
+00000270: 6872 6566 3d22 6874 7470 733a 2f2f 7468  href="https://th
+00000280: 6570 692e 7065 2f22 3e21 5b57 6562 7369  epi.pe/">![Websi
+00000290: 7465 5d28 6874 7470 733a 2f2f 696d 672e  te](https://img.
+000002a0: 7368 6965 6c64 732e 696f 2f77 6562 7369  shields.io/websi
+000002b0: 7465 3f75 726c 3d68 7474 7073 2533 4125  te?url=https%3A%
+000002c0: 3246 2532 4674 6865 7069 7065 2e75 702e  2F%2Fthepipe.up.
+000002d0: 7261 696c 7761 792e 6170 7025 3246 266c  railway.app%2F&l
+000002e0: 6162 656c 3d41 5049 2532 3073 7461 7475  abel=API%20statu
+000002f0: 7329 3c2f 613e 203c 6120 6872 6566 3d22  s)</a> <a href="
+00000300: 6874 7470 733a 2f2f 7468 6570 692e 7065  https://thepi.pe
+00000310: 2f22 3e21 5b67 6574 2041 5049 5d28 6874  /">![get API](ht
+00000320: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000330: 732e 696f 2f62 6164 6765 2f41 5049 2d61  s.io/badge/API-a
+00000340: 6363 6573 732d 626c 7565 293c 2f61 3e20  ccess-blue)</a> 
+00000350: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000360: 2f64 6973 636f 7264 2e67 672f 6258 664b  /discord.gg/bXfK
+00000370: 6547 7335 7156 223e 215b 4a6f 696e 2064  eGs5qV">![Join d
+00000380: 6973 636f 7264 5d28 6874 7470 733a 2f2f  iscord](https://
+00000390: 696d 672e 7368 6965 6c64 732e 696f 2f64  img.shields.io/d
+000003a0: 6973 636f 7264 2f31 3232 3738 3036 3230  iscord/122780620
+000003b0: 3034 3738 3034 3432 3734 3f63 6f6c 6f72  0478044274?color
+000003c0: 3d34 6636 3965 6626 6c61 6265 6c3d 4469  =4f69ef&label=Di
+000003d0: 7363 6f72 6426 6c6f 676f 3d64 6973 636f  scord&logo=disco
+000003e0: 7264 266c 6f67 6f43 6f6c 6f72 3d66 6666  rd&logoColor=fff
+000003f0: 6666 6629 3c2f 613e 0d0a 0d0a 2323 2320  fff)</a>....### 
+00000400: 4665 6564 2050 4446 732c 2055 524c 732c  Feed PDFs, URLs,
+00000410: 2053 6c69 6465 732c 2059 6f75 5475 6265   Slides, YouTube
+00000420: 2076 6964 656f 732c 2057 6f72 6420 646f   videos, Word do
+00000430: 6373 2061 6e64 206d 6f72 6520 696e 746f  cs and more into
+00000440: 2056 6973 696f 6e2d 4c61 6e67 7561 6765   Vision-Language
+00000450: 206d 6f64 656c 7320 7769 7468 206f 6e65   models with one
+00000460: 206c 696e 6520 6f66 2063 6f64 6520 e29a   line of code ..
+00000470: a10d 0a0d 0a54 6865 2050 6970 6520 6973  .....The Pipe is
+00000480: 2061 206d 756c 7469 6d6f 6461 6c2d 6669   a multimodal-fi
+00000490: 7273 7420 746f 6f6c 2066 6f72 2066 6565  rst tool for fee
+000004a0: 6469 6e67 2066 696c 6573 2061 6e64 2077  ding files and w
+000004b0: 6562 2070 6167 6573 2069 6e74 6f20 7669  eb pages into vi
+000004c0: 7369 6f6e 2d6c 616e 6775 6167 6520 6d6f  sion-language mo
+000004d0: 6465 6c73 2073 7563 6820 6173 2047 5054  dels such as GPT
+000004e0: 2d34 562e 2049 7420 6973 2062 6573 7420  -4V. It is best 
+000004f0: 666f 7220 4c4c 4d20 616e 6420 5241 4720  for LLM and RAG 
+00000500: 6170 706c 6963 6174 696f 6e73 2074 6861  applications tha
+00000510: 7420 7761 6e74 2074 6f20 7375 7070 6f72  t want to suppor
+00000520: 7420 636f 6d70 7265 6865 6e73 6976 6520  t comprehensive 
+00000530: 7465 7874 7561 6c20 616e 6420 7669 7375  textual and visu
+00000540: 616c 2075 6e64 6572 7374 616e 6469 6e67  al understanding
+00000550: 2061 6372 6f73 7320 6120 7769 6465 2072   across a wide r
+00000560: 616e 6765 206f 6620 6461 7461 2073 6f75  ange of data sou
+00000570: 7263 6573 2e20 5468 6520 5069 7065 2069  rces. The Pipe i
+00000580: 7320 6176 6169 6c61 626c 6520 6173 2061  s available as a
+00000590: 2068 6f73 7465 6420 4150 4920 6174 205b   hosted API at [
+000005a0: 7468 6570 692e 7065 5d28 6874 7470 733a  thepi.pe](https:
+000005b0: 2f2f 7468 6570 692e 7065 292c 206f 7220  //thepi.pe), or 
+000005c0: 6974 2063 616e 2062 6520 7365 7420 7570  it can be set up
+000005d0: 206c 6f63 616c 6c79 2069 6620 796f 7520   locally if you 
+000005e0: 6861 7665 2074 6865 2074 6865 2063 6f6d  have the the com
+000005f0: 7075 7465 2e0d 0a0d 0a21 5b53 6369 656e  pute.....![Scien
+00000600: 6365 2061 7373 6973 7461 6e74 2064 656d  ce assistant dem
+00000610: 6f5d 2868 7474 7073 3a2f 2f72 706e 7574  o](https://rpnut
+00000620: 7a65 6d75 7462 7275 6d63 7a77 7675 652e  zemutbrumczwvue.
+00000630: 7375 7061 6261 7365 2e63 6f2f 7374 6f72  supabase.co/stor
+00000640: 6167 652f 7631 2f6f 626a 6563 742f 7075  age/v1/object/pu
+00000650: 626c 6963 2f61 7373 6574 732f 7363 6965  blic/assets/scie
+00000660: 6e63 655f 6173 7369 7374 616e 7470 7932  nce_assistantpy2
+00000670: 2e70 6e67 290d 0a0d 0a0d 0a23 2320 4665  .png)......## Fe
+00000680: 6174 7572 6573 20f0 9f8c 9f0d 0a0d 0a2d  atures ........-
+00000690: 2045 7874 7261 6374 7320 7465 7874 2061   Extracts text a
+000006a0: 6e64 2076 6973 7561 6c73 2066 726f 6d20  nd visuals from 
+000006b0: 6669 6c65 7320 6f72 2077 6562 2070 6167  files or web pag
+000006c0: 6573 20f0 9f93 9a0d 0a2d 204f 7574 7075  es ......- Outpu
+000006d0: 7473 2063 6875 6e6b 7320 6f70 7469 6d69  ts chunks optimi
+000006e0: 7a65 6420 666f 7220 6d75 6c74 696d 6f64  zed for multimod
+000006f0: 616c 204c 4c4d 7320 616e 6420 5241 4720  al LLMs and RAG 
+00000700: 6672 616d 6577 6f72 6b73 20f0 9f96 bcef  frameworks .....
+00000710: b88f 0d0a 2d20 496e 7465 7270 7265 7420  ....- Interpret 
+00000720: 636f 6d70 6c65 7820 5044 4673 2c20 7765  complex PDFs, we
+00000730: 6220 7061 6765 732c 2064 6f63 732c 2076  b pages, docs, v
+00000740: 6964 656f 732c 2064 6174 612c 2061 6e64  ideos, data, and
+00000750: 206d 6f72 6520 f09f a7a0 0d0a 2d20 4175   more ......- Au
+00000760: 746f 2d63 6f6d 7072 6573 7320 7072 6f6d  to-compress prom
+00000770: 7074 7320 6578 6365 6564 696e 6720 796f  pts exceeding yo
+00000780: 7572 2063 686f 7365 6e20 746f 6b65 6e20  ur chosen token 
+00000790: 6c69 6d69 7420 f09f 93a6 0d0a 2d20 576f  limit ......- Wo
+000007a0: 726b 7320 6576 656e 2077 6974 6820 6d69  rks even with mi
+000007b0: 7373 696e 6720 6669 6c65 2065 7874 656e  ssing file exten
+000007c0: 7369 6f6e 732c 2069 6e2d 6d65 6d6f 7279  sions, in-memory
+000007d0: 2064 6174 6120 7374 7265 616d 7320 f09f   data streams ..
+000007e0: 92be 0d0a 2d20 576f 726b 7320 7769 7468  ....- Works with
+000007f0: 2063 6f64 6562 6173 6573 2c20 6769 7420   codebases, git 
+00000800: 7265 706f 732c 2061 6e64 2063 7573 746f  repos, and custo
+00000810: 6d20 696e 7465 6772 6174 696f 6e73 20f0  m integrations .
+00000820: 9f8c 900d 0a2d 204d 756c 7469 2d74 6872  .....- Multi-thr
+00000830: 6561 6465 6420 e29a a1ef b88f 0d0a 0d0a  eaded ..........
+00000840: 2323 2047 6574 7469 6e67 2053 7461 7274  ## Getting Start
+00000850: 6564 2020 f09f 9a80 0d0a 0d0a 5468 6520  ed  ........The 
+00000860: 5069 7065 2063 616e 2072 6561 6420 6120  Pipe can read a 
+00000870: 7769 6465 2061 7272 6179 206f 6620 6669  wide array of fi
+00000880: 6c65 2074 7970 6573 2c20 616e 6420 7468  le types, and th
+00000890: 7573 2068 6173 206d 616e 7920 6465 7065  us has many depe
+000008a0: 6e64 656e 6369 6573 2074 6861 7420 6d75  ndencies that mu
+000008b0: 7374 2062 6520 696e 7374 616c 6c65 6420  st be installed 
+000008c0: 7365 7061 7261 7465 6c79 2e20 4974 2061  separately. It a
+000008d0: 6c73 6f20 7265 7175 6972 6573 2061 2073  lso requires a s
+000008e0: 7472 6f6e 6720 6d61 6368 696e 6520 666f  trong machine fo
+000008f0: 7220 676f 6f64 2072 6573 706f 6e73 6520  r good response 
+00000900: 7469 6d65 732e 2046 6f72 2074 6869 7320  times. For this 
+00000910: 7265 6173 6f6e 2c20 7765 2068 6f73 7420  reason, we host 
+00000920: 6974 2061 7320 616e 2041 5049 2074 6861  it as an API tha
+00000930: 7420 776f 726b 7320 6f75 742d 6f66 2d74  t works out-of-t
+00000940: 6865 2d62 6f78 2e20 0d0a 0d0a 4669 7273  he-box. ....Firs
+00000950: 742c 2069 6e73 7461 6c6c 2054 6865 2050  t, install The P
+00000960: 6970 652e 200d 0a60 6060 0d0a 7069 7020  ipe. ..```..pip 
+00000970: 696e 7374 616c 6c20 7468 6570 6970 655f  install thepipe_
+00000980: 6170 690d 0a60 6060 0d0a 0d0a 5468 6520  api..```....The 
+00000990: 5069 7065 2069 7320 6176 6169 6c61 626c  Pipe is availabl
+000009a0: 6520 6173 2061 2068 6f73 7465 6420 4150  e as a hosted AP
+000009b0: 492c 206f 7220 6974 2063 616e 2062 6520  I, or it can be 
+000009c0: 7365 7420 7570 206c 6f63 616c 6c79 2e20  set up locally. 
+000009d0: 416e 2041 5049 206b 6579 2069 7320 7265  An API key is re
+000009e0: 636f 6d6d 656e 6465 6420 666f 7220 6f75  commended for ou
+000009f0: 742d 6f66 2d74 6865 2d62 6f78 2066 756e  t-of-the-box fun
+00000a00: 6374 696f 6e61 6c69 7479 2028 616c 7465  ctionality (alte
+00000a10: 726e 6174 6976 656c 792c 2073 6565 2074  rnatively, see t
+00000a20: 6865 206c 6f63 616c 2069 6e73 7461 6c6c  he local install
+00000a30: 6174 696f 6e20 7365 6374 696f 6e29 2e20  ation section). 
+00000a40: 456e 7375 7265 2074 6865 2060 5448 4550  Ensure the `THEP
+00000a50: 4950 455f 4150 495f 4b45 5960 2065 6e76  IPE_API_KEY` env
+00000a60: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
+00000a70: 6520 6973 2073 6574 2e20 446f 6e27 7420  e is set. Don't 
+00000a80: 6861 7665 2061 206b 6579 2079 6574 3f20  have a key yet? 
+00000a90: 5b47 6574 206f 6e65 2068 6572 655d 2868  [Get one here](h
+00000aa0: 7474 7073 3a2f 2f74 6865 7069 2e70 6529  ttps://thepi.pe)
+00000ab0: 2e0d 0a0d 0a4e 6f77 2079 6f75 2063 616e  .....Now you can
+00000ac0: 2065 7874 7261 6374 2063 6f6d 7072 6568   extract compreh
+00000ad0: 656e 7369 7665 2074 6578 7420 616e 6420  ensive text and 
+00000ae0: 7669 7375 616c 7320 6672 6f6d 2061 6e79  visuals from any
+00000af0: 2066 696c 653a 0d0a 6060 6070 7974 686f   file:..```pytho
+00000b00: 6e0d 0a66 726f 6d20 7468 6570 6970 655f  n..from thepipe_
+00000b10: 6170 6920 696d 706f 7274 2074 6865 7069  api import thepi
+00000b20: 7065 0d0a 6d65 7373 6167 6573 203d 2074  pe..messages = t
+00000b30: 6865 7069 7065 2e65 7874 7261 6374 2822  hepipe.extract("
+00000b40: 6578 616d 706c 652e 7064 6622 290d 0a60  example.pdf")..`
+00000b50: 6060 0d0a 4f72 2077 6562 7369 7465 733a  ``..Or websites:
+00000b60: 0d0a 6060 6070 7974 686f 6e0d 0a6d 6573  ..```python..mes
+00000b70: 7361 6765 7320 3d20 7468 6570 6970 652e  sages = thepipe.
+00000b80: 6578 7472 6163 7428 2268 7474 7073 3a2f  extract("https:/
+00000b90: 2f65 7861 6d70 6c65 2e63 6f6d 2229 0d0a  /example.com")..
+00000ba0: 6060 600d 0a54 6865 6e20 6665 6564 2069  ```..Then feed i
+00000bb0: 7420 696e 746f 2047 5054 2d34 5620 6c69  t into GPT-4V li
+00000bc0: 6b65 2073 6f3a 0d0a 6060 6070 7974 686f  ke so:..```pytho
+00000bd0: 6e0d 0a72 6573 706f 6e73 6520 3d20 6f70  n..response = op
+00000be0: 656e 6169 2e63 6861 742e 636f 6d70 6c65  enai.chat.comple
+00000bf0: 7469 6f6e 732e 6372 6561 7465 280d 0a20  tions.create(.. 
+00000c00: 2020 206d 6f64 656c 3d22 6770 742d 342d     model="gpt-4-
+00000c10: 7475 7262 6f22 2c0d 0a20 2020 206d 6573  turbo",..    mes
+00000c20: 7361 6765 7320 3d20 6d65 7373 6167 6573  sages = messages
+00000c30: 2c0d 0a29 0d0a 6060 600d 0a0d 0a21 5b4a  ,..)..```....![J
+00000c40: 7573 7420 6361 6c6c 204f 7065 6e41 495d  ust call OpenAI]
+00000c50: 2868 7474 7073 3a2f 2f72 706e 7574 7a65  (https://rpnutze
+00000c60: 6d75 7462 7275 6d63 7a77 7675 652e 7375  mutbrumczwvue.su
+00000c70: 7061 6261 7365 2e63 6f2f 7374 6f72 6167  pabase.co/storag
+00000c80: 652f 7631 2f6f 626a 6563 742f 7075 626c  e/v1/object/publ
+00000c90: 6963 2f61 7373 6574 732f 494d 475f 3031  ic/assets/IMG_01
+00000ca0: 3830 2e6a 7067 290d 0a0d 0a59 6f75 2063  80.jpg)....You c
+00000cb0: 616e 2061 6c73 6f20 7573 6520 5468 6520  an also use The 
+00000cc0: 5069 7065 2066 726f 6d20 7468 6520 636f  Pipe from the co
+00000cd0: 6d6d 616e 6420 6c69 6e65 2e20 4865 7265  mmand line. Here
+00000ce0: 2773 2068 6f77 2074 6f20 7265 6375 7273  's how to recurs
+00000cf0: 6976 656c 7920 6578 7472 6163 7420 6672  ively extract fr
+00000d00: 6f6d 2061 2064 6972 6563 746f 7279 2c20  om a directory, 
+00000d10: 6d61 7463 6869 6e67 206f 6e6c 7920 6669  matching only fi
+00000d20: 6c65 7320 636f 6e74 6169 6e69 6e67 2061  les containing a
+00000d30: 2073 7562 7374 7269 6e67 2028 696e 2074   substring (in t
+00000d40: 6869 7320 6578 616d 706c 652c 2074 7970  his example, typ
+00000d50: 6573 6372 6970 7420 6669 6c65 7329 2061  escript files) a
+00000d60: 6e64 2069 676e 6f72 6520 6669 6c65 7320  nd ignore files 
+00000d70: 636f 6e74 6169 6e69 6e67 206f 7468 6572  containing other
+00000d80: 2073 7562 7374 7269 6e67 7320 2869 6e20   substrings (in 
+00000d90: 7468 6973 2065 7861 6d70 6c65 2c20 616e  this example, an
+00000da0: 7974 6869 6e67 2069 6e20 7468 6520 2274  ything in the "t
+00000db0: 6573 7473 2220 666f 6c64 6572 293a 0d0a  ests" folder):..
+00000dc0: 6060 6062 6173 680d 0a74 6865 7069 7065  ```bash..thepipe
+00000dd0: 2070 6174 682f 746f 2f66 6f6c 6465 7220   path/to/folder 
+00000de0: 2d2d 6d61 7463 6820 7473 7820 2d2d 6967  --match tsx --ig
+00000df0: 6e6f 7265 2074 6573 7473 0d0a 6060 600d  nore tests..```.
+00000e00: 0a0d 0a0d 0a23 2320 5375 7070 6f72 7465  .....## Supporte
+00000e10: 6420 4669 6c65 2054 7970 6573 20f0 9f93  d File Types ...
+00000e20: 9a0d 0a0d 0a7c 2053 6f75 7263 6520 5479  .....| Source Ty
+00000e30: 7065 2020 2020 2020 2020 2020 2020 2020  pe              
+00000e40: 2020 2020 2020 2020 2020 2020 207c 2049               | I
+00000e50: 6e70 7574 2074 7970 6573 2020 2020 2020  nput types      
+00000e60: 2020 7c20 546f 6b65 6e20 436f 6d70 7265    | Token Compre
+00000e70: 7373 696f 6e20 f09f 979c efb8 8f20 7c20  ssion ....... | 
+00000e80: 496d 6167 6520 4578 7472 6163 7469 6f6e  Image Extraction
+00000e90: 20f0 9f91 81ef b88f 207c 204e 6f74 6573   ....... | Notes
+00000ea0: 20f0 9f93 8c20 2020 2020 2020 2020 2020   ....           
+00000eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ed0: 2020 2020 2020 207c 0d0a 7c2d 2d2d 2d2d         |..|-----
+00000ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ef0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000f00: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --|-------------
+00000f10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  -------------|--
+00000f30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000f40: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|--------------
+00000f50: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----|-----------
+00000f60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000f70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000f80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0d  --------------|.
+00000f90: 0a7c 2044 6972 6563 746f 7279 2020 2020  .| Directory    
+00000fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fb0: 2020 2020 2020 2020 207c 2041 6e79 2060           | Any `
+00000fc0: 2f70 6174 682f 746f 2f64 6972 6563 746f  /path/to/directo
+00000fd0: 7279 6020 2020 2020 2020 2020 2020 2020  ry`             
+00000fe0: 2020 2020 7c20 e29c 94ef b88f 2020 2020      | ......    
+00000ff0: 2020 2020 2020 2020 2020 207c 20e2 9c94             | ...
+00001000: efb8 8f20 2020 2020 2020 2020 2020 2020  ...             
+00001010: 2020 7c20 4578 7472 6163 7473 2066 726f    | Extracts fro
+00001020: 6d20 616c 6c20 6669 6c65 7320 696e 2064  m all files in d
+00001030: 6972 6563 746f 7279 2c20 7375 7070 6f72  irectory, suppor
+00001040: 7473 206d 6174 6368 2061 6e64 2069 676e  ts match and ign
+00001050: 6f72 6520 7061 7474 6572 6e73 207c 0d0a  ore patterns |..
+00001060: 7c20 436f 6465 2020 2020 2020 2020 2020  | Code          
+00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001080: 2020 2020 2020 2020 7c20 602e 7079 602c          | `.py`,
+00001090: 2060 2e74 7378 602c 2060 2e6a 7360 2c20   `.tsx`, `.js`, 
+000010a0: 602e 6874 6d6c 602c 2060 2e63 7373 602c  `.html`, `.css`,
+000010b0: 2060 2e63 7070 602c 2065 7463 207c 20e2   `.cpp`, etc | .
+000010c0: 9c94 efb8 8f20 2876 6172 6965 7329 2020  ..... (varies)  
+000010d0: 207c 20e2 9d8c 2020 2020 2020 2020 2020   | ...          
+000010e0: 2020 2020 207c 2043 6f6d 6269 6e65 7320       | Combines 
+000010f0: 616c 6c20 636f 6465 2066 696c 6573 2e20  all code files. 
+00001100: 602e 6360 2c20 602e 6370 7060 2c20 602e  `.c`, `.cpp`, `.
+00001110: 7079 6020 6172 6520 636f 6d70 7265 7373  py` are compress
+00001120: 6962 6c65 2077 6974 6820 6374 6167 732c  ible with ctags,
+00001130: 206f 7468 6572 7320 6172 6520 6e6f 7420   others are not 
+00001140: 7c0d 0a7c 2050 6c61 696e 7465 7874 2020  |..| Plaintext  
 00001150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001160: 2020 2020 2020 2020 2020 7c20 496e 7075            | Inpu
-00001170: 7420 7479 7065 7320 2020 2020 2020 207c  t types        |
-00001180: 2054 6f6b 656e 2043 6f6d 7072 6573 7369   Token Compressi
-00001190: 6f6e 20f0 9f97 9cef b88f 207c 2049 6d61  on ....... | Ima
-000011a0: 6765 2045 7874 7261 6374 696f 6e20 f09f  ge Extraction ..
-000011b0: 9181 efb8 8f20 7c20 4e6f 7465 7320 f09f  ..... | Notes ..
-000011c0: 938c 2020 2020 2020 2020 2020 2020 2020  ..              
-000011d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001160: 2020 2020 2020 2020 2020 207c 2060 2e74             | `.t
+00001170: 7874 602c 2060 2e6d 6460 2c20 602e 7274  xt`, `.md`, `.rt
+00001180: 6660 2c20 6574 6320 2020 2020 2020 2020  f`, etc         
+00001190: 2020 2020 2020 7c20 e29c 94ef b88f 2020        | ......  
+000011a0: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
+000011b0: 9d8c 2020 2020 2020 2020 2020 2020 2020  ..              
+000011c0: 207c 2052 6567 756c 6172 2074 6578 7420   | Regular text 
+000011d0: 6669 6c65 7320 2020 2020 2020 2020 2020  files           
 000011e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011f0: 2020 2020 7c0d 0a7c 2d2d 2d2d 2d2d 2d2d      |..|--------
-00001200: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001210: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
-00001220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001240: 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  ----------|-----
-00001250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d  --------------|-
-00001260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001270: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|--------------
-00001280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000012a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0d0a 7c20  -----------|..| 
-000012b0: 4469 7265 6374 6f72 7920 2020 2020 2020  Directory       
-000012c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012d0: 2020 2020 2020 7c20 416e 7920 602f 7061        | Any `/pa
-000012e0: 7468 2f74 6f2f 6469 7265 6374 6f72 7960  th/to/directory`
-000012f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001300: 207c 20e2 9c94 efb8 8f20 2020 2020 2020   | ......       
-00001310: 2020 2020 2020 2020 7c20 e29c 94ef b88f          | ......
-00001320: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00001330: 2045 7874 7261 6374 7320 6672 6f6d 2061   Extracts from a
-00001340: 6c6c 2066 696c 6573 2069 6e20 6469 7265  ll files in dire
-00001350: 6374 6f72 792c 2073 7570 706f 7274 7320  ctory, supports 
-00001360: 6d61 7463 6820 616e 6420 6967 6e6f 7265  match and ignore
-00001370: 2070 6174 7465 726e 7320 7c0d 0a7c 2043   patterns |..| C
-00001380: 6f64 6520 2020 2020 2020 2020 2020 2020  ode             
-00001390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013a0: 2020 2020 207c 2060 2e70 7960 2c20 602e       | `.py`, `.
-000013b0: 7473 7860 2c20 602e 6a73 602c 2060 2e68  tsx`, `.js`, `.h
-000013c0: 746d 6c60 2c20 602e 6373 7360 2c20 602e  tml`, `.css`, `.
-000013d0: 6370 7060 2c20 6574 6320 7c20 e29c 94ef  cpp`, etc | ....
-000013e0: b88f 2028 7661 7269 6573 2920 2020 7c20  .. (varies)   | 
-000013f0: e29d 8c20 2020 2020 2020 2020 2020 2020  ...             
-00001400: 2020 7c20 436f 6d62 696e 6573 2061 6c6c    | Combines all
-00001410: 2063 6f64 6520 6669 6c65 732e 2060 2e63   code files. `.c
-00001420: 602c 2060 2e63 7070 602c 2060 2e70 7960  `, `.cpp`, `.py`
-00001430: 2061 7265 2063 6f6d 7072 6573 7369 626c   are compressibl
-00001440: 6520 7769 7468 2063 7461 6773 2c20 6f74  e with ctags, ot
-00001450: 6865 7273 2061 7265 206e 6f74 207c 0d0a  hers are not |..
-00001460: 7c20 506c 6169 6e74 6578 7420 2020 2020  | Plaintext     
-00001470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001480: 2020 2020 2020 2020 7c20 602e 7478 7460          | `.txt`
-00001490: 2c20 602e 6d64 602c 2060 2e72 7466 602c  , `.md`, `.rtf`,
-000014a0: 2065 7463 2020 2020 2020 2020 2020 2020   etc            
-000014b0: 2020 207c 20e2 9c94 efb8 8f20 2020 2020     | ......     
-000014c0: 2020 2020 2020 2020 2020 7c20 e29d 8c20            | ... 
-000014d0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000014e0: 5265 6775 6c61 7220 7465 7874 2066 696c  Regular text fil
-000014f0: 6573 2020 2020 2020 2020 2020 2020 2020  es              
-00001500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001520: 2020 2020 2020 2020 7c0d 0a7c 2050 4446          |..| PDF
+000011f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001200: 2020 2020 2020 2020 2020 207c 0d0a 7c20             |..| 
+00001210: 5044 4620 2020 2020 2020 2020 2020 2020  PDF             
+00001220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001230: 2020 2020 2020 7c20 602e 7064 6660 2020        | `.pdf`  
+00001240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001260: 7c20 e29c 94ef b88f 2020 2020 2020 2020  | ......        
+00001270: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
+00001280: 2020 207c 2045 7874 7261 6374 7320 7465     | Extracts te
+00001290: 7874 2061 6e64 2069 6d61 6765 7320 6f66  xt and images of
+000012a0: 2065 6163 6820 7061 6765 3b20 6361 6e20   each page; can 
+000012b0: 7573 6520 4149 2066 6f72 2065 7874 7261  use AI for extra
+000012c0: 6374 696f 6e20 6f66 2074 6162 6c65 2064  ction of table d
+000012d0: 6174 6120 616e 6420 2069 6d61 6765 7320  ata and  images 
+000012e0: 7769 7468 696e 2070 6167 6573 207c 0d0a  within pages |..
+000012f0: 7c20 496d 6167 6520 2020 2020 2020 2020  | Image         
+00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001310: 2020 2020 2020 2020 7c20 602e 6a70 6760          | `.jpg`
+00001320: 2c20 602e 6a70 6567 602c 2060 2e70 6e67  , `.jpeg`, `.png
+00001330: 6020 7c20 e29d 8c20 2020 2020 2020 2020  ` | ...         
+00001340: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
+00001350: 2020 2020 2020 2020 2020 2020 207c 2045               | E
+00001360: 7874 7261 6374 7320 696d 6167 6573 2c20  xtracts images, 
+00001370: 7573 6573 204f 4352 2069 6620 7465 7874  uses OCR if text
+00001380: 5f6f 6e6c 7920 2020 2020 2020 2020 2020  _only           
+00001390: 2020 2020 2020 2020 2020 2020 207c 0d0a               |..
+000013a0: 7c20 5370 7265 6164 7368 6565 7420 2020  | Spreadsheet   
+000013b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013c0: 2020 2020 2020 2020 7c20 602e 6373 7660          | `.csv`
+000013d0: 2c20 602e 786c 7360 2c20 602e 786c 7378  , `.xls`, `.xlsx
+000013e0: 6020 2020 2020 2020 2020 2020 2020 7c20  `             | 
+000013f0: e29c 94ef b88f 2020 2020 2020 2020 2020  ......          
+00001400: 2020 2020 2020 7c20 e29d 8c20 2020 2020        | ...     
+00001410: 2020 2020 2020 2020 2020 7c20 4578 7472            | Extr
+00001420: 6163 7473 2064 6174 6120 6672 6f6d 2073  acts data from s
+00001430: 7072 6561 6473 6865 6574 733b 2063 6f6e  preadsheets; con
+00001440: 7665 7274 7320 6561 6368 2072 6f77 2069  verts each row i
+00001450: 6e74 6f20 6120 4a53 4f4e 2066 6f72 6d61  nto a JSON forma
+00001460: 7474 6564 2073 7472 696e 6720 2020 2020  tted string     
+00001470: 2020 2020 7c0d 0a7c 204a 7570 7974 6572      |..| Jupyter
+00001480: 204e 6f74 6562 6f6f 6b20 2020 2020 2020   Notebook       
+00001490: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000014a0: 2060 2e69 7079 6e62 6020 2020 2020 2020   `.ipynb`       
+000014b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014c0: 2020 2020 2020 2020 207c 20e2 9d8c 2020           | ...  
+000014d0: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
+000014e0: 9c94 efb8 8f20 2020 2020 2020 2020 2020  .....           
+000014f0: 2020 2020 7c20 4578 7472 6163 7473 2063      | Extracts c
+00001500: 6f64 652c 206d 6172 6b64 6f77 6e2c 2061  ode, markdown, a
+00001510: 6e64 2069 6d61 6765 7320 6672 6f6d 204a  nd images from J
+00001520: 7570 7974 6572 206e 6f74 6562 6f6f 6b73  upyter notebooks
 00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001550: 2020 207c 2060 2e70 6466 6020 2020 2020     | `.pdf`     
-00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001570: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
-00001580: 9c94 efb8 8f20 2020 2020 2020 2020 2020  .....           
-00001590: 2020 2020 7c20 e29c 94ef b88f 2020 2020      | ......    
-000015a0: 7c20 4578 7472 6163 7473 2074 6578 7420  | Extracts text 
-000015b0: 616e 6420 696d 6167 6573 206f 6620 6561  and images of ea
-000015c0: 6368 2070 6167 653b 2063 616e 2075 7365  ch page; can use
-000015d0: 2041 4920 666f 7220 6578 7472 6163 7469   AI for extracti
-000015e0: 6f6e 206f 6620 7461 626c 6520 6461 7461  on of table data
-000015f0: 2061 6e64 2020 696d 6167 6573 2077 6974   and  images wit
-00001600: 6869 6e20 7061 6765 7320 7c0d 0a7c 2049  hin pages |..| I
-00001610: 6d61 6765 2020 2020 2020 2020 2020 2020  mage            
-00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001630: 2020 2020 207c 2060 2e6a 7067 602c 2060       | `.jpg`, `
-00001640: 2e6a 7065 6760 2c20 602e 706e 6760 207c  .jpeg`, `.png` |
-00001650: 20e2 9d8c 2020 2020 2020 2020 2020 2020   ...            
-00001660: 2020 2020 7c20 e29c 94ef b88f 2020 2020      | ......    
-00001670: 2020 2020 2020 2020 2020 7c20 4578 7472            | Extr
-00001680: 6163 7473 2069 6d61 6765 732c 2075 7365  acts images, use
-00001690: 7320 4f43 5220 6966 2074 6578 745f 6f6e  s OCR if text_on
-000016a0: 6c79 2020 2020 2020 2020 2020 2020 2020  ly              
-000016b0: 2020 2020 2020 2020 2020 7c0d 0a7c 2044            |..| D
-000016c0: 6174 6120 5461 626c 6520 2020 2020 2020  ata Table       
-000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016e0: 2020 2020 7c20 602e 6373 7660 2c20 602e      | `.csv`, `.
-000016f0: 786c 7360 2c20 602e 786c 7378 6020 2020  xls`, `.xlsx`   
-00001700: 2020 2020 2020 2020 2020 7c20 e29c 94ef            | ....
-00001710: b88f 2020 2020 2020 2020 2020 2020 2020  ..              
-00001720: 2020 7c20 e29d 8c20 2020 2020 2020 2020    | ...         
-00001730: 2020 2020 2020 7c20 4578 7472 6163 7473        | Extracts
-00001740: 2064 6174 6120 6672 6f6d 2073 7072 6561   data from sprea
-00001750: 6473 6865 6574 733b 2063 6f6e 7665 7274  dsheets; convert
-00001760: 7320 746f 2074 6578 7420 7265 7072 6573  s to text repres
-00001770: 656e 7461 7469 6f6e 2e20 466f 7220 7665  entation. For ve
-00001780: 7279 206c 6172 6765 2064 6174 6173 6574  ry large dataset
-00001790: 732c 2077 696c 6c20 6f6e 6c79 2065 7874  s, will only ext
-000017a0: 7261 6374 2063 6f6c 756d 6e20 6e61 6d65  ract column name
-000017b0: 7320 616e 6420 7479 7065 7320 2020 2020  s and types     
-000017c0: 2020 2020 7c0d 0a7c 204a 7570 7974 6572      |..| Jupyter
-000017d0: 204e 6f74 6562 6f6f 6b20 2020 2020 2020   Notebook       
+00001550: 2020 7c0d 0a7c 204d 6963 726f 736f 6674    |..| Microsoft
+00001560: 2057 6f72 6420 446f 6375 6d65 6e74 2020   Word Document  
+00001570: 2020 2020 2020 2020 2020 2020 207c 2060               | `
+00001580: 2e64 6f63 7860 2020 2020 2020 2020 2020  .docx`          
+00001590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015a0: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
+000015b0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+000015c0: e29c 94ef b88f 2020 2020 2020 2020 2020  ......          
+000015d0: 2020 2020 207c 2045 7874 7261 6374 7320       | Extracts 
+000015e0: 7465 7874 2061 6e64 2069 6d61 6765 7320  text and images 
+000015f0: 6672 6f6d 2057 6f72 6420 646f 6375 6d65  from Word docume
+00001600: 6e74 7320 2020 2020 2020 2020 2020 2020  nts             
+00001610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001620: 2020 2020 2020 2020 2020 207c 0d0a 7c20             |..| 
+00001630: 4d69 6372 6f73 6f66 7420 506f 7765 7250  Microsoft PowerP
+00001640: 6f69 6e74 2050 7265 7365 6e74 6174 696f  oint Presentatio
+00001650: 6e20 2020 2020 7c20 602e 7070 7478 6020  n     | `.pptx` 
+00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001680: 7c20 e29c 94ef b88f 2020 2020 2020 2020  | ......        
+00001690: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
+000016a0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+000016b0: 4578 7472 6163 7473 2074 6578 7420 616e  Extracts text an
+000016c0: 6420 696d 6167 6573 2066 726f 6d20 506f  d images from Po
+000016d0: 7765 7250 6f69 6e74 2070 7265 7365 6e74  werPoint present
+000016e0: 6174 696f 6e73 2020 2020 2020 2020 2020  ations          
+000016f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001700: 2020 2020 7c0d 0a7c 2056 6964 656f 2020      |..| Video  
+00001710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001720: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00001730: 2060 2e6d 7034 602c 2060 2e6d 6f76 602c   `.mp4`, `.mov`,
+00001740: 2060 2e77 6d76 6020 2020 2020 7c20 e29c   `.wmv`     | ..
+00001750: 94ef b88f 2020 2020 2020 2020 2020 2020  ....            
+00001760: 2020 207c 20e2 9c94 efb8 8f20 2020 2020     | ......     
+00001770: 2020 2020 2020 2020 2020 207c 2045 7874             | Ext
+00001780: 7261 6374 7320 6672 616d 6573 2061 6e64  racts frames and
+00001790: 2061 7564 696f 2074 7261 6e73 6372 6970   audio transcrip
+000017a0: 7420 6672 6f6d 2076 6964 656f 7320 696e  t from videos in
+000017b0: 2070 6572 2d6d 696e 7574 6520 6368 756e   per-minute chun
+000017c0: 6b73 2e20 7c0d 0a7c 2041 7564 696f 2020  ks. |..| Audio  
+000017d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000017e0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000017f0: 2060 2e69 7079 6e62 6020 2020 2020 2020   `.ipynb`       
-00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001810: 2020 2020 2020 2020 207c 20e2 9d8c 2020           | ...  
-00001820: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
-00001830: 9c94 efb8 8f20 2020 2020 2020 2020 2020  .....           
-00001840: 2020 2020 7c20 4578 7472 6163 7473 2063      | Extracts c
-00001850: 6f64 652c 206d 6172 6b64 6f77 6e2c 2061  ode, markdown, a
-00001860: 6e64 2069 6d61 6765 7320 6672 6f6d 204a  nd images from J
-00001870: 7570 7974 6572 206e 6f74 6562 6f6f 6b73  upyter notebooks
-00001880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017f0: 2060 2e6d 7033 602c 2060 2e77 6176 6020   `.mp3`, `.wav` 
+00001800: 2020 2020 2020 2020 207c 20e2 9c94 efb8           | .....
+00001810: 8f20 2020 2020 2020 2020 2020 2020 2020  .               
+00001820: 7c20 e29d 8c20 2020 2020 2020 2020 2020  | ...           
+00001830: 2020 2020 207c 2045 7874 7261 6374 7320       | Extracts 
+00001840: 7465 7874 2066 726f 6d20 6175 6469 6f20  text from audio 
+00001850: 6669 6c65 733b 2073 7570 706f 7274 7320  files; supports 
+00001860: 7370 6565 6368 2d74 6f2d 7465 7874 2063  speech-to-text c
+00001870: 6f6e 7665 7273 696f 6e20 2020 2020 2020  onversion       
+00001880: 207c 200d 0a7c 2057 6562 7369 7465 2020   | ..| Website  
 00001890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018a0: 2020 7c0d 0a7c 204d 6963 726f 736f 6674    |..| Microsoft
-000018b0: 2057 6f72 6420 446f 6375 6d65 6e74 2020   Word Document  
-000018c0: 2020 2020 2020 2020 2020 2020 207c 2060               | `
-000018d0: 2e64 6f63 7860 2020 2020 2020 2020 2020  .docx`          
-000018e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018f0: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
-00001900: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00001910: e29c 94ef b88f 2020 2020 2020 2020 2020  ......          
-00001920: 2020 2020 207c 2045 7874 7261 6374 7320       | Extracts 
-00001930: 7465 7874 2061 6e64 2069 6d61 6765 7320  text and images 
-00001940: 6672 6f6d 2057 6f72 6420 646f 6375 6d65  from Word docume
-00001950: 6e74 7320 2020 2020 2020 2020 2020 2020  nts             
-00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001970: 2020 2020 2020 2020 2020 207c 0d0a 7c20             |..| 
-00001980: 4d69 6372 6f73 6f66 7420 506f 7765 7250  Microsoft PowerP
-00001990: 6f69 6e74 2050 7265 7365 6e74 6174 696f  oint Presentatio
-000019a0: 6e20 2020 2020 7c20 602e 7070 7478 6020  n     | `.pptx` 
-000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019d0: 7c20 e29c 94ef b88f 2020 2020 2020 2020  | ......        
-000019e0: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
-000019f0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00001a00: 4578 7472 6163 7473 2074 6578 7420 616e  Extracts text an
-00001a10: 6420 696d 6167 6573 2066 726f 6d20 506f  d images from Po
-00001a20: 7765 7250 6f69 6e74 2070 7265 7365 6e74  werPoint present
-00001a30: 6174 696f 6e73 2020 2020 2020 2020 2020  ations          
-00001a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a50: 2020 2020 7c0d 0a7c 2056 6964 656f 2020      |..| Video  
-00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a70: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00001a80: 2060 2e6d 7034 602c 2060 2e61 7669 602c   `.mp4`, `.avi`,
-00001a90: 2060 2e6d 6f76 602c 2060 2e77 6d76 6020   `.mov`, `.wmv` 
-00001aa0: 2020 2020 7c20 e29c 94ef b88f 2020 2020      | ......    
-00001ab0: 2020 2020 2020 2020 2020 207c 20e2 9c94             | ...
-00001ac0: efb8 8f20 2020 2020 2020 2020 2020 2020  ...             
-00001ad0: 2020 207c 2045 7874 7261 6374 7320 6672     | Extracts fr
-00001ae0: 616d 6573 2066 726f 6d20 7669 6465 6f20  ames from video 
-00001af0: 6669 6c65 733b 2073 7570 706f 7274 7320  files; supports 
-00001b00: 6672 616d 6520 6578 7472 6163 7469 6f6e  frame extraction
-00001b10: 2061 6e64 204f 4352 2066 6f72 2074 6578   and OCR for tex
-00001b20: 7420 6578 7472 6163 7469 6f6e 2066 726f  t extraction fro
-00001b30: 6d20 6672 616d 6573 207c 0d0a 7c20 4175  m frames |..| Au
-00001b40: 6469 6f20 2020 2020 2020 2020 2020 2020  dio             
-00001b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b60: 2020 2020 7c20 602e 6d70 3360 2c20 602e      | `.mp3`, `.
-00001b70: 7761 7660 2020 2020 2020 2020 2020 7c20  wav`          | 
-00001b80: e29c 94ef b88f 2020 2020 2020 2020 2020  ......          
-00001b90: 2020 2020 207c 20e2 9d8c 2020 2020 2020       | ...      
-00001ba0: 2020 2020 2020 2020 2020 7c20 4578 7472            | Extr
-00001bb0: 6163 7473 2074 6578 7420 6672 6f6d 2061  acts text from a
-00001bc0: 7564 696f 2066 696c 6573 3b20 7375 7070  udio files; supp
-00001bd0: 6f72 7473 2073 7065 6563 682d 746f 2d74  orts speech-to-t
-00001be0: 6578 7420 636f 6e76 6572 7369 6f6e 2020  ext conversion  
-00001bf0: 2020 2020 2020 7c20 0d0a 7c20 5765 6273        | ..| Webs
-00001c00: 6974 6520 2020 2020 2020 2020 2020 2020  ite             
-00001c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c20: 2020 7c20 5552 4c73 2028 696e 7075 7473    | URLs (inputs
-00001c30: 2073 7461 7274 696e 6720 7769 7468 2060   starting with `
-00001c40: 6874 7470 602c 2060 6874 7470 7360 2c20  http`, `https`, 
-00001c50: 6066 7470 6029 2020 2020 2020 2020 2020  `ftp`)          
-00001c60: 2020 207c 20e2 9c94 efb8 8f20 2020 2020     | ......     
-00001c70: 2020 2020 2020 2020 2020 207c 20e2 9c94             | ...
-00001c80: efb8 8f20 2020 207c 2045 7874 7261 6374  ...    | Extract
-00001c90: 7320 7465 7874 2066 726f 6d20 7765 6220  s text from web 
-00001ca0: 7061 6765 2061 6c6f 6e67 2077 6974 6820  page along with 
-00001cb0: 696d 6167 6520 286f 7220 696d 6167 6573  image (or images
-00001cc0: 2069 6620 7363 726f 6c6c 6162 6c65 293b   if scrollable);
-00001cd0: 2074 6578 742d 6f6e 6c79 2065 7874 7261   text-only extra
-00001ce0: 6374 696f 6e20 6176 6169 6c61 626c 6520  ction available 
-00001cf0: 2020 2020 2020 2020 207c 0d0a 7c20 4769           |..| Gi
-00001d00: 7448 7562 2052 6570 6f73 6974 6f72 7920  tHub Repository 
-00001d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d20: 2020 2020 7c20 4769 7448 7562 2072 6570      | GitHub rep
-00001d30: 6f20 5552 4c73 2028 696e 7075 7473 2073  o URLs (inputs s
-00001d40: 7461 7274 696e 6720 7769 7468 2060 6874  tarting with `ht
-00001d50: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001d60: 6020 6f72 2060 6874 7470 733a 2f2f 7777  ` or `https://ww
-00001d70: 772e 6769 7468 7562 2e63 6f6d 6029 2020  w.github.com`)  
-00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d90: 2020 2020 2020 2020 7c20 e29c 94ef b88f          | ......
-00001da0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00001db0: 20e2 9c94 efb8 8f20 2020 2020 2020 2020   ......         
-00001dc0: 2020 2020 2020 207c 2045 7874 7261 6374         | Extract
-00001dd0: 7320 6672 6f6d 2047 6974 4875 6220 7265  s from GitHub re
-00001de0: 706f 7369 746f 7269 6573 3b20 7375 7070  positories; supp
-00001df0: 6f72 7473 2062 7261 6e63 6820 7370 6563  orts branch spec
-00001e00: 6966 6963 6174 696f 6e20 2020 2020 2020  ification       
-00001e10: 2020 7c0d 0a7c 2059 6f75 5475 6265 2056    |..| YouTube V
-00001e20: 6964 656f 2020 2020 2020 2020 2020 2020  ideo            
-00001e30: 2020 2020 2020 2020 2020 2020 207c 2059               | Y
-00001e40: 6f75 5475 6265 2076 6964 656f 2055 524c  ouTube video URL
-00001e50: 7320 2869 6e70 7574 7320 7374 6172 7469  s (inputs starti
-00001e60: 6e67 2077 6974 6820 6068 7474 7073 3a2f  ng with `https:/
-00001e70: 2f79 6f75 7475 6265 2e63 6f6d 6020 6f72  /youtube.com` or
-00001e80: 2060 6874 7470 733a 2f2f 7777 772e 796f   `https://www.yo
-00001e90: 7574 7562 652e 636f 6d60 2920 2020 2020  utube.com`)     
-00001ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001eb0: 7c20 e29c 94ef b88f 2020 2020 2020 2020  | ......        
-00001ec0: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
-00001ed0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00001ee0: 2045 7874 7261 6374 7320 6672 616d 6573   Extracts frames
-00001ef0: 2061 6e64 2074 7261 6e73 6372 6970 7420   and transcript 
-00001f00: 6672 6f6d 2059 6f75 5475 6265 2076 6964  from YouTube vid
-00001f10: 656f 7320 696e 2070 6572 2d6d 696e 7574  eos in per-minut
-00001f20: 6520 6368 756e 6b73 2020 2020 2020 2020  e chunks        
-00001f30: 2020 7c0d 0a7c 205a 4950 2046 696c 6520    |..| ZIP File 
-00001f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f50: 2020 2020 2020 2020 2020 2020 207c 2060               | `
-00001f60: 2e7a 6970 6020 2020 2020 2020 2020 2020  .zip`           
-00001f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f80: 2020 2020 2020 207c 20e2 9c94 efb8 8f20         | ...... 
-00001f90: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00001fa0: e29c 94ef b88f 2020 2020 2020 2020 2020  ......          
-00001fb0: 2020 2020 2020 7c20 4578 7472 6163 7473        | Extracts
-00001fc0: 2063 6f6e 7465 6e74 7320 6f66 205a 4950   contents of ZIP
-00001fd0: 2066 696c 6573 3b20 7375 7070 6f72 7473   files; supports
-00001fe0: 206e 6573 7465 6420 6469 7265 6374 6f72   nested director
-00001ff0: 7920 6578 7472 6163 7469 6f6e 2020 2020  y extraction    
-00002000: 207c 0d0a 0d0a 2323 2048 6f77 2069 7420   |....## How it 
-00002010: 776f 726b 7320 f09f 9ba0 efb8 8f0d 0a0d  works ..........
-00002020: 0a54 6865 2069 6e70 7574 2073 6f75 7263  .The input sourc
-00002030: 6520 6973 2065 6974 6865 7220 6120 6669  e is either a fi
-00002040: 6c65 2070 6174 682c 2061 2055 524c 2c20  le path, a URL, 
-00002050: 6f72 2061 2064 6972 6563 746f 7279 2e20  or a directory. 
-00002060: 5468 6520 7069 7065 2077 696c 6c20 6578  The pipe will ex
-00002070: 7472 6163 7420 696e 666f 726d 6174 696f  tract informatio
-00002080: 6e20 6672 6f6d 2074 6865 2073 6f75 7263  n from the sourc
-00002090: 6520 616e 6420 7072 6f63 6573 7320 6974  e and process it
-000020a0: 2066 6f72 2064 6f77 6e73 7472 6561 6d20   for downstream 
-000020b0: 7573 6520 7769 7468 205b 6c61 6e67 7561  use with [langua
-000020c0: 6765 206d 6f64 656c 735d 2868 7474 7073  ge models](https
-000020d0: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
-000020e0: 6f72 672f 7769 6b69 2f4c 6172 6765 5f6c  org/wiki/Large_l
-000020f0: 616e 6775 6167 655f 6d6f 6465 6c29 2c20  anguage_model), 
-00002100: 5b76 6973 696f 6e20 7472 616e 7366 6f72  [vision transfor
-00002110: 6d65 7273 5d28 6874 7470 733a 2f2f 656e  mers](https://en
-00002120: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
-00002130: 696b 692f 5669 7369 6f6e 5f74 7261 6e73  iki/Vision_trans
-00002140: 666f 726d 6572 292c 206f 7220 5b76 6973  former), or [vis
-00002150: 696f 6e2d 6c61 6e67 7561 6765 206d 6f64  ion-language mod
-00002160: 656c 735d 2868 7474 7073 3a2f 2f61 7278  els](https://arx
-00002170: 6976 2e6f 7267 2f61 6273 2f32 3330 342e  iv.org/abs/2304.
-00002180: 3030 3638 3529 2e20 5468 6520 6f75 7470  00685). The outp
-00002190: 7574 2066 726f 6d20 7468 6520 7069 7065  ut from the pipe
-000021a0: 2069 7320 6120 7365 6e73 6962 6c65 206c   is a sensible l
-000021b0: 6973 7420 6f66 206d 756c 7469 6d6f 6461  ist of multimoda
-000021c0: 6c20 6d65 7373 6167 6573 2072 6570 7265  l messages repre
-000021d0: 7365 6e74 696e 6720 6368 756e 6b73 206f  senting chunks o
-000021e0: 6620 7468 6520 6578 7472 6163 7465 6420  f the extracted 
-000021f0: 696e 666f 726d 6174 696f 6e2c 2063 6172  information, car
-00002200: 6566 756c 6c79 2063 7261 6674 6564 2074  efully crafted t
-00002210: 6f20 6669 7420 7769 7468 696e 2063 6f6e  o fit within con
-00002220: 7465 7874 2077 696e 646f 7773 2066 6f72  text windows for
-00002230: 2061 6e79 206d 6f64 656c 7320 6672 6f6d   any models from
-00002240: 205b 6765 6d6d 612d 3762 5d28 6874 7470   [gemma-7b](http
-00002250: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
-00002260: 636f 2f67 6f6f 676c 652f 6765 6d6d 612d  co/google/gemma-
-00002270: 3762 2920 746f 205b 4750 542d 345d 2868  7b) to [GPT-4](h
-00002280: 7474 7073 3a2f 2f6f 7065 6e61 692e 636f  ttps://openai.co
-00002290: 6d2f 6770 742d 3429 2e20 5468 6520 6d65  m/gpt-4). The me
-000022a0: 7373 6167 6573 2072 6574 7572 6e65 6420  ssages returned 
-000022b0: 7368 6f75 6c64 206c 6f6f 6b20 6c69 6b65  should look like
-000022c0: 2074 6869 733a 0d0a 6060 606a 736f 6e0d   this:..```json.
-000022d0: 0a5b 0d0a 2020 7b0d 0a20 2020 2022 726f  .[..  {..    "ro
-000022e0: 6c65 223a 2022 7573 6572 222c 0d0a 2020  le": "user",..  
-000022f0: 2020 2263 6f6e 7465 6e74 223a 205b 0d0a    "content": [..
-00002300: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-00002310: 2022 7479 7065 223a 2022 7465 7874 222c   "type": "text",
-00002320: 0d0a 2020 2020 2020 2020 2274 6578 7422  ..        "text"
-00002330: 3a20 222e 2e2e 220d 0a20 2020 2020 207d  : "..."..      }
-00002340: 2c0d 0a20 2020 2020 207b 0d0a 2020 2020  ,..      {..    
-00002350: 2020 2020 2274 7970 6522 3a20 2269 6d61      "type": "ima
-00002360: 6765 5f75 726c 222c 0d0a 2020 2020 2020  ge_url",..      
-00002370: 2020 2269 6d61 6765 5f75 726c 223a 207b    "image_url": {
-00002380: 0d0a 2020 2020 2020 2020 2020 2275 726c  ..          "url
-00002390: 223a 2022 6461 7461 3a69 6d61 6765 2f6a  ": "data:image/j
-000023a0: 7065 673b 6261 7365 3634 2c2e 2e2e 220d  peg;base64,...".
-000023b0: 0a20 2020 2020 2020 207d 0d0a 2020 2020  .        }..    
-000023c0: 2020 7d0d 0a20 2020 205d 0d0a 2020 7d0d    }..    ]..  }.
-000023d0: 0a5d 0d0a 6060 600d 0a49 6620 796f 7520  .]..```..If you 
-000023e0: 7761 6e74 2074 6f20 6665 6564 2074 6865  want to feed the
-000023f0: 7365 206d 6573 7361 6765 7320 6469 7265  se messages dire
-00002400: 6374 6c79 2069 6e74 6f20 7468 6520 6d6f  ctly into the mo
-00002410: 6465 6c2c 2069 7420 6973 2069 6d70 6f72  del, it is impor
-00002420: 7461 6e74 2074 6f20 6265 206d 696e 6466  tant to be mindf
-00002430: 756c 206f 6620 7468 6520 746f 6b65 6e20  ul of the token 
-00002440: 6c69 6d69 742e 0d0a 4f70 656e 4149 2064  limit...OpenAI d
-00002450: 6f65 7320 6e6f 7420 616c 6c6f 7720 746f  oes not allow to
-00002460: 6f20 6d61 6e79 2069 6d61 6765 7320 696e  o many images in
-00002470: 2074 6865 2070 726f 6d70 7420 2873 6565   the prompt (see
-00002480: 2064 6973 6375 7373 696f 6e20 5b68 6572   discussion [her
-00002490: 655d 2868 7474 7073 3a2f 2f63 6f6d 6d75  e](https://commu
-000024a0: 6e69 7479 2e6f 7065 6e61 692e 636f 6d2f  nity.openai.com/
-000024b0: 742f 6770 742d 342d 7669 7369 6f6e 2d6d  t/gpt-4-vision-m
-000024c0: 6178 696d 756d 2d61 6d6f 756e 742d 6f66  aximum-amount-of
-000024d0: 2d69 6d61 6765 732f 3537 3331 3130 2f36  -images/573110/6
-000024e0: 2929 2c20 736f 206c 6f6e 6720 6669 6c65  )), so long file
-000024f0: 7320 7368 6f75 6c64 2062 6520 6578 7472  s should be extr
-00002500: 6163 7465 6420 7769 7468 2060 7465 7874  acted with `text
-00002510: 5f6f 6e6c 793d 5472 7565 6020 746f 2061  _only=True` to a
-00002520: 766f 6964 2074 6869 7320 6973 7375 652c  void this issue,
-00002530: 2077 6869 6c65 206c 6f6e 6720 7465 7874   while long text
-00002540: 2066 696c 6573 2073 686f 756c 6420 6569   files should ei
-00002550: 7468 6572 2062 6520 636f 6d70 7265 7373  ther be compress
-00002560: 6564 206f 7220 656d 6265 6464 6564 2069  ed or embedded i
-00002570: 6e20 6120 5241 4720 6672 616d 6577 6f72  n a RAG framewor
-00002580: 6b2e 0d0a 0d0a 5468 6520 7465 7874 2061  k.....The text a
-00002590: 6e64 2069 6d61 6765 7320 6672 6f6d 2074  nd images from t
-000025a0: 6865 7365 206d 6573 7361 6765 7320 6d61  hese messages ma
-000025b0: 7920 616c 736f 2062 6520 7072 6570 6172  y also be prepar
-000025c0: 6564 2066 6f72 2061 2076 6563 746f 7220  ed for a vector 
-000025d0: 6461 7461 6261 7365 2077 6974 6820 6074  database with `t
-000025e0: 6865 7069 7065 2e63 6f72 652e 6372 6561  hepipe.core.crea
-000025f0: 7465 5f63 6875 6e6b 735f 6672 6f6d 5f6d  te_chunks_from_m
-00002600: 6573 7361 6765 7360 206f 7220 666f 7220  essages` or for 
-00002610: 646f 776e 7374 7265 616d 2075 7365 2077  downstream use w
-00002620: 6974 6820 5241 4720 6672 616d 6577 6f72  ith RAG framewor
-00002630: 6b73 2e20 5b4c 6974 654c 4c4d 5d28 6874  ks. [LiteLLM](ht
-00002640: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00002650: 2f42 6572 7269 4149 2f6c 6974 656c 6c6d  /BerriAI/litellm
-00002660: 2920 6361 6e20 6265 2075 7365 6420 746f  ) can be used to
-00002670: 2065 6173 696c 7920 696e 7465 6772 6174   easily integrat
-00002680: 6520 5468 6520 5069 7065 2077 6974 6820  e The Pipe with 
-00002690: 616e 7920 4c4c 4d20 7072 6f76 6964 6572  any LLM provider
-000026a0: 2e20 0d0a 0d0a 4974 2075 7365 7320 6120  . ....It uses a 
-000026b0: 7661 7269 6574 7920 6f66 2068 6575 7269  variety of heuri
-000026c0: 7374 6963 7320 666f 7220 6f70 7469 6d61  stics for optima
-000026d0: 6c20 7065 7266 6f72 6d61 6e63 6520 7769  l performance wi
-000026e0: 7468 2076 6973 696f 6e2d 6c61 6e67 7561  th vision-langua
-000026f0: 6765 206d 6f64 656c 732c 2069 6e63 6c75  ge models, inclu
-00002700: 6469 6e67 2041 4920 6669 6c65 7479 7065  ding AI filetype
-00002710: 2064 6574 6563 7469 6f6e 2077 6974 6820   detection with 
-00002720: 5b66 696c 6574 7970 6520 6465 7465 6374  [filetype detect
-00002730: 696f 6e5d 2868 7474 7073 3a2f 2f6f 7065  ion](https://ope
-00002740: 6e73 6f75 7263 652e 676f 6f67 6c65 626c  nsource.googlebl
-00002750: 6f67 2e63 6f6d 2f32 3032 342f 3032 2f6d  og.com/2024/02/m
-00002760: 6167 696b 612d 6169 2d70 6f77 6572 6564  agika-ai-powered
-00002770: 2d66 6173 742d 616e 642d 6566 6669 6369  -fast-and-effici
-00002780: 656e 742d 6669 6c65 2d74 7970 652d 6964  ent-file-type-id
-00002790: 656e 7469 6669 6361 7469 6f6e 2e68 746d  entification.htm
-000027a0: 6c29 2c20 6f70 742d 696e 2041 4920 5b74  l), opt-in AI [t
-000027b0: 6162 6c65 2c20 6571 7561 7469 6f6e 2c20  able, equation, 
-000027c0: 616e 6420 6669 6775 7265 2065 7874 7261  and figure extra
-000027d0: 6374 696f 6e5d 2868 7474 7073 3a2f 2f74  ction](https://t
-000027e0: 6865 7069 2e70 652f 7072 6963 696e 6729  hepi.pe/pricing)
-000027f0: 2c20 6566 6669 6369 656e 7420 5b74 6f6b  , efficient [tok
-00002800: 656e 2063 6f6d 7072 6573 7369 6f6e 5d28  en compression](
-00002810: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-00002820: 672f 6162 732f 3234 3033 2e31 3239 3638  g/abs/2403.12968
-00002830: 292c 2061 7574 6f6d 6174 6963 205b 696d  ), automatic [im
-00002840: 6167 6520 656e 636f 6469 6e67 5d28 6874  age encoding](ht
-00002850: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
-00002860: 6961 2e6f 7267 2f77 696b 692f 4261 7365  ia.org/wiki/Base
-00002870: 3634 292c 205b 7265 7261 6e6b 696e 675d  64), [reranking]
-00002880: 2868 7474 7073 3a2f 2f61 7278 6976 2e6f  (https://arxiv.o
-00002890: 7267 2f61 6273 2f32 3331 302e 3036 3833  rg/abs/2310.0683
-000028a0: 3929 2066 6f72 205b 6c6f 7374 2d69 6e2d  9) for [lost-in-
-000028b0: 7468 652d 6d69 6464 6c65 5d28 6874 7470  the-middle](http
-000028c0: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
-000028d0: 732f 3233 3037 2e30 3331 3732 2920 6566  s/2307.03172) ef
-000028e0: 6665 6374 732c 2061 6e64 206d 6f72 652c  fects, and more,
-000028f0: 2061 6c6c 2070 7265 2d62 7569 6c74 2074   all pre-built t
-00002900: 6f20 776f 726b 206f 7574 2d6f 662d 7468  o work out-of-th
-00002910: 652d 626f 782e 0d0a 0d0a 215b 4465 6d6f  e-box.....![Demo
-00002920: 5d28 6874 7470 733a 2f2f 7270 6e75 747a  ](https://rpnutz
-00002930: 656d 7574 6272 756d 637a 7776 7565 2e73  emutbrumczwvue.s
-00002940: 7570 6162 6173 652e 636f 2f73 746f 7261  upabase.co/stora
-00002950: 6765 2f76 312f 6f62 6a65 6374 2f70 7562  ge/v1/object/pub
-00002960: 6c69 632f 6173 7365 7473 2f67 7261 6465  lic/assets/grade
-00002970: 722e 7079 2532 3028 3629 2e70 6e67 290d  r.py%20(6).png).
-00002980: 0a0d 0a0d 0a23 2320 4c6f 6361 6c20 496e  .....## Local In
-00002990: 7374 616c 6c61 7469 6f6e 20f0 9f9b a0ef  stallation .....
-000029a0: b88f 0d0a 0d0a 4966 2079 6f75 2064 6f20  ......If you do 
-000029b0: 6e6f 7420 7769 7368 2074 6f20 7573 6520  not wish to use 
-000029c0: 6f75 7220 4150 492c 2079 6f75 2061 7265  our API, you are
-000029d0: 2077 656c 636f 6d65 2068 6f73 7420 5468   welcome host Th
-000029e0: 6520 5069 7065 2066 6f72 2079 6f75 7273  e Pipe for yours
-000029f0: 656c 6620 6c6f 6361 6c6c 792e 200d 0a49  elf locally. ..I
-00002a00: 6620 796f 7520 6368 6f6f 7365 2074 6f20  f you choose to 
-00002a10: 646f 2074 6869 732c 2079 6f75 206d 7573  do this, you mus
-00002a20: 7420 696e 7374 616c 6c20 6120 6e75 6d62  t install a numb
-00002a30: 6572 206f 6620 6465 7065 6e64 656e 6369  er of dependenci
-00002a40: 6573 2066 6f72 2074 6865 2063 6f64 6520  es for the code 
-00002a50: 746f 2066 756e 6374 696f 6e20 636f 7272  to function corr
-00002a60: 6563 746c 792c 2073 6f6d 6520 6f66 2077  ectly, some of w
-00002a70: 6869 6368 206d 6179 2069 6e63 7572 2063  hich may incur c
-00002a80: 6f6d 7075 7465 2063 6f73 7473 2061 6e64  ompute costs and
-00002a90: 2f6f 7220 7265 7175 6972 6520 6120 4750  /or require a GP
-00002aa0: 5520 666f 7220 7265 6173 6f6e 6162 6c65  U for reasonable
-00002ab0: 2070 6572 666f 726d 616e 6365 2e20 4164   performance. Ad
-00002ac0: 6469 7469 6f6e 616c 2069 6e73 7461 6c6c  ditional install
-00002ad0: 6564 2064 6570 656e 6465 6e63 6965 7320  ed dependencies 
-00002ae0: 6172 6520 7265 7175 6972 6564 3a20 7079  are required: py
-00002af0: 746f 7263 682c 2075 6e69 7665 7273 616c  torch, universal
-00002b00: 2d63 7461 6773 2c20 706c 6179 7772 6967  -ctags, playwrig
-00002b10: 6874 2c20 7079 7465 7373 6572 6163 742c  ht, pytesseract,
-00002b20: 206c 6c6d 6c69 6e67 7561 2c20 6d6f 7669   llmlingua, movi
-00002b30: 6570 792c 2061 6e64 2070 7974 7562 652e  epy, and pytube.
-00002b40: 2054 6869 7320 696e 7374 616c 6c61 7469   This installati
-00002b50: 6f6e 2070 726f 6365 7373 2077 696c 6c20  on process will 
-00002b60: 6465 7065 6e64 206f 6e20 796f 7572 2073  depend on your s
-00002b70: 7973 7465 6d20 616e 6420 636f 6d70 7574  ystem and comput
-00002b80: 6520 6361 7061 6269 6c69 7469 6573 2e20  e capabilities. 
-00002b90: 4166 7465 7220 696e 7374 616c 6c69 6e67  After installing
-00002ba0: 2074 6865 6d2c 2066 6f6c 6c6f 7720 7468   them, follow th
-00002bb0: 6573 6520 7374 6570 7320 666f 7220 6120  ese steps for a 
-00002bc0: 6c6f 6361 6c20 7365 7475 703a 0d0a 0d0a  local setup:....
-00002bd0: 4172 6775 6d65 6e74 7320 6172 653a 0d0a  Arguments are:..
-00002be0: 2d20 6073 6f75 7263 6560 2028 7265 7175  - `source` (requ
-00002bf0: 6972 6564 293a 2063 616e 2062 6520 6120  ired): can be a 
-00002c00: 6669 6c65 2070 6174 682c 2061 2055 524c  file path, a URL
-00002c10: 2c20 6f72 2061 2064 6972 6563 746f 7279  , or a directory
-00002c20: 2070 6174 682e 0d0a 2d20 606c 6f63 616c   path...- `local
-00002c30: 6020 286f 7074 696f 6e61 6c29 3a20 5573  ` (optional): Us
-00002c40: 6520 7468 6520 6c6f 6361 6c20 7665 7273  e the local vers
-00002c50: 696f 6e20 6f66 2054 6865 2050 6970 6520  ion of The Pipe 
-00002c60: 696e 7374 6561 6420 6f66 2074 6865 2068  instead of the h
-00002c70: 6f73 7465 6420 4150 492e 0d0a 2d20 606d  osted API...- `m
-00002c80: 6174 6368 6020 286f 7074 696f 6e61 6c29  atch` (optional)
-00002c90: 3a20 5375 6273 7472 696e 6720 746f 206d  : Substring to m
-00002ca0: 6174 6368 2066 696c 6573 2069 6e20 7468  atch files in th
-00002cb0: 6520 6469 7265 6374 6f72 792e 2052 6567  e directory. Reg
-00002cc0: 6578 2069 7320 6e6f 7420 7965 7420 7375  ex is not yet su
-00002cd0: 7070 6f72 7465 642e 0d0a 2d20 6069 676e  pported...- `ign
-00002ce0: 6f72 6560 2028 6f70 7469 6f6e 616c 293a  ore` (optional):
-00002cf0: 2053 7562 7374 7269 6e67 2074 6f20 6967   Substring to ig
-00002d00: 6e6f 7265 2066 696c 6573 2069 6e20 7468  nore files in th
-00002d10: 6520 6469 7265 6374 6f72 792e 2052 6567  e directory. Reg
-00002d20: 6578 2069 7320 6e6f 7420 7965 7420 7375  ex is not yet su
-00002d30: 7070 6f72 7465 642e 0d0a 2d20 606c 696d  pported...- `lim
-00002d40: 6974 6020 286f 7074 696f 6e61 6c29 3a20  it` (optional): 
-00002d50: 5468 6520 746f 6b65 6e20 6c69 6d69 7420  The token limit 
-00002d60: 666f 7220 7468 6520 6f75 7470 7574 2070  for the output p
-00002d70: 726f 6d70 742c 2064 6566 6175 6c74 7320  rompt, defaults 
-00002d80: 746f 2031 3030 4b2e 2050 726f 6d70 7473  to 100K. Prompts
-00002d90: 2065 7863 6565 6469 6e67 2074 6865 206c   exceeding the l
-00002da0: 696d 6974 2077 696c 6c20 6265 2063 6f6d  imit will be com
-00002db0: 7072 6573 7365 642e 2054 6869 7320 6d61  pressed. This ma
-00002dc0: 7920 6e6f 7420 776f 726b 2061 7320 6578  y not work as ex
-00002dd0: 7065 6374 6564 2077 6974 6820 7468 6520  pected with the 
-00002de0: 4150 492c 2061 7320 6974 2069 7320 696e  API, as it is in
-00002df0: 2061 6374 6976 6520 6465 7665 6c6f 706d   active developm
-00002e00: 656e 742e 0d0a 2d20 6061 695f 6578 7472  ent...- `ai_extr
-00002e10: 6163 7469 6f6e 6020 286f 7074 696f 6e61  action` (optiona
-00002e20: 6c29 3a20 4578 7472 6163 7420 7461 626c  l): Extract tabl
-00002e30: 6573 2c20 6669 6775 7265 732c 2061 6e64  es, figures, and
-00002e40: 206d 6174 6820 6672 6f6d 2050 4446 7320   math from PDFs 
-00002e50: 7573 696e 6720 6f75 7220 6578 7472 6163  using our extrac
-00002e60: 746f 722e 2049 6e63 7572 7320 6578 7472  tor. Incurs extr
-00002e70: 6120 636f 7374 732e 0d0a 2d20 6074 6578  a costs...- `tex
-00002e80: 745f 6f6e 6c79 6020 286f 7074 696f 6e61  t_only` (optiona
-00002e90: 6c29 3a20 446f 206e 6f74 2065 7874 7261  l): Do not extra
-00002ea0: 6374 2069 6d61 6765 7320 6672 6f6d 2064  ct images from d
-00002eb0: 6f63 756d 656e 7473 206f 7220 7765 6273  ocuments or webs
-00002ec0: 6974 6573 2e20 4164 6469 7469 6f6e 616c  ites. Additional
-00002ed0: 6c79 2c20 696d 6167 6520 6669 6c65 7320  ly, image files 
-00002ee0: 7769 6c6c 2062 6520 7265 7072 6573 656e  will be represen
-00002ef0: 7465 6420 7769 7468 204f 4352 2069 6e73  ted with OCR ins
-00002f00: 7465 6164 206f 6620 6173 2069 6d61 6765  tead of as image
-00002f10: 732e 0d0a 0d0a 2320 5370 6f6e 736f 7273  s.....# Sponsors
-00002f20: 0d0a 0d0a 3c61 2068 7265 663d 2268 7474  ....<a href="htt
-00002f30: 7073 3a2f 2f63 616c 2e63 6f6d 2f65 6d6d  ps://cal.com/emm
-00002f40: 6574 742d 6d63 662f 3330 6d69 6e22 3e3c  ett-mcf/30min"><
-00002f50: 696d 6720 616c 743d 2242 6f6f 6b20 7573  img alt="Book us
-00002f60: 2077 6974 6820 4361 6c2e 636f 6d22 2073   with Cal.com" s
-00002f70: 7263 3d22 6874 7470 733a 2f2f 6361 6c2e  rc="https://cal.
-00002f80: 636f 6d2f 626f 6f6b 2d77 6974 682d 6361  com/book-with-ca
-00002f90: 6c2d 6461 726b 2e73 7667 2220 2f3e 3c2f  l-dark.svg" /></
-00002fa0: 613e 0d0a 0d0a 5468 616e 6b20 796f 7520  a>....Thank you 
-00002fb0: 746f 205b 4361 6c2e 636f 6d5d 2868 7474  to [Cal.com](htt
-00002fc0: 7073 3a2f 2f63 616c 2e63 6f6d 2f29 2066  ps://cal.com/) f
-00002fd0: 6f72 2073 706f 6e73 6f72 696e 6720 7468  or sponsoring th
-00002fe0: 6973 2070 726f 6a65 6374 2e20 436f 6e74  is project. Cont
-00002ff0: 6163 7420 656d 6d65 7474 4074 6865 7069  act emmett@thepi
-00003000: 2e70 6520 666f 7220 7370 6f6e 736f 7273  .pe for sponsors
-00003010: 6869 7020 696e 666f 726d 6174 696f 6e2e  hip information.
-00003020: 0d0a                                     ..
+000018a0: 2020 2020 2020 2020 2020 2020 207c 2055               | U
+000018b0: 524c 7320 2869 6e70 7574 7320 7374 6172  RLs (inputs star
+000018c0: 7469 6e67 2077 6974 6820 6068 7474 7060  ting with `http`
+000018d0: 2c20 6068 7474 7073 602c 2060 6674 7060  , `https`, `ftp`
+000018e0: 2920 2020 2020 2020 2020 2020 2020 7c20  )             | 
+000018f0: e29c 94ef b88f 2020 2020 2020 2020 2020  ......          
+00001900: 2020 2020 2020 7c20 e29c 94ef b88f 2020        | ......  
+00001910: 2020 7c20 4578 7472 6163 7473 2074 6578    | Extracts tex
+00001920: 7420 6672 6f6d 2077 6562 2070 6167 6520  t from web page 
+00001930: 616c 6f6e 6720 7769 7468 2069 6d61 6765  along with image
+00001940: 2028 6f72 2069 6d61 6765 7320 6966 2073   (or images if s
+00001950: 6372 6f6c 6c61 626c 6529 3b20 7465 7874  crollable); text
+00001960: 2d6f 6e6c 7920 6578 7472 6163 7469 6f6e  -only extraction
+00001970: 2061 7661 696c 6162 6c65 2020 2020 2020   available      
+00001980: 2020 2020 7c0d 0a7c 2047 6974 4875 6220      |..| GitHub 
+00001990: 5265 706f 7369 746f 7279 2020 2020 2020  Repository      
+000019a0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000019b0: 2047 6974 4875 6220 7265 706f 2055 524c   GitHub repo URL
+000019c0: 7320 2869 6e70 7574 7320 7374 6172 7469  s (inputs starti
+000019d0: 6e67 2077 6974 6820 6068 7474 7073 3a2f  ng with `https:/
+000019e0: 2f67 6974 6875 622e 636f 6d60 206f 7220  /github.com` or 
+000019f0: 6068 7474 7073 3a2f 2f77 7777 2e67 6974  `https://www.git
+00001a00: 6875 622e 636f 6d60 2920 2020 2020 2020  hub.com`)       
+00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a20: 2020 207c 20e2 9c94 efb8 8f20 2020 2020     | ......     
+00001a30: 2020 2020 2020 2020 2020 7c20 e29c 94ef            | ....
+00001a40: b88f 2020 2020 2020 2020 2020 2020 2020  ..              
+00001a50: 2020 7c20 4578 7472 6163 7473 2066 726f    | Extracts fro
+00001a60: 6d20 4769 7448 7562 2072 6570 6f73 6974  m GitHub reposit
+00001a70: 6f72 6965 733b 2073 7570 706f 7274 7320  ories; supports 
+00001a80: 6272 616e 6368 2073 7065 6369 6669 6361  branch specifica
+00001a90: 7469 6f6e 2020 2020 2020 2020 207c 0d0a  tion         |..
+00001aa0: 7c20 596f 7554 7562 6520 5669 6465 6f20  | YouTube Video 
+00001ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ac0: 2020 2020 2020 2020 7c20 596f 7554 7562          | YouTub
+00001ad0: 6520 7669 6465 6f20 5552 4c73 2028 696e  e video URLs (in
+00001ae0: 7075 7473 2073 7461 7274 696e 6720 7769  puts starting wi
+00001af0: 7468 2060 6874 7470 733a 2f2f 796f 7574  th `https://yout
+00001b00: 7562 652e 636f 6d60 206f 7220 6068 7474  ube.com` or `htt
+00001b10: 7073 3a2f 2f77 7777 2e79 6f75 7475 6265  ps://www.youtube
+00001b20: 2e63 6f6d 6029 2020 2020 2020 2020 2020  .com`)          
+00001b30: 2020 2020 2020 2020 2020 207c 20e2 9c94             | ...
+00001b40: efb8 8f20 2020 2020 2020 2020 2020 2020  ...             
+00001b50: 2020 7c20 e29c 94ef b88f 2020 2020 2020    | ......      
+00001b60: 2020 2020 2020 2020 2020 7c20 4578 7472            | Extr
+00001b70: 6163 7473 2066 7261 6d65 7320 616e 6420  acts frames and 
+00001b80: 7472 616e 7363 7269 7074 2066 726f 6d20  transcript from 
+00001b90: 596f 7554 7562 6520 7669 6465 6f73 2069  YouTube videos i
+00001ba0: 6e20 7065 722d 6d69 6e75 7465 2063 6875  n per-minute chu
+00001bb0: 6e6b 732e 2020 2020 2020 2020 2020 7c0d  nks.          |.
+00001bc0: 0a7c 205a 4950 2046 696c 6520 2020 2020  .| ZIP File     
+00001bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001be0: 2020 2020 2020 2020 207c 2060 2e7a 6970           | `.zip
+00001bf0: 6020 2020 2020 2020 2020 2020 2020 2020  `               
+00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c10: 2020 207c 20e2 9c94 efb8 8f20 2020 2020     | ......     
+00001c20: 2020 2020 2020 2020 2020 7c20 e29c 94ef            | ....
+00001c30: b88f 2020 2020 2020 2020 2020 2020 2020  ..              
+00001c40: 2020 7c20 4578 7472 6163 7473 2063 6f6e    | Extracts con
+00001c50: 7465 6e74 7320 6f66 205a 4950 2066 696c  tents of ZIP fil
+00001c60: 6573 3b20 7375 7070 6f72 7473 206e 6573  es; supports nes
+00001c70: 7465 6420 6469 7265 6374 6f72 7920 6578  ted directory ex
+00001c80: 7472 6163 7469 6f6e 2020 2020 207c 0d0a  traction     |..
+00001c90: 0d0a 2323 2048 6f77 2069 7420 776f 726b  ..## How it work
+00001ca0: 7320 f09f 9ba0 efb8 8f0d 0a0d 0a54 6865  s ...........The
+00001cb0: 2069 6e70 7574 2073 6f75 7263 6520 6973   input source is
+00001cc0: 2065 6974 6865 7220 6120 6669 6c65 2070   either a file p
+00001cd0: 6174 682c 2061 2055 524c 2c20 6f72 2061  ath, a URL, or a
+00001ce0: 2064 6972 6563 746f 7279 2e20 5468 6520   directory. The 
+00001cf0: 7069 7065 2077 696c 6c20 6578 7472 6163  pipe will extrac
+00001d00: 7420 696e 666f 726d 6174 696f 6e20 6672  t information fr
+00001d10: 6f6d 2074 6865 2073 6f75 7263 6520 616e  om the source an
+00001d20: 6420 7072 6f63 6573 7320 6974 2066 6f72  d process it for
+00001d30: 2064 6f77 6e73 7472 6561 6d20 7573 6520   downstream use 
+00001d40: 7769 7468 205b 6c61 6e67 7561 6765 206d  with [language m
+00001d50: 6f64 656c 735d 2868 7474 7073 3a2f 2f65  odels](https://e
+00001d60: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
+00001d70: 7769 6b69 2f4c 6172 6765 5f6c 616e 6775  wiki/Large_langu
+00001d80: 6167 655f 6d6f 6465 6c29 2c20 5b76 6973  age_model), [vis
+00001d90: 696f 6e20 7472 616e 7366 6f72 6d65 7273  ion transformers
+00001da0: 5d28 6874 7470 733a 2f2f 656e 2e77 696b  ](https://en.wik
+00001db0: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
+00001dc0: 5669 7369 6f6e 5f74 7261 6e73 666f 726d  Vision_transform
+00001dd0: 6572 292c 206f 7220 5b76 6973 696f 6e2d  er), or [vision-
+00001de0: 6c61 6e67 7561 6765 206d 6f64 656c 735d  language models]
+00001df0: 2868 7474 7073 3a2f 2f61 7278 6976 2e6f  (https://arxiv.o
+00001e00: 7267 2f61 6273 2f32 3330 342e 3030 3638  rg/abs/2304.0068
+00001e10: 3529 2e20 5468 6520 6f75 7470 7574 2066  5). The output f
+00001e20: 726f 6d20 7468 6520 7069 7065 2069 7320  rom the pipe is 
+00001e30: 6120 7365 6e73 6962 6c65 206c 6973 7420  a sensible list 
+00001e40: 6f66 206d 756c 7469 6d6f 6461 6c20 6d65  of multimodal me
+00001e50: 7373 6167 6573 2072 6570 7265 7365 6e74  ssages represent
+00001e60: 696e 6720 6368 756e 6b73 206f 6620 7468  ing chunks of th
+00001e70: 6520 6578 7472 6163 7465 6420 696e 666f  e extracted info
+00001e80: 726d 6174 696f 6e2c 2063 6172 6566 756c  rmation, careful
+00001e90: 6c79 2063 7261 6674 6564 2074 6f20 6669  ly crafted to fi
+00001ea0: 7420 7769 7468 696e 2063 6f6e 7465 7874  t within context
+00001eb0: 2077 696e 646f 7773 2066 6f72 2061 6e79   windows for any
+00001ec0: 206d 6f64 656c 7320 6672 6f6d 205b 6765   models from [ge
+00001ed0: 6d6d 612d 3762 5d28 6874 7470 733a 2f2f  mma-7b](https://
+00001ee0: 6875 6767 696e 6766 6163 652e 636f 2f67  huggingface.co/g
+00001ef0: 6f6f 676c 652f 6765 6d6d 612d 3762 2920  oogle/gemma-7b) 
+00001f00: 746f 205b 4750 542d 345d 2868 7474 7073  to [GPT-4](https
+00001f10: 3a2f 2f6f 7065 6e61 692e 636f 6d2f 6770  ://openai.com/gp
+00001f20: 742d 3429 2e20 5468 6520 6d65 7373 6167  t-4). The messag
+00001f30: 6573 2072 6574 7572 6e65 6420 7368 6f75  es returned shou
+00001f40: 6c64 206c 6f6f 6b20 6c69 6b65 2074 6869  ld look like thi
+00001f50: 733a 0d0a 6060 606a 736f 6e0d 0a5b 0d0a  s:..```json..[..
+00001f60: 2020 7b0d 0a20 2020 2022 726f 6c65 223a    {..    "role":
+00001f70: 2022 7573 6572 222c 0d0a 2020 2020 2263   "user",..    "c
+00001f80: 6f6e 7465 6e74 223a 205b 0d0a 2020 2020  ontent": [..    
+00001f90: 2020 7b0d 0a20 2020 2020 2020 2022 7479    {..        "ty
+00001fa0: 7065 223a 2022 7465 7874 222c 0d0a 2020  pe": "text",..  
+00001fb0: 2020 2020 2020 2274 6578 7422 3a20 222e        "text": ".
+00001fc0: 2e2e 220d 0a20 2020 2020 207d 2c0d 0a20  .."..      },.. 
+00001fd0: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
+00001fe0: 2274 7970 6522 3a20 2269 6d61 6765 5f75  "type": "image_u
+00001ff0: 726c 222c 0d0a 2020 2020 2020 2020 2269  rl",..        "i
+00002000: 6d61 6765 5f75 726c 223a 207b 0d0a 2020  mage_url": {..  
+00002010: 2020 2020 2020 2020 2275 726c 223a 2022          "url": "
+00002020: 6461 7461 3a69 6d61 6765 2f6a 7065 673b  data:image/jpeg;
+00002030: 6261 7365 3634 2c2e 2e2e 220d 0a20 2020  base64,..."..   
+00002040: 2020 2020 207d 0d0a 2020 2020 2020 7d0d       }..      }.
+00002050: 0a20 2020 205d 0d0a 2020 7d0d 0a5d 0d0a  .    ]..  }..]..
+00002060: 6060 600d 0a49 6620 796f 7520 7761 6e74  ```..If you want
+00002070: 2074 6f20 6665 6564 2074 6865 7365 206d   to feed these m
+00002080: 6573 7361 6765 7320 6469 7265 6374 6c79  essages directly
+00002090: 2069 6e74 6f20 7468 6520 6d6f 6465 6c2c   into the model,
+000020a0: 2069 7420 6973 2069 6d70 6f72 7461 6e74   it is important
+000020b0: 2074 6f20 6265 206d 696e 6466 756c 206f   to be mindful o
+000020c0: 6620 7468 6520 746f 6b65 6e20 6c69 6d69  f the token limi
+000020d0: 742e 0d0a 4f70 656e 4149 2064 6f65 7320  t...OpenAI does 
+000020e0: 6e6f 7420 616c 6c6f 7720 746f 6f20 6d61  not allow too ma
+000020f0: 6e79 2069 6d61 6765 7320 696e 2074 6865  ny images in the
+00002100: 2070 726f 6d70 7420 2873 6565 2064 6973   prompt (see dis
+00002110: 6375 7373 696f 6e20 5b68 6572 655d 2868  cussion [here](h
+00002120: 7474 7073 3a2f 2f63 6f6d 6d75 6e69 7479  ttps://community
+00002130: 2e6f 7065 6e61 692e 636f 6d2f 742f 6770  .openai.com/t/gp
+00002140: 742d 342d 7669 7369 6f6e 2d6d 6178 696d  t-4-vision-maxim
+00002150: 756d 2d61 6d6f 756e 742d 6f66 2d69 6d61  um-amount-of-ima
+00002160: 6765 732f 3537 3331 3130 2f36 2929 2c20  ges/573110/6)), 
+00002170: 736f 206c 6f6e 6720 6669 6c65 7320 7368  so long files sh
+00002180: 6f75 6c64 2062 6520 6578 7472 6163 7465  ould be extracte
+00002190: 6420 7769 7468 2060 7465 7874 5f6f 6e6c  d with `text_onl
+000021a0: 793d 5472 7565 6020 746f 2061 766f 6964  y=True` to avoid
+000021b0: 2074 6869 7320 6973 7375 652c 2077 6869   this issue, whi
+000021c0: 6c65 206c 6f6e 6720 7465 7874 2066 696c  le long text fil
+000021d0: 6573 2073 686f 756c 6420 6569 7468 6572  es should either
+000021e0: 2062 6520 636f 6d70 7265 7373 6564 206f   be compressed o
+000021f0: 7220 656d 6265 6464 6564 2069 6e20 6120  r embedded in a 
+00002200: 5241 4720 6672 616d 6577 6f72 6b2e 0d0a  RAG framework...
+00002210: 0d0a 5468 6520 7465 7874 2061 6e64 2069  ..The text and i
+00002220: 6d61 6765 7320 6672 6f6d 2074 6865 7365  mages from these
+00002230: 206d 6573 7361 6765 7320 6d61 7920 616c   messages may al
+00002240: 736f 2062 6520 7072 6570 6172 6564 2066  so be prepared f
+00002250: 6f72 2061 2076 6563 746f 7220 6461 7461  or a vector data
+00002260: 6261 7365 2077 6974 6820 6074 6865 7069  base with `thepi
+00002270: 7065 2e63 6f72 652e 6372 6561 7465 5f63  pe.core.create_c
+00002280: 6875 6e6b 735f 6672 6f6d 5f6d 6573 7361  hunks_from_messa
+00002290: 6765 7360 206f 7220 666f 7220 646f 776e  ges` or for down
+000022a0: 7374 7265 616d 2075 7365 2077 6974 6820  stream use with 
+000022b0: 5241 4720 6672 616d 6577 6f72 6b73 2e20  RAG frameworks. 
+000022c0: 5b4c 6974 654c 4c4d 5d28 6874 7470 733a  [LiteLLM](https:
+000022d0: 2f2f 6769 7468 7562 2e63 6f6d 2f42 6572  //github.com/Ber
+000022e0: 7269 4149 2f6c 6974 656c 6c6d 2920 6361  riAI/litellm) ca
+000022f0: 6e20 6265 2075 7365 6420 746f 2065 6173  n be used to eas
+00002300: 696c 7920 696e 7465 6772 6174 6520 5468  ily integrate Th
+00002310: 6520 5069 7065 2077 6974 6820 616e 7920  e Pipe with any 
+00002320: 4c4c 4d20 7072 6f76 6964 6572 2e20 0d0a  LLM provider. ..
+00002330: 0d0a 4974 2075 7365 7320 6120 7661 7269  ..It uses a vari
+00002340: 6574 7920 6f66 2068 6575 7269 7374 6963  ety of heuristic
+00002350: 7320 666f 7220 6f70 7469 6d61 6c20 7065  s for optimal pe
+00002360: 7266 6f72 6d61 6e63 6520 7769 7468 2076  rformance with v
+00002370: 6973 696f 6e2d 6c61 6e67 7561 6765 206d  ision-language m
+00002380: 6f64 656c 732c 2069 6e63 6c75 6469 6e67  odels, including
+00002390: 2041 4920 6669 6c65 7479 7065 2064 6574   AI filetype det
+000023a0: 6563 7469 6f6e 2077 6974 6820 5b66 696c  ection with [fil
+000023b0: 6574 7970 6520 6465 7465 6374 696f 6e5d  etype detection]
+000023c0: 2868 7474 7073 3a2f 2f6f 7065 6e73 6f75  (https://opensou
+000023d0: 7263 652e 676f 6f67 6c65 626c 6f67 2e63  rce.googleblog.c
+000023e0: 6f6d 2f32 3032 342f 3032 2f6d 6167 696b  om/2024/02/magik
+000023f0: 612d 6169 2d70 6f77 6572 6564 2d66 6173  a-ai-powered-fas
+00002400: 742d 616e 642d 6566 6669 6369 656e 742d  t-and-efficient-
+00002410: 6669 6c65 2d74 7970 652d 6964 656e 7469  file-type-identi
+00002420: 6669 6361 7469 6f6e 2e68 746d 6c29 2c20  fication.html), 
+00002430: 6f70 742d 696e 2041 4920 5b74 6162 6c65  opt-in AI [table
+00002440: 2c20 6571 7561 7469 6f6e 2c20 616e 6420  , equation, and 
+00002450: 6669 6775 7265 2065 7874 7261 6374 696f  figure extractio
+00002460: 6e5d 2868 7474 7073 3a2f 2f74 6865 7069  n](https://thepi
+00002470: 2e70 652f 7072 6963 696e 6729 2c20 6566  .pe/pricing), ef
+00002480: 6669 6369 656e 7420 5b74 6f6b 656e 2063  ficient [token c
+00002490: 6f6d 7072 6573 7369 6f6e 5d28 6874 7470  ompression](http
+000024a0: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
+000024b0: 732f 3234 3033 2e31 3239 3638 292c 2061  s/2403.12968), a
+000024c0: 7574 6f6d 6174 6963 205b 696d 6167 6520  utomatic [image 
+000024d0: 656e 636f 6469 6e67 5d28 6874 7470 733a  encoding](https:
+000024e0: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
+000024f0: 7267 2f77 696b 692f 4261 7365 3634 292c  rg/wiki/Base64),
+00002500: 205b 7265 7261 6e6b 696e 675d 2868 7474   [reranking](htt
+00002510: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
+00002520: 6273 2f32 3331 302e 3036 3833 3929 2066  bs/2310.06839) f
+00002530: 6f72 205b 6c6f 7374 2d69 6e2d 7468 652d  or [lost-in-the-
+00002540: 6d69 6464 6c65 5d28 6874 7470 733a 2f2f  middle](https://
+00002550: 6172 7869 762e 6f72 672f 6162 732f 3233  arxiv.org/abs/23
+00002560: 3037 2e30 3331 3732 2920 6566 6665 6374  07.03172) effect
+00002570: 732c 2061 6e64 206d 6f72 652c 2061 6c6c  s, and more, all
+00002580: 2070 7265 2d62 7569 6c74 2074 6f20 776f   pre-built to wo
+00002590: 726b 206f 7574 2d6f 662d 7468 652d 626f  rk out-of-the-bo
+000025a0: 782e 0d0a 0d0a 215b 4465 6d6f 5d28 6874  x.....![Demo](ht
+000025b0: 7470 733a 2f2f 7270 6e75 747a 656d 7574  tps://rpnutzemut
+000025c0: 6272 756d 637a 7776 7565 2e73 7570 6162  brumczwvue.supab
+000025d0: 6173 652e 636f 2f73 746f 7261 6765 2f76  ase.co/storage/v
+000025e0: 312f 6f62 6a65 6374 2f70 7562 6c69 632f  1/object/public/
+000025f0: 6173 7365 7473 2f67 7261 6465 722e 7079  assets/grader.py
+00002600: 2532 3028 3629 2e70 6e67 290d 0a0d 0a0d  %20(6).png).....
+00002610: 0a23 2320 4c6f 6361 6c20 496e 7374 616c  .## Local Instal
+00002620: 6c61 7469 6f6e 20f0 9f9b a0ef b88f 0d0a  lation .........
+00002630: 0d0a 5468 6520 5069 7065 2068 616e 646c  ..The Pipe handl
+00002640: 6573 2061 2077 6964 6520 6172 7261 7920  es a wide array 
+00002650: 6f66 2063 6f6d 706c 6578 2066 696c 6574  of complex filet
+00002660: 7970 6573 2c20 616e 6420 7468 7573 2072  ypes, and thus r
+00002670: 6571 7569 7265 7320 696e 7374 616c 6c61  equires installa
+00002680: 7469 6f6e 206f 6620 6d61 6e79 2064 6966  tion of many dif
+00002690: 6665 7265 6e74 2070 6163 6b61 6765 7320  ferent packages 
+000026a0: 746f 2066 756e 6374 696f 6e2e 2049 7420  to function. It 
+000026b0: 616c 736f 2072 6571 7569 7265 7320 6120  also requires a 
+000026c0: 7665 7279 2063 6170 6162 6c65 206d 6163  very capable mac
+000026d0: 6869 6e65 2066 6f72 2067 6f6f 6420 7265  hine for good re
+000026e0: 7370 6f6e 7365 2074 696d 6573 2e20 466f  sponse times. Fo
+000026f0: 7220 7468 6973 2072 6561 736f 6e2c 2077  r this reason, w
+00002700: 6520 686f 7374 2069 7420 6173 2061 6e20  e host it as an 
+00002710: 4150 4920 7468 6174 2077 6f72 6b73 206f  API that works o
+00002720: 7574 2d6f 662d 7468 652d 626f 782e 2054  ut-of-the-box. T
+00002730: 6f20 7573 6520 5468 6520 5069 7065 206c  o use The Pipe l
+00002740: 6f63 616c 6c79 2066 6f72 2066 7265 6520  ocally for free 
+00002750: 696e 7374 6561 642c 2079 6f75 2077 696c  instead, you wil
+00002760: 6c20 6e65 6564 205b 706c 6179 7772 6967  l need [playwrig
+00002770: 6874 5d28 6874 7470 733a 2f2f 6769 7468  ht](https://gith
+00002780: 7562 2e63 6f6d 2f6d 6963 726f 736f 6674  ub.com/microsoft
+00002790: 2f70 6c61 7977 7269 6768 7429 2c20 5b63  /playwright), [c
+000027a0: 7461 6773 5d28 6874 7470 733a 2f2f 6769  tags](https://gi
+000027b0: 7468 7562 2e63 6f6d 2f75 6e69 7665 7273  thub.com/univers
+000027c0: 616c 2d63 7461 6773 2f29 2c20 5b70 7974  al-ctags/), [pyt
+000027d0: 6573 7365 7261 6374 5d28 6874 7470 733a  esseract](https:
+000027e0: 2f2f 6769 7468 7562 2e63 6f6d 2f68 2f70  //github.com/h/p
+000027f0: 7974 6573 7365 7261 6374 292c 205b 7079  ytesseract), [py
+00002800: 7475 6265 5d28 6874 7470 733a 2f2f 6769  tube](https://gi
+00002810: 7468 7562 2e63 6f6d 2f70 7974 7562 652f  thub.com/pytube/
+00002820: 2920 616e 6420 7468 6520 7265 6d61 696e  ) and the remain
+00002830: 696e 6720 6c6f 6361 6c20 7079 7468 6f6e  ing local python
+00002840: 2072 6571 7569 7265 6d65 6e74 732c 2077   requirements, w
+00002850: 6869 6368 2064 6966 6665 7220 6672 6f6d  hich differ from
+00002860: 2074 6865 206d 6f72 6520 6c69 6768 7477   the more lightw
+00002870: 6569 6768 7420 4150 4920 7265 7175 6972  eight API requir
+00002880: 656d 656e 7473 3a0d 0a0d 0a60 6060 6261  ements:....```ba
+00002890: 7368 0d0a 6769 7420 636c 6f6e 6520 6874  sh..git clone ht
+000028a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000028b0: 2f65 6d63 662f 7468 6570 6970 650d 0a70  /emcf/thepipe..p
+000028c0: 6970 2069 6e73 7461 6c6c 202d 7220 7265  ip install -r re
+000028d0: 7175 6972 656d 656e 7473 5f6c 6f63 616c  quirements_local
+000028e0: 2e74 7874 0d0a 6060 600d 0a0d 0a54 6970  .txt..```....Tip
+000028f0: 2066 6f72 2077 696e 646f 7773 2075 7365   for windows use
+00002900: 7273 3a20 496e 7374 616c 6c20 7468 6520  rs: Install the 
+00002910: 7079 7468 6f6e 2d6c 6962 6d61 6769 6320  python-libmagic 
+00002920: 6269 6e61 7269 6573 2077 6974 6820 6070  binaries with `p
+00002930: 6970 2069 6e73 7461 6c6c 2070 7974 686f  ip install pytho
+00002940: 6e2d 6d61 6769 632d 6269 6e60 2e20 456e  n-magic-bin`. En
+00002950: 7375 7265 2074 6865 2060 7465 7373 6572  sure the `tesser
+00002960: 6163 742d 6f63 7260 2062 696e 6172 6965  act-ocr` binarie
+00002970: 7320 616e 6420 7468 6520 6063 7461 6773  s and the `ctags
+00002980: 6020 6269 6e61 7269 6573 2061 7265 2069  ` binaries are i
+00002990: 6e20 796f 7572 2050 4154 482e 2046 6f72  n your PATH. For
+000029a0: 2059 6f75 5475 6265 2076 6964 656f 2065   YouTube video e
+000029b0: 7874 7261 6374 696f 6e20 746f 2066 756e  xtraction to fun
+000029c0: 6374 696f 6e20 636f 6e73 6973 7465 6e74  ction consistent
+000029d0: 6c79 2c20 796f 7520 7769 6c6c 206e 6565  ly, you will nee
+000029e0: 6420 746f 206d 6f64 6966 7920 796f 7572  d to modify your
+000029f0: 2060 7079 7475 6265 6020 696e 7374 616c   `pytube` instal
+00002a00: 6c61 7469 6f6e 2074 6f20 7365 6e64 2061  lation to send a
+00002a10: 2076 616c 6964 2075 7365 7220 6167 656e   valid user agen
+00002a20: 7420 6865 6164 6572 2028 4920 6b6e 6f77  t header (I know
+00002a30: 2c20 6974 2773 2063 6f6d 706c 6963 6174  , it's complicat
+00002a40: 6564 2e20 5365 6520 5b74 6869 7320 6973  ed. See [this is
+00002a50: 7375 655d 2868 7474 7073 3a2f 2f67 6974  sue](https://git
+00002a60: 6875 622e 636f 6d2f 7079 7475 6265 2f70  hub.com/pytube/p
+00002a70: 7974 7562 652f 6973 7375 6573 2f33 3939  ytube/issues/399
+00002a80: 2920 666f 7220 6d6f 7265 292e 0d0a 0d0a  ) for more).....
+00002a90: 4e6f 7720 796f 7520 6361 6e20 7573 6520  Now you can use 
+00002aa0: 5468 6520 5069 7065 2077 6974 6820 5079  The Pipe with Py
+00002ab0: 7468 6f6e 3a0d 0a60 6060 6261 7368 0d0a  thon:..```bash..
+00002ac0: 6672 6f6d 2074 6865 7069 7065 5f61 7069  from thepipe_api
+00002ad0: 2069 6d70 6f72 7420 7468 6570 6970 650d   import thepipe.
+00002ae0: 0a63 6875 6e6b 7320 3d20 7468 6570 6970  .chunks = thepip
+00002af0: 652e 6578 7472 6163 7428 2265 7861 6d70  e.extract("examp
+00002b00: 6c65 2e70 6466 222c 206c 6f63 616c 3d54  le.pdf", local=T
+00002b10: 7275 6529 0d0a 6060 600d 0a0d 0a6f 7220  rue)..```....or 
+00002b20: 6672 6f6d 2074 6865 2063 6f6d 6d61 6e64  from the command
+00002b30: 206c 696e 653a 0d0a 6060 6062 6173 680d   line:..```bash.
+00002b40: 0a74 6865 7069 7065 2070 6174 682f 746f  .thepipe path/to
+00002b50: 2f66 6f6c 6465 7220 2d2d 6d61 7463 6820  /folder --match 
+00002b60: 2e74 7378 202d 2d69 676e 6f72 6520 7465  .tsx --ignore te
+00002b70: 7374 730d 0a60 6060 0d0a 0d0a 4172 6775  sts..```....Argu
+00002b80: 6d65 6e74 7320 6172 653a 0d0a 2d20 6073  ments are:..- `s
+00002b90: 6f75 7263 6560 2028 7265 7175 6972 6564  ource` (required
+00002ba0: 293a 2063 616e 2062 6520 6120 6669 6c65  ): can be a file
+00002bb0: 2070 6174 682c 2061 2055 524c 2c20 6f72   path, a URL, or
+00002bc0: 2061 2064 6972 6563 746f 7279 2070 6174   a directory pat
+00002bd0: 682e 0d0a 2d20 606c 6f63 616c 6020 286f  h...- `local` (o
+00002be0: 7074 696f 6e61 6c29 3a20 5573 6520 7468  ptional): Use th
+00002bf0: 6520 6c6f 6361 6c20 7665 7273 696f 6e20  e local version 
+00002c00: 6f66 2054 6865 2050 6970 6520 696e 7374  of The Pipe inst
+00002c10: 6561 6420 6f66 2074 6865 2068 6f73 7465  ead of the hoste
+00002c20: 6420 4150 492e 0d0a 2d20 606d 6174 6368  d API...- `match
+00002c30: 6020 286f 7074 696f 6e61 6c29 3a20 5375  ` (optional): Su
+00002c40: 6273 7472 696e 6720 746f 206d 6174 6368  bstring to match
+00002c50: 2066 696c 6573 2069 6e20 7468 6520 6469   files in the di
+00002c60: 7265 6374 6f72 792e 2052 6567 6578 2069  rectory. Regex i
+00002c70: 7320 6e6f 7420 7965 7420 7375 7070 6f72  s not yet suppor
+00002c80: 7465 642e 0d0a 2d20 6069 676e 6f72 6560  ted...- `ignore`
+00002c90: 2028 6f70 7469 6f6e 616c 293a 2053 7562   (optional): Sub
+00002ca0: 7374 7269 6e67 2074 6f20 6967 6e6f 7265  string to ignore
+00002cb0: 2066 696c 6573 2069 6e20 7468 6520 6469   files in the di
+00002cc0: 7265 6374 6f72 792e 2052 6567 6578 2069  rectory. Regex i
+00002cd0: 7320 6e6f 7420 7965 7420 7375 7070 6f72  s not yet suppor
+00002ce0: 7465 642e 0d0a 2d20 606c 696d 6974 6020  ted...- `limit` 
+00002cf0: 286f 7074 696f 6e61 6c29 3a20 5468 6520  (optional): The 
+00002d00: 746f 6b65 6e20 6c69 6d69 7420 666f 7220  token limit for 
+00002d10: 7468 6520 6f75 7470 7574 2070 726f 6d70  the output promp
+00002d20: 742c 2064 6566 6175 6c74 7320 746f 2031  t, defaults to 1
+00002d30: 3030 4b2e 2050 726f 6d70 7473 2065 7863  00K. Prompts exc
+00002d40: 6565 6469 6e67 2074 6865 206c 696d 6974  eeding the limit
+00002d50: 2077 696c 6c20 6265 2063 6f6d 7072 6573   will be compres
+00002d60: 7365 642e 2054 6869 7320 6d61 7920 6e6f  sed. This may no
+00002d70: 7420 776f 726b 2061 7320 6578 7065 6374  t work as expect
+00002d80: 6564 2077 6974 6820 7468 6520 4150 492c  ed with the API,
+00002d90: 2061 7320 6974 2069 7320 696e 2061 6374   as it is in act
+00002da0: 6976 6520 6465 7665 6c6f 706d 656e 742e  ive development.
+00002db0: 0d0a 2d20 6061 695f 6578 7472 6163 7469  ..- `ai_extracti
+00002dc0: 6f6e 6020 286f 7074 696f 6e61 6c29 3a20  on` (optional): 
+00002dd0: 4578 7472 6163 7420 7461 626c 6573 2c20  Extract tables, 
+00002de0: 6669 6775 7265 732c 2061 6e64 206d 6174  figures, and mat
+00002df0: 6820 6672 6f6d 2050 4446 7320 7573 696e  h from PDFs usin
+00002e00: 6720 6f75 7220 6578 7472 6163 746f 722e  g our extractor.
+00002e10: 2049 6e63 7572 7320 6578 7472 6120 636f   Incurs extra co
+00002e20: 7374 732e 0d0a 2d20 6074 6578 745f 6f6e  sts...- `text_on
+00002e30: 6c79 6020 286f 7074 696f 6e61 6c29 3a20  ly` (optional): 
+00002e40: 446f 206e 6f74 2065 7874 7261 6374 2069  Do not extract i
+00002e50: 6d61 6765 7320 6672 6f6d 2064 6f63 756d  mages from docum
+00002e60: 656e 7473 206f 7220 7765 6273 6974 6573  ents or websites
+00002e70: 2e20 4164 6469 7469 6f6e 616c 6c79 2c20  . Additionally, 
+00002e80: 696d 6167 6520 6669 6c65 7320 7769 6c6c  image files will
+00002e90: 2062 6520 7265 7072 6573 656e 7465 6420   be represented 
+00002ea0: 7769 7468 204f 4352 2069 6e73 7465 6164  with OCR instead
+00002eb0: 206f 6620 6173 2069 6d61 6765 732e 0d0a   of as images...
+00002ec0: 0d0a 2320 5370 6f6e 736f 7273 0d0a 0d0a  ..# Sponsors....
+00002ed0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00002ee0: 2f63 616c 2e63 6f6d 2f65 6d6d 6574 742d  /cal.com/emmett-
+00002ef0: 6d63 662f 3330 6d69 6e22 3e3c 696d 6720  mcf/30min"><img 
+00002f00: 616c 743d 2242 6f6f 6b20 7573 2077 6974  alt="Book us wit
+00002f10: 6820 4361 6c2e 636f 6d22 2073 7263 3d22  h Cal.com" src="
+00002f20: 6874 7470 733a 2f2f 6361 6c2e 636f 6d2f  https://cal.com/
+00002f30: 626f 6f6b 2d77 6974 682d 6361 6c2d 6461  book-with-cal-da
+00002f40: 726b 2e73 7667 2220 2f3e 3c2f 613e 0d0a  rk.svg" /></a>..
+00002f50: 0d0a 5468 616e 6b20 796f 7520 746f 205b  ..Thank you to [
+00002f60: 4361 6c2e 636f 6d5d 2868 7474 7073 3a2f  Cal.com](https:/
+00002f70: 2f63 616c 2e63 6f6d 2f29 2066 6f72 2073  /cal.com/) for s
+00002f80: 706f 6e73 6f72 696e 6720 7468 6973 2070  ponsoring this p
+00002f90: 726f 6a65 6374 2e20 436f 6e74 6163 7420  roject. Contact 
+00002fa0: 656d 6d65 7474 4074 6865 7069 2e70 6520  emmett@thepi.pe 
+00002fb0: 666f 7220 7370 6f6e 736f 7273 6869 7020  for sponsorship 
+00002fc0: 696e 666f 726d 6174 696f 6e2e            information.
```

