# Comparing `tmp/omop2survey-0.0.3.tar.gz` & `tmp/omop2survey-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omop2survey-0.0.3.tar", max compression
+gzip compressed data, was "omop2survey-0.0.4.tar", max compression
```

## Comparing `omop2survey-0.0.3.tar` & `omop2survey-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0     5296 2024-05-14 21:03:51.967987 omop2survey-0.0.3/README.md
--rw-r--r--   0        0        0      277 2024-05-14 21:03:51.980323 omop2survey-0.0.3/omop2survey/__init__.py
--rw-r--r--   0        0        0     4077 2024-05-14 20:57:26.446629 omop2survey-0.0.3/omop2survey/codebooks.py
--rw-r--r--   0        0        0     1570 2024-05-14 22:11:42.948443 omop2survey-0.0.3/omop2survey/pivot_data.py
--rw-r--r--   0        0        0      872 2024-05-11 22:10:49.324160 omop2survey-0.0.3/omop2survey/recode_missing.py
--rw-r--r--   0        0        0     7435 2024-05-14 23:18:11.071781 omop2survey-0.0.3/omop2survey/response_set.py
--rw-r--r--   0        0        0  1172489 2024-05-10 03:42:23.460428 omop2survey-0.0.3/omop2survey/survey_key.csv
--rw-r--r--   0        0        0      725 2024-05-15 03:34:18.106614 omop2survey-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6315 1970-01-01 00:00:00.000000 omop2survey-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     5296 2024-05-14 21:03:51.967987 omop2survey-0.0.4/README.md
+-rw-r--r--   0        0        0     6148 2024-05-17 04:16:32.815544 omop2survey-0.0.4/omop2survey/.DS_Store
+-rw-r--r--   0        0        0      323 2024-05-17 03:55:13.603705 omop2survey-0.0.4/omop2survey/__init__.py
+-rw-r--r--   0        0        0     6059 2024-05-17 03:55:13.579601 omop2survey-0.0.4/omop2survey/codebooks.py
+-rw-r--r--   0        0        0      571 2024-05-17 04:31:31.601715 omop2survey-0.0.4/omop2survey/hash_csv.py
+-rw-r--r--   0        0        0     2801 2024-05-17 03:52:36.052302 omop2survey-0.0.4/omop2survey/pivot_data.py
+-rw-r--r--   0        0        0      872 2024-05-17 03:49:20.928260 omop2survey-0.0.4/omop2survey/recode_missing.py
+-rw-r--r--   0        0        0     7434 2024-05-17 03:55:13.607873 omop2survey-0.0.4/omop2survey/response_set.py
+-rw-r--r--   0        0        0  1172489 2024-05-10 03:42:23.460428 omop2survey-0.0.4/omop2survey/survey_key.csv
+-rw-r--r--   0        0        0       64 2024-05-17 04:31:33.436399 omop2survey-0.0.4/omop2survey/survey_key_hash.txt
+-rw-r--r--   0        0        0      828 2024-05-17 04:39:02.850743 omop2survey-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6315 1970-01-01 00:00:00.000000 omop2survey-0.0.4/PKG-INFO
```

### Comparing `omop2survey-0.0.3/README.md` & `omop2survey-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `omop2survey-0.0.3/omop2survey/codebooks.py` & `omop2survey-0.0.4/omop2survey/codebooks.py`

 * *Files 26% similar despite different names*

```diff
@@ -118,7 +118,60 @@
     temp = formatted_codebook_df.to_html(index=False, escape=False)
     with open(file_path, 'w') as f:
         f.write(temp)
     display(FileLink(file_path))
     display(HTML(temp))
 
     return
+
+
+def codebook_html(input_data):
+    input_data['question'] = input_data['question'].str.strip().str.lower()
+    input_data['answer'] = input_data['answer'].str.strip().str.lower()
+
+    input_data = input_data.drop_duplicates(subset=['question_concept_id', 'question', 'answer_concept_id'])
+
+    grouped = input_data.groupby(['question_concept_id', 'question'], sort=False)
+
+    formatted_data = []
+
+    for (question_concept_id, question), group in grouped:
+        is_first = True
+
+        for idx, row in group.iterrows():
+            if is_first:
+                formatted_data.append({
+                    'question_concept_id': question_concept_id,
+                    'question': question,
+                    'answer_concept_id': row['answer_concept_id'],
+                    'answer_concept_id recoded as answer_numeric': row['answer_numeric'],
+                    'answer': row['answer'],
+                    'answer recoded as answer_text': row['answer_text']
+                })
+                is_first = False
+            else:
+                formatted_data.append({
+                    'question_concept_id': '',
+                    'question': '',
+                    'answer_concept_id': row['answer_concept_id'],
+                    'answer_concept_id recoded as answer_numeric': row['answer_numeric'],
+                    'answer': row['answer'],
+                    'answer recoded as answer_text': row['answer_text']
+                })
+
+    formatted_codebook_df = pd.DataFrame(formatted_data)
+
+    current_time = datetime.now().strftime("%Y%m%d_%H%M%S")
+
+    file_name = f'codebook_{current_time}.html'
+    workspace_dir = os.path.join(os.getcwd(), 'workspace')
+    os.makedirs(workspace_dir, exist_ok=True)
+    file_path = os.path.join(workspace_dir, file_name)
+
+    temp = formatted_codebook_df.to_html(index=False, escape=False)
+    with open(file_path, 'w') as f:
+        f.write(temp)
+
+    display(FileLink(file_path))
+    display(HTML(temp))
+
+    return
```

