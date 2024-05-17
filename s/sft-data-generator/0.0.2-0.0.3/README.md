# Comparing `tmp/sft-data-generator-0.0.2.tar.gz` & `tmp/sft-data-generator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sft-data-generator-0.0.2.tar", last modified: Wed May 15 12:16:09 2024, max compression
+gzip compressed data, was "sft-data-generator-0.0.3.tar", last modified: Fri May 17 05:12:21 2024, max compression
```

## Comparing `sft-data-generator-0.0.2.tar` & `sft-data-generator-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 12:16:09.371271 sft-data-generator-0.0.2/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1063 2024-05-15 10:04:42.000000 sft-data-generator-0.0.2/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-15 10:04:42.000000 sft-data-generator-0.0.2/MANIFEST.in
--rw-r--r--   0 codespace  (1000) codespace  (1000)     3159 2024-05-15 12:16:09.371271 sft-data-generator-0.0.2/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2479 2024-05-15 10:04:42.000000 sft-data-generator-0.0.2/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      778 2024-05-15 12:16:09.371271 sft-data-generator-0.0.2/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      296 2024-05-15 12:12:35.000000 sft-data-generator-0.0.2/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 12:16:09.363271 sft-data-generator-0.0.2/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 12:16:09.367271 sft-data-generator-0.0.2/src/sft_data_generator/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       92 2024-05-15 10:04:42.000000 sft-data-generator-0.0.2/src/sft_data_generator/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9076 2024-05-15 11:41:21.000000 sft-data-generator-0.0.2/src/sft_data_generator/main.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 12:16:09.371271 sft-data-generator-0.0.2/src/sft_data_generator.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     3159 2024-05-15 12:16:09.000000 sft-data-generator-0.0.2/src/sft_data_generator.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      411 2024-05-15 12:16:09.000000 sft-data-generator-0.0.2/src/sft_data_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-15 12:16:09.000000 sft-data-generator-0.0.2/src/sft_data_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       68 2024-05-15 12:16:09.000000 sft-data-generator-0.0.2/src/sft_data_generator.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      110 2024-05-15 12:16:09.000000 sft-data-generator-0.0.2/src/sft_data_generator.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       19 2024-05-15 12:16:09.000000 sft-data-generator-0.0.2/src/sft_data_generator.egg-info/top_level.txt
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 12:16:09.371271 sft-data-generator-0.0.2/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       91 2024-05-15 10:04:42.000000 sft-data-generator-0.0.2/tests/test_main.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 05:12:21.396856 sft-data-generator-0.0.3/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1063 2024-05-15 10:04:42.000000 sft-data-generator-0.0.3/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-15 10:04:42.000000 sft-data-generator-0.0.3/MANIFEST.in
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     3473 2024-05-17 05:12:21.396856 sft-data-generator-0.0.3/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2824 2024-05-17 05:10:57.000000 sft-data-generator-0.0.3/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      761 2024-05-17 05:12:21.396856 sft-data-generator-0.0.3/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      296 2024-05-17 05:07:01.000000 sft-data-generator-0.0.3/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 05:12:21.388856 sft-data-generator-0.0.3/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 05:12:21.392856 sft-data-generator-0.0.3/src/sft_data_generator/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       92 2024-05-15 10:04:42.000000 sft-data-generator-0.0.3/src/sft_data_generator/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9204 2024-05-17 05:08:04.000000 sft-data-generator-0.0.3/src/sft_data_generator/main.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 05:12:21.392856 sft-data-generator-0.0.3/src/sft_data_generator.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     3473 2024-05-17 05:12:21.000000 sft-data-generator-0.0.3/src/sft_data_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      411 2024-05-17 05:12:21.000000 sft-data-generator-0.0.3/src/sft_data_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-17 05:12:21.000000 sft-data-generator-0.0.3/src/sft_data_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       68 2024-05-17 05:12:21.000000 sft-data-generator-0.0.3/src/sft_data_generator.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       94 2024-05-17 05:12:21.000000 sft-data-generator-0.0.3/src/sft_data_generator.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       19 2024-05-17 05:12:21.000000 sft-data-generator-0.0.3/src/sft_data_generator.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 05:12:21.392856 sft-data-generator-0.0.3/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       91 2024-05-15 10:04:42.000000 sft-data-generator-0.0.3/tests/test_main.py
```

### Comparing `sft-data-generator-0.0.2/LICENSE` & `sft-data-generator-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sft-data-generator-0.0.2/PKG-INFO` & `sft-data-generator-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: sft-data-generator
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool for generating data for SFT using LLM
 Home-page: https://github.com/Treedy2020/sft_data_generator
 Author: Richard_Cui
 Author-email: treedy2020@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai~=1.13.3
 Requires-Dist: pandas~=2.2.1
 Requires-Dist: jsonlines~=4.0.0
