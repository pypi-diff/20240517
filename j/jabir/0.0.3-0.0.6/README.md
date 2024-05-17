# Comparing `tmp/jabir-0.0.3.tar.gz` & `tmp/jabir-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jabir-0.0.3.tar", last modified: Mon Jul 10 06:50:15 2023, max compression
+gzip compressed data, was "jabir-0.0.6.tar", last modified: Fri May 17 17:47:17 2024, max compression
```

## Comparing `jabir-0.0.3.tar` & `jabir-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 gashmard  (1001) gashmard  (1001)        0 2023-07-10 06:50:15.322894 jabir-0.0.3/
--rw-rw-r--   0 gashmard  (1001) gashmard  (1001)     1072 2023-05-22 14:45:10.000000 jabir-0.0.3/LICENSE
--rw-rw-r--   0 gashmard  (1001) gashmard  (1001)     1386 2023-07-10 06:50:15.322894 jabir-0.0.3/PKG-INFO
--rw-rw-r--   0 gashmard  (1001) gashmard  (1001)      912 2023-07-10 06:21:15.000000 jabir-0.0.3/README.md
-drwxrwxr-x   0 gashmard  (1001) gashmard  (1001)        0 2023-07-10 06:50:15.322894 jabir-0.0.3/jabir/
--rw-rw-r--   0 gashmard  (1001) gashmard  (1001)       42 2023-07-10 05:54:01.000000 jabir-0.0.3/jabir/__init__.py
--rw-rw-r--   0 gashmard  (1001) gashmard  (1001)   117327 2023-07-10 05:21:47.000000 jabir-0.0.3/jabir/jabir.py
-drwxrwxr-x   0 gashmard  (1001) gashmard  (1001)        0 2023-07-10 06:50:15.322894 jabir-0.0.3/jabir.egg-info/
--rw-rw-r--   0 gashmard  (1001) gashmard  (1001)     1386 2023-07-10 06:50:15.000000 jabir-0.0.3/jabir.egg-info/PKG-INFO
--rw-rw-r--   0 gashmard  (1001) gashmard  (1001)      175 2023-07-10 06:50:15.000000 jabir-0.0.3/jabir.egg-info/SOURCES.txt
--rw-rw-r--   0 gashmard  (1001) gashmard  (1001)        1 2023-07-10 06:50:15.000000 jabir-0.0.3/jabir.egg-info/dependency_links.txt
--rw-rw-r--   0 gashmard  (1001) gashmard  (1001)        6 2023-07-10 06:50:15.000000 jabir-0.0.3/jabir.egg-info/top_level.txt
--rw-rw-r--   0 gashmard  (1001) gashmard  (1001)       38 2023-07-10 06:50:15.322894 jabir-0.0.3/setup.cfg
--rw-rw-r--   0 gashmard  (1001) gashmard  (1001)      719 2023-07-10 06:43:31.000000 jabir-0.0.3/setup.py
+drwxrwxr-x   0 superuser  (1000) superuser  (1000)        0 2024-05-17 17:47:17.854188 jabir-0.0.6/
+-rw-r--r--   0 superuser  (1000) superuser  (1000)     1072 2024-05-17 17:35:22.000000 jabir-0.0.6/LICENSE
+-rw-r--r--   0 superuser  (1000) superuser  (1000)     1722 2024-05-17 17:47:17.850188 jabir-0.0.6/PKG-INFO
+-rw-r--r--   0 superuser  (1000) superuser  (1000)     1246 2024-05-17 17:34:47.000000 jabir-0.0.6/README.md
+drwxrwxr-x   0 superuser  (1000) superuser  (1000)        0 2024-05-17 17:47:17.850188 jabir-0.0.6/jabir/
+-rw-r--r--   0 superuser  (1000) superuser  (1000)       42 2024-05-17 17:08:28.000000 jabir-0.0.6/jabir/__init__.py
+-rw-r--r--   0 superuser  (1000) superuser  (1000)   122026 2024-05-17 17:11:02.000000 jabir-0.0.6/jabir/jabir.py
+drwxrwxr-x   0 superuser  (1000) superuser  (1000)        0 2024-05-17 17:47:17.850188 jabir-0.0.6/jabir.egg-info/
+-rw-r--r--   0 superuser  (1000) superuser  (1000)     1722 2024-05-17 17:47:17.000000 jabir-0.0.6/jabir.egg-info/PKG-INFO
+-rw-rw-r--   0 superuser  (1000) superuser  (1000)      175 2024-05-17 17:47:17.000000 jabir-0.0.6/jabir.egg-info/SOURCES.txt
+-rw-rw-r--   0 superuser  (1000) superuser  (1000)        1 2024-05-17 17:47:17.000000 jabir-0.0.6/jabir.egg-info/dependency_links.txt
+-rw-rw-r--   0 superuser  (1000) superuser  (1000)        6 2024-05-17 17:47:17.000000 jabir-0.0.6/jabir.egg-info/top_level.txt
+-rw-rw-r--   0 superuser  (1000) superuser  (1000)       38 2024-05-17 17:47:17.854188 jabir-0.0.6/setup.cfg
+-rw-r--r--   0 superuser  (1000) superuser  (1000)      721 2024-05-17 17:46:14.000000 jabir-0.0.6/setup.py
```

### Comparing `jabir-0.0.3/LICENSE` & `jabir-0.0.6/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Hassan Gashmard
+Copyright (c) 2024 Hassan Gashmard
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jabir-0.0.3/PKG-INFO` & `jabir-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: jabir
-Version: 0.0.3
-Summary: jaber is a package that generates 322 features for any material.
+Version: 0.0.6
+Summary: jabir is a package that generates 322 features for any material.
 Home-page: https://github.com/Gashmard/jabir
 Author: Hassan Gashmard
