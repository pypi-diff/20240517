# Comparing `tmp/plasmidhunter-1.3.tar.gz` & `tmp/plasmidhunter-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plasmidhunter-1.3.tar", last modified: Tue Dec 26 20:18:59 2023, max compression
+gzip compressed data, was "plasmidhunter-1.4.tar", last modified: Fri May 17 20:16:26 2024, max compression
```

## Comparing `plasmidhunter-1.3.tar` & `plasmidhunter-1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tianrm    (1001) tianrm    (1001)        0 2023-12-26 20:18:59.857629 plasmidhunter-1.3/
--rw-r--r--   0 tianrm    (1001) tianrm    (1001)    10219 2023-12-26 18:52:15.000000 plasmidhunter-1.3/LICENSE.md
--rw-r--r--   0 tianrm    (1001) tianrm    (1001)     2108 2023-12-26 20:18:59.857629 plasmidhunter-1.3/PKG-INFO
-drwxr-xr-x   0 tianrm    (1001) tianrm    (1001)        0 2023-12-26 20:18:59.819629 plasmidhunter-1.3/PlasmidHunter/
--rw-r--r--   0 tianrm    (1001) tianrm    (1001)     2478 2023-12-26 19:48:29.000000 plasmidhunter-1.3/PlasmidHunter/PlasmidHunter.py
--rw-r--r--   0 tianrm    (1001) tianrm    (1001)        0 2023-12-26 18:52:14.000000 plasmidhunter-1.3/PlasmidHunter/__init__.py
--rw-r--r--   0 tianrm    (1001) tianrm    (1001)     4453 2023-12-26 19:41:22.000000 plasmidhunter-1.3/PlasmidHunter/functions.py
-drwxr-xr-x   0 tianrm    (1001) tianrm    (1001)        0 2023-12-26 20:18:59.832629 plasmidhunter-1.3/PlasmidHunter/model/
--rw-r--r--   0 tianrm    (1001) tianrm    (1001) 10706062 2023-12-26 18:52:15.000000 plasmidhunter-1.3/PlasmidHunter/model/feature_genes.pkl
--rw-r--r--   0 tianrm    (1001) tianrm    (1001) 20167110 2023-12-26 18:52:15.000000 plasmidhunter-1.3/PlasmidHunter/model/guassiannb.pkl
--rw-r--r--   0 tianrm    (1001) tianrm    (1001)     1826 2023-12-26 19:57:20.000000 plasmidhunter-1.3/README.md
-drwxr-xr-x   0 tianrm    (1001) tianrm    (1001)        0 2023-12-26 20:18:59.857629 plasmidhunter-1.3/plasmidhunter.egg-info/
--rw-r--r--   0 tianrm    (1001) tianrm    (1001)     2108 2023-12-26 20:18:59.000000 plasmidhunter-1.3/plasmidhunter.egg-info/PKG-INFO
--rw-r--r--   0 tianrm    (1001) tianrm    (1001)      410 2023-12-26 20:18:59.000000 plasmidhunter-1.3/plasmidhunter.egg-info/SOURCES.txt
--rw-r--r--   0 tianrm    (1001) tianrm    (1001)        1 2023-12-26 20:18:59.000000 plasmidhunter-1.3/plasmidhunter.egg-info/dependency_links.txt
--rw-r--r--   0 tianrm    (1001) tianrm    (1001)       67 2023-12-26 20:18:59.000000 plasmidhunter-1.3/plasmidhunter.egg-info/entry_points.txt
--rw-r--r--   0 tianrm    (1001) tianrm    (1001)       60 2023-12-26 20:18:59.000000 plasmidhunter-1.3/plasmidhunter.egg-info/requires.txt
--rw-r--r--   0 tianrm    (1001) tianrm    (1001)       14 2023-12-26 20:18:59.000000 plasmidhunter-1.3/plasmidhunter.egg-info/top_level.txt
--rw-r--r--   0 tianrm    (1001) tianrm    (1001)       38 2023-12-26 20:18:59.857629 plasmidhunter-1.3/setup.cfg
--rw-r--r--   0 tianrm    (1001) tianrm    (1001)     1265 2023-12-26 20:18:53.000000 plasmidhunter-1.3/setup.py
+drwxr-xr-x   0 tianrm    (1001) tianrm    (1001)        0 2024-05-17 20:16:26.788220 plasmidhunter-1.4/
+-rw-r--r--   0 tianrm    (1001) tianrm    (1001)    10219 2024-05-16 21:33:43.000000 plasmidhunter-1.4/LICENSE.md
+-rw-r--r--   0 tianrm    (1001) tianrm    (1001)     2534 2024-05-17 20:16:26.786220 plasmidhunter-1.4/PKG-INFO
+drwxr-xr-x   0 tianrm    (1001) tianrm    (1001)        0 2024-05-17 20:16:26.708220 plasmidhunter-1.4/PlasmidHunter/
+-rw-r--r--   0 tianrm    (1001) tianrm    (1001)     2675 2024-05-17 16:54:15.000000 plasmidhunter-1.4/PlasmidHunter/PlasmidHunter.py
+-rw-r--r--   0 tianrm    (1001) tianrm    (1001)        0 2024-05-16 21:33:42.000000 plasmidhunter-1.4/PlasmidHunter/__init__.py
+-rw-r--r--   0 tianrm    (1001) tianrm    (1001)     4903 2024-05-17 15:09:09.000000 plasmidhunter-1.4/PlasmidHunter/functions.py
+drwxr-xr-x   0 tianrm    (1001) tianrm    (1001)        0 2024-05-17 20:16:26.756220 plasmidhunter-1.4/PlasmidHunter/model/
+-rw-r--r--   0 tianrm    (1001) tianrm    (1001)  2920081 2024-05-17 16:51:53.000000 plasmidhunter-1.4/PlasmidHunter/model/feature_genes.gz
+-rw-r--r--   0 tianrm    (1001) tianrm    (1001)  1528968 2024-05-17 15:10:13.000000 plasmidhunter-1.4/PlasmidHunter/model/guassiannb_model_params.json.gz
+-rw-r--r--   0 tianrm    (1001) tianrm    (1001)     2252 2024-05-17 15:22:23.000000 plasmidhunter-1.4/README.md
+drwxr-xr-x   0 tianrm    (1001) tianrm    (1001)        0 2024-05-17 20:16:26.786220 plasmidhunter-1.4/plasmidhunter.egg-info/
+-rw-r--r--   0 tianrm    (1001) tianrm    (1001)     2534 2024-05-17 20:16:26.000000 plasmidhunter-1.4/plasmidhunter.egg-info/PKG-INFO
+-rw-r--r--   0 tianrm    (1001) tianrm    (1001)      426 2024-05-17 20:16:26.000000 plasmidhunter-1.4/plasmidhunter.egg-info/SOURCES.txt
+-rw-r--r--   0 tianrm    (1001) tianrm    (1001)        1 2024-05-17 20:16:26.000000 plasmidhunter-1.4/plasmidhunter.egg-info/dependency_links.txt
+-rw-r--r--   0 tianrm    (1001) tianrm    (1001)       67 2024-05-17 20:16:26.000000 plasmidhunter-1.4/plasmidhunter.egg-info/entry_points.txt
+-rw-r--r--   0 tianrm    (1001) tianrm    (1001)       60 2024-05-17 20:16:26.000000 plasmidhunter-1.4/plasmidhunter.egg-info/requires.txt
+-rw-r--r--   0 tianrm    (1001) tianrm    (1001)       14 2024-05-17 20:16:26.000000 plasmidhunter-1.4/plasmidhunter.egg-info/top_level.txt
+-rw-r--r--   0 tianrm    (1001) tianrm    (1001)       38 2024-05-17 20:16:26.788220 plasmidhunter-1.4/setup.cfg
+-rw-r--r--   0 tianrm    (1001) tianrm    (1001)      749 2024-05-17 15:55:25.000000 plasmidhunter-1.4/setup.py
```

### Comparing `plasmidhunter-1.3/LICENSE.md` & `plasmidhunter-1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `plasmidhunter-1.3/PKG-INFO` & `plasmidhunter-1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plasmidhunter
-Version: 1.3
+Version: 1.4
 Requires-Python: ==3.10.*
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: numpy==1.25.0
 Requires-Dist: biopython
@@ -17,24 +17,43 @@
 # PlasmidHunter: Accurate and Fast Plasmid Prediction Based on Gene Content Using Machine Learning 
 
 Plasmids are extrachromosomal DNA found in microorganisms. They often carry beneficial genes that help bacteria adapt to harsh conditions. Plasmids are also important tools in genetic engineering, gene therapy, and drug production. However, it can be difficult to identify plasmid sequences from chromosomal sequences in genomic and metagenomic data. Here, we have developed a new tool called PlasmidHunter, which uses machine learning to predict plasmid sequences based on gene content profile. PlasmidHunter achieved high accuracies (up to 97.6%) and high speeds in benchmark tests including both simulated contigs and real metagenomic plasmidome data, outperforming other existing tools.
 
 Keywords: artificial intelligence (AI), machine learning (ML), plasmid prediction, genomic sequencing
 
 ## Installation and run
-conda create -n plasmidhunter -c bioconda -y python=3.10 diamond=2.1.8 prodigal
+conda create -n plasmidhunter -c bioconda -c conda-forge -y python=3.10 diamond=2.1.8 prodigal
 
 conda activate plasmidhunter
 
 pip install plasmidhunter
 
 plasmidhunter -h
+
 ## Result Interpretation
 The result is a tab-delimited table showing the prediction of each sequence. The columns include Prediction (0: chromosome, 1: plasmid), Probability of 0 (chromosome), and Probability of 1 (plasmid). 
 
+## Change Log
+v1.1 9/1/2022
+
+PlasmidHunter is now using much less memory.
+
+v1.2 11/23/2023
+
+PlasmidHunter has an expanded database for a higher annotation rate.
+
+PlasmidHunter is now accepting shorter contigs down to 1 Kbp and has a higher accuracy for short contigs.
+
+v1.3 4/2024
+Fixed some minor bugs
+
+v1.4 5/17/2024
+
+Converted model and feature pickle file into parameter file and text file, respectively.
+
 ## Citation
 PlasmidHunter: Accurate and fast prediction of plasmid sequences using gene content profile and machine learning
 
 Renmao Tian, Jizhong Zhou, Behzad Imanian
 
 bioRxiv 2023.02.01.526640; doi: https://doi.org/10.1101/2023.02.01.526640
```