-Requires-Dist: filetype~=1.2.0
 Requires-Dist: tqdm~=4.66.2
 Requires-Dist: setuptools~=68.2.2
 Requires-Dist: openpyxl~=3.1.2
 
 # SFT Data Generator
 
 This is a tool for generating data for Supervised Fine-Tuning (SFT) using large language models like GPT-3.5. It can read data from CSV or Excel files and generate corresponding output data using OpenAI's API based on a given prompt.
@@ -40,16 +39,19 @@
    ```
    pip install -r requirements.txt
    ```
 
 2. Prepare the input data file (CSV or Excel) and prompt template.
 
 3. Run the command:
-
+   ```bash
+   sft-data-generator --file_path <input_file_path> --prompt <prompt_template> --model <model_name> [other optional arguments]
    ```
+   or
+   ```bash
    python data_generator.py --file_path <input_file_path> --prompt <prompt_template> --model <model_name> [other optional arguments]
    ```
 
    Required arguments:
    - `--file_path`: Path to the input data file, must be a CSV or Excel file.
    - `--prompt`: Prompt template used for generating data.
    - `--model`: Name of the OpenAI model used for generating data, e.g., `gpt-3.5-turbo`.
@@ -62,12 +64,16 @@
    - `--openai_api_key`: OpenAI API key, if not given, will use the environment variable `OPENAI_API_KEY`.
    - `--json_output`: Whether to use JSON format output, defaults to False.
 
 4. The generated data will be saved in the specified output file, with each line being a JSON object.
 
 ## Example
 
+```bash
+sft-data-generator --file_path data.csv --prompt "Please generate a question-answer pair based on the given data:" --model gpt-3.5-turbo --batch_size 10 --generate_epoch 3
 ```
+or
+```bash
 python data_generator.py --file_path data.csv --prompt "Please generate a question-answer pair based on the given data:" --model gpt-3.5-turbo --batch_size 10 --generate_epoch 3
 ```
 
 This will read the `data.csv` file, use the prompt "Please generate a question-answer pair based on the given data:", call the `gpt-3.5-turbo` model with a batch size of 10, and generate 3 epochs of data. The output will be saved in the `data.csv.output.jsonl` file.
```

### Comparing `sft-data-generator-0.0.2/README.md` & `sft-data-generator-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -19,16 +19,19 @@
    ```
    pip install -r requirements.txt
    ```
 
 2. Prepare the input data file (CSV or Excel) and prompt template.
 
 3. Run the command:
-
+   ```bash
+   sft-data-generator --file_path <input_file_path> --prompt <prompt_template> --model <model_name> [other optional arguments]
    ```
+   or
+   ```bash
    python data_generator.py --file_path <input_file_path> --prompt <prompt_template> --model <model_name> [other optional arguments]
    ```
 
    Required arguments:
    - `--file_path`: Path to the input data file, must be a CSV or Excel file.
    - `--prompt`: Prompt template used for generating data.
    - `--model`: Name of the OpenAI model used for generating data, e.g., `gpt-3.5-turbo`.
@@ -41,12 +44,16 @@
    - `--openai_api_key`: OpenAI API key, if not given, will use the environment variable `OPENAI_API_KEY`.
    - `--json_output`: Whether to use JSON format output, defaults to False.
 
 4. The generated data will be saved in the specified output file, with each line being a JSON object.
 
 ## Example
 