-Author-email: Gashmard2020@gmail.com
+Author-email: HassanGashmard@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 ### jabir
 We developed the Python package named **jabir** to generate atomic features. It can generate **322 atomic features for any type of material**, such as Electron Affinity, Electric Polarizability, Thermal Conductivity, Pettifor number, etc. Jabir calculates statistical relationships for each physical and chemical feature based on Element, Subscript, and Fraction.
 
 ### Installation
-Jaber employs some other libraries and packages to generate atomic features of materials, which need to be installed. These packages consist of pandas, numpy, mendeleev, pymatgen, chemparse and tqdm.
+**Jabir** employs some other libraries and packages to generate atomic features of materials, which need to be installed. These packages consist of **pandas**, **numpy**, **mendeleev**, **pymatgen** and **tqdm**. Therefore, it’s necessary to install all these packages. If you encounter an error, it is probably due to the conflict of different versions of the packages, so be sure to install the following versions using the commands below:
+pip install mendeleev==0.16.1 , pip install pymatgen==2024.5.1 , pip install tqdm==4.66.4
 
 **Note:** If you encounter any difficulties installing these packages on your local system, you can utilize the **Google colab** environment to install and utilize them seamlessly.
 
 ### How to use jabir
 After installing jabir, simply execute the following two lines of code.
 > from jabir import main
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jabir-0.0.3/README.md` & `jabir-0.0.6/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 ### jabir
 We developed the Python package named **jabir** to generate atomic features. It can generate **322 atomic features for any type of material**, such as Electron Affinity, Electric Polarizability, Thermal Conductivity, Pettifor number, etc. Jabir calculates statistical relationships for each physical and chemical feature based on Element, Subscript, and Fraction.
 
 ### Installation
-Jaber employs some other libraries and packages to generate atomic features of materials, which need to be installed. These packages consist of pandas, numpy, mendeleev, pymatgen, chemparse and tqdm.
+**Jabir** employs some other libraries and packages to generate atomic features of materials, which need to be installed. These packages consist of **pandas**, **numpy**, **mendeleev**, **pymatgen** and **tqdm**. Therefore, it’s necessary to install all these packages. If you encounter an error, it is probably due to the conflict of different versions of the packages, so be sure to install the following versions using the commands below:
+pip install mendeleev==0.16.1 , pip install pymatgen==2024.5.1 , pip install tqdm==4.66.4
 
 **Note:** If you encounter any difficulties installing these packages on your local system, you can utilize the **Google colab** environment to install and utilize them seamlessly.
 
 ### How to use jabir
 After installing jabir, simply execute the following two lines of code.
 > from jabir import main
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jabir-0.0.3/jabir/jabir.py` & `jabir-0.0.6/jabir/jabir.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 
 import numpy as np
 import pandas as pd
+from tqdm import tqdm
 import sys
-import mendeleev
-from mendeleev import *
+import re
 from mendeleev import element
 from mendeleev.fetch import fetch_ionization_energies
-import chemparse
-import pymatgen
 from pymatgen.core.composition import Composition
-from tqdm.notebook import tqdm_notebook
 
 
 # Function to read and convert file to DataFrame
 def read_input_file(input_file):
     # Determine the file format based on the file extension
     file_extension = input_file.split('.')[-1].lower()
     if file_extension == 'csv':
