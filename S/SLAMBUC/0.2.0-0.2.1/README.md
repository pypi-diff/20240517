# Comparing `tmp/SLAMBUC-0.2.0.tar.gz` & `tmp/SLAMBUC-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SLAMBUC-0.2.0.tar", last modified: Mon Jul 17 15:27:22 2023, max compression
+gzip compressed data, was "SLAMBUC-0.2.1.tar", last modified: Wed Sep  6 16:40:59 2023, max compression
```

## Comparing `SLAMBUC-0.2.0.tar` & `SLAMBUC-0.2.1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.138270 SLAMBUC-0.2.0/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    11357 2023-06-30 19:22:13.000000 SLAMBUC-0.2.0/LICENSE
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    13287 2023-07-17 15:27:22.138270 SLAMBUC-0.2.0/PKG-INFO
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    12301 2023-07-17 15:20:23.000000 SLAMBUC-0.2.0/README.md
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.126269 SLAMBUC-0.2.0/SLAMBUC.egg-info/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    13287 2023-07-17 15:27:22.000000 SLAMBUC-0.2.0/SLAMBUC.egg-info/PKG-INFO
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     2316 2023-07-17 15:27:22.000000 SLAMBUC-0.2.0/SLAMBUC.egg-info/SOURCES.txt
--rw-rw-r--   0 czentye   (1000) czentye   (1000)        1 2023-07-17 15:27:22.000000 SLAMBUC-0.2.0/SLAMBUC.egg-info/dependency_links.txt
--rw-rw-r--   0 czentye   (1000) czentye   (1000)        1 2023-07-17 15:27:21.000000 SLAMBUC-0.2.0/SLAMBUC.egg-info/not-zip-safe
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      226 2023-07-17 15:27:22.000000 SLAMBUC-0.2.0/SLAMBUC.egg-info/requires.txt
--rw-rw-r--   0 czentye   (1000) czentye   (1000)       18 2023-07-17 15:27:22.000000 SLAMBUC-0.2.0/SLAMBUC.egg-info/top_level.txt
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     1948 2023-07-10 20:36:21.000000 SLAMBUC-0.2.0/pyproject.toml
--rw-rw-r--   0 czentye   (1000) czentye   (1000)       38 2023-07-17 15:27:22.138270 SLAMBUC-0.2.0/setup.cfg
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     2414 2023-07-17 15:22:22.000000 SLAMBUC-0.2.0/setup.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.126269 SLAMBUC-0.2.0/slambuc/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      596 2023-07-17 15:22:13.000000 SLAMBUC-0.2.0/slambuc/__init__.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.126269 SLAMBUC-0.2.0/slambuc/alg/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     1488 2023-07-17 14:17:13.000000 SLAMBUC-0.2.0/slambuc/alg/__init__.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.126269 SLAMBUC-0.2.0/slambuc/alg/chain/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      611 2023-07-05 20:30:38.000000 SLAMBUC-0.2.0/slambuc/alg/chain/__init__.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.126269 SLAMBUC-0.2.0/slambuc/alg/chain/dp/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      720 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/alg/chain/dp/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     3531 2023-07-14 09:45:49.000000 SLAMBUC-0.2.0/slambuc/alg/chain/dp/greedy.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     6082 2023-07-14 12:53:11.000000 SLAMBUC-0.2.0/slambuc/alg/chain/dp/min.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    13948 2023-07-14 12:26:08.000000 SLAMBUC-0.2.0/slambuc/alg/chain/dp/mtx.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.126269 SLAMBUC-0.2.0/slambuc/alg/chain/ser/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      688 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/alg/chain/ser/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     3455 2023-07-14 09:45:49.000000 SLAMBUC-0.2.0/slambuc/alg/chain/ser/greedy.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    12538 2023-07-14 09:55:33.000000 SLAMBUC-0.2.0/slambuc/alg/chain/ser/ilp.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.126269 SLAMBUC-0.2.0/slambuc/alg/ext/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      956 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/alg/ext/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     2432 2023-07-14 12:04:55.000000 SLAMBUC-0.2.0/slambuc/alg/ext/baseline.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    11000 2023-07-14 12:11:51.000000 SLAMBUC-0.2.0/slambuc/alg/ext/csp.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     8901 2023-07-14 12:12:50.000000 SLAMBUC-0.2.0/slambuc/alg/ext/greedy.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     7569 2023-07-14 12:15:57.000000 SLAMBUC-0.2.0/slambuc/alg/ext/min_cut.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.126269 SLAMBUC-0.2.0/slambuc/alg/service/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      646 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/alg/service/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     1581 2023-07-17 15:18:02.000000 SLAMBUC-0.2.0/slambuc/alg/service/common.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.126269 SLAMBUC-0.2.0/slambuc/alg/tree/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      652 2023-07-14 13:43:20.000000 SLAMBUC-0.2.0/slambuc/alg/tree/__init__.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.130269 SLAMBUC-0.2.0/slambuc/alg/tree/dp/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      738 2023-07-14 12:23:04.000000 SLAMBUC-0.2.0/slambuc/alg/tree/dp/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     6571 2023-07-14 15:03:47.000000 SLAMBUC-0.2.0/slambuc/alg/tree/dp/greedy.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    10080 2023-07-14 15:03:47.000000 SLAMBUC-0.2.0/slambuc/alg/tree/dp/meta.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     8311 2023-07-14 15:03:47.000000 SLAMBUC-0.2.0/slambuc/alg/tree/dp/min.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    10608 2023-07-14 15:03:47.000000 SLAMBUC-0.2.0/slambuc/alg/tree/dp/seq.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     3512 2023-07-14 15:03:47.000000 SLAMBUC-0.2.0/slambuc/alg/tree/dp/seq_state.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.130269 SLAMBUC-0.2.0/slambuc/alg/tree/layout/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      678 2023-07-14 13:31:02.000000 SLAMBUC-0.2.0/slambuc/alg/tree/layout/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    15230 2023-07-14 15:03:47.000000 SLAMBUC-0.2.0/slambuc/alg/tree/layout/ilp.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.130269 SLAMBUC-0.2.0/slambuc/alg/tree/par/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      880 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/alg/tree/par/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     3964 2023-07-14 15:03:47.000000 SLAMBUC-0.2.0/slambuc/alg/tree/par/greedy.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    20165 2023-07-14 15:09:47.000000 SLAMBUC-0.2.0/slambuc/alg/tree/par/ilp.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    19075 2023-07-14 15:19:54.000000 SLAMBUC-0.2.0/slambuc/alg/tree/par/pseudo.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    14051 2023-07-14 15:28:59.000000 SLAMBUC-0.2.0/slambuc/alg/tree/par/pseudo_mp.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.130269 SLAMBUC-0.2.0/slambuc/alg/tree/ser/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     1006 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/alg/tree/ser/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    39042 2023-07-14 15:05:26.000000 SLAMBUC-0.2.0/slambuc/alg/tree/ser/bicriteria.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     3807 2023-07-14 15:05:26.000000 SLAMBUC-0.2.0/slambuc/alg/tree/ser/greedy.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    20792 2023-07-14 15:12:10.000000 SLAMBUC-0.2.0/slambuc/alg/tree/ser/ilp.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    13015 2023-07-14 15:17:56.000000 SLAMBUC-0.2.0/slambuc/alg/tree/ser/ilp_cplex.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    16298 2023-07-14 15:31:33.000000 SLAMBUC-0.2.0/slambuc/alg/tree/ser/pseudo.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    26917 2023-07-14 15:36:32.000000 SLAMBUC-0.2.0/slambuc/alg/tree/ser/pseudo_mp.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    37129 2023-07-17 15:01:40.000000 SLAMBUC-0.2.0/slambuc/alg/util.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.130269 SLAMBUC-0.2.0/slambuc/gen/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      647 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/gen/__init__.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.130269 SLAMBUC-0.2.0/slambuc/gen/cluster/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      642 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/__init__.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.134269 SLAMBUC-0.2.0/slambuc/gen/cluster/hist/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     2214 2023-03-09 09:23:00.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/hist/cpl_hist.pkl
--rw-rw-r--   0 czentye   (1000) czentye   (1000)   255904 2023-03-09 12:08:00.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/hist/instance_num_hist.pkl
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     1419 2023-03-09 09:24:00.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/hist/level_hist.pkl
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      429 2023-03-09 09:28:00.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/hist/task_cpu_hist.pkl
--rw-rw-r--   0 czentye   (1000) czentye   (1000)   212962 2023-03-09 09:27:00.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/hist/task_duration_hist.pkl
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     2557 2023-03-09 09:30:00.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/hist/task_mem_hist.pkl
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     4077 2023-03-09 09:25:00.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/hist/task_num_hist.pkl
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     9982 2023-07-17 06:38:45.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/job_tree.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.134269 SLAMBUC-0.2.0/slambuc/gen/cluster/samples/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)   245994 2023-03-06 16:52:01.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/samples/batch_task.csv
--rw-rw-r--   0 czentye   (1000) czentye   (1000)  2397573 2023-03-01 10:28:19.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/samples/sample_tasks.csv
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     4094 2023-07-17 06:33:18.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/syn_job.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     5021 2023-07-17 07:03:22.000000 SLAMBUC-0.2.0/slambuc/gen/io.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.138270 SLAMBUC-0.2.0/slambuc/gen/microservice/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      643 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/gen/microservice/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     5425 2023-07-17 06:38:45.000000 SLAMBUC-0.2.0/slambuc/gen/microservice/faas_tree.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.138270 SLAMBUC-0.2.0/slambuc/gen/microservice/hist/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      865 2023-03-16 12:15:00.000000 SLAMBUC-0.2.0/slambuc/gen/microservice/hist/func_inv_rate_hist.pkl
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      897 2023-03-16 12:26:00.000000 SLAMBUC-0.2.0/slambuc/gen/microservice/hist/rw_overhead_hist.pkl
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     3489 2023-07-17 06:50:42.000000 SLAMBUC-0.2.0/slambuc/gen/microservice/power_ba_graph.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.138270 SLAMBUC-0.2.0/slambuc/gen/random/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      643 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/gen/random/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     2981 2023-07-17 06:54:00.000000 SLAMBUC-0.2.0/slambuc/gen/random/random_tree.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     3202 2023-07-17 07:09:04.000000 SLAMBUC-0.2.0/slambuc/gen/transform.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.138270 SLAMBUC-0.2.0/slambuc/misc/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      574 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/misc/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     3963 2023-07-17 07:11:05.000000 SLAMBUC-0.2.0/slambuc/misc/generator.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     6655 2023-07-17 07:18:15.000000 SLAMBUC-0.2.0/slambuc/misc/plot.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    28204 2023-07-17 14:17:13.000000 SLAMBUC-0.2.0/slambuc/misc/util.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.188498 SLAMBUC-0.2.1/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    11357 2023-06-30 19:22:13.000000 SLAMBUC-0.2.1/LICENSE
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    13286 2023-09-06 16:40:59.188498 SLAMBUC-0.2.1/PKG-INFO
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    12300 2023-07-20 14:07:33.000000 SLAMBUC-0.2.1/README.md
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.176498 SLAMBUC-0.2.1/SLAMBUC.egg-info/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    13286 2023-09-06 16:40:59.000000 SLAMBUC-0.2.1/SLAMBUC.egg-info/PKG-INFO
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     2316 2023-09-06 16:40:59.000000 SLAMBUC-0.2.1/SLAMBUC.egg-info/SOURCES.txt
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)        1 2023-09-06 16:40:59.000000 SLAMBUC-0.2.1/SLAMBUC.egg-info/dependency_links.txt
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)        1 2023-09-06 16:40:58.000000 SLAMBUC-0.2.1/SLAMBUC.egg-info/not-zip-safe
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      258 2023-09-06 16:40:59.000000 SLAMBUC-0.2.1/SLAMBUC.egg-info/requires.txt
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)       18 2023-09-06 16:40:59.000000 SLAMBUC-0.2.1/SLAMBUC.egg-info/top_level.txt
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     2186 2023-07-19 12:22:41.000000 SLAMBUC-0.2.1/pyproject.toml
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)       38 2023-09-06 16:40:59.188498 SLAMBUC-0.2.1/setup.cfg
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     2513 2023-07-19 15:17:18.000000 SLAMBUC-0.2.1/setup.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.176498 SLAMBUC-0.2.1/slambuc/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      596 2023-07-19 16:33:49.000000 SLAMBUC-0.2.1/slambuc/__init__.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.176498 SLAMBUC-0.2.1/slambuc/alg/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     1488 2023-07-17 14:17:13.000000 SLAMBUC-0.2.1/slambuc/alg/__init__.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.176498 SLAMBUC-0.2.1/slambuc/alg/chain/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      611 2023-07-05 20:30:38.000000 SLAMBUC-0.2.1/slambuc/alg/chain/__init__.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.176498 SLAMBUC-0.2.1/slambuc/alg/chain/dp/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      720 2023-07-03 16:04:48.000000 SLAMBUC-0.2.1/slambuc/alg/chain/dp/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     3531 2023-07-14 09:45:49.000000 SLAMBUC-0.2.1/slambuc/alg/chain/dp/greedy.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     6082 2023-07-14 12:53:11.000000 SLAMBUC-0.2.1/slambuc/alg/chain/dp/min.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    13948 2023-07-14 12:26:08.000000 SLAMBUC-0.2.1/slambuc/alg/chain/dp/mtx.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.176498 SLAMBUC-0.2.1/slambuc/alg/chain/ser/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      688 2023-07-03 16:04:48.000000 SLAMBUC-0.2.1/slambuc/alg/chain/ser/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     3455 2023-07-14 09:45:49.000000 SLAMBUC-0.2.1/slambuc/alg/chain/ser/greedy.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    12538 2023-07-14 09:55:33.000000 SLAMBUC-0.2.1/slambuc/alg/chain/ser/ilp.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.176498 SLAMBUC-0.2.1/slambuc/alg/ext/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      956 2023-07-03 16:04:48.000000 SLAMBUC-0.2.1/slambuc/alg/ext/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     2432 2023-07-14 12:04:55.000000 SLAMBUC-0.2.1/slambuc/alg/ext/baseline.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    11000 2023-07-14 12:11:51.000000 SLAMBUC-0.2.1/slambuc/alg/ext/csp.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     8901 2023-07-14 12:12:50.000000 SLAMBUC-0.2.1/slambuc/alg/ext/greedy.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     7569 2023-07-14 12:15:57.000000 SLAMBUC-0.2.1/slambuc/alg/ext/min_cut.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.176498 SLAMBUC-0.2.1/slambuc/alg/service/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      646 2023-07-03 16:04:48.000000 SLAMBUC-0.2.1/slambuc/alg/service/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     1583 2023-07-19 05:50:13.000000 SLAMBUC-0.2.1/slambuc/alg/service/common.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.180498 SLAMBUC-0.2.1/slambuc/alg/tree/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      652 2023-07-14 13:43:20.000000 SLAMBUC-0.2.1/slambuc/alg/tree/__init__.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.180498 SLAMBUC-0.2.1/slambuc/alg/tree/dp/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      738 2023-07-14 12:23:04.000000 SLAMBUC-0.2.1/slambuc/alg/tree/dp/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     6571 2023-07-14 15:03:47.000000 SLAMBUC-0.2.1/slambuc/alg/tree/dp/greedy.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    10080 2023-07-14 15:03:47.000000 SLAMBUC-0.2.1/slambuc/alg/tree/dp/meta.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     8311 2023-07-14 15:03:47.000000 SLAMBUC-0.2.1/slambuc/alg/tree/dp/min.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    10608 2023-07-14 15:03:47.000000 SLAMBUC-0.2.1/slambuc/alg/tree/dp/seq.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     3512 2023-07-14 15:03:47.000000 SLAMBUC-0.2.1/slambuc/alg/tree/dp/seq_state.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.180498 SLAMBUC-0.2.1/slambuc/alg/tree/layout/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      678 2023-07-14 13:31:02.000000 SLAMBUC-0.2.1/slambuc/alg/tree/layout/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    15230 2023-07-19 05:51:09.000000 SLAMBUC-0.2.1/slambuc/alg/tree/layout/ilp.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.180498 SLAMBUC-0.2.1/slambuc/alg/tree/par/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      880 2023-07-03 16:04:48.000000 SLAMBUC-0.2.1/slambuc/alg/tree/par/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     3964 2023-07-14 15:03:47.000000 SLAMBUC-0.2.1/slambuc/alg/tree/par/greedy.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    20165 2023-07-14 15:09:47.000000 SLAMBUC-0.2.1/slambuc/alg/tree/par/ilp.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    19075 2023-07-14 15:19:54.000000 SLAMBUC-0.2.1/slambuc/alg/tree/par/pseudo.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    14051 2023-07-14 15:28:59.000000 SLAMBUC-0.2.1/slambuc/alg/tree/par/pseudo_mp.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.180498 SLAMBUC-0.2.1/slambuc/alg/tree/ser/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     1006 2023-07-03 16:04:48.000000 SLAMBUC-0.2.1/slambuc/alg/tree/ser/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    39042 2023-07-14 15:05:26.000000 SLAMBUC-0.2.1/slambuc/alg/tree/ser/bicriteria.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     3807 2023-07-14 15:05:26.000000 SLAMBUC-0.2.1/slambuc/alg/tree/ser/greedy.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    20792 2023-07-14 15:12:10.000000 SLAMBUC-0.2.1/slambuc/alg/tree/ser/ilp.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    13015 2023-07-14 15:17:56.000000 SLAMBUC-0.2.1/slambuc/alg/tree/ser/ilp_cplex.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    16298 2023-07-14 15:31:33.000000 SLAMBUC-0.2.1/slambuc/alg/tree/ser/pseudo.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    26965 2023-07-19 11:00:10.000000 SLAMBUC-0.2.1/slambuc/alg/tree/ser/pseudo_mp.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    37129 2023-07-17 15:01:40.000000 SLAMBUC-0.2.1/slambuc/alg/util.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.180498 SLAMBUC-0.2.1/slambuc/gen/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      647 2023-07-03 16:04:48.000000 SLAMBUC-0.2.1/slambuc/gen/__init__.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.184498 SLAMBUC-0.2.1/slambuc/gen/cluster/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      642 2023-07-03 16:04:48.000000 SLAMBUC-0.2.1/slambuc/gen/cluster/__init__.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.184498 SLAMBUC-0.2.1/slambuc/gen/cluster/hist/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     2214 2023-03-09 09:23:00.000000 SLAMBUC-0.2.1/slambuc/gen/cluster/hist/cpl_hist.pkl
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)   255904 2023-03-09 12:08:00.000000 SLAMBUC-0.2.1/slambuc/gen/cluster/hist/instance_num_hist.pkl
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     1419 2023-03-09 09:24:00.000000 SLAMBUC-0.2.1/slambuc/gen/cluster/hist/level_hist.pkl
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      429 2023-03-09 09:28:00.000000 SLAMBUC-0.2.1/slambuc/gen/cluster/hist/task_cpu_hist.pkl
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)   212962 2023-03-09 09:27:00.000000 SLAMBUC-0.2.1/slambuc/gen/cluster/hist/task_duration_hist.pkl
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     2557 2023-03-09 09:30:00.000000 SLAMBUC-0.2.1/slambuc/gen/cluster/hist/task_mem_hist.pkl
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     4077 2023-03-09 09:25:00.000000 SLAMBUC-0.2.1/slambuc/gen/cluster/hist/task_num_hist.pkl
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    10012 2023-07-20 16:48:32.000000 SLAMBUC-0.2.1/slambuc/gen/cluster/job_tree.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.184498 SLAMBUC-0.2.1/slambuc/gen/cluster/samples/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)   245994 2023-03-06 16:52:01.000000 SLAMBUC-0.2.1/slambuc/gen/cluster/samples/batch_task.csv
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)  2397573 2023-03-01 10:28:19.000000 SLAMBUC-0.2.1/slambuc/gen/cluster/samples/sample_tasks.csv
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     4133 2023-07-20 16:52:30.000000 SLAMBUC-0.2.1/slambuc/gen/cluster/syn_job.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     5021 2023-07-17 07:03:22.000000 SLAMBUC-0.2.1/slambuc/gen/io.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.188498 SLAMBUC-0.2.1/slambuc/gen/microservice/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      643 2023-07-03 16:04:48.000000 SLAMBUC-0.2.1/slambuc/gen/microservice/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     5496 2023-07-20 16:45:18.000000 SLAMBUC-0.2.1/slambuc/gen/microservice/faas_tree.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.188498 SLAMBUC-0.2.1/slambuc/gen/microservice/hist/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      865 2023-03-16 12:15:00.000000 SLAMBUC-0.2.1/slambuc/gen/microservice/hist/func_inv_rate_hist.pkl
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      897 2023-03-16 12:26:00.000000 SLAMBUC-0.2.1/slambuc/gen/microservice/hist/rw_overhead_hist.pkl
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     3489 2023-07-17 06:50:42.000000 SLAMBUC-0.2.1/slambuc/gen/microservice/power_ba_graph.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.188498 SLAMBUC-0.2.1/slambuc/gen/random/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      643 2023-07-03 16:04:48.000000 SLAMBUC-0.2.1/slambuc/gen/random/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     2981 2023-07-17 06:54:00.000000 SLAMBUC-0.2.1/slambuc/gen/random/random_tree.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     3202 2023-07-17 07:09:04.000000 SLAMBUC-0.2.1/slambuc/gen/transform.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-09-06 16:40:59.188498 SLAMBUC-0.2.1/slambuc/misc/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      574 2023-07-03 16:04:48.000000 SLAMBUC-0.2.1/slambuc/misc/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     3963 2023-07-17 07:11:05.000000 SLAMBUC-0.2.1/slambuc/misc/generator.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     6655 2023-07-17 07:18:15.000000 SLAMBUC-0.2.1/slambuc/misc/plot.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    28665 2023-07-19 16:03:54.000000 SLAMBUC-0.2.1/slambuc/misc/util.py
```

### Comparing `SLAMBUC-0.2.0/LICENSE` & `SLAMBUC-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/PKG-INFO` & `SLAMBUC-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SLAMBUC
-Version: 0.2.0
+Version: 0.2.1
 Summary: Serverless Layout Adaptation with Memory-Bounds and User Constraints
 Author: Janos Czentye
 Author-email: Janos Czentye <czentye@tmit.bme.hu>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/hsnlab/SLAMBUC
 Project-URL: Homepage, https://github.com/hsnlab/SLAMBUC/wiki
 Project-URL: Issue Tracker, https://github.com/hsnlab/SLAMBUC/issues