### Comparing `omop2survey-0.0.3/omop2survey/pivot_data.py` & `omop2survey-0.0.4/omop2survey/pivot_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,7 +32,37 @@
     args = ["gsutil", "cp", f"./{file_name}", f"{my_bucket}/data/"]
     output = subprocess.run(args, capture_output=True)
     if output.returncode == 0:
         print(f"Pivoted dataset with numeric values saved and uploaded successfully to: {my_bucket}/data/{file_name}")
     else:
         print("Failed to upload the file:", output.stderr.decode())
 
+def pivot_local(data, file_name='pivot_n.csv'):
+    pivot_df = data.pivot_table(index='person_id',
+                                columns='question_concept_id',
+                                values='answer_numeric',
+                                aggfunc='first')
+
+    pivot_df.columns = ['q' + str(col) for col in pivot_df.columns]
+    workspace_dir = os.path.join(os.getcwd(), 'workspace')
+    os.makedirs(workspace_dir, exist_ok=True)
+    file_path = os.path.join(workspace_dir, file_name)
+
+    pivot_df.to_csv(file_path)
+
+    print(f"Pivoted dataset with numeric values saved successfully to: {file_path}")
+
+
+def pivot_text_local(data, file_name='pivot_t.csv'):
+    pivot_df = data.pivot_table(index='person_id',
+                                columns='question_concept_id',
+                                values='answer_text',
+                                aggfunc='first')
+
+    pivot_df.columns = ['q' + str(col) for col in pivot_df.columns]
+    workspace_dir = os.path.join(os.getcwd(), 'workspace')
+    os.makedirs(workspace_dir, exist_ok=True)
+    file_path = os.path.join(workspace_dir, file_name)
+
+    pivot_df.to_csv(file_path)
+
+    print(f"Pivoted dataset with text values saved successfully to: {file_path}")
```

### Comparing `omop2survey-0.0.3/omop2survey/recode_missing.py` & `omop2survey-0.0.4/omop2survey/recode_missing.py`

 * *Files identical despite different names*

### Comparing `omop2survey-0.0.3/omop2survey/response_set.py` & `omop2survey-0.0.4/omop2survey/response_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,14 @@
     if method == 'mean':
         df[scale_name] = df[variables].mean(axis=1)
     elif method == 'sum':
         df[scale_name] = df[variables].sum(axis=1)
 
     data = pd.merge(data, df[['person_id', scale_name]], on='person_id', how='left')
 
-
     print('Minimum score calculated:', df[scale_name].min())
     print('Maximum score calculated:', df[scale_name].max())
     print('Number of person_ids with NaN assigned:', data[scale_name].isna().sum())
     print('Number of person_ids with score calculated:', data[scale_name].notna().sum())
 
     return data
```

### Comparing `omop2survey-0.0.3/omop2survey/survey_key.csv` & `omop2survey-0.0.4/omop2survey/survey_key.csv`

 * *Files identical despite different names*

### Comparing `omop2survey-0.0.3/pyproject.toml` & `omop2survey-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 [tool.poetry]
 name = "omop2survey"
-version = "0.0.3"
+version = "0.0.4"
 description = "The 'omop2survey' Python package transforms standardized response codes from the OMOP CDM survey variables into numeric values and simplifies data preparation by providing functionalities for mapping and converting response codes, as well as handling missing data, facilitating easier and more reliable data analysis."
 authors = ["Elif Dede Yildirim <elifdy@auburn.edu>"]
 repository = "https://github.com/elifdy/omop2survey.git"
 license = "MIT"
 readme = "README.md"
+include = ["omop2survey/survey_key.csv"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.2.2"
 tabulate = "^0.9.0"
 openpyxl = "^3.1.2"
 
 
 
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
+[tool.poetry.scripts]
+hash_csv = "omop2survey.hash_csv:main"
```

### Comparing `omop2survey-0.0.3/PKG-INFO` & `omop2survey-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omop2survey
-Version: 0.0.3
+Version: 0.0.4
 Summary: The 'omop2survey' Python package transforms standardized response codes from the OMOP CDM survey variables into numeric values and simplifies data preparation by providing functionalities for mapping and converting response codes, as well as handling missing data, facilitating easier and more reliable data analysis.
 Home-page: https://github.com/elifdy/omop2survey.git
 License: MIT
 Author: Elif Dede Yildirim
 Author-email: elifdy@auburn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

