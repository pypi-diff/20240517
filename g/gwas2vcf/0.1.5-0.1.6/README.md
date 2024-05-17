# Comparing `tmp/gwas2vcf-0.1.5.tar.gz` & `tmp/gwas2vcf-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwas2vcf-0.1.5.tar", last modified: Fri May 17 20:24:34 2024, max compression
+gzip compressed data, was "gwas2vcf-0.1.6.tar", last modified: Fri May 17 20:26:06 2024, max compression
```

## Comparing `gwas2vcf-0.1.5.tar` & `gwas2vcf-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 20:24:34.896008 gwas2vcf-0.1.5/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       19 2024-05-17 19:26:12.000000 gwas2vcf-0.1.5/MANIFEST.in
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)      948 2024-05-17 20:24:34.896008 gwas2vcf-0.1.5/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      419 2024-05-17 19:59:19.000000 gwas2vcf-0.1.5/README.md
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 20:24:34.892008 gwas2vcf-0.1.5/gwas2vcf/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 19:50:34.000000 gwas2vcf-0.1.5/gwas2vcf/__init__.py
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     3227 2024-05-17 20:23:35.000000 gwas2vcf-0.1.5/gwas2vcf/convert_to_vcf.py
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 20:24:34.896008 gwas2vcf-0.1.5/gwas2vcf.egg-info/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)      948 2024-05-17 20:24:34.000000 gwas2vcf-0.1.5/gwas2vcf.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      282 2024-05-17 20:24:34.000000 gwas2vcf-0.1.5/gwas2vcf.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-17 20:24:34.000000 gwas2vcf-0.1.5/gwas2vcf.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       58 2024-05-17 20:24:34.000000 gwas2vcf-0.1.5/gwas2vcf.egg-info/entry_points.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       12 2024-05-17 20:24:34.000000 gwas2vcf-0.1.5/gwas2vcf.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        9 2024-05-17 20:24:34.000000 gwas2vcf-0.1.5/gwas2vcf.egg-info/top_level.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       79 2024-05-17 20:24:34.896008 gwas2vcf-0.1.5/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      913 2024-05-17 20:24:13.000000 gwas2vcf-0.1.5/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 20:26:06.679603 gwas2vcf-0.1.6/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       19 2024-05-17 19:26:12.000000 gwas2vcf-0.1.6/MANIFEST.in
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)      948 2024-05-17 20:26:06.679603 gwas2vcf-0.1.6/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      419 2024-05-17 19:59:19.000000 gwas2vcf-0.1.6/README.md
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 20:26:06.675603 gwas2vcf-0.1.6/gwas2vcf/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 19:50:34.000000 gwas2vcf-0.1.6/gwas2vcf/__init__.py
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     3017 2024-05-17 20:25:40.000000 gwas2vcf-0.1.6/gwas2vcf/convert_to_vcf.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 20:26:06.679603 gwas2vcf-0.1.6/gwas2vcf.egg-info/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)      948 2024-05-17 20:26:06.000000 gwas2vcf-0.1.6/gwas2vcf.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      282 2024-05-17 20:26:06.000000 gwas2vcf-0.1.6/gwas2vcf.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-17 20:26:06.000000 gwas2vcf-0.1.6/gwas2vcf.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       58 2024-05-17 20:26:06.000000 gwas2vcf-0.1.6/gwas2vcf.egg-info/entry_points.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       12 2024-05-17 20:26:06.000000 gwas2vcf-0.1.6/gwas2vcf.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        9 2024-05-17 20:26:06.000000 gwas2vcf-0.1.6/gwas2vcf.egg-info/top_level.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       79 2024-05-17 20:26:06.679603 gwas2vcf-0.1.6/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      913 2024-05-17 20:25:47.000000 gwas2vcf-0.1.6/setup.py
```

### Comparing `gwas2vcf-0.1.5/PKG-INFO` & `gwas2vcf-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwas2vcf
-Version: 0.1.5
+Version: 0.1.6
 Summary: A tool to convert GWAS TSV files to VCF format
 Home-page: https://github.com/VJ-Ulaganathan/gwas2vcf/
 Author: Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: vijay-kumar.ulaganathan@uni-tuebingen.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gwas2vcf-0.1.5/gwas2vcf/convert_to_vcf.py` & `gwas2vcf-0.1.6/gwas2vcf/convert_to_vcf.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,85 +1,80 @@