@@ -40,26 +37,131 @@
         sys.exit()
 
     # Rename the compound column to "formula"
     DataSet_for_Generation_322Features.rename(columns={Formula_column: "formula"}, inplace=True)
     print(f" The column containing \033[1m\033[97m\033[7m{Formula_column}\033[0m values names was chosen to generate atomic features.", '\n')
     return DataSet_for_Generation_322Features
 
+
+# ==> Start of Chemparse (Version: 0.1.3) code:  From here to the next 5 functions, the code is related to Chemparse package, 
+# and I got permission from its author to use its code here.
+# These 5 functions make a dictionary to be made from the compounds. 
+# For example, in MGB2, it says what index each element has.
+
+# function to return index of all instances of a substring in a string
+def find_all(sub, a_str):
+    start = 0
+    while True:
+        start = a_str.find(sub, start)
+        if start == -1: return
+        yield start
+        start += len(sub) # use start += 1 to find overlapping matches
+
+# functions to parse elemental formulas (handles both floats and ints)
+def get_first_elem(formula):
+    needed_split = False
+    for char in formula:
+        if formula.find(char) != 0 and (char.isupper() or char == "+" or char == "-"):
+            formula = formula.split(char)[0]
+            needed_split = True
+            return formula, needed_split
+        char_ind = list(find_all(char, formula))
+        if len(char_ind) > 1 and (char.isupper() or char == "+" or char == "-") and (formula[1] == char or formula[1].islower()) and sum(1 for c in formula[0:char_ind[1]] if c.isupper())==1:
+            formula = formula[0:char_ind[1]]
+            needed_split = True
+            return formula, needed_split
+    return formula, needed_split
+
+def inner_parse_formula(text):
+    formula_dict = {}
+    for i in range(0, len(text)):
+        element = re.findall("^[a-zA-Z-+]+", text)
+        if element == []:
+            break
+        else:
+            element, needed_split = get_first_elem(element[0])
+            text = text.replace(element, '', 1)
+            if needed_split:
+                number = 1.0
+            else:
+                try:
+                    number = float(re.findall(r"(^(?=.)([+-]?([0-9]*)(\.([0-9]+))?)([eE][+-]?\d+)?)", text)[0][0])
+                except:
+                    number = 1.0
+                text = re.sub(r"(^(?=.)([+-]?([0-9]*)(\.([0-9]+))?)([eE][+-]?\d+)?)", "", text)
+            if element not in list(formula_dict.keys()):
+                formula_dict[element] = number
+            else:
+                formula_dict[element] += number
+    return formula_dict
+
+def find_occurrences(s, ch):
+    return [i for i, letter in enumerate(s) if letter == ch]
+
+def parse_formula(text):
+    text = str(text)
+    # get indices of starting parentheses "(" and ending ")"
+    open_parenth_idx_list = find_occurrences(text, "(")
+    closed_parenth_idx_list = find_occurrences(text, ")")
+    if len(open_parenth_idx_list) != len(closed_parenth_idx_list):
+        raise Exception("Open and closed parentheses mismatch in formula '"+text+"'") 
+    for i in range(0, len(open_parenth_idx_list)-1):
+        if open_parenth_idx_list[i+1] < closed_parenth_idx_list[i]:
+            msg = ("Cannot parse nested parentheses in formula '"+text+"'")
+            raise Exception(msg)
+        if closed_parenth_idx_list[i] < open_parenth_idx_list[i]:
+            raise Exception("Closed parentheses detected before open parentheses in formula '"+text+"'")
+        if i == len(open_parenth_idx_list)-1:
+            if closed_parenth_idx_list[i+1] < open_parenth_idx_list[i+1]:
+                raise Exception("Closed parentheses detected before open parentheses in formula '"+text+"'")
+    seg_dict_list = []
+    for seg_i in range(0, len(open_parenth_idx_list)):
+        text = str(text)
+        # get indices of starting parentheses "(" and ending ")"
+        open_parenth_idx_list = find_occurrences(text, "(")
+        closed_parenth_idx_list = find_occurrences(text, ")")
+        seg = text[open_parenth_idx_list[0]:closed_parenth_idx_list[0]+1]
+        
+        try:
+            number = float(re.findall(r"(^(?=.)([+-]?([0-9]*)(\.([0-9]+))?)([eE][+-]?\d+)?)", text[closed_parenth_idx_list[0]+1:])[0][0])
+        except:
+            number = 1
+        seg_no_parenth = seg[1:-1]
+        seg_formula_dict = inner_parse_formula(seg_no_parenth)
+        seg_formula_dict_mult = {k:v*number for (k,v) in seg_formula_dict.items()}
+        endseg = re.sub(r"(^(?=.)(([0-9]*)(\.([0-9]+))?)([eE][+-]?\d+)?)", "", text[closed_parenth_idx_list[0]+1:])
+        text = text[:open_parenth_idx_list[0]]+endseg
+        seg_dict_list.append(seg_formula_dict_mult)
+    seg_dict_list.append(inner_parse_formula(text))
+    # merge and sum all segments
+    if len(seg_dict_list) > 1:
+        start_dict = seg_dict_list[0]
+        for i in range(1, len(seg_dict_list)):
+            next_dict = seg_dict_list[i]
+            start_dict = { k: start_dict.get(k, 0) + next_dict.get(k, 0) for k in set(start_dict) | set(next_dict) }
+        return start_dict
+    else:
+        return seg_dict_list[0]
+
+# ==> End of Chemparse (Version: 0.1.3) code:
+
+
 def data_preprocessing(DataSet_for_Generation_322Features):
     # Determine the column name of the formula
     target_column = "formula"
     # Checking the formula column to have the not a number or the same NaN
     if DataSet_for_Generation_322Features[target_column].isna().any():
         print(f"Column '{target_column}' contains \033[1m\033[97m\033[7m NaN \033[0m values.")
 
     List_Compound_Not_in_Periodic_Table=[]
     for index, row in DataSet_for_Generation_322Features.iterrows():
         # Creating a dictionary of elements