### Comparing `plasmidhunter-1.3/PlasmidHunter/PlasmidHunter.py` & `plasmidhunter-1.4/PlasmidHunter/PlasmidHunter.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 parser.add_argument('-i','--infile',dest='inp',required=True,help='Input fasta file. Only contigs > 1Kbp will be includded in the prediction.')
 parser.add_argument('-c','--cpu',dest='cpu',required=False,default=10, type=int, help='Number of processes to launch for the Prodigal gene prediction and Diamond alignment. [Default: 10]')
 parser.add_argument('-o','--outdir',dest='out',required=False,default='plasmid_prediction',help='Output directory of the prediction. The result file, predictions.tsv, includes the prediction results and corresponding probabilities [Default: plasmid_prediction]')
 args=parser.parse_args()
 
 def main():
     infile = args.inp
-    model = pkg_resources.resource_filename('PlasmidHunter', 'model/guassiannb.pkl')
-    feature_genes = pkg_resources.resource_filename('PlasmidHunter', 'model/feature_genes.pkl')
+    model = pkg_resources.resource_filename('PlasmidHunter', 'model/guassiannb_model_params.json.gz')
+    feature_genes = pkg_resources.resource_filename('PlasmidHunter', 'model/feature_genes.gz')
     database = f'{os.path.dirname(os.path.dirname(model))}/database/database.dmnd'
     if not os.path.exists(database):