+```bash
+sft-data-generator --file_path data.csv --prompt "Please generate a question-answer pair based on the given data:" --model gpt-3.5-turbo --batch_size 10 --generate_epoch 3
 ```
+or
+```bash
 python data_generator.py --file_path data.csv --prompt "Please generate a question-answer pair based on the given data:" --model gpt-3.5-turbo --batch_size 10 --generate_epoch 3
 ```
 
 This will read the `data.csv` file, use the prompt "Please generate a question-answer pair based on the given data:", call the `gpt-3.5-turbo` model with a batch size of 10, and generate 3 epochs of data. The output will be saved in the `data.csv.output.jsonl` file.
```

### Comparing `sft-data-generator-0.0.2/setup.cfg` & `sft-data-generator-0.0.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 package_dir = 
 	= src
 packages = find:
 install_requires = 
 	openai~=1.13.3
 	pandas~=2.2.1
 	jsonlines~=4.0.0
-	filetype~=1.2.0
 	tqdm~=4.66.2
 	setuptools~=68.2.2
 	openpyxl~=3.1.2
 python_requires = >=3.8
 
 [options.entry_points]
 console_scripts =
```

### Comparing `sft-data-generator-0.0.2/src/sft_data_generator/main.py` & `sft-data-generator-0.0.3/src/sft_data_generator/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,50 +46,58 @@
                 log_level (str, optional): The log level for the logger. Defaults to "WARNING".
                 output_file (str, optional): The path to the output file. If not provided, a default output file will be created.
                 sheet_names (List[str], optional): The names of the sheets to be read from an xlsx file. If not provided, all sheets will be read.
                 openai_base_url (str, optional): The base URL for the OpenAI API. If not provided, the value from the environment variable OPENAI_API_BASE will be used.
                 openai_api_key (str, optional): The API key for the OpenAI API. If not provided, the value from the environment variable OPENAI_API_KEY will be used.
             """
             self.set_logger(log_level)
-
-            kind = filetype.guess(file_path)
-            assert kind is not None and kind.extension in ['csv', 'xlsx'], \
-                f"File path should be a csv or xlsx file, but got {kind.extension} file."
-            if kind.extension == 'csv':
+            try:
                 self.data = pd.read_csv(file_path)
-            else:
+            except Exception as e:
                 if (sheet_names is None) or ("all" in [x.lower() for x in sheet_names]):
                     xls = pd.ExcelFile(file_path)
                     sheet_names = xls.sheet_names
-                    self.logger.warning(f"No special sheet name was set for xlsx file, use all sheet: {sheet_names}.")
+                    self.logger.warning(f"No special sheet name was set for xlsx file, use all sheets: {sheet_names}.")
                 self.data = pd.concat([pd.read_excel(file_path, sheet_name) for sheet_name in sheet_names])
 
             self.output_file = output_file if output_file is not None else file_path + '.output.jsonl'
             self.client = AsyncClient(
                 base_url=openai_base_url if openai_base_url is not None else os.environ.get("OPENAI_API_BASE"),
                 api_key=openai_api_key if openai_api_key is not None else os.environ.get("OPENAI_API_KEY")
             )
             self.prompt = prompt
             self.model = model
             self.batch_size = batch_size
             self.json_output = {"type": "json_object"} if json_output else NOT_GIVEN
             self.generate_epoch = generate_epoch
 
     def set_logger(self, log_level: str):
-        self.logger = logging.getLogger(__name__)
-        formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-        handler = logging.StreamHandler()
-        handler.setFormatter(formatter)
-        handler_log_level = getattr(logging, log_level, None)
-
-        if not isinstance(handler_log_level, int):
-            raise ValueError('Invalid log level: {}'.format(log_level))
-        handler.setLevel(handler_log_level)
+            """
+            Sets up the logger for the class.
+
+            Args:
+                log_level (str): The desired log level for the logger.
+
+            Raises:
+                ValueError: If an invalid log level is provided.
+
+            Returns:
+                None
+            """
+            self.logger = logging.getLogger(__name__)
+            formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+            handler = logging.StreamHandler()
+            handler.setFormatter(formatter)
+            handler_log_level = getattr(logging, log_level, None)
+
+            if not isinstance(handler_log_level, int):
+                raise ValueError('Invalid log level: {}'.format(log_level))
+            handler.setLevel(handler_log_level)
 
-        self.logger.addHandler(handler)
+            self.logger.addHandler(handler)
 
 
     # TODO Add the retry decorator for the get_data_sample function.
     async def get_data_sample(self, row_data: dict) -> dict | None:
         """
         Retrieves a data sample by generating a response using the OpenAI GPT model.
 
