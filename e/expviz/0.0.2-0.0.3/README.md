# Comparing `tmp/expviz-0.0.2.tar.gz` & `tmp/expviz-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expviz-0.0.2.tar", last modified: Thu Mar 14 20:23:53 2024, max compression
+gzip compressed data, was "expviz-0.0.3.tar", last modified: Fri May 17 17:36:01 2024, max compression
```

## Comparing `expviz-0.0.2.tar` & `expviz-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwx------   0 zihao.fu (672210089) domain users (672200513)        0 2024-03-14 20:23:53.158495 expviz-0.0.2/
--rw-r--r--   0 zihao.fu (672210089) domain users (672200513)     3670 2024-03-14 20:23:53.158495 expviz-0.0.2/PKG-INFO
--rw-------   0 zihao.fu (672210089) domain users (672200513)     3359 2024-03-14 18:00:19.000000 expviz-0.0.2/README.md
-drwx------   0 zihao.fu (672210089) domain users (672200513)        0 2024-03-14 20:23:53.158495 expviz-0.0.2/expviz/
--rw-------   0 zihao.fu (672210089) domain users (672200513)       66 2024-03-14 18:00:19.000000 expviz-0.0.2/expviz/__init__.py
--rw-------   0 zihao.fu (672210089) domain users (672200513)     6631 2024-03-14 18:04:44.000000 expviz-0.0.2/expviz/expviz.py
--rw-------   0 zihao.fu (672210089) domain users (672200513)       21 2024-03-14 20:22:39.000000 expviz-0.0.2/expviz/version.py
-drwx------   0 zihao.fu (672210089) domain users (672200513)        0 2024-03-14 20:23:53.158495 expviz-0.0.2/expviz.egg-info/
--rw-r--r--   0 zihao.fu (672210089) domain users (672200513)     3670 2024-03-14 20:23:53.000000 expviz-0.0.2/expviz.egg-info/PKG-INFO
--rw-------   0 zihao.fu (672210089) domain users (672200513)      234 2024-03-14 20:23:53.000000 expviz-0.0.2/expviz.egg-info/SOURCES.txt
--rw-------   0 zihao.fu (672210089) domain users (672200513)        1 2024-03-14 20:23:53.000000 expviz-0.0.2/expviz.egg-info/dependency_links.txt
--rw-------   0 zihao.fu (672210089) domain users (672200513)       11 2024-03-14 20:23:53.000000 expviz-0.0.2/expviz.egg-info/requires.txt
--rw-------   0 zihao.fu (672210089) domain users (672200513)        7 2024-03-14 20:23:53.000000 expviz-0.0.2/expviz.egg-info/top_level.txt
--rw-------   0 zihao.fu (672210089) domain users (672200513)       38 2024-03-14 20:23:53.158495 expviz-0.0.2/setup.cfg
--rw-------   0 zihao.fu (672210089) domain users (672200513)      738 2024-03-14 20:22:20.000000 expviz-0.0.2/setup.py
-drwx------   0 zihao.fu (672210089) domain users (672200513)        0 2024-03-14 20:23:53.158495 expviz-0.0.2/test/
--rw-------   0 zihao.fu (672210089) domain users (672200513)     1381 2024-03-14 18:00:19.000000 expviz-0.0.2/test/test.py
+drwx------   0 zihao.fu (672210089) domain users (672200513)        0 2024-05-17 17:36:01.585940 expviz-0.0.3/
+-rw-r--r--   0 zihao.fu (672210089) domain users (672200513)     3670 2024-05-17 17:36:01.585940 expviz-0.0.3/PKG-INFO
+-rw-------   0 zihao.fu (672210089) domain users (672200513)     3359 2024-03-14 18:00:19.000000 expviz-0.0.3/README.md
+drwx------   0 zihao.fu (672210089) domain users (672200513)        0 2024-05-17 17:36:01.585940 expviz-0.0.3/expviz/
+-rw-------   0 zihao.fu (672210089) domain users (672200513)       66 2024-03-14 18:00:19.000000 expviz-0.0.3/expviz/__init__.py
+-rw-------   0 zihao.fu (672210089) domain users (672200513)     7842 2024-05-17 17:31:57.000000 expviz-0.0.3/expviz/expviz.py
+-rw-------   0 zihao.fu (672210089) domain users (672200513)       22 2024-05-17 17:31:57.000000 expviz-0.0.3/expviz/version.py
+drwx------   0 zihao.fu (672210089) domain users (672200513)        0 2024-05-17 17:36:01.585940 expviz-0.0.3/expviz.egg-info/
+-rw-r--r--   0 zihao.fu (672210089) domain users (672200513)     3670 2024-05-17 17:36:01.000000 expviz-0.0.3/expviz.egg-info/PKG-INFO
+-rw-------   0 zihao.fu (672210089) domain users (672200513)      234 2024-05-17 17:36:01.000000 expviz-0.0.3/expviz.egg-info/SOURCES.txt
+-rw-------   0 zihao.fu (672210089) domain users (672200513)        1 2024-05-17 17:36:01.000000 expviz-0.0.3/expviz.egg-info/dependency_links.txt
+-rw-------   0 zihao.fu (672210089) domain users (672200513)       11 2024-05-17 17:36:01.000000 expviz-0.0.3/expviz.egg-info/requires.txt
+-rw-------   0 zihao.fu (672210089) domain users (672200513)        7 2024-05-17 17:36:01.000000 expviz-0.0.3/expviz.egg-info/top_level.txt
+-rw-------   0 zihao.fu (672210089) domain users (672200513)       38 2024-05-17 17:36:01.585940 expviz-0.0.3/setup.cfg
+-rw-------   0 zihao.fu (672210089) domain users (672200513)      738 2024-03-14 20:22:20.000000 expviz-0.0.3/setup.py
+drwx------   0 zihao.fu (672210089) domain users (672200513)        0 2024-05-17 17:36:01.585940 expviz-0.0.3/test/
+-rw-------   0 zihao.fu (672210089) domain users (672200513)     1381 2024-03-14 18:00:19.000000 expviz-0.0.3/test/test.py
```

### Comparing `expviz-0.0.2/PKG-INFO` & `expviz-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expviz
-Version: 0.0.2
+Version: 0.0.3
 Summary: Visualize experiments tables and figures.
 Home-page: https://github.com/fuzihaofzh/expviz
 Author: 
 Author-email: 
 Keywords: Shell env
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
```

### Comparing `expviz-0.0.2/README.md` & `expviz-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `expviz-0.0.2/expviz/expviz.py` & `expviz-0.0.3/expviz/expviz.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,86 @@
 import pandas as pd
 from tabulate import tabulate
 from IPython.display import display, HTML
 import os
 import json
 import numpy as np
 import matplotlib.pyplot as plt
+import copy 
 
 # Set global display options
 pd.set_option('display.max_colwidth', None)
 pd.set_option('display.width', None)
 
+def format_with_specified_pattern(number, pattern):
+    formatted_number = pattern.format(number)
+    
+    # 分离整数和小数部分
+    if '.' in formatted_number:
+        integer_part, fractional_part = formatted_number.split('.')
+    else:
+        integer_part, fractional_part = formatted_number, ''
+    
+    # 计算总有效数字个数
+    significant_digits = len(integer_part.replace('-', '')) + len(fractional_part)
+    
+    # 补齐零
+    if significant_digits < 3:
+        if '.' not in formatted_number:
+            formatted_number += '.'
+        formatted_number += '0' * (3 - significant_digits)
+    
+    return formatted_number
+
 # Function to convert nested dictionary to DataFrame
-def dict_to_dataframe(data, fmt='{:,.3g}', transpose = False, bold_col_max = False, bold_col_max_exclude_rows = []):
+def dict_to_dataframe(data, fmt='{:,.3g}', transpose = False, bold_col_max = False, bold_col_max_exclude_rows = [], cell_transform = lambda x : x):
+    data = copy.deepcopy(data)
     for exp in data:
         for metric in data[exp]:
             try:
-                data[exp][metric] = fmt.format(data[exp][metric])
+                data[exp][metric] = format_with_specified_pattern(cell_transform(data[exp][metric]), fmt) if type(data[exp][metric]) is float else data[exp][metric]
             except:
                 pass
     df = pd.DataFrame(data).T
     if transpose:
         df = df.T
     if bold_col_max:
         # Define the rows to be excluded from the max calculation
         exclude_rows = bold_col_max_exclude_rows
 
         # Function to apply LaTeX bold formatting to the max value in a Series excluding specified rows
         def apply_latex_bold_exclude(s):
+            # Convert to numeric and ignore errors; non-numeric become NaN
+            numeric_s = pd.to_numeric(s, errors='coerce')
+    
             # Exclude specified rows from max calculation
-            max_val = s.drop(index=exclude_rows).max()
-            return [f"\\textbf{{{val}}}" if val == max_val and idx not in exclude_rows else str(val) for idx, val in enumerate(s)]
+            max_val = numeric_s.drop(index=exclude_rows).max()
+            
+            # Apply LaTeX bold formatting to the max value if it's not in the excluded rows and is a number
+            # Keep the original string if it's NaN or non-numeric
+            return [f"\\textbf{{{val}}}" if idx not in exclude_rows and pd.notnull(numeric_s[idx]) and val == max_val else s[idx] for idx, val in enumerate(numeric_s)]
         df = df.apply(apply_latex_bold_exclude)
     return df
 
 # Function to convert DataFrame to LaTeX
 def to_latex(data, fmt='{:,.3g}', transpose=False, escape=None, **kwargs):
     df = dict_to_dataframe(data, fmt = fmt, transpose = transpose, **kwargs)
     latex_code = df.to_latex(escape=escape)
     
     # Fit the LaTeX table into the template
     table_tmp = """\\begin{table}[t]
     \\centering
     \\scriptsize
     
     %s
-    
     \caption{Caption Title.}
     \label{tab:tablename}
-    \end{table}
+\end{table}
     """
-    return table_tmp % latex_code
+    return table_tmp % latex_code.replace("\n", "\n    ")
 
 # Function to convert DataFrame to Markdown
 def to_markdown(data, fmt='{:,.3g}', transpose=False):
     df = dict_to_dataframe(data, fmt = fmt, transpose = transpose)
     markdown_table = tabulate(df, tablefmt="pipe", headers="keys")
     return markdown_table
 
@@ -160,8 +187,8 @@
     plt.legend(labelspacing=0)
     plt.grid(True, linestyle='--')
     
     # Save and show the plot
     plt.tight_layout()
     if save_path:
         plt.savefig(save_path, bbox_inches='tight')
-    plt.show()
+    plt.show()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `expviz-0.0.2/expviz.egg-info/PKG-INFO` & `expviz-0.0.3/expviz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expviz
-Version: 0.0.2
+Version: 0.0.3
 Summary: Visualize experiments tables and figures.
 Home-page: https://github.com/fuzihaofzh/expviz
 Author: 
 Author-email: 
 Keywords: Shell env
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
```

### Comparing `expviz-0.0.2/setup.py` & `expviz-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `expviz-0.0.2/test/test.py` & `expviz-0.0.3/test/test.py`

 * *Files identical despite different names*