-        print('Downloading database. Please wait some minutes ...')
-        os.mkdir(os.path.dirname(database))
+        print(f'{database}\nDownloading database. This will run only once. Please wait some minutes ...')
+        os.makedirs(os.path.dirname(database), exist_ok=True)
         download_file('https://zenodo.org/records/10431696/files/database.dmnd.gz?download=1', f'{database}.gz')
         unzip(f'{database}.gz')
 
     cpu = args.cpu
     outdir = args.out
 
     # filter short reads
@@ -35,16 +35,18 @@
     seq_num = filter_fasta(infile, outdir+'/input.fasta', 1000)
     cpu = min(seq_num, cpu)
 
     # generate gene profile
     dict1 = gene_content_profile(outdir+'/input.fasta', prodigal, database, cpu=cpu)
 
     # predicting
-    feature_genes = pickle.load(open(feature_genes, 'rb'))
-    clf = pickle.loads(pickle.load(open(model, 'rb')))
+    #feature_genes = pickle.load(open(feature_genes, 'rb'))
+    feature_genes = json.loads(gzip.open(feature_genes, "rt", encoding="utf-8").read())
+    #clf = pickle.loads(pickle.load(open(model, 'rb')))
+    clf = load_model_params(model)
     pred = predict(dict1, feature_genes, clf)
     pred.to_csv(outdir+'/predictions.tsv', sep='\t')
     os.remove(outdir+'/input.fasta')
     print('Prediction completed. See '+outdir+'/predictions.tsv for the prediction outputs and probabilities.\nPlease cite us if you find it helpful. Thank you!')
 
 if __name__ == '__main__':
     main()
