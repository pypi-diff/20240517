# Comparing `tmp/pytoda-1.1.4.tar.gz` & `tmp/pytoda-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytoda-1.1.4.tar", last modified: Tue Mar 19 08:57:16 2024, max compression
+gzip compressed data, was "pytoda-1.1.5.tar", last modified: Fri May 17 12:25:08 2024, max compression
```

## Comparing `pytoda-1.1.4.tar` & `pytoda-1.1.5.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:16.441994 pytoda-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-19 08:57:07.000000 pytoda-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-03-19 08:57:16.441994 pytoda-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-03-19 08:57:07.000000 pytoda-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:16.429993 pytoda-1.1.4/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-19 08:57:07.000000 pytoda-1.1.4/bin/pytoda-filter-invalid-smi
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-19 08:57:07.000000 pytoda-1.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:16.429993 pytoda-1.1.4/pytoda/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/data_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:16.433993 pytoda-1.1.4/pytoda/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/_cache_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/_csv_eager_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/_csv_lazy_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/_csv_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/_fasta_eager_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/_fasta_lazy_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/_smi_eager_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/_smi_lazy_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/_table_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/annotated_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/dataframe_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/distributional_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/drug_affinity_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/drug_sensitivity_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/drug_sensitivity_dose_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/gene_expression_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    13196 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/polymer_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11485 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/protein_protein_interaction_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15900 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/protein_sequence_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15088 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/set_matching_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/smiles_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:16.433993 pytoda-1.1.4/pytoda/datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12927 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/tests/test_annotated_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/tests/test_base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/tests/test_distributional_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/tests/test_drug_affinity_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/tests/test_drug_sensitivity_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/tests/test_drug_sensitivity_dose_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    16233 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/tests/test_gene_expression_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    17009 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/tests/test_polymer_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    22481 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/tests/test_protein_protein_interaction_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    25489 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/tests/test_protein_sequence_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    20797 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/tests/test_set_matching_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    16823 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/tests/test_smiles_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:16.437993 pytoda-1.1.4/pytoda/datasets/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/utils/background_tensors.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/utils/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/datasets/utils/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:16.437993 pytoda-1.1.4/pytoda/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/preprocessing/crawlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/preprocessing/smi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:16.437993 pytoda-1.1.4/pytoda/preprocessing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/preprocessing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/preprocessing/tests/test_crawlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/preprocessing/tests/test_smi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:16.437993 pytoda-1.1.4/pytoda/proteins/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/proteins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:16.437993 pytoda-1.1.4/pytoda/proteins/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/proteins/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   158899 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/proteins/metadata/kinase_activesite_alignment.smi
--rw-r--r--   0 runner    (1001) docker     (127)    19936 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/proteins/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/proteins/protein_feature_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     9304 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/proteins/protein_language.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:16.437993 pytoda-1.1.4/pytoda/proteins/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/proteins/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/proteins/tests/test_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/proteins/tests/test_protein_feature_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/proteins/tests/test_protein_language.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/proteins/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11629 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/proteins/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/proteins/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:16.437993 pytoda-1.1.4/pytoda/smiles/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/smiles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:16.437993 pytoda-1.1.4/pytoda/smiles/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/smiles/metadata/ATTRIBUTION
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/smiles/metadata/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/smiles/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/smiles/metadata/spe_chembl.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:16.441994 pytoda-1.1.4/pytoda/smiles/metadata/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/smiles/metadata/tokenizer/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/smiles/metadata/tokenizer/token_count.json
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/smiles/metadata/tokenizer/tokenizer_config.json
--rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/smiles/metadata/tokenizer/vocab.json
--rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/smiles/polymer_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/smiles/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    37596 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/smiles/smiles_language.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:16.441994 pytoda-1.1.4/pytoda/smiles/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/smiles/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6890 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/smiles/tests/test_polymer_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/smiles/tests/test_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11179 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/smiles/tests/test_smiles_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/smiles/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/smiles/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:16.441994 pytoda-1.1.4/pytoda/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/tests/test_data_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-19 08:57:07.000000 pytoda-1.1.4/pytoda/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 08:57:16.441994 pytoda-1.1.4/pytoda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-03-19 08:57:16.000000 pytoda-1.1.4/pytoda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-03-19 08:57:16.000000 pytoda-1.1.4/pytoda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 08:57:16.000000 pytoda-1.1.4/pytoda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-19 08:57:16.000000 pytoda-1.1.4/pytoda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-19 08:57:16.000000 pytoda-1.1.4/pytoda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-19 08:57:16.441994 pytoda-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-03-19 08:57:07.000000 pytoda-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:25:08.433522 pytoda-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-17 12:24:56.000000 pytoda-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-17 12:25:08.433522 pytoda-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-17 12:24:56.000000 pytoda-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:25:08.421522 pytoda-1.1.5/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-17 12:24:56.000000 pytoda-1.1.5/bin/pytoda-filter-invalid-smi
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-17 12:24:56.000000 pytoda-1.1.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:25:08.421522 pytoda-1.1.5/pytoda/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/data_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:25:08.425522 pytoda-1.1.5/pytoda/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/_cache_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/_csv_eager_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/_csv_lazy_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/_csv_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/_fasta_eager_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/_fasta_lazy_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/_smi_eager_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/_smi_lazy_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/_table_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/annotated_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/dataframe_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/distributional_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/drug_affinity_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/drug_sensitivity_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/drug_sensitivity_dose_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/gene_expression_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13196 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/polymer_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11485 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/protein_protein_interaction_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15900 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/protein_sequence_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15088 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/set_matching_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/smiles_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:25:08.425522 pytoda-1.1.5/pytoda/datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12927 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/tests/test_annotated_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/tests/test_base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/tests/test_distributional_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/tests/test_drug_affinity_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/tests/test_drug_sensitivity_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/tests/test_drug_sensitivity_dose_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16233 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/tests/test_gene_expression_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17009 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/tests/test_polymer_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22481 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/tests/test_protein_protein_interaction_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25489 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/tests/test_protein_sequence_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20797 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/tests/test_set_matching_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16823 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/tests/test_smiles_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:25:08.425522 pytoda-1.1.5/pytoda/datasets/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/utils/background_tensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/utils/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/datasets/utils/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:25:08.429522 pytoda-1.1.5/pytoda/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/preprocessing/crawlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/preprocessing/smi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:25:08.429522 pytoda-1.1.5/pytoda/preprocessing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/preprocessing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/preprocessing/tests/test_crawlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/preprocessing/tests/test_smi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:25:08.429522 pytoda-1.1.5/pytoda/proteins/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/proteins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:25:08.429522 pytoda-1.1.5/pytoda/proteins/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/proteins/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   158899 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/proteins/metadata/kinase_activesite_alignment.smi
+-rw-r--r--   0 runner    (1001) docker     (127)    19936 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/proteins/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/proteins/protein_feature_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9304 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/proteins/protein_language.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:25:08.429522 pytoda-1.1.5/pytoda/proteins/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/proteins/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/proteins/tests/test_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/proteins/tests/test_protein_feature_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/proteins/tests/test_protein_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/proteins/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11629 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/proteins/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/proteins/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:25:08.429522 pytoda-1.1.5/pytoda/smiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/smiles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:25:08.433522 pytoda-1.1.5/pytoda/smiles/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/smiles/metadata/ATTRIBUTION
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/smiles/metadata/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/smiles/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/smiles/metadata/spe_chembl.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:25:08.433522 pytoda-1.1.5/pytoda/smiles/metadata/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/smiles/metadata/tokenizer/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/smiles/metadata/tokenizer/token_count.json
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/smiles/metadata/tokenizer/tokenizer_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/smiles/metadata/tokenizer/vocab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/smiles/polymer_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/smiles/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37596 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/smiles/smiles_language.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:25:08.433522 pytoda-1.1.5/pytoda/smiles/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/smiles/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6890 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/smiles/tests/test_polymer_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/smiles/tests/test_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11179 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/smiles/tests/test_smiles_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/smiles/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/smiles/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:25:08.433522 pytoda-1.1.5/pytoda/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/tests/test_data_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-17 12:24:56.000000 pytoda-1.1.5/pytoda/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:25:08.433522 pytoda-1.1.5/pytoda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-17 12:25:08.000000 pytoda-1.1.5/pytoda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-05-17 12:25:08.000000 pytoda-1.1.5/pytoda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 12:25:08.000000 pytoda-1.1.5/pytoda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-17 12:25:08.000000 pytoda-1.1.5/pytoda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 12:25:08.000000 pytoda-1.1.5/pytoda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-17 12:25:08.433522 pytoda-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-17 12:24:56.000000 pytoda-1.1.5/setup.py
```

### Comparing `pytoda-1.1.4/LICENSE` & `pytoda-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/PKG-INFO` & `pytoda-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytoda
-Version: 1.1.4
+Version: 1.1.5
 Summary: pytoda: PaccMann PyTorch Dataset Classes.
 Home-page: https://github.com/PaccMann/paccmann_datasets
 Author: Matteo Manica, Jannis Born, Joris Cadow
 Author-email: drugilsberg@gmail.com, jannis.born@gmx.de, joriscadow@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -23,15 +23,15 @@
 Requires-Dist: selfies>=2.1.1
 Requires-Dist: upfp
 Requires-Dist: SmilesPE>=0.0.3
 Requires-Dist: pyfaidx
 Requires-Dist: pubchempy
 Requires-Dist: importlib_resources
 Requires-Dist: Unidecode