-        Element_dict=chemparse.parse_formula(row["formula"]) 
-        Element_dict_in_periodic_table=chemparse.parse_formula('Lr1Md1Fm1Es1Cf1Bk1Cm1Ac1Ra1Fr1Rn1At1Po1Pm1Xe1Kr1Ar1Ne1No1He1Al1Ag1Zn1Cd1Sn1Tl1Ti1Rh1In1Bi1Pb1Te1Hg1Ge1Th1Se1Mo1Ga1Sb1S1B1La1Nb1F1I1Pd1O1N1H1V1Au1Cr1Zr1Be1Fe1Si1Mg1Li1Er1Mn1As1Ru1Os1Ce1Cu1Gd1Ni1Sc1Ca1Sr1Y1Ho1Ta1C1U1Pt1Yb1Re1Am1P1W1Lu1Ba1Hf1Nd1K1Na1Cl1Pr1Co1Rb1Eu1Cs1Ir1Tc1Sm1Dy1Tm1Br1Tb1Pa1Np1Pu1')
+        # Element_dict=chemparse.parse_formula(row["formula"]) 
+        Element_dict=parse_formula(row["formula"])
+        Element_dict_in_periodic_table=parse_formula('Lr1Md1Fm1Es1Cf1Bk1Cm1Ac1Ra1Fr1Rn1At1Po1Pm1Xe1Kr1Ar1Ne1No1He1Al1Ag1Zn1Cd1Sn1Tl1Ti1Rh1In1Bi1Pb1Te1Hg1Ge1Th1Se1Mo1Ga1Sb1S1B1La1Nb1F1I1Pd1O1N1H1V1Au1Cr1Zr1Be1Fe1Si1Mg1Li1Er1Mn1As1Ru1Os1Ce1Cu1Gd1Ni1Sc1Ca1Sr1Y1Ho1Ta1C1U1Pt1Yb1Re1Am1P1W1Lu1Ba1Hf1Nd1K1Na1Cl1Pr1Co1Rb1Eu1Cs1Ir1Tc1Sm1Dy1Tm1Br1Tb1Pa1Np1Pu1')
         for k,v in Element_dict.items():
             if k not in Element_dict_in_periodic_table:
                 List_Compound_Not_in_Periodic_Table.append(row["formula"])
     if len(List_Compound_Not_in_Periodic_Table) != 0:
         print('\033[1m\033[97m\033[7m Contains problematic compounds \033[0m', 
                'These compounds contain elements not found in the periodic table=', List_Compound_Not_in_Periodic_Table)
 
@@ -71,15 +173,15 @@
             print("This compound is problematic, please correct", Elem,".  ", e)
 
 def Generation_322_Features(DataSet_for_Generation_322Features):
   import warnings
   warnings.filterwarnings('ignore')
   # Number_of_Elements
   Number_of_Elements=[]