-    import argparse
-    import pandas as pd
-    import gzip
-    from tqdm import tqdm
-    import pkg_resources
-
-    def parse_arguments():
-        parser = argparse.ArgumentParser(description="Convert GWAS TSV file to VCF format.")
-        parser.add_argument("-i", "--input", required=True, help="Input TSV.bgz file")
-        parser.add_argument("-o", "--output", required=True, help="Output VCF file (without .vcf.gz extension)")
-        
-        return parser.parse_args()
-
-    def main():
-        args = parse_arguments()
+##code for converting UK BioBank GWAS file to standard VCF4.0 format.
+##If you found our code useful, please consider following me on https://x.com/VK_Ulaganathan
 
-        if args.version:
-            version = pkg_resources.require("gwas2vcf")[0].version
-            print(f"gwas2vcf version {version}")
-            return
-
-        input_file = args.input
-        output_file = args.output
-
-        # Ensure the output file has the correct .vcf.gz extension
-        if not output_file.endswith(".vcf.gz"):
-            output_file += ".vcf.gz"
-
-        # Read the input file
-        with gzip.open(input_file, 'rt') as f:
-            df = pd.read_csv(f, sep='\t')
-
-        # Split the 'variant' column into 'CHROM', 'POS', 'REF', and 'ALT'
-        df[['CHROM', 'POS', 'REF', 'ALT']] = df['variant'].str.split(':', expand=True)
-
-        # Define the VCF header
-        vcf_header = [
-            "##fileformat=VCFv4.0",
-            "##source=GWAS",
-            "##INFO=<ID=AC,Number=A,Type=Integer,Description=\"Alternate Allele Count\">",
-            "##INFO=<ID=AF,Number=A,Type=Float,Description=\"Alternate Allele Frequency\">",
-            "##INFO=<ID=AN,Number=1,Type=Integer,Description=\"Total Number of Alleles\">",
-            "##INFO=<ID=low_confidence,Number=0,Type=Flag,Description=\"Low Confidence Variant\">",
-            "##FORMAT=<ID=GT,Number=1,Type=String,Description=\"Genotype\">",
-            "#CHROM\tPOS\tID\tREF\tALT\tQUAL\tFILTER\tINFO\tFORMAT\tsample"
-        ]
-
-        # Open the output VCF file for writing
-        with gzip.open(output_file, 'wt') as vcf:
-            # Write the VCF header
-            for line in vcf_header:
-                vcf.write(line + '\n')
+import pandas as pd
+import gzip
+import argparse
+from tqdm import tqdm
+
+def parse_arguments():
+    parser = argparse.ArgumentParser(description="Convert GWAS file VCF format.")
+    parser.add_argument("-i", "--input", required=True, help="please provide the path for the input file with the extension .bgz")
+    parser.add_argument("-o", "--output", required=True, help="please provide desire output file name, tool will automatically append the .vcf.gz extension")
+    return parser.parse_args()
+
+def main():
+    args = parse_arguments()
+    input_file = args.input
+    output_file = args.output
+
+    # Ensure the output file has the correct .vcf.gz extension
+    if not output_file.endswith(".vcf.gz"):
+        output_file += ".vcf.gz"
+
+    # Read the input file
+    with gzip.open(input_file, 'rt') as f:
+        df = pd.read_csv(f, sep='\t')
+
+    # Split the 'variant' column into 'CHROM', 'POS', 'REF', and 'ALT'
+    df[['CHROM', 'POS', 'REF', 'ALT']] = df['variant'].str.split(':', expand=True)
+
+    # Define the VCF header
+    vcf_header = [
+        "##fileformat=VCFv4.0",
+        "##source=GWAS",
+        "##INFO=<ID=AC,Number=A,Type=Integer,Description=\"Alternate Allele Count\">",
+        "##INFO=<ID=AF,Number=A,Type=Float,Description=\"Alternate Allele Frequency\">",
+        "##INFO=<ID=AN,Number=1,Type=Integer,Description=\"Total Number of Alleles\">",
+        "##INFO=<ID=low_confidence,Number=0,Type=Flag,Description=\"Low Confidence Variant\">",
+        "##FORMAT=<ID=GT,Number=1,Type=String,Description=\"Genotype\">",
+        "#CHROM\tPOS\tID\tREF\tALT\tQUAL\tFILTER\tINFO\tFORMAT\tsample"
+    ]
+
+    # Open the output VCF file for writing
+    with gzip.open(output_file, 'wt') as vcf:
+        # Write the VCF header
+        for line in vcf_header:
+            vcf.write(line + '\n')
+        
+        # Write the VCF body with progress bar
+        for _, row in tqdm(df.iterrows(), total=df.shape[0], desc="Processing rows"):
+            info_fields = [
+                f"AC={int(row['AC'])}",
+                f"AF={float(row['minor_AF'])}",
+                f"AN={2 * int(row['n_complete_samples'])}"  # assuming diploid samples
+            ]
+            if row['low_confidence_variant'] == 'true':
+                info_fields.append("low_confidence")
+            
+            info_str = ";".join(info_fields)
+            format_str = "GT"
+            sample_str = "./."
+
+            vcf_row = [
+                row['CHROM'],
+                row['POS'],
+                '.',
+                row['REF'],
+                row['ALT'],
+                '.',
+                'PASS' if row['low_confidence_variant'] == 'false' else 'LowQual',
+                info_str,
+                format_str,
+                sample_str
+            ]
             