-Requires-Dist: rdkit-pypi>=2021.9.3
+Requires-Dist: rdkit
 
 # PyToDa
 
 [![PyPI version](https://badge.fury.io/py/pytoda.svg)](https://badge.fury.io/py/pytoda)
 [![build](https://github.com/PaccMann/paccmann_datasets/workflows/build/badge.svg)](https://github.com/PaccMann/paccmann_datasets/actions)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `pytoda-1.1.4/README.md` & `pytoda-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/bin/pytoda-filter-invalid-smi` & `pytoda-1.1.5/bin/pytoda-filter-invalid-smi`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/data_splitter.py` & `pytoda-1.1.5/pytoda/data_splitter.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/__init__.py` & `pytoda-1.1.5/pytoda/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/_cache_datasource.py` & `pytoda-1.1.5/pytoda/datasets/_cache_datasource.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/_csv_eager_dataset.py` & `pytoda-1.1.5/pytoda/datasets/_csv_eager_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/_csv_lazy_dataset.py` & `pytoda-1.1.5/pytoda/datasets/_csv_lazy_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/_csv_statistics.py` & `pytoda-1.1.5/pytoda/datasets/_csv_statistics.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/_fasta_eager_dataset.py` & `pytoda-1.1.5/pytoda/datasets/_fasta_eager_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/_fasta_lazy_dataset.py` & `pytoda-1.1.5/pytoda/datasets/_fasta_lazy_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/_smi_eager_dataset.py` & `pytoda-1.1.5/pytoda/datasets/_smi_eager_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/_smi_lazy_dataset.py` & `pytoda-1.1.5/pytoda/datasets/_smi_lazy_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/_table_dataset.py` & `pytoda-1.1.5/pytoda/datasets/_table_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/annotated_dataset.py` & `pytoda-1.1.5/pytoda/datasets/annotated_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/base_dataset.py` & `pytoda-1.1.5/pytoda/datasets/base_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/dataframe_dataset.py` & `pytoda-1.1.5/pytoda/datasets/dataframe_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/distributional_dataset.py` & `pytoda-1.1.5/pytoda/datasets/distributional_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/drug_affinity_dataset.py` & `pytoda-1.1.5/pytoda/datasets/drug_affinity_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/drug_sensitivity_dataset.py` & `pytoda-1.1.5/pytoda/datasets/drug_sensitivity_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/drug_sensitivity_dose_dataset.py` & `pytoda-1.1.5/pytoda/datasets/drug_sensitivity_dose_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/gene_expression_dataset.py` & `pytoda-1.1.5/pytoda/datasets/gene_expression_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/polymer_dataset.py` & `pytoda-1.1.5/pytoda/datasets/polymer_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/protein_protein_interaction_dataset.py` & `pytoda-1.1.5/pytoda/datasets/protein_protein_interaction_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/protein_sequence_dataset.py` & `pytoda-1.1.5/pytoda/datasets/protein_sequence_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/set_matching_dataset.py` & `pytoda-1.1.5/pytoda/datasets/set_matching_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/smiles_dataset.py` & `pytoda-1.1.5/pytoda/datasets/smiles_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/tests/test_annotated_dataset.py` & `pytoda-1.1.5/pytoda/datasets/tests/test_annotated_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/tests/test_base_dataset.py` & `pytoda-1.1.5/pytoda/datasets/tests/test_base_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/tests/test_distributional_dataset.py` & `pytoda-1.1.5/pytoda/datasets/tests/test_distributional_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/tests/test_drug_affinity_dataset.py` & `pytoda-1.1.5/pytoda/datasets/tests/test_drug_affinity_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/tests/test_drug_sensitivity_dataset.py` & `pytoda-1.1.5/pytoda/datasets/tests/test_drug_sensitivity_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/tests/test_drug_sensitivity_dose_dataset.py` & `pytoda-1.1.5/pytoda/datasets/tests/test_drug_sensitivity_dose_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/tests/test_gene_expression_dataset.py` & `pytoda-1.1.5/pytoda/datasets/tests/test_gene_expression_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/tests/test_polymer_dataset.py` & `pytoda-1.1.5/pytoda/datasets/tests/test_polymer_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/tests/test_protein_protein_interaction_dataset.py` & `pytoda-1.1.5/pytoda/datasets/tests/test_protein_protein_interaction_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/tests/test_protein_sequence_dataset.py` & `pytoda-1.1.5/pytoda/datasets/tests/test_protein_sequence_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/tests/test_set_matching_dataset.py` & `pytoda-1.1.5/pytoda/datasets/tests/test_set_matching_dataset.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/tests/test_smiles_datasets.py` & `pytoda-1.1.5/pytoda/datasets/tests/test_smiles_datasets.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/utils/background_tensors.py` & `pytoda-1.1.5/pytoda/datasets/utils/background_tensors.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/utils/factories.py` & `pytoda-1.1.5/pytoda/datasets/utils/factories.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/utils/utils.py` & `pytoda-1.1.5/pytoda/datasets/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/datasets/utils/wrappers.py` & `pytoda-1.1.5/pytoda/datasets/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/files.py` & `pytoda-1.1.5/pytoda/files.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/preprocessing/crawlers.py` & `pytoda-1.1.5/pytoda/preprocessing/crawlers.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/preprocessing/smi.py` & `pytoda-1.1.5/pytoda/preprocessing/smi.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/preprocessing/tests/test_crawlers.py` & `pytoda-1.1.5/pytoda/preprocessing/tests/test_crawlers.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/preprocessing/tests/test_smi.py` & `pytoda-1.1.5/pytoda/preprocessing/tests/test_smi.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/proteins/metadata/kinase_activesite_alignment.smi` & `pytoda-1.1.5/pytoda/proteins/metadata/kinase_activesite_alignment.smi`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/proteins/processing.py` & `pytoda-1.1.5/pytoda/proteins/processing.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/proteins/protein_feature_language.py` & `pytoda-1.1.5/pytoda/proteins/protein_feature_language.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/proteins/protein_language.py` & `pytoda-1.1.5/pytoda/proteins/protein_language.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/proteins/tests/test_processing.py` & `pytoda-1.1.5/pytoda/proteins/tests/test_processing.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/proteins/tests/test_protein_feature_language.py` & `pytoda-1.1.5/pytoda/proteins/tests/test_protein_feature_language.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/proteins/tests/test_protein_language.py` & `pytoda-1.1.5/pytoda/proteins/tests/test_protein_language.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/proteins/tests/test_utils.py` & `pytoda-1.1.5/pytoda/proteins/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/proteins/transforms.py` & `pytoda-1.1.5/pytoda/proteins/transforms.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/proteins/utils.py` & `pytoda-1.1.5/pytoda/proteins/utils.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/smiles/metadata/ATTRIBUTION` & `pytoda-1.1.5/pytoda/smiles/metadata/ATTRIBUTION`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/smiles/metadata/README.md` & `pytoda-1.1.5/pytoda/smiles/metadata/README.md`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/smiles/metadata/spe_chembl.txt` & `pytoda-1.1.5/pytoda/smiles/metadata/spe_chembl.txt`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/smiles/metadata/tokenizer/token_count.json` & `pytoda-1.1.5/pytoda/smiles/metadata/tokenizer/token_count.json`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/smiles/metadata/tokenizer/vocab.json` & `pytoda-1.1.5/pytoda/smiles/metadata/tokenizer/vocab.json`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/smiles/polymer_language.py` & `pytoda-1.1.5/pytoda/smiles/polymer_language.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/smiles/processing.py` & `pytoda-1.1.5/pytoda/smiles/processing.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/smiles/smiles_language.py` & `pytoda-1.1.5/pytoda/smiles/smiles_language.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/smiles/tests/test_polymer_language.py` & `pytoda-1.1.5/pytoda/smiles/tests/test_polymer_language.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/smiles/tests/test_processing.py` & `pytoda-1.1.5/pytoda/smiles/tests/test_processing.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/smiles/tests/test_smiles_language.py` & `pytoda-1.1.5/pytoda/smiles/tests/test_smiles_language.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/smiles/tests/test_transforms.py` & `pytoda-1.1.5/pytoda/smiles/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/smiles/transforms.py` & `pytoda-1.1.5/pytoda/smiles/transforms.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/tests/test_data_splitter.py` & `pytoda-1.1.5/pytoda/tests/test_data_splitter.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/tests/test_files.py` & `pytoda-1.1.5/pytoda/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/tests/test_transforms.py` & `pytoda-1.1.5/pytoda/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/tests/utils.py` & `pytoda-1.1.5/pytoda/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/transforms.py` & `pytoda-1.1.5/pytoda/transforms.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/types.py` & `pytoda-1.1.5/pytoda/types.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda/warnings.py` & `pytoda-1.1.5/pytoda/warnings.py`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/pytoda.egg-info/PKG-INFO` & `pytoda-1.1.5/pytoda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytoda
-Version: 1.1.4
+Version: 1.1.5
 Summary: pytoda: PaccMann PyTorch Dataset Classes.
 Home-page: https://github.com/PaccMann/paccmann_datasets
 Author: Matteo Manica, Jannis Born, Joris Cadow
 Author-email: drugilsberg@gmail.com, jannis.born@gmx.de, joriscadow@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -23,15 +23,15 @@
 Requires-Dist: selfies>=2.1.1
 Requires-Dist: upfp
 Requires-Dist: SmilesPE>=0.0.3
 Requires-Dist: pyfaidx
 Requires-Dist: pubchempy
 Requires-Dist: importlib_resources
 Requires-Dist: Unidecode
-Requires-Dist: rdkit-pypi>=2021.9.3
+Requires-Dist: rdkit
 
 # PyToDa
 
 [![PyPI version](https://badge.fury.io/py/pytoda.svg)](https://badge.fury.io/py/pytoda)
 [![build](https://github.com/PaccMann/paccmann_datasets/workflows/build/badge.svg)](https://github.com/PaccMann/paccmann_datasets/actions)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `pytoda-1.1.4/pytoda.egg-info/SOURCES.txt` & `pytoda-1.1.5/pytoda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytoda-1.1.4/setup.py` & `pytoda-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         'selfies>=2.1.1',
         'upfp',
         'SmilesPE>=0.0.3',
         'pyfaidx',
         'pubchempy',
         'importlib_resources',
         'Unidecode',
-        'rdkit-pypi>=2021.9.3',
+        'rdkit',
     ],
     classifiers=[
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
```