```

### Comparing `plasmidhunter-1.3/PlasmidHunter/functions.py` & `plasmidhunter-1.4/PlasmidHunter/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from glob import glob
 import json
 import pickle
 from collections import Counter
 from Bio import SeqIO
 import requests
 import gzip
+from sklearn.naive_bayes import GaussianNB
 
 def unzip(infile):
     with gzip.open(infile, 'rb') as f_in:
         with open(infile[:-3], 'wb') as f_out:
             shutil.copyfileobj(f_in, f_out)
             os.remove(infile)
 
@@ -104,14 +105,27 @@
     mergefiles(temp_dir, f'{temp_dir}/proteins.faa')
     diamond_alignment(temp_dir+'/proteins.faa', database, cpu=cpu)
     dict1 = daa_to_hits(temp_dir+'/proteins.faa.daa')
     shutil.rmtree(temp_dir)
     
     return(dict1)
 
+def load_model_params(param_file): #
+    with gzip.open(param_file, 'rt', encoding='utf-8') as file:
+        json_str = file.read()
+    params = json.loads(json_str)
+
+    model = GaussianNB()
+    model.class_prior_ = np.array(params['class_prior_'])
+    model.theta_ = np.array(params['theta_'])
+    model.var_ = np.array(params['var_'])
+    model.classes_ = np.array(params['classes_'])
+
+    return model
+
 def predict(dict1, feature_genes, clf):
     print('Predicting using a model ...')
     dict1 = list(dict1.items())
     l = [dict1[i:i+50] for i in list(range(0, len(dict1), 50))]
     l = [dict(i) for i in l]
     out = pd.DataFrame()
```

### Comparing `plasmidhunter-1.3/README.md` & `plasmidhunter-1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,24 +5,43 @@
 # PlasmidHunter: Accurate and Fast Plasmid Prediction Based on Gene Content Using Machine Learning 
 
 Plasmids are extrachromosomal DNA found in microorganisms. They often carry beneficial genes that help bacteria adapt to harsh conditions. Plasmids are also important tools in genetic engineering, gene therapy, and drug production. However, it can be difficult to identify plasmid sequences from chromosomal sequences in genomic and metagenomic data. Here, we have developed a new tool called PlasmidHunter, which uses machine learning to predict plasmid sequences based on gene content profile. PlasmidHunter achieved high accuracies (up to 97.6%) and high speeds in benchmark tests including both simulated contigs and real metagenomic plasmidome data, outperforming other existing tools.
 
 Keywords: artificial intelligence (AI), machine learning (ML), plasmid prediction, genomic sequencing
 
 ## Installation and run