-            # Write the VCF body with progress bar
-            for _, row in tqdm(df.iterrows(), total=df.shape[0], desc="Processing rows"):
-                info_fields = [
-                    f"AC={int(row['AC'])}",
-                    f"AF={float(row['minor_AF'])}",
-                    f"AN={2 * int(row['n_complete_samples'])}"  # assuming diploid samples
-                ]
-                if row['low_confidence_variant'] == 'true':
-                    info_fields.append("low_confidence")
-                
-                info_str = ";".join(info_fields)
-                format_str = "GT"
-                sample_str = "./."
-
-                vcf_row = [
-                    row['CHROM'],
-                    row['POS'],
-                    '.',
-                    row['REF'],
-                    row['ALT'],
-                    '.',
-                    'PASS' if row['low_confidence_variant'] == 'false' else 'LowQual',
-                    info_str,
-                    format_str,
-                    sample_str
-                ]
-                
-                vcf.write("\t".join(vcf_row) + '\n')
+            vcf.write("\t".join(vcf_row) + '\n')
 
-    if __name__ == "__main__":
-        main()
+if __name__ == "__main__":
+    main()
```

### Comparing `gwas2vcf-0.1.5/gwas2vcf.egg-info/PKG-INFO` & `gwas2vcf-0.1.6/gwas2vcf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwas2vcf
-Version: 0.1.5
+Version: 0.1.6
 Summary: A tool to convert GWAS TSV files to VCF format
 Home-page: https://github.com/VJ-Ulaganathan/gwas2vcf/
 Author: Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: vijay-kumar.ulaganathan@uni-tuebingen.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gwas2vcf-0.1.5/setup.py` & `gwas2vcf-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="gwas2vcf",
-    version="0.1.5",
+    version="0.1.6",
     author="Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN",
     author_email="vijay-kumar.ulaganathan@uni-tuebingen.de",
     description="A tool to convert GWAS TSV files to VCF format",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/VJ-Ulaganathan/gwas2vcf/",
     packages=find_packages(),
```