-  for i in tqdm_notebook(range(1), desc='Please wait, the first step is running ... '):
+  for i in tqdm(range(1), desc='Please wait, the first step is running ... '):
     for index, row in DataSet_for_Generation_322Features.iterrows():
         comp = Composition(row['formula'])
         Number=len(comp) 
         Number_of_Elements.append(Number)   
     DataSet_for_Generation_322Features['Number_Elements']= Number_of_Elements 
 
     #  Sum_of_Subscript
@@ -555,17 +657,17 @@
   total_Ionic_Radius_Based_Elemental_variance=[]
   total_Ionic_Radius_Based_Elemental_max=[]
   total_Ionic_Radius_Based_Elemental_min=[]
   total_Ionic_Radius_Based_Elemental_range=[]  
   total_Ionic_Radius_Based_Elemental_std=[] # std= Standard deviation  
   total_Ionic_Radius_Based_Elemental_Ave_dev =[]   # Ave_dev=Average_deviation  
 
-  for index, row in tqdm_notebook(DataSet_for_Generation_322Features.iterrows(), total=len(DataSet_for_Generation_322Features), desc="Please wait, the last step is running ... "):
+  for index, row in tqdm(DataSet_for_Generation_322Features.iterrows(), total=len(DataSet_for_Generation_322Features), desc="Please wait, the last step is running ... "):
       
-      Element_dict=chemparse.parse_formula(row["formula"]) 
+      Element_dict=parse_formula(row["formula"]) 
       Elem = row["formula"]
       comp = Composition(Elem) 
 
       electronegativ_List=[]
       electronegativ_List_Based_on_fraction=[]                    
       elem_electronegativ_Subscript_List=[] 
       pettifor_number_List=[]  
@@ -1627,11 +1729,11 @@
     DataSet_for_Generation_322Features = read_input_file(input_file)
     rename_target_column(DataSet_for_Generation_322Features)
     data_preprocessing(DataSet_for_Generation_322Features)
     Generation_322_Features(DataSet_for_Generation_322Features)
     save_dataframe()
     return DataSet_for_Generation_322Features
   
-if __name__ == "__main__":
-    main()
+# if __name__ == "__main__":
+#     main()
```

### Comparing `jabir-0.0.3/jabir.egg-info/PKG-INFO` & `jabir-0.0.6/jabir.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: jabir
-Version: 0.0.3
-Summary: jaber is a package that generates 322 features for any material.
+Version: 0.0.6
+Summary: jabir is a package that generates 322 features for any material.
 Home-page: https://github.com/Gashmard/jabir
 Author: Hassan Gashmard
-Author-email: Gashmard2020@gmail.com
+Author-email: HassanGashmard@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 ### jabir
 We developed the Python package named **jabir** to generate atomic features. It can generate **322 atomic features for any type of material**, such as Electron Affinity, Electric Polarizability, Thermal Conductivity, Pettifor number, etc. Jabir calculates statistical relationships for each physical and chemical feature based on Element, Subscript, and Fraction.
 
 ### Installation
-Jaber employs some other libraries and packages to generate atomic features of materials, which need to be installed. These packages consist of pandas, numpy, mendeleev, pymatgen, chemparse and tqdm.
+**Jabir** employs some other libraries and packages to generate atomic features of materials, which need to be installed. These packages consist of **pandas**, **numpy**, **mendeleev**, **pymatgen** and **tqdm**. Therefore, it’s necessary to install all these packages. If you encounter an error, it is probably due to the conflict of different versions of the packages, so be sure to install the following versions using the commands below:
+pip install mendeleev==0.16.1 , pip install pymatgen==2024.5.1 , pip install tqdm==4.66.4
 
 **Note:** If you encounter any difficulties installing these packages on your local system, you can utilize the **Google colab** environment to install and utilize them seamlessly.
 
 ### How to use jabir
 After installing jabir, simply execute the following two lines of code.
 > from jabir import main
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jabir-0.0.3/setup.py` & `jabir-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "jabir",
-    version = "0.0.3",
+    version = "0.0.6",
     author = "Hassan Gashmard",
-    author_email = "Gashmard2020@gmail.com",
-    description = "jaber is a package that generates 322 features for any material.",
+    author_email = "HassanGashmard@gmail.com",
+    description = "jabir is a package that generates 322 features for any material.",
     long_description = long_description,
     license="MIT",
     long_description_content_type = "text/markdown",
     url = "https://github.com/Gashmard/jabir",
 
     classifiers = [
         "Programming Language :: Python :: 3",
```