-conda create -n plasmidhunter -c bioconda -y python=3.10 diamond=2.1.8 prodigal
+conda create -n plasmidhunter -c bioconda -c conda-forge -y python=3.10 diamond=2.1.8 prodigal
 
 conda activate plasmidhunter
 
 pip install plasmidhunter
 
 plasmidhunter -h
+
 ## Result Interpretation
 The result is a tab-delimited table showing the prediction of each sequence. The columns include Prediction (0: chromosome, 1: plasmid), Probability of 0 (chromosome), and Probability of 1 (plasmid). 
 
+## Change Log
+v1.1 9/1/2022
+
+PlasmidHunter is now using much less memory.
+
+v1.2 11/23/2023
+
+PlasmidHunter has an expanded database for a higher annotation rate.
+
+PlasmidHunter is now accepting shorter contigs down to 1 Kbp and has a higher accuracy for short contigs.
+
+v1.3 4/2024
+Fixed some minor bugs
+
+v1.4 5/17/2024
+
+Converted model and feature pickle file into parameter file and text file, respectively.
+
 ## Citation
 PlasmidHunter: Accurate and fast prediction of plasmid sequences using gene content profile and machine learning
 
 Renmao Tian, Jizhong Zhou, Behzad Imanian
 
 bioRxiv 2023.02.01.526640; doi: https://doi.org/10.1101/2023.02.01.526640
```

### Comparing `plasmidhunter-1.3/plasmidhunter.egg-info/PKG-INFO` & `plasmidhunter-1.4/plasmidhunter.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plasmidhunter
-Version: 1.3
+Version: 1.4
 Requires-Python: ==3.10.*
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: numpy==1.25.0
 Requires-Dist: biopython
@@ -17,24 +17,43 @@
 # PlasmidHunter: Accurate and Fast Plasmid Prediction Based on Gene Content Using Machine Learning 
 
 Plasmids are extrachromosomal DNA found in microorganisms. They often carry beneficial genes that help bacteria adapt to harsh conditions. Plasmids are also important tools in genetic engineering, gene therapy, and drug production. However, it can be difficult to identify plasmid sequences from chromosomal sequences in genomic and metagenomic data. Here, we have developed a new tool called PlasmidHunter, which uses machine learning to predict plasmid sequences based on gene content profile. PlasmidHunter achieved high accuracies (up to 97.6%) and high speeds in benchmark tests including both simulated contigs and real metagenomic plasmidome data, outperforming other existing tools.
 
 Keywords: artificial intelligence (AI), machine learning (ML), plasmid prediction, genomic sequencing
 
 ## Installation and run
-conda create -n plasmidhunter -c bioconda -y python=3.10 diamond=2.1.8 prodigal
+conda create -n plasmidhunter -c bioconda -c conda-forge -y python=3.10 diamond=2.1.8 prodigal
 
 conda activate plasmidhunter
 
 pip install plasmidhunter
 
 plasmidhunter -h
+
 ## Result Interpretation
 The result is a tab-delimited table showing the prediction of each sequence. The columns include Prediction (0: chromosome, 1: plasmid), Probability of 0 (chromosome), and Probability of 1 (plasmid). 
 
+## Change Log
+v1.1 9/1/2022
+
+PlasmidHunter is now using much less memory.
+
+v1.2 11/23/2023
+
+PlasmidHunter has an expanded database for a higher annotation rate.
+
+PlasmidHunter is now accepting shorter contigs down to 1 Kbp and has a higher accuracy for short contigs.
+
+v1.3 4/2024
+Fixed some minor bugs
+
+v1.4 5/17/2024
+
+Converted model and feature pickle file into parameter file and text file, respectively.
+
 ## Citation
 PlasmidHunter: Accurate and fast prediction of plasmid sequences using gene content profile and machine learning
 
 Renmao Tian, Jizhong Zhou, Behzad Imanian
 
 bioRxiv 2023.02.01.526640; doi: https://doi.org/10.1101/2023.02.01.526640
```