@@ -21,19 +21,20 @@
 Provides-Extra: tests
 Provides-Extra: validation
 Provides-Extra: doc
 License-File: LICENSE
 
 # Serverless Layout Adaptation with Memory-Bounds and User Constraints (SLAMBUC)
 
-![PyPI](https://img.shields.io/pypi/v/SLAMBUC)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/SLAMBUC)
-![PyPI - License](https://img.shields.io/pypi/l/SLAMBUC)
-![Algorithm tests](https://github.com/hsnlab/SLAMBUC/actions/workflows/python-alg-tests.yml/badge.svg?branch=main)
-
+[![PyPI](https://img.shields.io/pypi/v/SLAMBUC)](https://pypi.org/project/SLAMBUC/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/SLAMBUC)](https://pypi.org/project/SLAMBUC/#history)
+[![Downloads](https://static.pepy.tech/badge/slambuc)](https://pepy.tech/project/slambuc)
+[![PyPI - License](https://img.shields.io/pypi/l/SLAMBUC)](LICENSE)
+[![pytest](https://github.com/hsnlab/SLAMBUC/actions/workflows/python-alg-tests.yml/badge.svg?branch=main)](https://github.com/hsnlab/SLAMBUC/actions/workflows/python-alg-tests.yml)
+[![Algorithm validations](https://github.com/hsnlab/SLAMBUC/actions/workflows/python-alg-validation.yml/badge.svg?branch=main)](https://github.com/hsnlab/SLAMBUC/actions/workflows/python-alg-validation.yml)
 
 Collection of graph partitioning algorithms implemented in Python for composing cloud-native
 applications from standalone serverless functions in a cost-efficient and latency-constrained manner.
 
 ## Overview
 
 In the context of serverless computing, function fusion is a novel, high-level approach to improve
@@ -127,86 +128,83 @@
 To install additional dependencies, run the following commands.
 
 ```bash
 python3.11 -m pip install slambuc[tests]      # For executing tests
 python3.11 -m pip install slambuc[validation] # For using our test harness framework
 ```
 
-## Package structure
-
-* [slambuc](slambuc) - [Main package]
-    * [alg](slambuc/alg) - [algorithms]
-        * [chain](slambuc/alg/chain) - [Single Chain Partitioning]
-            * [dp](slambuc/alg/chain/dp) - [dynamic programming]
-            * [ser](slambuc/alg/chain/ser) - [linear programming]
-        * [ext](slambuc/alg/ext) - [External algorithms and Baselines]
-        * [service](slambuc/alg/service) - [Service Properties]
-        * [tree](slambuc/alg/tree) - [Tree Partitioning]
-            * [dp](slambuc/alg/tree/dp) - [chain-based algorithms]
-            * [layout](slambuc/alg/tree/layout) - [general partitioning]
-            * [par](slambuc/alg/tree/par) - [parallel executions models]
-            * [ser](slambuc/alg/tree/ser) - [serialized execution models]
-    * [gen](slambuc/gen) - [Input Generators]
-        * [cluster](slambuc/gen/cluster) - [data-parallel job trees]
-        * [microservice](slambuc/gen/microservice) - [serverless trees]
-        * [random](slambuc/gen/random) - [random trees]
-    * [misc](slambuc/misc) - [Miscellaneous utility codes]
-* [tests](tests) - [tests]
-* [validation](validation) - [Validation Framework]
-    * [data](validation/data) - [generated test data]
-    * [results](validation/results) - [measured result files]
-
 ## Usage
 
-Refer to the wiki for [formats, execution parameters, and examples](https://github.com/hsnlab/SLAMBUC/wiki).
+Refer to the wiki for [formats, execution parameters, examples, and API documentation](https://github.com/hsnlab/SLAMBUC/wiki).
 
 ## Example
 
+```python
+from slambuc.alg.tree.ser.pseudo import pseudo_ltree_partitioning
+from slambuc.misc.generator import get_random_tree
+
+# Get input parameters
+tree = get_random_tree(nodes=10)
+params = dict(tree=tree,
+              root=1,
+              M=6,
+              L=450,
+              cp_end=10,
+              delay=10)
+
+# Partitioning
+res = pseudo_ltree_partitioning(**params)
+print(f"Part: {res[0]}, opt. cost: {res[1]}, latency: {res[2]}")
+"Part: [[1, 2], [3, 4], [5, 6, 7, 8], [9], [10]], opt. cost: 1252, latency: 449"
+```
+
+## Algorithms
+
 Validation results of a subset of our algorithms with a fully-serialized block execution model,
 which are executed with our [validation script](tests/validate_algs.py) using different configurations 
 and a [random-generated input call graph](tests/data/graph_test_tree_ser.gml) of size 10.
 
 Used algorithmic parameters (if applicable):
   * Root node ID (root): 1
   * Memory limit (M): 6
   * Available vCPU count (N): 1
   * Critical path's end node ID (cp_end): 10 
-  * Latency limit: (L): inf
+  * Latency limit: (L): **500**
   * Platform delay: (delay): 10
   * Bidirectional elimination (bidirectional): True
   * Cost approximation ratio (Epsilon): 0.0
   * Latency violation ratio (Lambda): 0.0
 
 Exact algorithms are configured to yield all optimal solutions (if exists) with the numerating 
 format `{alg}_{num}`.
 
 Execution results:
 
-| Algorithm            | Partitioning                                        |   Cost |   Latency |   Time (s) |
-|----------------------|-----------------------------------------------------|--------|-----------|------------|
-| GREEDY_0             | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.0235749  |
-| GREEDY_1             | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0235749  |
-| GREEDY_2             | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.0235749  |
-| ILP_CFG_HYBRID       | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0167496  |
-| ILP_MTX              | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0197985  |
-| PSEUDO_B             | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.00047041 |
-| PSEUDO_L             | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00083811 |
-| BIFPTAS_L            | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00082326 |
-| BASELINE_NO_PART     | [[1], [2], [3], [4], [5], [6], [7], [8], [9], [10]] |   1090 |       472 | 9.38e-05   |
-| BASELINE_SINGLE      | [[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]]                   |    822 |       686 | 6.718e-05  |
+| Algorithm          | Partitioning                                        |   Cost | Latency                            |   Time (s) |
+|--------------------|-----------------------------------------------------|--------|------------------------------------|------------|
+| GREEDY_0           | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 | 443                                | 0.0235749  |
+| GREEDY_1           | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 | 474                                | 0.0235749  |
+| GREEDY_2           | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 | 471                                | 0.0235749  |
+| ILP_CFG_HYBRID     | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 | 474                                | 0.0167496  |
+| ILP_MTX            | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 | 474                                | 0.0197985  |
+| PSEUDO_B           | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 | 443                                | 0.00047041 |
+| PSEUDO_L           | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 | 471                                | 0.00083811 |
+| BIFPTAS_L          | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 | 471                                | 0.00082326 |
+| _BASELINE_NO_PART_ | [[1], [2], [3], [4], [5], [6], [7], [8], [9], [10]] |   1090 | 472                                | 9.38e-05   |
+| _BASELINE_SINGLE_  | [[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]]                   |    822 | <span style="color:red">686</span> | 6.718e-05  |
 
 ## Development and contribution
 
 If you would like to contribute, add a feature, or just play with the implementations, the development
 environment can be set up with the following commands.
 
 ```bash
 git clone https://github.com/hsnlab/SLAMBUC.git
 python3.11 -m pip install -U -r SLAMBUC/requirements.txt
-python3.11 -m pip install --ignore-requires-python --no-deps -e SLAMBUC/
+python3.11 -m pip install --no-deps -e SLAMBUC/
 # OR
 cd SLAMBUC && make install-req && make dev-install
 
 ## Remove editing-mode package outside of repo root
 python3.11 -m pip uninstall slambuc
 # OR
 make uninstall
```

### Comparing `SLAMBUC-0.2.0/README.md` & `SLAMBUC-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Serverless Layout Adaptation with Memory-Bounds and User Constraints (SLAMBUC)
 
-![PyPI](https://img.shields.io/pypi/v/SLAMBUC)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/SLAMBUC)
-![PyPI - License](https://img.shields.io/pypi/l/SLAMBUC)
-![Algorithm tests](https://github.com/hsnlab/SLAMBUC/actions/workflows/python-alg-tests.yml/badge.svg?branch=main)
-
+[![PyPI](https://img.shields.io/pypi/v/SLAMBUC)](https://pypi.org/project/SLAMBUC/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/SLAMBUC)](https://pypi.org/project/SLAMBUC/#history)
+[![Downloads](https://static.pepy.tech/badge/slambuc)](https://pepy.tech/project/slambuc)
+[![PyPI - License](https://img.shields.io/pypi/l/SLAMBUC)](LICENSE)
+[![pytest](https://github.com/hsnlab/SLAMBUC/actions/workflows/python-alg-tests.yml/badge.svg?branch=main)](https://github.com/hsnlab/SLAMBUC/actions/workflows/python-alg-tests.yml)
+[![Algorithm validations](https://github.com/hsnlab/SLAMBUC/actions/workflows/python-alg-validation.yml/badge.svg?branch=main)](https://github.com/hsnlab/SLAMBUC/actions/workflows/python-alg-validation.yml)
 
 Collection of graph partitioning algorithms implemented in Python for composing cloud-native
 applications from standalone serverless functions in a cost-efficient and latency-constrained manner.
 
 ## Overview
 
 In the context of serverless computing, function fusion is a novel, high-level approach to improve
@@ -102,86 +103,83 @@
 To install additional dependencies, run the following commands.
 
 ```bash
 python3.11 -m pip install slambuc[tests]      # For executing tests
 python3.11 -m pip install slambuc[validation] # For using our test harness framework
 ```
 
-## Package structure
-
-* [slambuc](slambuc) - [Main package]
-    * [alg](slambuc/alg) - [algorithms]
-        * [chain](slambuc/alg/chain) - [Single Chain Partitioning]
-            * [dp](slambuc/alg/chain/dp) - [dynamic programming]
-            * [ser](slambuc/alg/chain/ser) - [linear programming]
-        * [ext](slambuc/alg/ext) - [External algorithms and Baselines]
-        * [service](slambuc/alg/service) - [Service Properties]
-        * [tree](slambuc/alg/tree) - [Tree Partitioning]
-            * [dp](slambuc/alg/tree/dp) - [chain-based algorithms]
-            * [layout](slambuc/alg/tree/layout) - [general partitioning]
-            * [par](slambuc/alg/tree/par) - [parallel executions models]
-            * [ser](slambuc/alg/tree/ser) - [serialized execution models]
-    * [gen](slambuc/gen) - [Input Generators]
-        * [cluster](slambuc/gen/cluster) - [data-parallel job trees]
-        * [microservice](slambuc/gen/microservice) - [serverless trees]
-        * [random](slambuc/gen/random) - [random trees]
-    * [misc](slambuc/misc) - [Miscellaneous utility codes]
-* [tests](tests) - [tests]
-* [validation](validation) - [Validation Framework]
-    * [data](validation/data) - [generated test data]
-    * [results](validation/results) - [measured result files]
-
 ## Usage
 
-Refer to the wiki for [formats, execution parameters, and examples](https://github.com/hsnlab/SLAMBUC/wiki).
+Refer to the wiki for [formats, execution parameters, examples, and API documentation](https://github.com/hsnlab/SLAMBUC/wiki).
 
 ## Example
 
+```python
+from slambuc.alg.tree.ser.pseudo import pseudo_ltree_partitioning
+from slambuc.misc.generator import get_random_tree
+
+# Get input parameters
+tree = get_random_tree(nodes=10)
+params = dict(tree=tree,
+              root=1,
+              M=6,
+              L=450,
+              cp_end=10,
+              delay=10)
+
+# Partitioning
+res = pseudo_ltree_partitioning(**params)
+print(f"Part: {res[0]}, opt. cost: {res[1]}, latency: {res[2]}")
+"Part: [[1, 2], [3, 4], [5, 6, 7, 8], [9], [10]], opt. cost: 1252, latency: 449"
+```
+
+## Algorithms
+
 Validation results of a subset of our algorithms with a fully-serialized block execution model,
 which are executed with our [validation script](tests/validate_algs.py) using different configurations 
 and a [random-generated input call graph](tests/data/graph_test_tree_ser.gml) of size 10.
 
 Used algorithmic parameters (if applicable):
   * Root node ID (root): 1
   * Memory limit (M): 6
   * Available vCPU count (N): 1
   * Critical path's end node ID (cp_end): 10 
-  * Latency limit: (L): inf
+  * Latency limit: (L): **500**
   * Platform delay: (delay): 10
   * Bidirectional elimination (bidirectional): True
   * Cost approximation ratio (Epsilon): 0.0
   * Latency violation ratio (Lambda): 0.0
 
 Exact algorithms are configured to yield all optimal solutions (if exists) with the numerating 
 format `{alg}_{num}`.
 
 Execution results:
 
-| Algorithm            | Partitioning                                        |   Cost |   Latency |   Time (s) |
-|----------------------|-----------------------------------------------------|--------|-----------|------------|
-| GREEDY_0             | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.0235749  |
-| GREEDY_1             | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0235749  |
-| GREEDY_2             | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.0235749  |
-| ILP_CFG_HYBRID       | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0167496  |
-| ILP_MTX              | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0197985  |
-| PSEUDO_B             | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.00047041 |
-| PSEUDO_L             | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00083811 |
-| BIFPTAS_L            | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00082326 |
-| BASELINE_NO_PART     | [[1], [2], [3], [4], [5], [6], [7], [8], [9], [10]] |   1090 |       472 | 9.38e-05   |
-| BASELINE_SINGLE      | [[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]]                   |    822 |       686 | 6.718e-05  |
+| Algorithm          | Partitioning                                        |   Cost | Latency                            |   Time (s) |
+|--------------------|-----------------------------------------------------|--------|------------------------------------|------------|
+| GREEDY_0           | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 | 443                                | 0.0235749  |
+| GREEDY_1           | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 | 474                                | 0.0235749  |
+| GREEDY_2           | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 | 471                                | 0.0235749  |
+| ILP_CFG_HYBRID     | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 | 474                                | 0.0167496  |
+| ILP_MTX            | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 | 474                                | 0.0197985  |
+| PSEUDO_B           | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 | 443                                | 0.00047041 |
+| PSEUDO_L           | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 | 471                                | 0.00083811 |
+| BIFPTAS_L          | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 | 471                                | 0.00082326 |
+| _BASELINE_NO_PART_ | [[1], [2], [3], [4], [5], [6], [7], [8], [9], [10]] |   1090 | 472                                | 9.38e-05   |
+| _BASELINE_SINGLE_  | [[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]]                   |    822 | <span style="color:red">686</span> | 6.718e-05  |
 
 ## Development and contribution
 
 If you would like to contribute, add a feature, or just play with the implementations, the development
 environment can be set up with the following commands.
 
 ```bash
 git clone https://github.com/hsnlab/SLAMBUC.git
 python3.11 -m pip install -U -r SLAMBUC/requirements.txt
-python3.11 -m pip install --ignore-requires-python --no-deps -e SLAMBUC/
+python3.11 -m pip install --no-deps -e SLAMBUC/
 # OR
 cd SLAMBUC && make install-req && make dev-install
 
 ## Remove editing-mode package outside of repo root
 python3.11 -m pip uninstall slambuc
 # OR
 make uninstall
```

### Comparing `SLAMBUC-0.2.0/SLAMBUC.egg-info/PKG-INFO` & `SLAMBUC-0.2.1/SLAMBUC.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SLAMBUC
-Version: 0.2.0
+Version: 0.2.1
 Summary: Serverless Layout Adaptation with Memory-Bounds and User Constraints
 Author: Janos Czentye
 Author-email: Janos Czentye <czentye@tmit.bme.hu>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/hsnlab/SLAMBUC
 Project-URL: Homepage, https://github.com/hsnlab/SLAMBUC/wiki
 Project-URL: Issue Tracker, https://github.com/hsnlab/SLAMBUC/issues
@@ -21,19 +21,20 @@
 Provides-Extra: tests
 Provides-Extra: validation
 Provides-Extra: doc
 License-File: LICENSE
 
 # Serverless Layout Adaptation with Memory-Bounds and User Constraints (SLAMBUC)
 
-![PyPI](https://img.shields.io/pypi/v/SLAMBUC)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/SLAMBUC)
-![PyPI - License](https://img.shields.io/pypi/l/SLAMBUC)
-![Algorithm tests](https://github.com/hsnlab/SLAMBUC/actions/workflows/python-alg-tests.yml/badge.svg?branch=main)
-
+[![PyPI](https://img.shields.io/pypi/v/SLAMBUC)](https://pypi.org/project/SLAMBUC/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/SLAMBUC)](https://pypi.org/project/SLAMBUC/#history)
+[![Downloads](https://static.pepy.tech/badge/slambuc)](https://pepy.tech/project/slambuc)
+[![PyPI - License](https://img.shields.io/pypi/l/SLAMBUC)](LICENSE)
+[![pytest](https://github.com/hsnlab/SLAMBUC/actions/workflows/python-alg-tests.yml/badge.svg?branch=main)](https://github.com/hsnlab/SLAMBUC/actions/workflows/python-alg-tests.yml)
+[![Algorithm validations](https://github.com/hsnlab/SLAMBUC/actions/workflows/python-alg-validation.yml/badge.svg?branch=main)](https://github.com/hsnlab/SLAMBUC/actions/workflows/python-alg-validation.yml)
 
 Collection of graph partitioning algorithms implemented in Python for composing cloud-native
 applications from standalone serverless functions in a cost-efficient and latency-constrained manner.
 
 ## Overview
 
 In the context of serverless computing, function fusion is a novel, high-level approach to improve
@@ -127,86 +128,83 @@
 To install additional dependencies, run the following commands.
 
 ```bash
 python3.11 -m pip install slambuc[tests]      # For executing tests
 python3.11 -m pip install slambuc[validation] # For using our test harness framework
 ```
 
-## Package structure
-
-* [slambuc](slambuc) - [Main package]
-    * [alg](slambuc/alg) - [algorithms]
-        * [chain](slambuc/alg/chain) - [Single Chain Partitioning]
-            * [dp](slambuc/alg/chain/dp) - [dynamic programming]
-            * [ser](slambuc/alg/chain/ser) - [linear programming]
-        * [ext](slambuc/alg/ext) - [External algorithms and Baselines]
-        * [service](slambuc/alg/service) - [Service Properties]
-        * [tree](slambuc/alg/tree) - [Tree Partitioning]
-            * [dp](slambuc/alg/tree/dp) - [chain-based algorithms]
-            * [layout](slambuc/alg/tree/layout) - [general partitioning]
-            * [par](slambuc/alg/tree/par) - [parallel executions models]
-            * [ser](slambuc/alg/tree/ser) - [serialized execution models]
-    * [gen](slambuc/gen) - [Input Generators]
-        * [cluster](slambuc/gen/cluster) - [data-parallel job trees]
-        * [microservice](slambuc/gen/microservice) - [serverless trees]
-        * [random](slambuc/gen/random) - [random trees]
-    * [misc](slambuc/misc) - [Miscellaneous utility codes]
-* [tests](tests) - [tests]
-* [validation](validation) - [Validation Framework]
-    * [data](validation/data) - [generated test data]
-    * [results](validation/results) - [measured result files]
-
 ## Usage
 
-Refer to the wiki for [formats, execution parameters, and examples](https://github.com/hsnlab/SLAMBUC/wiki).
+Refer to the wiki for [formats, execution parameters, examples, and API documentation](https://github.com/hsnlab/SLAMBUC/wiki).
 
 ## Example
 
+```python
+from slambuc.alg.tree.ser.pseudo import pseudo_ltree_partitioning
+from slambuc.misc.generator import get_random_tree
+
+# Get input parameters
+tree = get_random_tree(nodes=10)
+params = dict(tree=tree,
+              root=1,
+              M=6,
+              L=450,
+              cp_end=10,
+              delay=10)
+
+# Partitioning
+res = pseudo_ltree_partitioning(**params)
+print(f"Part: {res[0]}, opt. cost: {res[1]}, latency: {res[2]}")
+"Part: [[1, 2], [3, 4], [5, 6, 7, 8], [9], [10]], opt. cost: 1252, latency: 449"
+```
+
+## Algorithms
+
 Validation results of a subset of our algorithms with a fully-serialized block execution model,
 which are executed with our [validation script](tests/validate_algs.py) using different configurations 
 and a [random-generated input call graph](tests/data/graph_test_tree_ser.gml) of size 10.
 
 Used algorithmic parameters (if applicable):
   * Root node ID (root): 1
   * Memory limit (M): 6
   * Available vCPU count (N): 1
   * Critical path's end node ID (cp_end): 10 
-  * Latency limit: (L): inf
+  * Latency limit: (L): **500**
   * Platform delay: (delay): 10
   * Bidirectional elimination (bidirectional): True
   * Cost approximation ratio (Epsilon): 0.0
   * Latency violation ratio (Lambda): 0.0
 
 Exact algorithms are configured to yield all optimal solutions (if exists) with the numerating 
 format `{alg}_{num}`.
 
 Execution results:
 
-| Algorithm            | Partitioning                                        |   Cost |   Latency |   Time (s) |
-|----------------------|-----------------------------------------------------|--------|-----------|------------|
-| GREEDY_0             | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.0235749  |
-| GREEDY_1             | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0235749  |
-| GREEDY_2             | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.0235749  |
-| ILP_CFG_HYBRID       | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0167496  |
-| ILP_MTX              | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0197985  |
-| PSEUDO_B             | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.00047041 |
-| PSEUDO_L             | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00083811 |
-| BIFPTAS_L            | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00082326 |
-| BASELINE_NO_PART     | [[1], [2], [3], [4], [5], [6], [7], [8], [9], [10]] |   1090 |       472 | 9.38e-05   |
-| BASELINE_SINGLE      | [[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]]                   |    822 |       686 | 6.718e-05  |
+| Algorithm          | Partitioning                                        |   Cost | Latency                            |   Time (s) |
+|--------------------|-----------------------------------------------------|--------|------------------------------------|------------|
+| GREEDY_0           | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 | 443                                | 0.0235749  |
+| GREEDY_1           | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 | 474                                | 0.0235749  |
+| GREEDY_2           | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 | 471                                | 0.0235749  |
+| ILP_CFG_HYBRID     | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 | 474                                | 0.0167496  |
+| ILP_MTX            | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 | 474                                | 0.0197985  |
+| PSEUDO_B           | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 | 443                                | 0.00047041 |
+| PSEUDO_L           | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 | 471                                | 0.00083811 |
+| BIFPTAS_L          | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 | 471                                | 0.00082326 |
+| _BASELINE_NO_PART_ | [[1], [2], [3], [4], [5], [6], [7], [8], [9], [10]] |   1090 | 472                                | 9.38e-05   |
+| _BASELINE_SINGLE_  | [[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]]                   |    822 | <span style="color:red">686</span> | 6.718e-05  |
 
 ## Development and contribution
 
 If you would like to contribute, add a feature, or just play with the implementations, the development
 environment can be set up with the following commands.
 
 ```bash
 git clone https://github.com/hsnlab/SLAMBUC.git
 python3.11 -m pip install -U -r SLAMBUC/requirements.txt
-python3.11 -m pip install --ignore-requires-python --no-deps -e SLAMBUC/
+python3.11 -m pip install --no-deps -e SLAMBUC/
 # OR
 cd SLAMBUC && make install-req && make dev-install
 
 ## Remove editing-mode package outside of repo root
 python3.11 -m pip uninstall slambuc
 # OR
 make uninstall
```

### Comparing `SLAMBUC-0.2.0/SLAMBUC.egg-info/SOURCES.txt` & `SLAMBUC-0.2.1/SLAMBUC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/pyproject.toml` & `SLAMBUC-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -30,32 +30,33 @@
 ]
 
 [project.urls]
 "Repository" = "https://github.com/hsnlab/SLAMBUC"
 "Homepage" = "https://github.com/hsnlab/SLAMBUC/wiki"
 "Issue Tracker" = "https://github.com/hsnlab/SLAMBUC/issues"
 
-[tool.setuptools.dynamic]
-version = { attr = "slambuc.__version__" }
-readme = { file = ["README.md"], content-type = 'text/markdown' }
-
 [project.optional-dependencies]
 tests = [
     'pygraphviz~=1.10',
+    'pytest~=7.4.0',
     'tabulate~=0.9.0'
 ]
 validation = [
     'tabulate~=0.9.0',
     'Click~=8.1.3',
     'psutil~=5.9.4'
 ]
 doc = [
     'pydoc-markdown~=4.8.2'
 ]
 
+[tool.setuptools.dynamic]
+version = { attr = "slambuc.__version__" }
+readme = { file = ["README.md"], content-type = 'text/markdown' }
+
 [tool.setuptools.packages.find]
 exclude = [
     "tests",
     "tests.*",
     "validation",
     "validation.*"
 ]
@@ -65,18 +66,27 @@
 
 [tool.setuptools.package-data]
 "*" = [
     '*.pkl',
     '*.csv'
 ]
 
+## Documentation
+
 [[tool.pydoc-markdown.loaders]]
 type = "python"
-search_path = [ "slambuc" ]
+search_path = ["slambuc"]
+
+[[tool.pydoc-markdown.processors]]
+type = ["filter", "smart", "crossref"]
 
 [tool.pydoc-markdown.renderer]
 type = "mkdocs"
 
 [[tool.pydoc-markdown.renderer.pages]]
 title = "SLAMBUC API Documentation"
 name = "index"
-contents = [ "slambuc.*" ]
+contents = ["slambuc", "slambuc.*"]
+
+[[tool.pydoc-markdown.renderer.mkdocs_config]]
+site_name = "SLAMBUC"
+repo_url = "https://github.com/hsnlab/SLAMBUC"
```

### Comparing `SLAMBUC-0.2.0/setup.py` & `SLAMBUC-0.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,24 +37,26 @@
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules"
     ],
     python_requires='>=3.10',
     license="Apache 2.0",
     keywords="cloud serverless ilp dp tree",
     install_requires=[
-        'cspy~=1.0.3',
-        'matplotlib~=3.7.1',
         'networkx~=3.1',
         'numpy~=1.25.0',
-        'pandas~=2.0.3',
         'PuLP~=2.7.0',
-        'scipy~=1.11.1'
+        'matplotlib~=3.7.1',
+        'pandas~=2.0.3',
+        'scipy~=1.11.1',
+        'cspy~=1.0.3',
     ],
-    extras_require={'tests': ['pygraphviz~=1.10',
-                              'tabulate~=0.9.0'],
+    extras_require={'tests': ['pytest~=7.4.0',
+                              'pygraphviz~=1.10',
+                              'tabulate~=0.9.0',
+                              'docplex~=2.25.236'],
                     'validation': ['tabulate~=0.9.0',
                                    'Click~=8.1.3',
                                    'psutil~=5.9.4']},
     package_data={'*': ['*.pkl',
                         '*.csv']},
     include_package_data=True,
     zip_safe=False
```

### Comparing `SLAMBUC-0.2.0/slambuc/__init__.py` & `SLAMBUC-0.2.1/slambuc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.2.0"
+__version__ = "0.2.1"
```

### Comparing `SLAMBUC-0.2.0/slambuc/alg/__init__.py` & `SLAMBUC-0.2.1/slambuc/alg/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/chain/__init__.py` & `SLAMBUC-0.2.1/slambuc/alg/chain/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/chain/dp/__init__.py` & `SLAMBUC-0.2.1/slambuc/alg/chain/dp/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/chain/dp/greedy.py` & `SLAMBUC-0.2.1/slambuc/alg/chain/dp/greedy.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/chain/dp/min.py` & `SLAMBUC-0.2.1/slambuc/alg/chain/dp/min.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/chain/dp/mtx.py` & `SLAMBUC-0.2.1/slambuc/alg/chain/dp/mtx.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/chain/ser/__init__.py` & `SLAMBUC-0.2.1/slambuc/alg/chain/ser/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/chain/ser/greedy.py` & `SLAMBUC-0.2.1/slambuc/alg/chain/ser/greedy.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/chain/ser/ilp.py` & `SLAMBUC-0.2.1/slambuc/alg/chain/ser/ilp.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/ext/__init__.py` & `SLAMBUC-0.2.1/slambuc/alg/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/ext/baseline.py` & `SLAMBUC-0.2.1/slambuc/alg/ext/baseline.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/ext/csp.py` & `SLAMBUC-0.2.1/slambuc/alg/ext/csp.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/ext/greedy.py` & `SLAMBUC-0.2.1/slambuc/alg/ext/greedy.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/ext/min_cut.py` & `SLAMBUC-0.2.1/slambuc/alg/ext/min_cut.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/service/__init__.py` & `SLAMBUC-0.2.1/slambuc/alg/service/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/service/common.py` & `SLAMBUC-0.2.1/slambuc/alg/service/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,20 +35,20 @@
 
 # Separator character for state names, separating nodes in the group (VSEP) and group from assigned flavor (FSEP)
 SEP = '|'
 ASSIGN = '@'
 
 
 class Flavor(typing.NamedTuple):
-    """Store subtree partitioning attributes for a given subcase"""
+    """Store subtree partitioning attributes for a given subcase."""
     mem: int = math.inf  # Available memory
     ncore: int = 1  # Available relative vCPU cores
     cfactor: float = 1.0  # Relative cost factor
 
     def __repr__(self):
         # return repr(tuple(self))
         return self.name
 
     @property
     def name(self) -> str:
-        """String representation of the given flavor"""
+        """String representation of the given flavor."""
         return f"F[{self.mem},{self.ncore},{self.cfactor}]"
```

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/__init__.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/dp/__init__.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/dp/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/dp/greedy.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/dp/greedy.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/dp/meta.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/dp/meta.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/dp/min.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/dp/min.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/dp/seq.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/dp/seq.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/dp/seq_state.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/dp/seq_state.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/layout/__init__.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/layout/ilp.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/layout/ilp.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/par/__init__.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/par/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/par/greedy.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/par/greedy.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/par/ilp.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/par/ilp.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/par/pseudo.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/par/pseudo.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/par/pseudo_mp.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/par/pseudo_mp.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/ser/__init__.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/ser/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/ser/bicriteria.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/ser/bicriteria.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/ser/greedy.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/ser/greedy.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/ser/ilp.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/ser/ilp.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/ser/ilp_cplex.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/ser/ilp_cplex.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/ser/pseudo.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/ser/pseudo.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/alg/tree/ser/pseudo_mp.py` & `SLAMBUC-0.2.1/slambuc/alg/tree/ser/pseudo_mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,16 @@
     :param root:    root node of the graph
     :param workers: workers count
     :return:        cut edges
     """
     ub = math.sqrt(len(tree) - 1)
     lb = ub if not workers else 1
     n = workers if workers else ub
-    return [e for e, _ in heapq.nlargest(n, list(isubtree_cutoffs(tree, root, lb, ub)), key=operator.itemgetter(1))]
+    return [e for e, _ in heapq.nlargest(round(n),
+                                         list(isubtree_cutoffs(tree, root, lb, ub)), key=operator.itemgetter(1))]
 
 
 def isubtree_sync_cutoffs(tree: nx.DiGraph, root: int = 1,
                           size: int = math.inf) -> Generator[tuple[tuple[int], int, set[int]]]:
     """
     Recursively return edges that cut off non-trivial subtrees from *tree* with given *size*.
```

### Comparing `SLAMBUC-0.2.0/slambuc/alg/util.py` & `SLAMBUC-0.2.1/slambuc/alg/util.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/gen/__init__.py` & `SLAMBUC-0.2.1/slambuc/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/gen/cluster/__init__.py` & `SLAMBUC-0.2.1/slambuc/gen/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/gen/cluster/hist/cpl_hist.pkl` & `SLAMBUC-0.2.1/slambuc/gen/cluster/hist/cpl_hist.pkl`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/gen/cluster/hist/instance_num_hist.pkl` & `SLAMBUC-0.2.1/slambuc/gen/cluster/hist/instance_num_hist.pkl`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/gen/cluster/hist/level_hist.pkl` & `SLAMBUC-0.2.1/slambuc/gen/cluster/hist/level_hist.pkl`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/gen/cluster/hist/task_duration_hist.pkl` & `SLAMBUC-0.2.1/slambuc/gen/cluster/hist/task_duration_hist.pkl`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/gen/cluster/hist/task_mem_hist.pkl` & `SLAMBUC-0.2.1/slambuc/gen/cluster/hist/task_mem_hist.pkl`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/gen/cluster/hist/task_num_hist.pkl` & `SLAMBUC-0.2.1/slambuc/gen/cluster/hist/task_num_hist.pkl`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/gen/cluster/job_tree.py` & `SLAMBUC-0.2.1/slambuc/gen/cluster/job_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import importlib.resources
 import itertools
 import pathlib
 import random
 from collections.abc import Generator
 
 import networkx as nx
 import numpy as np
@@ -23,16 +24,17 @@
 
 from slambuc.alg.service.common import *
 from slambuc.gen.cluster.syn_job import random_job
 from slambuc.gen.io import save_trees_to_file
 from slambuc.gen.transform import faasify_dag_by_duplication
 
 # Default sample job/task file of the installed spar package
-DEF_TASK_CSV = pathlib.Path(pathlib.Path(__file__).parent / "samples/sample_tasks.csv")
-DEF_BATCH_CSV = pathlib.Path(pathlib.Path(__file__).parent / "samples/batch_task.csv")
+SAMPLES_DIR = importlib.resources.files("slambuc.gen.cluster").joinpath("samples")
+DEF_TASK_CSV = SAMPLES_DIR / "sample_tasks.csv"
+DEF_BATCH_CSV = SAMPLES_DIR / "batch_task.csv"
 DEF_TASK_CSV_HEADER = ('job', 'task', 'duration', 'cpu', 'mem', 'num')
 DEF_TASK_CSV_COLS = (1, 2, 3, 4, 5, 6)
 # Default attributes for the front-end dispatcher function
 DISP_NODE = 0
 DISP_RUNTIME = 1
 DISP_MEM = 0.1
 # Default attributes of tree nodes
```

### Comparing `SLAMBUC-0.2.0/slambuc/gen/cluster/samples/batch_task.csv` & `SLAMBUC-0.2.1/slambuc/gen/cluster/samples/batch_task.csv`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/gen/cluster/samples/sample_tasks.csv` & `SLAMBUC-0.2.1/slambuc/gen/cluster/samples/sample_tasks.csv`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/gen/cluster/syn_job.py` & `SLAMBUC-0.2.1/slambuc/gen/cluster/syn_job.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import collections
+import importlib.resources
 import itertools
 import math
-import pathlib
 import pickle
 import random
 
 import pandas as pd
 import scipy
 
 # Random job generation source code is moved from package *spar* with adaptations to newer versions of Python3.11
 # and Scipy 1.10.  See also: https://github.com/All-less/trace-generator/blob/master/spar/generate.py
 
-HIST_DATA_DIR = pathlib.Path(__file__).parent / "hist"
+HIST_DATA_DIR = importlib.resources.files("slambuc.gen.cluster").joinpath("hist")
 DIST_CACHE = {}
 
 
 def draw(hist_name: str, num: int = 1, path: list = tuple(), ndigits: int = 2, positive: bool = True,
          output_integer: bool = False, seed: int = None) -> list[int | float]:
     """
     Draw random samples from a given distribution.
```

### Comparing `SLAMBUC-0.2.0/slambuc/gen/io.py` & `SLAMBUC-0.2.1/slambuc/gen/io.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/gen/microservice/__init__.py` & `SLAMBUC-0.2.1/slambuc/gen/microservice/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/gen/microservice/faas_tree.py` & `SLAMBUC-0.2.1/slambuc/gen/microservice/faas_tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import importlib.resources
 import itertools
 import pathlib
 import random
 from collections.abc import Generator
 
 import networkx as nx
 import numpy as np
@@ -37,15 +38,15 @@
 MEM_C = 11.652
 MEM_K = 0.221
 MEM_LAMBDA = 107.083
 MEM_DIST = scipy.stats.burr12(c=MEM_C, d=MEM_K, loc=0.0, scale=MEM_LAMBDA)
 
 # Empirical distribution parameters of function calls extracted from Alibaba traces
 # See also: https://github.com/alibaba/clusterdata/tree/master/cluster-trace-microservices-v2021
-HIST_DIR = pathlib.Path(__file__).parent / 'hist'
+HIST_DIR = importlib.resources.files("slambuc.gen.microservice").joinpath("hist")
 # Invocation rate per services
 RATE_HIST_NAME = "func_inv_rate_hist"
 RATE_DIST = scipy.stats.rv_histogram(load_hist_params(HIST_DIR, RATE_HIST_NAME), density=True)
 
 # Data R/W overhead
 DATA_HIST_NAME = "rw_overhead_hist"
 DATA_DIST = scipy.stats.rv_histogram(load_hist_params(HIST_DIR, DATA_HIST_NAME), density=True)
@@ -65,15 +66,15 @@
     :param dist:        build distribution object
     :param transform:   transform function applied on every attribute value
     :return:            generator of attributes
     """
     yield from transform(dist.rvs(size=n)).astype(int)
 
 
-def get_faas_tree(n: int, Alpha: float, a: float) -> nx.DiGraph:
+def get_faas_tree(n: int, Alpha: float = 1.0, a: float = 0.0) -> nx.DiGraph:
     """
     Generate service tree with attributes drawn from the predefined distributions.
 
     :param n:       number of nodes
     :param Alpha:   power of preferential attachment (default: 1.0)
     :param a:       attractiveness of vertices with no edges (default: 0.0)
     :return:        generated tree
@@ -121,9 +122,9 @@
                  for _ in range(iteration)]
         file_name = pathlib.Path(data_dir, f"{tree_name}_n{min_size}-{max_size}.npy").resolve()
         print(f"Saving trees into {file_name}...")
         save_trees_to_file(trees, file_name, padding=max_size)
 
 
 if __name__ == '__main__':
-    # verify_faas_tree(n=20)
-    generate_all_faas_trees("../../../validation/data")
+    verify_faas_tree(n=20)
+    # generate_all_faas_trees("../../../validation/data")
```

### Comparing `SLAMBUC-0.2.0/slambuc/gen/microservice/hist/func_inv_rate_hist.pkl` & `SLAMBUC-0.2.1/slambuc/gen/microservice/hist/func_inv_rate_hist.pkl`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/gen/microservice/hist/rw_overhead_hist.pkl` & `SLAMBUC-0.2.1/slambuc/gen/microservice/hist/rw_overhead_hist.pkl`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/gen/microservice/power_ba_graph.py` & `SLAMBUC-0.2.1/slambuc/gen/microservice/power_ba_graph.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/gen/random/__init__.py` & `SLAMBUC-0.2.1/slambuc/gen/random/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/gen/random/random_tree.py` & `SLAMBUC-0.2.1/slambuc/gen/random/random_tree.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/gen/transform.py` & `SLAMBUC-0.2.1/slambuc/gen/transform.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/misc/__init__.py` & `SLAMBUC-0.2.1/slambuc/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/misc/generator.py` & `SLAMBUC-0.2.1/slambuc/misc/generator.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/misc/plot.py` & `SLAMBUC-0.2.1/slambuc/misc/plot.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.2.0/slambuc/misc/util.py` & `SLAMBUC-0.2.1/slambuc/misc/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,30 +31,44 @@
 
 def get_cplex_path() -> str:
     """
     Return local CPLEX path.
 
     :return: path
     """
-    if isinstance(cp := subprocess.run(['which', 'cplex']), str):
-        return cp
-    return str(pathlib.Path(os.environ.get('CPLEX_HOME', '~/Programs/ibm/ILOG/CPLEX_Studio2211/cplex'),
-                            'bin/x86-64_linux/cplex').expanduser())
+    if cplex_path := subprocess.run(['which', 'cplex'], stdout=subprocess.PIPE).stdout.decode().strip():
+        return cplex_path
+    cplex_path = pathlib.Path(os.environ.get('CPLEX_HOME', '~/Programs/ibm/ILOG/CPLEX_Studio2211/cplex'),
+                              'bin/x86-64_linux/cplex').expanduser()
+    return str(cplex_path) if cplex_path.exists() else None
 
 
 def get_cpo_path() -> str:
     """
     Return local CPO path.
 
     :return: path
     """
-    if isinstance(cp := subprocess.run(['which', 'cpoptimizer']), str):
-        return cp
-    return str(pathlib.Path(os.environ.get('CPO_HOME', '~/Programs/ibm/ILOG/CPLEX_Studio2211/cpoptimizer'),
-                            'bin/x86-64_linux/cpoptimizer').expanduser())
+    if cpo_path := subprocess.run(['which', 'cpoptimizer'], stdout=subprocess.PIPE).stdout.decode().strip():
+        return cpo_path
+    cpo_path = pathlib.Path(os.environ.get('CPO_HOME', '~/Programs/ibm/ILOG/CPLEX_Studio2211/cpoptimizer'),
+                            'bin/x86-64_linux/cpoptimizer').expanduser()
+    return str(cpo_path) if cpo_path.exists() else None
+
+
+def get_glpk_path() -> str:
+    """
+    Return local GLPK path.
+
+    :return: path
+    """
+    if glpk_path := subprocess.run(['which', 'glpsol'], stdout=subprocess.PIPE).stdout.decode().strip():
+        return glpk_path
+    else:
+        return None
 
 
 def is_compatible(tree1: nx.DiGraph, tree2: nx.DiGraph) -> bool:
     """
     Return true if given second *tree2* has the same structure and edge/node attributes as the first *tree1*.
 
     :param tree1:   first tree
```