@@ -112,15 +120,15 @@
             )
             full_response = response.choices[0].message.content
             row_data['gpt-response'] = full_response
             self.logger.info(f"A response was generated by GPT:\n {full_response}")
             return row_data
         except openai.OpenAIError as e:
             self.logger.error(f"An error occurred when trying to get OpenAI response. "
-                                "Please check the RPM/TPM or account balance if you encounter this error: {e}")
+                              f"Please check the RPM/TPM or account balance or other info if you encounter this error: {e}")
             return None
 
     async def main_loop(self) -> None:
             """
             Executes the main loop for data generation.
 
             This method iterates over the data and generates samples in batches. The generated data is written to an output file.
```

### Comparing `sft-data-generator-0.0.2/src/sft_data_generator.egg-info/PKG-INFO` & `sft-data-generator-0.0.3/src/sft_data_generator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: sft-data-generator
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool for generating data for SFT using LLM
 Home-page: https://github.com/Treedy2020/sft_data_generator
 Author: Richard_Cui
 Author-email: treedy2020@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai~=1.13.3
 Requires-Dist: pandas~=2.2.1
 Requires-Dist: jsonlines~=4.0.0
-Requires-Dist: filetype~=1.2.0
 Requires-Dist: tqdm~=4.66.2
 Requires-Dist: setuptools~=68.2.2
 Requires-Dist: openpyxl~=3.1.2
 
 # SFT Data Generator
 
 This is a tool for generating data for Supervised Fine-Tuning (SFT) using large language models like GPT-3.5. It can read data from CSV or Excel files and generate corresponding output data using OpenAI's API based on a given prompt.
@@ -40,16 +39,19 @@
    ```
    pip install -r requirements.txt
    ```
 
 2. Prepare the input data file (CSV or Excel) and prompt template.
 
 3. Run the command:
-
+   ```bash
+   sft-data-generator --file_path <input_file_path> --prompt <prompt_template> --model <model_name> [other optional arguments]
    ```
+   or
+   ```bash
    python data_generator.py --file_path <input_file_path> --prompt <prompt_template> --model <model_name> [other optional arguments]
    ```
 
    Required arguments:
    - `--file_path`: Path to the input data file, must be a CSV or Excel file.
    - `--prompt`: Prompt template used for generating data.
    - `--model`: Name of the OpenAI model used for generating data, e.g., `gpt-3.5-turbo`.
@@ -62,12 +64,16 @@
    - `--openai_api_key`: OpenAI API key, if not given, will use the environment variable `OPENAI_API_KEY`.
    - `--json_output`: Whether to use JSON format output, defaults to False.
 
 4. The generated data will be saved in the specified output file, with each line being a JSON object.
 
 ## Example
 
+```bash
+sft-data-generator --file_path data.csv --prompt "Please generate a question-answer pair based on the given data:" --model gpt-3.5-turbo --batch_size 10 --generate_epoch 3
 ```
+or
+```bash
 python data_generator.py --file_path data.csv --prompt "Please generate a question-answer pair based on the given data:" --model gpt-3.5-turbo --batch_size 10 --generate_epoch 3
 ```
 
 This will read the `data.csv` file, use the prompt "Please generate a question-answer pair based on the given data:", call the `gpt-3.5-turbo` model with a batch size of 10, and generate 3 epochs of data. The output will be saved in the `data.csv.output.jsonl` file.
```

