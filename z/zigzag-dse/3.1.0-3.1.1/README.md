# Comparing `tmp/zigzag_dse-3.1.0.tar.gz` & `tmp/zigzag_dse-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigzag_dse-3.1.0.tar", last modified: Mon Apr 15 09:56:04 2024, max compression
+gzip compressed data, was "zigzag_dse-3.1.1.tar", last modified: Fri May 17 09:36:18 2024, max compression
```

## Comparing `zigzag_dse-3.1.0.tar` & `zigzag_dse-3.1.1.tar`

### file list

```diff
@@ -1,322 +1,167 @@
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.806481 zigzag_dse-3.1.0/
--rw-r--r--   0 asymons  (27005) micas     (3600)     1074 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/LICENSE
--rw-r--r--   0 asymons  (27005) micas     (3600)       88 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/MANIFEST.in
--rw-r--r--   0 asymons  (27005) micas     (3600)    10722 2024-04-15 09:56:04.803480 zigzag_dse-3.1.0/PKG-INFO
--rw-r--r--   0 asymons  (27005) micas     (3600)     8519 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/README.md
--rw-r--r--   0 asymons  (27005) micas     (3600)     1601 2024-04-15 09:51:10.000000 zigzag_dse-3.1.0/pyproject.toml
--rw-r--r--   0 asymons  (27005) micas     (3600)       38 2024-04-15 09:56:04.806481 zigzag_dse-3.1.0/setup.cfg
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.046449 zigzag_dse-3.1.0/tests/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.051449 zigzag_dse-3.1.0/tests/main/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.104452 zigzag_dse-3.1.0/tests/main/test_imc/
--rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/tests/main/test_imc/__init__.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1572 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/tests/main/test_imc/test_aimc.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1545 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/tests/main/test_imc/test_dimc.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.117452 zigzag_dse-3.1.0/tests/main/test_origin/
--rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_origin/__init__.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1253 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_origin/test_ascend_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1261 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_origin/test_edge_tpu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1266 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_origin/test_meta_prototype_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1262 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_origin/test_tesla_npu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1250 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_origin/test_tpu_like.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.131452 zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/
--rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/__init__.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2044 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/test_ascend_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2690 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/test_edge_tpu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2118 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/test_meta_prototype_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2087 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/test_tesla_npu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2378 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/test_tpu_like.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.143453 zigzag_dse-3.1.0/tests/main/test_without_unused_memory/
--rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_without_unused_memory/__init__.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1284 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_without_unused_memory/test_ascend_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1303 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_without_unused_memory/test_edge_tpu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1315 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_without_unused_memory/test_meta_prototype_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1309 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_without_unused_memory/test_tesla_npu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1294 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_without_unused_memory/test_tpu_like.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.151453 zigzag_dse-3.1.0/zigzag/
--rw-r--r--   0 asymons  (27005) micas     (3600)       22 2024-04-15 09:51:10.000000 zigzag_dse-3.1.0/zigzag/__init__.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2497 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/__main__.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    19803 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/api.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.152453 zigzag_dse-3.1.0/zigzag/classes/
--rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/__init__.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.156453 zigzag_dse-3.1.0/zigzag/classes/cacti/
--rw-r--r--   0 asymons  (27005) micas     (3600)      291 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/README.md
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.157454 zigzag_dse-3.1.0/zigzag/classes/cacti/__pycache__/
--rw-r--r--   0 asymons  (27005) micas     (3600)     3547 2024-02-27 13:47:53.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-39.pyc
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.316460 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/
--rw-r--r--   0 asymons  (27005) micas     (3600)     6576 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)     6555 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)     6920 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)     5324 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/README
--rw-r--r--   0 asymons  (27005) micas     (3600)     9282 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/TSV.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     3322 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/TSV.h
--rw-r--r--   0 asymons  (27005) micas     (3600)    41184 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/Ucache.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     3607 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/Ucache.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     5116 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/arbiter.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     2771 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/arbiter.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     2057 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/area.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     2416 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/area.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     8474 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/bank.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     2664 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/bank.h
--rw-r--r--   0 asymons  (27005) micas     (3600)    29279 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/basic_circuit.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     7364 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/basic_circuit.h
--rw-r--r--   0 asymons  (27005) micas     (3600)    11041 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cache.cfg_temp
--rw-r--r--   0 asymons  (27005) micas     (3600)    32713 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cache_old.cfg.out
--rwxr-xr-x   0 asymons  (27005) micas     (3600)  2421320 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti
--rw-r--r--   0 asymons  (27005) micas     (3600)      173 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti.i
--rw-r--r--   0 asymons  (27005) micas     (3600)     1334 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti.mk
--rw-r--r--   0 asymons  (27005) micas     (3600)    25297 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti_config_creator.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     5586 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti_interface.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)    27215 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti_interface.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     3747 2024-02-27 14:13:55.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti_top.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     7561 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/component.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     2837 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/component.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     9565 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/const.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     5001 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/contention.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)     7349 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/crossbar.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     3204 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/crossbar.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     9849 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/ddr3.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)    62337 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/decoder.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     7405 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/decoder.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     3712 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/dram.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)     9750 2024-03-19 15:11:36.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml
--rw-r--r--   0 asymons  (27005) micas     (3600)    17411 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/extio.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)      878 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/extio.h
--rw-r--r--   0 asymons  (27005) micas     (3600)    46185 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/extio_technology.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     9068 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/extio_technology.h
--rw-r--r--   0 asymons  (27005) micas     (3600)    23772 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/htree2.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     3595 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/htree2.h
--rw-r--r--   0 asymons  (27005) micas     (3600)   133713 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/io.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     2116 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/io.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     9850 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/lpddr.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)     7217 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/main.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)      407 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/makefile
--rw-r--r--   0 asymons  (27005) micas     (3600)    94813 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/mat.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     6122 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/mat.h
--rw-r--r--   0 asymons  (27005) micas     (3600)    16630 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/memcad.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)      553 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/memcad.h
--rw-r--r--   0 asymons  (27005) micas     (3600)    11483 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/memcad_parameters.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     4490 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/memcad_parameters.h
--rw-r--r--   0 asymons  (27005) micas     (3600)    29014 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/memorybus.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     5426 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/memorybus.h
--rw-r--r--   0 asymons  (27005) micas     (3600)    19629 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/nuca.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     3306 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/nuca.h
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.456466 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/
--rw-r--r--   0 asymons  (27005) micas     (3600)   134304 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   352744 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   157960 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   124352 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/area.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   156624 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   155192 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o
--rwxr-xr-x   0 asymons  (27005) micas     (3600)  2421320 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/cacti
--rw-r--r--   0 asymons  (27005) micas     (3600)   175768 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   159768 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/component.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   160680 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   207224 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   145592 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   180464 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   178384 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   411960 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/io.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   192248 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/main.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   270320 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   569648 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   280416 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   204480 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   256824 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   313848 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   124400 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   175432 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/router.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   128080 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   144976 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   228000 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   232752 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   111980 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/parameter.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)    20306 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/parameter.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     5286 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/powergating.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     3055 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/powergating.h
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     1886 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/regression.test
--rw-r--r--   0 asymons  (27005) micas     (3600)    10212 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/router.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     3721 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/router.h
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.468466 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/sample_config_files/
--rw-r--r--   0 asymons  (27005) micas     (3600)     8781 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)     8768 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)     8780 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)     8784 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.515468 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/
--rw-r--r--   0 asymons  (27005) micas     (3600)     9545 2024-03-19 15:11:38.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)      579 2024-03-19 15:11:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out
--rw-r--r--   0 asymons  (27005) micas     (3600)     9580 2024-04-15 09:35:55.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_-8238395692842152875.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)      578 2024-04-15 09:35:55.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_-8238395692842152875.cfg.out
--rw-r--r--   0 asymons  (27005) micas     (3600)     9580 2024-04-15 08:53:15.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_-8667919883845363313.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)      578 2024-04-15 08:53:15.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_-8667919883845363313.cfg.out
--rw-r--r--   0 asymons  (27005) micas     (3600)     9580 2024-04-15 09:35:38.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_2159937366902611545.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)      578 2024-04-15 09:35:38.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_2159937366902611545.cfg.out
--rw-r--r--   0 asymons  (27005) micas     (3600)     9580 2024-04-15 08:49:21.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_2582313971359678716.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)      578 2024-04-15 08:49:22.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_2582313971359678716.cfg.out
--rw-r--r--   0 asymons  (27005) micas     (3600)     9580 2024-04-15 08:40:34.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_3347886556911868882.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)      578 2024-04-15 08:40:35.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_3347886556911868882.cfg.out
--rw-r--r--   0 asymons  (27005) micas     (3600)     9580 2024-04-15 09:40:56.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_6701911052272027327.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)      578 2024-04-15 09:40:56.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_6701911052272027327.cfg.out
--rw-r--r--   0 asymons  (27005) micas     (3600)     9580 2024-04-15 08:36:19.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_748814760220054032.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)      578 2024-04-15 08:36:20.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_748814760220054032.cfg.out
--rw-r--r--   0 asymons  (27005) micas     (3600)     9578 2024-04-15 09:40:56.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_a.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)     3720 2024-04-15 09:40:56.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_a.cfg.out
--rw-r--r--   0 asymons  (27005) micas     (3600)     8332 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/subarray.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     2542 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/subarray.h
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.539469 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/
--rw-r--r--   0 asymons  (27005) micas     (3600)       25 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/16nm.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)    23666 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)     3842 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)     4575 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)     4759 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)     4755 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)    24571 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)     4758 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)    24570 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)     4742 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)    15087 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/technology.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)    41317 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/uca.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     4035 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/uca.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     2064 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/version_cacti.h
--rw-r--r--   0 asymons  (27005) micas     (3600)    29856 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/wire.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     4375 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/wire.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     7626 2024-02-27 13:47:51.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_parser.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.541469 zigzag_dse-3.1.0/zigzag/classes/cacti/self_gen/
--rw-r--r--   0 asymons  (27005) micas     (3600)     9549 2024-02-27 13:04:58.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/self_gen/cache.cfg
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.547470 zigzag_dse-3.1.0/zigzag/classes/cost_model/
--rw-r--r--   0 asymons  (27005) micas     (3600)    66253 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/cost_model/cost_model.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    20548 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/cost_model/cost_model_for_sram_imc.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.065450 zigzag_dse-3.1.0/zigzag/classes/hardware/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.583471 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/
--rw-r--r--   0 asymons  (27005) micas     (3600)    22537 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/AimcArray.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    40916 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/DimcArray.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2102 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/ImcArray.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1207 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/accelerator.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     9229 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/adder_hierarchy.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     6468 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/core.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      877 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/dimension.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    32673 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/get_cacti_cost.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    10610 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/imc_unit.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    11471 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/memory_hierarchy.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     3781 2024-02-21 09:50:55.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/memory_instance.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    12113 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/memory_level.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     3096 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/operational_array.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1742 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/operational_unit.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.068450 zigzag_dse-3.1.0/zigzag/classes/io/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.585471 zigzag_dse-3.1.0/zigzag/classes/io/accelerator/
--rw-r--r--   0 asymons  (27005) micas     (3600)     2799 2024-02-01 21:03:54.000000 zigzag_dse-3.1.0/zigzag/classes/io/accelerator/parser.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.604472 zigzag_dse-3.1.0/zigzag/classes/io/onnx/
--rw-r--r--   0 asymons  (27005) micas     (3600)     7699 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/io/onnx/conv.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      976 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/io/onnx/default.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     5776 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/io/onnx/gemm.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     4073 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/io/onnx/matmul.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     5079 2024-02-05 12:45:14.000000 zigzag_dse-3.1.0/zigzag/classes/io/onnx/model.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1311 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/io/onnx/parser.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     7792 2024-02-05 12:45:09.000000 zigzag_dse-3.1.0/zigzag/classes/io/onnx/utils.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.612472 zigzag_dse-3.1.0/zigzag/classes/mapping/
--rw-r--r--   0 asymons  (27005) micas     (3600)    40589 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/mapping/combined_mapping.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      578 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/mapping/loop.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     9463 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/mapping/mapping_assist_funcs.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.614472 zigzag_dse-3.1.0/zigzag/classes/mapping/memory/
--rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/mapping/memory/data_layout.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.617473 zigzag_dse-3.1.0/zigzag/classes/mapping/spatial/
--rw-r--r--   0 asymons  (27005) micas     (3600)     8091 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/mapping/spatial/spatial_mapping.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.622473 zigzag_dse-3.1.0/zigzag/classes/mapping/temporal/
--rw-r--r--   0 asymons  (27005) micas     (3600)      442 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/mapping/temporal/temporal_loop.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     7328 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/mapping/temporal/temporal_mapping.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.075450 zigzag_dse-3.1.0/zigzag/classes/opt/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.625473 zigzag_dse-3.1.0/zigzag/classes/opt/spatial/
--rw-r--r--   0 asymons  (27005) micas     (3600)    50477 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/opt/spatial/generator.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.077450 zigzag_dse-3.1.0/zigzag/classes/opt/temporal/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.636474 zigzag_dse-3.1.0/zigzag/classes/opt/temporal/loma/
--rw-r--r--   0 asymons  (27005) micas     (3600)    11540 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/opt/temporal/loma/engine.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      534 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/opt/temporal/loma/loop.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    16495 2024-02-21 09:50:55.000000 zigzag_dse-3.1.0/zigzag/classes/opt/temporal/loma/memory_allocator.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2901 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/opt/temporal/loma/multipermute.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.641474 zigzag_dse-3.1.0/zigzag/classes/opt/temporal/salsa/
--rw-r--r--   0 asymons  (27005) micas     (3600)     8704 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/opt/temporal/salsa/engine.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     3571 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/opt/temporal/salsa/state.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.692476 zigzag_dse-3.1.0/zigzag/classes/stages/
--rw-r--r--   0 asymons  (27005) micas     (3600)     3338 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/stages/CostModelStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1503 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/DumpStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     3212 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/GeneralParameterIteratorStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2087 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/LomaStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2245 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/MainInputParserStages.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      989 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/ONNXModelParserStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     5834 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/PEArrayScalingStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1522 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/PlotTemporalMappingsStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     5951 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/ReduceStages.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     9522 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/RemoveUnusedMemoryStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     6158 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/RunOptStages.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     6449 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/SalsaStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     7298 2024-03-19 15:05:18.000000 zigzag_dse-3.1.0/zigzag/classes/stages/SaveStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    30038 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/SearchUnusedMemoryStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    21259 2024-02-21 09:50:55.000000 zigzag_dse-3.1.0/zigzag/classes/stages/SpatialMappingConversionStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    14699 2024-02-21 09:50:55.000000 zigzag_dse-3.1.0/zigzag/classes/stages/SpatialMappingGeneratorStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2520 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/Stage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     3834 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/TemporalOrderingConversionStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2110 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/stages/WorkloadStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2906 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/__init__.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.704476 zigzag_dse-3.1.0/zigzag/classes/workload/
--rw-r--r--   0 asymons  (27005) micas     (3600)     2771 2024-04-15 08:09:03.000000 zigzag_dse-3.1.0/zigzag/classes/workload/dnn_workload.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2033 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/workload/dummy_node.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    20779 2024-04-15 08:33:58.000000 zigzag_dse-3.1.0/zigzag/classes/workload/layer_node.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1352 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/workload/onnx_workload.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    14521 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/workload/test_layer_node.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.084451 zigzag_dse-3.1.0/zigzag/inputs/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.083451 zigzag_dse-3.1.0/zigzag/inputs/examples/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.723477 zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/
--rwxr-xr-x   0 asymons  (27005) micas     (3600)    10181 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Aimc.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     8496 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Ascend_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     9857 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Dimc.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     5897 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Edge_TPU_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     5817 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Eyeriss_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     7146 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Meta_prototype.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     5162 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/TPU_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     7335 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Tesla_NPU_like.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.739478 zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/
--rw-r--r--   0 asymons  (27005) micas     (3600)      561 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/ascend_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      196 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/default.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)      566 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/default_imc.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      832 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/edge_tpu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      560 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/meta_prototype_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      610 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/tesla_npu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      557 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/tpu_like.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.749478 zigzag_dse-3.1.0/zigzag/inputs/examples/workload/
--rw-r--r--   0 asymons  (27005) micas     (3600)     4067 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/workload/alexnet.onnx
--rw-r--r--   0 asymons  (27005) micas     (3600)    71724 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/workload/mobilenetv2.onnx
--rw-r--r--   0 asymons  (27005) micas     (3600)    18600 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/workload/resnet18.onnx
--rw-r--r--   0 asymons  (27005) micas     (3600)    19065 2024-04-15 09:48:52.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/workload/resnet18.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.084451 zigzag_dse-3.1.0/zigzag/inputs/validation/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.085451 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.088451 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.087451 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.764479 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     7275 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc1_validation_subfunc.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     9625 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc2_validation_subfunc.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     7893 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc3_validation_subfunc.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     1584 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_cost_model.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     6082 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_validation.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)    12159 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/dimc_cost_model.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.089451 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.778479 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/
--rwxr-xr-x   0 asymons  (27005) micas     (3600)    12159 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_cost_model.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     5910 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     1723 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation4.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)    13681 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation_subfunc.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     7526 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation_subfunc4.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     3566 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/model_extration_28nm.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      736 2024-01-03 17:30:21.000000 zigzag_dse-3.1.0/zigzag/utils.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.091451 zigzag_dse-3.1.0/zigzag/visualization/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.782479 zigzag_dse-3.1.0/zigzag/visualization/graph/
--rw-r--r--   0 asymons  (27005) micas     (3600)     1527 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/visualization/graph/memory_hierarchy.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1280 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/visualization/graph/workload.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.786480 zigzag_dse-3.1.0/zigzag/visualization/results/
--rw-r--r--   0 asymons  (27005) micas     (3600)     8785 2024-03-19 14:52:57.000000 zigzag_dse-3.1.0/zigzag/visualization/results/plot_cme.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     4220 2024-04-15 08:09:03.000000 zigzag_dse-3.1.0/zigzag/visualization/results/print_mapping.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.801480 zigzag_dse-3.1.0/zigzag_dse.egg-info/
--rw-r--r--   0 asymons  (27005) micas     (3600)    10722 2024-04-15 09:56:03.000000 zigzag_dse-3.1.0/zigzag_dse.egg-info/PKG-INFO
--rw-r--r--   0 asymons  (27005) micas     (3600)    13397 2024-04-15 09:56:04.000000 zigzag_dse-3.1.0/zigzag_dse.egg-info/SOURCES.txt
--rw-r--r--   0 asymons  (27005) micas     (3600)        1 2024-04-15 09:56:03.000000 zigzag_dse-3.1.0/zigzag_dse.egg-info/dependency_links.txt
--rw-r--r--   0 asymons  (27005) micas     (3600)       52 2024-04-15 09:56:03.000000 zigzag_dse-3.1.0/zigzag_dse.egg-info/entry_points.txt
--rw-r--r--   0 asymons  (27005) micas     (3600)      144 2024-04-15 09:56:03.000000 zigzag_dse-3.1.0/zigzag_dse.egg-info/requires.txt
--rw-r--r--   0 asymons  (27005) micas     (3600)       18 2024-04-15 09:56:03.000000 zigzag_dse-3.1.0/zigzag_dse.egg-info/top_level.txt
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:18.010040 zigzag_dse-3.1.1/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1074 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/LICENSE
+-rw-r--r--   0 asymons  (27005) micas     (3600)       88 2024-01-03 17:20:40.000000 zigzag_dse-3.1.1/MANIFEST.in
+-rw-r--r--   0 asymons  (27005) micas     (3600)    10698 2024-05-17 09:36:18.008040 zigzag_dse-3.1.1/PKG-INFO
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8519 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/README.md
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.673026 zigzag_dse-3.1.1/lab1/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3577 2024-05-17 09:24:49.000000 zigzag_dse-3.1.1/lab1/main.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.602023 zigzag_dse-3.1.1/lab2/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.675026 zigzag_dse-3.1.1/lab2/solutions/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3509 2024-05-17 09:24:49.000000 zigzag_dse-3.1.1/lab2/solutions/main.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.678026 zigzag_dse-3.1.1/lab3/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1484 2024-05-17 09:24:49.000000 zigzag_dse-3.1.1/lab3/main.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1577 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/pyproject.toml
+-rw-r--r--   0 asymons  (27005) micas     (3600)       38 2024-05-17 09:36:18.010040 zigzag_dse-3.1.1/setup.cfg
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.605023 zigzag_dse-3.1.1/tests/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.609023 zigzag_dse-3.1.1/tests/main/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.685027 zigzag_dse-3.1.1/tests/main/test_imc/
+-rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/tests/main/test_imc/__init__.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1598 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/tests/main/test_imc/test_aimc.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1571 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/tests/main/test_imc/test_dimc.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.698027 zigzag_dse-3.1.1/tests/main/test_origin/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1159 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/tests/main/test_origin/test_ascend_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1159 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/tests/main/test_origin/test_edge_tpu_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1172 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/tests/main/test_origin/test_meta_prototype_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1158 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/tests/main/test_origin/test_tesla_npu_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1144 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/tests/main/test_origin/test_tpu_like.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.713028 zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/
+-rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-05-15 14:16:38.000000 zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/__init__.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2070 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/test_ascend_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2716 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/test_edge_tpu_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2144 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/test_meta_prototype_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2113 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/test_tesla_npu_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2281 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/test_tpu_like.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.726028 zigzag_dse-3.1.1/tests/main/test_without_unused_memory/
+-rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_without_unused_memory/__init__.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1310 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_without_unused_memory/test_ascend_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1329 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_without_unused_memory/test_edge_tpu_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1341 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_without_unused_memory/test_meta_prototype_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1335 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_without_unused_memory/test_tesla_npu_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1320 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/tests/main/test_without_unused_memory/test_tpu_like.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.738029 zigzag_dse-3.1.1/zigzag/
+-rw-r--r--   0 asymons  (27005) micas     (3600)       22 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/__init__.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3175 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/__main__.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    20951 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/api.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.740029 zigzag_dse-3.1.1/zigzag/cacti/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.745029 zigzag_dse-3.1.1/zigzag/cacti/cacti_master/
+-rw-r--r--   0 asymons  (27005) micas     (3600)    19996 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/cacti/cacti_master/cacti_config_creator.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     4266 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/cacti/cacti_master/cacti_top.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     7388 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/cacti/cacti_parser.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.751029 zigzag_dse-3.1.1/zigzag/cost_model/
+-rw-r--r--   0 asymons  (27005) micas     (3600)    19531 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/cost_model/CostModelEvaluationForIMC.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    58803 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/cost_model/cost_model.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3460 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/cost_model/port_activity.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3417 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/datatypes.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.615023 zigzag_dse-3.1.1/zigzag/hardware/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.816032 zigzag_dse-3.1.1/zigzag/hardware/architecture/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1164 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/Accelerator.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      912 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/Adder.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    22786 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/AimcArray.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5441 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/Core.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    41212 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/DimcArray.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1881 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/ImcArray.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8583 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/MemoryHierarchy.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3730 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/MemoryInstance.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    27401 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/get_cacti_cost.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    10950 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/imc_unit.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     7046 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/memory_level.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2680 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/memory_port.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2830 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/operational_array.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1728 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/hardware/architecture/operational_unit.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.618023 zigzag_dse-3.1.1/zigzag/inputs/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.619024 zigzag_dse-3.1.1/zigzag/inputs/validation/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.620024 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.648025 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.647025 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.834033 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     7533 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc1_validation_subfunc.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)    10670 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc2_validation_subfunc.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     8317 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc3_validation_subfunc.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     1557 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_cost_model.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     5101 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_validation.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)    12528 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/dimc_cost_model.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.651025 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.850033 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)    12528 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_cost_model.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     5094 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     1433 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation4.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)    15946 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation_subfunc.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     8348 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation_subfunc4.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     3649 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/model_extration_28nm.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.865034 zigzag_dse-3.1.1/zigzag/mapping/
+-rw-r--r--   0 asymons  (27005) micas     (3600)    31830 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/mapping/Mapping.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8281 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/mapping/SpatialMappingInternal.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     6848 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/mapping/TemporalMapping.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8031 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/mapping/data_movement.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8296 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/mapping/mapping_assist_funcs.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    14492 2024-05-16 14:37:13.000000 zigzag_dse-3.1.1/zigzag/mapping/spatial_mapping.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.656025 zigzag_dse-3.1.1/zigzag/opt/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.874034 zigzag_dse-3.1.1/zigzag/opt/loma/
+-rw-r--r--   0 asymons  (27005) micas     (3600)    11960 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/opt/loma/LomaEngine.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      532 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/opt/loma/Loop.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    17039 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/opt/loma/MemoryAllocator.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2444 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/opt/loma/multipermute.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.878034 zigzag_dse-3.1.1/zigzag/opt/salsa/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8189 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/opt/salsa/SalsaEngine.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3528 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/opt/salsa/SalsaState.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.893035 zigzag_dse-3.1.1/zigzag/parser/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9155 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/parser/AcceleratorValidator.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     4035 2024-05-16 12:47:21.000000 zigzag_dse-3.1.1/zigzag/parser/MappingValidator.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3405 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/parser/UpgradedValidator.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5314 2024-05-16 09:09:31.000000 zigzag_dse-3.1.1/zigzag/parser/WorkloadValidator.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     7711 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/parser/accelerator_factory.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.909036 zigzag_dse-3.1.1/zigzag/parser/onnx/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5399 2024-05-16 12:47:21.000000 zigzag_dse-3.1.1/zigzag/parser/onnx/ConvParser.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1029 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/parser/onnx/DefaultNodeParser.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     4987 2024-05-16 12:47:21.000000 zigzag_dse-3.1.1/zigzag/parser/onnx/GemmParser.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3435 2024-05-16 12:47:21.000000 zigzag_dse-3.1.1/zigzag/parser/onnx/MatMulParser.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     4209 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/parser/onnx/ONNXModelParser.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1931 2024-05-16 12:47:21.000000 zigzag_dse-3.1.1/zigzag/parser/onnx/ONNXOperatorParser.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     7891 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/parser/onnx/utils.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    11778 2024-05-16 12:47:21.000000 zigzag_dse-3.1.1/zigzag/parser/workload_factory.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.959038 zigzag_dse-3.1.1/zigzag/stages/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1515 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/AcceleratorParserStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2721 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/CostModelStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1542 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/DumpStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2556 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/GeneralParameterIteratorStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1831 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/LomaStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      731 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/MainStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      862 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/ONNXModelParserStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     6002 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/PEArrayScalingStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1630 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/PlotTemporalMappingsStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9273 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/RemoveUnusedMemoryStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     6024 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/SalsaStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    28132 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/SearchUnusedMemoryStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    14263 2024-05-16 15:04:44.000000 zigzag_dse-3.1.1/zigzag/stages/SpatialMappingConversionStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    33280 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/SpatialMappingGeneratorStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1980 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/Stage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3034 2024-05-16 12:47:21.000000 zigzag_dse-3.1.1/zigzag/stages/TemporalOrderingConversionStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2427 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/WorkloadParserStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1908 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/WorkloadStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5236 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/reduce_stages.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     6322 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/run_opt_stages.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     6348 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/stages/save_stages.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2146 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/utils.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.663025 zigzag_dse-3.1.1/zigzag/visualization/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.964038 zigzag_dse-3.1.1/zigzag/visualization/graph/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1626 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/visualization/graph/memory_hierarchy.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      963 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/visualization/graph/workload.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.969038 zigzag_dse-3.1.1/zigzag/visualization/results/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9369 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/visualization/results/plot_cme.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5532 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/visualization/results/print_mapping.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:17.989039 zigzag_dse-3.1.1/zigzag/workload/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1130 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/workload/DNNWorkload.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2260 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/workload/DummyNode.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      890 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/workload/LayerAttribute.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      611 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/workload/LayerNodeABC.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1083 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/workload/ONNXWorkload.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1063 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/workload/Workload.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     6904 2024-05-16 12:47:21.000000 zigzag_dse-3.1.1/zigzag/workload/layer_attributes.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    14891 2024-05-15 14:16:39.000000 zigzag_dse-3.1.1/zigzag/workload/layer_node.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-05-17 09:36:18.005040 zigzag_dse-3.1.1/zigzag_dse.egg-info/
+-rw-r--r--   0 asymons  (27005) micas     (3600)    10698 2024-05-17 09:36:17.000000 zigzag_dse-3.1.1/zigzag_dse.egg-info/PKG-INFO
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5368 2024-05-17 09:36:17.000000 zigzag_dse-3.1.1/zigzag_dse.egg-info/SOURCES.txt
+-rw-r--r--   0 asymons  (27005) micas     (3600)        1 2024-05-17 09:36:17.000000 zigzag_dse-3.1.1/zigzag_dse.egg-info/dependency_links.txt
+-rw-r--r--   0 asymons  (27005) micas     (3600)       52 2024-05-17 09:36:17.000000 zigzag_dse-3.1.1/zigzag_dse.egg-info/entry_points.txt
+-rw-r--r--   0 asymons  (27005) micas     (3600)      116 2024-05-17 09:36:17.000000 zigzag_dse-3.1.1/zigzag_dse.egg-info/requires.txt
+-rw-r--r--   0 asymons  (27005) micas     (3600)       39 2024-05-17 09:36:17.000000 zigzag_dse-3.1.1/zigzag_dse.egg-info/top_level.txt
```

### Comparing `zigzag_dse-3.1.0/LICENSE` & `zigzag_dse-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.0/PKG-INFO` & `zigzag_dse-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigzag-dse
-Version: 3.1.0
+Version: 3.1.1
 Summary: ZigZag - Deep Learning Hardware Design Space Exploration
 Author-email: Arne Symons <arne.symons@kuleuven.be>, Linyan Mei <linyan.mei@kuleuven.be>
 License: MIT License
         
         Copyright (c) 2021 MICAS (KU Leuven)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,26 +25,26 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/ZigZag-Project/zigzag
 Keywords: zigzag,dse,design-space-exploration,machine-learning,deep-learning,mapping
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: networkx
 Requires-Dist: sympy
 Requires-Dist: matplotlib
 Requires-Dist: onnx
 Requires-Dist: tqdm
 Requires-Dist: multiprocessing_on_dill
 Requires-Dist: pyyaml
-Requires-Dist: tomli; python_version < "3.11"
+Requires-Dist: tomli
 Provides-Extra: dev
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # ZigZag [Documentation](https://kuleuven-micas.github.io/zigzag/) [Tutorial](https://www.youtube.com/watch?v=VgUuG4QaSQQ&list=PLUi74Rw4uFDIuK_6FCF9Bv7SMJlHfG4l3&index=1)
```

### Comparing `zigzag_dse-3.1.0/README.md` & `zigzag_dse-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `zigzag_dse-3.1.0/pyproject.toml` & `zigzag_dse-3.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 where = ["."]  # ["."] by default
 include = ["*"]  # ["*"] by default
 exclude = ["inputs*", "outputs*", "docs*"]
 namespaces = true  # true by default
 
 [project]
 name = "zigzag-dse"
-version = "3.1.0"
+version = "3.1.1"
 description = "ZigZag - Deep Learning Hardware Design Space Exploration"
 readme = "README.md"
 authors = [{ name = "Arne Symons", email = "arne.symons@kuleuven.be" }, { name = "Linyan Mei", email = "linyan.mei@kuleuven.be" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
@@ -26,30 +26,30 @@
     'networkx',
     'sympy',
     'matplotlib',
     'onnx',
     'tqdm',
     'multiprocessing_on_dill',
     'pyyaml',
-    'tomli; python_version < "3.11"',
+    'tomli',
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.11"
 
 
 [project.optional-dependencies]
 dev = ["bumpver", "pip-tools", "build", "twine"]
 
 [project.urls]
 Homepage = "https://github.com/ZigZag-Project/zigzag"
 
 [project.scripts]
 realpython = "zigzag.__main__:main"
 
 [tool.bumpver]
-current_version = "3.1.0"
+current_version = "3.1.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `zigzag_dse-3.1.0/tests/main/test_imc/test_aimc.py` & `zigzag_dse-3.1.1/tests/main/test_imc/test_aimc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import pytest
+import sys
 
+sys.path.append("../zigzag")
 from zigzag.api import get_hardware_performance_zigzag_imc
 
 workloads = (
     "zigzag/inputs/examples/workload/alexnet.onnx",
     "zigzag/inputs/examples/workload/mobilenetv2.onnx",
     "zigzag/inputs/examples/workload/resnet18.onnx",
     "zigzag.inputs.examples.workload.resnet18",
@@ -26,15 +28,13 @@
 @pytest.fixture
 def accelerator():
     return "zigzag.inputs.examples.hardware.Aimc"
 
 
 @pytest.mark.parametrize("workload", workloads)
 def test_api(workload, accelerator, mapping):
-    (energy, latency, tclk, area, cmes) = get_hardware_performance_zigzag_imc(
-        workload, accelerator, mapping
-    )
+    (energy, latency, tclk, area, cmes) = get_hardware_performance_zigzag_imc(workload, accelerator, mapping)
     (expected_energy, expected_latency, expected_tclk, expected_area) = ens_lats_clks_areas[workload]
     assert energy == pytest.approx(expected_energy)
     assert latency == pytest.approx(expected_latency)
     assert tclk == pytest.approx(expected_tclk)
     assert area == pytest.approx(expected_area)
```

### Comparing `zigzag_dse-3.1.0/tests/main/test_imc/test_dimc.py` & `zigzag_dse-3.1.1/tests/main/test_imc/test_dimc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import pytest
+import sys
 
+sys.path.append("../zigzag")
 from zigzag.api import get_hardware_performance_zigzag_imc
 
 workloads = (
     "zigzag/inputs/examples/workload/alexnet.onnx",
     "zigzag/inputs/examples/workload/mobilenetv2.onnx",
     "zigzag/inputs/examples/workload/resnet18.onnx",
     "zigzag.inputs.examples.workload.resnet18",
@@ -26,15 +28,13 @@
 @pytest.fixture
 def accelerator():
     return "zigzag.inputs.examples.hardware.Dimc"
 
 
 @pytest.mark.parametrize("workload", workloads)
 def test_api(workload, accelerator, mapping):
-    (energy, latency, tclk, area, cmes) = get_hardware_performance_zigzag_imc(
-        workload, accelerator, mapping
-    )
+    (energy, latency, tclk, area, cmes) = get_hardware_performance_zigzag_imc(workload, accelerator, mapping)
     (expected_energy, expected_latency, expected_tclk, expected_area) = ens_lats_clks_areas[workload]
     assert energy == pytest.approx(expected_energy)
     assert latency == pytest.approx(expected_latency)
     assert tclk == pytest.approx(expected_tclk)
     assert area == pytest.approx(expected_area)
```

### Comparing `zigzag_dse-3.1.0/tests/main/test_origin/test_ascend_like.py` & `zigzag_dse-3.1.1/tests/main/test_without_unused_memory/test_ascend_like.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import pytest
+import sys
 
-from zigzag.api import get_hardware_performance_zigzag
+sys.path.append("../zigzag")
+from zigzag.api import get_hardware_performance_zigzag_without_unused_memory
 
 workloads = (
     "zigzag/inputs/examples/workload/alexnet.onnx",
     "zigzag/inputs/examples/workload/mobilenetv2.onnx",
     "zigzag/inputs/examples/workload/resnet18.onnx",
     "zigzag.inputs.examples.workload.resnet18",
 )
 
 # Expected energy and latency for each workload defined above
 ens_lats = {
-    "zigzag/inputs/examples/workload/alexnet.onnx": (5738192980.375, 8728331),
-    "zigzag/inputs/examples/workload/mobilenetv2.onnx": (1913797698.5250015, 7426499),
-    "zigzag/inputs/examples/workload/resnet18.onnx": (1858697886.165, 3720129),
-    "zigzag.inputs.examples.workload.resnet18": (2408671233.7250004, 4804196),
+    "zigzag/inputs/examples/workload/alexnet.onnx": (5649555894.9, 8637780),
+    "zigzag/inputs/examples/workload/mobilenetv2.onnx": (1881386179.71, 6486685),
+    "zigzag/inputs/examples/workload/resnet18.onnx": (1709089377.83, 3583047),
+    "zigzag.inputs.examples.workload.resnet18": (2243493483.15, 4657130),
 }
 
 
 @pytest.fixture
 def mapping():
     return "zigzag.inputs.examples.mapping.ascend_like"
 
@@ -26,13 +28,11 @@
 @pytest.fixture
 def accelerator():
     return "zigzag.inputs.examples.hardware.Ascend_like"
 
 
 @pytest.mark.parametrize("workload", workloads)
 def test_api(workload, accelerator, mapping):
-    (energy, latency, cmes) = get_hardware_performance_zigzag(
-        workload, accelerator, mapping
-    )
+    (energy, latency, cmes) = get_hardware_performance_zigzag_without_unused_memory(workload, accelerator, mapping)
     (expected_energy, expected_latency) = ens_lats[workload]
     assert energy == pytest.approx(expected_energy)
     assert latency == pytest.approx(expected_latency)
```

### Comparing `zigzag_dse-3.1.0/tests/main/test_origin/test_edge_tpu_like.py` & `zigzag_dse-3.1.1/tests/main/test_without_unused_memory/test_edge_tpu_like.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import pytest
+import sys
 
-from zigzag.api import get_hardware_performance_zigzag
+sys.path.append("../zigzag")
+from zigzag.api import get_hardware_performance_zigzag_without_unused_memory
 
 workloads = (
     "zigzag/inputs/examples/workload/alexnet.onnx",
     "zigzag/inputs/examples/workload/mobilenetv2.onnx",
     "zigzag/inputs/examples/workload/resnet18.onnx",
     "zigzag.inputs.examples.workload.resnet18",
 )
 
 # Expected energy and latency for each workload defined above
 ens_lats = {
-    "zigzag/inputs/examples/workload/alexnet.onnx": (5657179533.855, 8256774),
-    "zigzag/inputs/examples/workload/mobilenetv2.onnx": (1694757317.6950002, 3722532),
-    "zigzag/inputs/examples/workload/resnet18.onnx": (1903877328.0199995, 3363983),
-    "zigzag.inputs.examples.workload.resnet18": (2413350265.7900004, 4314851),
+    "zigzag/inputs/examples/workload/alexnet.onnx": (5568602396.684999, 8134431),
+    "zigzag/inputs/examples/workload/mobilenetv2.onnx": (751128562.4699999, 2427487),
+    "zigzag/inputs/examples/workload/resnet18.onnx": (1784539639.4349997, 3176546),
+    "zigzag.inputs.examples.workload.resnet18": (2115122870.395, 3884789),
 }
 
 
 @pytest.fixture
 def mapping():
     return "zigzag.inputs.examples.mapping.edge_tpu_like"
 
@@ -26,13 +28,11 @@
 @pytest.fixture
 def accelerator():
     return "zigzag.inputs.examples.hardware.Edge_TPU_like"
 
 
 @pytest.mark.parametrize("workload", workloads)
 def test_api(workload, accelerator, mapping):
-    (energy, latency, cmes) = get_hardware_performance_zigzag(
-        workload, accelerator, mapping
-    )
+    (energy, latency, cmes) = get_hardware_performance_zigzag_without_unused_memory(workload, accelerator, mapping)
     (expected_energy, expected_latency) = ens_lats[workload]
     assert energy == pytest.approx(expected_energy)
     assert latency == pytest.approx(expected_latency)
```

### Comparing `zigzag_dse-3.1.0/tests/main/test_origin/test_meta_prototype_like.py` & `zigzag_dse-3.1.1/tests/main/test_without_unused_memory/test_meta_prototype_like.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import pytest
+import sys
 
-from zigzag.api import get_hardware_performance_zigzag
+sys.path.append("../zigzag")
+from zigzag.api import get_hardware_performance_zigzag_without_unused_memory
 
 workloads = (
     "zigzag/inputs/examples/workload/alexnet.onnx",
     "zigzag/inputs/examples/workload/mobilenetv2.onnx",
     "zigzag/inputs/examples/workload/resnet18.onnx",
     "zigzag.inputs.examples.workload.resnet18",
 )
 
 # Expected energy and latency for each workload defined above
 ens_lats = {
-    "zigzag/inputs/examples/workload/alexnet.onnx": (5771558839.89, 8400651),
-    "zigzag/inputs/examples/workload/mobilenetv2.onnx": (1731935837.864999, 3594631),
-    "zigzag/inputs/examples/workload/resnet18.onnx": (1869519792.3449998, 3408373),
-    "zigzag.inputs.examples.workload.resnet18": (2419893343.4549994, 4176163),
+    "zigzag/inputs/examples/workload/alexnet.onnx": (5679695605.4400015, 8299150),
+    "zigzag/inputs/examples/workload/mobilenetv2.onnx": (901092009.6000001, 2610609),
+    "zigzag/inputs/examples/workload/resnet18.onnx": (1730672410.3200004, 3262009),
+    "zigzag.inputs.examples.workload.resnet18": (2265438430.2299995, 4017227),
 }
 
 
 @pytest.fixture
 def mapping():
     return "zigzag.inputs.examples.mapping.meta_prototype_like"
 
@@ -26,13 +28,11 @@
 @pytest.fixture
 def accelerator():
     return "zigzag.inputs.examples.hardware.Meta_prototype"
 
 
 @pytest.mark.parametrize("workload", workloads)
 def test_api(workload, accelerator, mapping):
-    (energy, latency, cmes) = get_hardware_performance_zigzag(
-        workload, accelerator, mapping
-    )
+    (energy, latency, cmes) = get_hardware_performance_zigzag_without_unused_memory(workload, accelerator, mapping)
     (expected_energy, expected_latency) = ens_lats[workload]
     assert energy == pytest.approx(expected_energy)
     assert latency == pytest.approx(expected_latency)
```

### Comparing `zigzag_dse-3.1.0/tests/main/test_origin/test_tesla_npu_like.py` & `zigzag_dse-3.1.1/tests/main/test_without_unused_memory/test_tesla_npu_like.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import pytest
+import sys
 
-from zigzag.api import get_hardware_performance_zigzag
+sys.path.append("../zigzag")
+from zigzag.api import get_hardware_performance_zigzag_without_unused_memory
 
 workloads = (
     "zigzag/inputs/examples/workload/alexnet.onnx",
     "zigzag/inputs/examples/workload/mobilenetv2.onnx",
     "zigzag/inputs/examples/workload/resnet18.onnx",
     "zigzag.inputs.examples.workload.resnet18",
 )
 
 # Expected energy and latency for each workload defined above
 ens_lats = {
-    "zigzag/inputs/examples/workload/alexnet.onnx": (6131950030.816001, 8486444),
-    "zigzag/inputs/examples/workload/mobilenetv2.onnx": (1671933042.2130003, 2909436),
-    "zigzag/inputs/examples/workload/resnet18.onnx": (1863717063.505, 3395752),
-    "zigzag.inputs.examples.workload.resnet18": (2375316568.8910007, 4082454),
+    "zigzag/inputs/examples/workload/alexnet.onnx": (6040086796.366001, 8389669),
+    "zigzag/inputs/examples/workload/mobilenetv2.onnx": (930702060.6110002, 1965457),
+    "zigzag/inputs/examples/workload/resnet18.onnx": (1724869681.4799998, 3257898),
+    "zigzag.inputs.examples.workload.resnet18": (2220861655.6660004, 3934616),
 }
 
 
 @pytest.fixture
 def mapping():
     return "zigzag.inputs.examples.mapping.tesla_npu_like"
 
@@ -26,13 +28,11 @@
 @pytest.fixture
 def accelerator():
     return "zigzag.inputs.examples.hardware.Tesla_NPU_like"
 
 
 @pytest.mark.parametrize("workload", workloads)
 def test_api(workload, accelerator, mapping):
-    (energy, latency, cmes) = get_hardware_performance_zigzag(
-        workload, accelerator, mapping
-    )
+    (energy, latency, cmes) = get_hardware_performance_zigzag_without_unused_memory(workload, accelerator, mapping)
     (expected_energy, expected_latency) = ens_lats[workload]
     assert energy == pytest.approx(expected_energy)
     assert latency == pytest.approx(expected_latency)
```

### Comparing `zigzag_dse-3.1.0/tests/main/test_origin/test_tpu_like.py` & `zigzag_dse-3.1.1/tests/main/test_without_unused_memory/test_tpu_like.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import pytest
+import sys
 
-from zigzag.api import get_hardware_performance_zigzag
+sys.path.append("../zigzag")
+from zigzag.api import get_hardware_performance_zigzag_without_unused_memory
 
 workloads = (
     "zigzag/inputs/examples/workload/alexnet.onnx",
     "zigzag/inputs/examples/workload/mobilenetv2.onnx",
     "zigzag/inputs/examples/workload/resnet18.onnx",
     "zigzag.inputs.examples.workload.resnet18",
 )
 
 # Expected energy and latency for each workload defined above
 ens_lats = {
-    "zigzag/inputs/examples/workload/alexnet.onnx": (5567502618.941999, 9078209),
-    "zigzag/inputs/examples/workload/mobilenetv2.onnx": (1904494517.552001, 23112606),
-    "zigzag/inputs/examples/workload/resnet18.onnx": (1795904779.6570003, 4160591),
-    "zigzag.inputs.examples.workload.resnet18": (2296491401.491, 4909027),
+    "zigzag/inputs/examples/workload/alexnet.onnx": (5475639384.492001, 8979956),
+    "zigzag/inputs/examples/workload/mobilenetv2.onnx": (952688145.0069999, 21873214),
+    "zigzag/inputs/examples/workload/resnet18.onnx": (1659252422.016, 4000289),
+    "zigzag.inputs.examples.workload.resnet18": (1982830786.5119998, 4509235),
 }
 
 
 @pytest.fixture
 def mapping():
     return "zigzag.inputs.examples.mapping.tpu_like"
 
@@ -26,13 +28,11 @@
 @pytest.fixture
 def accelerator():
     return "zigzag.inputs.examples.hardware.TPU_like"
 
 
 @pytest.mark.parametrize("workload", workloads)
 def test_api(workload, accelerator, mapping):
-    (energy, latency, cmes) = get_hardware_performance_zigzag(
-        workload, accelerator, mapping
-    )
+    (energy, latency, cmes) = get_hardware_performance_zigzag_without_unused_memory(workload, accelerator, mapping)
     (expected_energy, expected_latency) = ens_lats[workload]
     assert energy == pytest.approx(expected_energy)
     assert latency == pytest.approx(expected_latency)
```

### Comparing `zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/test_ascend_like.py` & `zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/test_meta_prototype_like.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 import pytest
+import sys
 
+sys.path.append("../zigzag")
 from zigzag.api import get_hardware_performance_zigzag_with_mix_spatial_mapping
 
-# Test case for when spatial_mapping is provided, while spatial_mapping_hint is not provided.
+# Test case for when an incomplete spatial_mapping is provided and spatial_mapping_hint is also provided.
 
 workloads = (
     "zigzag/inputs/examples/workload/alexnet.onnx",
     "zigzag/inputs/examples/workload/mobilenetv2.onnx",
     "zigzag/inputs/examples/workload/resnet18.onnx",
     "zigzag.inputs.examples.workload.resnet18",
 )
 
 # Expected energy and latency for each workload defined above
 ens_lats = {
-    "zigzag/inputs/examples/workload/alexnet.onnx": (5667407342.66, 8528846),
-    "zigzag/inputs/examples/workload/mobilenetv2.onnx": (921552096.0700004, 3828967),
-    "zigzag/inputs/examples/workload/resnet18.onnx": (1679218425.5100002, 3713386),
-    "zigzag.inputs.examples.workload.resnet18": (2290766279.31, 4442443),
+    "zigzag/inputs/examples/workload/alexnet.onnx": (5679695605, 8299150),
+    "zigzag/inputs/examples/workload/mobilenetv2.onnx": (901092009, 2610609),
+    "zigzag/inputs/examples/workload/resnet18.onnx": (1730672410, 3262009),
+    "zigzag.inputs.examples.workload.resnet18": (2265438430, 4017227),
 }
 
 
 @pytest.fixture
 def mapping():
-    ascend_like_mapping = {
+    meta_prototype_like_mapping = {
         "default": {
             "core_allocation": 1,
             "spatial_mapping": {
-                "D1": ("K", 16),
-                "D2": (("C", 4), ("FX", 3)),
-                "D3": ("OX", 2),
-                "D4": ("OY", 2),
+                "D1": ("K", 32),
+                # "D2": ("C", 2),
+                "D3": (("OX", 2), ("OY", 2)),
+                "D4": (("OX", 2), ("OY", 2)),
             },
+            "spatial_mapping_hint": {"D2": ["C"]},
             "memory_operand_links": {"O": "O", "W": "I2", "I": "I1"},
         },
         "Add": {
             "core_allocation": 1,
             "spatial_mapping": {
-                "D1": ("G", 16),
+                "D1": ("G", 32),
                 "D2": ("C", 1),
                 "D3": ("OX", 1),
                 "D4": ("OY", 1),
             },
             "memory_operand_links": {"O": "O", "X": "I2", "Y": "I1"},
         },
     }
-
-    return ascend_like_mapping
+    return meta_prototype_like_mapping
 
 
 @pytest.fixture
 def accelerator():
-    return "zigzag.inputs.examples.hardware.Ascend_like"
+    return "zigzag.inputs.examples.hardware.Meta_prototype"
 
 
 @pytest.mark.parametrize("workload", workloads)
 def test_api(workload, accelerator, mapping):
-    (energy, latency, cmes) = get_hardware_performance_zigzag_with_mix_spatial_mapping(
-        workload, accelerator, mapping
-    )
+    (energy, latency, cmes) = get_hardware_performance_zigzag_with_mix_spatial_mapping(workload, accelerator, mapping)
     (expected_energy, expected_latency) = ens_lats[workload]
     assert energy == pytest.approx(expected_energy)
     assert latency == pytest.approx(expected_latency)
```

### Comparing `zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/test_edge_tpu_like.py` & `zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/test_edge_tpu_like.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import pytest
+import sys
 
+sys.path.append("../zigzag")
 from zigzag.api import get_hardware_performance_zigzag_with_mix_spatial_mapping
 
 # Test case for when both spatial_mapping and spatial_mapping_hint are provided.
 
 workloads = (
     "zigzag/inputs/examples/workload/alexnet.onnx",
     "zigzag/inputs/examples/workload/mobilenetv2.onnx",
@@ -67,13 +69,11 @@
 @pytest.fixture
 def accelerator():
     return "zigzag.inputs.examples.hardware.Edge_TPU_like"
 
 
 @pytest.mark.parametrize("workload", workloads)
 def test_api(workload, accelerator, mapping):
-    (energy, latency, cmes) = get_hardware_performance_zigzag_with_mix_spatial_mapping(
-        workload, accelerator, mapping
-    )
+    (energy, latency, cmes) = get_hardware_performance_zigzag_with_mix_spatial_mapping(workload, accelerator, mapping)
     (expected_energy, expected_latency) = ens_lats[workload]
     assert energy == pytest.approx(expected_energy)
     assert latency == pytest.approx(expected_latency)
```

### Comparing `zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/test_meta_prototype_like.py` & `zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/test_tesla_npu_like.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,59 @@
 import pytest
+import sys
 
+sys.path.append("../zigzag")
 from zigzag.api import get_hardware_performance_zigzag_with_mix_spatial_mapping
 
-# Test case for when an incomplete spatial_mapping is provided and spatial_mapping_hint is also provided.
+# Test case for when only spatial_mapping_hint is provided.
 
 workloads = (
     "zigzag/inputs/examples/workload/alexnet.onnx",
     "zigzag/inputs/examples/workload/mobilenetv2.onnx",
     "zigzag/inputs/examples/workload/resnet18.onnx",
     "zigzag.inputs.examples.workload.resnet18",
 )
 
 # Expected energy and latency for each workload defined above
 ens_lats = {
-    "zigzag/inputs/examples/workload/alexnet.onnx": (5679695605, 8299150),
-    "zigzag/inputs/examples/workload/mobilenetv2.onnx": (901092009, 2610609),
-    "zigzag/inputs/examples/workload/resnet18.onnx": (1730672410, 3262009),
-    "zigzag.inputs.examples.workload.resnet18": (2265438430, 4017227),
+    "zigzag/inputs/examples/workload/alexnet.onnx": (6044768678, 8370470),
+    "zigzag/inputs/examples/workload/mobilenetv2.onnx": (930702060, 1965457),
+    "zigzag/inputs/examples/workload/resnet18.onnx": (1724869681, 3257898),
+    "zigzag.inputs.examples.workload.resnet18": (2220861655, 3934616),
 }
 
 
 @pytest.fixture
 def mapping():
-    meta_prototype_like_mapping = {
+    tesla_npu_like_mapping = {
         "default": {
             "core_allocation": 1,
-            "spatial_mapping": {
-                "D1": ("K", 32),
-                # "D2": ("C", 2),
-                "D3": (("OX", 2), ("OY", 2)),
-                "D4": (("OX", 2), ("OY", 2)),
-            },
-            "spatial_mapping_hint": {"D2": ["C"]},
+            # "spatial_mapping": {"D1": ("K", 32), "D2": ("OX", 8), "D3": ("OY", 4)},
+            "spatial_mapping_hint": {"D1": ["K"], "D2": ["OX", "OY"]},
             "memory_operand_links": {"O": "O", "W": "I2", "I": "I1"},
         },
         "Add": {
             "core_allocation": 1,
-            "spatial_mapping": {
-                "D1": ("G", 32),
-                "D2": ("C", 1),
-                "D3": ("OX", 1),
-                "D4": ("OY", 1),
-            },
+            "spatial_mapping": {"D1": ("G", 32), "D2": ("OX", 1), "D3": ("OY", 1)},
             "memory_operand_links": {"O": "O", "X": "I2", "Y": "I1"},
         },
+        "Pooling": {
+            "core_allocation": 1,
+            "spatial_mapping": {"D1": ("G", 32), "D2": ("OX", 1), "D3": ("OY", 1)},
+            "memory_operand_links": {"O": "O", "W": "I2", "I": "I1"},
+        },
     }
-    return meta_prototype_like_mapping
+
+    return tesla_npu_like_mapping
 
 
 @pytest.fixture
 def accelerator():
-    return "zigzag.inputs.examples.hardware.Meta_prototype"
+    return "zigzag.inputs.examples.hardware.Tesla_NPU_like"
 
 
 @pytest.mark.parametrize("workload", workloads)
 def test_api(workload, accelerator, mapping):
-    (energy, latency, cmes) = get_hardware_performance_zigzag_with_mix_spatial_mapping(
-        workload, accelerator, mapping
-    )
+    (energy, latency, cmes) = get_hardware_performance_zigzag_with_mix_spatial_mapping(workload, accelerator, mapping)
     (expected_energy, expected_latency) = ens_lats[workload]
     assert energy == pytest.approx(expected_energy)
     assert latency == pytest.approx(expected_latency)
```

### Comparing `zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/test_tesla_npu_like.py` & `zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/test_ascend_like.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,63 @@
 import pytest
+import sys
 
+sys.path.append("../zigzag")
 from zigzag.api import get_hardware_performance_zigzag_with_mix_spatial_mapping
 
-# Test case for when only spatial_mapping_hint is provided.
+# Test case for when spatial_mapping is provided, while spatial_mapping_hint is not provided.
 
 workloads = (
     "zigzag/inputs/examples/workload/alexnet.onnx",
     "zigzag/inputs/examples/workload/mobilenetv2.onnx",
     "zigzag/inputs/examples/workload/resnet18.onnx",
     "zigzag.inputs.examples.workload.resnet18",
 )
 
 # Expected energy and latency for each workload defined above
 ens_lats = {
-    "zigzag/inputs/examples/workload/alexnet.onnx": (6044768678, 8370470),
-    "zigzag/inputs/examples/workload/mobilenetv2.onnx": (930702060, 1965457),
-    "zigzag/inputs/examples/workload/resnet18.onnx": (1724869681, 3257898),
-    "zigzag.inputs.examples.workload.resnet18": (2220861655, 3934616),
+    "zigzag/inputs/examples/workload/alexnet.onnx": (5667407342.66, 8528846),
+    "zigzag/inputs/examples/workload/mobilenetv2.onnx": (921552096.0700004, 3828967),
+    "zigzag/inputs/examples/workload/resnet18.onnx": (1679218425.5100002, 3713386),
+    "zigzag.inputs.examples.workload.resnet18": (2290766279.31, 4442443),
 }
 
 
 @pytest.fixture
 def mapping():
-    tesla_npu_like_mapping = {
+    ascend_like_mapping = {
         "default": {
             "core_allocation": 1,
-            # "spatial_mapping": {"D1": ("K", 32), "D2": ("OX", 8), "D3": ("OY", 4)},
-            "spatial_mapping_hint": {"D1": ["K"], "D2": ["OX", "OY"]},
+            "spatial_mapping": {
+                "D1": ("K", 16),
+                "D2": (("C", 4), ("FX", 3)),
+                "D3": ("OX", 2),
+                "D4": ("OY", 2),
+            },
             "memory_operand_links": {"O": "O", "W": "I2", "I": "I1"},
         },
         "Add": {
             "core_allocation": 1,
-            "spatial_mapping": {"D1": ("G", 32), "D2": ("OX", 1), "D3": ("OY", 1)},
+            "spatial_mapping": {
+                "D1": ("G", 16),
+                "D2": ("C", 1),
+                "D3": ("OX", 1),
+                "D4": ("OY", 1),
+            },
             "memory_operand_links": {"O": "O", "X": "I2", "Y": "I1"},
         },
-        "Pooling": {
-            "core_allocation": 1,
-            "spatial_mapping": {"D1": ("G", 32), "D2": ("OX", 1), "D3": ("OY", 1)},
-            "memory_operand_links": {"O": "O", "W": "I2", "I": "I1"},
-        },
     }
 
-    return tesla_npu_like_mapping
+    return ascend_like_mapping
 
 
 @pytest.fixture
 def accelerator():
-    return "zigzag.inputs.examples.hardware.Tesla_NPU_like"
+    return "zigzag.inputs.examples.hardware.Ascend_like"
 
 
 @pytest.mark.parametrize("workload", workloads)
 def test_api(workload, accelerator, mapping):
-    (energy, latency, cmes) = get_hardware_performance_zigzag_with_mix_spatial_mapping(
-        workload, accelerator, mapping
-    )
+    (energy, latency, cmes) = get_hardware_performance_zigzag_with_mix_spatial_mapping(workload, accelerator, mapping)
     (expected_energy, expected_latency) = ens_lats[workload]
     assert energy == pytest.approx(expected_energy)
     assert latency == pytest.approx(expected_latency)
```

### Comparing `zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/test_tpu_like.py` & `zigzag_dse-3.1.1/tests/main/test_with_mix_spatial_mapping/test_tpu_like.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import pytest
+import sys
 
+sys.path.append("../zigzag")
 from zigzag.api import get_hardware_performance_zigzag_with_mix_spatial_mapping
 
 # Test case for when more non-existent dimensions are provided in spatial_mapping_hint.
 
 workloads = (
     "zigzag/inputs/examples/workload/alexnet.onnx",
     "zigzag/inputs/examples/workload/mobilenetv2.onnx",
@@ -21,19 +23,18 @@
 
 
 @pytest.fixture
 def mapping():
     tpu_like_mapping = {
         "default": {
             "core_allocation": 1,
-            # "spatial_mapping": {
-            #     "D1": ("K", 32),
-            #     "D2": (("C", 2), ("FX", 3), ("FY", 3)),
-            # },
-            # D3 and D4 in spatial_mapping_hint will not work, since they do not exist in the hardware dimensions.
+            "spatial_mapping": {
+                "D1": ("K", 32),
+                "D2": (("C", 2), ("FX", 3), ("FY", 3)),
+            },
             "spatial_mapping_hint": {
                 "D1": ["K"],
                 "D2": ["C", "FX", "FY"],
                 "D3": ["K", "OX"],
                 "D4": ["OX", "OY"],
             },
             "memory_operand_links": {"O": "O", "W": "I2", "I": "I1"},
@@ -56,13 +57,11 @@
 @pytest.fixture
 def accelerator():
     return "zigzag.inputs.examples.hardware.TPU_like"
 
 
 @pytest.mark.parametrize("workload", workloads)
 def test_api(workload, accelerator, mapping):
-    (energy, latency, cmes) = get_hardware_performance_zigzag_with_mix_spatial_mapping(
-        workload, accelerator, mapping
-    )
+    (energy, latency, cmes) = get_hardware_performance_zigzag_with_mix_spatial_mapping(workload, accelerator, mapping)
     (expected_energy, expected_latency) = ens_lats[workload]
     assert energy == pytest.approx(expected_energy)
     assert latency == pytest.approx(expected_latency)
```

### Comparing `zigzag_dse-3.1.0/tests/main/test_without_unused_memory/test_ascend_like.py` & `zigzag_dse-3.1.1/tests/main/test_origin/test_edge_tpu_like.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 import pytest
 
-from zigzag.api import get_hardware_performance_zigzag_without_unused_memory
+from zigzag.api import get_hardware_performance_zigzag
 
 workloads = (
-    "zigzag/inputs/examples/workload/alexnet.onnx",
-    "zigzag/inputs/examples/workload/mobilenetv2.onnx",
-    "zigzag/inputs/examples/workload/resnet18.onnx",
-    "zigzag.inputs.examples.workload.resnet18",
+    "inputs/workload/alexnet.onnx",
+    "inputs/workload/mobilenetv2.onnx",
+    "inputs/workload/resnet18.onnx",
+    "inputs/workload/resnet18.yaml",
 )
 
 # Expected energy and latency for each workload defined above
 ens_lats = {
-    "zigzag/inputs/examples/workload/alexnet.onnx": (5649555894.9, 8637780),
-    "zigzag/inputs/examples/workload/mobilenetv2.onnx": (1881386179.71, 6486685),
-    "zigzag/inputs/examples/workload/resnet18.onnx": (1709089377.83, 3583047),
-    "zigzag.inputs.examples.workload.resnet18": (2243493483.15, 4657130),
+    "inputs/workload/alexnet.onnx": (5657178248.6, 8221391.0),
+    "inputs/workload/mobilenetv2.onnx": (1680773377.4499998, 3562331.0),
+    "inputs/workload/resnet18.onnx": (1902637139.1499994, 3333310.0),
+    "inputs/workload/resnet18.yaml": (2413348670.67, 4268451.0),
 }
 
 
 @pytest.fixture
 def mapping():
-    return "zigzag.inputs.examples.mapping.ascend_like"
+    return "inputs/mapping/edge_tpu_like.yaml"
 
 
 @pytest.fixture
 def accelerator():
-    return "zigzag.inputs.examples.hardware.Ascend_like"
+    return "inputs/hardware/edge_tpu_like.yaml"
 
 
 @pytest.mark.parametrize("workload", workloads)
 def test_api(workload, accelerator, mapping):
-    (energy, latency, cmes) = get_hardware_performance_zigzag_without_unused_memory(
-        workload, accelerator, mapping
-    )
+    (energy, latency, cmes) = get_hardware_performance_zigzag(workload, accelerator, mapping)
     (expected_energy, expected_latency) = ens_lats[workload]
+    print(f"'{workload}': ({energy}, {latency}),")
     assert energy == pytest.approx(expected_energy)
     assert latency == pytest.approx(expected_latency)
```

### Comparing `zigzag_dse-3.1.0/tests/main/test_without_unused_memory/test_edge_tpu_like.py` & `zigzag_dse-3.1.1/tests/main/test_origin/test_tpu_like.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 import pytest
 
-from zigzag.api import get_hardware_performance_zigzag_without_unused_memory
+from zigzag.api import get_hardware_performance_zigzag
 
 workloads = (
-    "zigzag/inputs/examples/workload/alexnet.onnx",
-    "zigzag/inputs/examples/workload/mobilenetv2.onnx",
-    "zigzag/inputs/examples/workload/resnet18.onnx",
-    "zigzag.inputs.examples.workload.resnet18",
+    "inputs/workload/alexnet.onnx",
+    "inputs/workload/mobilenetv2.onnx",
+    "inputs/workload/resnet18.onnx",
+    "inputs/workload/resnet18.yaml",
 )
 
 # Expected energy and latency for each workload defined above
 ens_lats = {
-    "zigzag/inputs/examples/workload/alexnet.onnx": (5568602396.684999, 8134431),
-    "zigzag/inputs/examples/workload/mobilenetv2.onnx": (751128562.4699999, 2427487),
-    "zigzag/inputs/examples/workload/resnet18.onnx": (1784539639.4349997, 3176546),
-    "zigzag.inputs.examples.workload.resnet18": (2115122870.395, 3884789),
+    "inputs/workload/alexnet.onnx": (5567501203.632, 9061821.0),
+    "inputs/workload/mobilenetv2.onnx": (1904482765.907, 23101112.0),
+    "inputs/workload/resnet18.onnx": (1795904402.5120003, 4158539.0),
+    "inputs/workload/resnet18.yaml": (2296490149.296, 4906975.0),
 }
 
 
 @pytest.fixture
 def mapping():
-    return "zigzag.inputs.examples.mapping.edge_tpu_like"
+    return "inputs/mapping/tpu_like.yaml"
 
 
 @pytest.fixture
 def accelerator():
-    return "zigzag.inputs.examples.hardware.Edge_TPU_like"
+    return "inputs/hardware/tpu_like.yaml"
 
 
 @pytest.mark.parametrize("workload", workloads)
 def test_api(workload, accelerator, mapping):
-    (energy, latency, cmes) = get_hardware_performance_zigzag_without_unused_memory(
-        workload, accelerator, mapping
-    )
+    (energy, latency, _) = get_hardware_performance_zigzag(workload, accelerator, mapping)
     (expected_energy, expected_latency) = ens_lats[workload]
+    print(f"{workload}: ({energy}, {latency}),")
     assert energy == pytest.approx(expected_energy)
     assert latency == pytest.approx(expected_latency)
```

### Comparing `zigzag_dse-3.1.0/tests/main/test_without_unused_memory/test_tesla_npu_like.py` & `zigzag_dse-3.1.1/tests/main/test_origin/test_meta_prototype_like.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 import pytest
 
-from zigzag.api import get_hardware_performance_zigzag_without_unused_memory
+from zigzag.api import get_hardware_performance_zigzag
 
 workloads = (
-    "zigzag/inputs/examples/workload/alexnet.onnx",
-    "zigzag/inputs/examples/workload/mobilenetv2.onnx",
-    "zigzag/inputs/examples/workload/resnet18.onnx",
-    "zigzag.inputs.examples.workload.resnet18",
+    "inputs/workload/alexnet.onnx",
+    "inputs/workload/mobilenetv2.onnx",
+    "inputs/workload/resnet18.onnx",
+    "inputs/workload/resnet18.yaml",
 )
 
 # Expected energy and latency for each workload defined above
 ens_lats = {
-    "zigzag/inputs/examples/workload/alexnet.onnx": (6040086796.366001, 8389669),
-    "zigzag/inputs/examples/workload/mobilenetv2.onnx": (930702060.6110002, 1965457),
-    "zigzag/inputs/examples/workload/resnet18.onnx": (1724869681.4799998, 3257898),
-    "zigzag.inputs.examples.workload.resnet18": (2220861655.6660004, 3934616),
+    "inputs/workload/alexnet.onnx": (5771499135.4800005, 8338950.0),
+    "inputs/workload/mobilenetv2.onnx": (1728572789.1600003, 3429446.0),
+    "inputs/workload/resnet18.onnx": (1869036158.08, 3366695.0),
+    "inputs/workload/resnet18.yaml": (2418511845.2400002, 4130645.0),
 }
 
 
 @pytest.fixture
 def mapping():
-    return "zigzag.inputs.examples.mapping.tesla_npu_like"
+    return "inputs/mapping/meta_prototype_like.yaml"
 
 
 @pytest.fixture
 def accelerator():
-    return "zigzag.inputs.examples.hardware.Tesla_NPU_like"
+    return "inputs/hardware/meta_prototype.yaml"
 
 
 @pytest.mark.parametrize("workload", workloads)
 def test_api(workload, accelerator, mapping):
-    (energy, latency, cmes) = get_hardware_performance_zigzag_without_unused_memory(
-        workload, accelerator, mapping
-    )
+    (energy, latency, cmes) = get_hardware_performance_zigzag(workload, accelerator, mapping)
     (expected_energy, expected_latency) = ens_lats[workload]
+    print(f"'{workload}': ({energy}, {latency}),")
     assert energy == pytest.approx(expected_energy)
     assert latency == pytest.approx(expected_latency)
```

### Comparing `zigzag_dse-3.1.0/tests/main/test_without_unused_memory/test_tpu_like.py` & `zigzag_dse-3.1.1/tests/main/test_origin/test_ascend_like.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 import pytest
 
-from zigzag.api import get_hardware_performance_zigzag_without_unused_memory
+from zigzag.api import get_hardware_performance_zigzag
 
 workloads = (
-    "zigzag/inputs/examples/workload/alexnet.onnx",
-    "zigzag/inputs/examples/workload/mobilenetv2.onnx",
-    "zigzag/inputs/examples/workload/resnet18.onnx",
-    "zigzag.inputs.examples.workload.resnet18",
+    "inputs/workload/alexnet.onnx",
+    "inputs/workload/mobilenetv2.onnx",
+    "inputs/workload/resnet18.onnx",
+    "inputs/workload/resnet18.yaml",
 )
 
 # Expected energy and latency for each workload defined above
 ens_lats = {
-    "zigzag/inputs/examples/workload/alexnet.onnx": (5475639384.492001, 8979956),
-    "zigzag/inputs/examples/workload/mobilenetv2.onnx": (952688145.0069999, 21873214),
-    "zigzag/inputs/examples/workload/resnet18.onnx": (1659252422.016, 4000289),
-    "zigzag.inputs.examples.workload.resnet18": (1982830786.5119998, 4509235),
+    "inputs/workload/alexnet.onnx": (5738188827.200001, 8696068.0),
+    "inputs/workload/mobilenetv2.onnx": (1913154775.600001, 7359658.0),
+    "inputs/workload/resnet18.onnx": (1860963861.6800003, 3698589.0),
+    "inputs/workload/resnet18.yaml": (2411783423.28, 4779709.0),
 }
 
 
 @pytest.fixture
 def mapping():
-    return "zigzag.inputs.examples.mapping.tpu_like"
+    return "inputs/mapping/ascend_like.yaml"
 
 
 @pytest.fixture
 def accelerator():
-    return "zigzag.inputs.examples.hardware.TPU_like"
+    return "inputs/hardware/ascend_like.yaml"
 
 
 @pytest.mark.parametrize("workload", workloads)
 def test_api(workload, accelerator, mapping):
-    (energy, latency, cmes) = get_hardware_performance_zigzag_without_unused_memory(
-        workload, accelerator, mapping
-    )
+    (energy, latency, cmes) = get_hardware_performance_zigzag(workload, accelerator, mapping)
     (expected_energy, expected_latency) = ens_lats[workload]
+    print(f"'{workload}': ({energy}, {latency}),")
     assert energy == pytest.approx(expected_energy)
     assert latency == pytest.approx(expected_latency)
```

### Comparing `zigzag_dse-3.1.0/zigzag/__main__.py` & `zigzag_dse-3.1.1/lab2/solutions/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,86 @@
-from zigzag.classes.stages import *
+import os
+import sys
 import argparse
+import re
 
-def main():
-    # Get the onnx model, the mapping and accelerator arguments
-    parser = argparse.ArgumentParser(description="Setup zigzag inputs")
-    parser.add_argument('--model', metavar='path', required=True, help='path to onnx model, e.g. inputs/examples/my_onnx_model.onnx')
-    parser.add_argument('--mapping', metavar='path', required=True, help='path to mapping file, e.g., inputs.examples.my_mapping')
-    parser.add_argument('--accelerator', metavar='path', required=True, help='module path to the accelerator, e.g. inputs.examples.accelerator1')
-    args = parser.parse_args()
-
-    # Initialize the logger
-    import logging as _logging
-    _logging_level = _logging.INFO
-    # _logging_format = '%(asctime)s - %(name)s.%(funcName)s +%(lineno)s - %(levelname)s - %(message)s'
-    _logging_format = '%(asctime)s - %(funcName)s +%(lineno)s - %(levelname)s - %(message)s'
-    _logging.basicConfig(level=_logging_level,
-                        format=_logging_format)
-
-    # Initialize the MainStage which will start execution.
-    # The first argument of this init is the list of stages that will be executed in sequence.
-    # The second argument of this init are the arguments required for these different stages.
-    mainstage = MainStage([  # Initializes the MainStage as entry point
+sys.path.insert(0, os.getcwd())
+from zigzag.stages.CostModelStage import CostModelStage
+from zigzag.stages.MainStage import MainStage
+from zigzag.stages.SpatialMappingGeneratorStage import SpatialMappingGeneratorStage
+from zigzag.stages.WorkloadStage import WorkloadStage
+from zigzag.stages.ONNXModelParserStage import ONNXModelParserStage
+from zigzag.stages.AcceleratorParserStage import AcceleratorParserStage
+from zigzag.stages.LomaStage import LomaStage
+from zigzag.stages.save_stages import CompleteSaveStage
+from zigzag.stages.reduce_stages import MinimalLatencyStage
+
+
+from zigzag.visualization.results.plot_cme import (
+    bar_plot_cost_model_evaluations_breakdown,
+)
+
+# Get the onnx model, the mapping and accelerator arguments
+parser = argparse.ArgumentParser(description="Setup zigzag inputs")
+parser.add_argument(
+    "--model",
+    metavar="path",
+    required=True,
+    help="path to onnx model, e.g. inputs/examples/my_onnx_model.onnx",
+)
+parser.add_argument(
+    "--mapping",
+    metavar="path",
+    required=True,
+    help="path to mapping file, e.g., inputs.examples.my_mapping",
+)
+parser.add_argument(
+    "--accelerator",
+    metavar="path",
+    required=True,
+    help="module path to the accelerator, e.g. inputs.examples.accelerator1",
+)
+args = parser.parse_args()
+
+# Initialize the logger
+import logging as _logging
+
+_logging_level = _logging.INFO
+# _logging_format = "%(asctime)s - %(funcName)s +%(lineno)s - %(levelname)s - %(message)s"
+_logging_format = "%(asctime)s - %(levelname)s - %(message)s"
+_logging.basicConfig(level=_logging_level, format=_logging_format)
+
+hw_name = args.accelerator.split(".")[-1]
+wl_name = re.split(r"/|\.", args.model)[-1]
+if wl_name == "onnx":
+    wl_name = re.split(r"/|\.", args.model)[-2]
+experiment_id = f"{hw_name}-{wl_name}"
+
+# Initialize the MainStage which will start execution.
+# The first argument of this init is the list of stages that will be executed in sequence.
+# The second argument of this init are the arguments required for these different stages.
+mainstage = MainStage(
+    [  # Initializes the MainStage as entry point
         ONNXModelParserStage,  # Parses the ONNX Model into the workload
         AcceleratorParserStage,  # Parses the accelerator
-        SimpleSaveStage,  # Saves all received CMEs information to a json
+        CompleteSaveStage,  # Saves all received CMEs information to a json
         WorkloadStage,  # Iterates through the different layers in the workload
-        SpatialMappingConversionStage,  # Generates multiple spatial mappings (SM)
+        SpatialMappingGeneratorStage,  # Generates multiple spatial mappings (SM)
         MinimalLatencyStage,  # Reduces all CMEs, returning minimal latency one
-        LomaStage,  # Generates multiple temporal mappings (TM)
-        CostModelStage  # Evaluates generated SM and TM through cost model
+        LomaStage,  # Converts defined temporal_ordering to temporal mapping
+        CostModelStage,  # Evaluates generated SM and TM through cost model
     ],
-        accelerator_path=args.accelerator,  # required by AcceleratorParserStage
-        onnx_model_path=args.model,  # required by ONNXModelParserStage
-        mapping_path=args.mapping,  # required by ONNXModelParserStage
-        dump_filename_pattern="outputs/{datetime}.json",  # output file save pattern
-        loma_lpf_limit=6,  # required by LomaStage
-        loma_show_progress_bar=True,  # shows a progress bar while iterating over temporal mappings
-    )
-
-    # Launch the MainStage
-    mainstage.run()
+    accelerator=args.accelerator,  # required by AcceleratorParserStage
+    workload=args.model,  # required by ONNXModelParserStage
+    mapping=args.mapping,  # required by ONNXModelParserStage
+    dump_filename_pattern=f"lab2/outputs/{experiment_id}-?.json",  # output file save pattern, ? will be replaced
+    loma_lpf_limit=6,  # required by LomaStage
+    loma_show_progress_bar=True,  # shows a progress bar while iterating over temporal mappings
+    nb_mappings_generated=100,
+)
 
-if __name__ == "__main__":
-    main()
+# Launch the MainStage
+answers = mainstage.run()
+# Plot the energy and latency breakdown of our cost model evaluation
+cme = answers[0][0]
+save_path = "lab2/outputs/breakdown.png"
+bar_plot_cost_model_evaluations_breakdown([cme], save_path=save_path, xtick_rotation=0)
```

### Comparing `zigzag_dse-3.1.0/zigzag/api.py` & `zigzag_dse-3.1.1/zigzag/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,61 @@
-from zigzag.classes.stages import *
-from zigzag.classes.cost_model.cost_model import CostModelEvaluation
-from typing import Type
-import re
 from onnx import ModelProto
+import re
+from datetime import datetime
+from typing import Any
+
+from zigzag.stages.CostModelStage import CostModelStage
+from zigzag.stages.MainStage import MainStage
+from zigzag.stages.ONNXModelParserStage import ONNXModelParserStage
+from zigzag.stages.PEArrayScalingStage import PEArrayScalingStage
+from zigzag.stages.SpatialMappingGeneratorStage import SpatialMappingGeneratorStage
+from zigzag.stages.WorkloadStage import WorkloadStage
+from zigzag.stages.WorkloadParserStage import WorkloadParserStage
+from zigzag.stages.AcceleratorParserStage import AcceleratorParserStage
+from zigzag.stages.reduce_stages import MinimalEDPStage, MinimalEnergyStage, MinimalLatencyStage, SumStage
+from zigzag.stages.save_stages import CompleteSaveStage, PickleSaveStage, SimpleSaveStage
+from zigzag.stages.LomaStage import LomaStage
+from zigzag.cost_model.cost_model import CostModelEvaluationABC
+from zigzag.stages.SearchUnusedMemoryStage import SearchUnusedMemoryStage
+from zigzag.stages.RemoveUnusedMemoryStage import RemoveUnusedMemoryStage
+
 
 def get_hardware_performance_zigzag(
-    workload,
-    accelerator,
-    mapping,
-    opt="latency",
-    dump_filename_pattern="outputs/{datetime}.json",
-    pickle_filename="outputs/list_of_cmes.pickle",
+    workload: str | dict[int, dict[str, Any]] | ModelProto,
+    accelerator: str,
+    mapping: str | dict[str, dict[str, Any]],
+    opt: str = "latency",
+    dump_filename_pattern: str = f"outputs/{datetime.now()}.json",
+    pickle_filename: str = "outputs/list_of_cmes.pickle",
     lpf_limit: int = 6,
-    cost_model_class: Type = CostModelEvaluation,
-):
+) -> tuple[float, float, list[tuple[CostModelEvaluationABC, Any]]]:
+    """
+    # TODO the API should be better documented
+    """
     # Initialize the logger
     import logging as _logging
 
     _logging_level = _logging.INFO
-    _logging_format = (
-        "%(asctime)s - %(funcName)s +%(lineno)s - %(levelname)s - %(message)s"
-    )
+    _logging_format = "%(asctime)s - %(funcName)s +%(lineno)s - %(levelname)s - %(message)s"
     _logging.basicConfig(level=_logging_level, format=_logging_format)
 
-    # Sanity check on the optimization criterion
-    if opt == "energy":
-        opt_stage = MinimalEnergyStage
-    elif opt == "latency":
-        opt_stage = MinimalLatencyStage
-    elif opt == "EDP":
-        opt_stage = MinimalEDPStage
-    else:
-        raise NotImplementedError(
-            "Optimization criterion 'opt' should be either 'energy' or 'latency' or 'EDP'."
-        )
+    match opt:
+        case "energy":
+            opt_stage = MinimalEnergyStage
+        case "latency":
+            opt_stage = MinimalLatencyStage
+        case "EDP":
+            opt_stage = MinimalEDPStage
+        case _:
+            raise NotImplementedError("Optimization criterion 'opt' should be either 'energy' or 'latency' or 'EDP'.")
 
     # Check workload format and based on it select the correct workload parser stage
-    try:
-        if isinstance(workload, ModelProto) or workload.split(".")[-1] == "onnx":
-            workload_parser_stage = ONNXModelParserStage
-        else:
-            workload_parser_stage = WorkloadParserStage
-    except:
+    if isinstance(workload, ModelProto) or (isinstance(workload, str) and workload.split(".")[-1] == "onnx"):
+        workload_parser_stage = ONNXModelParserStage
+    else:
         workload_parser_stage = WorkloadParserStage
 
     mainstage = MainStage(
         [  # Initialize the MainStage as entry point
             workload_parser_stage,  # Parse the ONNX Model into the workload
             AcceleratorParserStage,  # Parse the accelerator module/passthrough given accelerator
             SimpleSaveStage,  # Save the summed CME energy and latency to a json
@@ -53,74 +63,69 @@
             SumStage,  # Sum up the received best CME across all layers of the workload
             WorkloadStage,  # Iterate through the different layers in the workload
             CompleteSaveStage,  # Save each processed layer to a json
             opt_stage,  # Reduce all CMEs, returning minimal energy/latency one
             SpatialMappingGeneratorStage,  # Generate multiple spatial mappings (SM)
             opt_stage,  # Reduce all CMEs, returning minimal energy/latency one
             LomaStage,  # Generate multiple temporal mappings (TM)
-            # TemporalOrderingConversionStage,  # Based on the fixed temporal mapping order, generate one temporal mapping (TM)
+            # TemporalOrderingConversionStage,  # Based on the fixed temporal mapping order, generate one temporal
+            # mapping (TM)
             CostModelStage,  # Evaluate generated SM and TM through cost model
         ],
         accelerator=accelerator,  # required by AcceleratorParserStage
         workload=workload,  # required by workload_parser_stage
         mapping=mapping,  # required by workload_parser_stage
         dump_filename_pattern=dump_filename_pattern,  # output file save pattern
         pickle_filename=pickle_filename,  # filename for pickled list of cmes
         loma_lpf_limit=lpf_limit,  # required by LomaStage
         loma_show_progress_bar=True,
-        # If we need access the same input data multiple times from the innermost memory level and the data size is smaller than the memory read bw,
-        # take into account only one-time access cost (assume the data can stay at the output pins of the memory as long as it is needed).
+        enable_weight_diagonal_mapping=False,
+        # If we need access the same input data multiple times from the innermost memory level and the data size is
+        # smaller than the memory read bw,
+        # take into account only one-time access cost (assume the data can stay at the output pins of the memory as
+        # long as it is needed).
         # By default, if the parameter is not defined, it will be set as False internally.
         access_same_data_considered_as_no_access=True,
-        cost_model_class=cost_model_class,
     )
 
     # Launch the MainStage
-    answers = mainstage.run()
-    # Get CME from answer
-    cmes = answers
+    cmes = mainstage.run()
 
     return cmes[0][0].energy_total, cmes[0][0].latency_total2, cmes
 
+
 def get_hardware_performance_zigzag_imc(
-    workload,
-    accelerator,
-    mapping,
-    opt="latency",
-    dump_filename_pattern="outputs/layer_?.json",
-    pickle_filename="outputs/list_of_cmes.pickle",
-):
+    workload: str | dict[int, dict[str, Any]] | ModelProto,
+    accelerator: str,
+    mapping: str | dict[str, dict[str, Any]],
+    opt: str = "latency",
+    dump_filename_pattern: str = "outputs/layer_?.json",
+    pickle_filename: str = "outputs/list_of_cmes.pickle",
+) -> tuple[float, float, list[tuple[CostModelEvaluationABC, Any]]]:
     # Initialize the logger
     import logging as _logging
 
     _logging_level = _logging.INFO
-    _logging_format = ( 
-        "%(asctime)s - %(funcName)s +%(lineno)s - %(levelname)s - %(message)s"
-    )   
+    _logging_format = "%(asctime)s - %(funcName)s +%(lineno)s - %(levelname)s - %(message)s"
     _logging.basicConfig(level=_logging_level, format=_logging_format)
 
-    # Sanity check on the optimization criterion
-    if opt == "energy":
-        opt_stage = MinimalEnergyStage
-    elif opt == "latency":
-        opt_stage = MinimalLatencyStage
-    elif opt == "EDP":
-        opt_stage = MinimalEDPStage
-    else:
-        raise NotImplementedError(
-            "Optimization criterion 'opt' should be either 'energy' or 'latency' or 'EDP'."
-        )   
+    match opt:
+        case "energy":
+            opt_stage = MinimalEnergyStage
+        case "latency":
+            opt_stage = MinimalLatencyStage
+        case "EDP":
+            opt_stage = MinimalEDPStage
+        case _:
+            raise NotImplementedError("Optimization criterion 'opt' should be either 'energy' or 'latency' or 'EDP'.")
 
     # Check workload format and based on it select the correct workload parser stage
-    try:
-        if workload.split(".")[-1] == "onnx":
-            workload_parser_stage = ONNXModelParserStage
-        else:
-            workload_parser_stage = WorkloadParserStage
-    except:
+    if isinstance(workload, ModelProto) or (isinstance(workload, str) and workload.split(".")[-1] == "onnx"):
+        workload_parser_stage = ONNXModelParserStage
+    else:
         workload_parser_stage = WorkloadParserStage
 
     mainstage = MainStage(
         [  # Initialize the MainStage as entry point
             workload_parser_stage,  # Parse the ONNX Model into the workload
             AcceleratorParserStage,  # Parse the accelerator module/passthrough given accelerator
             SimpleSaveStage,  # Save the summed CME energy and latency to a json
@@ -130,77 +135,78 @@
             WorkloadStage,  # Iterate through the different layers in the workload
             RemoveUnusedMemoryStage,  # Remove unnecessary memory instances
             CompleteSaveStage,  # Save each processed layer to a json
             opt_stage,  # Reduce all CMEs, returning minimal energy/latency one
             SpatialMappingGeneratorStage,  # Generate multiple spatial mappings (SM)
             opt_stage,  # Reduce all CMEs, returning minimal energy/latency one
             LomaStage,  # Generate multiple temporal mappings (TM)
-            # TemporalOrderingConversionStage,  # Based on the fixed temporal mapping order, generate one temporal mapping (TM)
+            # TemporalOrderingConversionStage,  # Based on the fixed temporal mapping order, generate one temporal
+            # mapping (TM)
             CostModelStage,  # Evaluate generated SM and TM through cost model
         ],
         accelerator=accelerator,  # required by AcceleratorParserStage
         workload=workload,  # required by workload_parser_stage
         mapping=mapping,  # required by workload_parser_stage
         dump_filename_pattern=dump_filename_pattern,  # output file save pattern
         pickle_filename=pickle_filename,  # filename for pickled list of cmes
         loma_lpf_limit=6,  # required by LomaStage
         enable_mix_spatial_mapping_generation=True,  # enable auto-generation of mix spatial mapping
-        maximize_hardware_utilization=True, # only evaluate spatial mapping with top2 utilization (fast simulation)
+        maximize_hardware_utilization=True,  # only evaluate spatial mapping with top2 utilization (fast simulation)
         enable_weight_diagonal_mapping=True,  # required by SpatialMappingGeneratorStage
         loma_show_progress_bar=True,
-        # If we need access the same input data multiple times from the innermost memory level and the data size is smaller than the memory read bw,
-        # take into account only one-time access cost (assume the data can stay at the output pins of the memory as long as it is needed).
+        # If we need access the same input data multiple times from the innermost memory level and the data size is
+        # smaller than the memory read bw,
+        # take into account only one-time access cost (assume the data can stay at the output pins of the memory as
+        # long as it is needed).
         # By default, if the parameter is not defined, it will be set as False internally.
         access_same_data_considered_as_no_access=True,
     )
 
     # Launch the MainStage
-    answers = mainstage.run()
-    # Get CME from answer
-    cmes = answers
+    cmes = mainstage.run()
+
+    return (
+        cmes[0][0].energy_total,
+        cmes[0][0].latency_total2,
+        cmes[0][0].tclk,
+        cmes[0][0].area_total,
+        cmes,
+    )
 
-    return cmes[0][0].energy_total, cmes[0][0].latency_total2, cmes[0][0].tclk, cmes[0][0].area_total, cmes
 
 def get_hardware_performance_zigzag_pe_array_scaling(
-    workload,
-    accelerator,
-    mapping,
+    workload: str | dict[int, dict[str, Any]] | ModelProto,
+    accelerator: str,
+    mapping: str | dict[str, dict[str, Any]],
     pe_array_scaling,
-    opt="latency",
-    dump_filename_pattern="outputs/{datetime}.json",
-    pickle_filename="outputs/list_of_cmes.pickle",
-):
+    opt: str = "latency",
+    dump_filename_pattern: str = "outputs/{datetime}.json",
+    pickle_filename: str = "outputs/list_of_cmes.pickle",
+) -> tuple[float, float, list[tuple[CostModelEvaluationABC, Any]]]:
     # Initialize the logger
     import logging as _logging
 
     _logging_level = _logging.INFO
-    _logging_format = (
-        "%(asctime)s - %(funcName)s +%(lineno)s - %(levelname)s - %(message)s"
-    )
+    _logging_format = "%(asctime)s - %(funcName)s +%(lineno)s - %(levelname)s - %(message)s"
     _logging.basicConfig(level=_logging_level, format=_logging_format)
 
-    # Sanity check on the optimization criterion
-    if opt == "energy":
-        opt_stage = MinimalEnergyStage
-    elif opt == "latency":
-        opt_stage = MinimalLatencyStage
-    elif opt == "EDP":
-        opt_stage = MinimalEDPStage
-    else:
-        raise NotImplementedError(
-            "Optimization criterion 'opt' should be either 'energy' or 'latency' or 'EDP'."
-        )
+    match opt:
+        case "energy":
+            opt_stage = MinimalEnergyStage
+        case "latency":
+            opt_stage = MinimalLatencyStage
+        case "EDP":
+            opt_stage = MinimalEDPStage
+        case _:
+            raise NotImplementedError("Optimization criterion 'opt' should be either 'energy' or 'latency' or 'EDP'.")
 
     # Check workload format and based on it select the correct workload parser stage
-    try:
-        if workload.split(".")[-1] == "onnx":
-            workload_parser_stage = ONNXModelParserStage
-        else:
-            workload_parser_stage = WorkloadParserStage
-    except:
+    if isinstance(workload, ModelProto) or (isinstance(workload, str) and workload.split(".")[-1] == "onnx"):
+        workload_parser_stage = ONNXModelParserStage
+    else:
         workload_parser_stage = WorkloadParserStage
 
     mainstage = MainStage(
         [  # Initialize the MainStage as entry point
             workload_parser_stage,  # Parse the ONNX Model into the workload
             AcceleratorParserStage,  # Parse the accelerator module/passthrough given accelerator
             PEArrayScalingStage,  # Scale the PE array of the given accelerator
@@ -209,75 +215,71 @@
             SumStage,  # Sum up the received best CME across all layers of the workload
             WorkloadStage,  # Iterate through the different layers in the workload
             CompleteSaveStage,  # Save each processed layer to a json
             opt_stage,  # Reduce all CMEs, returning minimal energy/latency one
             SpatialMappingGeneratorStage,  # Generate multiple spatial mappings (SM)
             opt_stage,  # Reduce all CMEs, returning minimal energy/latency one
             LomaStage,  # Generate multiple temporal mappings (TM)
-            # TemporalOrderingConversionStage,  # Based on the fixed temporal mapping order, generate one temporal mapping (TM)
+            # TemporalOrderingConversionStage,  # Based on the fixed temporal mapping order, generate one temporal
+            # mapping (TM)
             CostModelStage,  # Evaluate generated SM and TM through cost model
         ],
         accelerator=accelerator,  # required by AcceleratorParserStage
         workload=workload,  # required by workload_parser_stage
         mapping=mapping,  # required by workload_parser_stage
         dump_filename_pattern=dump_filename_pattern,  # output file save pattern
         pickle_filename=pickle_filename,  # filename for pickled list of cmes
         loma_lpf_limit=6,  # required by LomaStage
         loma_show_progress_bar=True,
-        # If we need access the same input data multiple times from the innermost memory level and the data size is smaller than the memory read bw,
-        # take into account only one-time access cost (assume the data can stay at the output pins of the memory as long as it is needed).
+        # If we need access the same input data multiple times from the innermost memory level and the data size is
+        # smaller than the memory read bw,
+        # take into account only one-time access cost (assume the data can stay at the output pins of the memory as long
+        # as it is needed).
         # By default, if the parameter is not defined, it will be set as False internally.
         access_same_data_considered_as_no_access=True,
         pe_array_scaling=pe_array_scaling,
     )
 
     # Launch the MainStage
     answers = mainstage.run()
     # Get CME from answer
     cmes = answers
 
     return cmes[0][0].energy_total, cmes[0][0].latency_total2, cmes
 
 
 def get_hardware_performance_zigzag_without_unused_memory(
-    workload,
-    accelerator,
-    mapping,
-    opt="latency",
-    dump_filename_pattern="outputs/{datetime}.json",
-    pickle_filename="outputs/list_of_cmes.pickle",
-):
+    workload: str | dict[int, dict[str, Any]] | ModelProto,
+    accelerator: str,
+    mapping: str | dict[str, dict[str, Any]],
+    opt: str = "latency",
+    dump_filename_pattern: str = "outputs/{datetime}.json",
+    pickle_filename: str = "outputs/list_of_cmes.pickle",
+) -> tuple[float, float, list[tuple[CostModelEvaluationABC, Any]]]:
     # Initialize the logger
     import logging as _logging
 
     _logging_level = _logging.INFO
-    _logging_format = (
-        "%(asctime)s - %(funcName)s +%(lineno)s - %(levelname)s - %(message)s"
-    )
+    _logging_format = "%(asctime)s - %(funcName)s +%(lineno)s - %(levelname)s - %(message)s"
     _logging.basicConfig(level=_logging_level, format=_logging_format)
 
-    # Sanity check on the optimization criterion
-    if opt == "energy":
-        opt_stage = MinimalEnergyStage
-    elif opt == "latency":
-        opt_stage = MinimalLatencyStage
-    elif opt == "EDP":
-        opt_stage = MinimalEDPStage
-    else:
-        raise NotImplementedError(
-            "Optimization criterion 'opt' should be either 'energy' or 'latency' or 'EDP'."
-        )
+    match opt:
+        case "energy":
+            opt_stage = MinimalEnergyStage
+        case "latency":
+            opt_stage = MinimalLatencyStage
+        case "EDP":
+            opt_stage = MinimalEDPStage
+        case _:
+            raise NotImplementedError("Optimization criterion 'opt' should be either 'energy' or 'latency' or 'EDP'.")
 
     # Check workload format and based on it select the correct workload parser stage
-    try:
-        if workload.split(".")[-1] == "onnx":
-            workload_parser_stage = ONNXModelParserStage
-        else:
-            workload_parser_stage = WorkloadParserStage
-    except:
+    if isinstance(workload, ModelProto) or (isinstance(workload, str) and workload.split(".")[-1] == "onnx"):
+        workload_parser_stage = ONNXModelParserStage
+    else:
         workload_parser_stage = WorkloadParserStage
 
     mainstage = MainStage(
         [  # Initialize the MainStage as entry point
             workload_parser_stage,  # Parse the ONNX Model into the workload
             AcceleratorParserStage,  # Parse the accelerator module/passthrough given accelerator
             SimpleSaveStage,  # Save the summed CME energy and latency to a json
@@ -287,73 +289,70 @@
             WorkloadStage,  # Iterate through the different layers in the workload
             RemoveUnusedMemoryStage,  # Remove unused memory instance
             CompleteSaveStage,  # Save each processed layer to a json
             opt_stage,  # Reduce all CMEs, returning minimal energy/latency one
             SpatialMappingGeneratorStage,  # Generate multiple spatial mappings (SM)
             opt_stage,  # Reduce all CMEs, returning minimal energy/latency one
             LomaStage,  # Generate multiple temporal mappings (TM)
-            # TemporalOrderingConversionStage,  # Based on the fixed temporal mapping order, generate one temporal mapping (TM)
+            # TemporalOrderingConversionStage,  # Based on the fixed temporal mapping order, generate one temporal
+            # mapping (TM)
             CostModelStage,  # Evaluate generated SM and TM through cost model
         ],
         accelerator=accelerator,  # required by AcceleratorParserStage
         workload=workload,  # required by workload_parser_stage
         mapping=mapping,  # required by workload_parser_stage
         dump_filename_pattern=dump_filename_pattern,  # output file save pattern
         pickle_filename=pickle_filename,  # filename for pickled list of cmes
         loma_lpf_limit=6,  # required by LomaStage
         loma_show_progress_bar=True,
-        # If we need access the same input data multiple times from the innermost memory level and the data size is smaller than the memory read bw,
-        # take into account only one-time access cost (assume the data can stay at the output pins of the memory as long as it is needed).
+        # If we need access the same input data multiple times from the innermost memory level and the data size is
+        # smaller than the memory read bw,
+        # take into account only one-time access cost (assume the data can stay at the output pins of the memory as long
+        # as it is needed).
         # By default, if the parameter is not defined, it will be set as False internally.
         access_same_data_considered_as_no_access=True,
     )
 
     # Launch the MainStage
     answers = mainstage.run()
     # Get CME from answer
     cmes = answers
 
     return cmes[0][0].energy_total, cmes[0][0].latency_total2, cmes
 
+
 def get_hardware_performance_zigzag_with_mix_spatial_mapping(
-    workload,
-    accelerator,
-    mapping,
-    opt="latency",
-    dump_filename_pattern="outputs/{datetime}.json",
-    pickle_filename="outputs/list_of_cmes.pickle",
-):
+    workload: str | dict[int, dict[str, Any]] | ModelProto,
+    accelerator: str,
+    mapping: str | dict[str, dict[str, Any]],
+    opt: str = "latency",
+    dump_filename_pattern: str = "outputs/{datetime}.json",
+    pickle_filename: str = "outputs/list_of_cmes.pickle",
+) -> tuple[float, float, list[tuple[CostModelEvaluationABC, Any]]]:
     # Initialize the logger
     import logging as _logging
 
     _logging_level = _logging.INFO
-    _logging_format = (
-        "%(asctime)s - %(funcName)s +%(lineno)s - %(levelname)s - %(message)s"
-    )
+    _logging_format = "%(asctime)s - %(funcName)s +%(lineno)s - %(levelname)s - %(message)s"
     _logging.basicConfig(level=_logging_level, format=_logging_format)
 
-    # Sanity check on the optimization criterion
-    if opt == "energy":
-        opt_stage = MinimalEnergyStage
-    elif opt == "latency":
-        opt_stage = MinimalLatencyStage
-    elif opt == "EDP":
-        opt_stage = MinimalEDPStage
-    else:
-        raise NotImplementedError(
-            "Optimization criterion 'opt' should be either 'energy' or 'latency' or 'EDP'."
-        )
+    match opt:
+        case "energy":
+            opt_stage = MinimalEnergyStage
+        case "latency":
+            opt_stage = MinimalLatencyStage
+        case "EDP":
+            opt_stage = MinimalEDPStage
+        case _:
+            raise NotImplementedError("Optimization criterion 'opt' should be either 'energy' or 'latency' or 'EDP'.")
 
     # Check workload format and based on it select the correct workload parser stage
-    try:
-        if workload.split(".")[-1] == "onnx":
-            workload_parser_stage = ONNXModelParserStage
-        else:
-            workload_parser_stage = WorkloadParserStage
-    except:
+    if isinstance(workload, ModelProto) or (isinstance(workload, str) and workload.split(".")[-1] == "onnx"):
+        workload_parser_stage = ONNXModelParserStage
+    else:
         workload_parser_stage = WorkloadParserStage
 
     mainstage = MainStage(
         [  # Initialize the MainStage as entry point
             workload_parser_stage,  # Parse the ONNX Model into the workload
             AcceleratorParserStage,  # Parse the accelerator module/passthrough given accelerator
             SimpleSaveStage,  # Save the summed CME energy and latency to a json
@@ -363,39 +362,42 @@
             WorkloadStage,  # Iterate through the different layers in the workload
             RemoveUnusedMemoryStage,  # Remove unused memory instance
             CompleteSaveStage,  # Save each processed layer to a json
             opt_stage,  # Reduce all CMEs, returning minimal energy/latency one
             SpatialMappingGeneratorStage,  # Generate multiple spatial mappings (SM)
             opt_stage,  # Reduce all CMEs, returning minimal energy/latency one
             LomaStage,  # Generate multiple temporal mappings (TM)
-            # TemporalOrderingConversionStage,  # Based on the fixed temporal mapping order, generate one temporal mapping (TM)
+            # TemporalOrderingConversionStage,  # Based on the fixed temporal mapping order, generate one temporal
+            # mapping (TM)
             CostModelStage,  # Evaluate generated SM and TM through cost model
         ],
         accelerator=accelerator,  # required by AcceleratorParserStage
         workload=workload,  # required by workload_parser_stage
         mapping=mapping,  # required by workload_parser_stage
         dump_filename_pattern=dump_filename_pattern,  # output file save pattern
         pickle_filename=pickle_filename,  # filename for pickled list of cmes
         loma_lpf_limit=6,  # required by LomaStage
         loma_show_progress_bar=True,
-        # If we need access the same input data multiple times from the innermost memory level and the data size is smaller than the memory read bw,
-        # take into account only one-time access cost (assume the data can stay at the output pins of the memory as long as it is needed).
+        # If we need access the same input data multiple times from the innermost memory level and the data size is
+        # smaller than the memory read bw,
+        # take into account only one-time access cost (assume the data can stay at the output pins of the memory as long
+        # as it is needed).
         # By default, if the parameter is not defined, it will be set as False internally.
         access_same_data_considered_as_no_access=True,
         enable_mix_spatial_mapping_generation=True,  # enable auto-generation of mix spatial mapping
-        maximize_hardware_utilization=True, # only evaluate spatial mapping with highest hardware utilization (fast simulation speed)
     )
 
     # Launch the MainStage
     answers = mainstage.run()
     # Get CME from answer
     cmes = answers
 
     return cmes[0][0].energy_total, cmes[0][0].latency_total2, cmes
 
+
 if __name__ == "__main__":
     workload = "zigzag/inputs/examples/workload/mobilenetv2.onnx"
     # workload = 'inputs.examples.workload.resnet18'
     accelerator = "zigzag.inputs.examples.hardware.TPU_like"
     mapping = "zigzag.inputs.examples.mapping.tpu_like"
 
     hw_name = accelerator.split(".")[-1]
@@ -410,14 +412,7 @@
         accelerator,
         mapping,
         pe_array_scaling=2,
         opt="EDP",
         dump_filename_pattern=f"outputs/{experiment_id}-layer_?.json",
         pickle_filename=f"outputs/{pkl_name}.pickle",
     )
-    # print(f'Answer = {answer}')
-
-    # import pickle
-    # path = f"outputs/{pkl_name}.pickle"
-    # with open(path, 'rb') as f:
-    #     data = pickle.load(f)
-    # f.close()
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti_config_creator.py` & `zigzag_dse-3.1.1/zigzag/hardware/architecture/get_cacti_cost.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,393 +1,630 @@
 import os
+import platform
 
 
 class CactiConfig:
 
     def __init__(self):
         # content = f.readlines()
-        self.baseline_config = ['# power gating\n',
-                                '-Array Power Gating - "false"\n',
-                                '-WL Power Gating - "false"\n',
-                                '-CL Power Gating - "false"\n',
-                                '-Bitline floating - "false"\n',
-                                '-Interconnect Power Gating - "false"\n',
-                                '-Power Gating Performance Loss 0.01\n',
-                                '\n',
-                                '# following three parameters are meaningful only for main memories\n',
-                                '-page size (bits) 8192 \n',
-                                '-burst length 8\n',
-                                '-internal prefetch width 8\n',
-                                '\n',
-                                '# following parameter can have one of five values -- (itrs-hp, itrs-lstp, itrs-lop, lp-dram, comm-dram)\n',
-                                '-Data array cell type - "itrs-hp"\n',
-                                '//-Data array cell type - "itrs-lstp"\n',
-                                '//-Data array cell type - "itrs-lop"\n',
-                                '\n',
-                                '# following parameter can have one of three values -- (itrs-hp, itrs-lstp, itrs-lop)\n',
-                                '-Data array peripheral type - "itrs-hp"\n',
-                                '//-Data array peripheral type - "itrs-lstp"\n',
-                                '//-Data array peripheral type - "itrs-lop"\n',
-                                '\n',
-                                '# following parameter can have one of five values -- (itrs-hp, itrs-lstp, itrs-lop, lp-dram, comm-dram)\n',
-                                '-Tag array cell type - "itrs-hp"\n',
-                                '//-Tag array cell type - "itrs-lstp"\n',
-                                '//-Tag array cell type - "itrs-lop"\n',
-                                '\n',
-                                '# following parameter can have one of three values -- (itrs-hp, itrs-lstp, itrs-lop)\n',
-                                '-Tag array peripheral type - "itrs-hp"\n',
-                                '//-Tag array peripheral type - "itrs-lstp"\n',
-                                '//-Tag array peripheral type - "itrs-lop\n',
-                                '\n',
-                                '\n',
-                                '// 300-400 in steps of 10\n',
-                                '-operating temperature (K) 360\n',
-                                '\n',
-                                '# to model special structure like branch target buffers, directory, etc. \n',
-                                '# change the tag size parameter\n',
-                                '# if you want cacti to calculate the tagbits, set the tag size to "default"\n',
-                                '-tag size (b) "default"\n',
-                                '//-tag size (b) 22\n',
-                                '\n',
-                                '# fast - data and tag access happen in parallel\n',
-                                '# sequential - data array is accessed after accessing the tag array\n',
-                                '# normal - data array lookup and tag access happen in parallel\n',
-                                '#          final data block is broadcasted in data array h-tree \n',
-                                '#          after getting the signal from the tag array\n',
-                                '//-access mode (normal, sequential, fast) - "fast"\n',
-                                '-access mode (normal, sequential, fast) - "normal"\n',
-                                '//-access mode (normal, sequential, fast) - "sequential"\n',
-                                '\n',
-                                '\n',
-                                '# DESIGN OBJECTIVE for UCA (or banks in NUCA)\n',
-                                '-design objective (weight delay, dynamic power, leakage power, cycle time, area) 0:0:0:100:0\n',
-                                '\n',
-                                '# Percentage deviation from the minimum value \n',
-                                '# Ex: A deviation value of 10:1000:1000:1000:1000 will try to find an organization\n',
-                                '# that compromises at most 10% delay. \n',
-                                '# NOTE: Try reasonable values for % deviation. Inconsistent deviation\n',
-                                '# percentage values will not produce any valid organizations. For example,\n',
-                                '# 0:0:100:100:100 will try to identify an organization that has both\n',
-                                '# least delay and dynamic power. Since such an organization is not possible, CACTI will\n',
-                                '# throw an error. Refer CACTI-6 Technical report for more details\n',
-                                '-deviate (delay, dynamic power, leakage power, cycle time, area) 20:100000:100000:100000:100000\n',
-                                '\n',
-                                '# Objective for NUCA\n',
-                                '-NUCAdesign objective (weight delay, dynamic power, leakage power, cycle time, area) 100:100:0:0:100\n',
-                                '-NUCAdeviate (delay, dynamic power, leakage power, cycle time, area) 10:10000:10000:10000:10000\n',
-                                '\n',
-                                '# Set optimize tag to ED or ED^2 to obtain a cache configuration optimized for\n',
-                                '# energy-delay or energy-delay sq. product\n',
-                                '# Note: Optimize tag will disable weight or deviate values mentioned above\n',
-                                '# Set it to NONE to let weight and deviate values determine the \n',
-                                '# appropriate cache configuration\n',
-                                '//-Optimize ED or ED^2 (ED, ED^2, NONE): "ED"\n',
-                                '-Optimize ED or ED^2 (ED, ED^2, NONE): "ED^2"\n',
-                                '//-Optimize ED or ED^2 (ED, ED^2, NONE): "NONE"\n',
-                                '\n',
-                                '-Cache model (NUCA, UCA)  - "UCA"\n',
-                                '//-Cache model (NUCA, UCA)  - "NUCA"\n',
-                                '\n',
-                                '# In order for CACTI to find the optimal NUCA bank value the following\n',
-                                '# variable should be assigned 0.\n',
-                                '-NUCA bank count 0\n',
-                                '\n',
-                                '# NOTE: for nuca network frequency is set to a default value of \n',
-                                '# 5GHz in time.c. CACTI automatically\n',
-                                '# calculates the maximum possible frequency and downgrades this value if necessary\n',
-                                '\n',
-                                '# By default CACTI considers both full-swing and low-swing \n',
-                                '# wires to find an optimal configuration. However, it is possible to \n',
-                                '# restrict the search space by changing the signaling from "default" to \n',
-                                '# "fullswing" or "lowswing" type.\n',
-                                '-Wire signaling (fullswing, lowswing, default) - "Global_30"\n',
-                                '//-Wire signaling (fullswing, lowswing, default) - "default"\n',
-                                '//-Wire signaling (fullswing, lowswing, default) - "lowswing"\n',
-                                '\n',
-                                '//-Wire inside mat - "global"\n',
-                                '-Wire inside mat - "semi-global"\n',
-                                '//-Wire outside mat - "global"\n',
-                                '-Wire outside mat - "semi-global"\n',
-                                '\n',
-                                '-Interconnect projection - "conservative"\n',
-                                '//-Interconnect projection - "aggressive"\n',
-                                '\n',
-                                '# Contention in network (which is a function of core count and cache level) is one of\n',
-                                '# the critical factor used for deciding the optimal bank count value\n',
-                                '# core count can be 4, 8, or 16\n',
-                                '//-Core count 4\n',
-                                '-Core count 8\n',
-                                '//-Core count 16\n',
-                                '-Cache level (L2/L3) - "L3"\n',
-                                '\n',
-                                '-Add ECC - "true"\n',
-                                '\n',
-                                '//-Print level (DETAILED, CONCISE) - "CONCISE"\n',
-                                '-Print level (DETAILED, CONCISE) - "DETAILED"\n',
-                                '\n',
-                                '# for debugging\n',
-                                '-Print input parameters - "true"\n',
-                                '//-Print input parameters - "false"\n',
-                                '# force CACTI to model the cache with the \n',
-                                '# following Ndbl, Ndwl, Nspd, Ndsam,\n',
-                                '# and Ndcm values\n',
-                                '//-Force cache config - "true"\n',
-                                '-Force cache config - "false"\n',
-                                '-Ndwl 1\n',
-                                '-Ndbl 1\n',
-                                '-Nspd 0\n',
-                                '-Ndcm 1\n',
-                                '-Ndsam1 0\n',
-                                '-Ndsam2 0\n',
-                                '\n',
-                                '\n',
-                                '\n',
-                                '#### Default CONFIGURATION values for baseline external IO parameters to DRAM. More details can be found in the CACTI-IO technical report (), especially Chapters 2 and 3.\n',
-                                '\n',
-                                '# Memory Type (D3=DDR3, D4=DDR4, L=LPDDR2, W=WideIO, S=Serial). Additional memory types can be defined by the user in extio_technology.cc, along with their technology and configuration parameters.\n',
-                                '\n',
-                                '-dram_type "DDR3"\n',
-                                '//-dram_type "DDR4"\n',
-                                '//-dram_type "LPDDR2"\n',
-                                '//-dram_type "WideIO"\n',
-                                '//-dram_type "Serial"\n',
-                                '\n',
-                                '# Memory State (R=Read, W=Write, I=Idle  or S=Sleep) \n',
-                                '\n',
-                                '//-io state  "READ"\n',
-                                '-io state "WRITE"\n',
-                                '//-io state "IDLE"\n',
-                                '//-io state "SLEEP"\n',
-                                '\n',
-                                '#Address bus timing. To alleviate the timing on the command and address bus due to high loading (shared across all memories on the channel), the interface allows for multi-cycle timing options. \n',
-                                '\n',
-                                '//-addr_timing 0.5 //DDR\n',
-                                '-addr_timing 1.0 //SDR (half of DQ rate)\n',
-                                '//-addr_timing 2.0 //2T timing (One fourth of DQ rate)\n',
-                                '//-addr_timing 3.0 // 3T timing (One sixth of DQ rate)\n',
-                                '\n',
-                                '# Memory Density (Gbit per memory/DRAM die)\n',
-                                '\n',
-                                '-mem_density 4 Gb //Valid values 2^n Gb\n',
-                                '\n',
-                                '# IO frequency (MHz) (frequency of the external memory interface).\n',
-                                '\n',
-                                '-bus_freq 800 MHz //As of current memory standards (2013), valid range 0 to 1.5 GHz for DDR3, 0 to 533 MHz for LPDDR2, 0 - 800 MHz for WideIO and 0 - 3 GHz for Low-swing differential. However this can change, and the user is free to define valid ranges based on new memory types or extending beyond existing standards for existing dram types.\n',
-                                '\n',
-                                '# Duty Cycle (fraction of time in the Memory State defined above)\n',
-                                '\n',
-                                '-duty_cycle 1.0 //Valid range 0 to 1.0\n',
-                                '\n',
-                                '# Activity factor for Data (0->1 transitions) per cycle (for DDR, need to account for the higher activity in this parameter. E.g. max. activity factor for DDR is 1.0, for SDR is 0.5)\n',
-                                ' \n',
-                                '-activity_dq 1.0 //Valid range 0 to 1.0 for DDR, 0 to 0.5 for SDR\n',
-                                '\n',
-                                '# Activity factor for Control/Address (0->1 transitions) per cycle (for DDR, need to account for the higher activity in this parameter. E.g. max. activity factor for DDR is 1.0, for SDR is 0.5)\n',
-                                '\n',
-                                '-activity_ca 0.5 //Valid range 0 to 1.0 for DDR, 0 to 0.5 for SDR, 0 to 0.25 for 2T, and 0 to 0.17 for 3T\n',
-                                '\n',
-                                '# Number of DQ pins \n',
-                                '\n',
-                                '-num_dq 72 //Number of DQ pins. Includes ECC pins.\n',
-                                '\n',
-                                '# Number of DQS pins. DQS is a data strobe that is sent along with a small number of data-lanes so the source synchronous timing is local to these DQ bits. Typically, 1 DQS per byte (8 DQ bits) is used. The DQS is also typucally differential, just like the CLK pin. \n',
-                                '\n',
-                                '-num_dqs 18 //2 x differential pairs. Include ECC pins as well. Valid range 0 to 18. For x4 memories, could have 36 DQS pins.\n',
-                                '\n',
-                                '# Number of CA pins \n',
-                                '\n',
-                                '-num_ca 25 //Valid range 0 to 35 pins.\n',
-                                '\n',
-                                '# Number of CLK pins. CLK is typically a differential pair. In some cases additional CLK pairs may be used to limit the loading on the CLK pin. \n',
-                                '\n',
-                                '-num_clk  2 //2 x differential pair. Valid values: 0/2/4.\n',
-                                '\n',
-                                '# Number of Physical Ranks\n',
-                                '\n',
-                                '-num_mem_dq 2 //Number of ranks (loads on DQ and DQS) per buffer/register. If multiple LRDIMMs or buffer chips exist, the analysis for capacity and power is reported per buffer/register. \n',
-                                '\n',
-                                '# Width of the Memory Data Bus\n',
-                                '\n',
-                                '-mem_data_width 8 //x4 or x8 or x16 or x32 memories. For WideIO upto x128.\n',
-                                '\n',
-                                '# RTT Termination Resistance\n',
-                                '\n',
-                                '-rtt_value 10000\n',
-                                '\n',
-                                '# RON Termination Resistance\n',
-                                '\n',
-                                '-ron_value 34\n',
-                                '\n',
-                                '# Time of flight for DQ\n',
-                                '\n',
-                                '-tflight_value\n',
-                                '\n',
-                                '# Parameter related to MemCAD\n',
-                                '\n',
-                                '# Number of BoBs: 1,2,3,4,5,6,\n',
-                                '-num_bobs 1\n',
-                                '\t\n',
-                                '# Memory System Capacity in GB\n',
-                                '-capacity 80\t\n',
-                                '\t\n',
-                                '# Number of Channel per BoB: 1,2. \n',
-                                '-num_channels_per_bob 1\t\n',
-                                '\n',
-                                '# First Metric for ordering different design points\t\n',
-                                '-first metric "Cost"\n',
-                                '#-first metric "Bandwidth"\n',
-                                '#-first metric "Energy"\n',
-                                '\t\n',
-                                '# Second Metric for ordering different design points\t\n',
-                                '#-second metric "Cost"\n',
-                                '-second metric "Bandwidth"\n',
-                                '#-second metric "Energy"\n',
-                                '\n',
-                                '# Third Metric for ordering different design points\t\n',
-                                '#-third metric "Cost"\n',
-                                '#-third metric "Bandwidth"\n',
-                                '-third metric "Energy"\t\n',
-                                '\t\n',
-                                '\t\n',
-                                '# Possible DIMM option to consider\n',
-                                '#-DIMM model "JUST_UDIMM"\n',
-                                '#-DIMM model "JUST_RDIMM"\n',
-                                '#-DIMM model "JUST_LRDIMM"\n',
-                                '-DIMM model "ALL"\n',
-                                '\n',
-                                '#if channels of each bob have the same configurations\n',
-                                '#-mirror_in_bob "T"\n',
-                                '-mirror_in_bob "F"\n',
-                                '\n',
-                                '#if we want to see all channels/bobs/memory configurations explored\t\n',
-                                '#-verbose "T"\n',
-                                '#-verbose "F"\n',
-                                '\n',
-                                '=======USER DEFINE======= \n']
+        self.baseline_config = [
+            "# power gating\n",
+            '-Array Power Gating - "false"\n',
+            '-WL Power Gating - "false"\n',
+            '-CL Power Gating - "false"\n',
+            '-Bitline floating - "false"\n',
+            '-Interconnect Power Gating - "false"\n',
+            "-Power Gating Performance Loss 0.01\n",
+            "\n",
+            "# following three parameters are meaningful only for main memories\n",
+            "-page size (bits) 8192 \n",
+            "-burst length 8\n",
+            "-internal prefetch width 8\n",
+            "\n",
+            "# following parameter can have one of five values -- (itrs-hp, itrs-lstp, itrs-lop, lp-dram, comm-dram)\n",
+            '-Data array cell type - "itrs-hp"\n',
+            '//-Data array cell type - "itrs-lstp"\n',
+            '//-Data array cell type - "itrs-lop"\n',
+            "\n",
+            "# following parameter can have one of three values -- (itrs-hp, itrs-lstp, itrs-lop)\n",
+            '-Data array peripheral type - "itrs-hp"\n',
+            '//-Data array peripheral type - "itrs-lstp"\n',
+            '//-Data array peripheral type - "itrs-lop"\n',
+            "\n",
+            "# following parameter can have one of five values -- (itrs-hp, itrs-lstp, itrs-lop, lp-dram, comm-dram)\n",
+            '-Tag array cell type - "itrs-hp"\n',
+            '//-Tag array cell type - "itrs-lstp"\n',
+            '//-Tag array cell type - "itrs-lop"\n',
+            "\n",
+            "# following parameter can have one of three values -- (itrs-hp, itrs-lstp, itrs-lop)\n",
+            '-Tag array peripheral type - "itrs-hp"\n',
+            '//-Tag array peripheral type - "itrs-lstp"\n',
+            '//-Tag array peripheral type - "itrs-lop\n',
+            "\n",
+            "\n",
+            "// 300-400 in steps of 10\n",
+            "-operating temperature (K) 360\n",
+            "\n",
+            "# to model special structure like branch target buffers, directory, etc. \n",
+            "# change the tag size parameter\n",
+            '# if you want cacti to calculate the tagbits, set the tag size to "default"\n',
+            '-tag size (b) "default"\n',
+            "//-tag size (b) 22\n",
+            "\n",
+            "# fast - data and tag access happen in parallel\n",
+            "# sequential - data array is accessed after accessing the tag array\n",
+            "# normal - data array lookup and tag access happen in parallel\n",
+            "#          final data block is broadcasted in data array h-tree \n",
+            "#          after getting the signal from the tag array\n",
+            '//-access mode (normal, sequential, fast) - "fast"\n',
+            '-access mode (normal, sequential, fast) - "normal"\n',
+            '//-access mode (normal, sequential, fast) - "sequential"\n',
+            "\n",
+            "\n",
+            "# DESIGN OBJECTIVE for UCA (or banks in NUCA)\n",
+            "-design objective (weight delay, dynamic power, leakage power, cycle time, area) 0:0:0:100:0\n",
+            "\n",
+            "# Percentage deviation from the minimum value \n",
+            "# Ex: A deviation value of 10:1000:1000:1000:1000 will try to find an organization\n",
+            "# that compromises at most 10% delay. \n",
+            "# NOTE: Try reasonable values for % deviation. Inconsistent deviation\n",
+            "# percentage values will not produce any valid organizations. For example,\n",
+            "# 0:0:100:100:100 will try to identify an organization that has both\n",
+            "# least delay and dynamic power. Since such an organization is not possible, CACTI will\n",
+            "# throw an error. Refer CACTI-6 Technical report for more details\n",
+            "-deviate (delay, dynamic power, leakage power, cycle time, area) 20:100000:100000:100000:100000\n",
+            "\n",
+            "# Objective for NUCA\n",
+            "-NUCAdesign objective (weight delay, dynamic power, leakage power, cycle time, area) 100:100:0:0:100\n",
+            "-NUCAdeviate (delay, dynamic power, leakage power, cycle time, area) 10:10000:10000:10000:10000\n",
+            "\n",
+            "# Set optimize tag to ED or ED^2 to obtain a cache configuration optimized for\n",
+            "# energy-delay or energy-delay sq. product\n",
+            "# Note: Optimize tag will disable weight or deviate values mentioned above\n",
+            "# Set it to NONE to let weight and deviate values determine the \n",
+            "# appropriate cache configuration\n",
+            '//-Optimize ED or ED^2 (ED, ED^2, NONE): "ED"\n',
+            '-Optimize ED or ED^2 (ED, ED^2, NONE): "ED^2"\n',
+            '//-Optimize ED or ED^2 (ED, ED^2, NONE): "NONE"\n',
+            "\n",
+            '-Cache model (NUCA, UCA)  - "UCA"\n',
+            '//-Cache model (NUCA, UCA)  - "NUCA"\n',
+            "\n",
+            "# In order for CACTI to find the optimal NUCA bank value the following\n",
+            "# variable should be assigned 0.\n",
+            "-NUCA bank count 0\n",
+            "\n",
+            "# NOTE: for nuca network frequency is set to a default value of \n",
+            "# 5GHz in time.c. CACTI automatically\n",
+            "# calculates the maximum possible frequency and downgrades this value if necessary\n",
+            "\n",
+            "# By default CACTI considers both full-swing and low-swing \n",
+            "# wires to find an optimal configuration. However, it is possible to \n",
+            '# restrict the search space by changing the signaling from "default" to \n',
+            '# "fullswing" or "lowswing" type.\n',
+            '-Wire signaling (fullswing, lowswing, default) - "Global_30"\n',
+            '//-Wire signaling (fullswing, lowswing, default) - "default"\n',
+            '//-Wire signaling (fullswing, lowswing, default) - "lowswing"\n',
+            "\n",
+            '//-Wire inside mat - "global"\n',
+            '-Wire inside mat - "semi-global"\n',
+            '//-Wire outside mat - "global"\n',
+            '-Wire outside mat - "semi-global"\n',
+            "\n",
+            '-Interconnect projection - "conservative"\n',
+            '//-Interconnect projection - "aggressive"\n',
+            "\n",
+            "# Contention in network (which is a function of core count and cache level) is one of\n",
+            "# the critical factor used for deciding the optimal bank count value\n",
+            "# core count can be 4, 8, or 16\n",
+            "//-Core count 4\n",
+            "-Core count 8\n",
+            "//-Core count 16\n",
+            '-Cache level (L2/L3) - "L3"\n',
+            "\n",
+            '-Add ECC - "true"\n',
+            "\n",
+            '//-Print level (DETAILED, CONCISE) - "CONCISE"\n',
+            '-Print level (DETAILED, CONCISE) - "DETAILED"\n',
+            "\n",
+            "# for debugging\n",
+            '-Print input parameters - "true"\n',
+            '//-Print input parameters - "false"\n',
+            "# force CACTI to model the cache with the \n",
+            "# following Ndbl, Ndwl, Nspd, Ndsam,\n",
+            "# and Ndcm values\n",
+            '//-Force cache config - "true"\n',
+            '-Force cache config - "false"\n',
+            "-Ndwl 1\n",
+            "-Ndbl 1\n",
+            "-Nspd 0\n",
+            "-Ndcm 1\n",
+            "-Ndsam1 0\n",
+            "-Ndsam2 0\n",
+            "\n",
+            "\n",
+            "\n",
+            "#### Default CONFIGURATION values for baseline external IO parameters to DRAM. More details can be found in the CACTI-IO technical report (), especially Chapters 2 and 3.\n",
+            "\n",
+            "# Memory Type (D3=DDR3, D4=DDR4, L=LPDDR2, W=WideIO, S=Serial). Additional memory types can be defined by the user in extio_technology.cc, along with their technology and configuration parameters.\n",
+            "\n",
+            '-dram_type "DDR3"\n',
+            '//-dram_type "DDR4"\n',
+            '//-dram_type "LPDDR2"\n',
+            '//-dram_type "WideIO"\n',
+            '//-dram_type "Serial"\n',
+            "\n",
+            "# Memory State (R=Read, W=Write, I=Idle  or S=Sleep) \n",
+            "\n",
+            '//-io state  "READ"\n',
+            '-io state "WRITE"\n',
+            '//-io state "IDLE"\n',
+            '//-io state "SLEEP"\n',
+            "\n",
+            "#Address bus timing. To alleviate the timing on the command and address bus due to high loading (shared across all memories on the channel), the interface allows for multi-cycle timing options. \n",
+            "\n",
+            "//-addr_timing 0.5 //DDR\n",
+            "-addr_timing 1.0 //SDR (half of DQ rate)\n",
+            "//-addr_timing 2.0 //2T timing (One fourth of DQ rate)\n",
+            "//-addr_timing 3.0 // 3T timing (One sixth of DQ rate)\n",
+            "\n",
+            "# Memory Density (Gbit per memory/DRAM die)\n",
+            "\n",
+            "-mem_density 4 Gb //Valid values 2^n Gb\n",
+            "\n",
+            "# IO frequency (MHz) (frequency of the external memory interface).\n",
+            "\n",
+            "-bus_freq 800 MHz //As of current memory standards (2013), valid range 0 to 1.5 GHz for DDR3, 0 to 533 MHz for LPDDR2, 0 - 800 MHz for WideIO and 0 - 3 GHz for Low-swing differential. However this can change, and the user is free to define valid ranges based on new memory types or extending beyond existing standards for existing dram types.\n",
+            "\n",
+            "# Duty Cycle (fraction of time in the Memory State defined above)\n",
+            "\n",
+            "-duty_cycle 1.0 //Valid range 0 to 1.0\n",
+            "\n",
+            "# Activity factor for Data (0->1 transitions) per cycle (for DDR, need to account for the higher activity in this parameter. E.g. max. activity factor for DDR is 1.0, for SDR is 0.5)\n",
+            " \n",
+            "-activity_dq 1.0 //Valid range 0 to 1.0 for DDR, 0 to 0.5 for SDR\n",
+            "\n",
+            "# Activity factor for Control/Address (0->1 transitions) per cycle (for DDR, need to account for the higher activity in this parameter. E.g. max. activity factor for DDR is 1.0, for SDR is 0.5)\n",
+            "\n",
+            "-activity_ca 0.5 //Valid range 0 to 1.0 for DDR, 0 to 0.5 for SDR, 0 to 0.25 for 2T, and 0 to 0.17 for 3T\n",
+            "\n",
+            "# Number of DQ pins \n",
+            "\n",
+            "-num_dq 72 //Number of DQ pins. Includes ECC pins.\n",
+            "\n",
+            "# Number of DQS pins. DQS is a data strobe that is sent along with a small number of data-lanes so the source synchronous timing is local to these DQ bits. Typically, 1 DQS per byte (8 DQ bits) is used. The DQS is also typucally differential, just like the CLK pin. \n",
+            "\n",
+            "-num_dqs 18 //2 x differential pairs. Include ECC pins as well. Valid range 0 to 18. For x4 memories, could have 36 DQS pins.\n",
+            "\n",
+            "# Number of CA pins \n",
+            "\n",
+            "-num_ca 25 //Valid range 0 to 35 pins.\n",
+            "\n",
+            "# Number of CLK pins. CLK is typically a differential pair. In some cases additional CLK pairs may be used to limit the loading on the CLK pin. \n",
+            "\n",
+            "-num_clk  2 //2 x differential pair. Valid values: 0/2/4.\n",
+            "\n",
+            "# Number of Physical Ranks\n",
+            "\n",
+            "-num_mem_dq 2 //Number of ranks (loads on DQ and DQS) per buffer/register. If multiple LRDIMMs or buffer chips exist, the analysis for capacity and power is reported per buffer/register. \n",
+            "\n",
+            "# Width of the Memory Data Bus\n",
+            "\n",
+            "-mem_data_width 8 //x4 or x8 or x16 or x32 memories. For WideIO upto x128.\n",
+            "\n",
+            "# RTT Termination Resistance\n",
+            "\n",
+            "-rtt_value 10000\n",
+            "\n",
+            "# RON Termination Resistance\n",
+            "\n",
+            "-ron_value 34\n",
+            "\n",
+            "# Time of flight for DQ\n",
+            "\n",
+            "-tflight_value\n",
+            "\n",
+            "# Parameter related to MemCAD\n",
+            "\n",
+            "# Number of BoBs: 1,2,3,4,5,6,\n",
+            "-num_bobs 1\n",
+            "\t\n",
+            "# Memory System Capacity in GB\n",
+            "-capacity 80\t\n",
+            "\t\n",
+            "# Number of Channel per BoB: 1,2. \n",
+            "-num_channels_per_bob 1\t\n",
+            "\n",
+            "# First Metric for ordering different design points\t\n",
+            '-first metric "Cost"\n',
+            '#-first metric "Bandwidth"\n',
+            '#-first metric "Energy"\n',
+            "\t\n",
+            "# Second Metric for ordering different design points\t\n",
+            '#-second metric "Cost"\n',
+            '-second metric "Bandwidth"\n',
+            '#-second metric "Energy"\n',
+            "\n",
+            "# Third Metric for ordering different design points\t\n",
+            '#-third metric "Cost"\n',
+            '#-third metric "Bandwidth"\n',
+            '-third metric "Energy"\t\n',
+            "\t\n",
+            "\t\n",
+            "# Possible DIMM option to consider\n",
+            '#-DIMM model "JUST_UDIMM"\n',
+            '#-DIMM model "JUST_RDIMM"\n',
+            '#-DIMM model "JUST_LRDIMM"\n',
+            '-DIMM model "ALL"\n',
+            "\n",
+            "#if channels of each bob have the same configurations\n",
+            '#-mirror_in_bob "T"\n',
+            '-mirror_in_bob "F"\n',
+            "\n",
+            "#if we want to see all channels/bobs/memory configurations explored\t\n",
+            '#-verbose "T"\n',
+            '#-verbose "F"\n',
+            "\n",
+            "=======USER DEFINE======= \n",
+        ]
 
         self.config_options = {}
-        self.config_options['cache_size'] = {'string': '-size (bytes) ',
-                                             'option': [64, 128, 256, 512, 1024, 2048, 4096, 8192, 16384, 32768,
-                                                        65536, 131072, 262144, 524288, 1048576, 2097152, 4194304,
-                                                        8388608, 16777216, 33554432, 134217728, 67108864,
-                                                        1073741824],
-                                             'default': 64}
-
-        self.config_options['line_size'] = {'string': '-block size (bytes) ',
-                                            'option': [8, 16, 24],
-                                            'default': 64}
-
-        # Unit for IO_bus_width is bit.
-        self.config_options['IO_bus_width'] = {'string': '-output/input bus width ',
-                                               'option': [4, 8, 16, 24, 32, 64, 128],
-                                               'default': 128}
-
-        self.config_options['associativity'] = {'string': '-associativity ',
-                                                'option': [0, 1, 2, 4],
-                                                'default': 1}
-
-        self.config_options['rd_wr_port'] = {'string': '-read-write port ',
-                                             'option': [0, 1, 2, 3, 4],
-                                             'default': 0}
-
-        self.config_options['ex_rd_port'] = {'string': '-exclusive read port ',
-                                             'option': [0, 1, 2, 3, 4],
-                                             'default': 2}
-
-        self.config_options['ex_wr_port'] = {'string': '-exclusive write port ',
-                                             'option': [0, 1, 2, 3, 4],
-                                             'default': 2}
-
-        self.config_options['single_rd_port'] = {'string': '-single ended read ports ',
-                                                 'option': [0, 1, 2, 3, 4],
-                                                 'default': 0}
-
-        self.config_options['bank_count'] = {'string': '-UCA bank count ',
-                                             'option': [1, 2, 4, 8, 16],
-                                             'default': 1}
-
-        self.config_options['technology'] = {'string': '-technology (u) ',
-                                             'option': [0.022, 0.028, 0.040, 0.032, 0.065, 0.090],
-                                             'default': 0.090}
-
-        self.config_options['mem_type'] = {'string': '-cache type ',
-                                           'option': ['"cache"', '"ram"', '"main memory"'],
-                                           'default': '"ram"'}
+        """ entire memory size (unit: Byte, range: >= 64)"""
+        self.config_options["cache_size"] = {
+            "string": "-size (bytes) ",
+            "option": [
+                64,
+                128,
+                256,
+                512,
+                1024,
+                2048,
+                4096,
+                8192,
+                16384,
+                32768,
+                65536,
+                131072,
+                262144,
+                524288,
+                1048576,
+                2097152,
+                4194304,
+                8388608,
+                16777216,
+                33554432,
+                134217728,
+                67108864,
+                1073741824,
+            ],
+            "default": 64,
+        }
+
+        """ number of bytes on a single row (constraint: bitwidth >= IO_bus_width)"""
+        self.config_options["line_size"] = {
+            "string": "-block size (bytes) ",
+            "option": [8, 16, 24],
+            "default": 64,
+        }
+
+        """ IO bus width (unit: bit). Minimum: 4 (smaller than 4 will results in generation fail) """
+        self.config_options["IO_bus_width"] = {
+            "string": "-output/input bus width ",
+            "option": [4, 8, 16, 24, 32, 64, 128],
+            "default": 64,
+        }
+
+        self.config_options["associativity"] = {
+            "string": "-associativity ",
+            "option": [0, 1, 2, 4],
+            "default": 1,
+        }
+
+        """ number of wr port """
+        self.config_options["rd_wr_port"] = {
+            "string": "-read-write port ",
+            "option": [0, 1, 2, 3, 4],
+            "default": 1,
+        }
+
+        """ number of exclusive read port """
+        self.config_options["ex_rd_port"] = {
+            "string": "-exclusive read port ",
+            "option": [0, 1, 2, 3, 4],
+            "default": 0,
+        }
+
+        """ number of exclusive write port """
+        self.config_options["ex_wr_port"] = {
+            "string": "-exclusive write port ",
+            "option": [0, 1, 2, 3, 4],
+            "default": 0,
+        }
+
+        self.config_options["single_rd_port"] = {
+            "string": "-single ended read ports ",
+            "option": [0, 1, 2, 3, 4],
+            "default": 0,
+        }
+
+        """ number of bank """
+        self.config_options["bank_count"] = {
+            "string": "-UCA bank count ",
+            "option": [1, 2, 4, 8, 16],
+            "default": 1,
+        }
+
+        """ technology node """
+        self.config_options["technology"] = {
+            "string": "-technology (u) ",
+            "option": [0.022, 0.028, 0.040, 0.032, 0.065, 0.090],
+            "default": 0.065,
+        }
+        """ memory type """
+        self.config_options["mem_type"] = {
+            "string": "-cache type ",
+            "option": ['"cache"', '"ram"', '"main memory"'],
+            "default": '"ram"',
+        }
+
+        """ working temperature (unit: K, Temperature must be between 300 and 400 Kelvin and multiple of 10) """
+        self.config_options["temperature"] = {
+            "string": "-operating temperature (K) ",
+            "option": [300, 310, 320, 330],
+            "default": 300,
+        }
 
         return
 
     def change_default_value(self, name_list, new_value_list):
         for idx, name in enumerate(name_list):
-            self.config_options[name]['default'] = new_value_list[idx]
+            self.config_options[name]["default"] = new_value_list[idx]
 
     def write_config(self, user_config, path):
         f = open(path, "w+")
-        f.write(''.join(self.baseline_config))
-        f.write(''.join(user_config))
+        f.write("".join(self.baseline_config))
+        f.write("".join(user_config))
         f.close()
 
-    def call_cacti(self, cacti_master_path, self_gen_cfg_path):
+    def call_cacti(self, path):
         # os.system('./cacti -infile ./self_gen/cache.cfg')
-
-        print('##########################################################################################')
-        original_cwd = os.getcwd()
-        # Change the directory to the cacti master directory as using absolute paths yields a "Segmentation fault"
-        os.chdir(cacti_master_path)
-        common_path = os.path.commonpath([cacti_master_path, self_gen_cfg_path])
-        if common_path != cacti_master_path:
-            raise NotImplementedError("Config path for cacti should be inside cacti_master folder.")
-        self_gen_cfg_path_relative = f"./{os.path.relpath(self_gen_cfg_path, start=cacti_master_path)}"
-        cacti_cmd = f'./cacti -infile {self_gen_cfg_path_relative}'
-        stream = os.popen(cacti_cmd)
+        # print('##########################################################################################')
+        # stream = os.popen('./cacti -infile %s' %path)
+        stream = os.popen("./cacti -infile %s &> /dev/null" % path)
+        # stream = os.popen('./cacti -infile %s' %path)
         output = stream.readlines()
         for l in output:
-            print(l, end = '')
-        # Change back to the original working directory
-        os.chdir(original_cwd)
+            print(l, end="")
         return output
 
-    def cacti_auto(self, user_input, cacti_master_path, self_gen_cfg_path):
-        '''
+    def cacti_auto(self, user_input, path):
+        """
         user_input format can be 1 out of these 3:
         user_input = ['default']
         user_input = ['single', [['mem_type', 'technology', ...], ['"ram"', 0.028, ...]]
         user_input = ['sweep', ['IO_bus_width'/'']]
-        '''
-        print(f"{self_gen_cfg_path=}")
+        """
+
         user_config = []
-        if user_input[0] == 'default':
+        """ use default value for each parameter """
+        if user_input[0] == "default":
             for itm in self.config_options.keys():
-                user_config.append(self.config_options[itm]['string'] + str(self.config_options[itm]['default']) + '\n')
-            self.write_config(user_config, self_gen_cfg_path)
-            self.call_cacti(cacti_master_path, self_gen_cfg_path)
+                user_config.append(self.config_options[itm]["string"] + str(self.config_options[itm]["default"]) + "\n")
+            self.write_config(user_config, path)
+            self.call_cacti(path)
 
-        if user_input[0] == 'single':
+        """ use user defined value for each user defined parameter """
+        if user_input[0] == "single":
             for itm in self.config_options.keys():
                 if itm in user_input[1][0]:
                     ii = user_input[1][0].index(itm)
-                    user_config.append(self.config_options[itm]['string'] + str(user_input[1][1][ii]) + '\n')
+                    user_config.append(self.config_options[itm]["string"] + str(user_input[1][1][ii]) + "\n")
                 else:
-                    user_config.append(self.config_options[itm]['string'] + str(self.config_options[itm]['default']) + '\n')
-            self.write_config(user_config, self_gen_cfg_path)
-            self.call_cacti(cacti_master_path, self_gen_cfg_path)
+                    user_config.append(
+                        self.config_options[itm]["string"] + str(self.config_options[itm]["default"]) + "\n"
+                    )
+            self.write_config(user_config, path)
+            self.call_cacti(path)
 
-        if user_input[0] == 'sweep':
+        if user_input[0] == "sweep":
             # produce non-sweeping term
             common_part = []
             for itm in self.config_options.keys():
                 if itm not in user_input[1]:
-                    common_part.append(self.config_options[itm]['string'] + str(self.config_options[itm]['default']) + '\n')
+                    common_part.append(
+                        self.config_options[itm]["string"] + str(self.config_options[itm]["default"]) + "\n"
+                    )
 
             for itm in user_input[1]:
-                for va in self.config_options[itm]['option']:
-                    user_config.append([self.config_options[itm]['string'] + str(va) + '\n'])
+                for va in self.config_options[itm]["option"]:
+                    user_config.append([self.config_options[itm]["string"] + str(va) + "\n"])
 
             for ii in range(len(user_config)):
                 user_config[ii] += common_part
 
             for ii in range(len(user_config)):
-                self.write_config(user_config[ii], self_gen_cfg_path)
-                self.call_cacti(cacti_master_path, self_gen_cfg_path)
-
-
+                self.write_config(user_config[ii], path)
+                self.call_cacti(path)
 
 
+def get_cacti_cost(cacti_path, tech_node, mem_type, mem_size_in_byte, bw, hd_hash="a"):
+    """
+    extract time, area, r_energy, w_energy cost from cacti 7.0
+    :param cacti_path:          the location of cacti
+    :param tech_node:           technology node (directly supported node by CACTI: 0.022, 0.032, 0.045, 0.065, 0.09, 0.18)
+    :param mem_type:            memory type (sram or dram)
+    :param mem_size_in_byte:    memory size (unit: byte)
+    :param bw:                  memory IO bitwidth
+    :param hd_hash:             input file suffix when generating CACTI input file (useful and in avoid of file conflict for multi-processing simulation)
+    Attention: for CACTI, the miminum mem_size=64B, minimum_rows=32
+    """
+    import logging as _logging
+
+    _logging_level = _logging.CRITICAL
+    _logging_format = "%(asctime)s - %(funcName)s +%(lineno)s - %(levelname)s - %(message)s"
+    _logging.basicConfig(level=_logging_level, format=_logging_format)
+
+    # get current system (linux or windows)
+    system = platform.system()  # "Linux" or "Windows"
+
+    # get the current working directory
+    cwd = os.getcwd()
+
+    # change the working directory
+    os.chdir(cacti_path)
+
+    # input parameters definition
+    if tech_node == 0.028:
+        tech = 0.032  # technology: 32 nm (corresponding VDD = 0.9)
+        scaling_factor = 0.9 * 0.9
+    else:
+        tech = tech_node
+        scaling_factor = 1
+    if mem_type == "dram":
+        mem = '"main memory"'
+    elif mem_type == "sram":
+        mem = '"ram"'
+    else:
+        msg = f"mem_type can only be dram or sram. Now it is: {mem_type}"
+        raise ValueError(msg)
+
+    """
+    due to the growth of the area cost estimation from CACTI exceeds 1x when bw > 32, it will be set to 1x.
+    """
+    # check if bw > 32
+    if bw > 32:  # adjust the setting for CACTI
+        rows = mem_size_in_byte * 8 / bw
+        line_size = int(32 / 8)
+        IO_bus_width = 32
+        mem_size_in_byte_adjust = rows * 32 / 8
+    else:  # normal case
+        rows = mem_size_in_byte * 8 / bw
+        line_size = int(bw / 8)  # how many bytes on a row
+        IO_bus_width = bw
+        mem_size_in_byte_adjust = mem_size_in_byte
+
+    file_path = "./self_gen"  # location for input file (cache.cfg) and output file (cache.cfg.out)
+    os.makedirs(file_path, exist_ok=True)
+
+    # clear target folder
+    # if system == 'Linux':
+    #     os.system(f'rm -f {file_path}/cache_{hd_hash}.cfg.out')
+    # elif system == 'Windows':
+    #     os.system(f'del {file_path}/cache_{hd_hash}.cfg.out')
+    # else:
+    #     # user-defined command
+    #     breakpoint()
+
+    C = CactiConfig()
+    C.cacti_auto(
+        [
+            "single",
+            [
+                ["technology", "cache_size", "line_size", "IO_bus_width", "mem_type"],
+                [tech, mem_size_in_byte_adjust, line_size, IO_bus_width, mem],
+            ],
+        ],
+        f"{file_path}/cache_{hd_hash}.cfg",
+    )
+    # read out result
+    try:
+        f = open(f"{file_path}/cache_{hd_hash}.cfg.out", "r")
+    except:
+        msg = f"CACTI failed. [current setting] rows: {rows}, bw: {bw}, mem size (byte): {mem_size_in_byte}"
+        _logging.critical(msg)
+        msg = f"[CACTI minimal requirement] rows: >= 32, bw: >= 8, mem size (byte): >=64"
+        _logging.critical(msg)
+        exit()
+    result = {}
+    raw_result = f.readlines()
+    f.close()
+    for ii, each_line in enumerate(raw_result):
+        if ii == 0:
+            attribute_list = each_line.split(",")
+            for each_attribute in attribute_list:
+                result[each_attribute] = []
+        else:
+            for jj, each_value in enumerate(each_line.split(",")):
+                try:
+                    result[attribute_list[jj]].append(float(each_value))
+                except:
+                    pass
+    # get required cost
+    try:
+        access_time = scaling_factor * float(result[" Access time (ns)"][-1])  # unit: ns
+        if bw > 32:
+            area = scaling_factor * float(result[" Area (mm2)"][-1]) * 2 * bw / 32  # unit: mm2
+            r_cost = scaling_factor * float(result[" Dynamic read energy (nJ)"][-1]) * bw / 32  # unit: nJ
+            w_cost = scaling_factor * float(result[" Dynamic write energy (nJ)"][-1]) * bw / 32  # unit: nJ
+        else:
+            area = scaling_factor * float(result[" Area (mm2)"][-1]) * 2  # unit: mm2
+            r_cost = scaling_factor * float(result[" Dynamic read energy (nJ)"][-1])  # unit: nJ
+            w_cost = scaling_factor * float(result[" Dynamic write energy (nJ)"][-1])  # unit: nJ
+    except KeyError:
+        _logging.critical(f"**KeyError** in result, current result: {result}")
+        breakpoint()
+
+    # clear generated files
+    # if system == 'Linux':
+    #     os.system(f'rm {file_path}/cache_{hd_hash}.cfg.out') # remove output file
+    #     os.system(f'rm {file_path}/cache_{hd_hash}.cfg') # remove input file
+    # elif system == 'Windows':
+    #     os.system(f'del {file_path}/cache_{hd_hash}.cfg.out') # remove output file
+    #     os.system(f'del {file_path}/cache_{hd_hash}.cfg') # remove input file
+    # else:
+    #     # user-defined command
+    #     breakpoint()
+
+    # change back the working directory
+    os.chdir(cwd)
+
+    # round the value to avoid too long data representation
+    area = round(area, 7)  # keep 3 valid digits
+    r_cost *= 1000  # unit: pJ/access
+    w_cost *= 1000  # unit: pJ/access
+
+    return access_time, area, r_cost, w_cost
+
+
+def get_w_cost_per_weight_from_cacti(cacti_path, tech_param, hd_param, dimensions):
+    # Get w_cost for imc cell group
+    # Used in user-provided hardware input file, when it is needed.
+    # cacti_path = "zigzag/classes/cacti/cacti_master"
+    tech_node = tech_param["tech_node"]
+    wl_dim = hd_param["wordline_dimension"]
+    bl_dim = hd_param["bitline_dimension"]
+    wl_dim_size = dimensions[wl_dim]
+    bl_dim_size = dimensions[bl_dim]
+    group_depth = hd_param["group_depth"]
+    w_pres = hd_param["weight_precision"]
+    cell_array_size = wl_dim_size * bl_dim_size * group_depth * w_pres / 8  # array size. unit: byte
+    array_bw = wl_dim_size * w_pres  # imc array bandwidth. unit: bit
+
+    # we will call cacti to get the area (mm^2), access_time (ns), r_cost (nJ/access), w_cost (nJ/access)
+    access_time, area, r_cost, w_cost = get_cacti_cost(
+        cacti_path=cacti_path,
+        tech_node=tech_node,
+        mem_type="sram",
+        mem_size_in_byte=cell_array_size,
+        bw=array_bw,
+    )
+    w_cost_per_weight_writing = w_cost * w_pres / array_bw  # pJ/weight
+    w_cost_per_weight_writing = round(w_cost_per_weight_writing, 3)  # keep 3 valid digits
+    return w_cost_per_weight_writing  # unit: pJ/weight
+
+
+if __name__ == "__main__":
+    # an example for use (28nm, mem size: 32rows * 32 cols, bw: 32 bit)
+    for bw in [32]:
+        mem_size = 32 * 32 / 8  # byte
+        rows = mem_size * 8 / bw
+        access_time, area, r_cost, w_cost = get_cacti_cost(
+            cacti_path="../../cacti/cacti_master",
+            tech_node=0.028,
+            mem_type="sram",
+            mem_size_in_byte=mem_size,
+            bw=bw,
+        )
+        print(
+            f"access time (ns): {access_time}, area (mm2): {area}, r_cost (pJ)/bit: {r_cost*1000/bw}, w_cost (pJ)/bit: {w_cost*1000/bw}"
+        )
+    exit()
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti_top.py` & `zigzag_dse-3.1.1/zigzag/cacti/cacti_master/cacti_top.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,113 +1,156 @@
 import yaml
 import os
 import argparse
 
-from zigzag.classes.cacti.cacti_master.cacti_config_creator import CactiConfig
-
+from zigzag.cacti.cacti_master.cacti_config_creator import CactiConfig
 
 parser = argparse.ArgumentParser()
-parser.add_argument('--mem_type')
-parser.add_argument('--cache_size')
-parser.add_argument('--IO_bus_width')
-parser.add_argument('--ex_rd_port')
-parser.add_argument('--ex_wr_port')
-parser.add_argument('--rd_wr_port')
-parser.add_argument('--bank_count')
-parser.add_argument('--mem_pool_path')
-parser.add_argument('--technology')
+parser.add_argument("--mem_type")
+parser.add_argument("--cache_size")
+parser.add_argument("--IO_bus_width")
+parser.add_argument("--ex_rd_port")
+parser.add_argument("--ex_wr_port")
+parser.add_argument("--rd_wr_port")
+parser.add_argument("--bank_count")
+parser.add_argument("--mem_pool_path")
+parser.add_argument("--technology")
 args = parser.parse_args()
 
 
-mem_pool_path = args.mem_pool_path
+mem_pool_path: str = args.mem_pool_path
 cacti_master_path = os.path.dirname(mem_pool_path)
 print(f"{cacti_master_path=}")
 
-self_gen_folder_name = 'self_gen'
+self_gen_folder_name = "self_gen"
 self_gen_path = os.path.join(cacti_master_path, self_gen_folder_name)
 if not os.path.isdir(self_gen_path):
     os.mkdir(self_gen_path)
 
-os.system(f'rm -rf {self_gen_path}/*')
+os.system(f"rm -rf {self_gen_path}/*")
 C = CactiConfig()
 
-'''Function 1: set default value'''
+# Function 1: set default value
 # C.change_default_value(['technology'], [0.090])
 
-'''Function 2: use default values to run CACTI'''
+# Function 2: use default values to run CACTI
 # C.cacti_auto(['default'], file_path + '/cache.cfg')
 
-'''Function 3: use user-defined + default values to run CACTI'''
+# Function 3: use user-defined + default values to run CACTI
 # C.cacti_auto(['single', [['technology', 'cache_size'],[0.022, 524288]]], file_path+'/cache.cfg')
 
-'''Function 4: sweep any one variable using the default list & other default value'''
+# Function 4: sweep any one variable using the default list & other default value
 # C.cacti_auto(['sweep', ['IO_bus_width']], file_path+'/cache.cfg')
 
-''' Combining Function 1 & 4 to do multi-variable sweep '''
+#  Combining Function 1 & 4 to do multi-variable sweep
 
-mem_type = args.mem_type
+mem_type: str = args.mem_type
 
-if mem_type == 'sram':
+if mem_type == "sram":
     mem_type = '"ram"'
 else:
-    mem_type == '"main memory"'
+    mem_type = '"main memory"'
 
 cache_size = args.cache_size
 IO_bus_width = args.IO_bus_width
 ex_rd_port = args.ex_rd_port
 ex_wr_port = args.ex_wr_port
 rd_wr_port = args.rd_wr_port
 bank_count = args.bank_count
 
 technology = args.technology
 
 
-C.cacti_auto(['single', [['mem_type', 'cache_size', 'IO_bus_width', 'ex_rd_port', 'ex_wr_port', 'rd_wr_port', 'bank_count', 'technology'],[mem_type, cache_size, IO_bus_width, ex_rd_port, ex_wr_port, rd_wr_port, bank_count, technology]]], cacti_master_path, f'{self_gen_path}/cache.cfg')
+C.cacti_auto(
+    [
+        "single",
+        [
+            [
+                "mem_type",
+                "cache_size",
+                "IO_bus_width",
+                "ex_rd_port",
+                "ex_wr_port",
+                "rd_wr_port",
+                "bank_count",
+                "technology",
+            ],
+            [
+                mem_type,
+                cache_size,
+                IO_bus_width,
+                ex_rd_port,
+                ex_wr_port,
+                rd_wr_port,
+                bank_count,
+                technology,
+            ],
+        ],
+    ],
+    cacti_master_path,
+    f"{self_gen_path}/cache.cfg",
+)
 
 result = {}
-with open('%s/cache.cfg.out' % self_gen_path, 'r') as fp:
+with open("%s/cache.cfg.out" % self_gen_path, "r") as fp:
     raw_result = fp.readlines()
     for ii, each_line in enumerate(raw_result):
         if ii == 0:
-            attribute_list = each_line.split(',')
+            attribute_list = each_line.split(",")
             for each_attribute in attribute_list:
                 result[each_attribute] = []
         else:
-            for jj, each_value in enumerate(each_line.split(',')):
+            for jj, each_value in enumerate(each_line.split(",")):
                 try:
                     result[attribute_list[jj]].append(float(each_value))
                 except:
                     pass
 
 
-for i in range(len(result[' Capacity (bytes)'])):
-    size_byte = result[' Capacity (bytes)'][i]
-    area = result[' Area (mm2)'][i]
-    read_word = result[' Dynamic read energy (nJ)'][i]
-    write_word = result[' Dynamic write energy (nJ)'][i]
-    mem_bw = result[' Output width (bits)'][i]
+for i in range(len(result[" Capacity (bytes)"])):
+    size_byte = result[" Capacity (bytes)"][i]
+    area = result[" Area (mm2)"][i]
+    read_word = result[" Dynamic read energy (nJ)"][i]
+    write_word = result[" Dynamic write energy (nJ)"][i]
+    mem_bw = result[" Output width (bits)"][i]
     utilization_rate = 0.7
 
     if mem_type == '"ram"':
-        mem_type = 'sram'
+        mem_type = "sram"
     else:
-        mem_type = 'dram'
-
-    mem_name = str(int(size_byte)) + '_Byte_' + str(int(mem_bw)) + '_BW_' + str(ex_rd_port) + '_' + str(ex_wr_port) + '_' + str(rd_wr_port) + '_BANK_COUNT_' + str(bank_count) + '_TECH_' + str(technology)
+        mem_type = "dram"
 
-    new_result = {'%s' % mem_name: {
-        'size_byte': int(size_byte),
-        'size_bit': int(size_byte * 8),
-        'area': area,
-        'cost': {'read_word': read_word, 'write_word': write_word},
-        'IO_bus_width': int(mem_bw),
-        'ex_rd_port': ex_rd_port,
-        'ex_wr_port': ex_wr_port,
-        'rd_wr_port': rd_wr_port,
-        'bank_count': bank_count, 
-        'memory_type': mem_type,
-        'technology': technology,
-    }}
-    with open(mem_pool_path, 'a+') as fp:
+    mem_name = (
+        str(int(size_byte))
+        + "_Byte_"
+        + str(int(mem_bw))
+        + "_BW_"
+        + str(ex_rd_port)
+        + "_"
+        + str(ex_wr_port)
+        + "_"
+        + str(rd_wr_port)
+        + "_BANK_COUNT_"
+        + str(bank_count)
+        + "_TECH_"
+        + str(technology)
+    )
+
+    new_result = {
+        "%s"
+        % mem_name: {
+            "size_byte": int(size_byte),
+            "size_bit": int(size_byte * 8),
+            "area": area,
+            "cost": {"read_word": read_word, "write_word": write_word},
+            "IO_bus_width": int(mem_bw),
+            "ex_rd_port": ex_rd_port,
+            "ex_wr_port": ex_wr_port,
+            "rd_wr_port": rd_wr_port,
+            "bank_count": bank_count,
+            "memory_type": mem_type,
+            "technology": technology,
+        }
+    }
+    with open(mem_pool_path, "a+") as fp:
         yaml.dump(new_result, fp)
-        fp.write('\n')
-
+        fp.write("\n")
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_parser.py` & `zigzag_dse-3.1.1/zigzag/cacti/cacti_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,50 @@
+from typing import Any
 import yaml
 import os
 import subprocess
 
 import logging
 
 logger = logging.getLogger(__name__)
 
-##  Class that provides the interface between ZigZag and CACTI.
+
 class CactiParser:
+    """!  Class that provides the interface between ZigZag and CACTI."""
 
     ## Path of current directory
     cacti_path = os.path.dirname(os.path.realpath(__file__))
     ## Path to cached cacti simulated memories
     MEM_POOL_PATH = f"{cacti_path}/cacti_master/example_mem_pool.yaml"
     ## Path to cacti python script to extract costs
     CACTI_TOP_PATH = f"{cacti_path}/cacti_master/cacti_top.py"
 
-    ## The class constructor
     def __init__(self):
+        """"""
         pass
-    
-    ## This function checks if the provided memory configuration was already used in the past.
-    # @param mem_type
-    # @param size
-    # @param r_bw
-    # @param r_port
-    # @param w_port
-    # @param rw_port
-    # @param bank
-    # @param mem_pool_path  Path to cached cacti simulated memories
-    # @return True          The requested memory item has been simulated once.
-    # @return False         The requested memory item has not been simualted so far.
+
     def item_exists(
         self,
-        mem_type,
-        size,
-        r_bw,
-        r_port,
-        w_port,
-        rw_port,
-        bank,
-        technology,
-        mem_pool_path=MEM_POOL_PATH,
-    ):
-        with open(mem_pool_path, "r") as fp:
-            memory_pool = yaml.full_load(fp)
+        size: int,
+        r_bw: int,
+        r_port: int,
+        w_port: int,
+        rw_port: int,
+        bank: int,
+        technology: float,
+        mem_pool_path: str = MEM_POOL_PATH,
+    ) -> bool:
+        """! This function checks whether the provided memory configuration was already used in the past.
+        @param mem_pool_path  Path to cached cacti simulated memories
+        @return Return wether the requested memory item has been simulated before.
+        """
+        with open(mem_pool_path, "r") as fp:  # pylint: disable=W1514
+            memory_pool: None | dict[str, dict[str, Any]] = yaml.full_load(fp)
 
-        if memory_pool != None:
+        if memory_pool is not None:
             for instance in memory_pool:
 
                 IO_bus_width = int(memory_pool[instance]["IO_bus_width"])
                 ex_rd_port = int(memory_pool[instance]["ex_rd_port"])
                 ex_wr_port = int(memory_pool[instance]["ex_wr_port"])
                 rd_wr_port = int(memory_pool[instance]["rd_wr_port"])
                 cache_size = int(memory_pool[instance]["size_bit"])
@@ -66,42 +60,35 @@
                     and (bank_count == bank)
                     and (tech == technology)
                 ):
                     return True
 
         return False
 
-    ## This function simulates a new item by calling CACTI7 based on the provided parameters
-    # @param mem_type
-    # @param size
-    # @param r_bw
-    # @param r_port
-    # @param w_port
-    # @param rw_port
-    # @param bank
-    # @param mem_pool_path  Path to cached cacti simulated memories
-    # @param cacti_top_path Path to cacti python script to extract costs
     def create_item(
         self,
-        mem_type,
-        size,
-        r_bw,
-        r_port,
-        w_port,
-        rw_port,
-        bank,
-        technology=0.022,
-        mem_pool_path=MEM_POOL_PATH,
-        cacti_top_path=CACTI_TOP_PATH,
-    ):
-        # print("No match in Cacti memory pool found!", size, r_bw, r_port, w_port, rw_port, bank)
-        # os.chdir(f'{CACTI_PATH}/cacti-master/')
+        mem_type: str,
+        size: int,
+        r_bw: int,
+        r_port: int,
+        w_port: int,
+        rw_port: int,
+        bank: int,
+        technology: float = 0.022,
+        mem_pool_path: str = MEM_POOL_PATH,
+        cacti_top_path: str = CACTI_TOP_PATH,
+    ) -> None:
+        """! This function simulates a new item by calling CACTI7 based on the provided parameters
+        @param mem_pool_path  Path to cached cacti simulated memories
+        @param cacti_top_path Path to cacti python script to extract costs
+        """
 
         p = subprocess.call(
             [
+                "PYTHONPATH=$(pwd)",
                 "python",
                 cacti_top_path,
                 "--mem_type",
                 str(mem_type),
                 "--cache_size",
                 str(int(size / 8)),
                 "--IO_bus_width",
@@ -118,62 +105,57 @@
                 str(mem_pool_path),
                 "--technology",
                 str(technology),
             ]
         )
 
         if p != 0:
-            raise ChildProcessError(
-                f"Cacti subprocess call failed with return value {p}."
-            )
+            raise ChildProcessError(f"Cacti subprocess call failed with return value {p}.")
 
-    ## This functions checks first if the memory with the provided parameters was already simulated once.
-    # In case it hasn't been simulated, then it will create a new memory item based on the provided parameters.
-    # @param mem_type
-    # @param size
-    # @param r_bw
-    # @param r_port
-    # @param w_port
-    # @param rw_port
-    # @param bank
-    # @param mem_pool_path  Path to cached cacti simulated memories
-    # @param cacti_top_path Path to cacti python script to extract costs
     def get_item(
         self,
-        mem_type,
-        size,
-        r_bw,
-        r_port,
-        w_port,
-        rw_port,
-        bank,
-        technology=0.022,
-        mem_pool_path=MEM_POOL_PATH,
-        cacti_top_path=CACTI_TOP_PATH,
-    ):
+        mem_type: str,
+        size: int,
+        r_bw: int,
+        r_port: int,
+        w_port: int,
+        rw_port: int,
+        bank: int,
+        technology: float = 0.022,
+        mem_pool_path: str = MEM_POOL_PATH,
+        cacti_top_path: str = CACTI_TOP_PATH,
+    ) -> tuple[float, float, float]:
+        """! This functions checks first if the memory with the provided parameters was already simulated once.
+        In case it hasn't been simulated, then it will create a new memory item based on the provided parameters.
+        @param mem_pool_path  Path to cached cacti simulated memories
+        @param cacti_top_path Path to cacti python script to extract costs
+        """
         if not os.path.exists(cacti_top_path):
             raise FileNotFoundError(f"Cacti top file doesn't exist: {cacti_top_path}.")
 
-        logger.info(
-            f"Extracting memory costs with CACTI for size = {size} and r_bw = {r_bw}."
-        )
+        logger.info(f"Extracting memory costs with CACTI for size = {size} and r_bw = {r_bw}.")
 
         if mem_type == "rf":
             new_mem_type = "sram"
             new_size = int(size * 128)
             new_r_bw = int(r_bw)
-            logger.warning(
-                f"Type {mem_type} -> {new_mem_type}. Size {size} -> {new_size}. BW {r_bw} -> {new_r_bw}."
-            )
+            logger.warning(f"Type {mem_type} -> {new_mem_type}. Size {size} -> {new_size}. BW {r_bw} -> {new_r_bw}.")
             mem_type = new_mem_type
             size = new_size
             r_bw = new_r_bw
 
         if not self.item_exists(
-            mem_type, size, r_bw, r_port, w_port, rw_port, bank, technology, mem_pool_path, 
+            size,
+            r_bw,
+            r_port,
+            w_port,
+            rw_port,
+            bank,
+            technology,
+            mem_pool_path,
         ):
             self.create_item(
                 mem_type,
                 size,
                 r_bw,
                 r_port,
                 w_port,
@@ -181,17 +163,17 @@
                 bank,
                 technology,
                 mem_pool_path,
                 cacti_top_path,
             )
 
         with open(mem_pool_path, "r") as fp:
-            memory_pool = yaml.full_load(fp)
+            memory_pool: None | dict[str, dict[str, Any]] = yaml.full_load(fp)
 
-        if memory_pool != None:
+        if memory_pool is not None:
             for instance in memory_pool:
 
                 IO_bus_width = int(memory_pool[instance]["IO_bus_width"])
                 area = memory_pool[instance]["area"]
                 bank_count = int(memory_pool[instance]["bank_count"])
                 read_cost = memory_pool[instance]["cost"]["read_word"] * 1000
                 write_cost = memory_pool[instance]["cost"]["write_word"] * 1000
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/cost_model/cost_model.py` & `zigzag_dse-3.1.1/zigzag/cost_model/cost_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,292 +1,325 @@
+from abc import ABCMeta, abstractmethod
 import logging
-from typing import Dict, List, Tuple
 from math import ceil
 import numpy as np
-from zigzag.classes.mapping.combined_mapping import Mapping
-from zigzag.classes.mapping.combined_mapping import FourWayDataMoving
-from zigzag.utils import pickle_deepcopy
+from zigzag.cost_model.port_activity import PortActivity, PortBeginOrEndActivity
+from zigzag.datatypes import Constants, LayerOperand, MemoryOperand
+from zigzag.hardware.architecture.Accelerator import Accelerator
+from zigzag.hardware.architecture.MemoryInstance import MemoryInstance
+from zigzag.mapping.Mapping import Mapping
+from zigzag.mapping.data_movement import DataDirection, FourWayDataMoving
+from zigzag.mapping.SpatialMappingInternal import SpatialMappingInternal
+from zigzag.mapping.TemporalMapping import TemporalMapping
+from zigzag.workload.layer_node import LayerNode
+from zigzag.utils import json_repr_handler, pickle_deepcopy
 
 logger = logging.getLogger(__name__)
 
-##  Class that collects all the data transfer rate (periodic) information for each DTL (data transfer link).
-class PortActivity:
 
-    ## The class constructor
-    # @param real_cycle     (int)     Within each period, the actual number of cycles used for transferring the amount of data, depended on the memory bw and the data amount to be transferred at that memory level.
-    # @param allowed_cycle  (int)
-    # @param period         (int)     The turnaround cycle at that memory level, which equals to the product of all the temporal loops of current and below memory level.
-    # @param period_count   (int)     The total number of period across the whole NN layer computation.
-    # @param layer_op       (str)
-    # @param mem_lv         (int)
-    # @param mov_dir        (str)
-    def __init__(
-        self,
-        real_cycle: int,
-        allowed_cycle: int,
-        period: int,
-        period_count: int,
-        layer_op: str,
-        mem_lv: int,
-        mov_dir: str,
-    ):
-        ## Within each period, the actual number of cycles used for transferring the amount of data, depended on the memory bw and the data amount to be transferred at that memory level.
-        self.real_cycle = real_cycle
-        self.allowed_cycle = allowed_cycle
-        ## The turnaround cycle at that memory level, which equals to the product of all the temporal loops of current and below memory level.
-        self.period = period
-        ## The total number of period across the whole NN layer computation.
-        self.period_count = period_count
-        self.served_op_lv_dir = (layer_op, mem_lv, mov_dir)
-        """ stalling (+) or slacking (-) cycle in one period """
-        self.SS_per_period = real_cycle - allowed_cycle
-        """ stalling (+) or slacking (-) cycle in total computation """
-        self.SS = (real_cycle - allowed_cycle) * (period_count - 1)
-        """ total memory updating window allowed """
-        self.MUW = allowed_cycle * (period_count - 1)
+class CostModelEvaluationABC(metaclass=ABCMeta):
+    """! Superclass for CostModelEvaluation and CumulativeCME"""
 
-    def __str__(self):
-        return str(self.served_op_lv_dir)
+    @abstractmethod
+    def __init__(self) -> None:
+        # Attributes that all subclasses should define
+        self.mem_energy_breakdown: dict[LayerOperand, list[float]]
+        self.mem_energy_breakdown_further: dict[LayerOperand, list[FourWayDataMoving]]
+        self.memory_word_access: dict[LayerOperand, list[FourWayDataMoving]]
+        self.MAC_energy: float
+        self.mem_energy: float
+        self.energy_total: float
+        self.data_loading_cycle: float
+        self.data_offloading_cycle: float
+        self.ideal_cycle: float
+        self.ideal_temporal_cycle: float
+        self.latency_total0: float
+        self.latency_total1: float
+        self.latency_total2: float
+        self.MAC_spatial_utilization: float
+        self.MAC_utilization0: float
+        self.MAC_utilization1: float
+        self.MAC_utilization2: float
 
-    def __repr__(self):
-        return str(self.served_op_lv_dir)
+        self.accelerator: Accelerator | None
 
-    def __eq__(self, other) -> bool:
-        return str(self.served_op_lv_dir) == other
+    def __add__(self, other: "CostModelEvaluationABC") -> "CumulativeCME":
+        result = CumulativeCME()
 
-    def __hash__(self):
-        return str(self.served_op_lv_dir)
+        # Energy
+        result.MAC_energy = self.MAC_energy + other.MAC_energy
+        result.mem_energy = self.mem_energy + other.mem_energy
+        result.energy_total = self.energy_total + other.energy_total
+
+        for layer_op, breakdown_this in self.mem_energy_breakdown.items():
+            if layer_op in other.mem_energy_breakdown.keys():
+                breakdown_other = other.mem_energy_breakdown[layer_op]
+                list_temp: list[float] = []
+                breakdown_len = min(len(breakdown_this), len(breakdown_other))
+                for i in range(breakdown_len):
+                    list_temp.append(breakdown_this[i] + breakdown_other[i])
+
+                list_temp += breakdown_this[breakdown_len:]
+                list_temp += breakdown_other[breakdown_len:]
+                result.mem_energy_breakdown[layer_op] = list_temp
+
+        for layer_op, breakdown_this in self.mem_energy_breakdown_further.items():
+            if layer_op in other.mem_energy_breakdown_further.keys():
+                breakdown_other = other.mem_energy_breakdown_further[layer_op]
+                list_temp2: list[FourWayDataMoving] = []
+                breakdown_len = min(len(breakdown_this), len(breakdown_other))
+                for i in range(breakdown_len):
+                    list_temp2.append(breakdown_this[i] + breakdown_other[i])
+                list_temp2 += breakdown_this[breakdown_len:]
+                list_temp2 += breakdown_other[breakdown_len:]
+                result.mem_energy_breakdown_further[layer_op] = list_temp2
+
+        # Add the operands from other that are either in `self` or `other`, but not yet in `result`
+        op_diff_self = set(self.mem_energy_breakdown.keys()) - set(result.mem_energy_breakdown.keys())
+        op_diff_other = set(other.mem_energy_breakdown.keys()) - set(result.mem_energy_breakdown.keys())
+        for layer_op in op_diff_self:
+            result.mem_energy_breakdown[layer_op] = self.mem_energy_breakdown[layer_op]
+            result.mem_energy_breakdown_further[layer_op] = self.mem_energy_breakdown_further[layer_op]
+        for layer_op in op_diff_other:
+            result.mem_energy_breakdown[layer_op] = other.mem_energy_breakdown[layer_op]
+            result.mem_energy_breakdown_further[layer_op] = other.mem_energy_breakdown_further[layer_op]
 
+        # Memory access
+        for layer_op, accesses_this in self.memory_word_access.items():
+            if layer_op in other.memory_word_access.keys():
+                accesses_other = other.memory_word_access[layer_op]
+                length = min(len(accesses_this), len(accesses_other))
+                list_temp3: list[FourWayDataMoving] = []
+                for i in range(length):
+                    list_temp3.append(accesses_this[i] + accesses_other[i])
+                list_temp3 += accesses_this[length:]
+                list_temp3 += accesses_other[length:]
+                result.memory_word_access[layer_op] = list_temp3
+
+        for layer_op in op_diff_self:
+            result.memory_word_access[layer_op] = self.memory_word_access[layer_op]
+        for layer_op in op_diff_other:
+            result.memory_word_access[layer_op] = other.memory_word_access[layer_op]
 
-## Class that collects all the data transfer rate information for each DTL (data transfer link).
-class PortBeginOrEndActivity:
-
-    ## The class constructor
-    # @param real_cycle     (int)   the actual number of cycles used for transferring the amount of data,
-    #                               depended on the memory bw and the data amount to be transferred at that memory level
-    # @param data_in_charge (int)   one-period data transfer amount (bit)
-    # @param mem_bw         (int)   bit/cycle
-    # @param layer_op       (str)
-    # @param mem_lv         (int)
-    # @param mov_dir        (str)   data moving direction
-    def __init__(
-        self,
-        real_cycle: int,
-        data_in_charge: int,
-        mem_bw: int,
-        layer_op: str,
-        mem_lv: int,
-        mov_dir: str,
-    ):
-        ## the actual number of cycles used for transferring the amount of data,
-        # depended on the memory bw and the data amount to be transferred at that memory level
-        self.real_cycle = real_cycle
-        ## one-period data transfer amount (bit)
-        self.data_in_charge = data_in_charge
-        ## bit/cycle
-        self.mem_bw = mem_bw
-        self.served_op_lv_dir = (layer_op, mem_lv, mov_dir)
+        # Latency
+        result.data_loading_cycle = self.data_loading_cycle + other.data_loading_cycle
+        result.data_offloading_cycle = self.data_offloading_cycle + other.data_offloading_cycle
+        result.ideal_cycle = self.ideal_cycle + other.ideal_cycle
+        result.ideal_temporal_cycle = self.ideal_temporal_cycle + other.ideal_temporal_cycle
+        result.latency_total0 = self.latency_total0 + other.latency_total0
+        result.latency_total1 = self.latency_total1 + other.latency_total1
+        result.latency_total2 = self.latency_total2 + other.latency_total2
 
-    def __str__(self):
-        return str(self.served_op_lv_dir)
+        # MAC utilization
+        result.MAC_spatial_utilization = result.ideal_cycle / result.ideal_temporal_cycle
+        result.MAC_utilization0 = result.ideal_cycle / result.latency_total0
+        result.MAC_utilization1 = result.ideal_cycle / result.latency_total1
+        result.MAC_utilization2 = result.ideal_cycle / result.latency_total2
+
+        for cme in (self, other):
+            if isinstance(cme, CostModelEvaluation):
+                result.layer_ids.append(cme.layer.id)
+                result.core_ids.append(cme.core_id)
+            elif isinstance(cme, CumulativeCME):
+                result.layer_ids += cme.layer_ids
+                result.core_ids += cme.core_ids
+
+        # Select accelerator for result
+        if isinstance(self, CumulativeCME) and self.accelerator is None:
+            assert other.accelerator is not None, "Accelerator undefined on both CMEs being added"
+            result.accelerator = other.accelerator
+        elif isinstance(other, CumulativeCME) and other.accelerator is None:
+            assert self.accelerator is not None, "Accelerator undefined on both CMEs being added"
+            result.accelerator = self.accelerator
+        elif self.accelerator is not None and other.accelerator is not None:
+            if self.accelerator.name.startswith(other.accelerator.name):
+                result.accelerator = other.accelerator
+            elif other.accelerator.name.startswith(self.accelerator.name):
+                result.accelerator = self.accelerator
+            else:
+                raise ValueError("Adding CMEs of unrelated accelerators")
 
-    def __repr__(self):
-        return str(self.served_op_lv_dir)
+        return result
 
+    def __mul__(self, number: float):
+        result: "CostModelEvaluationABC" = pickle_deepcopy(self)
 
-## Given a cost model evaluation and a memory instance, compute the memory's
-# total instantaneous bandwidth required throughout this layer's execution.
-# @param cme: CostModelEvaluation
-# @param memory_instance: MemoryInstance
-# @return total_inst_bw
-def get_total_inst_bandwidth(cme, memory_instance):
-    """
-    Get the instantaneous offchip bandwidth required throughout this layer's execution.
-    """
-    # Check which operands require offchip memory throughout the computation
-    offchip_mem_operands = []
-    for op, memory_levels in cme.mem_hierarchy_dict.items():
-        last_mem_level = memory_levels[-1]
-        if last_mem_level.memory_instance == memory_instance:
-            offchip_mem_operands.append(op)
-    # Obtain the required instantaneous bandwidth to/from offchip for these operands
-    total_inst_bw = FourWayDataMoving(0, 0, 0, 0)
-    for mem_op in offchip_mem_operands:
-        layer_op = next(
-            l_op
-            for l_op, m_op in cme.layer.memory_operand_links.items()
-            if m_op == mem_op
-        )
-        inst_bw_4way = cme.mapping.unit_mem_data_movement[layer_op][-1].req_mem_bw_inst
-        total_inst_bw += inst_bw_4way
-    return total_inst_bw
-
-
-## Given a certain operand's storage level (for example (A,1): operand A's 1st memory level),
-# return a list of the rest operand's storage levels that share physical memory with the former one (A1)
-# @param mem_op
-# @param mem_lv
-# @param memory_sharing_list
-# @return mem_share_grp
-def get_shared_mem_list(mem_op, mem_lv, memory_sharing_list) -> List[Tuple]:
-    for mem_share_group in memory_sharing_list:
-        mem_share_grp = list(mem_share_group.items())
-        mem_target = (mem_op, mem_lv)
-        if mem_target in mem_share_grp:
-            return mem_share_grp
-
-
-## Generate the integer spatial mapping from fractional spatial mapping (due to greedy mapping support).
-# Later the fractional one is used for calculating energy, and the integer one is used for calculating latency
-# @param spatial_mapping
-# @return spatial_mapping_int
-def spatial_mapping_fractional_to_int(spatial_mapping: Dict):
-    spatial_mapping_int = pickle_deepcopy(spatial_mapping)
-    for op, su_all_lv in spatial_mapping.items():
-        if not su_all_lv:
-            continue
-        for lv, su_one_level in enumerate(su_all_lv):
-            for idx, su in enumerate(su_one_level):
-                if type(su[1]) != int:
-                    spatial_mapping_int[op][lv][idx] = (su[0], ceil(su[1]))
-
-    return spatial_mapping_int
-
-
-##  This function calculates the union length of all the share-port MUW (memory updating window).
-#   The following encoding has to be used:
-#   - 'P' for single period length
-#   - 'A' for allowed MUW per period
-#   - 'PC' for period count within the whole layer computation
-#
-#   Pre-process the port_duty_list to generate input_dict, which looks like:
-#   - input_dict = {'O1': {'P': 3, 'A': 1, 'PC': 8}, 'O2': {'P': 6, 'A': 2, 'PC': 4}, 'O3': {'P': 12, 'A': 4, 'PC': 2}}
-#
-#   @param port_duty_list List of port activity objects
-#   @reutrn
-def calc_MUW_union(port_duty_list):
-
-    input_dict = {}
-    for port_duty in port_duty_list:
-        """as long as one of the port duty can make use of the whole computation time, the MUW union is set to
-        the whole computation time"""
-        if port_duty.period == port_duty.allowed_cycle:
-            return port_duty.period * port_duty.period_count
-        key = str(port_duty.served_op_lv_dir)
-        input_dict[key] = {
-            "P": port_duty.period,
-            "A": port_duty.allowed_cycle,
-            "PC": port_duty.period_count,
+        # Energy
+        result.MAC_energy *= number
+        result.mem_energy *= number
+        result.energy_total *= number
+
+        result.mem_energy_breakdown = {
+            op: [result.mem_energy_breakdown[op][i] * number for i in range(len(result.mem_energy_breakdown[op]))]
+            for op in result.mem_energy_breakdown.keys()
+        }
+        result.mem_energy_breakdown_further = {
+            op: [
+                result.mem_energy_breakdown_further[op][i] * number
+                for i in range(len(result.mem_energy_breakdown_further[op]))
+            ]
+            for op in result.mem_energy_breakdown_further.keys()
         }
 
-    max_period = 0
-    max_period_operand = None
-    for op in input_dict:
-        if input_dict[op]["P"] > max_period:
-            max_period = input_dict[op]["P"]
-            max_period_operand = op
-
-    indicators = np.zeros((len(input_dict), max_period), dtype=np.int8)
-    for i, op in enumerate(input_dict):
-        """reshape to period of this operand"""
-        indicators_reshape = indicators.reshape(
-            (len(input_dict), -1, input_dict[op]["P"])
+        # Memory access
+        result.memory_word_access = {
+            op: [result.memory_word_access[op][i] * number for i in range(len(result.memory_word_access[op]))]
+            for op in result.memory_word_access.keys()
+        }
+
+        # Latency
+        result.data_loading_cycle *= number
+        result.data_offloading_cycle *= number
+        result.ideal_cycle *= number
+        result.ideal_temporal_cycle *= number
+        result.latency_total0 *= number
+        result.latency_total1 *= number
+        result.latency_total2 *= number
+
+        # MAC utilization
+        result.MAC_spatial_utilization = result.ideal_cycle / result.ideal_temporal_cycle
+        result.MAC_utilization0 = result.ideal_cycle / result.latency_total0
+        result.MAC_utilization1 = result.ideal_cycle / result.latency_total1
+        result.MAC_utilization2 = result.ideal_cycle / result.latency_total2
+
+        return result
+
+    def __simplejsonrepr__(self) -> dict[str, float]:
+        """! Simple JSON representation used for saving this object to a simple json file."""
+        return {"energy": self.energy_total, "latency": self.latency_total2}
+
+    def __jsonrepr__(self):
+        """! JSON representation used for saving this object to a json file."""
+        return json_repr_handler(
+            {
+                "outputs": {
+                    "memory": {
+                        "utilization": (self.mem_utili_shared if isinstance(self, CostModelEvaluation) else None),
+                        "word_accesses": self.memory_word_access,
+                    },
+                    "energy": {
+                        "energy_total": self.energy_total,
+                        "operational_energy": self.MAC_energy,
+                        "memory_energy": self.mem_energy,
+                        "memory_energy_breakdown_per_level": self.mem_energy_breakdown,
+                        "memory_energy_breakdown_per_level_per_operand": self.mem_energy_breakdown_further,
+                    },
+                    "latency": {
+                        "data_onloading": self.latency_total1 - self.latency_total0,
+                        "computation": self.latency_total0,
+                        "data_offloading": self.latency_total2 - self.latency_total1,
+                    },
+                    "spatial": {
+                        "mac_utilization": {
+                            "ideal": self.MAC_spatial_utilization,
+                            "stalls": self.MAC_utilization0,
+                            "stalls_onloading": self.MAC_utilization1,
+                            "stalls_onloading_offloading": self.MAC_utilization2,
+                        }
+                    },
+                },
+                "inputs": {
+                    "accelerator": self.accelerator,
+                    "layer": (
+                        self.layer
+                        if isinstance(self, CostModelEvaluation)
+                        else self.layer_ids if isinstance(self, CumulativeCME) else None
+                    ),
+                    "spatial_mapping": (self.spatial_mapping_int if isinstance(self, CostModelEvaluation) else None),
+                    "temporal_mapping": (self.temporal_mapping if isinstance(self, CostModelEvaluation) else None),
+                },
+            }
         )
-        """ fill in first few time units as used """
-        indicators_reshape[i, :, : input_dict[op]["A"]] = 1
 
-    union = max_period - (~indicators.any(0)).sum(dtype=np.uint64)
 
-    # take sum across operands => how many operand need memory for every time unit
-    # Subtract 1 => number of stalls
-    # Clip by 0 (-1 is not -1 stall)
-    # Sum across time units (only remaining axis)
-    # stall = (indicators.sum(0, dtype=np.int8) - 1).clip(min=0).sum()
-
-    """ Multiply with number of periods of largest period (as it was normalized to largest period) """
-    return union * input_dict[max_period_operand]["PC"]
-
-
-## Class that stores inputs and runs them through the zigzag cost model.
-#
-# Initialize the cost model evaluation with the following inputs:
-# - accelerator: the accelerator that includes the core on which to run the layer
-# - layer: the layer to run
-# - spatial_mapping: the spatial mapping
-# - temporal_mapping: the temporal mapping
-#
-# From these parameters, the following attributes are computed:
-# * core: The core on which the layer is ran. This should be specified in the LayerNode attributes.
-# * mapping: The combined spatial and temporal mapping object where access patterns are computed.
-#
-# The following cost model attributes are also initialized:
-# - mem_energy_breakdown: The energy breakdown for all operands
-# - energy: The total energy
-#
-# After initialization, the cost model evaluation is run.
-class CostModelEvaluation:
-
-    ## The class constructor
-    # After initialization, the cost model evaluation is run
-    # @param accelerator the accelerator that includes the core on which to run the
-    # @param layer the layer to run
-    # @param spatial_mapping the spatial mapping
-    # @param temporal_mapping the temporal mapping
-    # @param access_same_data_considered_as_no_access (optional)
+class CumulativeCME(CostModelEvaluationABC):
+    """! Represents the sum of multiple CMEs. This class only contains attributes that make sense for cumulated CMEs"""
+
+    def __init__(self):
+        self.mem_energy_breakdown: dict[LayerOperand, list[float]] = dict()
+        self.mem_energy_breakdown_further: dict[LayerOperand, list[FourWayDataMoving]] = dict()
+        self.memory_word_access: dict[LayerOperand, list[FourWayDataMoving]] = dict()
+
+        self.layer_ids: list[int] = []
+        self.core_ids: list[int] = []
+
+        self.MAC_energy: float = 0.0
+        self.mem_energy: float = 0.0
+        self.energy_total: float = 0.0
+        self.data_loading_cycle: float = 0.0
+        self.data_offloading_cycle: float = 0.0
+        self.ideal_cycle: float = 0.0
+        self.ideal_temporal_cycle: float = 0.0
+        self.latency_total0: float = 0.0
+        self.latency_total1: float = 0.0
+        self.latency_total2: float = 0.0
+
+        self.accelerator = None
+
+
+class CostModelEvaluation(CostModelEvaluationABC):
+    """! Class that stores inputs and runs them through the zigzag cost model.
+
+    Initialize the cost model evaluation with the following inputs:
+    - accelerator: the accelerator that includes the core on which to run the layer
+    - layer: the layer to run
+    - spatial_mapping: the spatial mapping
+    - temporal_mapping: the temporal mapping
+
+    From these parameters, the following attributes are computed:
+    * core: The core on which the layer is ran. This should be specified in the LayerNode attributes.
+    * mapping: The combined spatial and temporal mapping object where access patterns are computed.
+
+    The following cost model attributes are also initialized:
+    - mem_energy_breakdown: The energy breakdown for all operands
+    - energy: The total energy
+
+    After initialization, the cost model evaluation is run.
+    """
+
     def __init__(
         self,
         *,
-        accelerator,
-        layer,
-        spatial_mapping,
-        spatial_mapping_int,
-        temporal_mapping,
-        access_same_data_considered_as_no_access=True,
+        accelerator: Accelerator,
+        layer: LayerNode,
+        spatial_mapping: SpatialMappingInternal,
+        spatial_mapping_int: SpatialMappingInternal,
+        temporal_mapping: TemporalMapping,
+        access_same_data_considered_as_no_access: bool = True,
     ):
-        self.accelerator = accelerator
-        self.layer = layer
+        """
+        After initialization, the cost model evaluation is run
+        @param accelerator the accelerator that includes the core on which to run the
+        @param layer the layer to run
+        @param access_same_data_considered_as_no_access (optional)
+        """
+        self.accelerator: Accelerator = accelerator  # type: ignore
+        self.layer: LayerNode = layer
         self.spatial_mapping = spatial_mapping
-        self.spatial_mapping_int = (
-            spatial_mapping_int  # the original spatial mapping without decimal
-        )
+        self.spatial_mapping_int = spatial_mapping_int  # the original spatial mapping without decimal
         self.temporal_mapping = temporal_mapping
-        self.access_same_data_considered_as_no_access = (
-            access_same_data_considered_as_no_access
-        )
+        self.access_same_data_considered_as_no_access = access_same_data_considered_as_no_access
 
-        self.core_id = layer.core_allocation
-        self.mem_level_list = (
-            accelerator.get_core(self.core_id).get_memory_hierarchy().mem_level_list
-        )
-        self.mem_hierarchy_dict = accelerator.get_core(
-            self.core_id
-        ).get_memory_hierarchy_dict()
-        self.mem_size_dict = accelerator.get_core(self.core_id).get_memory_size_dict()
-        self.mem_r_bw_dict, self.mem_w_bw_dict = accelerator.get_core(
-            self.core_id
-        ).get_memory_bw_dict()
-        self.mem_r_bw_min_dict, self.mem_w_bw_min_dict = accelerator.get_core(
-            self.core_id
-        ).get_memory_bw_min_dict()
-        self.mem_sharing_list = accelerator.get_core(
-            self.core_id
-        ).get_memory_sharing_list()
-        self.layer_op_to_mem_op = layer.memory_operand_links
-        self.mem_op_to_layer_op = dict(
-            [(value, key) for key, value in self.layer_op_to_mem_op.items()]
-        )
+        self.core_id = layer.core_allocation[0]
+        core = accelerator.get_core(self.core_id)
+        self.mem_level_list = core.memory_hierarchy.mem_level_list
+        self.mem_hierarchy_dict = core.mem_hierarchy_dict
+        self.mem_size_dict = core.mem_size_dict
+        self.mem_r_bw_dict, self.mem_w_bw_dict = core.get_memory_bw_dict()
+        self.mem_r_bw_min_dict, self.mem_w_bw_min_dict = core.get_memory_bw_min_dict()
+        self.mem_sharing_list = core.mem_sharing_list
+        self.memory_operand_links = layer.memory_operand_links
+
+        self.cumulative_layer_ids: list[int] = []  # In case the CME results from adding other CMEs together
+        self.cumulative_core_ids: list[int] = []
 
-        """ generate the integer spatial mapping from fractional spatial mapping (due to greedy mapping support).
-        Later the fractional one is used for calculating energy, and the integer one is used for calculating latency"""
-        # self.spatial_mapping_dict_int = spatial_mapping_fractional_to_int(
-        #     self.spatial_mapping.mapping_dict_origin
-        # )
+        # generate the integer spatial mapping from fractional spatial mapping (due to greedy mapping support).
+        # Later the fractional one is used for calculating energy, and the integer one is used for calculating latency
         self.spatial_mapping_dict_int = self.spatial_mapping_int.mapping_dict_origin
 
-        # For constructing Mapping object,  the last parameter "self.access_same_data_considered_as_no_access" is optional
         self.mapping = Mapping(
             self.accelerator,
             self.spatial_mapping,
             self.temporal_mapping,
             self.layer,
             self.access_same_data_considered_as_no_access,
         )
@@ -299,1121 +332,766 @@
         )
 
         self.active_mem_level = self.mapping.mem_level
 
         # Run the cost model evaluation
         self.run()
 
-    def __str__(self):
-        return f"CostModelEvaluation(layer={self.layer}, core={self.core_id})"
-
-    def __repr__(self):
-        return str(self)
-
-    # JSON representation used for saving this object to a json file.
-    def __jsonrepr__(self):
-        return {
-            "outputs": {
-                "memory": {
-                    "utilization": self.mem_utili_shared
-                    if hasattr(self, "mem_utili_shared")
-                    else None,
-                    "word_accesses": self.memory_word_access,
-                },
-                "energy": {
-                    "energy_total": self.energy_total,
-                    "operational_energy": self.MAC_energy,
-                    "memory_energy": self.mem_energy,
-                    "memory_energy_breakdown_per_level": self.mem_energy_breakdown,
-                    "memory_energy_breakdown_per_level_per_operand": self.mem_energy_breakdown_further,
-                },
-                "latency": {
-                    "data_onloading": self.latency_total1 - self.latency_total0,
-                    "computation": self.latency_total0,
-                    "data_offloading": self.latency_total2 - self.latency_total1,
-                },
-                "spatial": {
-                    "mac_utilization": {
-                        "ideal": self.MAC_spatial_utilization,
-                        "stalls": self.MAC_utilization0,
-                        "stalls_onloading": self.MAC_utilization1,
-                        "stalls_onloading_offloading": self.MAC_utilization2,
-                    }
-                },
-            },
-            "inputs": {
-                "accelerator": self.accelerator,
-                "layer": self.layer,
-                "spatial_mapping": self.spatial_mapping_int
-                if hasattr(self, "spatial_mapping_int")
-                else None,
-                "temporal_mapping": self.temporal_mapping
-                if hasattr(self, "temporal_mapping")
-                else None,
-            },
-        }
-
-    ## Simple JSON representation used for saving this object to a simple json file.
-    def __simplejsonrepr__(self):
-        return {"energy": self.energy_total, "latency": self.latency_total2}
-
-    ## Run the cost model evaluation.
-    def run(self):
+    def run(self) -> None:
+        """! Run the cost model evaluation."""
         self.calc_memory_utilization()
         self.calc_memory_word_access()
         self.calc_energy()
         self.calc_latency()
 
-    ## Calculate occupancy for each physical memory based on the mapping.
-    def calc_memory_utilization(self):
+    def __get_shared_mem_list(
+        self,
+        mem_op: MemoryOperand,
+        mem_lv: int,
+        memory_sharing_list: list[dict[MemoryOperand, int]],
+    ) -> list[tuple[MemoryOperand, int]] | None:
+        """! Given a certain operand's storage level (for example (A,1): operand A's 1st memory level),
+        return a list of the rest operand's storage levels that share physical memory with the former one (A1)
+        """
+        for mem_share_group in memory_sharing_list:
+            mem_share_grp = list(mem_share_group.items())
+            mem_target = (mem_op, mem_lv)
+            if mem_target in mem_share_grp:
+                return mem_share_grp
+
+    def __calc_MUW_union(self, port_duty_list: list[PortActivity]) -> int | float:
+        """!  This function calculates the union length of all the share-port MUW (memory updating window).
+        The following encoding has to be used:
+        - 'P' for single period length
+        - 'A' for allowed MUW per period
+        - 'PC' for period count within the whole layer computation
+
+        Pre-process the port_duty_list to generate input_dict, which looks like:
+        - input_dict = {'O1': {'P': 3, 'A': 1, 'PC': 8}, 'O2': {'P': 6, 'A': 2, 'PC': 4},
+        'O3': {'P': 12, 'A': 4, 'PC': 2}}
+        # TODO clean up
+        """
+
+        input_dict: dict[str, dict[str, int | float]] = {}
+        # As long as one of the port duty can make use of the whole computation time, the MUW union is
+        # set to the whole computation time
+        for port_duty in port_duty_list:
+            if port_duty.period == port_duty.allowed_cycle:
+                return port_duty.period * port_duty.period_count
+            key = str(port_duty.served_op_lv_dir)
+            input_dict[key] = {
+                "P": port_duty.period,
+                "A": port_duty.allowed_cycle,
+                "PC": port_duty.period_count,
+            }
+
+        max_period = 0
+        max_period_operand: str = ""
+        for op, values in input_dict.items():
+            if values["P"] > max_period:
+                max_period = values["P"]
+                max_period_operand = op
+
+        indicators: np.ndarray = np.zeros((len(input_dict), max_period), dtype=np.int8)
+        for i, op in enumerate(input_dict):
+            # reshape to period of this operand
+            indicators_reshape: np.ndarray = indicators.reshape((len(input_dict), -1, input_dict[op]["P"]))
+            # fill in first few time units as used
+            indicators_reshape[i, :, : input_dict[op]["A"]] = 1
+
+        union = max_period - (~indicators.any(0)).sum(dtype=np.uint64)
+
+        # take sum across operands => how many operand need memory for every time unit
+        # Subtract 1 => number of stalls
+        # Clip by 0 (-1 is not -1 stall)
+        # Sum across time units (only remaining axis)
+        # stall = (indicators.sum(0, dtype=np.int8) - 1).clip(min=0).sum()
+
+        # Multiply with number of periods of largest period (as it was normalized to largest period)
+        return union * input_dict[max_period_operand]["PC"]
+
+    def calc_memory_utilization(self) -> None:
+        """! Calculate occupancy for each physical memory based on the mapping."""
         # mem_utili_individual: the memory utilization of each operand individually.
         # mem_utili_shared: the memory utilization taking operand memory sharing into consideration.
-        mem_utili_individual = {}
-        effective_mem_utili_individual = {}
-        for layer_op in self.layer.operand_list:
+        mem_utili_individual: dict[LayerOperand, list[float]] = {}
+        effective_mem_utili_individual: dict[LayerOperand, list[float]] = {}
+        for layer_op in self.layer.layer_operands:
             mem_utili_individual[layer_op] = []
             effective_mem_utili_individual[layer_op] = []
             for mem_lv in range(self.active_mem_level[layer_op]):
                 mem_utilization = (
                     self.mapping.data_bit_per_level_unrolled[layer_op][mem_lv + 1]
-                    / self.mem_size_dict[self.layer_op_to_mem_op[layer_op]][mem_lv]
+                    / self.mem_size_dict[self.memory_operand_links.layer_to_mem_op(layer_op)][mem_lv]
                 )
                 assert mem_utilization <= 1, (
                     f"Operand {layer_op} memory level {mem_lv}'s individual memory utilization is "
                     f"{mem_utilization}, which is larger than 1 "
                     f"(memory level starts from 0)"
                 )
                 mem_utili_individual[layer_op].append(mem_utilization)
 
                 # if we do not count copied data in parallel memories as effective, what is the utilization then? =>
                 effective_mem_utilization = (
                     self.mapping.effective_data_bit[layer_op][mem_lv + 1]
-                    / self.mem_size_dict[self.layer_op_to_mem_op[layer_op]][mem_lv]
-                )
-                effective_mem_utili_individual[layer_op].append(
-                    effective_mem_utilization
+                    / self.mem_size_dict[self.memory_operand_links.layer_to_mem_op(layer_op)][mem_lv]
                 )
+                effective_mem_utili_individual[layer_op].append(effective_mem_utilization)
 
-        mem_utili_shared = pickle_deepcopy(mem_utili_individual)
-        effective_mem_utili_shared = pickle_deepcopy(effective_mem_utili_individual)
+        mem_utili_shared: dict[LayerOperand, list[float]] = pickle_deepcopy(mem_utili_individual)
+        effective_mem_utili_shared: dict[LayerOperand, list[float]] = pickle_deepcopy(effective_mem_utili_individual)
         for mem_share_dict in self.mem_sharing_list:
             mem_utilization = 0
             effective_mem_utilization = 0
             for mem_op, mem_lv in mem_share_dict.items():
-                try:
-                    layer_op = self.mem_op_to_layer_op[mem_op]
-                except:  # mem to layer op might not contain this mem op (e.g. pooling layer)
-                    continue
-                mem_utilization += mem_utili_individual[layer_op][mem_lv]
-                effective_mem_utilization += effective_mem_utili_individual[layer_op][
-                    mem_lv
-                ]
+                # mem to layer op might not contain this mem op (e.g. pooling layer)
+                if self.memory_operand_links.contains_mem_op(mem_op):
+                    layer_op = self.memory_operand_links.mem_to_layer_op(mem_op)
+                    mem_utilization += mem_utili_individual[layer_op][mem_lv]
+                    effective_mem_utilization += effective_mem_utili_individual[layer_op][mem_lv]
             assert mem_utilization <= 1, (
                 f"Memory shared by {mem_share_dict} (memory operand, memory level) has shared utilization of "
                 f"{mem_utilization}, which is > 1 "
                 f"(memory level starts from 0)."
             )
             for mem_op, mem_lv in mem_share_dict.items():
-                try:
-                    layer_op = self.mem_op_to_layer_op[mem_op]
-                except:  # mem to layer op might not contain this mem op (e.g. pooling layer)
-                    continue
-                mem_utili_shared[layer_op][mem_lv] = mem_utilization
-                effective_mem_utili_shared[layer_op][mem_lv] = effective_mem_utilization
+                if self.memory_operand_links.contains_mem_op(mem_op):
+                    layer_op = self.memory_operand_links.mem_to_layer_op(mem_op)
+                    mem_utili_shared[layer_op][mem_lv] = mem_utilization
+                    effective_mem_utili_shared[layer_op][mem_lv] = effective_mem_utilization
 
         self.mem_utili_individual = mem_utili_individual
         self.mem_utili_shared = mem_utili_shared
         self.effective_mem_utili_individual = effective_mem_utili_individual
         self.effective_mem_utili_shared = effective_mem_utili_shared
 
-    ## Calculates the memory word access based on unit memory's data element move count and the physical memory bw.
-    def calc_memory_word_access(self):
-        memory_word_access = {}
-        for layer_op in self.layer.operand_list:
+    def calc_memory_word_access(self) -> None:
+        """! Calculates the memory word access based on unit memory's data element move count and the physical
+        memory bw."""
+        memory_word_access: dict[LayerOperand, list[FourWayDataMoving]] = {}
+        for layer_op in self.layer.layer_operands:
             memory_word_access[layer_op] = []
             for mem_lv in range(self.mapping.mem_level[layer_op]):
-                """wr_in_by_low"""
-                data_elem_move_per_period = self.mapping.unit_mem_data_movement[
-                    layer_op
-                ][mem_lv].data_trans_amount_per_period.wr_in_by_low
-                data_precision = self.mapping.unit_mem_data_movement[layer_op][
+                # wr_in_by_low
+                data_elem_move_per_period = self.mapping.unit_mem_data_movement[layer_op][
                     mem_lv
-                ].data_precision.wr_in_by_low
+                ].data_trans_amount_per_period.wr_in_by_low
+                data_precision = self.mapping.unit_mem_data_movement[layer_op][mem_lv].data_precision.wr_in_by_low
                 if data_elem_move_per_period == 0 or data_precision == 0:
-                    wr_in_by_low = 0
+                    wr_in_by_low: int = 0
                 else:
                     total_period_count = self.mapping.unit_mem_data_movement[layer_op][
                         mem_lv
                     ].data_trans_period_count.wr_in_by_low
-                    max_bw = self.mem_w_bw_dict[self.layer_op_to_mem_op[layer_op]][
-                        mem_lv
-                    ]
-                    min_bw = self.mem_w_bw_min_dict[self.layer_op_to_mem_op[layer_op]][
-                        mem_lv
-                    ]
-                    if mem_lv > 0:
-                        another_side_bw = self.mem_r_bw_dict[
-                            self.layer_op_to_mem_op[layer_op]
-                        ][mem_lv - 1] * (
-                            self.spatial_mapping.unit_unique[layer_op][mem_lv]
-                            / self.spatial_mapping.unit_unique[layer_op][mem_lv + 1]
-                        )
-                        data_elem_move_per_cycle_in_a_period = min(
-                            (another_side_bw / data_precision),
-                            (max_bw / data_precision),
-                            data_elem_move_per_period,
-                        )
-                        cycle_in_a_period = ceil(
-                            data_elem_move_per_period
-                            / data_elem_move_per_cycle_in_a_period
-                        )
-                    else:
-                        data_elem_move_per_cycle_in_a_period = data_elem_move_per_period
-                        cycle_in_a_period = 1
-                    # wr_in_by_low = (
-                    #    ceil(
-                    #        (data_elem_move_per_cycle_in_a_period * data_precision)
-                    #        / min_bw
-                    #    )
-                    #    * (min_bw / max_bw)
-                    #    * total_period_count
-                    #    * cycle_in_a_period
-                    #    * self.mapping.spatial_mapping.unit_count[layer_op][mem_lv + 1]
-                    # )
-
-                    # 2023/06/30, solve the memory access granuarity issue - Jiacong Sun, Linyan Mei
-                    # Originally we used the cycle_in_a_period to compute the memory word access.
-                    # This neglected the finer-grained memory access possibility (the min_bw, the minimal memory access granuarity, like half-word access).
-                    # Now we changed to calculation based on min_bw.
-                    wr_in_by_low = (
+                    max_bw = self.mem_w_bw_dict[self.memory_operand_links.layer_to_mem_op(layer_op)][mem_lv]
+                    min_bw = self.mem_w_bw_min_dict[self.memory_operand_links.layer_to_mem_op(layer_op)][mem_lv]
+                    wr_in_by_low = int(
                         ceil((data_elem_move_per_period * data_precision) / min_bw)
                         * (min_bw / max_bw)
                         * total_period_count
                         * self.mapping.spatial_mapping.unit_count[layer_op][mem_lv + 1]
                     )
 
-                """ rd_out_to_low """
-                data_elem_move_per_period = self.mapping.unit_mem_data_movement[
-                    layer_op
-                ][mem_lv].data_trans_amount_per_period.rd_out_to_low
-                data_precision = self.mapping.unit_mem_data_movement[layer_op][
+                # rd_out_to_low
+                data_elem_move_per_period = self.mapping.unit_mem_data_movement[layer_op][
                     mem_lv
-                ].data_precision.rd_out_to_low
+                ].data_trans_amount_per_period.rd_out_to_low
+                data_precision = self.mapping.unit_mem_data_movement[layer_op][mem_lv].data_precision.rd_out_to_low
                 if data_elem_move_per_period == 0 or data_precision == 0:
-                    rd_out_to_low = 0
+                    rd_out_to_low: int = 0
                 else:
                     total_period_count = self.mapping.unit_mem_data_movement[layer_op][
                         mem_lv
                     ].data_trans_period_count.rd_out_to_low
-                    max_bw = self.mem_r_bw_dict[self.layer_op_to_mem_op[layer_op]][
-                        mem_lv
-                    ]
-                    min_bw = self.mem_r_bw_min_dict[self.layer_op_to_mem_op[layer_op]][
-                        mem_lv
-                    ]
-                    if mem_lv > 0:
-                        another_side_bw = self.mem_w_bw_dict[
-                            self.layer_op_to_mem_op[layer_op]
-                        ][mem_lv - 1] * (
-                            self.spatial_mapping.unit_unique[layer_op][mem_lv]
-                            / self.spatial_mapping.unit_unique[layer_op][mem_lv + 1]
-                        )
-                        data_elem_move_per_cycle_in_a_period = min(
-                            (another_side_bw / data_precision),
-                            (max_bw / data_precision),
-                            data_elem_move_per_period,
-                        )
-                        cycle_in_a_period = ceil(
-                            data_elem_move_per_period
-                            / data_elem_move_per_cycle_in_a_period
-                        )
-                        # rd_out_to_low = (
-                        #    ceil(
-                        #        (data_elem_move_per_cycle_in_a_period * data_precision)
-                        #        / min_bw
-                        #    )
-                        #    * (min_bw / max_bw)
-                        #    * total_period_count
-                        #    * cycle_in_a_period
-                        #    * self.mapping.spatial_mapping.unit_count[layer_op][
-                        #        mem_lv + 1
-                        #    ]
-                        # )
-                    # else:
-
-                    # 2023/06/30, solve the memory access granuarity issue - Jiacong Sun, Linyan Mei
-                    # Originally we used the cycle_in_a_period to compute the memory word access.
-                    # This neglected the finer-grained memory access possibility (the min_bw, the minimal memory access granuarity, like half-word access).
-                    # Now we changed to calculation based on min_bw.
-                    rd_out_to_low = (
+                    max_bw = self.mem_r_bw_dict[self.memory_operand_links.layer_to_mem_op(layer_op)][mem_lv]
+                    min_bw = self.mem_r_bw_min_dict[self.memory_operand_links.layer_to_mem_op(layer_op)][mem_lv]
+                    rd_out_to_low = int(
                         ceil((data_elem_move_per_period * data_precision) / min_bw)
                         * (min_bw / max_bw)
                         * total_period_count
                         * self.mapping.spatial_mapping.unit_count[layer_op][mem_lv + 1]
                     )
 
-                """ rd_out_to_high """
-                data_elem_move_per_period = self.mapping.unit_mem_data_movement[
-                    layer_op
-                ][mem_lv].data_trans_amount_per_period.rd_out_to_high
+                # rd_out_to_high
+                data_elem_move_per_period = self.mapping.unit_mem_data_movement[layer_op][
+                    mem_lv
+                ].data_trans_amount_per_period.rd_out_to_high
                 if data_elem_move_per_period == 0:
-                    rd_out_to_high = 0
+                    rd_out_to_high: int = 0
                 else:
-                    data_precision = self.mapping.unit_mem_data_movement[layer_op][
-                        mem_lv
-                    ].data_precision.rd_out_to_high
+                    data_precision = self.mapping.unit_mem_data_movement[layer_op][mem_lv].data_precision.rd_out_to_high
                     total_period_count = self.mapping.unit_mem_data_movement[layer_op][
                         mem_lv
                     ].data_trans_period_count.rd_out_to_high
-                    max_bw = self.mem_r_bw_dict[self.layer_op_to_mem_op[layer_op]][
-                        mem_lv
-                    ]
-                    min_bw = self.mem_r_bw_min_dict[self.layer_op_to_mem_op[layer_op]][
-                        mem_lv
-                    ]
-                    rd_out_to_high = (
+                    max_bw = self.mem_r_bw_dict[self.memory_operand_links.layer_to_mem_op(layer_op)][mem_lv]
+                    min_bw = self.mem_r_bw_min_dict[self.memory_operand_links.layer_to_mem_op(layer_op)][mem_lv]
+                    rd_out_to_high = int(
                         ceil((data_elem_move_per_period * data_precision) / min_bw)
                         * (min_bw / max_bw)
                         * total_period_count
                         * self.mapping.spatial_mapping.unit_count[layer_op][mem_lv + 1]
                     )
 
-                """ wr_in_by_high """
-                data_elem_move_per_period = self.mapping.unit_mem_data_movement[
-                    layer_op
-                ][mem_lv].data_trans_amount_per_period.wr_in_by_high
+                # wr_in_by_high
+                data_elem_move_per_period = self.mapping.unit_mem_data_movement[layer_op][
+                    mem_lv
+                ].data_trans_amount_per_period.wr_in_by_high
                 if data_elem_move_per_period == 0:
-                    wr_in_by_high = 0
+                    wr_in_by_high: int = 0
                 else:
-                    data_precision = self.mapping.unit_mem_data_movement[layer_op][
-                        mem_lv
-                    ].data_precision.wr_in_by_high
+                    data_precision = self.mapping.unit_mem_data_movement[layer_op][mem_lv].data_precision.wr_in_by_high
                     total_period_count = self.mapping.unit_mem_data_movement[layer_op][
                         mem_lv
                     ].data_trans_period_count.wr_in_by_high
-                    max_bw = self.mem_w_bw_dict[self.layer_op_to_mem_op[layer_op]][
-                        mem_lv
-                    ]
-                    min_bw = self.mem_w_bw_min_dict[self.layer_op_to_mem_op[layer_op]][
-                        mem_lv
-                    ]
-                    wr_in_by_high = (
+                    max_bw = self.mem_w_bw_dict[self.memory_operand_links.layer_to_mem_op(layer_op)][mem_lv]
+                    min_bw = self.mem_w_bw_min_dict[self.memory_operand_links.layer_to_mem_op(layer_op)][mem_lv]
+                    wr_in_by_high = int(
                         ceil((data_elem_move_per_period * data_precision) / min_bw)
                         * (min_bw / max_bw)
                         * total_period_count
                         * self.mapping.spatial_mapping.unit_count[layer_op][mem_lv + 1]
                     )
 
-                """ All """
+                # All
                 memory_word_access_single = FourWayDataMoving(
                     rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
                 )
                 memory_word_access[layer_op].append(memory_word_access_single)
 
         self.memory_word_access = memory_word_access
 
-    ## Calculates the energy cost of this cost model evaluation by calculating the memory reading/writing energy.
-    def calc_energy(self):
-        # - TODO: Interconnection energy
+    def calc_energy(self) -> None:
+        """! Calculates the energy cost of this cost model evaluation by calculating the memory reading/writing
+        energy."""
+        # TODO: Interconnection energy
         self.calc_MAC_energy_cost()
         self.calc_memory_energy_cost()
 
-    ## Calculate the dynamic MAC energy
-    def calc_MAC_energy_cost(self):
+    def calc_MAC_energy_cost(self) -> None:
+        """! Calculate the dynamic MAC energy"""
         core = self.accelerator.get_core(self.core_id)
         single_MAC_energy = core.operational_array.unit.cost
         self.MAC_energy = single_MAC_energy * self.layer.total_MAC_count
 
-    ## Computes the memories reading/writing energy by converting the access patterns in self.mapping to
-    # energy breakdown using the memory hierarchy of the core on which the layer is mapped.
-    #
-    # The energy breakdown is saved in self.mem_energy_breakdown.
-    #
-    # The energy total consumption is saved in self.energy_total.
     def calc_memory_energy_cost(self):
+        """! Computes the memories reading/writing energy by converting the access patterns in self.mapping to
+        energy breakdown using the memory hierarchy of the core on which the layer is mapped.
+
+        The energy breakdown is saved in self.mem_energy_breakdown.
+
+        The energy total consumption is saved in self.energy_total.
+        """
         core = self.accelerator.get_core(self.core_id)
         mem_hierarchy = core.memory_hierarchy
 
-        mem_energy_breakdown = {}
-        mem_energy_breakdown_further = {}
+        mem_energy_breakdown: dict[LayerOperand, list[float]] = {}
+        mem_energy_breakdown_further: dict[LayerOperand, list[FourWayDataMoving]] = {}
         energy_total = 0
-        for (layer_op, mem_access_list_per_op) in self.memory_word_access.items():
-            """Retrieve the memory levels in the hierarchy for this memory operand"""
-            mem_op = self.layer_op_to_mem_op[layer_op]
+
+        # Retrieve the memory levels in the hierarchy for this memory operand
+        for layer_op, mem_access_list_per_op in self.memory_word_access.items():
+            mem_op = self.memory_operand_links.layer_to_mem_op(layer_op)
             memory_levels = mem_hierarchy.get_memory_levels(mem_op=mem_op)
 
-            breakdown = (
-                []
-            )  # Stores the energy breakdown of a single layer operand (W, I, ...)
-            breakdown_further = []  # Stores
-            for (access_count, memory_level) in zip(
-                mem_access_list_per_op, memory_levels
-            ):
+            breakdown: list[float] = []  # Stores the energy breakdown of a single layer operand (W, I, ...)
+            breakdown_further: list[FourWayDataMoving] = []
+            for access_count, memory_level in zip(mem_access_list_per_op, memory_levels):
                 energy_cost_per_read_out = memory_level.read_energy
                 energy_cost_per_write_in = memory_level.write_energy
-                read_out_energy_to_above = access_count.get_total_read_outs_to_above(
+                read_out_energy_to_above: float = access_count.get_total_read_outs_to_above(
                     scaling=energy_cost_per_read_out
                 )
-                write_in_energy_from_above = (
-                    access_count.get_total_write_ins_from_above(
-                        scaling=energy_cost_per_write_in
-                    )
+                write_in_energy_from_above: float = access_count.get_total_write_ins_from_above(
+                    scaling=energy_cost_per_write_in
                 )
-                read_out_energy_to_below = access_count.get_total_read_outs_to_below(
+                read_out_energy_to_below: float = access_count.get_total_read_outs_to_below(
                     scaling=energy_cost_per_read_out
                 )
-                write_in_energy_from_below = (
-                    access_count.get_total_write_ins_from_below(
-                        scaling=energy_cost_per_write_in
-                    )
-                )
-                total_read_out_energy = (
-                    read_out_energy_to_above + read_out_energy_to_below
-                )
-                total_write_in_energy = (
-                    write_in_energy_from_above + write_in_energy_from_below
+                write_in_energy_from_below: float = access_count.get_total_write_ins_from_below(
+                    scaling=energy_cost_per_write_in
                 )
+                total_read_out_energy = read_out_energy_to_above + read_out_energy_to_below
+                total_write_in_energy = write_in_energy_from_above + write_in_energy_from_below
                 total_energy_cost_memory = total_read_out_energy + total_write_in_energy
-                breakdown.append(
-                    total_energy_cost_memory
-                )  # Here the breakdown only saves the total energy cost per memory level
+                # Here the breakdown only saves the total energy cost per memory level
+                breakdown.append(total_energy_cost_memory)
                 breakdown_further.append(
                     FourWayDataMoving(
                         read_out_energy_to_below,
                         write_in_energy_from_below,
                         read_out_energy_to_above,
                         write_in_energy_from_above,
                     )
-                )  # here it contains the full split
+                )
                 energy_total += total_energy_cost_memory
             mem_energy_breakdown[layer_op] = breakdown
             mem_energy_breakdown_further[layer_op] = breakdown_further
-        self.mem_energy_breakdown = mem_energy_breakdown
-        self.mem_energy_breakdown_further = mem_energy_breakdown_further
+        self.mem_energy_breakdown: dict[LayerOperand, list[float]] = mem_energy_breakdown
+        self.mem_energy_breakdown_further: dict[LayerOperand, list[FourWayDataMoving]] = mem_energy_breakdown_further
         self.mem_energy = energy_total
-        self.energy_total = self.mem_energy + self.MAC_energy
+        self.energy_total: float = self.mem_energy + self.MAC_energy
         logger.debug(f"Ran {self}. Total energy = {self.energy_total}")
 
-    ##  Calculate latency in 4 steps
-    #
-    # 1) As we already calculated the ideal data transfer rate in combined_mapping.py (in the Mapping class),
-    # here we start with calculating the required (or allowed) memory updating window by comparing the effective
-    # data size with the physical memory size at each level. If the effective data size is smaller than 50%
-    # of the physical memory size, then we take the whole period as the allowed memory updating window (double buffer effect);
-    # otherwise we take the the period divided by the top_ir_loop as the allowed memory updating window.
-    #
-    # 2) Then, we compute the real data transfer rate given the actual memory bw per functional port pair,
-    # assuming we have enough memory ports.
-    #
-    # 3) In reality, there is no infinite memory port to use. So, as the second step, we combine the real
-    # data transfer attributes per physical memory port.
-    #
-    # 4) Finally, we combine the stall/slack of each memory port to get the final latency.
-    def calc_latency(self):
+    def calc_latency(self) -> None:
+        """!  Calculate latency in 4 steps
+
+        1) As we already calculated the ideal data transfer rate in combined_mapping.py (in the Mapping class),
+        here we start with calculating the required (or allowed) memory updating window by comparing the effective
+        data size with the physical memory size at each level. If the effective data size is smaller than 50%
+        of the physical memory size, then we take the whole period as the allowed memory updating window
+        (double buffer effect);
+        otherwise we take the the period divided by the top_ir_loop as the allowed memory updating window.
+
+        2) Then, we compute the real data transfer rate given the actual memory bw per functional port pair,
+        assuming we have enough memory ports.
+
+        3) In reality, there is no infinite memory port to use. So, as the second step, we combine the real
+        data transfer attributes per physical memory port.
+
+        4) Finally, we combine the stall/slack of each memory port to get the final latency.
+        """
         self.calc_double_buffer_flag()
-        self.calc_allowed_and_real_data_transfer_cycle_per_DTL()
-        self.combine_data_transfer_rate_per_physical_port()
+        self.__calc_allowed_and_real_data_transfer_cycle_per_DTL()
+        self.__combine_data_transfer_rate_per_physical_port()
         self.calc_data_loading_offloading_latency()
         self.calc_overall_latency()
 
-    ## This function checks the double-buffer possibility for each operand at each memory level
-    # (minimal memory BW requirement case) by comparing the physical memory size with the effective
-    # data size, taking into account the memory sharing between operands.
-    def calc_double_buffer_flag(self):
-        double_buffer_true = {}
-        for layer_op in self.layer.operand_list:
-            mem_op = self.layer_op_to_mem_op[layer_op]
-            """ start with False for each operand at the lowest arch level (MAC array level) """
+    def calc_double_buffer_flag(self) -> None:
+        """! This function checks the double-buffer possibility for each operand at each memory level
+        (minimal memory BW requirement case) by comparing the physical memory size with the effective
+        data size, taking into account the memory sharing between operands.
+        """
+        double_buffer_true: dict[LayerOperand, list[bool]] = {}
+        for layer_op in self.layer.layer_operands:
+            mem_op = self.memory_operand_links.layer_to_mem_op(layer_op)
+            # start with False for each operand at the lowest arch level (MAC array level)
             double_buffer_true[layer_op] = [False]
             for mem_lv in range(0, self.mapping_int.mem_level[layer_op]):
                 if self.effective_mem_utili_shared[layer_op][mem_lv] <= 0.5:
                     double_buffer_true[layer_op].append(True)
                 elif (
                     self.effective_mem_utili_individual[layer_op][mem_lv]
                     <= 1 - self.effective_mem_utili_shared[layer_op][mem_lv]
                 ):
                     double_buffer_true[layer_op].append(True)
-                    shared_mem_list = get_shared_mem_list(
-                        mem_op, mem_lv, self.mem_sharing_list
-                    )
-                    """ When one of the operand in the shared memory get the "double-buffer" chance, 
-                    all operands of that shared memory level need to update the memory utilization 
-                    for later memory free space evaluation """
-                    for shared_mem_op, shared_mem_lv in shared_mem_list:
-                        try:
-                            shared_layer_op = self.mem_op_to_layer_op[shared_mem_op]
-                        except:  # mem op to layer op might not have this mem op (e.g. pooling layer)
-                            continue
-                        self.effective_mem_utili_shared[shared_layer_op][
-                            shared_mem_lv
-                        ] += self.effective_mem_utili_individual[layer_op][mem_lv]
+                    shared_mem_list = self.__get_shared_mem_list(mem_op, mem_lv, self.mem_sharing_list)
+                    # When one of the operand in the shared memory get the "double-buffer" chance,
+                    # all operands of that shared memory level need to update the memory utilization
+                    # for later memory free space evaluation
+                    if shared_mem_list is not None:
+                        for shared_mem_op, shared_mem_lv in shared_mem_list:
+                            if self.memory_operand_links.contains_mem_op(shared_mem_op):
+                                shared_layer_op = self.memory_operand_links.mem_to_layer_op(shared_mem_op)
+                                self.effective_mem_utili_shared[shared_layer_op][
+                                    shared_mem_lv
+                                ] += self.effective_mem_utili_individual[layer_op][mem_lv]
                 else:
                     double_buffer_true[layer_op].append(False)
 
         self.double_buffer_true = double_buffer_true
 
-    ## Construct a 4-way data transfer pattern for each unit mem, calculate
-    # {allowed_mem_updating_cycle, real_data_trans_cycle, DTL_SS_cycle} per period
-    def calc_allowed_and_real_data_transfer_cycle_per_DTL(self):
-        allowed_mem_updat_cycle = {}
-        real_data_trans_cycle = {}
-        """ stall (+) or slack (-) cycle within each period per virtual data transfer link (DTL) """
+    def __calc_allowed_and_real_data_transfer_cycle_per_DTL(self):
+        """! Construct a 4-way data transfer pattern for each unit mem, calculate
+        {allowed_mem_updating_cycle, real_data_trans_cycle, DTL_SS_cycle} per period
+        # TODO cleanup
+        """
+        allowed_mem_updat_cycle: dict[LayerOperand, list[FourWayDataMoving]] = dict()
+        real_data_trans_cycle: dict[LayerOperand, list[FourWayDataMoving]] = dict()
+        # stall (+) or slack (-) cycle within each period per virtual data transfer link (DTL)
         DTL_SS_cycle = {}
 
-        for layer_op in self.layer.operand_list:
+        for layer_op in self.layer.layer_operands:
             allowed_mem_updat_cycle[layer_op] = []
             real_data_trans_cycle[layer_op] = []
             DTL_SS_cycle[layer_op] = []
-            mem_op = self.layer_op_to_mem_op[layer_op]
+            mem_op = self.memory_operand_links.layer_to_mem_op(layer_op)
             for mem_lv in range(self.mapping_int.mem_level[layer_op]):
-                """======================================allowed_mem_updating_cycle(below)====================================="""
-                """ wr_in_by_low & rd_out_to_low"""
+                #  wr_in_by_low & rd_out_to_low
                 if self.double_buffer_true[layer_op][mem_lv]:
-                    wr_in_by_low_allowed = self.mapping_int.unit_mem_data_movement[
-                        layer_op
-                    ][mem_lv].data_trans_period.wr_in_by_low
-                    rd_out_to_low_allowed = self.mapping_int.unit_mem_data_movement[
-                        layer_op
-                    ][mem_lv].data_trans_period.rd_out_to_low
+                    wr_in_by_low_allowed = self.mapping_int.unit_mem_data_movement[layer_op][
+                        mem_lv
+                    ].data_trans_period.wr_in_by_low
+                    rd_out_to_low_allowed = self.mapping_int.unit_mem_data_movement[layer_op][
+                        mem_lv
+                    ].data_trans_period.rd_out_to_low
                 else:
-                    wr_in_by_low_allowed = self.mapping_int.unit_mem_data_movement[
-                        layer_op
-                    ][mem_lv].inst_data_trans_window.wr_in_by_low
-                    rd_out_to_low_allowed = self.mapping_int.unit_mem_data_movement[
-                        layer_op
-                    ][mem_lv].inst_data_trans_window.rd_out_to_low
+                    wr_in_by_low_allowed = self.mapping_int.unit_mem_data_movement[layer_op][
+                        mem_lv
+                    ].inst_data_trans_window.wr_in_by_low
+                    rd_out_to_low_allowed = self.mapping_int.unit_mem_data_movement[layer_op][
+                        mem_lv
+                    ].inst_data_trans_window.rd_out_to_low
 
-                """ wr_in_by_high & rd_out_to_high """
+                # #  wr_in_by_high & rd_out_to_high
                 if self.double_buffer_true[layer_op][mem_lv + 1]:
-                    wr_in_by_high_allowed = self.mapping_int.unit_mem_data_movement[
-                        layer_op
-                    ][mem_lv].data_trans_period.wr_in_by_high
-                    rd_out_to_high_allowed = self.mapping_int.unit_mem_data_movement[
-                        layer_op
-                    ][mem_lv].data_trans_period.rd_out_to_high
+                    wr_in_by_high_allowed = self.mapping_int.unit_mem_data_movement[layer_op][
+                        mem_lv
+                    ].data_trans_period.wr_in_by_high
+                    rd_out_to_high_allowed = self.mapping_int.unit_mem_data_movement[layer_op][
+                        mem_lv
+                    ].data_trans_period.rd_out_to_high
                 else:
-                    wr_in_by_high_allowed = self.mapping_int.unit_mem_data_movement[
-                        layer_op
-                    ][mem_lv].inst_data_trans_window.wr_in_by_high
-                    rd_out_to_high_allowed = self.mapping_int.unit_mem_data_movement[
-                        layer_op
-                    ][mem_lv].inst_data_trans_window.rd_out_to_high
+                    wr_in_by_high_allowed = self.mapping_int.unit_mem_data_movement[layer_op][
+                        mem_lv
+                    ].inst_data_trans_window.wr_in_by_high
+                    rd_out_to_high_allowed = self.mapping_int.unit_mem_data_movement[layer_op][
+                        mem_lv
+                    ].inst_data_trans_window.rd_out_to_high
 
-                """ All """
+                # All
                 updating_window = FourWayDataMoving(
                     rd_out_to_low_allowed,
                     wr_in_by_low_allowed,
                     rd_out_to_high_allowed,
                     wr_in_by_high_allowed,
                 )
                 allowed_mem_updat_cycle[layer_op].append(updating_window)
-                """ ======================================allowed_mem_updating_cycle(above)===================================== """
 
-                """ =========================================real_data_trans_cycle(below)======================================== """
-                """ wr_in_by_low """
-                data_precision = self.mapping_int.unit_mem_data_movement[layer_op][
-                    mem_lv
-                ].data_precision.wr_in_by_low
+                # wr_in_by_low
+                data_precision = self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_precision.wr_in_by_low
                 data_trans_amount = self.mapping_int.unit_mem_data_movement[layer_op][
                     mem_lv
                 ].data_trans_amount_per_period.wr_in_by_low
                 mem_bw = self.mem_w_bw_dict[mem_op][mem_lv]
                 wr_in_by_low_real = ceil(data_trans_amount * data_precision / mem_bw)
 
-                """ rd_out_to_low """
-                data_precision = self.mapping_int.unit_mem_data_movement[layer_op][
-                    mem_lv
-                ].data_precision.rd_out_to_low
+                #  rd_out_to_low
+                data_precision = self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_precision.rd_out_to_low
                 data_trans_amount = self.mapping_int.unit_mem_data_movement[layer_op][
                     mem_lv
                 ].data_trans_amount_per_period.rd_out_to_low
                 mem_bw = self.mem_r_bw_dict[mem_op][mem_lv]
                 rd_out_to_low_real = ceil(data_trans_amount * data_precision / mem_bw)
 
-                """ rd_out_to_high """
-                data_precision = self.mapping_int.unit_mem_data_movement[layer_op][
-                    mem_lv
-                ].data_precision.rd_out_to_high
+                #  rd_out_to_high
+                data_precision = self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_precision.rd_out_to_high
                 data_trans_amount = self.mapping_int.unit_mem_data_movement[layer_op][
                     mem_lv
                 ].data_trans_amount_per_period.rd_out_to_high
                 mem_bw = self.mem_r_bw_dict[mem_op][mem_lv]
                 rd_out_to_high_real = ceil(data_trans_amount * data_precision / mem_bw)
 
-                """ wr_in_by_high """
-                data_precision = self.mapping_int.unit_mem_data_movement[layer_op][
-                    mem_lv
-                ].data_precision.wr_in_by_high
+                #  wr_in_by_high
+                data_precision = self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_precision.wr_in_by_high
                 data_trans_amount = self.mapping_int.unit_mem_data_movement[layer_op][
                     mem_lv
                 ].data_trans_amount_per_period.wr_in_by_high
                 mem_bw = self.mem_w_bw_dict[mem_op][mem_lv]
                 wr_in_by_high_real = ceil(data_trans_amount * data_precision / mem_bw)
 
-                """ All """
+                # All
                 real_data_trans = FourWayDataMoving(
                     rd_out_to_low_real,
                     wr_in_by_low_real,
                     rd_out_to_high_real,
                     wr_in_by_high_real,
                 )
                 real_data_trans_cycle[layer_op].append(real_data_trans)
-                """ =========================================real_data_trans_cycle(above)======================================= """
 
         self.allowed_mem_updat_cycle = allowed_mem_updat_cycle
         self.real_data_trans_cycle = real_data_trans_cycle
 
-    ## Consider memory sharing and port sharing, combine the data transfer activity
-    # Step 1: collect port activity per memory instance per physical memory port
-    # Step 2: calculate SS combine and MUW union parameters per physical memory port
-    def combine_data_transfer_rate_per_physical_port(self):
+    def __combine_data_transfer_rate_per_physical_port(self) -> None:
+        """! Consider memory sharing and port sharing, combine the data transfer activity
+        Step 1: collect port activity per memory instance per physical memory port
+        Step 2: calculate SS combine and MUW union parameters per physical memory port
+        """
         # Step 1: collect port activity per memory instance per physical memory port
-        port_activity_collect = []
+        port_activity_collect: list[dict[str, list[PortActivity]]] = []
         for mem_instance in self.mem_level_list:
-            port_activity_single = {}
+            port_activity_single: dict[str, list[PortActivity]] = {}
             port_list = mem_instance.port_list
             for port in port_list:
                 port_activity_single[str(port)] = []
                 for mem_op, mem_lv, mov_dir in port.served_op_lv_dir:
-                    try:
-                        layer_op = self.mem_op_to_layer_op[mem_op]
-                    except:  # mem op to layer might not have this mem op (e.g. pooling layer)
-                        continue
-                    period_count = getattr(
-                        self.mapping_int.unit_mem_data_movement[layer_op][
+                    if self.memory_operand_links.contains_mem_op(mem_op):
+                        layer_op = self.memory_operand_links.mem_to_layer_op(mem_op)
+                        period_count = self.mapping_int.unit_mem_data_movement[layer_op][
                             mem_lv
-                        ].data_trans_period_count,
-                        mov_dir,
-                    )
-                    if period_count == 0:
-                        # skip the inactive data movement activities because they won't impact SS
-                        continue
-                    period = getattr(
-                        self.mapping_int.unit_mem_data_movement[layer_op][
+                        ].data_trans_period_count.get_single_dir_data(mov_dir)
+                        if period_count == 0:
+                            # skip the inactive data movement activities because they won't impact SS
+                            continue
+                        period = self.mapping_int.unit_mem_data_movement[layer_op][
                             mem_lv
-                        ].data_trans_period,
-                        mov_dir,
-                    )
-                    real_cycle = getattr(
-                        self.real_data_trans_cycle[layer_op][mem_lv], mov_dir
-                    )
-                    allowed_cycle = getattr(
-                        self.allowed_mem_updat_cycle[layer_op][mem_lv], mov_dir
-                    )
-                    port_activity = PortActivity(
-                        real_cycle,
-                        allowed_cycle,
-                        period,
-                        period_count,
-                        layer_op,
-                        mem_lv,
-                        mov_dir,
-                    )
-                    port_activity_single[str(port)].append(port_activity)
+                        ].data_trans_period.get_single_dir_data(mov_dir)
+                        real_cycle = self.real_data_trans_cycle[layer_op][mem_lv].get_single_dir_data(mov_dir)
+                        allowed_cycle = self.allowed_mem_updat_cycle[layer_op][mem_lv].get_single_dir_data(mov_dir)
+                        port_activity = PortActivity(
+                            real_cycle,
+                            allowed_cycle,
+                            period,
+                            period_count,
+                            layer_op,
+                            mem_lv,
+                            mov_dir,
+                        )
+                        port_activity_single[str(port)].append(port_activity)
             port_activity_collect.append(port_activity_single)
         self.port_activity_collect = port_activity_collect
 
         # Step 2: calculate SS combine and MUW union parameters per physical memory port
-        SS_comb_collect = [
-            {port: None for port in mem_ports} for mem_ports in port_activity_collect
+        SS_comb_collect: list[dict[str, int | float]] = [
+            {port: 0 for port in mem_ports} for mem_ports in port_activity_collect
         ]
-        SS_comb_list = [0]
+        SS_comb_list: list[int | float] = [0]
         # intermediate parameters saved for debugging purpose
-        MUW_union_collect = [
-            {port: None for port in mem_ports} for mem_ports in port_activity_collect
-        ]
+        MUW_union_collect: list[dict[str, int | float]] = [{} for _ in port_activity_collect]
 
         for idx, mem_ports in enumerate(port_activity_collect):
             for port_name, port_activity in mem_ports.items():
                 if len(port_activity) == 1:
                     MUW_union_collect[idx][port_name] = port_activity[0].allowed_cycle
                     SS_comb_collect[idx][port_name] = port_activity[0].SS
                     SS_comb_list.append(port_activity[0].SS)
                 elif len(port_activity) != 0:
-                    MUW_union_collect[idx][port_name] = calc_MUW_union(port_activity)
+                    MUW_union_collect[idx][port_name] = self.__calc_MUW_union(port_activity)
                     SS_positive_sum = 0
                     SS_negative_sum = 0
                     MUW_sum = 0
                     for port_d in port_activity:
                         if port_d.SS > 0:
                             SS_positive_sum += port_d.SS
                         else:
                             SS_negative_sum += port_d.SS
                         MUW_sum += port_d.MUW
-                    SS_comb = SS_positive_sum + max(
-                        0, SS_negative_sum + MUW_sum - MUW_union_collect[idx][port_name]
-                    )
+                    SS_comb = SS_positive_sum + max(0, SS_negative_sum + MUW_sum - MUW_union_collect[idx][port_name])
                     SS_comb_collect[idx][port_name] = SS_comb
                     SS_comb_list.append(SS_comb)
 
         self.MUW_union_collect = MUW_union_collect
         self.SS_comb_collect = SS_comb_collect
         # Assuming all the memory ports can work in parallel
         self.SS_comb = max(SS_comb_list)
 
-    ## Calculate the initial/final data loading/off-loading cycle by separating out
-    # the first-time input operands' / the last-time output operand's data movement
-    # on corresponding ports.
     def calc_data_loading_offloading_latency(self):
+        """! Calculate the initial/final data loading/off-loading cycle by separating out
+        the first-time input operands' / the last-time output operand's data movement
+        on corresponding ports.
+        """
         # Collect ports' initial data-loading and final data-offloading activities
-        data_loading_per_mem_inst = []
-        data_loading_cc_per_op = {op: {} for op in self.layer.input_operands}
-        data_offloading_per_mem_inst = []
-        data_offloading_cc_per_op = {}
-        for mem_inst_idx, mem_instance in enumerate(self.mem_level_list):
-            data_loading_single = {}
-            data_offloading_single = {}
+        data_loading_per_mem_inst: list[dict[str, list[PortBeginOrEndActivity]]] = []
+        data_loading_cc_per_op: dict[LayerOperand, dict[str, tuple[int | float, bool]]] = {
+            op: {} for op in self.layer.input_operands
+        }
+        data_offloading_per_mem_inst: list[dict[str, list[PortBeginOrEndActivity]]] = []
+        data_offloading_cc_per_op: dict[str, int | float] = {}
+        for mem_instance in self.mem_level_list:
+            data_loading_single: dict[str, list[PortBeginOrEndActivity]] = {}
+            data_offloading_single: dict[str, list[PortBeginOrEndActivity]] = {}
             port_list = mem_instance.port_list
             for port in port_list:
                 data_loading_single[str(port)] = []
                 data_offloading_single[str(port)] = []
                 served_operands = set(
-                    s[0] for s in port.served_op_lv_dir if s[0] in ["I1", "I2"]
+                    s[0] for s in port.served_op_lv_dir if s[0] in [Constants.MEM_OP_1, Constants.MEM_OP_2]
                 )
                 port_is_shared_by_two_input_operands = len(served_operands) > 1
                 for mem_op, mem_lv, mov_dir in port.served_op_lv_dir:
-                    try:
-                        layer_op = self.mem_op_to_layer_op[mem_op]
-                    except:  # mem op to layer op might not have this mem op (e.g. pooling layer)
-                        continue
-                    period_count = getattr(
-                        self.mapping_int.unit_mem_data_movement[layer_op][
+                    if self.memory_operand_links.contains_mem_op(mem_op):
+                        layer_op = self.memory_operand_links.mem_to_layer_op(mem_op)
+                        period_count = self.mapping_int.unit_mem_data_movement[layer_op][
                             mem_lv
-                        ].data_trans_period_count,
-                        mov_dir,
-                    )
-                    if period_count == 0:
-                        # skip for the inactive data movement
-                        continue
-                    if mem_op in ["I1", "I2"]:
-                        real_cycle = getattr(
-                            self.real_data_trans_cycle[layer_op][mem_lv], mov_dir
-                        )
-                        data_in_charge = getattr(
-                            self.mapping_int.unit_mem_data_movement[layer_op][
+                        ].data_trans_period_count.get_single_dir_data(mov_dir)
+                        if period_count == 0:
+                            # skip for the inactive data movement
+                            continue
+                        if mem_op in [Constants.MEM_OP_1, Constants.MEM_OP_2]:
+                            real_cycle = self.real_data_trans_cycle[layer_op][mem_lv].get_single_dir_data(mov_dir)
+                            data_in_charge = self.mapping_int.unit_mem_data_movement[layer_op][
                                 mem_lv
-                            ].data_trans_amount_per_period,
-                            mov_dir,
-                        ) * getattr(
-                            self.mapping_int.unit_mem_data_movement[layer_op][
+                            ].data_trans_amount_per_period.get_single_dir_data(
+                                mov_dir
+                            ) * self.mapping_int.unit_mem_data_movement[
+                                layer_op
+                            ][
                                 mem_lv
-                            ].data_precision,
-                            mov_dir,
-                        )
-                        if mov_dir[:2] == "rd":
-                            mem_bw = self.mem_r_bw_dict[mem_op][mem_lv]
+                            ].data_precision.get_single_dir_data(
+                                mov_dir
+                            )
+                            if mov_dir == DataDirection.RD_OUT_TO_HIGH or mov_dir == DataDirection.RD_OUT_TO_LOW:
+                                mem_bw = self.mem_r_bw_dict[mem_op][mem_lv]
+                            else:
+                                mem_bw = self.mem_w_bw_dict[mem_op][mem_lv]
+                            port_activity = PortBeginOrEndActivity(
+                                real_cycle,
+                                data_in_charge,
+                                mem_bw,
+                                layer_op,
+                                mem_lv,
+                                mov_dir,
+                            )
+                            data_loading_single[str(port)].append(port_activity)
+                            data_loading_cc_per_op[layer_op][layer_op.name + str(mem_lv) + "_" + str(mov_dir)] = (
+                                real_cycle,
+                                port_is_shared_by_two_input_operands,
+                            )
                         else:
-                            mem_bw = self.mem_w_bw_dict[mem_op][mem_lv]
-                        port_activity = PortBeginOrEndActivity(
-                            real_cycle,
-                            data_in_charge,
-                            mem_bw,
-                            layer_op,
-                            mem_lv,
-                            mov_dir,
-                        )
-                        data_loading_single[str(port)].append(port_activity)
-                        data_loading_cc_per_op[layer_op][
-                            layer_op + str(mem_lv) + "_" + mov_dir
-                        ] = (real_cycle, port_is_shared_by_two_input_operands)
-                    else:
-                        if mov_dir in ["rd_out_to_low", "wr_in_by_high"]:
-                            # don't consider partial sum flowing in the final data off-loading stage
-                            continue
-                        real_cycle = getattr(
-                            self.real_data_trans_cycle[layer_op][mem_lv], mov_dir
-                        )
-                        data_in_charge = getattr(
-                            self.mapping_int.unit_mem_data_movement[layer_op][
+                            if mov_dir == DataDirection.RD_OUT_TO_LOW or mov_dir == DataDirection.WR_IN_BY_HIGH:
+                                # don't consider partial sum flowing in the final data off-loading stage
+                                continue
+                            real_cycle = self.real_data_trans_cycle[layer_op][mem_lv].get_single_dir_data(mov_dir)
+                            data_in_charge = self.mapping_int.unit_mem_data_movement[layer_op][
                                 mem_lv
-                            ].data_trans_amount_per_period,
-                            mov_dir,
-                        ) * getattr(
-                            self.mapping_int.unit_mem_data_movement[layer_op][
+                            ].data_trans_amount_per_period.get_single_dir_data(
+                                mov_dir
+                            ) * self.mapping_int.unit_mem_data_movement[
+                                layer_op
+                            ][
                                 mem_lv
-                            ].data_precision,
-                            mov_dir,
-                        )
-                        if mov_dir[:2] == "rd":
-                            mem_bw = self.mem_r_bw_dict[mem_op][mem_lv]
-                        else:
-                            mem_bw = self.mem_w_bw_dict[mem_op][mem_lv]
-                        port_activity = PortBeginOrEndActivity(
-                            real_cycle,
-                            data_in_charge,
-                            mem_bw,
-                            layer_op,
-                            mem_lv,
-                            mov_dir,
-                        )
-                        data_offloading_single[str(port)].append(port_activity)
-                        data_offloading_cc_per_op[
-                            layer_op + str(mem_lv) + "_" + mov_dir
-                        ] = real_cycle
+                            ].data_precision.get_single_dir_data(
+                                mov_dir
+                            )
+                            if mov_dir == DataDirection.RD_OUT_TO_HIGH:
+                                mem_bw = self.mem_r_bw_dict[mem_op][mem_lv]
+                            else:
+                                mem_bw = self.mem_w_bw_dict[mem_op][mem_lv]
+
+                            port_activity = PortBeginOrEndActivity(
+                                real_cycle,
+                                data_in_charge,
+                                mem_bw,
+                                layer_op,
+                                mem_lv,
+                                mov_dir,
+                            )
+                            data_offloading_single[str(port)].append(port_activity)
+                            data_offloading_cc_per_op[layer_op.name + str(mem_lv) + "_" + str(mov_dir)] = real_cycle
 
             data_loading_per_mem_inst.append(data_loading_single)
             data_offloading_per_mem_inst.append(data_offloading_single)
         self.data_loading_per_mem_inst = data_loading_per_mem_inst
         self.data_loading_cc_per_op = data_loading_cc_per_op
         self.data_offloading_per_mem_inst = data_offloading_per_mem_inst
         self.data_offloading_per_op = data_offloading_cc_per_op
 
         # Combine ports' initial data-loading activities to get the data loading cycle amount
-        data_loading_cc_pair_combined_per_op = {
+        data_loading_cc_pair_combined_per_op: dict[LayerOperand, list[int | float]] = {
             op: [] for op in self.layer.input_operands
         }
-        data_loading_individual_part = {op: 0 for op in self.layer.input_operands}
-        data_loading_half_shared_part = {op: 0 for op in self.layer.input_operands}
-        data_loading_shared_part = {op: 0 for op in self.layer.input_operands}
+        data_loading_individual_part: dict[LayerOperand, int | float] = {op: 0 for op in self.layer.input_operands}
+        data_loading_half_shared_part: dict[LayerOperand, int | float] = {op: 0 for op in self.layer.input_operands}
+        data_loading_shared_part: dict[LayerOperand, int | float] = {op: 0 for op in self.layer.input_operands}
         for layer_op in self.layer.input_operands:
             for mem_lv in range(self.active_mem_level[layer_op] - 1):
                 elem1 = data_loading_cc_per_op[layer_op][
-                    layer_op + str(mem_lv) + "_" + "wr_in_by_high"
+                    layer_op.name + str(mem_lv) + "_" + str(DataDirection.WR_IN_BY_HIGH)
                 ]
                 elem2 = data_loading_cc_per_op[layer_op][
-                    layer_op + str(mem_lv + 1) + "_" + "rd_out_to_low"
+                    layer_op.name + str(mem_lv + 1) + "_" + str(DataDirection.RD_OUT_TO_LOW)
                 ]
                 completely_shared = elem1[1] and elem2[1]
                 completely_separate = not (elem1[1]) and not (elem2[1])
                 longest_loading_cc = max(elem1[0], elem2[0])
                 # for the ports that serve the same data movement purpose, take the longest data loading cycle
                 data_loading_cc_pair_combined = longest_loading_cc
-                data_loading_cc_pair_combined_per_op[layer_op].append(
-                    data_loading_cc_pair_combined
-                )
+                data_loading_cc_pair_combined_per_op[layer_op].append(data_loading_cc_pair_combined)
                 if completely_separate:
                     data_loading_individual_part[layer_op] += longest_loading_cc
                 elif completely_shared:
                     data_loading_shared_part[layer_op] += longest_loading_cc
                 else:
                     # the data transfer link between two memory levels is half-shared,
                     # i.e. on one memory side, the port is shared, while on another memory side,
                     # there are different memories with separate ports
                     data_loading_half_shared_part[layer_op] = longest_loading_cc
 
         if len(self.layer.input_operands) == 1:
-            data_loading_cycle = data_loading_individual_part[
-                self.layer.input_operands[0]
-            ]
+            data_loading_cycle = data_loading_individual_part[self.layer.input_operands[0]]
         else:
             op1 = self.layer.input_operands[0]
             op2 = self.layer.input_operands[1]
             possible1 = data_loading_shared_part[op1] + max(
-                data_loading_shared_part[op2]
-                + data_loading_half_shared_part[op2]
-                + data_loading_individual_part[op2],
+                data_loading_shared_part[op2] + data_loading_half_shared_part[op2] + data_loading_individual_part[op2],
                 data_loading_half_shared_part[op1] + data_loading_individual_part[op1],
             )
             possible2 = data_loading_shared_part[op2] + max(
-                data_loading_shared_part[op1]
-                + data_loading_half_shared_part[op1]
-                + data_loading_individual_part[op1],
+                data_loading_shared_part[op1] + data_loading_half_shared_part[op1] + data_loading_individual_part[op1],
                 data_loading_half_shared_part[op2] + data_loading_individual_part[op2],
             )
             data_loading_cycle = min(possible1, possible2)
 
         self.data_loading_cc_pair_combined_per_op = data_loading_cc_pair_combined_per_op
         self.data_loading_individual_part = data_loading_individual_part
         self.data_loading_half_shared_part = data_loading_half_shared_part
         self.data_loading_shared_part = data_loading_shared_part
         self.data_loading_cycle = data_loading_cycle
 
         # Combine ports' final data-offloading activities to get the data offloading cycle amount
         # TODO Only considered the worst case for now
         #  (assumed that all the ports are working in series during the final data off-loading phase)
-        data_offloading_cc_pair_combined = []
+        data_offloading_cc_pair_combined: list[int | float] = []
         layer_op = self.layer.output_operand
         for mem_lv in range(self.active_mem_level[layer_op] - 1):
-            elem1 = data_offloading_cc_per_op[
-                layer_op + str(mem_lv) + "_" + "rd_out_to_high"
-            ]
-            elem2 = data_offloading_cc_per_op[
-                layer_op + str(mem_lv + 1) + "_" + "wr_in_by_low"
-            ]
+            elem1 = data_offloading_cc_per_op[layer_op.name + str(mem_lv) + "_" + str(DataDirection.RD_OUT_TO_HIGH)]
+            elem2 = data_offloading_cc_per_op[layer_op.name + str(mem_lv + 1) + "_" + str(DataDirection.WR_IN_BY_LOW)]
             longest_offloading_cc = max(elem1, elem2)
             # for the ports that serve the same data movement purpose, take the longest data loading cycle
             data_offloading_cc_pair_combined.append(longest_offloading_cc)
         data_offloading_cycle = sum(data_offloading_cc_pair_combined)
 
         self.data_offloading_cc_pair_combined = data_offloading_cc_pair_combined
         self.data_offloading_cycle = data_offloading_cycle
 
-    ## This function integrates the previous calculated SScomb, data loading and off-loading cycle to get the overall latency
-    def calc_overall_latency(self, cycles_per_mac=1):
+    def calc_overall_latency(self, cycles_per_mac: int = 1) -> None:
+        """! This function integrates the previous calculated SScomb, data loading and off-loading cycle to get the
+        overall latency"""
         # @param cycles_per_mac: cycle counts per mac operand (>1 for bit-serial computation)
         # the ideal cycle count assuming the MAC array is 100% utilized
-        ideal_cycle = ceil(
-            self.layer.total_MAC_count
-            / self.accelerator.get_core(self.core_id).operational_array.total_unit_count
-        ) * cycles_per_mac
+        ideal_cycle = int(
+            ceil(
+                self.layer.total_MAC_count / self.accelerator.get_core(self.core_id).operational_array.total_unit_count
+            )
+            * cycles_per_mac
+        )
 
         # the ideal temporal cycle count given the spatial mapping (the spatial mapping can be non-ideal)
         ideal_temporal_cycle = self.mapping_int.temporal_mapping.total_cycle * cycles_per_mac
         MAC_spatial_utilization = ideal_cycle / ideal_temporal_cycle
 
         # Total latency without the initial data loading and the final data off-loading
         latency_total0 = ideal_temporal_cycle + self.SS_comb
         MAC_utilization0 = ideal_cycle / latency_total0
 
         # Total latency with the initial data loading, but without the final data off-loading
         latency_total1 = ideal_temporal_cycle + self.SS_comb + self.data_loading_cycle
         MAC_utilization1 = ideal_cycle / latency_total1
 
         # Total latency with both the initial data loading and the final data off-loading
-        latency_total2 = (
-            ideal_temporal_cycle
-            + self.SS_comb
-            + self.data_loading_cycle
-            + self.data_offloading_cycle
-        )
+        latency_total2 = ideal_temporal_cycle + self.SS_comb + self.data_loading_cycle + self.data_offloading_cycle
         MAC_utilization2 = ideal_cycle / latency_total2
 
         self.ideal_cycle = ideal_cycle
         self.ideal_temporal_cycle = ideal_temporal_cycle
         self.MAC_spatial_utilization = MAC_spatial_utilization
         self.latency_total0 = latency_total0
         self.latency_total1 = latency_total1
         self.latency_total2 = latency_total2
         self.MAC_utilization0 = MAC_utilization0
         self.MAC_utilization1 = MAC_utilization1
         self.MAC_utilization2 = MAC_utilization2
 
-    def __add__(self, other):
-        sum = pickle_deepcopy(self)
-
-        ## Energy
-        sum.MAC_energy += other.MAC_energy
-        sum.mem_energy += other.mem_energy
-        for op in sum.mem_energy_breakdown.keys():
-            if op in other.mem_energy_breakdown.keys():
-                l = []
-                for i in range(
-                    min(len(self.mem_energy_breakdown[op]), len(other.mem_energy_breakdown[op]))
-                ):
-                    l.append(
-                        self.mem_energy_breakdown[op][i] + other.mem_energy_breakdown[op][i]
-                    )
-                i = min(len(self.mem_energy_breakdown[op]), len(other.mem_energy_breakdown[op]))
-                l += self.mem_energy_breakdown[op][i:]
-                l += other.mem_energy_breakdown[op][i:]
-                sum.mem_energy_breakdown[op] = l
-
-        for op in sum.mem_energy_breakdown_further.keys():
-            if op in other.mem_energy_breakdown_further.keys():
-                l = []
-                for i in range(
-                    min(
-                        len(self.mem_energy_breakdown_further[op]),
-                        len(other.mem_energy_breakdown_further[op]),
-                    )
-                ):
-                    l.append(
-                        self.mem_energy_breakdown_further[op][i]
-                        + other.mem_energy_breakdown_further[op][i]
-                    )
-                i = min(
-                    len(self.mem_energy_breakdown_further[op]),
-                    len(other.mem_energy_breakdown_further[op]),
-                )
-                l += self.mem_energy_breakdown_further[op][i:]
-                l += other.mem_energy_breakdown_further[op][i:]
-                sum.mem_energy_breakdown_further[op] = l
-
-        # Get all the operands from other that are not in self and add them to the energy breakdown as well
-        op_diff = set(other.mem_energy_breakdown.keys()) - set(self.mem_energy_breakdown.keys())
-        for op in op_diff:
-            sum.mem_energy_breakdown[op] = other.mem_energy_breakdown[op]
-            sum.mem_energy_breakdown_further[op] = other.mem_energy_breakdown_further[op]
-
-        sum.energy_total += other.energy_total
-
-        ## Memory access
-        for op in sum.memory_word_access.keys():
-            if op in other.memory_word_access.keys():
-                l = []
-                for i in range(
-                    min(
-                        len(self.memory_word_access[op]),
-                        len(other.memory_word_access[op]),
-                    )
-                ):
-                    l.append(
-                        self.memory_word_access[op][i] + other.memory_word_access[op][i]
-                    )
-                i = min(
-                    len(self.memory_word_access[op]), len(other.memory_word_access[op])
-                )
-                l += self.memory_word_access[op][i:]
-                l += other.memory_word_access[op][i:]
-                sum.memory_word_access[op] = l
-        for op in op_diff:
-            sum.memory_word_access[op] = other.memory_word_access[op]
-
-        ## Latency
-        sum.data_loading_cycle += other.data_loading_cycle
-        sum.data_offloading_cycle += other.data_offloading_cycle
-        sum.ideal_cycle += other.ideal_cycle
-        sum.ideal_temporal_cycle += other.ideal_temporal_cycle  # ideal computation cycles without stalling
-        sum.latency_total0 += other.latency_total0
-        sum.latency_total1 += other.latency_total1
-        sum.latency_total2 += other.latency_total2
-
-        ## MAC utilization
-        sum.MAC_spatial_utilization = sum.ideal_cycle / sum.ideal_temporal_cycle
-        sum.MAC_utilization0 = sum.ideal_cycle / sum.latency_total0
-        sum.MAC_utilization1 = sum.ideal_cycle / sum.latency_total1
-        sum.MAC_utilization2 = sum.ideal_cycle / sum.latency_total2
-
-        ## layer
-        if type(sum.layer) != list:
-            sum.layer = [sum.layer.id]
-        if type(other.layer) != list:
-            other_layer = [other.layer.id]
-        sum.layer += other_layer
-
-        ## core_id
-        if type(sum.core_id) != list:
-            sum.core_id = [sum.core_id]
-        if type(other.layer) != list:
-            other_core_id = [other.core_id]
-        sum.core_id += other_core_id
-
-        ## Not addable
-        func = [
-            "calc_allowed_and_real_data_transfer_cycle_per_DTL",
-            "calc_data_loading_offloading_latency",
-            "calc_double_buffer_flag",
-            "calc_overall_latency",
-            "calc_MAC_energy_cost",
-            "calc_energy",
-            "calc_latency",
-            "calc_memory_energy_cost",
-            "calc_memory_utilization",
-            "calc_memory_word_access",
-            "combine_data_transfer_rate_per_physical_port",
-            "run",
-        ]
-        add_attr = [
-            "MAC_energy",
-            "mem_energy",
-            "mem_energy_breakdown",
-            "mem_energy_breakdown_further",
-            "energy_total",
-            "memory_word_access",
-            "data_loading_cycle",
-            "data_offloading_cycle",
-            "ideal_cycle",
-            "ideal_temporal_cycle",
-            "latency_total0",
-            "latency_total1",
-            "latency_total2",
-            "MAC_spatial_utilization",
-            "MAC_utilization0",
-            "MAC_utilization1",
-            "MAC_utilization2",
-            "layer",
-            "core_id",
-        ]
-
-        if hasattr(self, "accelerator") and hasattr(other, "accelerator"):
-            if self.accelerator.name.startswith(other.accelerator.name):
-                sum.accelerator = other.accelerator
-                add_attr.append("accelerator")
-            elif other.accelerator.name.startswith(self.accelerator.name):
-                add_attr.append("accelerator")
-        else:
-            pass
-
-        for attr in dir(sum):
-            if attr not in (func + add_attr) and attr[0] != "_":
-                delattr(sum, attr)
-
-        return sum
+    def get_total_inst_bandwidth(self, memory_instance: MemoryInstance) -> FourWayDataMoving:
+        """Given a cost model evaluation and a memory instance, compute the memory's total instantaneous bandwidth
+        required throughout the execution of the layer that corresponds to this CME. Returns empty bandwidth
+        requirements if the given memory instance is not included in this CME's memory hierarchy.
+        NOTE: this function is used in Stream
+        """
+        # Check which operands require offchip memory throughout the computation
+        offchip_mem_operands: list[MemoryOperand] = []
+        for op, memory_levels in self.mem_hierarchy_dict.items():
+            last_mem_level = memory_levels[-1]
+            if last_mem_level.memory_instance == memory_instance:
+                offchip_mem_operands.append(op)
+        # Obtain the required instantaneous bandwidth to/from offchip for these operands
+        total_inst_bw = FourWayDataMoving(0, 0, 0, 0)
+        for mem_op in offchip_mem_operands:
+            layer_op = self.layer.memory_operand_links.mem_to_layer_op(mem_op)
+            inst_bw_4way = self.mapping.unit_mem_data_movement[layer_op][-1].req_mem_bw_inst
+            total_inst_bw += inst_bw_4way
+        return total_inst_bw
 
-    def __mul__(self, number):
-        mul = pickle_deepcopy(self)
-
-        # Energy
-        mul.MAC_energy *= number
-        mul.mem_energy *= number
-        mul.mem_energy_breakdown = {
-            op: [
-                mul.mem_energy_breakdown[op][i] * number
-                for i in range(len(mul.mem_energy_breakdown[op]))
-            ]
-            for op in mul.mem_energy_breakdown.keys()
-        }
-        mul.mem_energy_breakdown_further = {
-            op: [
-                mul.mem_energy_breakdown_further[op][i] * number
-                for i in range(len(mul.mem_energy_breakdown_further[op]))
-            ]
-            for op in mul.mem_energy_breakdown_further.keys()
-        }
-        mul.energy_total *= number
-
-        # Memory access
-        mul.memory_word_access = {
-            op: [
-                mul.memory_word_access[op][i] * number
-                for i in range(len(mul.memory_word_access[op]))
-            ]
-            for op in mul.memory_word_access.keys()
-        }
-
-        # Latency
-        mul.data_loading_cycle *= number
-        mul.data_offloading_cycle *= number
-        mul.ideal_cycle *= number
-        mul.ideal_temporal_cycle *= number
-        mul.latency_total0 *= number
-        mul.latency_total1 *= number
-        mul.latency_total2 *= number
-
-        # MAC utilization
-        mul.MAC_spatial_utilization = mul.ideal_cycle / mul.ideal_temporal_cycle
-        mul.MAC_utilization0 = mul.ideal_cycle / mul.latency_total0
-        mul.MAC_utilization1 = mul.ideal_cycle / mul.latency_total1
-        mul.MAC_utilization2 = mul.ideal_cycle / mul.latency_total2
-
-        # Not addable
-        func = [
-            "calc_allowed_and_real_data_transfer_cycle_per_DTL",
-            "calc_data_loading_offloading_latency",
-            "calc_double_buffer_flag",
-            "calc_overall_latency",
-            "calc_MAC_energy_cost",
-            "calc_energy",
-            "calc_latency",
-            "calc_memory_energy_cost",
-            "calc_memory_utilization",
-            "calc_memory_word_access",
-            "combine_data_transfer_rate_per_physical_port",
-            "run",
-        ]
-        mul_attr = [
-            "MAC_energy",
-            "mem_energy",
-            "mem_energy_breakdown",
-            "mem_energy_breakdown_further",
-            "energy_total",
-            "memory_word_access",
-            "data_loading_cycle",
-            "data_offloading_cycle",
-            "ideal_cycle",
-            "ideal_temporal_cycle",
-            "latency_total0",
-            "latency_total1",
-            "latency_total2",
-            "MAC_spatial_utilization",
-            "MAC_utilization0",
-            "MAC_utilization1",
-            "MAC_utilization2",
-            "layer",
-            "accelerator",
-        ]
-
-        for attr in dir(mul):
-            if attr not in (func + mul_attr) and attr[0] != "_":
-                delattr(mul, attr)
+    def __str__(self):
+        return f"CostModelEvaluation({self.layer}, core {self.core_id})"
 
-        return mul
+    def __repr__(self):
+        return str(self)
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/cost_model/cost_model_for_sram_imc.py` & `zigzag_dse-3.1.1/zigzag/cost_model/CostModelEvaluationForIMC.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,252 +1,155 @@
 import logging
+from termios import ICANON
+from zigzag.hardware.architecture.ImcArray import ImcArray
 from zigzag.utils import pickle_deepcopy
-from zigzag.classes.cost_model.cost_model import (
-    CostModelEvaluation, PortActivity)
+from zigzag.cost_model.cost_model import CostModelEvaluation, PortActivity
 
 logger = logging.getLogger(__name__)
 
-## Class that stores inputs and runs them through the zigzag cost model.
-#
-# Initialize the cost model evaluation with the following inputs:
-# - accelerator: the accelerator that includes the core on which to run the layer
-# - layer: the layer to run
-# - spatial_mapping: the spatial mapping
-# - temporal_mapping: the temporal mapping
-#
-# From these parameters, the following attributes are computed:
-# * core: The core on which the layer is ran. This should be specified in the LayerNode attributes.
-# * mapping: The combined spatial and temporal mapping object where access patterns are computed.
-#
-# The following cost model attributes are also initialized:
-# - mem_energy_breakdown: The energy breakdown for all operands
-# - energy: The total energy
-#
-# After initialization, the cost model evaluation is run.
-class CostModelEvaluationForIMC(CostModelEvaluation):
-
-    ## The class constructor
-    # After initialization, the cost model evaluation is run
-    # @param accelerator the accelerator that includes the core on which to run the
-    # @param layer the layer to run
-    # @param spatial_mapping the spatial mapping
-    # @param temporal_mapping the temporal mapping
-    # @param access_same_data_considered_as_no_access (optional)
-    def __init__(
-        self,
-        *,
-        accelerator,
-        layer,
-        spatial_mapping,
-        spatial_mapping_int,
-        temporal_mapping,
-        access_same_data_considered_as_no_access=True,
-    ):
-        super().__init__(accelerator=accelerator,
-                         layer=layer,
-                         spatial_mapping=spatial_mapping,
-                         spatial_mapping_int=spatial_mapping_int,
-                         temporal_mapping=temporal_mapping,
-                         access_same_data_considered_as_no_access=access_same_data_considered_as_no_access)
-
-    def __str__(self):
-        return super().__str__()
 
-    def __repr__(self):
-        return super().__repr__()
+class CostModelEvaluationForIMC(CostModelEvaluation):
+    """! Class that stores inputs and runs them through the zigzag cost model.
 
-    # JSON representation used for saving this object to a json file.
-    def __jsonrepr__(self):
-        # latency_total0 breakdown
-        computation_breakdown = {
-            "mac_computation": self.ideal_temporal_cycle,
-            "weight_loading": self.SS_comb,
-        }
+    Initialize the cost model evaluation with the following inputs:
+    - accelerator: the accelerator that includes the core on which to run the layer
+    - layer: the layer to run
+    - spatial_mapping: the spatial mapping
+    - temporal_mapping: the temporal mapping
+
+    From these parameters, the following attributes are computed:
+    * core: The core on which the layer is ran. This should be specified in the LayerNode attributes.
+    * mapping: The combined spatial and temporal mapping object where access patterns are computed.
+
+    The following cost model attributes are also initialized:
+    - mem_energy_breakdown: The energy breakdown for all operands
+    - energy: The total energy
 
-        return {
-            "outputs": {
-                "memory": {
-                    "utilization": self.mem_utili_shared
-                    if hasattr(self, "mem_utili_shared")
-                    else None,
-                    "word_accesses": self.memory_word_access,
-                },
-                "energy": {
-                    "energy_total": self.energy_total,
-                    "operational_energy": self.MAC_energy,
-                    "operational_energy_breakdown": self.MAC_energy_breakdown,
-                    "memory_energy": self.mem_energy,
-                    "memory_energy_breakdown_per_level": self.mem_energy_breakdown,
-                    "memory_energy_breakdown_per_level_per_operand": self.mem_energy_breakdown_further,
-                },
-                "latency": {
-                    "data_onloading": self.latency_total1 - self.latency_total0,
-                    "computation": self.latency_total0,
-                    "data_offloading": self.latency_total2 - self.latency_total1,
-                    "computation_breakdown": computation_breakdown,
-                },
-                "clock": {
-                    "tclk (ns)": self.tclk,
-                    "tclk_breakdown (ns)": self.tclk_breakdown,
-                },
-                "area (mm^2)": {
-                    "total_area": self.area_total,
-                    "total_area_breakdown:": {
-                        "imc_area": self.imc_area,
-                        "mem_area": self.mem_area,
-                    },
-                    "total_area_breakdown_further": {
-                        "imc_area_breakdown": self.imc_area_breakdown,
-                        "mem_area_breakdown": self.mem_area_breakdown,
-                    },
-                },
-                "spatial": {
-                    "mac_utilization": {
-                        "ideal": self.MAC_spatial_utilization,
-                        "stalls": self.MAC_utilization0,
-                        "stalls_onloading": self.MAC_utilization1,
-                        "stalls_onloading_offloading": self.MAC_utilization2,
-                    }
-                },
-            },
-            "inputs": {
-                "accelerator": self.accelerator,
-                "layer": self.layer,
-                "spatial_mapping": self.spatial_mapping_int
-                if hasattr(self, "spatial_mapping_int")
-                else None,
-                "temporal_mapping": self.temporal_mapping
-                if hasattr(self, "temporal_mapping")
-                else None,
-            },
-        }
+    After initialization, the cost model evaluation is run.
+    """
 
-    ## Simple JSON representation used for saving this object to a simple json file.
-    def __simplejsonrepr__(self):
-        return {"energy": self.energy_total, "latency": self.latency_total2, "tclk": self.tclk, "area": self.area_total}
+    def __init__(self):
+        super().__init__(...)  # TODO
+        operational_array = self.accelerator.get_core(self.core_id).operational_array
+        self.imc_area = operational_array.total_area
+        assert isinstance(operational_array, ImcArray)
+        self.operational_array: ImcArray = operational_array
 
-    ## Run the cost model evaluation.
-    def run(self):
+    def run(self) -> None:
+        """! Run the cost model evaluation."""
         super().calc_memory_utilization()
         super().calc_memory_word_access()
         self.calc_energy()
         self.calc_latency()
         self.collect_area_data()
 
     def collect_area_data(self):
         # get imc area
-        operational_array = self.accelerator.get_core(self.core_id).operational_array
-        self.imc_area = operational_array.total_area
-        self.imc_area_breakdown = operational_array.area_breakdown
+
+        self.imc_area_breakdown = self.operational_array.area_breakdown
         # get mem area
         self.mem_area = 0
         self.mem_area_breakdown = {}
         for mem in self.mem_level_list:
             memory_instance = mem.memory_instance
             memory_instance_name = memory_instance.name
             self.mem_area += memory_instance.area
             self.mem_area_breakdown[memory_instance_name] = memory_instance.area
         # get total area
         self.area_total = self.imc_area + self.mem_area
 
-    ## Calculates the energy cost of this cost model evaluation by calculating the memory reading/writing energy.
     def calc_energy(self):
+        """! Calculates the energy cost of this cost model evaluation by calculating the memory reading/writing energy."""
         # - TODO: Interconnection energy
         self.calc_MAC_energy_cost()
         super().calc_memory_energy_cost()
 
-    ## Calculate the dynamic MAC energy
     def calc_MAC_energy_cost(self):
+        """! Calculate the dynamic MAC energy"""
         core = self.accelerator.get_core(self.core_id)
         self.MAC_energy_breakdown = core.operational_array.unit.get_energy_for_a_layer(self.layer, self.mapping)
         self.MAC_energy = sum([energy for energy in self.MAC_energy_breakdown.values()])
 
-    ##  Calculate latency in 4 steps
-    #
-    # 1) As we already calculated the ideal data transfer rate in combined_mapping.py (in the Mapping class),
-    # here we start with calculating the required (or allowed) memory updating window by comparing the effective
-    # data size with the physical memory size at each level. If the effective data size is smaller than 50%
-    # of the physical memory size, then we take the whole period as the allowed memory updating window (double buffer effect);
-    # otherwise we take the the period divided by the top_ir_loop as the allowed memory updating window.
-    #
-    # 2) Then, we compute the real data transfer rate given the actual memory bw per functional port pair,
-    # assuming we have enough memory ports.
-    #
-    # 3) In reality, there is no infinite memory port to use. So, as the second step, we combine the real
-    # data transfer attributes per physical memory port.
-    #
-    # 4) Finally, we combine the stall/slack of each memory port to get the final latency.
     def calc_latency(self):
+        """!  Calculate latency in 4 steps
+
+        1) As we already calculated the ideal data transfer rate in combined_mapping.py (in the Mapping class),
+        here we start with calculating the required (or allowed) memory updating window by comparing the effective
+        data size with the physical memory size at each level. If the effective data size is smaller than 50%
+        of the physical memory size, then we take the whole period as the allowed memory updating window (double buffer effect);
+        otherwise we take the the period divided by the top_ir_loop as the allowed memory updating window.
+
+        2) Then, we compute the real data transfer rate given the actual memory bw per functional port pair,
+        assuming we have enough memory ports.
+
+        3) In reality, there is no infinite memory port to use. So, as the second step, we combine the real
+        data transfer attributes per physical memory port.
+
+        4) Finally, we combine the stall/slack of each memory port to get the final latency.
+        """
         super().calc_double_buffer_flag()
         super().calc_allowed_and_real_data_transfer_cycle_per_DTL()
         # Update the latency model to fit IMC requirement
         self.combine_data_transfer_rate_per_physical_port()
         super().calc_data_loading_offloading_latency()
         # find the cycle count per mac
         operational_array = self.accelerator.get_core(self.core_id).operational_array
         hd_param = operational_array.unit.hd_param
         cycles_per_mac = hd_param["input_precision"] / hd_param["input_bit_per_cycle"]
         super().calc_overall_latency(cycles_per_mac=cycles_per_mac)
 
-    ## This function calculate the stalling cycles for IMC (In-Memory-Computing) hardware template
-    # Consider memory sharing and port sharing, combine the data transfer activity
-    # Step 1: collect port activity per memory instance per physical memory port
-    # Step 2: calculate SS combine and MUW union parameters per physical memory port
-    # Note: this calculation is incorrect when following conditions are ALL true:
-    # (1) there are more than two mem levels for storing weights, e.g. dram -> cache -> IMC cells
-    # (2) extra stalling is introduced due to the intermediate mem levels (e.g. due to insifficuent bw of cache)
     def combine_data_transfer_rate_per_physical_port(self):
+        """! This function calculate the stalling cycles for IMC (In-Memory-Computing) hardware template
+        Consider memory sharing and port sharing, combine the data transfer activity
+        Step 1: collect port activity per memory instance per physical memory port
+        Step 2: calculate SS combine and MUW union parameters per physical memory port
+        Note: this calculation is incorrect when following conditions are ALL true:
+        (1) there are more than two mem levels for storing weights, e.g. dram -> cache -> IMC cells
+        (2) extra stalling is introduced due to the intermediate mem levels (e.g. due to insifficuent bw of cache)
+        """
         # Step 1: collect port activity per memory instance per physical memory port
         port_activity_collect = []
         for mem_instance in self.mem_level_list:
             port_activity_single = {}
             port_list = mem_instance.port_list
             for port in port_list:
                 port_activity_single[str(port)] = []
                 for mem_op, mem_lv, mov_dir in port.served_op_lv_dir:
                     try:
                         layer_op = self.mem_op_to_layer_op[mem_op]
                     except:  # mem op to layer might not have this mem op (e.g. pooling layer)
                         continue
                     period_count = getattr(
-                        self.mapping_int.unit_mem_data_movement[layer_op][
-                            mem_lv
-                        ].data_trans_period_count,
+                        self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_trans_period_count,
                         mov_dir,
                     )
                     if period_count == 0:
                         # skip the inactive data movement activities because they won't impact SS
                         continue
                     period = getattr(
-                        self.mapping_int.unit_mem_data_movement[layer_op][
-                            mem_lv
-                        ].data_trans_period,
+                        self.mapping_int.unit_mem_data_movement[layer_op][mem_lv].data_trans_period,
                         mov_dir,
                     )
-                    real_cycle = getattr(
-                        self.real_data_trans_cycle[layer_op][mem_lv], mov_dir
-                    )
-                    allowed_cycle = getattr(
-                        self.allowed_mem_updat_cycle[layer_op][mem_lv], mov_dir
-                    )
+                    real_cycle = getattr(self.real_data_trans_cycle[layer_op][mem_lv], mov_dir)
+                    allowed_cycle = getattr(self.allowed_mem_updat_cycle[layer_op][mem_lv], mov_dir)
                     port_activity = PortActivity(
                         real_cycle,
                         allowed_cycle,
                         period,
                         period_count,
                         layer_op,
                         mem_lv,
                         mov_dir,
                     )
                     port_activity_single[str(port)].append(port_activity)
             port_activity_collect.append(port_activity_single)
         self.port_activity_collect = port_activity_collect
 
         # Step 2: calculate weight loading cycles
-        layer_const_operand = self.layer.constant_operands[0] # e.g. "W"
+        layer_const_operand = self.layer.constant_operands[0]  # e.g. "W"
         # get spatial mapping in a macro
         core = next(iter(self.accelerator.cores))
         operational_array = core.operational_array
         memory_hierarchy = core.mem_hierarchy_dict
         hd_param = operational_array.unit.hd_param
         wl_dim = hd_param["wordline_dimension"]
         bl_dim = hd_param["bitline_dimension"]
@@ -257,21 +160,21 @@
                     spatial_mapping_in_macro.append(loop)
                 else:  # mix layer_dim unrolling
                     for element in loop:
                         spatial_mapping_in_macro.append(element)
         # check if there is only one mem level for weight in accelerator. No weight loading required if that is the case.
         weight_mem_op = self.layer_op_to_mem_op[layer_const_operand]
         weight_mem_hierarchy: list = memory_hierarchy[weight_mem_op]
-        if len(weight_mem_hierarchy) == 1: # there is only one mem level for weight
+        if len(weight_mem_hierarchy) == 1:  # there is only one mem level for weight
             require_weight_loading = False
         else:
             require_weight_loading = True
         # check how many times of weight reloading is required
         # here assume imc cells is the lowest mem level for weight and rw_port
-        for imc_port, imc_ports in port_activity_collect[0].items(): # 0: the lowest mem node in the graph
+        for imc_port, imc_ports in port_activity_collect[0].items():  # 0: the lowest mem node in the graph
             for port in imc_ports:
                 if port.served_op_lv_dir[2] == "wr_in_by_high":
                     nb_of_weight_reload_periods = port.period_count
 
         # get the number of mapped rows in a macro
         imc_macro = operational_array.unit
         mapped_rows_total = imc_macro.mapped_rows_total
@@ -301,37 +204,38 @@
             if op in other.MAC_energy_breakdown.keys():
                 sum.MAC_energy_breakdown[op] = self.MAC_energy_breakdown[op] + other.MAC_energy_breakdown[op]
 
         for op in sum.mem_energy_breakdown.keys():
             if op in other.mem_energy_breakdown.keys():
                 l = []
                 for i in range(
-                    min(len(self.mem_energy_breakdown[op]), len(other.mem_energy_breakdown[op]))
-                ):
-                    l.append(
-                        self.mem_energy_breakdown[op][i] + other.mem_energy_breakdown[op][i]
+                    min(
+                        len(self.mem_energy_breakdown[op]),
+                        len(other.mem_energy_breakdown[op]),
                     )
-                i = min(len(self.mem_energy_breakdown[op]), len(other.mem_energy_breakdown[op]))
+                ):
+                    l.append(self.mem_energy_breakdown[op][i] + other.mem_energy_breakdown[op][i])
+                i = min(
+                    len(self.mem_energy_breakdown[op]),
+                    len(other.mem_energy_breakdown[op]),
+                )
                 l += self.mem_energy_breakdown[op][i:]
                 l += other.mem_energy_breakdown[op][i:]
                 sum.mem_energy_breakdown[op] = l
 
         for op in sum.mem_energy_breakdown_further.keys():
             if op in other.mem_energy_breakdown_further.keys():
                 l = []
                 for i in range(
                     min(
                         len(self.mem_energy_breakdown_further[op]),
                         len(other.mem_energy_breakdown_further[op]),
                     )
                 ):
-                    l.append(
-                        self.mem_energy_breakdown_further[op][i]
-                        + other.mem_energy_breakdown_further[op][i]
-                    )
+                    l.append(self.mem_energy_breakdown_further[op][i] + other.mem_energy_breakdown_further[op][i])
                 i = min(
                     len(self.mem_energy_breakdown_further[op]),
                     len(other.mem_energy_breakdown_further[op]),
                 )
                 l += self.mem_energy_breakdown_further[op][i:]
                 l += other.mem_energy_breakdown_further[op][i:]
                 sum.mem_energy_breakdown_further[op] = l
@@ -354,20 +258,16 @@
                 l = []
                 for i in range(
                     min(
                         len(self.memory_word_access[op]),
                         len(other.memory_word_access[op]),
                     )
                 ):
-                    l.append(
-                        self.memory_word_access[op][i] + other.memory_word_access[op][i]
-                    )
-                i = min(
-                    len(self.memory_word_access[op]), len(other.memory_word_access[op])
-                )
+                    l.append(self.memory_word_access[op][i] + other.memory_word_access[op][i])
+                i = min(len(self.memory_word_access[op]), len(other.memory_word_access[op]))
                 l += self.memory_word_access[op][i:]
                 l += other.memory_word_access[op][i:]
                 sum.memory_word_access[op] = l
         for op in op_diff:
             sum.memory_word_access[op] = other.memory_word_access[op]
 
         ## Latency
@@ -458,7 +358,75 @@
 
         for attr in dir(sum):
             if attr not in (func + add_attr) and attr[0] != "_":
                 delattr(sum, attr)
 
         return sum
 
+    # JSON representation used for saving this object to a json file.
+    def __jsonrepr__(self):
+        # latency_total0 breakdown
+        computation_breakdown = {
+            "mac_computation": self.ideal_temporal_cycle,
+            "weight_loading": self.SS_comb,
+        }
+
+        return {
+            "outputs": {
+                "memory": {
+                    "utilization": (self.mem_utili_shared if hasattr(self, "mem_utili_shared") else None),
+                    "word_accesses": self.memory_word_access,
+                },
+                "energy": {
+                    "energy_total": self.energy_total,
+                    "operational_energy": self.MAC_energy,
+                    "operational_energy_breakdown": self.MAC_energy_breakdown,
+                    "memory_energy": self.mem_energy,
+                    "memory_energy_breakdown_per_level": self.mem_energy_breakdown,
+                    "memory_energy_breakdown_per_level_per_operand": self.mem_energy_breakdown_further,
+                },
+                "latency": {
+                    "data_onloading": self.latency_total1 - self.latency_total0,
+                    "computation": self.latency_total0,
+                    "data_offloading": self.latency_total2 - self.latency_total1,
+                    "computation_breakdown": computation_breakdown,
+                },
+                "clock": {
+                    "tclk (ns)": self.tclk,
+                    "tclk_breakdown (ns)": self.tclk_breakdown,
+                },
+                "area (mm^2)": {
+                    "total_area": self.area_total,
+                    "total_area_breakdown:": {
+                        "imc_area": self.imc_area,
+                        "mem_area": self.mem_area,
+                    },
+                    "total_area_breakdown_further": {
+                        "imc_area_breakdown": self.imc_area_breakdown,
+                        "mem_area_breakdown": self.mem_area_breakdown,
+                    },
+                },
+                "spatial": {
+                    "mac_utilization": {
+                        "ideal": self.MAC_spatial_utilization,
+                        "stalls": self.MAC_utilization0,
+                        "stalls_onloading": self.MAC_utilization1,
+                        "stalls_onloading_offloading": self.MAC_utilization2,
+                    }
+                },
+            },
+            "inputs": {
+                "accelerator": self.accelerator,
+                "layer": self.layer,
+                "spatial_mapping": (self.spatial_mapping_int if hasattr(self, "spatial_mapping_int") else None),
+                "temporal_mapping": (self.temporal_mapping if hasattr(self, "temporal_mapping") else None),
+            },
+        }
+
+    def __simplejsonrepr__(self):
+        """! Simple JSON representation used for saving this object to a simple json file."""
+        return {
+            "energy": self.energy_total,
+            "latency": self.latency_total2,
+            "tclk": self.tclk,
+            "area": self.area_total,
+        }
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/AimcArray.py` & `zigzag_dse-3.1.1/zigzag/hardware/architecture/AimcArray.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-import numpy as np
+"""
+README
+  . class AimcArray (defines the energy/area/delay cost of an ADC, a DAC and an AIMC array)
+How to use this file?
+  . This file is internally called in ZigZag-IMC framework.
+  . It can also be run independently, for mainly debugging. An example is given at the end of the file.
+"""
+
 import math
-import copy
+
+from zigzag.hardware.architecture.DimcArray import UserSpatialMappingGenerator
+
+
 if __name__ == "__main__":
     from imc_unit import ImcUnit
     from DimcArray import DimcArray
     import logging as _logging
+
     _logging_level = _logging.INFO
-    _logging_format = '%(asctime)s - %(funcName)s +%(lineno)s - %(levelname)s - %(message)s'
-    _logging.basicConfig(level=_logging_level,
-                         format=_logging_format)
+    _logging_format = "%(asctime)s - %(funcName)s +%(lineno)s - %(levelname)s - %(message)s"
+    _logging.basicConfig(level=_logging_level, format=_logging_format)
 else:
     import logging as _logging
-    from zigzag.classes.hardware.architecture.imc_unit import ImcUnit
-    from zigzag.classes.hardware.architecture.DimcArray import DimcArray
+    from zigzag.hardware.architecture.imc_unit import ImcUnit
+    from zigzag.hardware.architecture.DimcArray import DimcArray
 
-###############################################################################################################
-# README
-#   . class AimcArray (defines the energy/area/delay cost of an ADC, a DAC and an AIMC array)
-# How to use this file?
-#   . This file is internally called in ZigZag-IMC framework.
-#   . It can also be run independently, for mainly debugging. An example is given at the end of the file.
-###############################################################################################################
 
 class AimcArray(ImcUnit):
     # definition of an Analog In-SRAM-Computing (DIMC) core
     # constraint:
     #     -- activation precision must be in the power of 2.
     #     -- input_bit_per_cycle must be in the power of 2.
-    def __init__(self,tech_param:dict, hd_param:dict, dimensions:dict):
+    def __init__(self, tech_param: dict, hd_param: dict, dimensions: dict):
         # @param tech_param: technology related parameters
         # @param hd_param: IMC cores' parameters
         # @param dimensions: IMC cores' dimensions
         super().__init__(tech_param, hd_param, dimensions)
 
     def __jsonrepr__(self):
         """
@@ -39,211 +42,251 @@
         """
         # not implemented
         # return {"operational_unit": self.unit, "dimensions": self.dimensions}
         pass
 
     def get_adc_cost(self):
         """single ADC cost calculation"""
-        """area (mm^2)"""
+        # area (mm^2)
         if self.hd_param["adc_resolution"] == 1:
             adc_area = 0
-        else: # formula extracted and validated against 3 AIMC papers on 28nm
+        else:  # formula extracted and validated against 3 AIMC papers on 28nm
             k1 = -0.0369
             k2 = 1.206
-            adc_area = 10**(k1*self.hd_param["adc_resolution"]+k2) * 2**self.hd_param["adc_resolution"] * (10**-6) # unit: mm^2
-        """delay (ns)"""
-        k3 = 0.00653 # ns
-        k4 = 0.640 # ns
-        adc_delay = self.hd_param["adc_resolution"] * (k3*self.dimensions["D2"] + k4) # unit: ns
-        """energy (fJ)"""
-        k5 = 100 # fF
-        k6 = 0.001 # fF
-        adc_energy = (k5 * self.hd_param["adc_resolution"] + k6 * 4**self.hd_param["adc_resolution"]) * self.logic_unit.tech_param["vdd"]**2 # unit: fJ
-        adc_energy = adc_energy/1000 # unit: pJ
+            adc_area = (
+                10 ** (k1 * self.hd_param["adc_resolution"] + k2) * 2 ** self.hd_param["adc_resolution"] * (10**-6)
+            )  # unit: mm^2
+        # delay (ns)
+        k3 = 0.00653  # ns
+        k4 = 0.640  # ns
+        adc_delay = self.hd_param["adc_resolution"] * (k3 * self.dimensions["D2"] + k4)  # unit: ns
+        # energy (fJ)
+        k5 = 100  # fF
+        k6 = 0.001  # fF
+        adc_energy = (
+            k5 * self.hd_param["adc_resolution"] + k6 * 4 ** self.hd_param["adc_resolution"]
+        ) * self.logic_unit.tech_param[
+            "vdd"
+        ] ** 2  # unit: fJ
+        adc_energy = adc_energy / 1000  # unit: pJ
         return adc_area, adc_delay, adc_energy
 
     def get_dac_cost(self):
         """single DAC cost calculation"""
-        """area (mm^2)"""
-        dac_area = 0 # neglected
-        """delay (ns)"""
-        dac_delay = 0 # neglected
-        """energy (fJ)"""
+        # area (mm^2)
+        dac_area = 0  # neglected
+        # delay (ns)
+        dac_delay = 0  # neglected
+        # energy (fJ)
         if self.hd_param["input_bit_per_cycle"] == 1:
             dac_energy = 0
         else:
-            k0 = 50e-3 # pF
-            dac_energy = k0 * self.hd_param["input_bit_per_cycle"] * self.logic_unit.tech_param["vdd"]**2 # unit: pJ
+            k0 = 50e-3  # pF
+            dac_energy = k0 * self.hd_param["input_bit_per_cycle"] * self.logic_unit.tech_param["vdd"] ** 2  # unit: pJ
         return dac_area, dac_delay, dac_energy
 
-    ## get area of AIMC macros (cells, mults, adders, adders_pv, accumulators. Not include input/output regs)
     def get_area(self):
+        """! get area of AIMC macros (cells, mults, adders, adders_pv, accumulators. Not include input/output regs)"""
         # area of cell array
         tech_node = self.logic_unit.tech_param["tech_node"]
         group_depth = self.hd_param["group_depth"]
         w_pres = self.hd_param["weight_precision"]
         if self.hd_param["enable_cacti"] == True:
-            single_cell_array_area = self.get_single_cell_array_cost_from_cacti(tech_node,
-                                                                                self.wl_dim_size,
-                                                                                self.bl_dim_size,
-                                                                                group_depth,
-                                                                                w_pres)[1]
+            single_cell_array_area = self.get_single_cell_array_cost_from_cacti(
+                tech_node, self.wl_dim_size, self.bl_dim_size, group_depth, w_pres
+            )[1]
             # at this point, we have the area of single cell array. Then multiply it with the number of banks.
             area_cells = single_cell_array_area * self.nb_of_banks  # total cell array area in the core
         else:
             # TODO: [TO BE SUPPORTED OR YOU CAN MODIFY YOURSELF]
             area_cells = None  # user-provided cell array area (from somewhere?)
             raise Exception(f"User-provided cell area is not supported yet.")
 
         # area of multiplier array
-        area_mults = self.logic_unit.get_1b_multiplier_area() * w_pres * \
-                     self.wl_dim_size * self.bl_dim_size * self.nb_of_banks
+        area_mults = (
+            self.logic_unit.get_1b_multiplier_area() * w_pres * self.wl_dim_size * self.bl_dim_size * self.nb_of_banks
+        )
 
         # area of ADCs
         area_adcs = self.get_adc_cost()[0] * w_pres * self.wl_dim_size * self.nb_of_banks
 
         # area of DACs
         area_dacs = self.get_dac_cost()[0] * self.bl_dim_size * self.nb_of_banks
 
         # area of adders with place values after ADC conversion (type: RCA)
         nb_inputs_of_adder_pv = w_pres
         if nb_inputs_of_adder_pv == 1:
             nb_of_1b_adder_pv = 0
         else:
             adder_depth_pv = math.log2(nb_inputs_of_adder_pv)
-            assert adder_depth_pv % 1 == 0, \
-                f"[AimcArray] The value [{nb_inputs_of_adder_pv}] of [weight_precision] is not in the power of 2."
+            assert (
+                adder_depth_pv % 1 == 0
+            ), f"[AimcArray] The value [{nb_inputs_of_adder_pv}] of [weight_precision] is not in the power of 2."
             adder_depth_pv = int(adder_depth_pv)  # float -> int for simplicity
             adder_input_precision = self.hd_param["adc_resolution"]
-            nb_of_1b_adder_pv = adder_input_precision * (nb_inputs_of_adder_pv - 1) + nb_inputs_of_adder_pv * (adder_depth_pv - 0.5)  # nb of 1b adders in a single place-value adder tree
+            nb_of_1b_adder_pv = adder_input_precision * (nb_inputs_of_adder_pv - 1) + nb_inputs_of_adder_pv * (
+                adder_depth_pv - 0.5
+            )  # nb of 1b adders in a single place-value adder tree
             nb_of_1b_adder_pv *= self.wl_dim_size * self.nb_of_banks  # multiply with nb_of_adder_trees
         area_adders_pv = self.logic_unit.get_1b_adder_area() * nb_of_1b_adder_pv
 
         # area of accumulators (adder type: RCA)
         if self.hd_param["input_bit_per_cycle"] == self.hd_param["input_precision"]:
             area_accumulators = 0
         else:
-            accumulator_output_pres = w_pres + self.hd_param["adc_resolution"] + self.hd_param["input_precision"] # output precision from adders_pv + required shifted bits
+            accumulator_output_pres = (
+                w_pres + self.hd_param["adc_resolution"] + self.hd_param["input_precision"]
+            )  # output precision from adders_pv + required shifted bits
             nb_of_1b_adder_accumulator = accumulator_output_pres * self.wl_dim_size * self.nb_of_banks
-            nb_of_1b_reg_accumulator = nb_of_1b_adder_accumulator # number of regs in an accumulator
-            area_accumulators = self.logic_unit.get_1b_adder_area() * nb_of_1b_adder_accumulator + \
-                                self.logic_unit.get_1b_reg_area() * nb_of_1b_reg_accumulator
+            nb_of_1b_reg_accumulator = nb_of_1b_adder_accumulator  # number of regs in an accumulator
+            area_accumulators = (
+                self.logic_unit.get_1b_adder_area() * nb_of_1b_adder_accumulator
+                + self.logic_unit.get_1b_reg_area() * nb_of_1b_reg_accumulator
+            )
 
         # total area of imc
-        self.area_breakdown = { # unit: same with in input hd file
-            "cells":    area_cells,
-            "mults":    area_mults,
-            "adcs":     area_adcs,
-            "dacs":     area_dacs,
-            "adders_pv":area_adders_pv,
-            "accumulators": area_accumulators
+        self.area_breakdown = {  # unit: same with in input hd file
+            "cells": area_cells,
+            "mults": area_mults,
+            "adcs": area_adcs,
+            "dacs": area_dacs,
+            "adders_pv": area_adders_pv,
+            "accumulators": area_accumulators,
         }
         self.area = sum([v for v in self.area_breakdown.values()])
         # return self.area_breakdown
 
-    ## get delay of imc macros (worst path: dacs -> mults -> adcs -> adders -> accumulators)
     def get_delay(self):
+        """! get delay of imc macros (worst path: dacs -> mults -> adcs -> adders -> accumulators)"""
         # delay of dacs
         dly_dacs = self.get_dac_cost()[1]
 
         # delay of multipliers
         dly_mults = self.logic_unit.get_1b_multiplier_dly()
 
         # delay of adcs
         dly_adcs = self.get_adc_cost()[1]
 
         # delay of adders_pv (adder type: RCA, worst path: in-to-sum -> in-to-sum -> ... -> in-to-cout -> cin-to-cout -> ... -> cin-to-cout)
-        w_pres = self.hd_param["weight_precision"] # weight precision
+        w_pres = self.hd_param["weight_precision"]  # weight precision
         nb_inputs_of_adder_pv = w_pres
         if nb_inputs_of_adder_pv == 1:
             dly_adders_pv = 0
         else:
             adder_depth_pv = math.log2(nb_inputs_of_adder_pv)
             adder_depth_pv = int(adder_depth_pv)  # float -> int for simplicity
-            adder_pv_output_precision = nb_inputs_of_adder_pv + self.hd_param["adc_resolution"] # output precision from adders_pv
-            dly_adders_pv = (adder_depth_pv-1) * self.logic_unit.get_1b_adder_dly_in2sum() + \
-                            self.logic_unit.get_1b_adder_dly_in2cout() + \
-                            (adder_pv_output_precision-1) * self.logic_unit.get_1b_adder_dly_cin2cout()
+            adder_pv_output_precision = (
+                nb_inputs_of_adder_pv + self.hd_param["adc_resolution"]
+            )  # output precision from adders_pv
+            dly_adders_pv = (
+                (adder_depth_pv - 1) * self.logic_unit.get_1b_adder_dly_in2sum()
+                + self.logic_unit.get_1b_adder_dly_in2cout()
+                + (adder_pv_output_precision - 1) * self.logic_unit.get_1b_adder_dly_cin2cout()
+            )
 
         # delay of accumulators (adder type: RCA)
         if self.hd_param["input_bit_per_cycle"] == self.hd_param["input_precision"]:
             dly_accumulators = 0
         else:
             accumulator_input_pres = adder_pv_output_precision
-            accumulator_output_pres = self.hd_param["weight_precision"] + self.hd_param["adc_resolution"] + self.hd_param["input_precision"]  # output precision from adders_pv + required shifted bits
-            dly_accumulators = self.logic_unit.get_1b_adder_dly_in2cout() + \
-                               (accumulator_output_pres-accumulator_input_pres) * self.logic_unit.get_1b_adder_dly_cin2cout()
+            accumulator_output_pres = (
+                self.hd_param["weight_precision"] + self.hd_param["adc_resolution"] + self.hd_param["input_precision"]
+            )  # output precision from adders_pv + required shifted bits
+            dly_accumulators = (
+                self.logic_unit.get_1b_adder_dly_in2cout()
+                + (accumulator_output_pres - accumulator_input_pres) * self.logic_unit.get_1b_adder_dly_cin2cout()
+            )
 
         # total delay of imc
         self.delay_breakdown = {
-            "dacs":     dly_dacs,
-            "mults":    dly_mults,
-            "adcs":     dly_adcs,
-            "adders_pv":dly_adders_pv,
-            "accumulators": dly_accumulators
+            "dacs": dly_dacs,
+            "mults": dly_mults,
+            "adcs": dly_adcs,
+            "adders_pv": dly_adders_pv,
+            "accumulators": dly_accumulators,
         }
         self.delay = sum([v for v in self.delay_breakdown.values()])
         # return self.delay_breakdown
 
-    ## macro-level one-cycle energy of imc arrays (fully utilization, no weight updating)
-    # (components: cells, mults, adders, adders_pv, accumulators. Not include input/output regs)
     def get_peak_energy_single_cycle(self):
+        """! macro-level one-cycle energy of imc arrays (fully utilization, no weight updating)
+        (components: cells, mults, adders, adders_pv, accumulators. Not include input/output regs)
+        """
         layer_const_operand_pres = self.hd_param["weight_precision"]
         layer_act_operand_pres = self.hd_param["input_precision"]
-        """energy of precharging"""
+        # energy of precharging
         energy_precharging = 0
 
-        """energy of DACs"""
+        # energy of DACs
         energy_dacs = self.get_dac_cost()[2] * self.bl_dim_size * self.nb_of_banks
 
-        """energy of cell array (bitline accumulation, type: voltage-based)"""
-        energy_cells = (self.logic_unit.tech_param["bl_cap"] * (self.logic_unit.tech_param["vdd"] ** 2) * layer_const_operand_pres) * \
-                       self.wl_dim_size * self.bl_dim_size * self.nb_of_banks
+        # energy of cell array (bitline accumulation, type: voltage-based)
+        energy_cells = (
+            (self.logic_unit.tech_param["bl_cap"] * (self.logic_unit.tech_param["vdd"] ** 2) * layer_const_operand_pres)
+            * self.wl_dim_size
+            * self.bl_dim_size
+            * self.nb_of_banks
+        )
 
-        """energy of ADCs"""
+        # energy of ADCs
         energy_adcs = self.get_adc_cost()[2] * layer_const_operand_pres * self.wl_dim_size * self.nb_of_banks
 
-        """energy of multiplier array"""
-        energy_mults = (self.logic_unit.get_1b_multiplier_energy() * layer_const_operand_pres) * \
-                       self.bl_dim_size * self.wl_dim_size * self.nb_of_banks
+        # energy of multiplier array
+        energy_mults = (
+            (self.logic_unit.get_1b_multiplier_energy() * layer_const_operand_pres)
+            * self.bl_dim_size
+            * self.wl_dim_size
+            * self.nb_of_banks
+        )
 
-        """energy of adders_pv (type: RCA)"""
+        # energy of adders_pv (type: RCA)
         nb_inputs_of_adder_pv = layer_const_operand_pres
         if nb_inputs_of_adder_pv == 1:
             energy_adders_pv = 0
         else:
             adder_pv_input_precision = self.hd_param["adc_resolution"]
-            nb_of_1b_adder_pv = adder_pv_input_precision * (nb_inputs_of_adder_pv - 1) + nb_inputs_of_adder_pv * (math.log2(nb_inputs_of_adder_pv) - 0.5)
-            energy_adders_pv = nb_of_1b_adder_pv * self.logic_unit.get_1b_adder_energy() * self.wl_dim_size * self.nb_of_banks
+            nb_of_1b_adder_pv = adder_pv_input_precision * (nb_inputs_of_adder_pv - 1) + nb_inputs_of_adder_pv * (
+                math.log2(nb_inputs_of_adder_pv) - 0.5
+            )
+            energy_adders_pv = (
+                nb_of_1b_adder_pv * self.logic_unit.get_1b_adder_energy() * self.wl_dim_size * self.nb_of_banks
+            )
 
-        """energy of accumulators (adder type: RCA)"""
+        # energy of accumulators (adder type: RCA)
         if self.hd_param["input_bit_per_cycle"] == layer_act_operand_pres:
             energy_accumulators = 0
         else:
             accumulator_output_pres = layer_act_operand_pres + layer_const_operand_pres + math.log2(self.bl_dim_size)
-            energy_accumulators = (self.logic_unit.get_1b_adder_energy() + self.logic_unit.get_1b_reg_energy()) * accumulator_output_pres * \
-                                  self.wl_dim_size * self.nb_of_banks
+            energy_accumulators = (
+                (self.logic_unit.get_1b_adder_energy() + self.logic_unit.get_1b_reg_energy())
+                * accumulator_output_pres
+                * self.wl_dim_size
+                * self.nb_of_banks
+            )
 
         peak_energy_breakdown = {  # unit: pJ (the unit borrowed from CACTI)
             "precharging": energy_precharging,
             "dacs": energy_dacs,
             "adcs": energy_adcs,
             "analog_bitlines": energy_cells,
             "mults": energy_mults,
             "adders_pv": energy_adders_pv,
-            "accumulators": energy_accumulators
+            "accumulators": energy_accumulators,
         }
         # peak_energy = sum([v for v in peak_energy_breakdown.values()])
         return peak_energy_breakdown
 
-    ## macro-level peak performance of imc arrays (fully utilization, no weight updating)
     def get_macro_level_peak_performance(self):
-        nb_of_macs_per_cycle = self.wl_dim_size * self.bl_dim_size / \
-                               (self.hd_param["input_precision"] / self.hd_param["input_bit_per_cycle"]) * \
-                               self.nb_of_banks
+        """! macro-level peak performance of imc arrays (fully utilization, no weight updating)"""
+        nb_of_macs_per_cycle = (
+            self.wl_dim_size
+            * self.bl_dim_size
+            / (self.hd_param["input_precision"] / self.hd_param["input_bit_per_cycle"])
+            * self.nb_of_banks
+        )
 
         self.get_area()
         self.get_delay()
 
         clock_cycle_period = self.delay  # unit: ns
         peak_energy_per_cycle = sum([v for v in self.get_peak_energy_single_cycle().values()])  # unit: pJ
         imc_area = self.area  # unit: mm^2
@@ -260,158 +303,198 @@
 
     def get_energy_for_a_layer(self, layer, mapping):
         """check if operand precision defined in the layer is supported"""
         # currently in the energy model, the input and weight precision defined in the workload file should be the same with in the hd input file.
         # this check can be removed if variable precision is supported in the future.
 
         # activation/weight representation
-        layer_act_operand, layer_const_operand = DimcArray.identify_layer_operand_representation(layer)
+        layer_act_operand, layer_const_operand = UserSpatialMappingGenerator.identify_layer_operand_representation(
+            layer
+        )
 
         layer_const_operand_pres = layer.operand_precision[layer_const_operand]
         layer_act_operand_pres = layer.operand_precision[layer_act_operand]
         weight_pres_in_hd_param = self.hd_param["weight_precision"]
         act_pres_in_hd_param = self.hd_param["input_precision"]
 
         # currently in the energy model, the input and weight precision defined in the workload file should be the same with in the hd input file.
         # this check can be removed if variable precision is supported in the future.
-        assert layer_const_operand_pres == weight_pres_in_hd_param, \
-            f"Weight precision defined in the workload [{layer_const_operand_pres}] not equal to the one defined in the hardware hd_param [{weight_pres_in_hd_param}]."
-        assert layer_act_operand_pres == act_pres_in_hd_param, \
-            f"Activation precision defined in the workload [{layer_act_operand_pres}] not equal to the one defined in the hardware hd_param [{act_pres_in_hd_param}]."
-
-        """parameter extraction"""
-        mapped_rows_total, mapped_rows_for_adder, mapped_cols, macro_activation_times = DimcArray.get_mapped_oa_dim(
-            layer, self.wl_dim, self.bl_dim)
+        assert (
+            layer_const_operand_pres == weight_pres_in_hd_param
+        ), f"Weight precision defined in the workload [{layer_const_operand_pres}] not equal to the one defined in the hardware hd_param [{weight_pres_in_hd_param}]."
+        assert (
+            layer_act_operand_pres == act_pres_in_hd_param
+        ), f"Activation precision defined in the workload [{layer_act_operand_pres}] not equal to the one defined in the hardware hd_param [{act_pres_in_hd_param}]."
+
+        # parameter extraction
+        (
+            mapped_rows_total,
+            mapped_rows_for_adder,
+            mapped_cols,
+            macro_activation_times,
+        ) = DimcArray.get_mapped_oa_dim(layer, self.wl_dim, self.bl_dim)
         self.mapped_rows_total = mapped_rows_total
 
-        """energy calculation"""
-        """energy of precharging"""
-        energy_precharging, mapped_group_depth = DimcArray.get_precharge_energy(self.hd_param, self.logic_unit.tech_param, layer, mapping)
+        # # energy calculation
+        # # energy of precharging
+        energy_precharging, mapped_group_depth = DimcArray.get_precharge_energy(
+            self.hd_param, self.logic_unit.tech_param, layer, mapping
+        )
         self.mapped_group_depth = mapped_group_depth
 
-        """energy of DACs"""
-        energy_dacs = self.get_dac_cost()[2] * mapped_rows_total * \
-                      layer_act_operand_pres / self.hd_param["input_bit_per_cycle"] * macro_activation_times
-
-        """energy of cell array (bitline accumulation, type: voltage-based)"""
-        energy_cells = (self.logic_unit.tech_param["bl_cap"] * (self.logic_unit.tech_param["vdd"]**2) * layer_const_operand_pres) * \
-                       mapped_cols * \
-                       self.bl_dim_size * \
-                       layer_act_operand_pres / self.hd_param["input_bit_per_cycle"] * \
-                       macro_activation_times
-
-        """energy of ADCs"""
-        energy_adcs = self.get_adc_cost()[2] * layer_const_operand_pres * mapped_cols * \
-                      layer_act_operand_pres / self.hd_param["input_bit_per_cycle"] * macro_activation_times
-
-        """energy of multiplier array"""
-        energy_mults = (self.logic_unit.get_1b_multiplier_energy() * layer_const_operand_pres) *\
-                       (mapped_rows_total * self.wl_dim_size) * \
-                       (layer_act_operand_pres / self.hd_param["input_bit_per_cycle"]) * \
-                       macro_activation_times
+        # # energy of DACs
+        energy_dacs = (
+            self.get_dac_cost()[2]
+            * mapped_rows_total
+            * layer_act_operand_pres
+            / self.hd_param["input_bit_per_cycle"]
+            * macro_activation_times
+        )
+
+        # # energy of cell array (bitline accumulation, type: voltage-based)
+        energy_cells = (
+            (self.logic_unit.tech_param["bl_cap"] * (self.logic_unit.tech_param["vdd"] ** 2) * layer_const_operand_pres)
+            * mapped_cols
+            * self.bl_dim_size
+            * layer_act_operand_pres
+            / self.hd_param["input_bit_per_cycle"]
+            * macro_activation_times
+        )
+
+        # # energy of ADCs
+        energy_adcs = (
+            self.get_adc_cost()[2]
+            * layer_const_operand_pres
+            * mapped_cols
+            * layer_act_operand_pres
+            / self.hd_param["input_bit_per_cycle"]
+            * macro_activation_times
+        )
+
+        # # energy of multiplier array
+        energy_mults = (
+            (self.logic_unit.get_1b_multiplier_energy() * layer_const_operand_pres)
+            * (mapped_rows_total * self.wl_dim_size)
+            * (layer_act_operand_pres / self.hd_param["input_bit_per_cycle"])
+            * macro_activation_times
+        )
 
-        """energy of adders_pv (type: RCA)"""
+        # # energy of adders_pv (type: RCA)
         nb_inputs_of_adder_pv = layer_const_operand_pres
         if nb_inputs_of_adder_pv == 1:
             energy_adders_pv = 0
         else:
             adder_pv_input_precision = self.hd_param["adc_resolution"]
-            nb_of_1b_adder_pv = adder_pv_input_precision * (nb_inputs_of_adder_pv-1) + nb_inputs_of_adder_pv*(math.log2(nb_inputs_of_adder_pv)-0.5)
-            energy_adders_pv = nb_of_1b_adder_pv * self.logic_unit.get_1b_adder_energy() * mapped_cols * \
-                               layer_act_operand_pres / self.hd_param["input_bit_per_cycle"] * macro_activation_times
+            nb_of_1b_adder_pv = adder_pv_input_precision * (nb_inputs_of_adder_pv - 1) + nb_inputs_of_adder_pv * (
+                math.log2(nb_inputs_of_adder_pv) - 0.5
+            )
+            energy_adders_pv = (
+                nb_of_1b_adder_pv
+                * self.logic_unit.get_1b_adder_energy()
+                * mapped_cols
+                * layer_act_operand_pres
+                / self.hd_param["input_bit_per_cycle"]
+                * macro_activation_times
+            )
 
-        """energy of accumulators (adder type: RCA)"""
+        # # energy of accumulators (adder type: RCA)
         if self.hd_param["input_bit_per_cycle"] == layer_act_operand_pres:
             energy_accumulators = 0
         else:
             accumulator_output_pres = layer_act_operand_pres + layer_const_operand_pres + math.log2(self.bl_dim_size)
-            energy_accumulators = (self.logic_unit.get_1b_adder_energy() + self.logic_unit.get_1b_reg_energy()) * accumulator_output_pres * \
-                                  mapped_cols * \
-                                  layer_act_operand_pres / self.hd_param["input_bit_per_cycle"] * macro_activation_times
+            energy_accumulators = (
+                (self.logic_unit.get_1b_adder_energy() + self.logic_unit.get_1b_reg_energy())
+                * accumulator_output_pres
+                * mapped_cols
+                * layer_act_operand_pres
+                / self.hd_param["input_bit_per_cycle"]
+                * macro_activation_times
+            )
 
-        self.energy_breakdown = { # unit: pJ (the unit borrowed from CACTI)
+        self.energy_breakdown = {  # unit: pJ (the unit borrowed from CACTI)
             "precharging": energy_precharging,
             "dacs": energy_dacs,
             "adcs": energy_adcs,
             "analog_bitlines": energy_cells,
             "mults": energy_mults,
             "adders_pv": energy_adders_pv,
-            "accumulators": energy_accumulators
+            "accumulators": energy_accumulators,
         }
         self.energy = sum([v for v in self.energy_breakdown.values()])
         return self.energy_breakdown
 
+
 if __name__ == "__main__":
-#
-##### IMC hardware dimension illustration (keypoint: adders' accumulation happens on D2)
-#
-#       |<------------------------ D1 ----------------------------->| (nb_of_columns/macro = D1 * weight_precision)
-#    -  +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++    \
-#    ^  +                                                           +  +  D3 (nb_of_macros)
-#    |  +         ^     +++++++                                     +   +  \
-#    |  +         |     +  W  +                                     +   +
-#    |  +   group_depth +++++++                                     +   +
-#    |  +         |     +  W  +                                     +   +
-#    |  +         v     +++++++                                     +   +
-#    |  +                  |                                        +   +
-#    |  +                  v                                        +   +
-#    |  +               multipliers -\                              +   +
-#    |  +        .                    \                             +   +
-#       +        .                     - adders (DIMC)              +   +
-#   D2  +        .                    / OR adcs (AIMC)              +   +
-#       +               multipliers -/       |                      +   +
-#    |  +                  ^                 |                      +   +
-#    |  +                  |                 |                      +   +
-#    |  +         ^     +++++++              v                      +   +
-#    |  +         |     +  W  +          adders_pv (place value)    +   +
-#    |  +   group_depth +++++++              |                      +   +
-#    |  +         |     +  W  +              v                      +   +
-#    |  +         v     +++++++         accumulators                +   +
-#    |  +                                    |                      +   +
-#    v  +                                    |                      +   +
-#    -  +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++   +
-#          +                                 |                        + +
-#           +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
-#   (nb_of_rows/macro = D2 * group_depth)    |
-#                                            v
-#                                        outputs
-#
+    #
+    # #### IMC hardware dimension illustration (keypoint: adders' accumulation happens on D2)
+    #
+    #       |<------------------------ D1 ----------------------------->| (nb_of_columns/macro = D1 * weight_precision)
+    #    -  +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++    \
+    #    ^  +                                                           +  +  D3 (nb_of_macros)
+    #    |  +         ^     +++++++                                     +   +  \
+    #    |  +         |     +  W  +                                     +   +
+    #    |  +   group_depth +++++++                                     +   +
+    #    |  +         |     +  W  +                                     +   +
+    #    |  +         v     +++++++                                     +   +
+    #    |  +                  |                                        +   +
+    #    |  +                  v                                        +   +
+    #    |  +               multipliers -\                              +   +
+    #    |  +        .                    \                             +   +
+    #       +        .                     - adders (DIMC)              +   +
+    #   D2  +        .                    / OR adcs (AIMC)              +   +
+    #       +               multipliers -/       |                      +   +
+    #    |  +                  ^                 |                      +   +
+    #    |  +                  |                 |                      +   +
+    #    |  +         ^     +++++++              v                      +   +
+    #    |  +         |     +  W  +          adders_pv (place value)    +   +
+    #    |  +   group_depth +++++++              |                      +   +
+    #    |  +         |     +  W  +              v                      +   +
+    #    |  +         v     +++++++         accumulators                +   +
+    #    |  +                                    |                      +   +
+    #    v  +                                    |                      +   +
+    #    -  +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++   +
+    #          +                                 |                        + +
+    #           +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+    #   (nb_of_rows/macro = D2 * group_depth)    |
+    #                                            v
+    #                                        outputs
+    #
     tech_param_28nm = {
-        "tech_node":0.028,              # unit: um
-        "vdd":      0.9,                # unit: V
-        "nd2_cap":  0.7/1e3,            # unit: pF
-        "xor2_cap": 0.7*1.5/1e3,        # unit: pF
-        "dff_cap":  0.7*3/1e3,          # unit: pF
-        "nd2_area": 0.614/1e6,          # unit: mm^2
-        "xor2_area":0.614*2.4/1e6,      # unit: mm^2
-        "dff_area": 0.614*6/1e6,        # unit: mm^2
-        "nd2_dly":  0.0478,             # unit: ns
-        "xor2_dly": 0.0478*2.4,         # unit: ns
+        "tech_node": 0.028,  # unit: um
+        "vdd": 0.9,  # unit: V
+        "nd2_cap": 0.7 / 1e3,  # unit: pF
+        "xor2_cap": 0.7 * 1.5 / 1e3,  # unit: pF
+        "dff_cap": 0.7 * 3 / 1e3,  # unit: pF
+        "nd2_area": 0.614 / 1e6,  # unit: mm^2
+        "xor2_area": 0.614 * 2.4 / 1e6,  # unit: mm^2
+        "dff_area": 0.614 * 6 / 1e6,  # unit: mm^2
+        "nd2_dly": 0.0478,  # unit: ns
+        "xor2_dly": 0.0478 * 2.4,  # unit: ns
         # "dff_dly":  0.0478*3.4,         # unit: ns
     }
     dimensions = {
-        "D1": 32/8, # wordline dimension
-        "D2": 32,   # bitline dimension
-        "D3": 1,    # nb_macros
+        "D1": 32 / 8,  # wordline dimension
+        "D2": 32,  # bitline dimension
+        "D3": 1,  # nb_macros
     }  # {"D1": ("K", 4), "D2": ("C", 32),}
 
-    """hd_param example for AIMC"""
+    # hd_param example for AIMC
     hd_param_aimc = {
-        "pe_type":              "in_sram_computing",    # required for CostModelStage
-        "imc_type":             "analog",               # "digital" or "analog". Or else: pure digital
-        "input_precision":      8,      # activation precision
-        "weight_precision":     8,      # weight precision
-        "input_bit_per_cycle":  2,      # nb_bits of input/cycle
-        "group_depth":          1,      # m factor
-        "adc_resolution":       8,      # adc resolution
-        "wordline_dimension":   "D1",   # wordline dimension
-        "bitline_dimension":    "D2",   # bitline dimension
-        "enable_cacti":         True,   # use CACTI to estimated cell array area cost (cell array exclude build-in logic part)
+        "pe_type": "in_sram_computing",  # required for CostModelStage
+        "imc_type": "analog",  # "digital" or "analog". Or else: pure digital
+        "input_precision": 8,  # activation precision
+        "weight_precision": 8,  # weight precision
+        "input_bit_per_cycle": 2,  # nb_bits of input/cycle
+        "group_depth": 1,  # m factor
+        "adc_resolution": 8,  # adc resolution
+        "wordline_dimension": "D1",  # wordline dimension
+        "bitline_dimension": "D2",  # bitline dimension
+        "enable_cacti": True,  # use CACTI to estimated cell array area cost (cell array exclude build-in logic part)
     }
-    hd_param_aimc["adc_resolution"] = hd_param_aimc["input_bit_per_cycle"] + 0.5*math.log2(dimensions["D2"])
+    hd_param_aimc["adc_resolution"] = hd_param_aimc["input_bit_per_cycle"] + 0.5 * math.log2(dimensions["D2"])
     aimc = AimcArray(tech_param_28nm, hd_param_aimc, dimensions)
     aimc.get_area()
     aimc.get_delay()
     logger = _logging.getLogger(__name__)
     logger.info(f"Total IMC area (mm^2): {aimc.area}")
     logger.info(f"area breakdown: {aimc.area_breakdown}")
     logger.info(f"delay (ns): {aimc.delay}")
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/DimcArray.py` & `zigzag_dse-3.1.1/zigzag/hardware/architecture/DimcArray.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,262 +1,320 @@
+"""
+README
+  . class DimcArray (defines the energy/area/delay cost of a DIMC array)
+How to use this file?
+  . This file is internally called in ZigZag-IMC framework.
+#   . It can also be run independently, for mainly debugging. An example is given at the end of the file.
+"""
+
 import numpy as np
 import math
 import copy
+
+from zigzag.workload.layer_node import LayerNode
+
 if __name__ == "__main__" or __name__ == "DimcArray":
     # branch when the script is run locally or called by AimcArray.py
     from imc_unit import ImcUnit
     import logging as _logging
+
     _logging_level = _logging.INFO
-    _logging_format = '%(asctime)s - %(funcName)s +%(lineno)s - %(levelname)s - %(message)s'
-    _logging.basicConfig(level=_logging_level,
-                         format=_logging_format)
+    _logging_format = "%(asctime)s - %(funcName)s +%(lineno)s - %(levelname)s - %(message)s"
+    _logging.basicConfig(level=_logging_level, format=_logging_format)
 else:
     import logging as _logging
-    from zigzag.classes.hardware.architecture.imc_unit import ImcUnit
+    from zigzag.hardware.architecture.imc_unit import ImcUnit
+
+
+class UserSpatialMappingGenerator:
+    """Dummy class to get rid of ruff lint check warnings.
+    This should be removed and the code should be updated accordingly.
+    """
 
-###############################################################################################################
-# README
-#   . class DimcArray (defines the energy/area/delay cost of a DIMC array)
-# How to use this file?
-#   . This file is internally called in ZigZag-IMC framework.
-#   . It can also be run independently, for mainly debugging. An example is given at the end of the file.
-###############################################################################################################
 
 class DimcArray(ImcUnit):
     # definition of a Digtal In-SRAM-Computing (DIMC) core
     # constraint:
     #     -- activation precision must be in the power of 2.
     #     -- input_bit_per_cycle must be in the power of 2.
-    def __init__(self,tech_param:dict, hd_param:dict, dimensions:dict):
+    def __init__(self, tech_param: dict, hd_param: dict, dimensions: dict):
         # @param tech_param: technology related parameters
         # @param hd_param: IMC cores' parameters
         # @param dimensions: IMC cores' dimensions
         super().__init__(tech_param, hd_param, dimensions)
 
     def __jsonrepr__(self):
         """
         JSON Representation of this class to save it to a json file.
         """
         # not implemented
-        #return {"operational_unit": self.unit, "dimensions": self.dimensions}
+        # return {"operational_unit": self.unit, "dimensions": self.dimensions}
         pass
 
-    ## area of imc macros (cells, mults, adders, adders_pv, accumulators. Not include input/output regs)
     def get_area(self):
+        """! area of imc macros (cells, mults, adders, adders_pv, accumulators. Not include input/output regs)"""
         # area of cell array
         tech_node = self.logic_unit.tech_param["tech_node"]
         group_depth = self.hd_param["group_depth"]
         w_pres = self.hd_param["weight_precision"]
         if self.hd_param["enable_cacti"] == True:
-            single_cell_array_area = self.get_single_cell_array_cost_from_cacti(tech_node,
-                                                                                self.wl_dim_size,
-                                                                                self.bl_dim_size,
-                                                                                group_depth,
-                                                                                w_pres)[1]
+            single_cell_array_area = self.get_single_cell_array_cost_from_cacti(
+                tech_node, self.wl_dim_size, self.bl_dim_size, group_depth, w_pres
+            )[1]
             # at this point, we have the area of single cell array. Then multiply it with the number of banks.
-            area_cells = single_cell_array_area * self.nb_of_banks # total cell array area in the core
+            area_cells = single_cell_array_area * self.nb_of_banks  # total cell array area in the core
         else:
             # TODO: [TO BE SUPPORTED OR YOU CAN MODIFY YOURSELF]
             area_cells = None  # user-provided cell array area (from somewhere?)
             raise Exception(f"User-provided cell area is not supported yet.")
 
-        """area of multiplier array"""
-        area_mults = self.logic_unit.get_1b_multiplier_area() * self.hd_param["input_bit_per_cycle"] * \
-                     w_pres * self.wl_dim_size * self.bl_dim_size * self.nb_of_banks
-
-        """area of adder trees (type: RCA)"""
-        adder_input_pres = w_pres # input precision of the adder tree
-        nb_inputs_of_adder = self.bl_dim_size # the number of inputs of the adder tree
+        # area of multiplier array
+        area_mults = (
+            self.logic_unit.get_1b_multiplier_area()
+            * self.hd_param["input_bit_per_cycle"]
+            * w_pres
+            * self.wl_dim_size
+            * self.bl_dim_size
+            * self.nb_of_banks
+        )
+
+        # area of adder trees (type: RCA)
+        adder_input_pres = w_pres  # input precision of the adder tree
+        nb_inputs_of_adder = self.bl_dim_size  # the number of inputs of the adder tree
         adder_depth = math.log2(nb_inputs_of_adder)
-        assert adder_depth%1==0, \
-            f"[DimcArray] The number of inputs [{nb_inputs_of_adder}] for the adder tree is not in the power of 2."
-        adder_depth = int(adder_depth) # float -> int for simplicity
-        adder_output_pres = adder_input_pres + adder_depth # output precision of the adder tree
-        nb_of_1b_adder_in_single_adder_tree = nb_inputs_of_adder * (adder_input_pres+1) - (adder_input_pres+adder_depth+1) # nb of 1b adders in a single adder tree
+        assert (
+            adder_depth % 1 == 0
+        ), f"[DimcArray] The number of inputs [{nb_inputs_of_adder}] for the adder tree is not in the power of 2."
+        adder_depth = int(adder_depth)  # float -> int for simplicity
+        adder_output_pres = adder_input_pres + adder_depth  # output precision of the adder tree
+        nb_of_1b_adder_in_single_adder_tree = nb_inputs_of_adder * (adder_input_pres + 1) - (
+            adder_input_pres + adder_depth + 1
+        )  # nb of 1b adders in a single adder tree
         nb_of_adder_trees = self.hd_param["input_bit_per_cycle"] * self.wl_dim_size * self.nb_of_banks
         area_adders = self.logic_unit.get_1b_adder_area() * nb_of_1b_adder_in_single_adder_tree * nb_of_adder_trees
 
-        """area of extra adders with place values (pv) when input_bit_per_cycle>1 (type: RCA)"""
+        # area of extra adders with place values (pv) when input_bit_per_cycle>1 (type: RCA)
         nb_inputs_of_adder_pv = self.hd_param["input_bit_per_cycle"]
         if nb_inputs_of_adder_pv == 1:
-            nb_of_1b_adder_pv = 0 # number of 1b adder in an pv_adder tree
-            nb_of_adder_trees_pv = 0 # number of pv_adder trees
+            nb_of_1b_adder_pv = 0  # number of 1b adder in an pv_adder tree
+            nb_of_adder_trees_pv = 0  # number of pv_adder trees
         else:
             adder_depth_pv = math.log2(nb_inputs_of_adder_pv)
             input_precision_pv = adder_output_pres
-            assert adder_depth_pv%1==0, \
-                f"[DimcArray] The value [{nb_inputs_of_adder_pv}] of [input_bit_per_cycle] is not in the power of 2."
-            adder_depth_pv = int(adder_depth_pv) # float -> int for simplicity
-            nb_of_1b_adder_pv = input_precision_pv * (nb_inputs_of_adder_pv-1) + nb_inputs_of_adder_pv * (adder_depth_pv-0.5) # nb of 1b adders in a single place-value adder tree
+            assert (
+                adder_depth_pv % 1 == 0
+            ), f"[DimcArray] The value [{nb_inputs_of_adder_pv}] of [input_bit_per_cycle] is not in the power of 2."
+            adder_depth_pv = int(adder_depth_pv)  # float -> int for simplicity
+            nb_of_1b_adder_pv = input_precision_pv * (nb_inputs_of_adder_pv - 1) + nb_inputs_of_adder_pv * (
+                adder_depth_pv - 0.5
+            )  # nb of 1b adders in a single place-value adder tree
             nb_of_adder_trees_pv = self.wl_dim_size * self.nb_of_banks
         area_adders_pv = self.logic_unit.get_1b_adder_area() * nb_of_1b_adder_pv * nb_of_adder_trees_pv
 
-        """area of accumulators (adder type: RCA)"""
+        # area of accumulators (adder type: RCA)
         if self.hd_param["input_bit_per_cycle"] == self.hd_param["input_precision"]:
             area_accumulators = 0
         else:
-            accumulator_output_pres = self.hd_param["input_precision"]+self.hd_param["weight_precision"]+math.log2(self.bl_dim_size)
-            nb_of_1b_adder_accumulator = accumulator_output_pres * self.wl_dim_size * self.nb_of_banks # number of 1b adder in all accumulators
-            nb_of_1b_reg_accumulator = nb_of_1b_adder_accumulator # number of regs in all accumulators
-            area_accumulators = self.logic_unit.get_1b_adder_area() * nb_of_1b_adder_accumulator + \
-                                self.logic_unit.get_1b_reg_area() * nb_of_1b_reg_accumulator
-        """total area of imc"""
-        self.area_breakdown = { # unit: same with in input hd file
-            "cells":    area_cells,
-            "mults":    area_mults,
-            "adders":   area_adders,
-            "adders_pv":area_adders_pv,
-            "accumulators": area_accumulators
+            accumulator_output_pres = (
+                self.hd_param["input_precision"] + self.hd_param["weight_precision"] + math.log2(self.bl_dim_size)
+            )
+            nb_of_1b_adder_accumulator = (
+                accumulator_output_pres * self.wl_dim_size * self.nb_of_banks
+            )  # number of 1b adder in all accumulators
+            nb_of_1b_reg_accumulator = nb_of_1b_adder_accumulator  # number of regs in all accumulators
+            area_accumulators = (
+                self.logic_unit.get_1b_adder_area() * nb_of_1b_adder_accumulator
+                + self.logic_unit.get_1b_reg_area() * nb_of_1b_reg_accumulator
+            )
+        # total area of imc
+        self.area_breakdown = {  # unit: same with in input hd file
+            "cells": area_cells,
+            "mults": area_mults,
+            "adders": area_adders,
+            "adders_pv": area_adders_pv,
+            "accumulators": area_accumulators,
         }
         self.area = sum([v for v in self.area_breakdown.values()])
         # return self.area_breakdown
 
     def get_delay(self):
-        """delay of imc arrays (worst path: mults -> adders -> adders_pv -> accumulators) """
-        """ unit: ns (if CACTI is used). whatever it can be otherwise. """
+        """delay of imc arrays (worst path: mults -> adders -> adders_pv -> accumulators)
+        unit: ns (if CACTI is used). whatever it can be otherwise."""
         dly_mults = self.logic_unit.get_1b_multiplier_dly()
 
-        """delay of adders (tree) (type: RCA)"""
+        # delay of adders (tree) (type: RCA)
         adder_input_pres = self.hd_param["weight_precision"]
         nb_inputs_of_adder = self.bl_dim_size
         adder_depth = math.log2(nb_inputs_of_adder)
-        assert adder_depth%1==0, \
-            f"[DimcArray] The number of inputs [{nb_inputs_of_adder}] for the adder tree is not in the power of 2."
+        assert (
+            adder_depth % 1 == 0
+        ), f"[DimcArray] The number of inputs [{nb_inputs_of_adder}] for the adder tree is not in the power of 2."
         adder_depth = int(adder_depth)  # float -> int for simplicity
         adder_output_pres = adder_input_pres + adder_depth
-        dly_adders = (adder_depth-1) * self.logic_unit.get_1b_adder_dly_in2sum() + \
-                     self.logic_unit.get_1b_adder_dly_in2cout() + \
-                     (adder_output_pres-1-1) * self.logic_unit.get_1b_adder_dly_cin2cout()
+        dly_adders = (
+            (adder_depth - 1) * self.logic_unit.get_1b_adder_dly_in2sum()
+            + self.logic_unit.get_1b_adder_dly_in2cout()
+            + (adder_output_pres - 1 - 1) * self.logic_unit.get_1b_adder_dly_cin2cout()
+        )
 
-        """delay of adders_pv (type: RCA)"""
+        # delay of adders_pv (type: RCA)
         nb_inputs_of_adder_pv = self.hd_param["input_bit_per_cycle"]
         if nb_inputs_of_adder_pv == 1:
             dly_adders_pv = 0
             accumulator_input_pres = adder_output_pres
         else:
             adder_depth_pv = math.log2(nb_inputs_of_adder_pv)
-            assert adder_depth_pv%1==0, \
-                f"[DimcArray] The value [{nb_inputs_of_adder_pv}] of [input_bit_per_cycle] is not in the power of 2."
+            assert (
+                adder_depth_pv % 1 == 0
+            ), f"[DimcArray] The value [{nb_inputs_of_adder_pv}] of [input_bit_per_cycle] is not in the power of 2."
             adder_depth_pv = int(adder_depth_pv)  # float -> int for simplicity
             adder_pv_input_precision = adder_output_pres
-            adder_pv_output_precision = nb_inputs_of_adder_pv + adder_output_pres  # output precision from adders_pv (depth + input_precision)
+            adder_pv_output_precision = (
+                nb_inputs_of_adder_pv + adder_output_pres
+            )  # output precision from adders_pv (depth + input_precision)
             accumulator_input_pres = adder_pv_output_precision
-            dly_adders_pv = (adder_depth_pv - 1) * self.logic_unit.get_1b_adder_dly_in2sum() + self.logic_unit.get_1b_adder_dly_in2cout() + (adder_pv_output_precision - adder_pv_input_precision-1) * self.logic_unit.get_1b_adder_dly_cin2cout()
-
-        """delay of accumulators (adder type: RCA)"""
-        accumulator_output_pres = self.hd_param["input_precision"] + self.hd_param["weight_precision"] + math.log2(self.bl_dim_size)
-        accumulator_output_pres = int(accumulator_output_pres) # float -> int for simplicity
-        if accumulator_output_pres == accumulator_input_pres: # no accumulator
+            dly_adders_pv = (
+                (adder_depth_pv - 1) * self.logic_unit.get_1b_adder_dly_in2sum()
+                + self.logic_unit.get_1b_adder_dly_in2cout()
+                + (adder_pv_output_precision - adder_pv_input_precision - 1)
+                * self.logic_unit.get_1b_adder_dly_cin2cout()
+            )
+
+        # delay of accumulators (adder type: RCA)
+        accumulator_output_pres = (
+            self.hd_param["input_precision"] + self.hd_param["weight_precision"] + math.log2(self.bl_dim_size)
+        )
+        accumulator_output_pres = int(accumulator_output_pres)  # float -> int for simplicity
+        if accumulator_output_pres == accumulator_input_pres:  # no accumulator
             dly_accumulators = 0
         else:
-            dly_accumulators = self.logic_unit.get_1b_adder_dly_in2cout() + \
-                               (accumulator_output_pres - accumulator_input_pres) * self.logic_unit.get_1b_adder_dly_cin2cout()
+            dly_accumulators = (
+                self.logic_unit.get_1b_adder_dly_in2cout()
+                + (accumulator_output_pres - accumulator_input_pres) * self.logic_unit.get_1b_adder_dly_cin2cout()
+            )
 
-        """total delay of imc"""
+        # total delay of imc
         self.delay_breakdown = {
-            "mults":    dly_mults,
-            "adders":   dly_adders,
-            "adders_pv":dly_adders_pv,
-            "accumulators": dly_accumulators
+            "mults": dly_mults,
+            "adders": dly_adders,
+            "adders_pv": dly_adders_pv,
+            "accumulators": dly_accumulators,
         }
         self.delay = sum([v for v in self.delay_breakdown.values()])
         # return self.delay_breakdown
 
     def get_peak_energy_single_cycle(self):
         """
         macro-level one-cycle energy of imc arrays (fully utilization, no weight updating)
         (components: cells, mults, adders, adders_pv, accumulators. Not include input/output regs)
         """
         w_pres = self.hd_param["weight_precision"]
-        """energy of precharging"""
+        # energy of precharging
         energy_precharging = 0
 
-        """energy of multiplier array"""
-        nb_of_mults = self.hd_param["input_bit_per_cycle"] * \
-                     w_pres * self.wl_dim_size * self.bl_dim_size * self.nb_of_banks
+        # energy of multiplier array
+        nb_of_mults = (
+            self.hd_param["input_bit_per_cycle"] * w_pres * self.wl_dim_size * self.bl_dim_size * self.nb_of_banks
+        )
         energy_mults = self.logic_unit.get_1b_multiplier_energy() * nb_of_mults
 
-        """energy of adder trees (type: RCA)"""
-        adder_input_pres = w_pres # input precision of the adder tree
-        nb_inputs_of_adder = self.bl_dim_size # the number of inputs of the adder tree
+        # energy of adder trees (type: RCA)
+        adder_input_pres = w_pres  # input precision of the adder tree
+        nb_inputs_of_adder = self.bl_dim_size  # the number of inputs of the adder tree
         adder_depth = math.log2(nb_inputs_of_adder)
-        assert adder_depth%1==0, \
-            f"[DimcArray] The number of inputs [{nb_inputs_of_adder}] for the adder tree is not in the power of 2."
-        adder_depth = int(adder_depth) # float -> int for simplicity
-        adder_output_pres = adder_input_pres + adder_depth # output precision of the adder tree
-        nb_of_1b_adder_in_single_adder_tree = nb_inputs_of_adder * (adder_input_pres+1) - (adder_input_pres+adder_depth+1) # nb of 1b adders in a single adder tree
+        assert (
+            adder_depth % 1 == 0
+        ), f"[DimcArray] The number of inputs [{nb_inputs_of_adder}] for the adder tree is not in the power of 2."
+        adder_depth = int(adder_depth)  # float -> int for simplicity
+        adder_output_pres = adder_input_pres + adder_depth  # output precision of the adder tree
+        nb_of_1b_adder_in_single_adder_tree = nb_inputs_of_adder * (adder_input_pres + 1) - (
+            adder_input_pres + adder_depth + 1
+        )  # nb of 1b adders in a single adder tree
         nb_of_adder_trees = self.hd_param["input_bit_per_cycle"] * self.wl_dim_size * self.nb_of_banks
         energy_adders = self.logic_unit.get_1b_adder_energy() * nb_of_1b_adder_in_single_adder_tree * nb_of_adder_trees
 
-        """energy of adders_pv (type: RCA)"""
+        # energy of adders_pv (type: RCA)
         nb_inputs_of_adder_pv = self.hd_param["input_bit_per_cycle"]
         if nb_inputs_of_adder_pv == 1:
             energy_adders_pv = 0
         else:
             adder_pv_input_precision = adder_output_pres
-            nb_of_1b_adder_pv = adder_pv_input_precision * (nb_inputs_of_adder_pv - 1) + nb_inputs_of_adder_pv * (math.log2(nb_inputs_of_adder_pv) - 0.5)
+            nb_of_1b_adder_pv = adder_pv_input_precision * (nb_inputs_of_adder_pv - 1) + nb_inputs_of_adder_pv * (
+                math.log2(nb_inputs_of_adder_pv) - 0.5
+            )
             nb_of_adder_trees_pv = self.wl_dim_size * self.nb_of_banks
             energy_adders_pv = self.logic_unit.get_1b_adder_energy() * nb_of_1b_adder_pv * nb_of_adder_trees_pv
 
-        """energy of accumulators (adder type: RCA)"""
+        # energy of accumulators (adder type: RCA)
         if self.hd_param["input_bit_per_cycle"] == self.hd_param["input_precision"]:
             energy_accumulators = 0
         else:
-            accumulator_output_pres = self.hd_param["input_precision"]+self.hd_param["weight_precision"]+math.log2(self.bl_dim_size)
-            nb_of_1b_adder_accumulator = accumulator_output_pres * self.wl_dim_size * self.nb_of_banks # number of 1b adder in all accumulators
-            nb_of_1b_reg_accumulator = nb_of_1b_adder_accumulator # number of regs in all accumulators
-            energy_accumulators = self.logic_unit.get_1b_adder_energy() * nb_of_1b_adder_accumulator + \
-                                self.logic_unit.get_1b_reg_energy() * nb_of_1b_reg_accumulator
+            accumulator_output_pres = (
+                self.hd_param["input_precision"] + self.hd_param["weight_precision"] + math.log2(self.bl_dim_size)
+            )
+            nb_of_1b_adder_accumulator = (
+                accumulator_output_pres * self.wl_dim_size * self.nb_of_banks
+            )  # number of 1b adder in all accumulators
+            nb_of_1b_reg_accumulator = nb_of_1b_adder_accumulator  # number of regs in all accumulators
+            energy_accumulators = (
+                self.logic_unit.get_1b_adder_energy() * nb_of_1b_adder_accumulator
+                + self.logic_unit.get_1b_reg_energy() * nb_of_1b_reg_accumulator
+            )
 
         peak_energy_breakdown = {  # unit: pJ (the unit borrowed from CACTI)
             "precharging": energy_precharging,
             "mults": energy_mults,
             "adders": energy_adders,
             "adders_pv": energy_adders_pv,
-            "accumulators": energy_accumulators
+            "accumulators": energy_accumulators,
         }
         # peak_energy = sum([v for v in peak_energy_breakdown.values()])
         return peak_energy_breakdown
 
     def get_macro_level_peak_performance(self):
         """
         macro-level peak performance of imc arrays (fully utilization, no weight updating)
         """
-        nb_of_macs_per_cycle = self.wl_dim_size * self.bl_dim_size / \
-                               (self.hd_param["input_precision"] / self.hd_param["input_bit_per_cycle"]) * \
-                               self.nb_of_banks
+        nb_of_macs_per_cycle = (
+            self.wl_dim_size
+            * self.bl_dim_size
+            / (self.hd_param["input_precision"] / self.hd_param["input_bit_per_cycle"])
+            * self.nb_of_banks
+        )
 
         self.get_area()
         self.get_delay()
 
-        clock_cycle_period = self.delay # unit: ns
-        peak_energy_per_cycle = sum([v for v in self.get_peak_energy_single_cycle().values()]) # unit: pJ
-        imc_area = self.area # unit: mm^2
+        clock_cycle_period = self.delay  # unit: ns
+        peak_energy_per_cycle = sum([v for v in self.get_peak_energy_single_cycle().values()])  # unit: pJ
+        imc_area = self.area  # unit: mm^2
 
         tops_peak = nb_of_macs_per_cycle * 2 / clock_cycle_period / 1000
         topsw_peak = nb_of_macs_per_cycle * 2 / peak_energy_per_cycle
         topsmm2_peak = tops_peak / imc_area
 
         logger = _logging.getLogger(__name__)
         logger.info(f"Current macro-level peak performance:")
         logger.info(f"TOP/s: {tops_peak}, TOP/s/W: {topsw_peak}, TOP/s/mm^2: {topsmm2_peak}")
 
         return tops_peak, topsw_peak, topsmm2_peak
 
     @staticmethod
-    def calculate_mapped_rows_total_when_diagonal_mapping_found(layer, layer_const_operand, layer_act_operand, sm_on_wl_dim, sm_on_bl_dim):
+    def calculate_mapped_rows_total_when_diagonal_mapping_found(
+        layer: LayerNode, layer_const_operand, layer_act_operand, sm_on_wl_dim, sm_on_bl_dim
+    ):
         # This function is used for calcualting the total mapped number of rows when OX, OY unroll is found,
         # which requires a diagonal data mapping.
         # If OX, OY unroll does not exist, you can also use this function to calculate the total mapped number of rows.
         # The only drawback is the simulation time is longer.
         # First, fetch the dimension name of OX / OY (they are weight ir loops)
-        weight_ir_layer_dims: list = layer.operand_loop_dim[layer_const_operand]["ir"]
+        weight_ir_layer_dims = layer.loop_relevancy_info.get_ir_layer_dims(layer_const_operand)
         # Second, we will find out what pr loops they pair with. Create a dict to record them down for later use.
         # For neural network, OX pairs with FX, OY with FY. So, it is assumed the pair size is in 2.
-        act_pr_layer_dims: dict = layer.operand_loop_dim[layer_act_operand]["pr"]
+        act_pr_layer_dims = layer.loop_relevancy_info.get_pr_layer_dims(layer_act_operand)
         pr_sm: dict = {}
         pr_sm_link: dict = {}
         for [layer_dim1, layer_dim2] in act_pr_layer_dims.values():
             # for weight_ir_layer_dim in weight_ir_layer_dims:
             if layer_dim1 in weight_ir_layer_dims:
                 pr_sm[layer_dim2] = {layer_dim1: 1}  # 1 by default, which means no mapping found
                 pr_sm_link[layer_dim1] = layer_dim2
@@ -277,17 +335,17 @@
         # Then, we calculate the total mapped number of rows
         # mapped_rows_total: used for energy estimation of wordline and multipliers
         # mapped_rows_for_adder: number of activated inputs of an adder tree, used for energy estimation of adder trees
         if isinstance(sm_on_bl_dim[0], str):  # single layer mapping
             layer_dim = sm_on_bl_dim[0]
             layer_dim_size = sm_on_bl_dim[1]
             # pr_sm.keys() include FX, FY
-            if layer_dim not in pr_sm.keys(): # e.g. ("C", 2)
+            if layer_dim not in pr_sm.keys():  # e.g. ("C", 2)
                 additional_diag_rows = 0
-            else: # e.g. ("FX", 2)
+            else:  # e.g. ("FX", 2)
                 additional_diag_rows = list(pr_sm[layer_dim].values())[0] - 1
             mapped_rows_total = layer_dim_size + additional_diag_rows
             mapped_rows_for_adder = layer_dim_size
         else:  # mix layer_dim mapping (e.g. (("C",2), ("FX",2)) )
             # mapped_rows_total = Cu * (OYu + FYu - 1) * (OXu + FXu - 1)
             # mapped_rows_for_adder = Cu * FYu * FXu
             # In reality, OXu, OYu will not both exist. But the function still support this by the equation above.
@@ -296,29 +354,31 @@
             for element in sm_on_bl_dim:
                 layer_dim = element[0]
                 layer_dim_size = element[1]
                 if layer_dim not in pr_sm.keys():
                     additional_diag_rows = 0
                 else:
                     additional_diag_rows = list(pr_sm[layer_dim].values())[0] - 1
-                mapped_rows_total *= (layer_dim_size + additional_diag_rows)
+                mapped_rows_total *= layer_dim_size + additional_diag_rows
                 mapped_rows_for_adder *= layer_dim_size
         # Lastly, ceil to an upper integer, as required in the adder-trees model.
         mapped_rows_total = math.ceil(mapped_rows_total)
         mapped_rows_for_adder = math.ceil(mapped_rows_for_adder)
         return mapped_rows_total, mapped_rows_for_adder
 
     @staticmethod
     def get_mapped_oa_dim(layer, wl_dim, bl_dim):
         """
         get the mapped oa_dim in current mapping. The energy of unmapped oa_dim will be set to 0.
         """
 
         # activation/weight representation
-        layer_act_operand, layer_const_operand = DimcArray.identify_layer_operand_representation(layer)
+        layer_act_operand, layer_const_operand = UserSpatialMappingGenerator.identify_layer_operand_representation(
+            layer
+        )
 
         spatial_mapping = copy.deepcopy(layer.user_spatial_mapping)
 
         # Figure out the spatial mapping in a single macro
         spatial_mapping_in_macro = []
         for layer_dim, loop in spatial_mapping.items():
             if layer_dim in [wl_dim, bl_dim]:  # serve the dimension inside the macro
@@ -329,346 +389,424 @@
                         spatial_mapping_in_macro.append(element)
 
         # We will firstly derive how many number of PE columns and rows are mapping.
         # Later, energy of unmapped rows and columns will be set to 0.
         # We start from deriving the number of mapped columns in each macro.
         # the sm loop would do not exist if did not find any
         if wl_dim not in spatial_mapping.keys():
-            mapped_cols = 1 # mapped number of wl dims
+            mapped_cols = 1  # mapped number of wl dims
             weight_ir_loop_on_wl_dim = False  # if there is OX / OY mapped on wl dims
         else:
             sm_on_wl_dim = spatial_mapping[wl_dim]  # spatial mapping on wl_dimension
             if isinstance(sm_on_wl_dim[0], str):  # single layer mapping (e.g. ("K", 2))
                 mapped_cols = sm_on_wl_dim[1]  # floating number is also supported for calculation
             else:  # mix layer_dim mapping (e.g. (("K",2), ("OX",2)) )
                 mapped_cols = math.prod([v[1] for v in sm_on_wl_dim])
             # We then calculate the number of mapped rows in each macro.
             # As there might be OX / OY unrolling, which results in a diagonal mapping, we will have a special check on that
             # Firstly check if there is OX / OY unrolling
-            weight_ir_layer_dims: list = layer.operand_loop_dim[layer_const_operand]["ir"]
+            weight_ir_layer_dims: list = layer[layer_const_operand]["ir"]
             weight_ir_loop_on_wl_dim = False  # set default value
             if isinstance(sm_on_wl_dim[0], str):  # single layer mapping (e.g. ("K", 2))
                 weight_ir_loop_on_wl_dim = True if sm_on_wl_dim[0] in weight_ir_layer_dims else False
             else:  # mix layer_dim mapping (e.g. (("K",2), ("OX",2)) )
                 for element in sm_on_wl_dim:
                     layer_dim = element[0]
                     if layer_dim in weight_ir_layer_dims:
                         weight_ir_loop_on_wl_dim = True
                         break
 
         # Calculate total mapped number of rows
         if bl_dim in spatial_mapping.keys():
             sm_on_bl_dim = spatial_mapping[bl_dim]  # spatial mapping on bl_dimension
-            if not weight_ir_loop_on_wl_dim:  # if False: mean there is no OX / OY unrolling on wl_dim, so no diagonal unrolling required
+            if (
+                not weight_ir_loop_on_wl_dim
+            ):  # if False: mean there is no OX / OY unrolling on wl_dim, so no diagonal unrolling required
                 if isinstance(sm_on_bl_dim[0], str):  # single layer mapping (e.g. ("FX", 2))
                     mapped_rows_total = sm_on_bl_dim[1]  # floating number is also supported for calculation
                 else:  # mix layer_dim mapping (e.g. (("C",2), ("FX",2)) )
                     mapped_rows_total = math.prod([v[1] for v in sm_on_bl_dim])
                 mapped_rows_total = math.ceil(mapped_rows_total)  # must be an integer, as it is used for adder trees.
                 mapped_rows_for_adder = mapped_rows_total
             else:
-                mapped_rows_total, mapped_rows_for_adder = DimcArray.calculate_mapped_rows_total_when_diagonal_mapping_found(
-                    layer,
-                    layer_const_operand,
-                    layer_act_operand,
-                    sm_on_wl_dim,
-                    sm_on_bl_dim)
-        else: # there is no sm loop on bl_dim
+                mapped_rows_total, mapped_rows_for_adder = (
+                    DimcArray.calculate_mapped_rows_total_when_diagonal_mapping_found(
+                        layer,
+                        layer_const_operand,
+                        layer_act_operand,
+                        sm_on_wl_dim,
+                        sm_on_bl_dim,
+                    )
+                )
+        else:  # there is no sm loop on bl_dim
             mapped_rows_total = 1
             mapped_rows_for_adder = 1
 
         # Get the number of time of activating macro
         # Note: it is normalized to a hardware that has only one macro (see equation below)
         # Equation = total MAC number of a layer/spatial mapping on a single macro
         macro_activation_times = layer.total_MAC_count / np.prod([x[1] for x in spatial_mapping_in_macro])
-        return mapped_rows_total, mapped_rows_for_adder, mapped_cols, macro_activation_times
+        return (
+            mapped_rows_total,
+            mapped_rows_for_adder,
+            mapped_cols,
+            macro_activation_times,
+        )
 
     @staticmethod
-    def get_precharge_energy(hd_param, tech_param, layer, mapping):
+    def get_precharge_energy(hd_param, tech_param, layer: LayerNode, mapping):
         # calculate pre-charging energy on local bitlines for specific layer and mapping
         # also calculate mapped group depth (number of weights stored in a cell group)
         group_depth = hd_param["group_depth"]
         if group_depth > 1:
             # Pre-charge operation is required on local bitline if group_depth > 1
             # The final pre-charge energy = energy/PE * nb_of_precharge_times
             # nb_of_precharge_times is normalized to single PE.
 
             # activation/weight representation
-            layer_act_operand, layer_const_operand = DimcArray.identify_layer_operand_representation(layer)
+            layer_act_operand, layer_const_operand = UserSpatialMappingGenerator.identify_layer_operand_representation(
+                layer
+            )
 
             # Get the precharge interval between two precharge operations
             precharge_interval = 1  # 1: precharge every cycle
             tm_loops_in_cell_group: list = mapping.temporal_mapping.mapping_dic_origin[layer_const_operand][0]
             # As loops close to the beginning will be executed firstly, we will count how many weight ir loops there are
             # until we reach a weight r loop
-            weight_r_layer_dims: list = layer.operand_loop_dim[layer_const_operand]["r"]
-            weight_ir_layer_dims: list = layer.operand_loop_dim[layer_const_operand]["ir"]
-            for (loop_name, loop_size) in tm_loops_in_cell_group:
+            weight_r_layer_dims = layer.loop_relevancy_info.get_r_layer_dims(layer_const_operand)
+            weight_ir_layer_dims = layer.loop_relevancy_info.get_ir_layer_dims(layer_const_operand)
+
+            for loop_name, loop_size in tm_loops_in_cell_group:
                 if loop_name in weight_ir_layer_dims:
                     precharge_interval *= loop_size
                 else:
                     break  # break when we meet the first ir loop of weight
             # Equation: nb_of_precharge_times = rd_out_to_low_count_of_lowest_weight_mem / precharge_intervals
-            nb_of_precharge_times = mapping.unit_mem_data_movement[layer_const_operand][0].data_elem_move_count.rd_out_to_low / precharge_interval
-            single_pe_precharge_energy = ((tech_param["wl_cap"] * (tech_param["vdd"] ** 2)) + \
-                                          (tech_param["bl_cap"] * (tech_param["vdd"] ** 2) * group_depth)) * \
-                                         (hd_param["weight_precision"])
+            nb_of_precharge_times = (
+                mapping.unit_mem_data_movement[layer_const_operand][0].data_elem_move_count.rd_out_to_low
+                / precharge_interval
+            )
+            single_pe_precharge_energy = (
+                (tech_param["wl_cap"] * (tech_param["vdd"] ** 2))
+                + (tech_param["bl_cap"] * (tech_param["vdd"] ** 2) * group_depth)
+            ) * (hd_param["weight_precision"])
             energy_precharging = single_pe_precharge_energy * nb_of_precharge_times
             # Calculate mapped_group_depth
             mapped_group_depth = 1
-            for (loop_name, loop_size) in tm_loops_in_cell_group:
+            for loop_name, loop_size in tm_loops_in_cell_group:
                 if loop_name in weight_r_layer_dims:
                     mapped_group_depth *= loop_size
         else:
             energy_precharging = 0
             mapped_group_depth = 1
         return energy_precharging, mapped_group_depth
 
-    def get_mults_energy(self, hd_param, logic_unit, layer, mapped_rows_total, wl_dim_size, macro_activation_times) -> float:
+    def get_mults_energy(
+        self,
+        hd_param,
+        logic_unit,
+        layer,
+        mapped_rows_total,
+        wl_dim_size,
+        macro_activation_times,
+    ) -> float:
         """
         calculate energy spent on multipliers for specific layer and mapping
         """
         # activation/weight representation
-        layer_act_operand, layer_const_operand = self.identify_layer_operand_representation(layer)
+        layer_act_operand, layer_const_operand = UserSpatialMappingGenerator.identify_layer_operand_representation(
+            layer
+        )
 
         layer_act_operand_pres = layer.operand_precision[layer_act_operand]
-        nb_of_mapped_mults_in_macro = hd_param["weight_precision"] * hd_param["input_bit_per_cycle"] * \
-                                      mapped_rows_total * wl_dim_size
-        nb_of_activation_times = macro_activation_times * \
-                                 (layer_act_operand_pres / hd_param["input_bit_per_cycle"])
+        nb_of_mapped_mults_in_macro = (
+            hd_param["weight_precision"] * hd_param["input_bit_per_cycle"] * mapped_rows_total * wl_dim_size
+        )
+        nb_of_activation_times = macro_activation_times * (layer_act_operand_pres / hd_param["input_bit_per_cycle"])
         energy_mults = logic_unit.get_1b_multiplier_energy() * nb_of_mapped_mults_in_macro * nb_of_activation_times
         return energy_mults
 
-    def get_adder_trees_energy(self, layer, logic_unit, mapped_rows_for_adder, bl_dim_size, mapped_cols, layer_act_operand_pres, macro_activation_times):
+    def get_adder_trees_energy(
+        self,
+        layer,
+        logic_unit,
+        mapped_rows_for_adder,
+        bl_dim_size,
+        mapped_cols,
+        layer_act_operand_pres,
+        macro_activation_times,
+    ):
         """
         get the energy spent on RCA adder trees for specific layer and mapping
         """
         # activation/weight representation
-        layer_act_operand, layer_const_operand = self.identify_layer_operand_representation(layer)
+        layer_act_operand, layer_const_operand = UserSpatialMappingGenerator.identify_layer_operand_representation(
+            layer
+        )
 
         layer_const_operand_pres = layer.operand_precision[layer_const_operand]
         nb_inputs_of_adder = bl_dim_size  # physical number of inputs in a single adder tree
         adder_depth = math.log2(nb_inputs_of_adder)
-        assert nb_inputs_of_adder % 1 == 0, \
-            f"The number of inputs for an adder tree [{nb_inputs_of_adder}] is not in the power of 2."
+        assert (
+            nb_inputs_of_adder % 1 == 0
+        ), f"The number of inputs for an adder tree [{nb_inputs_of_adder}] is not in the power of 2."
         adder_depth = int(adder_depth)  # float -> int for simplicity
         mapped_inputs = mapped_rows_for_adder  # number of used inputs for an adder tree
         adder_input_pres = layer_const_operand_pres  # input precision for a single adder tree
         adder_output_pres = adder_input_pres + adder_depth
-        nb_of_1b_adder = nb_inputs_of_adder * (adder_input_pres + 1) - (adder_input_pres + adder_depth + 1)  # nb of 1b adders in a single adder tree
+        # nb of 1b adders in a single adder tree
+        nb_of_1b_adder = nb_inputs_of_adder * (adder_input_pres + 1) - (adder_input_pres + adder_depth + 1)
 
         # In the adders' model, we classify the basic FA (1-b full adder) as two types:
         # 1. fully activated FA: two of its inputs having data comes in. (higher energy cost)
         # 2. half activated FA: only one of its inputs having data comes in.
         # The 2nd type has lower energy cost, because no carry will be generated and the carry path stays unchanged.
         # Below we figure out how many there are of fully activated FA and half activated FA
         if mapped_inputs >= 1:
             if mapped_inputs >= nb_inputs_of_adder:
-                """
-                :param fully_activated_number_of_1b_adder: fully activated 1b adder, probably will produce a carry
-                :param half_activated_number_of_1b_adder: only 1 input is activate and the other port is 0, so carry path is activated.
-                """
+                # :param fully_activated_number_of_1b_adder: fully activated 1b adder, probably will produce a carry
+                # :param half_activated_number_of_1b_adder: only 1 input is activate and the other port is 0, so carry path is activated.
+
                 fully_activated_number_of_1b_adder = nb_of_1b_adder
                 half_activated_number_of_1b_adder = 0
             else:
-                """
-                find out fully_activated_number_of_1b_adder and half_activated_number_of_1b_adder when inputs are not fully mapped.
-                method: iteratively check if left_input is bigger or smaller than baseline, which will /2 each time, until left_input == 1
-                :param left_input: the number of inputs waiting for processing
-                :param baseline: serves as references for left_input
-                """
+
+                # find out fully_activated_number_of_1b_adder and half_activated_number_of_1b_adder when inputs are not fully mapped.
+                # method: iteratively check if left_input is bigger or smaller than baseline, which will /2 each time, until left_input == 1
+                # :param left_input: the number of inputs waiting for processing
+                # :param baseline: serves as references for left_input
+
                 fully_activated_number_of_1b_adder = 0
                 half_activated_number_of_1b_adder = 0
                 left_input = mapped_inputs
                 baseline = nb_inputs_of_adder
                 while left_input != 0:
                     baseline = baseline / 2
                     activated_depth = int(math.log2(baseline))
                     if left_input <= 1 and baseline == 1:  # special case
                         fully_activated_number_of_1b_adder += 0
                         half_activated_number_of_1b_adder += adder_input_pres
                         left_input = 0
                     elif left_input > baseline:
-                        fully_activated_number_of_1b_adder += baseline * (adder_input_pres + 1) - (adder_input_pres + activated_depth + 1) + (adder_input_pres + activated_depth)
+                        fully_activated_number_of_1b_adder += (
+                            baseline * (adder_input_pres + 1)
+                            - (adder_input_pres + activated_depth + 1)
+                            + (adder_input_pres + activated_depth)
+                        )
                         half_activated_number_of_1b_adder += 0
                         left_input = left_input - baseline
                     elif left_input < baseline:
                         half_activated_number_of_1b_adder += adder_input_pres + activated_depth
                     else:  # left_input == baseline
-                        fully_activated_number_of_1b_adder += baseline * (adder_input_pres + 1) - (adder_input_pres + activated_depth + 1)
+                        fully_activated_number_of_1b_adder += baseline * (adder_input_pres + 1) - (
+                            adder_input_pres + activated_depth + 1
+                        )
                         half_activated_number_of_1b_adder += adder_input_pres + activated_depth
                         left_input = left_input - baseline
 
-            single_adder_tree_energy = fully_activated_number_of_1b_adder * logic_unit.get_1b_adder_energy() + \
-                                       half_activated_number_of_1b_adder * logic_unit.get_1b_adder_energy_half_activated()
+            single_adder_tree_energy = (
+                fully_activated_number_of_1b_adder * logic_unit.get_1b_adder_energy()
+                + half_activated_number_of_1b_adder * logic_unit.get_1b_adder_energy_half_activated()
+            )
             nb_of_activation_times = mapped_cols * layer_act_operand_pres * macro_activation_times
             energy_adders = single_adder_tree_energy * nb_of_activation_times
         else:
             energy_adders = 0
         return energy_adders, adder_output_pres
 
-    def get_adder_pv_energy(self, nb_inputs_of_adder_pv, input_precision, logic_unit, layer_act_operand_pres, input_bit_per_cycle, mapped_cols, macro_activation_times):
+    def get_adder_pv_energy(
+        self,
+        nb_inputs_of_adder_pv,
+        input_precision,
+        logic_unit,
+        layer_act_operand_pres,
+        input_bit_per_cycle,
+        mapped_cols,
+        macro_activation_times,
+    ):
         """
         get the energy for adder tree with input having place value (pv)
         """
         if nb_inputs_of_adder_pv == 1:
             energy_adders_pv = 0
         else:
             adder_pv_input_precision = input_precision
-            nb_of_1b_adder_pv = adder_pv_input_precision * (nb_inputs_of_adder_pv - 1) + nb_inputs_of_adder_pv * (math.log2(nb_inputs_of_adder_pv) - 0.5)
+            nb_of_1b_adder_pv = adder_pv_input_precision * (nb_inputs_of_adder_pv - 1) + nb_inputs_of_adder_pv * (
+                math.log2(nb_inputs_of_adder_pv) - 0.5
+            )
             nb_of_activation_times = mapped_cols * layer_act_operand_pres / input_bit_per_cycle * macro_activation_times
             energy_adders_pv = logic_unit.get_1b_adder_energy() * nb_of_1b_adder_pv * nb_of_activation_times
         return energy_adders_pv
 
     def get_energy_for_a_layer(self, layer, mapping):
         """
         get the imc array energy for specific layer with specific mapping
-        """
-        """check if operand precision defined in the layer is the same with in hardware template"""
+        check if operand precision defined in the layer is the same with in hardware template"""
         # activation/weight representation
-        layer_act_operand, layer_const_operand = self.identify_layer_operand_representation(layer)
+        layer_act_operand, layer_const_operand = UserSpatialMappingGenerator.identify_layer_operand_representation(
+            layer
+        )
 
         layer_const_operand_pres = layer.operand_precision[layer_const_operand]
         layer_act_operand_pres = layer.operand_precision[layer_act_operand]
         weight_pres_in_hd_param = self.hd_param["weight_precision"]
         act_pres_in_hd_param = self.hd_param["input_precision"]
 
         # currently in the energy model, the input and weight precision defined in the workload file should be the same with in the hd input file.
         # this check can be removed if variable precision is supported in the future.
-        assert layer_const_operand_pres == weight_pres_in_hd_param, \
-                f"Weight precision defined in the workload [{layer_const_operand_pres}] not equal to the one defined in the hardware hd_param [{weight_pres_in_hd_param}]."
-        assert layer_act_operand_pres == act_pres_in_hd_param, \
-                f"Activation precision defined in the workload [{layer_act_operand_pres}] not equal to the one defined in the hardware hd_param [{act_pres_in_hd_param}]."
-
-        """parameter extraction"""
-        mapped_rows_total, mapped_rows_for_adder, mapped_cols, macro_activation_times = DimcArray.get_mapped_oa_dim(layer, self.wl_dim, self.bl_dim)
+        assert (
+            layer_const_operand_pres == weight_pres_in_hd_param
+        ), f"Weight precision defined in the workload [{layer_const_operand_pres}] not equal to the one defined in the hardware hd_param [{weight_pres_in_hd_param}]."
+        assert (
+            layer_act_operand_pres == act_pres_in_hd_param
+        ), f"Activation precision defined in the workload [{layer_act_operand_pres}] not equal to the one defined in the hardware hd_param [{act_pres_in_hd_param}]."
+
+        # parameter extraction
+        (
+            mapped_rows_total,
+            mapped_rows_for_adder,
+            mapped_cols,
+            macro_activation_times,
+        ) = DimcArray.get_mapped_oa_dim(layer, self.wl_dim, self.bl_dim)
         self.mapped_rows_total = mapped_rows_total
 
-        """energy calculation"""
-        """energy of precharging"""
-        energy_precharging, mapped_group_depth = DimcArray.get_precharge_energy(self.hd_param, self.logic_unit.tech_param, layer, mapping)
+        # energy calculation
+        # energy of precharging
+        energy_precharging, mapped_group_depth = DimcArray.get_precharge_energy(
+            self.hd_param, self.logic_unit.tech_param, layer, mapping
+        )
         self.mapped_group_depth = mapped_group_depth
 
-        """energy of multiplier array"""
-        energy_mults = self.get_mults_energy(self.hd_param, self.logic_unit, layer, mapped_rows_total, self.wl_dim_size, macro_activation_times)
+        # energy of multiplier array
+        energy_mults = self.get_mults_energy(
+            self.hd_param,
+            self.logic_unit,
+            layer,
+            mapped_rows_total,
+            self.wl_dim_size,
+            macro_activation_times,
+        )
+
+        # energy of adder trees (type: RCA)
+        energy_adders, adder_output_pres = self.get_adder_trees_energy(
+            layer,
+            self.logic_unit,
+            mapped_rows_for_adder,
+            self.bl_dim_size,
+            mapped_cols,
+            layer_act_operand_pres,
+            macro_activation_times,
+        )
 
-        """energy of adder trees (type: RCA)"""
-        energy_adders, adder_output_pres = self.get_adder_trees_energy(layer, self.logic_unit, mapped_rows_for_adder,
-                                           self.bl_dim_size, mapped_cols, layer_act_operand_pres, macro_activation_times)
-
-        """energy of adders_pv (type: RCA)"""
+        # energy of adders_pv (type: RCA)
         nb_inputs_of_adder_pv = self.hd_param["input_bit_per_cycle"]
         input_bit_per_cycle = self.hd_param["input_bit_per_cycle"]
-        energy_adders_pv = self.get_adder_pv_energy(nb_inputs_of_adder_pv, adder_output_pres, self.logic_unit, layer_act_operand_pres,
-                                                    input_bit_per_cycle, mapped_cols, macro_activation_times)
+        energy_adders_pv = self.get_adder_pv_energy(
+            nb_inputs_of_adder_pv,
+            adder_output_pres,
+            self.logic_unit,
+            layer_act_operand_pres,
+            input_bit_per_cycle,
+            mapped_cols,
+            macro_activation_times,
+        )
 
-        """energy of accumulators (adder type: RCA)"""
+        # energy of accumulators (adder type: RCA)
         if input_bit_per_cycle == layer_act_operand_pres:
             energy_accumulators = 0
         else:
-            accumulator_output_pres = self.hd_param["input_precision"]+self.hd_param["weight_precision"]+math.log2(self.bl_dim_size)
+            accumulator_output_pres = (
+                self.hd_param["input_precision"] + self.hd_param["weight_precision"] + math.log2(self.bl_dim_size)
+            )
             nb_of_activation_times = mapped_cols * layer_act_operand_pres / input_bit_per_cycle * macro_activation_times
-            energy_accumulators = (self.logic_unit.get_1b_adder_energy() + self.logic_unit.get_1b_reg_energy()) * \
-                                  accumulator_output_pres * nb_of_activation_times
+            energy_accumulators = (
+                (self.logic_unit.get_1b_adder_energy() + self.logic_unit.get_1b_reg_energy())
+                * accumulator_output_pres
+                * nb_of_activation_times
+            )
 
-        self.energy_breakdown = { # unit: pJ (the unit borrowed from CACTI)
+        self.energy_breakdown = {  # unit: pJ (the unit borrowed from CACTI)
             "precharging": energy_precharging,
             "mults": energy_mults,
             "adders": energy_adders,
             "adders_pv": energy_adders_pv,
-            "accumulators": energy_accumulators
+            "accumulators": energy_accumulators,
         }
         self.energy = sum([v for v in self.energy_breakdown.values()])
         return self.energy_breakdown
 
-    @staticmethod
-    def identify_layer_operand_representation(layer):
-        # activation representation: list (conv layers)
-        act_operand = [operand for operand in layer.operand_loop_dim.keys() if
-                       len(layer.operand_loop_dim[operand]["pr"]) > 0]
-        if len(act_operand) == 0:  # true for fully-connected (fc) layers
-            # weight representation (fc layers)
-            const_operand = [operand for operand in layer.operand_loop_dim.keys() if
-                             len(layer.operand_loop_dim[operand]["ir"]) == 0][0]
-            # activation representation (fc layers)
-            act_operand = [operand for operand in layer.input_operands if operand != const_operand][0]
-        else:
-            act_operand = act_operand[0]
-            # weight representation (conv layers)
-            const_operand = [operand for operand in layer.input_operands if operand != act_operand][0]
-        return act_operand, const_operand
 
 if __name__ == "__main__":
-#
-##### IMC hardware dimension illustration (keypoint: adders' accumulation happens on D2)
-#
-#       |<------------------------ D1 ----------------------------->| (nb_of_columns/macro = D1 * weight_precision)
-#    -  +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++    \
-#    ^  +                                                           +  +  D3 (nb_of_macros)
-#    |  +         ^     +++++++                                     +   +  \
-#    |  +         |     +  W  +                                     +   +
-#    |  +   group_depth +++++++                                     +   +
-#    |  +         |     +  W  +                                     +   +
-#    |  +         v     +++++++                                     +   +
-#    |  +                  |                                        +   +
-#    |  +                  v                                        +   +
-#    |  +               multipliers -\                              +   +
-#    |  +        .                    \                             +   +
-#       +        .                     - adders (DIMC)              +   +
-#   D2  +        .                    / OR adcs (AIMC)              +   +
-#       +               multipliers -/       |                      +   +
-#    |  +                  ^                 |                      +   +
-#    |  +                  |                 |                      +   +
-#    |  +         ^     +++++++              v                      +   +
-#    |  +         |     +  W  +          adders_pv (place value)    +   +
-#    |  +   group_depth +++++++              |                      +   +
-#    |  +         |     +  W  +              v                      +   +
-#    |  +         v     +++++++         accumulators                +   +
-#    |  +                                    |                      +   +
-#    v  +                                    |                      +   +
-#    -  +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++   +
-#          +                                 |                        + +
-#           +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
-#   (nb_of_rows/macro = D2 * group_depth)    |
-#                                            v
-#                                        outputs
-#
+    #
+    # #### IMC hardware dimension illustration (keypoint: adders' accumulation happens on D2)
+    #
+    #       |<------------------------ D1 ----------------------------->| (nb_of_columns/macro = D1 * weight_precision)
+    #    -  +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++    \
+    #    ^  +                                                           +  +  D3 (nb_of_macros)
+    #    |  +         ^     +++++++                                     +   +  \
+    #    |  +         |     +  W  +                                     +   +
+    #    |  +   group_depth +++++++                                     +   +
+    #    |  +         |     +  W  +                                     +   +
+    #    |  +         v     +++++++                                     +   +
+    #    |  +                  |                                        +   +
+    #    |  +                  v                                        +   +
+    #    |  +               multipliers -\                              +   +
+    #    |  +        .                    \                             +   +
+    #       +        .                     - adders (DIMC)              +   +
+    #   D2  +        .                    / OR adcs (AIMC)              +   +
+    #       +               multipliers -/       |                      +   +
+    #    |  +                  ^                 |                      +   +
+    #    |  +                  |                 |                      +   +
+    #    |  +         ^     +++++++              v                      +   +
+    #    |  +         |     +  W  +          adders_pv (place value)    +   +
+    #    |  +   group_depth +++++++              |                      +   +
+    #    |  +         |     +  W  +              v                      +   +
+    #    |  +         v     +++++++         accumulators                +   +
+    #    |  +                                    |                      +   +
+    #    v  +                                    |                      +   +
+    #    -  +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++   +
+    #          +                                 |                        + +
+    #           +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+    #   (nb_of_rows/macro = D2 * group_depth)    |
+    #                                            v
+    #                                        outputs
+    #
 
     tech_param_28nm = {
-        "tech_node":0.028,              # unit: um
-        "vdd":      0.9,                # unit: V
-        "nd2_cap":  0.7/1e3,            # unit: pF
-        "xor2_cap": 0.7*1.5/1e3,        # unit: pF
-        "dff_cap":  0.7*3/1e3,          # unit: pF
-        "nd2_area": 0.614/1e6,          # unit: mm^2
-        "xor2_area":0.614*2.4/1e6,      # unit: mm^2
-        "dff_area": 0.614*6/1e6,        # unit: mm^2
-        "nd2_dly":  0.0478,             # unit: ns
-        "xor2_dly": 0.0478*2.4,         # unit: ns
+        "tech_node": 0.028,  # unit: um
+        "vdd": 0.9,  # unit: V
+        "nd2_cap": 0.7 / 1e3,  # unit: pF
+        "xor2_cap": 0.7 * 1.5 / 1e3,  # unit: pF
+        "dff_cap": 0.7 * 3 / 1e3,  # unit: pF
+        "nd2_area": 0.614 / 1e6,  # unit: mm^2
+        "xor2_area": 0.614 * 2.4 / 1e6,  # unit: mm^2
+        "dff_area": 0.614 * 6 / 1e6,  # unit: mm^2
+        "nd2_dly": 0.0478,  # unit: ns
+        "xor2_dly": 0.0478 * 2.4,  # unit: ns
         # "dff_dly":  0.0478*3.4,         # unit: ns
     }
     dimensions = {
-        "D1": 32/8, # wordline dimension
-        "D2": 32,   # bitline dimension
-        "D3": 1,    # nb_macros
+        "D1": 32 / 8,  # wordline dimension
+        "D2": 32,  # bitline dimension
+        "D3": 1,  # nb_macros
     }  # {"D1": ("K", 4), "D2": ("C", 32),}
 
     """hd_param example for DIMC"""
     hd_param = {
-        "pe_type":              "in_sram_computing",    # required for CostModelStage
-        "imc_type":             "digital",              # "digital" or "analog". Or else: pure digital
-        "input_precision":      8,      # activation precison
-        "weight_precision":     8,      # weight precision
-        "input_bit_per_cycle":  1,      # nb_bits of input/cycle
-        "group_depth":          1,      # m factor
-        "wordline_dimension":   "D1",   # wordline dimension
+        "pe_type": "in_sram_computing",  # required for CostModelStage
+        "imc_type": "digital",  # "digital" or "analog". Or else: pure digital
+        "input_precision": 8,  # activation precison
+        "weight_precision": 8,  # weight precision
+        "input_bit_per_cycle": 1,  # nb_bits of input/cycle
+        "group_depth": 1,  # m factor
+        "wordline_dimension": "D1",  # wordline dimension
         # hardware dimension where input reuse happens (corresponds to the served dimension of input regs)
-        "bitline_dimension":    "D2",   # bitline dimension
+        "bitline_dimension": "D2",  # bitline dimension
         # hardware dimension where accumulation happens (corresponds to the served dimension of output regs)
-        "enable_cacti":         True,   # use CACTI to estimated cell array area cost (cell array exclude build-in logic part)
+        "enable_cacti": True,  # use CACTI to estimated cell array area cost (cell array exclude build-in logic part)
     }
     dimc = DimcArray(tech_param_28nm, hd_param, dimensions)
     dimc.get_area()
     dimc.get_delay()
     logger = _logging.getLogger(__name__)
     logger.info(f"Total IMC area (mm^2): {dimc.area}")
     logger.info(f"area breakdown: {dimc.area_breakdown}")
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/ImcArray.py` & `zigzag_dse-3.1.1/zigzag/hardware/architecture/ImcArray.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,39 @@
-import numpy as np
-from typing import Dict
-if __name__ == "__main__":
-    from dimension import Dimension
-    from DimcArray import DimcArray
-    from AimcArray import AimcArray
-    from operational_array import OperationalArray
-else:
-    from zigzag.classes.hardware.architecture.dimension import Dimension
-    from zigzag.classes.hardware.architecture.DimcArray import DimcArray
-    from zigzag.classes.hardware.architecture.AimcArray import AimcArray
-    from zigzag.classes.hardware.architecture.operational_array import OperationalArray
+from zigzag.hardware.architecture.DimcArray import DimcArray
+from zigzag.hardware.architecture.AimcArray import AimcArray
+from zigzag.hardware.architecture.operational_array import OperationalArray
+from zigzag.utils import json_repr_handler
 
 
 class ImcArray(OperationalArray):
-    def __init__(self, tech_param: Dict[str, float], hd_param: dict, dimensions: Dict[str, int]):
-        # This class defines the general IMC array (including AIMC and DIMC)
-        # @param tech_param: definition of technology-related parameters
-        # @param hd_param: hardware architecture parameters except dimensions
-        # @param dimensions: dimensions definition
+    """! This class defines the general IMC array (including AIMC and DIMC)"""
+
+    def __init__(self, tech_param: dict[str, float], hd_param: dict, dimensions: dict[str, int]):
+        """!
+        @param tech_param: definition of technology-related parameters
+        @param hd_param: hardware architecture parameters except dimensions
+        @param dimensions: dimensions definition
+        """
         if hd_param["imc_type"] == "digital":
-            super().__init__(operational_unit=DimcArray(tech_param, hd_param, dimensions),
-                             dimensions=dimensions)
+            super().__init__(
+                operational_unit=DimcArray(tech_param, hd_param, dimensions),
+                dimensions=dimensions,
+            )
         elif hd_param["imc_type"] == "analog":
-            super().__init__(operational_unit=AimcArray(tech_param, hd_param, dimensions),
-                             dimensions=dimensions)
+            super().__init__(
+                operational_unit=AimcArray(tech_param, hd_param, dimensions),
+                dimensions=dimensions,
+            )
 
-        self.unit.get_area() # update self.area and self.area_breakdown
-        self.unit.get_delay() # update self.delay and self.delay_breakdown
+        self.unit.get_area()  # update self.area and self.area_breakdown
+        self.unit.get_delay()  # update self.delay and self.delay_breakdown
         self.area_breakdown = self.unit.area_breakdown
         self.total_area = self.unit.area
-        self.tclk_breakdown = self.unit.delay_breakdown # clock period breakdown
-        self.tclk = self.unit.delay # maximum clock period (unit: ns)
+        self.tclk_breakdown = self.unit.delay_breakdown  # clock period breakdown
+        self.tclk = self.unit.delay  # maximum clock period (unit: ns)
         self.pe_type = hd_param["pe_type"]
         self.imc_type = hd_param["imc_type"]
         self.tops_peak, self.topsw_peak, self.topsmm2_peak = self.unit.get_macro_level_peak_performance()
 
     def __jsonrepr__(self):
         # JSON Representation of this class to save it to a json file.
-        return {"operational_unit": self.unit, "dimensions": self.dimensions}
-
+        return json_repr_handler({"operational_unit": self.unit, "dimensions": self.dimensions})
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/accelerator.py` & `zigzag_dse-3.1.1/zigzag/hardware/architecture/Accelerator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing import Set
-from zigzag.classes.hardware.architecture.core import Core
-from zigzag.classes.hardware.architecture.memory_instance import MemoryInstance
+from zigzag.hardware.architecture.Core import Core
+from zigzag.utils import json_repr_handler
 
-##  The Accelerator class houses a set of Cores with an additional Global Buffer.
-# This Global Buffer sits above the cores, and can optionally be disabled.
-class Accelerator:
 
-    def __init__(self, name, core_set: Set[Core]):
-        self.name = name
-        self.cores = sorted([core for core in core_set], key=lambda core: core.id)
+class Accelerator:
+    """!  The Accelerator class houses a set of Cores with an additional Global Buffer.
+    This Global Buffer sits above the cores, and can optionally be disabled.
+    """
+
+    def __init__(self, name: str, core_set: set[Core]):
+        self.name: str = name
+        self.cores = sorted(list(core_set), key=lambda core: core.id)
 
     def __str__(self) -> str:
         return f"Accelerator({self.name})"
 
     def __repr__(self) -> str:
         return str(self)
 
-    ## JSON representation used for saving this object to a json file.
     def __jsonrepr__(self):
-        return {"name": self.name, "cores": self.cores}
+        """! JSON representation used for saving this object to a json file."""
+        return json_repr_handler({"name": self.name, "cores": self.cores})
 
-    ## Return the core with id 'core_id'.
-    # Raises ValueError() when a core_id is not found in the available cores.
-    def get_core(self, core_id: int or str) -> Core:
+    def get_core(self, core_id: int) -> Core:
+        """! Return the core with id 'core_id'.
+        Raises ValueError() when a core_id is not found in the available cores.
+        """
         core = next((core for core in self.cores if core.id == core_id), None)
         if not core:
-            raise ValueError(
-                f"Requested core with id {core_id} is not present in accelerator."
-            )
+            raise ValueError(f"Requested core with id {core_id} is not present in accelerator.")
         return core
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/core.py` & `zigzag_dse-3.1.1/zigzag/hardware/architecture/Core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,175 +1,130 @@
-from zigzag.classes.hardware.architecture.memory_instance import MemoryInstance
-from zigzag.classes.hardware.architecture.operational_array import OperationalArray
-from zigzag.classes.hardware.architecture.memory_hierarchy import MemoryHierarchy
-import networkx as nx
+from zigzag.datatypes import MemoryOperand
+from zigzag.hardware.architecture.MemoryInstance import MemoryInstance
+from zigzag.hardware.architecture.memory_level import MemoryLevel
+from zigzag.hardware.architecture.operational_array import OperationalArray
+from zigzag.hardware.architecture.MemoryHierarchy import MemoryHierarchy
+
+from zigzag.mapping.spatial_mapping import SpatialMapping
+from zigzag.utils import json_repr_handler
+
 
-## The Core class houses the array of multipliers and the attached memory hierarchy.
-## This class supports a singular multiplier array and memory hierarchy, runtime flexibility should be implemented on top.
 class Core:
+    """! The Core class houses the array of multipliers and the attached memory hierarchy.
+    This class supports a singular multiplier array and memory hierarchy, runtime flexibility should be implemented
+    on top.
+    """
 
-    ## The class constructor
-    # @param id
-    # @param operational_array
-    # @param memory_hierarchy
-    # @param dataflows
     def __init__(
         self,
-        id: int,
+        core_id: int,
         operational_array: OperationalArray,
         memory_hierarchy: MemoryHierarchy,
-        dataflows: list = None,
+        dataflows: SpatialMapping | None = None,
     ):
-        self.id = id
+
+        self.id = core_id
         self.operational_array = operational_array
         self.memory_hierarchy = memory_hierarchy
-        self.dataflows = (
-            dataflows  # save the possible spatial dataflows inside the Core
-        )
-        self.check_valid()
+        self.mem_hierarchy_dict: dict[MemoryOperand, list[MemoryLevel]] = {}
 
+        self.dataflows = dataflows
         self.recalculate_memory_hierarchy_information()
 
-    def __str__(self) -> str:
-        return f"Core({self.id})"
-
-    def __repr__(self) -> str:
-        return str(self)
-
-    # JSON representation used for saving this object to a json file.
-    def __jsonrepr__(self):
-        return self.__dict__
-
-    def __hash__(self) -> int:
-        return hash(self.id)
-
-    def __eq__(self, __o: object) -> bool:
-        if not isinstance(__o, Core):
-            return False
-        return (
-            self.id == __o.id
-            and self.operational_array == __o.operational_array
-            and self.memory_hierarchy == __o.memory_hierarchy
-        )
-
-    def equals(self, other: object) -> bool:
-        return (
-            isinstance(other, Core)
-            and self.operational_array == other.operational_array
-            and self.memory_hierarchy == other.memory_hierarchy
-        )
-
-    def check_valid(self):
-        # TODO
-        pass
+    def get_memory_level(self, mem_op: MemoryOperand, mem_lv: int) -> MemoryLevel:
+        """! Returns a specific memory level in the memory hierarchy for the memory operand"""
+        # Sort the nodes topologically and filter out all memories that don't store mem_op
+        memory = [node for node in self.memory_hierarchy.topological_sort() if mem_op in node.operands]
+        return memory[mem_lv]
 
     def recalculate_memory_hierarchy_information(self):
-        self.generate_memory_hierarchy_dict()
-        self.generate_memory_sharing_list()
+        self.__generate_memory_hierarchy_dict()
+        self.__generate_memory_sharing_list()
 
-    def generate_memory_hierarchy_dict(self):
+    def __generate_memory_hierarchy_dict(self):
         mem_operands = self.memory_hierarchy.nb_levels.keys()
-        mem_hierarchy_dict = {}
-        mem_size_dict = {}
-        mem_r_bw_dict = {}
-        mem_w_bw_dict = {}
-        mem_r_bw_min_dict = {}
-        mem_w_bw_min_dict = {}
+        mem_hierarchy_dict: dict[MemoryOperand, list[MemoryLevel]] = {}
+        mem_size_dict: dict[MemoryOperand, list[int]] = {}
+        mem_r_bw_dict: dict[MemoryOperand, list[int]] = {}
+        mem_w_bw_dict: dict[MemoryOperand, list[int]] = {}
+        mem_r_bw_min_dict: dict[MemoryOperand, list[int]] = {}
+        mem_w_bw_min_dict: dict[MemoryOperand, list[int]] = {}
         for mem_op in mem_operands:
             mem_hierarchy_dict[mem_op] = [
-                node
-                for node in nx.topological_sort(self.memory_hierarchy)
-                if mem_op in node.operands
+                node for node in self.memory_hierarchy.topological_sort() if mem_op in node.operands
             ]
             mem_size_dict[mem_op] = [
                 node.memory_instance.size
-                for node in nx.topological_sort(self.memory_hierarchy)
+                for node in self.memory_hierarchy.topological_sort()
                 if mem_op in node.operands
             ]
             mem_r_bw_dict[mem_op] = [
                 node.memory_instance.r_bw
-                for node in nx.topological_sort(self.memory_hierarchy)
+                for node in self.memory_hierarchy.topological_sort()
                 if mem_op in node.operands
             ]
             mem_w_bw_dict[mem_op] = [
                 node.memory_instance.w_bw
-                for node in nx.topological_sort(self.memory_hierarchy)
+                for node in self.memory_hierarchy.topological_sort()
                 if mem_op in node.operands
             ]
             mem_r_bw_min_dict[mem_op] = [
                 node.memory_instance.r_bw_min
-                for node in nx.topological_sort(self.memory_hierarchy)
+                for node in self.memory_hierarchy.topological_sort()
                 if mem_op in node.operands
             ]
             mem_w_bw_min_dict[mem_op] = [
                 node.memory_instance.w_bw_min
-                for node in nx.topological_sort(self.memory_hierarchy)
+                for node in self.memory_hierarchy.topological_sort()
                 if mem_op in node.operands
             ]
         self.mem_hierarchy_dict = mem_hierarchy_dict
         self.mem_size_dict = mem_size_dict
         self.mem_r_bw_dict = mem_r_bw_dict
         self.mem_w_bw_dict = mem_w_bw_dict
         self.mem_r_bw_min_dict = mem_r_bw_min_dict
         self.mem_w_bw_min_dict = mem_w_bw_min_dict
 
-    ## Generates a list of dictionary that indicates which operand's which memory levels are sharing the same physical memory
-    def generate_memory_sharing_list(self):
-        memory_sharing_list = []
+    def __generate_memory_sharing_list(self):
+        """! Generates a list of dictionary that indicates which operand's which memory levels are sharing the same
+        physical memory"""
+        memory_sharing_list: list[dict[MemoryOperand, int]] = []
         for mem_lv in self.mem_hierarchy_dict.values():
             for mem in mem_lv:
                 operand_mem_share = mem.mem_level_of_operands
-                if (
-                    len(operand_mem_share) > 1
-                    and operand_mem_share not in memory_sharing_list
-                ):
+                if len(operand_mem_share) > 1 and operand_mem_share not in memory_sharing_list:
                     memory_sharing_list.append(operand_mem_share)
 
         self.mem_sharing_list = memory_sharing_list
 
-    def get_memory_hierarchy(self):
-        return self.memory_hierarchy
-
-    def get_memory_hierarchy_dict(self):
-        return self.mem_hierarchy_dict
-
-    def get_memory_size_dict(self):
-        return self.mem_size_dict
+    def get_top_memory_instance(self, mem_op: MemoryOperand) -> MemoryInstance:
+        if mem_op not in self.memory_hierarchy.get_operands():
+            raise ValueError(f"Memory operand {mem_op} not in {self}.")
+        mem_level = self.memory_hierarchy.get_operand_top_level(mem_op)
+        mem_instance = mem_level.memory_instance
+        return mem_instance
 
     def get_memory_bw_dict(self):
         return self.mem_r_bw_dict, self.mem_w_bw_dict
 
     def get_memory_bw_min_dict(self):
         return self.mem_r_bw_min_dict, self.mem_w_bw_min_dict
 
-    def get_memory_sharing_list(self):
-        return self.mem_sharing_list
+    def __str__(self) -> str:
+        return f"Core({self.id})"
 
-    ## Returns a specific memory level in the memory hierarchy for the memory operand
-    def get_memory_level(self, mem_op: str, mem_lv: int):
-        # Sort the nodes topologically and filter out all memories that don't store mem_op
-        memory = [
-            node
-            for node in nx.topological_sort(self.memory_hierarchy)
-            if mem_op in node.operands
-        ]
-        return memory[mem_lv]
+    def __repr__(self) -> str:
+        return str(self)
 
-    ## Get the lowest shared memory level between mem_op1 (>= mem_lv1) and mem_op2 (>= mem_lv2).
-    def get_lowest_shared_mem_level_above(self, mem_op1, mem_lv1, mem_op2, mem_lv2):
-        for lv, mem in enumerate(self.mem_hierarchy_dict[mem_op1][mem_lv1:]):
-            if (
-                mem_op2 in mem.operands
-                and mem_lv2 <= mem.mem_level_of_operands[mem_op2]
-            ):
-                return mem
+    def __jsonrepr__(self):
+        return json_repr_handler(self.__dict__)
 
-        raise Exception(
-            f"{mem_op1}'s level {mem_lv1} and {mem_op2}'s level {mem_lv2} don't have a shared memory above!"
-        )
+    def __hash__(self) -> int:
+        return hash(self.id)
 
-    def get_top_memory_instance(self, mem_op) -> MemoryInstance:
-        if mem_op not in self.memory_hierarchy.get_operands():
-            raise ValueError(f"Memory operand {mem_op} not in {self}.")
-        mem_level = self.memory_hierarchy.get_operand_top_level(mem_op)
-        mem_instance = mem_level.memory_instance
-        return mem_instance
+    def __eq__(self, other: object) -> bool:
+        return (
+            isinstance(other, Core)
+            and self.id == other.id
+            and self.operational_array == other.operational_array
+            and self.memory_hierarchy == other.memory_hierarchy
+        )
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/imc_unit.py` & `zigzag_dse-3.1.1/zigzag/hardware/architecture/imc_unit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,85 +1,103 @@
+"""
+This file includes:
+  . class LogicUnit (defines the energy/area/delay cost of multipliers, adders, regs)
+  . class ImcArray (provides initialization function, used for class DimcArray and AimcArray)
+"""
+
 import math
+
+from zigzag.hardware.architecture.operational_unit import OperationalUnit
+
 if __name__ == "__main__" or __name__ == "imc_unit":
     # branch when the script is run locally or called by A/DimcArray.py
     from get_cacti_cost import get_cacti_cost
 else:
-    from zigzag.classes.hardware.architecture.get_cacti_cost import get_cacti_cost
+    from zigzag.hardware.architecture.get_cacti_cost import get_cacti_cost
 
-###############################################################################################################
-# This file includes:
-#   . class LogicUnit (defines the energy/area/delay cost of multipliers, adders, regs)
-#   . class ImcArray (provides initialization function, used for class DimcArray and AimcArray)
-###############################################################################################################
 
 class LogicUnit:
     """cost (energy, area, delay) of 1b adder, 1b multiplier, 1b register is defined in this class"""
-    def __init__(self, tech_param:dict):
+
+    def __init__(self, tech_param: dict):
         """
-        Input example:
-        tech_param_28nm = {
-        "vdd":      0.9,            # unit: V
-        "nd2_cap":  0.7/1e3,        # unit: pF
-        "nd2_area": 0.614/1e6,      # unit: mm^2
-        "nd2_dly":  0.0478,         # unit: ns
-        "xor2_cap": 0.7*1.5/1e3,    # unit: pF
-        "xor2_area":0.614*2.4/1e6,  # unit: mm^2
-        "xor2_dly": 0.0478*1.5,     # unit: ns
-        "dff_cap":  0.7*3/1e3,      # unit: pF
-        "dff_area": 0.0614*6/1e6,   # unit: mm^2
-        "dff_dly":  0.0478*3.4,     # unit: ns
-    }
+            Input example:
+            tech_param_28nm = {
+            "vdd":      0.9,            # unit: V
+            "nd2_cap":  0.7/1e3,        # unit: pF
+            "nd2_area": 0.614/1e6,      # unit: mm^2
+            "nd2_dly":  0.0478,         # unit: ns
+            "xor2_cap": 0.7*1.5/1e3,    # unit: pF
+            "xor2_area":0.614*2.4/1e6,  # unit: mm^2
+            "xor2_dly": 0.0478*1.5,     # unit: ns
+            "dff_cap":  0.7*3/1e3,      # unit: pF
+            "dff_area": 0.0614*6/1e6,   # unit: mm^2
+            "dff_dly":  0.0478*3.4,     # unit: ns
+        }
         """
-        """check input firstly"""
+        # check input firstly
         self.check_tech_param(tech_param)
-        """initialization"""
+        # initialization
         self.tech_param = tech_param
-        self.tech_param["wl_cap"] = tech_param["nd2_cap"]/2 # wordline cap of each SRAM cell is treated as NAND2_cap/2
-        self.tech_param["bl_cap"] = tech_param["nd2_cap"]/2  # bitline cap of each SRAM cell is treated as NAND2_cap/2
+        self.tech_param["wl_cap"] = (
+            tech_param["nd2_cap"] / 2
+        )  # wordline cap of each SRAM cell is treated as NAND2_cap/2
+        self.tech_param["bl_cap"] = tech_param["nd2_cap"] / 2  # bitline cap of each SRAM cell is treated as NAND2_cap/2
 
     def check_tech_param(self, tech_param):
-        required_param = ["tech_node", "vdd", "nd2_cap", "nd2_area", "nd2_dly", "xor2_cap", "xor2_area", "xor2_dly", "dff_cap", "dff_area"]
+        required_param = [
+            "tech_node",
+            "vdd",
+            "nd2_cap",
+            "nd2_area",
+            "nd2_dly",
+            "xor2_cap",
+            "xor2_area",
+            "xor2_dly",
+            "dff_cap",
+            "dff_area",
+        ]
         for ii_a, a in enumerate(required_param):
             if a not in tech_param.keys():
                 raise Exception(f"[LogicUnit] Incorrect input, required param [{a}] not found.")
             if not (isinstance(tech_param[a], int) or isinstance(tech_param[a], float)):
                 raise Exception(f"[LogicUnit] Incorrect input, value [{tech_param[a]}] of param [{a}] is not a num.")
             if tech_param[a] <= 0:
                 raise Exception(f"[LogicUnit] Incorrect input, value [{tech_param[a]}] of param [{a}] is not positive.")
 
     def get_1b_adder_energy(self):
-        """energy of 1b full adder"""
-        """Assume a 1b adder has 3 ND2 gate and 2 XOR2 gate"""
-        adder_cap =  3 * self.tech_param["nd2_cap"] + 2 *  self.tech_param["xor2_cap"]
-        return adder_cap * (self.tech_param["vdd"]**2) # unit: pJ
+        """energy of 1b full adder
+        Assume a 1b adder has 3 ND2 gate and 2 XOR2 gate"""
+        adder_cap = 3 * self.tech_param["nd2_cap"] + 2 * self.tech_param["xor2_cap"]
+        return adder_cap * (self.tech_param["vdd"] ** 2)  # unit: pJ
 
     def get_1b_adder_energy_half_activated(self):
         """energy of 1b full adder when 1 input is 0"""
         adder_cap = 2 * self.tech_param["xor2_cap"]
         return adder_cap * (self.tech_param["vdd"] ** 2)  # unit: pJ
 
     def get_1b_multiplier_energy(self):
-        """energy of 1b multiplier"""
-        """1b mult includes 1 NOR gate, which is assumed as the same cost of ND2 gate"""
-        """why 0.5: considering weight stays constant during multiplication"""
-        return 0.5 * self.tech_param["nd2_cap"] * (self.tech_param["vdd"] ** 2) # unit: pJ
+        """energy of 1b multiplier
+        1b mult includes 1 NOR gate, which is assumed as the same cost of ND2 gate
+        why 0.5: considering weight stays constant during multiplication"""
+        return 0.5 * self.tech_param["nd2_cap"] * (self.tech_param["vdd"] ** 2)  # unit: pJ
 
     def get_1b_reg_energy(self):
         """energy of 1b DFF"""
-        return self.tech_param["dff_cap"] * (self.tech_param["vdd"] ** 2) # unit: pJ
+        return self.tech_param["dff_cap"] * (self.tech_param["vdd"] ** 2)  # unit: pJ
 
     def get_1b_adder_area(self):
-        """area of 1b full adder"""
-        """Assume a 1b adder has 3 ND2 gate and 2 XOR2 gate"""
+        """area of 1b full adder
+        Assume a 1b adder has 3 ND2 gate and 2 XOR2 gate"""
         adder_area = 3 * self.tech_param["nd2_area"] + 2 * self.tech_param["xor2_area"]
         return adder_area
 
     def get_1b_multiplier_area(self):
-        """area of 1b multiplier"""
-        """1b mult includes 1 NOR gate, which is assumed as the same cost of ND2 gate"""
+        """area of 1b multiplier
+        1b mult includes 1 NOR gate, which is assumed as the same cost of ND2 gate"""
         return self.tech_param["nd2_area"]
 
     def get_1b_reg_area(self):
         """area of 1b DFF"""
         return self.tech_param["dff_area"]
 
     def get_1b_adder_dly_in2sum(self):
@@ -94,104 +112,132 @@
 
     def get_1b_adder_dly_cin2cout(self):
         """delay of 1b adder: carry-in to carry-out"""
         adder_dly = 2 * self.tech_param["nd2_dly"]
         return adder_dly
 
     def get_1b_multiplier_dly(self):
-        """delay of 1b multiplier"""
-        """1b mult includes 1 NOR gate, which is assumed as the same cost of ND2 gate"""
+        """delay of 1b multiplier
+        1b mult includes 1 NOR gate, which is assumed as the same cost of ND2 gate"""
         return self.tech_param["nd2_dly"]
 
     def get_1b_reg_dly(self):
-        """delay of 1b DFF"""
-        """why 0? Compared to others, it's negligible"""
+        """delay of 1b DFF
+        why 0? Compared to others, it's negligible"""
         return 0
 
+
 class ImcUnit:
-    """definition of general initilization function for D/AIMC"""
-    def __init__(self,tech_param:dict, hd_param:dict, dimensions:dict):
+    """definition of general initilization function for D/AIMC
+    # TODO ImcUnit should inherit from OperationalUnit since ImcArray inherits from OperationalArray
+    """
+
+    def __init__(self, tech_param: dict, hd_param: dict, dimensions: dict):
         """check input firstly"""
         self.check_input(hd_param, dimensions)
-        """initialization"""
+        # initialization
         self.hd_param = hd_param
         self.dimensions = dimensions
-        self.wl_dim = hd_param["wordline_dimension"] # wl_dim should be the same with the dimension served by input_reg.
-        self.bl_dim = hd_param["bitline_dimension"] # bl_dim should be the same with the dimension served by output_reg.
-        self.wl_dim_size = dimensions[self.wl_dim] # dimension where wordline is
-        self.bl_dim_size = dimensions[self.bl_dim] # dimension where bitline (adder tree) is
-        self.nb_of_banks = math.prod([dimensions[oa_dim] for oa_dim in dimensions if oa_dim not in [self.wl_dim, self.bl_dim]])
+        self.wl_dim = hd_param[
+            "wordline_dimension"
+        ]  # wl_dim should be the same with the dimension served by input_reg.
+        self.bl_dim = hd_param[
+            "bitline_dimension"
+        ]  # bl_dim should be the same with the dimension served by output_reg.
+        self.wl_dim_size = dimensions[self.wl_dim]  # dimension where wordline is
+        self.bl_dim_size = dimensions[self.bl_dim]  # dimension where bitline (adder tree) is
+        self.nb_of_banks = math.prod(
+            [dimensions[oa_dim] for oa_dim in dimensions if oa_dim not in [self.wl_dim, self.bl_dim]]
+        )
         # tech_param will be checked and initialized in LogicUnit class
         self.logic_unit = LogicUnit(tech_param)
         # parameters to be updated in function
         self.energy = None
         self.energy_breakdown = None
         self.area = None
         self.area_breakdown = None
         self.delay = None
         self.delay_breakdown = None
         self.mapped_rows_total = None
         self.mapped_group_depth = None
 
-
     def check_input(self, hd_param, dimensions):
         # check if required_hd_param is provided
         # check if there is any negative dimension value
         required_hd_param = [
-            "imc_type", "input_precision", "weight_precision", "input_bit_per_cycle", "group_depth",
-            "wordline_dimension", "bitline_dimension", "enable_cacti"
+            "imc_type",
+            "input_precision",
+            "weight_precision",
+            "input_bit_per_cycle",
+            "group_depth",
+            "wordline_dimension",
+            "bitline_dimension",
+            "enable_cacti",
         ]
         for ii_a, a in enumerate(required_hd_param):
             if a not in hd_param.keys():
                 raise Exception(f"[ImcArray] Incorrect hd_param, required param [{a}] not found.")
             if a == "imc_type":
                 if hd_param[a] not in ["digital", "analog"]:
-                    raise Exception(f"[ImcArray] Incorrect imc_type in hd_param, either [analog] or [digital] is expected.")
+                    raise Exception(
+                        f"[ImcArray] Incorrect imc_type in hd_param, either [analog] or [digital] is expected."
+                    )
             elif a == "wordline_dimension" or a == "bitline_dimension":
                 if not isinstance(hd_param[a], str) or hd_param[a] not in dimensions.keys():
                     raise Exception(f"[ImcArray] param [{a}] is not a str or is not a key in dimensions.")
             elif a == "enable_cacti":
                 if not isinstance(hd_param[a], bool):
                     raise Exception(f"[ImcArray] param [{a}] is not bool (Ture, False).")
             else:
                 if not (isinstance(hd_param[a], int) or isinstance(hd_param[a], float)):
-                    raise Exception(f"[ImcArray] Incorrect hd_param, value [{hd_param[a]}] of param [{a}] is not a num.")
+                    raise Exception(
+                        f"[ImcArray] Incorrect hd_param, value [{hd_param[a]}] of param [{a}] is not a num."
+                    )
                 if hd_param[a] <= 0:
-                    raise Exception(f"[ImcArray] Incorrect hd_param, value [{hd_param[a]}] of param [{a}] is not positive.")
+                    raise Exception(
+                        f"[ImcArray] Incorrect hd_param, value [{hd_param[a]}] of param [{a}] is not positive."
+                    )
                 if a == "input_bit_per_cycle" and hd_param[a] > hd_param["input_precision"]:
                     input_precision = hd_param["input_precision"]
-                    raise Exception(f"[ImcArray] Incorrect hd_param, value [{hd_param[a]}] of param [{a}] is bigger than [input_precision] ({input_precision}).")
+                    raise Exception(
+                        f"[ImcArray] Incorrect hd_param, value [{hd_param[a]}] of param [{a}] is bigger than [input_precision] ({input_precision})."
+                    )
         for oa_dim in dimensions.keys():
             if dimensions[oa_dim] <= 0:
-                raise Exception(f"[ImcArray] Incorrect dimensions, value [{dimensions[a]}] of param [{a}] is not a positive number.")
+                raise Exception(
+                    f"[ImcArray] Incorrect dimensions, value [{dimensions[a]}] of param [{a}] is not a positive number."
+                )
         if hd_param["imc_type"] == "analog":
             a = "adc_resolution"
             if a not in hd_param.keys():
                 raise Exception(f"[ImcArray] Incorrect hd_param, required param [{a}] not found.")
             # if adc_resolution is not a number or adc_resolution <= 0
             if (not (isinstance(hd_param[a], int) or isinstance(hd_param[a], float))) or (hd_param[a] <= 0):
-                raise Exception(f"[ImcArray] Incorrect hd_param, value [{hd_param[a]}] of param [{a}] is not a positive number.")
+                raise Exception(
+                    f"[ImcArray] Incorrect hd_param, value [{hd_param[a]}] of param [{a}] is not a positive number."
+                )
 
     def get_single_cell_array_cost_from_cacti(self, tech_node, wl_dim_size, bl_dim_size, group_depth, w_pres):
-        """get the area, energy cost of a single macro (cell array) using CACTI"""
-        """this function is called when cacti is required for cost estimation"""
-        """
+        """get the area, energy cost of a single macro (cell array) using CACTI
+        this function is called when cacti is required for cost estimation
         @param tech_node:   the technology node (e.g. 0.028, 0.032, 0.022 ... unit: um)
         @param wl_dim_size: the size of dimension where wordline is.
         @param bl_dim_size: the size of dimension where bitline (adder tree) is.
         @param group_depth: the size of each cell group (number of SRAM cells on local bitline)
         @param w_pres:      weight precision (number of SRAM cells required to store a operand)
         """
-        cell_array_size = wl_dim_size * bl_dim_size * group_depth * w_pres / 8 # array size. unit: byte
-        array_bw = wl_dim_size * w_pres # imc array bandwidth. unit: bit
+        cell_array_size = wl_dim_size * bl_dim_size * group_depth * w_pres / 8  # array size. unit: byte
+        array_bw = wl_dim_size * w_pres  # imc array bandwidth. unit: bit
 
         # we will call cacti to get the area (mm^2), access_time (ns), r_cost (nJ/access), w_cost (nJ/access)
         if __name__ == "imc_unit":
             cacti_path = "../../cacti/cacti_master"
         else:
             cacti_path = "zigzag/classes/cacti/cacti_master"
-        access_time, area, r_cost, w_cost = get_cacti_cost(cacti_path=cacti_path,
-                                                           tech_node=tech_node,
-                                                           mem_type="sram",
-                                                           mem_size_in_byte=cell_array_size,
-                                                           bw=array_bw)
+        access_time, area, r_cost, w_cost = get_cacti_cost(
+            cacti_path=cacti_path,
+            tech_node=tech_node,
+            mem_type="sram",
+            mem_size_in_byte=cell_array_size,
+            bw=array_bw,
+        )
         return access_time, area, r_cost, w_cost
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/memory_instance.py` & `zigzag_dse-3.1.1/zigzag/hardware/architecture/MemoryInstance.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,56 @@
-from zigzag.classes.cacti.cacti_parser import CactiParser
+from zigzag.cacti.cacti_parser import CactiParser
+from zigzag.utils import json_repr_handler
+
 
-## Description missing
 class MemoryInstance:
 
-    ## The class constructor
-    # Collect all the basic information of a physical memory module.
-    # @param name: memory module name, e.g. 'SRAM_512KB_BW_16b', 'I_RF'.
-    # @param size: total memory capacity (unit: bit).
-    # @param r_bw/w_bw: memory bandwidth (or wordlength) (unit: bit/cycle).
-    # @param r_cost/w_cost: memory unit data access energy.
-    # @param area: memory area (unit can be whatever user-defined unit).
-    # @param r_port: number of memory read port.
-    # @param w_port: number of memory write port (rd_port and wr_port can work in parallel).
-    # @param rw_port: number of memory port for both read and write (read and write cannot happen in parallel).
-    # @param latency: memory access latency (unit: number of cycles).
-    # @param min_r_granularity (int): The minimal number of bits than can be read in a clock cycle (can be a less than r_bw)
-    # @param min_w_granularity (int): The minimal number of bits that can be written in a clock cycle (can be less than w_bw)
-    # @param mem_type (str): The type of memory. Used for CACTI cost extraction.
-    # @param auto_cost_extraction (bool): Automatically extract the read cost, write cost and area using CACTI.
-    # @param double_buffering_support (bool): Support for double buffering on this memory instance.
     def __init__(
         self,
         name: str,
         size: int,
         r_bw: int,
         w_bw: int = 0,
         r_cost: float = 0,
         w_cost: float = 0,
         area: float = 0,
         r_port: int = 1,
         w_port: int = 1,
         rw_port: int = 0,
         latency: int = 1,
-        min_r_granularity=None,
-        min_w_granularity=None,
+        min_r_granularity: int | None = None,
+        min_w_granularity: int | None = None,
         mem_type: str = "sram",
         auto_cost_extraction: bool = False,
         double_buffering_support: bool = False,
     ):
+        """
+        Collect all the basic information of a physical memory module.
+        @param name: memory module name, e.g. 'SRAM_512KB_BW_16b', 'I_RF'.
+        @param size: total memory capacity (unit: bit).
+        @param r_bw/w_bw: memory bandwidth (or word length) (unit: bit/cycle).
+        @param r_cost/w_cost: memory unit data access energy (unit: pJ/access).
+        @param area: memory area (unit can be whatever user-defined unit).
+        @param r_port: number of memory read port.
+        @param w_port: number of memory write port (rd_port and wr_port can work in parallel).
+        @param rw_port: number of memory port for both read and write (read and write cannot happen in parallel).
+        @param latency: memory access latency (unit: number of cycles).
+        @param min_r_granularity (int): The minimal number of bits than can be read in a clock cycle (can be a less than
+          r_bw)
+        @param min_w_granularity (int): The minimal number of bits that can be written in a clock cycle (can be less
+        than w_bw)
+        @param mem_type (str): The type of memory. Used for CACTI cost extraction.
+        @param auto_cost_extraction (bool): Automatically extract the read cost, write cost and area using CACTI.
+        @param double_buffering_support (bool): Support for double buffering on this memory instance.
+        """
         if auto_cost_extraction:
             # Size must be a multiple of 8 when using CACTI
-            assert (
-                size % 8 == 0
-            ), "Memory size must be a multiple of 8 when automatically extracting costs using CACTI."
+            assert size % 8 == 0, "Memory size must be a multiple of 8 when automatically extracting costs using CACTI."
             cacti_parser = CactiParser()
-            (
-                _,
-                r_bw,
-                w_bw,
-                r_cost,
-                w_cost,
-                area,
-                bank,
-                r_port,
-                w_port,
-                rw_port,
-            ) = cacti_parser.get_item(
+            r_cost, w_cost, area = cacti_parser.get_item(
                 mem_type=mem_type,
                 size=size,
                 r_bw=r_bw,
                 r_port=r_port,
                 w_port=w_port,
                 rw_port=rw_port,
                 bank=1,
@@ -68,31 +59,30 @@
         self.name = name
         self.size = size
         self.r_bw = r_bw
         self.w_bw = w_bw
         self.r_cost = r_cost
         self.w_cost = w_cost
         self.area = area
-        self.r_port = r_port
-        self.w_port = w_port
-        self.rw_port = rw_port
+        self.r_port_nb = r_port
+        self.w_port_nb = w_port
+        self.rw_port_nb = rw_port
         self.latency = latency
         self.double_buffering_support = double_buffering_support
-        if not min_r_granularity:
-            self.r_bw_min = r_bw
-        else:
-            self.r_bw_min = min_r_granularity
-        if not min_w_granularity:
-            self.w_bw_min = w_bw
-        else:
-            self.w_bw_min = min_w_granularity
 
-    ## JSON Representation of this class to save it to a json file.
+        self.r_bw_min: int = min_r_granularity if min_r_granularity is not None else r_bw
+        self.w_bw_min: int = min_w_granularity if min_w_granularity is not None else w_bw
+
+    def update_size(self, new_size: int) -> None:
+        """! Update the memory size of this instance."""
+        self.size = new_size
+
     def __jsonrepr__(self):
-        return self.__dict__
+        """! JSON Representation of this class to save it to a json file."""
+        return json_repr_handler(self.__dict__)
 
     def __eq__(self, other: object) -> bool:
         return isinstance(other, MemoryInstance) and self.__dict__ == other.__dict__
 
     def __hash__(self):
         return id(self)  # unique for every object within its lifetime
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/operational_array.py` & `zigzag_dse-3.1.1/zigzag/hardware/architecture/operational_array.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,74 @@
-from typing import Dict
+from typing import Any
 import numpy as np
-from zigzag.classes.hardware.architecture.dimension import Dimension
-from zigzag.classes.hardware.architecture.operational_unit import (
+from zigzag.datatypes import OADimension
+from zigzag.hardware.architecture.operational_unit import (
     OperationalUnit,
     Multiplier,
 )
+from zigzag.utils import json_repr_handler
+
 
-## This class captures multi-dimensional operational array size.
 class OperationalArray:
-    ## The class constructor
-    # @param operational_unit: an OperationalUnit object including precision and single operation energy, later we
-    # can add idle energy also (e.g. for situations that one or two of the input operands is zero).
-    # @param dimensions: define the name and size of each multiplier array dimensions, e.g. {'D1': 3, 'D2': 5}.
-    def __init__(self, operational_unit: OperationalUnit, dimensions: Dict[str, int]):
-        self.unit = operational_unit
+    """! This class captures multi-dimensional operational array size."""
+
+    def __init__(self, operational_unit: OperationalUnit, dimensions: dict[OADimension, int]):
+        """
+        @param operational_unit: an OperationalUnit object including precision and single operation energy, later we
+        can add idle energy also (e.g. for situations that one or two of the input operands is zero).
+        @param dimensions: define the name and size of each multiplier array dimensions, e.g. {'D1': 3, 'D2': 5}.
+        """
+        self.unit: OperationalUnit = operational_unit
         self.total_unit_count = int(np.prod(list(dimensions.values())))
-        try:
-            self.total_area = operational_unit.area * self.total_unit_count
-        except TypeError:  # branch for IMC
-            self.total_area = operational_unit.area
-
-        base_dims = [
-            Dimension(idx, name, size)
-            for idx, (name, size) in enumerate(dimensions.items())
-        ]
-        self.dimensions = base_dims
-        self.dimension_sizes = [dim.size for dim in base_dims]
-        self.nb_dimensions = len(base_dims)
+        self.oa_dim_sizes = dimensions
+        self.total_area = operational_unit.area * self.total_unit_count
 
-    # JSON Representation of this class to save it to a json file.
     def __jsonrepr__(self):
-        return {"operational_unit": self.unit, "dimensions": self.dimensions}
+        return json_repr_handler({"operational_unit": self.unit, "dimensions": self.oa_dim_sizes})
 
-    def __eq__(self, __o: object) -> bool:
-        if not isinstance(__o, OperationalArray):
-            return False
-        return self.unit == __o.unit and self.dimensions == __o.dimensions
+    def __eq__(self, other: Any) -> bool:
+        return (
+            isinstance(other, OperationalArray) and self.unit == other.unit and self.oa_dim_sizes == other.oa_dim_sizes
+        )
 
 
-## Description missing
 class MultiplierArray(OperationalArray):
-    pass
 
+    def __init__(
+        self,
+        multiplier: Multiplier,
+        dimensions: dict[OADimension, int],
+        operand_spatial_sharing: dict[str, set[tuple[int, ...]]] | None = None,
+    ):
+        super(MultiplierArray, self).__init__(multiplier, dimensions)
+        self.multiplier = self.unit
+        self.operand_spatial_sharing = operand_spatial_sharing
+
+
+# def multiplier_array_example1():
+#     """Multiplier array variables"""
+#     multiplier_input_precision = [8, 8]
+#     multiplier_energy = 0.5
+#     multiplier_area = 0.1
+#     dimensions = {"D1": 14, "D2": 3, "D3": 4}
+#     operand_spatial_sharing = {
+#         "I1": {(1, 0, 0)},
+#         "O": {(0, 1, 0)},
+#         "I2": {(0, 0, 1), (1, 1, 0)},
+#     }
+#     multiplier = Multiplier(multiplier_input_precision, multiplier_energy, multiplier_area)
+#     multiplier_array = MultiplierArray(multiplier, dimensions, operand_spatial_sharing)
+
+#     return multiplier_array
+
+
+# def multiplier_array_example2():
+#     """Multiplier array variables"""
+#     multiplier_input_precision = [8, 8]
+#     multiplier_energy = 0.5
+#     multiplier_area = 0.1
+#     dimensions = {"D1": 14, "D2": 12}
+#     operand_spatial_sharing = {"I1": {(1, 0)}, "O": {(0, 1)}, "I2": {(1, 1)}}
+#     multiplier = Multiplier(multiplier_input_precision, multiplier_energy, multiplier_area)
+#     multiplier_array = MultiplierArray(multiplier, dimensions, operand_spatial_sharing)
 
-def multiplier_array_example1():
-    """Multiplier array variables"""
-    multiplier_input_precision = [8, 8]
-    multiplier_energy = 0.5
-    multiplier_area = 0.1
-    dimensions = {"D1": 14, "D2": 3, "D3": 4}
-    operand_spatial_sharing = {
-        "I1": {(1, 0, 0)},
-        "O": {(0, 1, 0)},
-        "I2": {(0, 0, 1), (1, 1, 0)},
-    }
-    multiplier = Multiplier(
-        multiplier_input_precision, multiplier_energy, multiplier_area
-    )
-    multiplier_array = MultiplierArray(multiplier, dimensions, operand_spatial_sharing)
-
-    return multiplier_array
-
-
-def multiplier_array_example2():
-    """Multiplier array variables"""
-    multiplier_input_precision = [8, 8]
-    multiplier_energy = 0.5
-    multiplier_area = 0.1
-    dimensions = {"D1": 14, "D2": 12}
-    operand_spatial_sharing = {"I1": {(1, 0)}, "O": {(0, 1)}, "I2": {(1, 1)}}
-    multiplier = Multiplier(
-        multiplier_input_precision, multiplier_energy, multiplier_area
-    )
-    multiplier_array = MultiplierArray(multiplier, dimensions, operand_spatial_sharing)
-
-    return multiplier_array
-
-
-if __name__ == "__main__":
-    multiplier_array = multiplier_array_example1()
-    for os in multiplier_array.operand_spatial_sharing:
-        print(
-            f"{os}\tdirection: {os.direction} operand: {os.operand} instances: {os.instances}"
-        )
+#     return multiplier_array
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/operational_unit.py` & `zigzag_dse-3.1.1/zigzag/hardware/architecture/operational_unit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,45 @@
-from typing import List
+from zigzag.utils import json_repr_handler
+
 
-## General class for a unit that performs a certain operation. For example: a multiplier unit.
 class OperationalUnit:
-    
-    ## The class constructor
-    # @param input_precision: The bit precision of the operation inputs.
-    # @param output_precision: The bit precision of the operation outputs.
-    # @param unit_cost: The energy cost of performing a single operation.
-    # @param unit_area: The area of a single operational unit.
+    """! General class for a unit that performs a certain operation. For example: a multiplier unit."""
+
     def __init__(
         self,
-        input_precision: List[int],
+        input_precision: list[int],
         output_precision: int,
         unit_cost: float,
         unit_area: float,
     ):
+        """
+        @param input_precision: The bit precision of the operation inputs.
+        @param output_precision: The bit precision of the operation outputs.
+        @param unit_cost: The energy cost of performing a single operation.
+        @param unit_area: The area of a single operational unit.
+        """
         self.input_precision = input_precision
         self.output_precision = output_precision
         self.precision = input_precision + [output_precision]
         self.cost = unit_cost
         self.area = unit_area
 
-    ## JSON Representation of this class to save it to a json file.
     def __jsonrepr__(self):
-        return self.__dict__
+        """! JSON Representation of this class to save it to a json file."""
+        return json_repr_handler(self.__dict__)
 
     def __eq__(self, __o: object) -> bool:
         if not isinstance(__o, OperationalUnit):
             return False
-        return (
-            self.precision == __o.precision
-            and self.cost == __o.cost
-            and self.area == __o.area
-        )
+        return self.precision == __o.precision and self.cost == __o.cost and self.area == __o.area
 
 
-## Description missing
 class Multiplier(OperationalUnit):
 
-    ## The class constructor
-    # @param input_precision: The bit precision of the multiplication inputs.
-    # @param energy_cost: The energy cost of performing a single multiplication.
-    # @param area: The area of a single multiplier.
-    def __init__(self, input_precision: List[int], energy_cost: float, area: float):
+    def __init__(self, input_precision: list[int], energy_cost: float, area: float):
+        """
+        @param input_precision: The bit precision of the multiplication inputs.
+        @param energy_cost: The energy cost of performing a single multiplication.
+        @param area: The area of a single multiplier.
+        """
         output_precision = sum(input_precision)
         super().__init__(input_precision, output_precision, energy_cost, area)
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/io/onnx/utils.py` & `zigzag_dse-3.1.1/zigzag/parser/onnx/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-import enum
 import importlib
 import logging
 from dataclasses import dataclass
 from enum import auto
 from os import path
-from typing import List
+from typing import Any, List
+from enum import Enum
 import pickle
-
 import onnx
-from onnx import AttributeProto, helper, compose
+from onnx import AttributeProto, helper, compose, ModelProto, GraphProto, NodeProto, TypeProto
 
 logger = logging.getLogger(__name__)
 
 BRANCH_ATTRIBUTE = "branch"
 
-## Parse the input accelerator residing in accelerator_path.
-# @param mapping_path
-def parse_mapping_from_path(mapping_path):
+
+def parse_mapping_from_path(mapping_path: str | None) -> dict[str, dict[str, Any]]:
+    """! Parse the input accelerator residing in accelerator_path.
+    @param mapping_path
+    """
     # Sanity check on mapping_path
     if mapping_path is None:
         # Update the mapping_path to the default mapping file
         if path.exists("inputs/examples/mapping/default.py"):
             mapping_path = "zigzag.inputs.examples.mapping.default"
         else:
-            raise ValueError(
-                "No mapping path/dict provided, and default was not found."
-            )
+            raise ValueError("No mapping path/dict provided, and default was not found.")
     if "/" in mapping_path and mapping_path.split(".")[-1] in [
         "pickle",
         "pkl",
         "mapping",
     ]:
         # Load in the pickle mapping file
         with open(mapping_path, "rb") as fp:
@@ -38,40 +37,41 @@
         global module
         module = importlib.import_module(mapping_path)
         mapping = module.mapping
     if "default" in mapping:
         default_present = "\u2705"
     else:
         default_present = "\u274C"
-    logger.debug(
-        f"Parsed mapping with {len(mapping)} different entries. Default: {default_present}."
-    )
+    logger.debug(f"Parsed mapping with {len(mapping)} different entries. Default: {default_present}.")
     return mapping
 
 
-def parse_onnx_model_from_path(onnx_model_path):
-    return onnx.load(onnx_model_path, load_external_data=False)
+def parse_onnx_model_from_path(onnx_model_path: str) -> ModelProto:
+    return onnx.load(onnx_model_path, load_external_data=False)  # type: ignore
+
 
-def add_attribute(node, name, value):
+def add_attribute(node: NodeProto, name: str, value: Any):
     attr = helper.make_attribute(name, value)
     if hasattr(node, "attribute"):
         node.attribute.append(attr)
     else:
         raise ValueError(f"{node} doesn't have an attribute field.")
 
-def add_branch_attribute(graph, branch=0):
+
+def add_branch_attribute(graph: GraphProto, branch: int = 0):
     for node in graph.node:
         add_attribute(node, BRANCH_ATTRIBUTE, branch)
         if node.op_type in ["If"]:
             g0 = node.attribute[0].g  # then or else branch
             g1 = node.attribute[1].g  # then or else branch
             add_branch_attribute(g0, branch + 1)
             add_branch_attribute(g1, branch + 1)
 
-def unroll_branches(graph):
+
+def unroll_branches(graph: GraphProto) -> GraphProto:
     seen_if = False
     new_graph = graph
     for node in graph.node:
         if node.op_type in ["If"]:
             if seen_if:
                 raise ValueError("Unrolling only implemented for single If operator in model.")
             seen_if = True
@@ -91,63 +91,62 @@
             # Add value info to subgraph input if it's not present
             if input_name not in [vi.name for vi in g0.input]:
                 g0.input.extend([value_info])
             # g0 is the graph we will combine with the original one
             new_graph = compose.merge_graphs(graph, g0, io_map=[(input_name, input_name)])
             break
     return new_graph
-            
-def is_dynamic(model):
+
+
+def is_dynamic(model: ModelProto):
     return "If" in [n.op_type for n in model.graph.node]
 
-## Modifies the given onnx model if there's dynamic behavior in terms of an 'If' operator.
-# All nodes are assigned a 'branch' attribute which specifies in which branch they live.
-# The branch attribute starts from 0 and increases for each seen If operator.
-# The nested graphs of the 'If' operators are then unrolled into a planar onnx model.
-def parse_dynamic_onnx_model(model):
+
+def parse_dynamic_onnx_model(model: ModelProto) -> ModelProto:
+    """! Modifies the given onnx model if there's dynamic behavior in terms of an 'If' operator.
+    All nodes are assigned a 'branch' attribute which specifies in which branch they live.
+    The branch attribute starts from 0 and increases for each seen If operator.
+    The nested graphs of the 'If' operators are then unrolled into a planar onnx model.
+    """
     new_model = model
     if is_dynamic(model):
         add_branch_attribute(model.graph)
         pass
         graph = unroll_branches(model.graph)
         new_model = helper.make_model(graph)
     return new_model
 
-## Retrieves the attrs[name_idx].ints from attrs.
-# If attrs[name_idx] is of type INTS, attrs[name_idx].ints is returned.
-# If attrs[name_idx] is of type INT, attrs[name_idx].i is returned.
-# If name does not exist in attrs, the default provided by the caller is used.
-# If the caller doesn't supply a default, an error is thrown.
-# @param name
-# @param attrs
-# @param default
-def get_attribute_ints_with_name(name, attrs, default=None):
+
+def get_attribute_ints_with_name(name: str, attrs: Any, default: list[int] | int | None = None) -> list[int] | int:
+    """! Retrieves the attrs[name_idx].ints from attrs.
+    If attrs[name_idx] is of type INTS, attrs[name_idx].ints is returned.
+    If attrs[name_idx] is of type INT, attrs[name_idx].i is returned.
+    If name does not exist in attrs, the default provided by the caller is used.
+    If the caller doesn't supply a default, an error is thrown.
+
+    """
     attrs_names = [attr.name for attr in attrs]
     try:
         name_idx = attrs_names.index(name)
         attr_type = attrs[name_idx].type
         if attr_type == AttributeProto.AttributeType.INT:
-            return attrs[name_idx].i
+            return int(attrs[name_idx].i)
         elif attr_type == AttributeProto.AttributeType.INTS:
-            return attrs[name_idx].ints
+            return list(attrs[name_idx].ints)
         else:
-            raise NotImplementedError(
-                f"Attribute extraction of type {attr_type} not supported."
-            )
+            raise NotImplementedError(f"Attribute extraction of type {attr_type} not supported.")
     except ValueError:
         if default is not None:
             return default
         else:
-            raise ValueError(
-                f"attrs has no attribute called {name} and no default was given. Names = {attrs_names}."
-            )
+            raise ValueError(f"attrs has no attribute called {name} and no default was given. Names = {attrs_names}.")
+
 
+class OnnxTensorCategory(Enum):
 
-## Description missing
-class OnnxTensorCategory(enum.Enum):
     Input = auto()
     Output = auto()
     Hidden = auto()
     Constant = auto()
 
     @property
     def is_output(self):
@@ -163,63 +162,55 @@
 
     @property
     def is_constant(self):
         return self == OnnxTensorCategory.Constant
 
 
 @dataclass
-## Description missing
 class OnnxTensorType:
+
     shape: List[int]
     elem_type: int
     category: OnnxTensorCategory
 
     @staticmethod
-    def from_tensor_type(tensor_type, category: OnnxTensorCategory):
+    def from_tensor_type(tensor_type: TypeProto.Tensor, category: OnnxTensorCategory):
         shape = [d.dim_value for d in tensor_type.shape.dim]
         elem_type = tensor_type.elem_type
 
         return OnnxTensorType(shape, elem_type, category)
 
 
-def get_onnx_tensor_type(name, model):
+def get_onnx_tensor_type(name: str, model: ModelProto):
     for input in model.graph.input:
         if input.name == name:
-            return OnnxTensorType.from_tensor_type(
-                input.type.tensor_type, OnnxTensorCategory.Input
-            )
+            return OnnxTensorType.from_tensor_type(input.type.tensor_type, OnnxTensorCategory.Input)
 
     for output in model.graph.output:
         if output.name == name:
-            return OnnxTensorType.from_tensor_type(
-                output.type.tensor_type, OnnxTensorCategory.Output
-            )
+            return OnnxTensorType.from_tensor_type(output.type.tensor_type, OnnxTensorCategory.Output)
 
     for value_info in model.graph.value_info:
         if value_info.name == name:
-            return OnnxTensorType.from_tensor_type(
-                value_info.type.tensor_type, OnnxTensorCategory.Hidden
-            )
+            return OnnxTensorType.from_tensor_type(value_info.type.tensor_type, OnnxTensorCategory.Hidden)
 
     for init in model.graph.initializer:
         if init.name == name:
             # initializers are represented a bit differently from other tensors
-            return OnnxTensorType(
-                list(init.dims), init.data_type, OnnxTensorCategory.Constant
-            )
+            return OnnxTensorType(list(init.dims), init.data_type, OnnxTensorCategory.Constant)
 
     raise KeyError(
         f""
         f"Could not find type for value {name} in model. "
         f"Make sure you are loading in an inferred model, "
         f"see https://github.com/onnx/onnx/blob/main/docs/PythonAPIOverview.md#running-shape-inference-on-an-onnx-model"
     )
 
 
-def get_node_input_output_dimension_shapes(node, model):
+def get_node_input_output_dimension_shapes(node: NodeProto, model: ModelProto):
     # assumed it is the first input, don't see a way to otherwise know
     input_name = node.input[0]
     input_shape = get_onnx_tensor_type(input_name, model).shape
 
     output_name = node.output[0]
     output_shape = get_onnx_tensor_type(output_name, model).shape
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/mapping/combined_mapping.py` & `zigzag_dse-3.1.1/zigzag/mapping/Mapping.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,557 +1,344 @@
-from typing import Dict
-from math import prod
-from zigzag.classes.workload.layer_node import LayerNode
-from zigzag.classes.mapping.spatial.spatial_mapping import SpatialMapping
-from zigzag.classes.mapping.temporal.temporal_mapping import TemporalMapping
-from zigzag.classes.hardware.architecture.accelerator import Accelerator
-import zigzag.classes.mapping.mapping_assist_funcs as mapping_assist_funcs
-
-## The standard four-way data moving attribute of a memory interface.
-class FourWayDataMoving:
-
-    ## The class constructor
-    # @param rd_out_to_low
-    # @param wr_in_by_low
-    # @param rd_out_to_high
-    # @param wr_in_by_high
-    def __init__(self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high):
-        self.rd_out_to_low = rd_out_to_low
-        self.wr_in_by_low = wr_in_by_low
-        self.rd_out_to_high = rd_out_to_high
-        self.wr_in_by_high = wr_in_by_high
-        """ format used in the original ZigZag version """
-        self.info_list = [
-            (self.rd_out_to_low, self.wr_in_by_low),
-            (self.rd_out_to_high, self.wr_in_by_high),
-        ]
-
-    def update_single_dir_data(self, dir: str, new_value):
-        setattr(self, dir, new_value)
-        self.info_list = [
-            (self.rd_out_to_low, self.wr_in_by_low),
-            (self.rd_out_to_high, self.wr_in_by_high),
-        ]
-
-    ## Return the total amount of times this memory interface is read from to the level above.
-    # If scaling is the energy cost per read, this returns the total read energy.
-    def get_total_read_outs_to_above(self, scaling: float = 1):
-        return scaling * self.rd_out_to_high
-
-    ## Return the total amount of times this memory interface is read from to the level below.
-    # If scaling is the energy cost per read, this returns the total read energy.
-    def get_total_read_outs_to_below(self, scaling: float = 1):
-        return scaling * self.rd_out_to_low
-
-    ## Return the total amount of times this memory interface is written to from the level above.
-    # If scaling is the energy cost per write, this returns the total read energy.
-    def get_total_write_ins_from_above(self, scaling: float = 1):
-        return scaling * self.wr_in_by_high
-
-    ## Return the total amount of times this memory interface is written to from the level below.
-    # If scaling is the energy cost per write, this returns the total read energy.
-    def get_total_write_ins_from_below(self, scaling: float = 1):
-        return scaling * self.wr_in_by_low
-
-    def __add__(self, other):
-        return FourWayDataMoving(
-            self.rd_out_to_low + other.rd_out_to_low,
-            self.wr_in_by_low + other.wr_in_by_low,
-            self.rd_out_to_high + other.rd_out_to_high,
-            self.wr_in_by_high + other.wr_in_by_high,
-        )
-
-    def __mul__(self, other):
-        return FourWayDataMoving(
-            self.rd_out_to_low * other,
-            self.wr_in_by_low * other,
-            self.rd_out_to_high * other,
-            self.wr_in_by_high * other,
-        )
-
-    def __iter__(self):
-        for e in ["rd_out_to_low", "wr_in_by_low", "rd_out_to_high", "wr_in_by_high"]:
-            yield e
-
-    def __repr__(self):
-        return f"4waydatamoving (rd /\\: {self.rd_out_to_high}, wr V: {self.wr_in_by_high}, rd V: {self.rd_out_to_low}, wr /\\: {self.wr_in_by_low})"
-
-    def __jsonrepr__(self):
-        return repr(self)
-
-    def __getitem__(self, item):
-        if hasattr(self, item):
-            return getattr(self, item)
-        else:
-            raise KeyError()
-
-
-## Collect the memory access pattern for each unit memory (memory that only hold one operand at one level).
-class DataMovePattern:
-
-    ## The class construcotr
-    # @param operand
-    # @param mem_level
-    def __init__(self, operand, mem_level):
-        self.name = operand + str(mem_level)
-        self.data_elem_move_count = FourWayDataMoving(0, 0, 0, 0)
-        self.data_precision = FourWayDataMoving(0, 0, 0, 0)
-        self.req_mem_bw_aver = FourWayDataMoving(0, 0, 0, 0)
-        self.req_mem_bw_inst = FourWayDataMoving(0, 0, 0, 0)
-        self.data_trans_period = FourWayDataMoving(0, 0, 0, 0)
-        self.data_trans_period_count = FourWayDataMoving(0, 0, 0, 0)
-        self.data_trans_amount_per_period = FourWayDataMoving(0, 0, 0, 0)
-        self.inst_data_trans_window = FourWayDataMoving(0, 0, 0, 0)
-
-    # For every memory, there are 4 data transfer link in the hierarchy: 
-    # rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
-
-    def set_data_elem_move_count(
-        self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
-    ):
-        self.data_elem_move_count = FourWayDataMoving(
-            rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
-        )
-
-    def set_data_precision(
-        self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
-    ):
-        self.data_precision = FourWayDataMoving(
-            rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
-        )
-
-    def set_req_mem_bw_aver(
-        self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
-    ):
-        self.req_mem_bw_aver = FourWayDataMoving(
-            rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
-        )
-
-    def set_req_mem_bw_inst(
-        self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
-    ):
-        self.req_mem_bw_inst = FourWayDataMoving(
-            rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
-        )
-
-    def set_data_trans_period(
-        self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
-    ):
-        # data_trans_period: every how many cycle, the memory link need to be activated for a certain duration
-        self.data_trans_period = FourWayDataMoving(
-            rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
-        )
-
-    def set_data_trans_period_count(
-        self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
-    ):
-        # data_trans_period_count: to finish all the for-loop computation, how many such ideal_period is required
-        self.data_trans_period_count = FourWayDataMoving(
-            rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
-        )
+import math
+from zigzag.datatypes import Constants, LayerOperand
+from zigzag.hardware.architecture.memory_port import DataDirection
+from zigzag.mapping.data_movement import DataMovePattern
+from zigzag.workload.layer_node import LayerNode
+from zigzag.mapping.SpatialMappingInternal import SpatialMappingInternal
+from zigzag.mapping.TemporalMapping import TemporalMapping, TemporalMappingDict
+from zigzag.hardware.architecture.Accelerator import Accelerator
+from zigzag.mapping.mapping_assist_funcs import SpatialMappingPerMemLvl
+import zigzag.mapping.mapping_assist_funcs as mapping_assist_funcs
 
-    def set_data_trans_amount_per_period(
-        self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
-    ):
-        # data_trans_amount_per_period: data amount that being transferred for each single period
-        self.data_trans_amount_per_period = FourWayDataMoving(
-            rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
-        )
-
-    def set_inst_data_trans_window(
-        self, rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
-    ):
-        # inst_data_trans_window: the allowed memory updating window, assuming the served memory level
-        # is non-double buffered (thus need to avoid the data overwriting issue
-        self.inst_data_trans_window = FourWayDataMoving(
-            rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
-        )
 
-    ## update a single direction value for all data move attributes
-    def update_single_dir_data(self, direction, new_value):
-        self.data_elem_move_count.update_single_dir_data(direction, new_value)
-        self.data_precision.update_single_dir_data(direction, new_value)
-        self.req_mem_bw_aver.update_single_dir_data(direction, new_value)
-        self.req_mem_bw_inst.update_single_dir_data(direction, new_value)
-        self.data_trans_period.update_single_dir_data(direction, new_value)
-        self.data_trans_period_count.update_single_dir_data(direction, new_value)
-        self.data_trans_amount_per_period.update_single_dir_data(direction, new_value)
-        self.inst_data_trans_window.update_single_dir_data(direction, new_value)
-
-    def __str__(self):
-        return self.name
-
-    def __repr__(self):
-        return str(self)
-
-
-## Collect information of a complete mapping (spatial and temporal)
-# 
-# NOTE: Mapping is HW-unaware, i.e. Mapping doesn't take in HW information
-# like memory bw, access cost, size and so on.
 class Mapping:
+    """! Collect information of a complete mapping (spatial and temporal)
+
+    NOTE: Mapping is HW-unaware, i.e. Mapping doesn't take in HW information
+    like memory bw, access cost, size and so on.
+    """
 
-    ## The class construcotr
-    # @param accelerator
-    # @param spatial mapping
-    # @param temporal mapping
-    # @param layer_node
-    # @param access_same_data_considered_as_no_access
     def __init__(
         self,
         accelerator: Accelerator,
-        spatial_mapping: Dict or SpatialMapping,
-        temporal_mapping: Dict or TemporalMapping,
+        spatial_mapping: SpatialMappingPerMemLvl | SpatialMappingInternal,
+        temporal_mapping: TemporalMappingDict | TemporalMapping,
         layer_node: LayerNode,
         access_same_data_considered_as_no_access: bool = False,
     ):
         # Mapping object can be initialized with separate spatial and temporal mappings
         self.accelerator = accelerator
-        if type(spatial_mapping) is SpatialMapping:
+        if isinstance(spatial_mapping, SpatialMappingInternal):
             self.spatial_mapping = spatial_mapping
         else:
-            self.spatial_mapping = SpatialMapping(spatial_mapping, layer_node)
-        if type(temporal_mapping) is TemporalMapping:
+            self.spatial_mapping = SpatialMappingInternal(spatial_mapping, layer_node)
+        if isinstance(temporal_mapping, TemporalMapping):
             self.temporal_mapping = temporal_mapping
         else:
             self.temporal_mapping = TemporalMapping(temporal_mapping, layer_node)
         self.layer_node = layer_node
-        self.operand_list = layer_node.operand_list
-        self.access_same_data_considered_as_no_access = (
-            access_same_data_considered_as_no_access
-        )
+        self.operand_list = layer_node.layer_operands
+        self.access_same_data_considered_as_no_access = access_same_data_considered_as_no_access
         self.mem_level = self.temporal_mapping.mem_level
-        # Initialize unit_mem_data_movement, which collects all the important data movement info 
-        # related to each unit memory, such as data access count, data precision, required memory BW to 
+        # Initialize unit_mem_data_movement, which collects all the important data movement info
+        # related to each unit memory, such as data access count, data precision, required memory BW to
         # prevent stall, data transfer rate, etc.
-        self.unit_mem_data_movement = {
-            op: [[] for _ in range(self.mem_level[op])] for op in self.operand_list
+        self.unit_mem_data_movement: dict[LayerOperand, list[DataMovePattern]] = {  # type: ignore
+            op: [None for _ in range(self.mem_level[op])] for op in self.operand_list
         }
 
-        # Combine spatial and temporal mapping dictionary into "joint_mapping_dict" in order to 
+        # Combine spatial and temporal mapping dictionary into "joint_mapping_dict" in order to
         # enable decoupling pr loops into r and ir loops in one go
         self.combine_spatial_temporal_mapping_dict()
 
         # Decouple pr loops into r and ir loops, preparing for later mapping info extraction
         self.combined_mapping_dict_1s1t_reform = mapping_assist_funcs.decouple_pr_loop(
             self.combined_mapping_dict_1s1t, layer_node
         )
         self.combined_mapping_dict_1s2t_reform = mapping_assist_funcs.decouple_pr_loop(
             self.combined_mapping_dict_1s2t, layer_node
         )
 
         # Distinguish final output from partial output: "psum_flag"
-        self.distinguish_output()
+        self.psum_flag = self.get_psum_flags()
 
         # Generate a dictionary that collect data precision for each operand at each arch level
         self.gen_data_precision_dict()
 
         # Generate r/ir loop size list at each level for each operand
         self.gen_r_ir_loop_list()
 
-        # Calculate data size at each memory level, including total data size and 
-        # unrolled data size (data at each unrolled memory unit). Unit used: # element 
+        # Calculate data size at each memory level, including total data size and
+        # unrolled data size (data at each unrolled memory unit). Unit used: # element
         self.calc_data_size()
 
         # Calculate the effective data size at each unrolled memory unit.
         # Effective data size: the unrolled data size divided by all top r loops at that level.
         # Unit used: # element
         self.calc_effective_data_size()
 
-        # Calculate data access count at each memory level. Unit used: # element 
+        # Calculate data access count at each memory level. Unit used: # element
         # NOTE: this data access is not memory word access!
         self.calc_data_access()
 
         # Calculate required memory bandwidth and the periodic data transfer pattern
         self.calc_req_mem_bw_and_data_transfer_rate()
 
         # Ignore the data traffic between the top level memory and the external world
         self.disable_data_traffic_external()
 
-    ## Combine spatial and temporal mapping dictionary into combined_mapping_dict by
-    # inserting spatial loops above temporal loops at each level.
-    #
-    # - combined_mapping_dict_1s1t: corresponding level's smap and tmap are merged together.
-    # Each level's data size is the total data size.
-    # - combined_mapping_dict_1s2t: each level's smap is merged to level+1's tmap.
-    # Each level's data size is the unrolled data size.
     def combine_spatial_temporal_mapping_dict(self):
+        """! Combine spatial and temporal mapping dictionary into combined_mapping_dict by
+        inserting spatial loops above temporal loops at each level.
+
+        - combined_mapping_dict_1s1t: corresponding level's smap and tmap are merged together.
+        Each level's data size is the total data size.
+        - combined_mapping_dict_1s2t: each level's smap is merged to level+1's tmap.
+        Each level's data size is the unrolled data size.
+        """
 
         # Initialization
         combined_mapping_dict_1s1t = {
-            op: [[] for _ in range(self.spatial_mapping.arch_level[op])]
-            for op in self.operand_list
+            op: [[] for _ in range(self.spatial_mapping.arch_level[op])] for op in self.operand_list
         }
         combined_mapping_dict_1s2t = {
-            op: [[] for _ in range(self.spatial_mapping.arch_level[op] + 1)]
-            for op in self.operand_list
+            op: [[] for _ in range(self.spatial_mapping.arch_level[op] + 1)] for op in self.operand_list
         }
         su_dict_seed = self.spatial_mapping.mapping_dict_origin
         # Add an empty innermost level and an empty outermost level
         tm_dict_seed = {
-            op: [[]] + tm_list + [[]]
-            for op, tm_list in self.temporal_mapping.mapping_dic_stationary.items()
+            op: [[]] + tm_list + [[]] for op, tm_list in self.temporal_mapping.mapping_dic_stationary.items()
         }
 
         # Combining
         for operand in self.operand_list:
             for level, current_level_su_loops in enumerate(su_dict_seed[operand]):
                 current_level_tm_loops = tm_dict_seed[operand][level]
                 above_level_tm_loops = tm_dict_seed[operand][level + 1]
-                combined_mapping_dict_1s1t[operand][level] = (
-                    current_level_tm_loops + current_level_su_loops
-                )
-                combined_mapping_dict_1s2t[operand][level + 1] = (
-                    above_level_tm_loops + current_level_su_loops
-                )
+                combined_mapping_dict_1s1t[operand][level] = current_level_tm_loops + current_level_su_loops
+                combined_mapping_dict_1s2t[operand][level + 1] = above_level_tm_loops + current_level_su_loops
 
         self.combined_mapping_dict_1s1t = combined_mapping_dict_1s1t
         self.combined_mapping_dict_1s2t = combined_mapping_dict_1s2t
 
-    ## This function generates an list "psum_flag" that identify whether an output memory
-    # level holds partial or final output.
-    # E.g., psum_flag = [True, True, False] means that there are 3 memory levels for output and only the outermost
-    # memory level hold the final output, the 1st and 2nd memory levels need to store partial output for some time.
-    # For indexing convenience, we add an extra False to the end of the psum_flag list.
-    def distinguish_output(self):
+    def get_psum_flags(self) -> list[bool]:
+        """! This function generates an list "psum_flag" that identify whether an output memory
+        level holds partial or final output.
+        E.g., psum_flag = [True, True, False] means that there are 3 memory levels for output and only the outermost
+        memory level hold the final output, the 1st and 2nd memory levels need to store partial output for some time.
+        For indexing convenience, we add an extra False to the end of the psum_flag list.
+        # TODO cleanup
+        """
         output_operand = self.layer_node.output_operand
-        output_loop_dim_relevancy = self.layer_node.operand_loop_dim_reform[
-            output_operand
-        ]
+        loop_dim_relevancy = self.layer_node.pr_decoupled_relevancy_info
         # output_ir_flag indicate whether at an architectural level, there is output's ir loop in it.
         # True for yes, there is.
         output_arch_level = self.spatial_mapping.arch_level[output_operand]
         output_ir_flag = [False] * output_arch_level
-        for level, current_level_loops in enumerate(
-            self.combined_mapping_dict_1s1t_reform[output_operand]
-        ):
+        for level, current_level_loops in enumerate(self.combined_mapping_dict_1s1t_reform[output_operand]):
             for loop_type, loop_dim in current_level_loops:
-                if loop_type in output_loop_dim_relevancy["ir"] and loop_dim > 1:
+                if loop_type in loop_dim_relevancy.get_ir_layer_dims(output_operand) and loop_dim > 1:
                     output_ir_flag[level] = True
                     break
-        # reversely check from current level to the top level whether there is ir loop shows up in the middle, 
+        # reversely check from current level to the top level whether there is ir loop shows up in the middle,
         # False means final output is present at current level
-        psum_flag_H2L = [
-            any(output_ir_flag[lv:output_arch_level])
-            for lv in reversed(range(output_arch_level))
-        ]
+        psum_flag_H2L = [any(output_ir_flag[lv:output_arch_level]) for lv in reversed(range(output_arch_level))]
         psum_flag_L2H = list(reversed(psum_flag_H2L))
-        self.psum_flag = psum_flag_L2H[1:] + [
-            False
-        ]  # add an extra False on top for later indexing convenience
+        return psum_flag_L2H[1:] + [False]  # add an extra False on top for later indexing convenience
 
-    ## This function generates a dictionary that collect data precision for each operand at each arch level
     def gen_data_precision_dict(self):
+        """! This function generates a dictionary that collect data precision for each operand at each arch level"""
         input_operands = self.layer_node.input_operands
         output_operand = self.layer_node.output_operand
-        data_precision_dict = {
-            op: [self.layer_node.operand_precision[op]] * (self.mem_level[op] + 1)
-            for op in input_operands
+        data_precision_dict: dict[LayerOperand, list[int]] = {
+            op: [self.layer_node.operand_precision[op]] * (self.mem_level[op] + 1) for op in input_operands
         }
         data_precision_dict[output_operand] = []
         for i in range(self.mem_level[output_operand] + 1):
             if self.psum_flag[i]:
-                data_precision_dict[output_operand].append(
-                    self.layer_node.operand_precision[output_operand]
-                )
+                data_precision_dict[output_operand].append(self.layer_node.operand_precision[output_operand])
             else:
                 data_precision_dict[output_operand].append(
-                    self.layer_node.operand_precision[output_operand + "_final"]
+                    self.layer_node.operand_precision[Constants.FINAL_OUTPUT_LAYER_OP]
                 )
         self.data_precision_dict = data_precision_dict
 
-    ## Given the combined mapping, generate r/ir loop size list at each level for each operand
     def gen_r_ir_loop_list(self):
+        """! Given the combined mapping, generate r/ir loop size list at each level for each operand
+        # TODO cleanup
+        """
         combined_mapping = self.combined_mapping_dict_1s1t_reform
         combined_mapping2 = self.combined_mapping_dict_1s2t_reform
-        relevancy_table = self.layer_node.operand_loop_dim_reform
+        relevancy_table = self.layer_node.pr_decoupled_relevancy_info
         r_loop_size_per_level = {
             op: [
-                prod(
+                math.prod(
                     [
                         lp_dim
                         for lp_type, lp_dim in combined_mapping[op][lv]
-                        if lp_type in relevancy_table[op]["r"]
+                        if lp_type in relevancy_table.get_r_layer_dims(op)
                     ]
                 )
                 for lv in range(self.spatial_mapping.arch_level[op])
             ]
             for op in self.operand_list
         }
         r_loop_size_per_level2 = {
             op: [
-                prod(
+                math.prod(
                     [
                         lp_dim
                         for lp_type, lp_dim in combined_mapping2[op][lv]
-                        if lp_type in relevancy_table[op]["r"]
+                        if lp_type in relevancy_table.get_r_layer_dims(op)
                     ]
                 )
                 for lv in range(self.spatial_mapping.arch_level[op])
             ]
             for op in self.operand_list
         }
         ir_loop_size_per_level = {
             op: [
-                prod(
+                math.prod(
                     [
                         lp_dim
                         for lp_type, lp_dim in combined_mapping[op][lv]
-                        if lp_type in relevancy_table[op]["ir"]
+                        if lp_type in relevancy_table.get_ir_layer_dims(op)
                     ]
                 )
                 for lv in range(self.spatial_mapping.arch_level[op])
             ]
             for op in self.operand_list
         }
         ir_loop_size_per_level2 = {
             op: [
-                prod(
+                math.prod(
                     [
                         lp_dim
                         for lp_type, lp_dim in combined_mapping2[op][lv]
-                        if lp_type in relevancy_table[op]["ir"]
+                        if lp_type in relevancy_table.get_ir_layer_dims(op)
                     ]
                 )
                 for lv in range(self.spatial_mapping.arch_level[op])
             ]
             for op in self.operand_list
         }
 
         # current and below levels (cabl) r loop size
         r_loop_size_cabl = {
             op: [
-                round(prod(r_loop_size_per_level[op][0 : lv + 1]))
+                round(math.prod(r_loop_size_per_level[op][0 : lv + 1]))
                 for lv in range(self.spatial_mapping.arch_level[op])
             ]
             for op in self.operand_list
         }
         r_loop_size_cabl2 = {
             op: [
-                round(prod(r_loop_size_per_level2[op][0 : lv + 1]))
+                round(math.prod(r_loop_size_per_level2[op][0 : lv + 1]))
                 for lv in range(self.spatial_mapping.arch_level[op])
             ]
             for op in self.operand_list
         }
         # current and below levels (cabl) ir loop size
         ir_loop_size_cabl = {
-            op: [
-                prod(ir_loop_size_per_level[op][0 : lv + 1])
-                for lv in range(self.spatial_mapping.arch_level[op])
-            ]
+            op: [math.prod(ir_loop_size_per_level[op][0 : lv + 1]) for lv in range(self.spatial_mapping.arch_level[op])]
             for op in self.operand_list
         }
         # current and below levels (cabl) ir loop size
         ir_loop_size_cabl2 = {
             op: [
-                prod(ir_loop_size_per_level2[op][0 : lv + 1])
-                for lv in range(self.spatial_mapping.arch_level[op])
+                math.prod(ir_loop_size_per_level2[op][0 : lv + 1]) for lv in range(self.spatial_mapping.arch_level[op])
             ]
             for op in self.operand_list
         }
         # current and above levels (caal) ir loop size, only for output operand for calculating psum backflow access count
         output_operand = self.layer_node.output_operand
         O_ir_loop_size_caal = [
-            prod(
-                ir_loop_size_per_level[output_operand][
-                    lv : self.spatial_mapping.arch_level[output_operand]
-                ]
-            )
+            math.prod(ir_loop_size_per_level[output_operand][lv : self.spatial_mapping.arch_level[output_operand]])
             for lv in range(self.spatial_mapping.arch_level[output_operand])
         ]
-        # append two extra 1 to the list to facilitate the psum bcakflow access calculation later
+        # append two extra 1 to the list to facilitate the psum backflow access calculation later
         # We can see it as adding two output memory levels on top with no data reuse.
         O_ir_loop_size_caal.extend([1, 1])
 
         self.r_loop_size_per_level = r_loop_size_per_level
         self.r_loop_size_per_level2 = r_loop_size_per_level2
         self.ir_loop_size_per_level = ir_loop_size_per_level
         self.r_loop_size_cabl = r_loop_size_cabl
         self.r_loop_size_cabl2 = r_loop_size_cabl2
         self.ir_loop_size_cabl = ir_loop_size_cabl
         self.ir_loop_size_cabl2 = ir_loop_size_cabl2
         self.O_ir_loop_size_caal = O_ir_loop_size_caal
 
-    ## Based on the r loop size list, calculate the data size held by each architectural level.
     def calc_data_size(self):
+        """! Based on the r loop size list, calculate the data size held by each architectural level."""
         # data_elem_per_level_unrolled: data size held inside of each unrolled unit at each architectural level
         # data_elem_per_level: total data size at each architectural level (= data_elem_per_level_unrolled * unique unit count)
         data_elem_per_level_unrolled = {
-            op: [
-                round(self.r_loop_size_cabl2[op][lv])
-                for lv in range(self.spatial_mapping.arch_level[op])
-            ]
+            op: [round(self.r_loop_size_cabl2[op][lv]) for lv in range(self.spatial_mapping.arch_level[op])]
             for op in self.operand_list
         }
 
         data_bit_per_level_unrolled = {
             op: [
                 round(self.r_loop_size_cabl2[op][lv]) * self.data_precision_dict[op][lv]
                 for lv in range(self.spatial_mapping.arch_level[op])
             ]
             for op in self.operand_list
         }
 
         data_elem_per_level = {
             op: [
                 round(data_elem_unrolled * self.spatial_mapping.unit_unique[op][lv])
-                for lv, data_elem_unrolled in enumerate(
-                    data_elem_per_level_unrolled[op]
-                )
+                for lv, data_elem_unrolled in enumerate(data_elem_per_level_unrolled[op])
             ]
             for op in self.operand_list
         }
 
         data_bit_per_level = {
             op: [
-                round(data_elem_unrolled * self.spatial_mapping.unit_unique[op][lv])
-                * self.data_precision_dict[op][lv]
-                for lv, data_elem_unrolled in enumerate(
-                    data_elem_per_level_unrolled[op]
-                )
+                round(data_elem_unrolled * self.spatial_mapping.unit_unique[op][lv]) * self.data_precision_dict[op][lv]
+                for lv, data_elem_unrolled in enumerate(data_elem_per_level_unrolled[op])
             ]
             for op in self.operand_list
         }
 
         self.data_elem_per_level_unrolled = data_elem_per_level_unrolled
         self.data_bit_per_level_unrolled = data_bit_per_level_unrolled
         self.data_elem_per_level = data_elem_per_level
         self.data_bit_per_level = data_bit_per_level
 
-    ## Calculate the effective data size for getting the allowed memory updating window in latency calculation.
-    # The effective data size is calculated by using data_elem_per_level_unrolled divided by the top r loops.
     def calc_effective_data_size(self):
+        """! Calculate the effective data size for getting the allowed memory updating window in latency calculation.
+        The effective data size is calculated by using data_elem_per_level_unrolled divided by the top r loops.
+        """
         effective_data_elem = {
             op: [
                 data_elem_unrolled // self.temporal_mapping.top_r_loop_size[op][lv]
-                for lv, data_elem_unrolled in enumerate(
-                    self.data_elem_per_level_unrolled[op]
-                )
+                for lv, data_elem_unrolled in enumerate(self.data_elem_per_level_unrolled[op])
             ]
             for op in self.operand_list
         }
 
         effective_data_bit = {
             op: [
                 data_bit_unrolled // self.temporal_mapping.top_r_loop_size[op][lv]
-                for lv, data_bit_unrolled in enumerate(
-                    self.data_bit_per_level_unrolled[op]
-                )
+                for lv, data_bit_unrolled in enumerate(self.data_bit_per_level_unrolled[op])
             ]
             for op in self.operand_list
         }
         self.effective_data_elem = effective_data_elem
         self.effective_data_bit = effective_data_bit
 
-    ## Based on the ir loop size list and the total MAC Op count, calculate the data access
-    # at each memory level in a bottom-up way.
     def calc_data_access(self):
+        """! Based on the ir loop size list and the total MAC Op count, calculate the data access
+        at each memory level in a bottom-up way.
+        """
         total_MAC_count = self.layer_node.total_MAC_count
 
-        # data_access_raw doesn't distinguish read and write, doesn't distinguish input operands from output operand 
+        # data_access_raw doesn't distinguish read and write, doesn't distinguish input operands from output operand
         # data_access_raw: each memory levels' spatial loops and temporal loops are put together (combined_mapping_dict_1s1t)
         # data_access_raw2: each memory levels' spatial loops are put to memory level + 1s' temporal loops location (combined_mapping_dict_1s2t)
         data_access_raw = {
             op: [
                 round(total_MAC_count / self.ir_loop_size_cabl[op][lv])
                 for lv in range(self.spatial_mapping.arch_level[op])
             ]
@@ -573,29 +360,25 @@
             for mem_level in range(self.mem_level[operand]):
                 unit_mem_data_movement = DataMovePattern(operand, mem_level)
 
                 # data access count
                 if (
                     self.access_same_data_considered_as_no_access
                     and mem_level == 0
-                    and self.accelerator.get_core(
-                        self.layer_node.get_core_allocation()
-                    ).mem_r_bw_dict[self.layer_node.memory_operand_links[operand]][
-                        mem_level
-                    ]
+                    and self.accelerator.get_core(self.layer_node.core_allocation[0]).mem_r_bw_dict[
+                        self.layer_node.memory_operand_links[operand]
+                    ][mem_level]
                     >= self.data_bit_per_level[operand][mem_level]
                     // self.spatial_mapping.unit_unique[operand][mem_level + 1]
                 ):
                     # If we need access the same input data multiple times from the innermost memory level and the data size is smaller than the memory read bw,
                     # take into account only one-time access cost (assume the data can stay at the output pins of the memory as long as it is needed).
                     rd_out_to_low = (
                         data_access_raw[operand][mem_level]
-                        // self.temporal_mapping.MAC_level_data_stationary_cycle[
-                            operand
-                        ]
+                        // self.temporal_mapping.MAC_level_data_stationary_cycle[operand]
                     )
                 else:
                     rd_out_to_low = data_access_raw[operand][mem_level]
                 wr_in_by_low = 0
                 rd_out_to_high = 0
                 wr_in_by_high = data_access_raw2[operand][mem_level + 1]
                 unit_mem_data_movement.set_data_elem_move_count(
@@ -616,97 +399,84 @@
                 self.unit_mem_data_movement[operand][mem_level] = unit_mem_data_movement
 
         # For output operand
         output_operand = self.layer_node.output_operand
         for mem_level in range(self.mem_level[output_operand]):
             unit_mem_data_movement = DataMovePattern(output_operand, mem_level)
 
-            # Note that the index for data_access_raw is arch_level, which is one level more than mem_level. 
-            # the first arch_level means the operational array level (e.g. MAC array level); 
+            # Note that the index for data_access_raw is arch_level, which is one level more than mem_level.
+            # the first arch_level means the operational array level (e.g. MAC array level);
             # the first mem_level means the innermost memory level (e.g. register file level.
 
             # data access count
             wr_in_by_low = data_access_raw[output_operand][mem_level]
             rd_out_to_low = self.layer_node.operand_size_elem[output_operand] * (
                 self.O_ir_loop_size_caal[mem_level + 1] - 1
             )
 
             rd_out_to_high = data_access_raw2[output_operand][mem_level + 1]
             wr_in_by_high = self.layer_node.operand_size_elem[output_operand] * (
                 self.O_ir_loop_size_caal[mem_level + 2] - 1
             )
 
-            unit_mem_data_movement.set_data_elem_move_count(
-                rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high
-            )
+            unit_mem_data_movement.set_data_elem_move_count(rd_out_to_low, wr_in_by_low, rd_out_to_high, wr_in_by_high)
 
             # data precision
             if rd_out_to_low != 0:
                 # partial output data precision
                 wr_in_by_low_pre = self.layer_node.operand_precision[output_operand]
                 rd_out_to_low_pre = self.layer_node.operand_precision[output_operand]
             else:
                 # final output data precision
-                wr_in_by_low_pre = self.layer_node.operand_precision[
-                    output_operand + "_final"
-                ]
+                wr_in_by_low_pre = self.layer_node.operand_precision[Constants.FINAL_OUTPUT_LAYER_OP]
                 rd_out_to_low_pre = 0
             if wr_in_by_high != 0:
                 # partial output data precision
                 wr_in_by_high_pre = self.layer_node.operand_precision[output_operand]
                 rd_out_to_high_pre = self.layer_node.operand_precision[output_operand]
             else:
                 # final output data precision
                 wr_in_by_high_pre = 0
-                rd_out_to_high_pre = self.layer_node.operand_precision[
-                    output_operand + "_final"
-                ]
+                rd_out_to_high_pre = self.layer_node.operand_precision[Constants.FINAL_OUTPUT_LAYER_OP]
 
             unit_mem_data_movement.set_data_precision(
                 rd_out_to_low_pre,
                 wr_in_by_low_pre,
                 rd_out_to_high_pre,
                 wr_in_by_high_pre,
             )
 
-            self.unit_mem_data_movement[output_operand][
-                mem_level
-            ] = unit_mem_data_movement
+            self.unit_mem_data_movement[output_operand][mem_level] = unit_mem_data_movement
 
-    ## This function calculates the average & instant required memory bw and the periodic data transfer pattern.
     def calc_req_mem_bw_and_data_transfer_rate(self):
+        """! This function calculates the average & instant required memory bw and the periodic data transfer pattern."""
 
         if self.access_same_data_considered_as_no_access:
             # For input operands, add operational array level's 'MAC_level_data_stationary_cycle' cycle in the below to align with the list length of data_each_level
             cycle_each_level = {
                 op: [self.temporal_mapping.MAC_level_data_stationary_cycle[op]]
                 + self.temporal_mapping.cycle_cabl_level[op]
                 for op in self.layer_node.input_operands
             }
             # For output operands, add operational array level's 1 cycle in the below to align with the list length of data_each_level
-            cycle_each_level[self.layer_node.output_operand] = [
-                1
-            ] + self.temporal_mapping.cycle_cabl_level[self.layer_node.output_operand]
+            cycle_each_level[self.layer_node.output_operand] = [1] + self.temporal_mapping.cycle_cabl_level[
+                self.layer_node.output_operand
+            ]
         else:
-            cycle_each_level = {
-                op: [1] + self.temporal_mapping.cycle_cabl_level[op]
-                for op in self.operand_list
-            }
+            cycle_each_level = {op: [1] + self.temporal_mapping.cycle_cabl_level[op] for op in self.operand_list}
         data_each_level_unrolled = self.data_elem_per_level_unrolled
 
-        # Add the mem BW boost factor 1 on the top (the memory BW boost factor from outside to top memory) 
+        # Add the mem BW boost factor 1 on the top (the memory BW boost factor from outside to top memory)
         # to align with the list length of data_each_level
-        mem_bw_boost_factor = {
-            op: self.spatial_mapping.mem_bw_boost[op] + [1] for op in self.operand_list
-        }
+        mem_bw_boost_factor = {op: self.spatial_mapping.mem_bw_boost[op] + [1] for op in self.operand_list}
 
-        # req_mem_bw_raw doesn't distinguish read and write, doesn't distinguish input operands from output operand 
-        # "_L/_H" indicates for each data transfer link (DTL), the lower/higher memory level's required BW, 
-        # e.g. for the DTL of Global Buffer (Weight) talking to spatially unrolled Weight Reg File, 
-        # each Weight Reg File's required write BW is indicated by "_L", 
+        # req_mem_bw_raw doesn't distinguish read and write, doesn't distinguish input operands from output operand
+        # "_L/_H" indicates for each data transfer link (DTL), the lower/higher memory level's required BW,
+        # e.g. for the DTL of Global Buffer (Weight) talking to spatially unrolled Weight Reg File,
+        # each Weight Reg File's required write BW is indicated by "_L",
         # while Global Buffer (Weight)'s required read BW is indicate by "_H"
         req_mem_bw_L_raw = {
             op: [
                 data_each_level_unrolled[op][lv] / cycle_each_level[op][lv]
                 for lv in range(self.spatial_mapping.arch_level[op])
             ]
             for op in self.operand_list
@@ -732,80 +502,62 @@
                 wr_in_by_high_bw = req_mem_bw_L_raw[operand][mem_level + 1]
                 self.unit_mem_data_movement[operand][mem_level].set_req_mem_bw_aver(
                     rd_out_to_low_bw,
                     wr_in_by_low_bw,
                     rd_out_to_high_bw,
                     wr_in_by_high_bw,
                 )
-                # data transfer period 
+                # data transfer period
                 rd_out_to_low_pd = cycle_each_level[operand][mem_level]
                 wr_in_by_low_pd = 0
                 rd_out_to_high_pd = 0
                 wr_in_by_high_pd = cycle_each_level[operand][mem_level + 1]
                 self.unit_mem_data_movement[operand][mem_level].set_data_trans_period(
                     rd_out_to_low_pd,
                     wr_in_by_low_pd,
                     rd_out_to_high_pd,
                     wr_in_by_high_pd,
                 )
                 # data transfer period count
-                rd_out_to_low_pc = (
-                    self.temporal_mapping.total_cycle
-                    // cycle_each_level[operand][mem_level]
-                )
+                rd_out_to_low_pc = self.temporal_mapping.total_cycle // cycle_each_level[operand][mem_level]
                 wr_in_by_low_pc = 0
                 rd_out_to_high_pc = 0
-                wr_in_by_high_pc = (
-                    self.temporal_mapping.total_cycle
-                    // cycle_each_level[operand][mem_level + 1]
-                )
-                self.unit_mem_data_movement[operand][
-                    mem_level
-                ].set_data_trans_period_count(
+                wr_in_by_high_pc = self.temporal_mapping.total_cycle // cycle_each_level[operand][mem_level + 1]
+                self.unit_mem_data_movement[operand][mem_level].set_data_trans_period_count(
                     rd_out_to_low_pc,
                     wr_in_by_low_pc,
                     rd_out_to_high_pc,
                     wr_in_by_high_pc,
                 )
                 # per-period data transfer amount
                 rd_out_to_low_da = (
-                    data_each_level_unrolled[operand][mem_level]
-                    * mem_bw_boost_factor[operand][mem_level]
+                    data_each_level_unrolled[operand][mem_level] * mem_bw_boost_factor[operand][mem_level]
                 )
                 wr_in_by_low_da = 0
                 rd_out_to_high_da = 0
                 wr_in_by_high_da = data_each_level_unrolled[operand][mem_level + 1]
 
-                self.unit_mem_data_movement[operand][
-                    mem_level
-                ].set_data_trans_amount_per_period(
+                self.unit_mem_data_movement[operand][mem_level].set_data_trans_amount_per_period(
                     rd_out_to_low_da,
                     wr_in_by_low_da,
                     rd_out_to_high_da,
                     wr_in_by_high_da,
                 )
 
-        # For output operand 
+        # For output operand
         output_operand = self.layer_node.output_operand
         for mem_level in range(self.mem_level[output_operand]):
             wr_in_by_low_bw = req_mem_bw_H_raw[output_operand][mem_level]
             rd_out_to_high_bw = req_mem_bw_L_raw[output_operand][mem_level + 1]
             wr_in_by_low_pd = cycle_each_level[output_operand][mem_level]
             rd_out_to_high_pd = cycle_each_level[output_operand][mem_level + 1]
-            wr_in_by_low_pc = (
-                self.temporal_mapping.total_cycle
-                // cycle_each_level[output_operand][mem_level]
-            )
-            rd_out_to_high_pc = (
-                self.temporal_mapping.total_cycle
-                // cycle_each_level[output_operand][mem_level + 1]
-            )
+            wr_in_by_low_pc = self.temporal_mapping.total_cycle // cycle_each_level[output_operand][mem_level]
+            rd_out_to_high_pc = self.temporal_mapping.total_cycle // cycle_each_level[output_operand][mem_level + 1]
             wr_in_by_low_da = (
-                data_each_level_unrolled[output_operand][mem_level]
-                * mem_bw_boost_factor[output_operand][mem_level]
+                data_each_level_unrolled[output_operand][mem_level] * mem_bw_boost_factor[output_operand][mem_level]
             )
             rd_out_to_high_da = data_each_level_unrolled[output_operand][mem_level + 1]
 
             if self.psum_flag[mem_level]:
                 rd_out_to_low_bw = wr_in_by_low_bw
                 rd_out_to_low_pd = wr_in_by_low_pd
                 rd_out_to_low_pc = wr_in_by_low_pc
@@ -828,87 +580,57 @@
                 wr_in_by_high_da = 0
 
             # average required memory BW
             self.unit_mem_data_movement[output_operand][mem_level].set_req_mem_bw_aver(
                 rd_out_to_low_bw, wr_in_by_low_bw, rd_out_to_high_bw, wr_in_by_high_bw
             )
             # data transfer period
-            self.unit_mem_data_movement[output_operand][
-                mem_level
-            ].set_data_trans_period(
+            self.unit_mem_data_movement[output_operand][mem_level].set_data_trans_period(
                 rd_out_to_low_pd, wr_in_by_low_pd, rd_out_to_high_pd, wr_in_by_high_pd
             )
             # data transfer period count
-            self.unit_mem_data_movement[output_operand][
-                mem_level
-            ].set_data_trans_period_count(
+            self.unit_mem_data_movement[output_operand][mem_level].set_data_trans_period_count(
                 rd_out_to_low_pc, wr_in_by_low_pc, rd_out_to_high_pc, wr_in_by_high_pc
             )
             # per-period data transfer amount
-            self.unit_mem_data_movement[output_operand][
-                mem_level
-            ].set_data_trans_amount_per_period(
+            self.unit_mem_data_movement[output_operand][mem_level].set_data_trans_amount_per_period(
                 rd_out_to_low_da, wr_in_by_low_da, rd_out_to_high_da, wr_in_by_high_da
             )
 
         # Calculate the instant memory updating behavior.
         top_ir_loop_size = self.temporal_mapping.top_ir_loop_size
         for operand in self.operand_list:
-            for level, data_movement_item in enumerate(
-                self.unit_mem_data_movement[operand]
-            ):
+            for level, data_movement_item in enumerate(self.unit_mem_data_movement[operand]):
                 req_mem_bw_aver = data_movement_item.req_mem_bw_aver
                 # calculate "instant required memory BW" based on "average required memory BW"
-                rd_out_to_low_bw = (
-                    req_mem_bw_aver.rd_out_to_low * top_ir_loop_size[operand][level]
-                )
-                wr_in_by_low_bw = (
-                    req_mem_bw_aver.wr_in_by_low * top_ir_loop_size[operand][level]
-                )
-                rd_out_to_high_bw = (
-                    req_mem_bw_aver.rd_out_to_high
-                    * top_ir_loop_size[operand][level + 1]
-                )
-                wr_in_by_high_bw = (
-                    req_mem_bw_aver.wr_in_by_high * top_ir_loop_size[operand][level + 1]
-                )
+                rd_out_to_low_bw = req_mem_bw_aver.rd_out_to_low * top_ir_loop_size[operand][level]
+                wr_in_by_low_bw = req_mem_bw_aver.wr_in_by_low * top_ir_loop_size[operand][level]
+                rd_out_to_high_bw = req_mem_bw_aver.rd_out_to_high * top_ir_loop_size[operand][level + 1]
+                wr_in_by_high_bw = req_mem_bw_aver.wr_in_by_high * top_ir_loop_size[operand][level + 1]
                 data_movement_item.set_req_mem_bw_inst(
                     rd_out_to_low_bw,
                     wr_in_by_low_bw,
                     rd_out_to_high_bw,
                     wr_in_by_high_bw,
                 )
 
                 data_trans_period = data_movement_item.data_trans_period
                 # calculate "instant data transferring window", assuming non-double buffered memory
-                rd_out_to_low_wd = (
-                    data_trans_period.rd_out_to_low // top_ir_loop_size[operand][level]
-                )
-                wr_in_by_low_wd = (
-                    data_trans_period.wr_in_by_low // top_ir_loop_size[operand][level]
-                )
-                rd_out_to_high_wd = (
-                    data_trans_period.rd_out_to_high
-                    // top_ir_loop_size[operand][level + 1]
-                )
-                wr_in_by_high_wd = (
-                    data_trans_period.wr_in_by_high
-                    // top_ir_loop_size[operand][level + 1]
-                )
+                rd_out_to_low_wd = data_trans_period.rd_out_to_low // top_ir_loop_size[operand][level]
+                wr_in_by_low_wd = data_trans_period.wr_in_by_low // top_ir_loop_size[operand][level]
+                rd_out_to_high_wd = data_trans_period.rd_out_to_high // top_ir_loop_size[operand][level + 1]
+                wr_in_by_high_wd = data_trans_period.wr_in_by_high // top_ir_loop_size[operand][level + 1]
                 data_movement_item.set_inst_data_trans_window(
                     rd_out_to_low_wd,
                     wr_in_by_low_wd,
                     rd_out_to_high_wd,
                     wr_in_by_high_wd,
                 )
 
-    ## This function set all the data traffic between the top level memory and the external world to 0
-    # in unit_mem_data_movement.
     def disable_data_traffic_external(self):
+        """! This function set all the data traffic between the top level memory and the external world to 0
+        in unit_mem_data_movement.
+        """
         for operand in self.operand_list:
             mem_level = self.mem_level[operand] - 1
-            self.unit_mem_data_movement[operand][mem_level].update_single_dir_data(
-                "rd_out_to_high", 0
-            )
-            self.unit_mem_data_movement[operand][mem_level].update_single_dir_data(
-                "wr_in_by_high", 0
-            )
+            self.unit_mem_data_movement[operand][mem_level].update_single_dir_data(DataDirection.RD_OUT_TO_HIGH, 0)
+            self.unit_mem_data_movement[operand][mem_level].update_single_dir_data(DataDirection.WR_IN_BY_HIGH, 0)
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/mapping/mapping_assist_funcs.py` & `zigzag_dse-3.1.1/zigzag/mapping/mapping_assist_funcs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,128 +1,94 @@
-from typing import Dict, List
-from typing import TYPE_CHECKING
+from typing import TypeAlias
 from math import prod
-from copy import deepcopy
 
+from zigzag.datatypes import LayerOperand, PrLoop, UnrollFactor, LayerDim
+from zigzag.workload.layer_attributes import LayerDimSizes
 from zigzag.utils import pickle_deepcopy
+from zigzag.workload.layer_node import LayerNode
 
-if TYPE_CHECKING:
-    from zigzag.classes.workload.layer_node import LayerNode
+SpatialMappingPerMemLvl: TypeAlias = dict[LayerOperand, list[list[tuple[LayerDim, UnrollFactor | float]]]]
 
-## Collect information of each single loop tuple in mapping.
-# Applied range: from the lowest architectural level to the current level.
-class Loop:
-
-    ## The class constructor
-    # @param loop
-    # @param MAC_op
-    # @param data_elem
-    def __init__(self, loop: tuple, MAC_op: int, data_elem: int):
-        self.loop = loop
-        self.MAC_op = MAC_op
-        self.data_elem = data_elem
-        self.reuse = MAC_op / data_elem
-
-    def __str__(self):
-        return str(self.loop)
-
-    def __repr__(self):
-        return str(self.loop)
-
-## This function decouples the pr loops into data size (r loops) and data reuse (ir loops).
-# It also provides a transferred mapping dictionary in which the pr loops are replaced by r and ir loops.
-def decouple_pr_loop(mapping_dict: Dict, layer_node: "LayerNode"):
 
-    operand_loop_dim = {
-        op: layer_node.operand_loop_dim[op] for op in mapping_dict.keys()
-    }
-    r_ir_operand_loop_LUT = {
-        op: relevance["r"] + relevance["ir"]
-        for (op, relevance) in operand_loop_dim.items()
+def decouple_pr_loop(mapping_dict: SpatialMappingPerMemLvl, layer_node: "LayerNode") -> SpatialMappingPerMemLvl:
+    """! This function decouples the pr loops into data size (r loops) and data reuse (ir loops).
+    It also provides a transferred mapping dictionary in which the pr loops are replaced by r and ir loops.
+    # TODO cleanup
+    """
+
+    relevancy_info = layer_node.loop_relevancy_info
+    r_ir_operand_loop_lut: dict[LayerOperand, list[LayerDim]] = {
+        layer_op: relevancy_info.get_r_layer_dims(layer_op) + relevancy_info.get_ir_layer_dims(layer_op)
+        for layer_op in layer_node.layer_operands
     }
-    pr_operand_loop_LUT = {
-        op: relevance["pr"]
-        for (op, relevance) in operand_loop_dim.items()
-        if relevance["pr"] != {}
+    pr_operand_loop_lut: dict[LayerOperand, PrLoop] = {
+        layer_op: relevancy_info.get_pr_layer_dims(layer_op)
+        for layer_op in layer_node.layer_operands
+        if len(relevancy_info.get_pr_layer_dims(layer_op)) > 0
     }
-    pr_operand_list = list(pr_operand_loop_LUT.keys())
-    mapping_dict_reform = pickle_deepcopy(mapping_dict)
+
+    pr_operand_list = list(pr_operand_loop_lut.keys())
+    mapping_dict_reform: SpatialMappingPerMemLvl = pickle_deepcopy(mapping_dict)
 
     # current and below level pr data size
-    cabl_pr_data_size = {}
+    cabl_pr_data_size: dict[LayerOperand, dict[LayerDim, list[list[float]]]] = {}
     # current and below level pr data reuse
-    cabl_pr_data_reuse = {}
+    cabl_pr_data_reuse: dict[LayerOperand, dict[LayerDim, list[list[float]]]] = dict()
 
     # each single pr loop data size
-    per_pr_data_size = {}
+    per_pr_data_size: dict[LayerOperand, dict[LayerDim, list[list[float]]]] = dict()
     # each single pr loop data reuse
-    per_pr_data_reuse = {}
+    per_pr_data_reuse: dict[LayerOperand, dict[LayerDim, list[list[float]]]] = dict()
 
     for operand in pr_operand_list:
 
         # initialize current and below level pr loop size
-        cabl_pr_lp_size = {
-            pr_data_dim: {
-                pr_loop_dim: 1
-                for pr_loop_dim in pr_operand_loop_LUT[operand][pr_data_dim]
-            }
-            for pr_data_dim in pr_operand_loop_LUT[operand].keys()
+        cabl_pr_lp_size: dict[LayerDim, dict[LayerDim, UnrollFactor]] = {
+            pr_data_dim: {pr_loop_dim: 1 for pr_loop_dim in pr_operand_loop_lut[operand][pr_data_dim]}
+            for pr_data_dim in pr_operand_loop_lut[operand]
         }
 
         # initialize current and below level pr data size
         cabl_pr_data_size[operand] = {
-            pr_data_dim: [[] for _ in range(len(mapping_dict[operand]))]
-            for pr_data_dim in pr_operand_loop_LUT[operand].keys()
+            pr_data_dim: [[] for _ in range(len(mapping_dict[operand]))] for pr_data_dim in pr_operand_loop_lut[operand]
         }
 
         # initialize current and below level pr data reuse
         cabl_pr_data_reuse[operand] = {
-            pr_data_dim: [[] for _ in range(len(mapping_dict[operand]))]
-            for pr_data_dim in pr_operand_loop_LUT[operand].keys()
+            pr_data_dim: [[] for _ in range(len(mapping_dict[operand]))] for pr_data_dim in pr_operand_loop_lut[operand]
         }
 
         # initialize per pr loop data size
         per_pr_data_size[operand] = {
-            pr_data_dim: [[] for _ in range(len(mapping_dict[operand]))]
-            for pr_data_dim in pr_operand_loop_LUT[operand].keys()
+            pr_data_dim: [[] for _ in range(len(mapping_dict[operand]))] for pr_data_dim in pr_operand_loop_lut[operand]
         }
 
         # initialize per pr loop data reuse
         per_pr_data_reuse[operand] = {
             pr_data_dim: [[] for _ in range(len(mapping_dict[operand]))]
-            for pr_data_dim in pr_operand_loop_LUT[operand].keys()
+            for pr_data_dim in pr_operand_loop_lut[operand].keys()
         }
 
         # update the cabl_pr_lp_size by multiply pr loop size across architectural level
         for level, loop_list in enumerate(mapping_dict[operand]):
             for loop_type, loop_size in loop_list:
-                if loop_type in r_ir_operand_loop_LUT[operand]:
+                if loop_type in r_ir_operand_loop_lut[operand]:
                     continue
-                for pr_data_dim in pr_operand_loop_LUT[operand].keys():
-                    if any(
-                        lp_type == loop_type
-                        for lp_type in pr_operand_loop_LUT[operand][pr_data_dim]
-                    ):
+                for pr_data_dim in pr_operand_loop_lut[operand].keys():
+                    if any(lp_type == loop_type for lp_type in pr_operand_loop_lut[operand][pr_data_dim]):
                         cabl_pr_lp_size[pr_data_dim][loop_type] *= loop_size
 
                         # compute pr related data dimension size and data dimension reuse at current and below joint levels
                         # based on pr_funcs (dynamic functions extracted in LayerNode). Each pr loop is decoupled into r and ir loops.
                         pr_loop_combined_to_r = layer_node.calc_tensor_dim(
-                            cabl_pr_lp_size[pr_data_dim], pr_data_dim
-                        )
-                        pr_loop_combined_to_ir = (
-                            prod(cabl_pr_lp_size[pr_data_dim].values())
-                            / pr_loop_combined_to_r
-                        )
-                        cabl_pr_data_size[operand][pr_data_dim][level].append(
-                            pr_loop_combined_to_r
-                        )
-                        cabl_pr_data_reuse[operand][pr_data_dim][level].append(
-                            pr_loop_combined_to_ir
+                            pr_data_dim, LayerDimSizes(cabl_pr_lp_size[pr_data_dim])
                         )
+                        pr_loop_combined_to_ir = prod(cabl_pr_lp_size[pr_data_dim].values()) / pr_loop_combined_to_r
+                        cabl_pr_data_size[operand][pr_data_dim][level].append(pr_loop_combined_to_r)
+                        cabl_pr_data_reuse[operand][pr_data_dim][level].append(pr_loop_combined_to_ir)
 
         # compute pr related data dimension size and data dimension reuse at each level for each pr loop
         # based on cabl_pr_data_size/cabl_pr_data_reuse """
         for pr_data_dim in cabl_pr_data_size[operand].keys():
             data_size_list = cabl_pr_data_size[operand][pr_data_dim]
             data_reuse_list = cabl_pr_data_reuse[operand][pr_data_dim]
             previous_data_size = 1
@@ -138,84 +104,57 @@
                     previous_data_size = data_size_list[level][idx]
                     previous_data_data_reuse = data_reuse_list[level][idx]
 
         mapping_dict_reform[operand] = replace_pr_loop_in_mapping(
             mapping_dict[operand],
             per_pr_data_size[operand],
             per_pr_data_reuse[operand],
-            pr_operand_loop_LUT[operand],
-            r_ir_operand_loop_LUT[operand],
+            pr_operand_loop_lut[operand],
+            r_ir_operand_loop_lut[operand],
         )
 
-    # return mapping_dict_reform, cabl_pr_data_size, cabl_pr_data_reuse, per_pr_data_size, per_pr_data_reuse
     return mapping_dict_reform
 
-## This function replaces all pr loops in a mapping of a single operand with r and ir loops.
-# @param single_operand_mapping
-# @param per_pr_data_size
-# @param per_pr_data_reuse
-# @param pr_operand_loop_LUT
-# @param r_ir_operand_loop_LUT
+
 def replace_pr_loop_in_mapping(
-    single_operand_mapping: Dict,
-    per_pr_data_size: Dict,
-    per_pr_data_reuse: Dict,
-    pr_operand_loop_LUT: Dict,
-    r_ir_operand_loop_LUT: List,
-):
-    mapping_new = pickle_deepcopy(single_operand_mapping)
+    single_operand_mapping: list[list[tuple[LayerDim, UnrollFactor]]],
+    per_pr_data_size: dict[LayerDim, list[list[float]]],
+    per_pr_data_reuse: dict[LayerDim, list[list[float]]],
+    pr_operand_loop_lut: PrLoop,
+    r_ir_operand_loop_lut: list[LayerDim],
+) -> list[list[tuple[LayerDim, UnrollFactor]]]:
+    """! This function replaces all pr loops in a mapping of a single operand with r and ir loops."""
+    mapping_new: list[list[tuple[LayerDim, UnrollFactor]]] = pickle_deepcopy(single_operand_mapping)
 
     for level, loop_list in enumerate(single_operand_mapping):
         # Introduce the current level pr loop index to distinguish different pr loops at the same architectural level
-        cl_pr_lp_idx_local = {
-            pr_data_dim: 0 for pr_data_dim in pr_operand_loop_LUT.keys()
-        }
+        cl_pr_lp_idx_local = {pr_data_dim: 0 for pr_data_dim in pr_operand_loop_lut.keys()}
         cl_pr_lp_idx_global = 0
-        for idx, (loop_type, loop_size) in enumerate(loop_list):
-            if loop_type in r_ir_operand_loop_LUT:
+        for idx, (loop_type, _) in enumerate(loop_list):
+            if loop_type in r_ir_operand_loop_lut:
                 continue
-            for pr_data_dim in pr_operand_loop_LUT.keys():
-                if any(
-                    lp_type == loop_type for lp_type in pr_operand_loop_LUT[pr_data_dim]
-                ):
+            for pr_data_dim in pr_operand_loop_lut.keys():
+                if any(lp_type == loop_type for lp_type in pr_operand_loop_lut[pr_data_dim]):
                     # replace the pr loop in the mapping by r loop
                     pr_idx_local = cl_pr_lp_idx_local[pr_data_dim]
                     pr_idx_global = cl_pr_lp_idx_global
                     mapping_new[level][idx + pr_idx_global] = (
-                        pr_data_dim + "_r",
+                        pr_data_dim.create_r_version(),
                         per_pr_data_size[pr_data_dim][level][pr_idx_local],
                     )
-                    # insert ir loop after the r loop 
-                    # NOTE: Here we insert the ir loop after/above the r loop, which indicates that we ignore the input FIFO effect
-                    # during current level feeds data to below level. We could also insert the ir loop before/below the r loop,
-                    # which leads to more energy-efficient mapping if the innermost ir loop merging down is enabled.
+                    # insert ir loop after the r loop
+                    # NOTE: Here we insert the ir loop after/above the r loop, which indicates that we ignore the input
+                    # FIFO effect during current level feeds data to below level. We could also insert the ir loop
+                    # before/below the r loop, which leads to more energy-efficient mapping if the innermost ir loop
+                    # merging down is enabled.
                     mapping_new[level].insert(
                         idx + pr_idx_global + 1,
                         (
-                            pr_data_dim + "_ir",
+                            pr_data_dim.create_ir_version(),
                             per_pr_data_reuse[pr_data_dim][level][pr_idx_local],
                         ),
                     )
                     # update the pr loop index
                     cl_pr_lp_idx_local[pr_data_dim] += 1
                     cl_pr_lp_idx_global += 1
 
     return mapping_new
-
-
-# This function generates detailed information for each single loop item for each operand.
-def calc_data_size_MAC_count_per_loop(
-    mapping_dict_reform: Dict, operand_loop_dim_reform: Dict
-):
-    detailed_mapping_dict = deepcopy(mapping_dict_reform)
-    for operand, mapping_list in mapping_dict_reform.items():
-        MAC_count = 1
-        data_elem = 1
-        for level, loop_list in enumerate(mapping_dict_reform[operand]):
-            for idx, (loop_type, loop_size) in enumerate(loop_list):
-                MAC_count *= loop_size
-                if loop_type in operand_loop_dim_reform[operand]["r"]:
-                    data_elem *= loop_size
-                detailed_mapping_dict[operand][level][idx] = Loop(
-                    (loop_type, loop_size), round(MAC_count), round(data_elem)
-                )
-    return detailed_mapping_dict
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/mapping/spatial/spatial_mapping.py` & `zigzag_dse-3.1.1/zigzag/mapping/SpatialMappingInternal.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-from typing import Dict
 from math import prod
-from typing import TYPE_CHECKING
 
-if TYPE_CHECKING:
-    from zigzag.classes.workload.layer_node import LayerNode
-import zigzag.classes.mapping.mapping_assist_funcs as mapping_assist_funcs
-
-## Class that collect all the info related to spatial mapping.
-class SpatialMapping:
-
-    ## The class constructor
-    # @param spatial_mapping_dict
-    # @param layer_node
-    def __init__(self, spatial_mapping_dict: Dict, layer_node: "LayerNode"):
+
+from zigzag.datatypes import LayerDim, LayerOperand, UnrollFactor
+from zigzag.workload.layer_node import LayerNode
+from zigzag.mapping.mapping_assist_funcs import SpatialMappingPerMemLvl, decouple_pr_loop
+from zigzag.utils import json_repr_handler
+
+
+class SpatialMappingInternal:
+    """! Class that collect all the info related to spatial mapping."""
+
+    def __init__(self, spatial_mapping_dict: SpatialMappingPerMemLvl, layer_node: "LayerNode"):
+
         self.mapping_dict_origin = spatial_mapping_dict
-        self.mapping_dict_reform = mapping_assist_funcs.decouple_pr_loop(
-            spatial_mapping_dict, layer_node
-        )
+        self.mapping_dict_reform: SpatialMappingPerMemLvl = decouple_pr_loop(spatial_mapping_dict, layer_node)
         self.layer_node = layer_node
-        self.operand_list = layer_node.operand_list
+        self.layer_operands: list[LayerOperand] = layer_node.layer_operands
 
         # Extract architecture level count for each operand from spatial mapping definition, starting from MAC level
-        self.arch_level = {op: len(smap) for (op, smap) in spatial_mapping_dict.items()}
+        self.arch_level = {op: len(smap) for op, smap in spatial_mapping_dict.items()}
 
         # Calculate unrolled loop size for different loop types (r/ir/total)
         self.calc_unroll_size()
 
         # Calculate total/unique/duplicate unit count
         self.calc_unit_count()
 
         # Calculate data serve scope: each data element serves/(is served by) how many unit at below level
-        # NOTE: data_serve_scope doesn't include MAC level, thus is one level less than other spatial mapping attributes.
+        # NOTE: data_serve_scope doesn't include MAC level, thus is one level less than other spatial mapping
+        # attributes.
         self.calc_data_serve_scope()
 
         # Calculate memory bandwidth incremental factor between architectural levels
         # mem_bw_boost_factor doesn't include MAC level, thus is one level less than other spatial mapping attributes.
         self.calc_mem_bw_boost_factor()
 
         # Added for loma: Get list of the spatially unrolled loops, without any information about arch levels
@@ -42,150 +40,137 @@
 
     def __str__(self):
         return f"SpatialMapping({self.mapping_dict_origin})"
 
     def __repr__(self):
         return str(self)
 
-    ## JSON representation of this object to save it to a file.
     def __jsonrepr__(self):
-        return {"spatial_mapping": self.mapping_dict_origin}
+        """! JSON representation of this object to save it to a file."""
+        return json_repr_handler({"spatial_mapping": self.mapping_dict_origin})
 
-    ## Return the unrolled loops for operand 'op' at level 'level'.
-    # 'level' = 0 would signify the operational level.
-    # @param op
-    # @param level
-    def get_unrolling(self, op: str, level: int):
+    def get_unrolling(self, op: LayerOperand, level: int):
+        """! Return the unrolled loops for operand 'op' at level 'level'.
+        'level' = 0 would signify the operational level.
+        """
         return self.mapping_dict_origin[op][level]
 
-    def get_unrolling_all(self, op: str, min_level: int) -> list:
+    def get_unrolling_all(self, op: LayerOperand, min_level: int) -> list[tuple[LayerDim, UnrollFactor]]:
         """Return all the spatial loops at a given level and above for a given operand.
 
         Args:
             op (str): The layer operand for which to return the spatial loops.
             min_level (int): The lowest level.
 
         Returns:
             list: A list of all spatial loops at given level and above.
+        # TODO this has the same functionality as SpatialMapping.flatten_unrollings()
         """
-        spatial_loops = []
+        spatial_loops: list[tuple[LayerDim, UnrollFactor]] = []
         for level in range(min_level, self.arch_level[op]):
             spatial_loops += self.get_unrolling(op, level)
         return spatial_loops
 
-    ## Calculate unrolled loop size for different loop types (r/ir/total) per operand per architecture level
-    def calc_unroll_size(self):
+    def calc_unroll_size(self) -> None:
+        """! Calculate unrolled loop size for different loop types (r/ir/total) per operand per architecture level"""
 
         # Initialization
-        unroll_size_r = {op: [1] * arch_lv for (op, arch_lv) in self.arch_level.items()}
-        unroll_size_ir = {
-            op: [1] * arch_lv for (op, arch_lv) in self.arch_level.items()
+        unroll_size_r: dict[LayerOperand, list[UnrollFactor]] = {
+            op: [1] * arch_lv for op, arch_lv in self.arch_level.items()
         }
-        unroll_size_total = {
-            op: [1] * arch_lv for (op, arch_lv) in self.arch_level.items()
+        unroll_size_ir: dict[LayerOperand, list[UnrollFactor]] = {
+            op: [1] * arch_lv for op, arch_lv in self.arch_level.items()
+        }
+        unroll_size_total: dict[LayerOperand, list[UnrollFactor]] = {
+            op: [1] * arch_lv for op, arch_lv in self.arch_level.items()
         }
 
         # Go through the reformed spatial mapping and extract the unroll size
-        for operand in self.operand_list:
-            for level, current_level_loops in enumerate(
-                self.mapping_dict_reform[operand]
-            ):
-                for loop_type, loop_dim in current_level_loops:
-                    if (
-                        loop_type
-                        in self.layer_node.operand_loop_dim_reform[operand]["r"]
-                    ):
-                        unroll_size_r[operand][level] *= loop_dim
+        for layer_op in self.layer_operands:
+            for level, current_level_loops in enumerate(self.mapping_dict_reform[layer_op]):
+                for layer_dim, loop_dim in current_level_loops:
+                    # TODO use pr_decoupled_relevancy_info
+                    if layer_dim in self.layer_node.pr_decoupled_relevancy_info.get_r_layer_dims(layer_op):
+                        unroll_size_r[layer_op][level] *= loop_dim
                     else:
-                        unroll_size_ir[operand][level] *= loop_dim
-                    unroll_size_total[operand][level] *= loop_dim
+                        unroll_size_ir[layer_op][level] *= loop_dim
+                    unroll_size_total[layer_op][level] *= loop_dim
 
         self.unroll_size_r = unroll_size_r
         self.unroll_size_ir = unroll_size_ir
         self.unroll_size_total = unroll_size_total
 
-    ## Calculate total/unique/duplicate unit count per operand per architecture level
     def calc_unit_count(self):
+        """! Calculate total/unique/duplicate unit count per operand per architecture level"""
         # Number of unit at each level (for each operand)
         # Added round call as number doesn't remain integer due to self.mapping_dict_reform number instability
         unit_count = {
             op: [
-                round(
-                    round(prod(self.unroll_size_total[op][lv : self.arch_level[op]]), 3)
-                )
+                round(round(prod(self.unroll_size_total[op][lv : self.arch_level[op]]), 3))
                 for lv in range(self.arch_level[op])
             ]
-            for op in self.operand_list
+            for op in self.layer_operands
         }
 
-        """ ASSERT: The bottom level (MAC level) unit count must be the same for all operand """
+        #  ASSERT: The bottom level (MAC level) unit count must be the same for all operand
         bottom_unit_count = [unit_count[op][0] for op in unit_count.keys()]
         assert all(
             x == bottom_unit_count[0] for x in bottom_unit_count
         ), f"The MAC level unit count is not the same for all operand {bottom_unit_count}, please correct the spatial mapping."
 
-        """ Number of unit at each level that hold unique data (for each operand) """
+        #  Number of unit at each level that hold unique data (for each operand)
         unit_unique = {
-            op: [
-                prod(self.unroll_size_r[op][lv : self.arch_level[op]])
-                for lv in range(self.arch_level[op])
-            ]
-            for op in self.operand_list
+            op: [prod(self.unroll_size_r[op][lv : self.arch_level[op]]) for lv in range(self.arch_level[op])]
+            for op in self.layer_operands
         }
 
-        """ Number of unit at each level that hold the same data (for each operand) """
+        #  Number of unit at each level that hold the same data (for each operand)
         unit_duplicate = {
-            op: [
-                prod(self.unroll_size_ir[op][lv : self.arch_level[op]])
-                for lv in range(self.arch_level[op])
-            ]
-            for op in self.operand_list
+            op: [prod(self.unroll_size_ir[op][lv : self.arch_level[op]]) for lv in range(self.arch_level[op])]
+            for op in self.layer_operands
         }
 
         self.unit_count = unit_count
         self.unit_unique = unit_unique
         self.unit_duplicate = unit_duplicate
 
-    ## Calculate data serve scope, i.e., for input operands, it means that each data element
-    # is broadcast to how many unit at below level; for output operand, it means that how
-    # many unit add/collect their output values to one result, and push it to above level
-    #
-    # NOTE: data_serve_scope doesn't include MAC level, thus is one level less than other spatial mapping attributes.
-    #
-    # data_serve_scope is calculated by dividing unit_duplicate at current level by unit_count at one level above.
     def calc_data_serve_scope(self):
+        """! Calculate data serve scope, i.e., for input operands, it means that each data element
+        is broadcast to how many unit at below level; for output operand, it means that how
+        many unit add/collect their output values to one result, and push it to above level
+
+        NOTE: data_serve_scope doesn't include MAC level, thus is one level less than other spatial mapping attributes.
+
+        data_serve_scope is calculated by dividing unit_duplicate at current level by unit_count at one level above.
+        """
         data_serve_scope = {
-            op: [
-                self.unit_duplicate[op][lv] / self.unit_duplicate[op][lv + 1]
-                for lv in range(self.arch_level[op] - 1)
-            ]
-            for op in self.operand_list
+            op: [self.unit_duplicate[op][lv] / self.unit_duplicate[op][lv + 1] for lv in range(self.arch_level[op] - 1)]
+            for op in self.layer_operands
         }
 
         self.data_serve_scope = data_serve_scope
 
-    ## Calculate memory bandwidth incremental factor between architectural levels.
-    #
-    # NOTE: mem_bw_boost doesn't include MAC level, thus is one level less than other spatial mapping attributes.
-    #
-    # mem_bw_boost can calculated by either dividing unit_unique at current level by unit_count at one level above.
     def calc_mem_bw_boost_factor(self):
+        """! Calculate memory bandwidth incremental factor between architectural levels.
+
+        NOTE: mem_bw_boost doesn't include MAC level, thus is one level less than other spatial mapping attributes.
+
+        mem_bw_boost can calculated by either dividing unit_unique at current level by unit_count at one level above.
+        """
         mem_bw_boost = {
             op: [
-                round(self.unit_unique[op][lv] / self.unit_unique[op][lv + 1])
-                for lv in range(self.arch_level[op] - 1)
+                round(self.unit_unique[op][lv] / self.unit_unique[op][lv + 1]) for lv in range(self.arch_level[op] - 1)
             ]
-            for op in self.operand_list
+            for op in self.layer_operands
         }
 
         self.mem_bw_boost = mem_bw_boost
 
-    # Save the loops that were unrolled spatially in a list without any arch level information for easy access in loma.
-    def save_spatial_loop_dim_size(self):
-        # We take one of the input operands and go through the spatial mapping dict for that operand.
-        # Which operand shouldn't matter as all operands store the same loops, but possibly at different arch levels.
+    def save_spatial_loop_dim_size(self) -> None:
+        """! Save the loops that were unrolled spatially in a list without any arch level information for easy access in loma.
+        We take one of the input operands and go through the spatial mapping dict for that operand.
+        Which operand shouldn't matter as all operands store the same loops, but possibly at different arch levels."""
+
         op = self.layer_node.input_operands[0]
-        self.spatial_loop_dim_size = [
-            loop
-            for spatial_loops in self.mapping_dict_origin[op]
-            for loop in spatial_loops
+        self.spatial_loop_dim_size: list[tuple[LayerDim, UnrollFactor]] = [
+            loop for spatial_loops in self.mapping_dict_origin[op] for loop in spatial_loops
         ]
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/mapping/temporal/temporal_mapping.py` & `zigzag_dse-3.1.1/zigzag/mapping/TemporalMapping.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,124 +1,101 @@
-from typing import Dict
-from math import prod
-from zigzag.classes.workload.layer_node import LayerNode
-from zigzag.utils import pickle_deepcopy
+from typing import TypeAlias
+import math
+
+from zigzag.datatypes import LayerDim, LayerOperand, UnrollFactor
+from zigzag.workload.layer_node import LayerNode
+from zigzag.utils import json_repr_handler, pickle_deepcopy
+
+TemporalMappingDict: TypeAlias = dict[LayerOperand, list[list[tuple[LayerDim, UnrollFactor]]]]
+
 
-## Class that collect all the info related to temporal mapping.
 class TemporalMapping:
+    """! Class that collect all the info related to temporal mapping."""
 
-    ## The class constructor
-    # @param temporal_mapping_dict
-    # @param layer_node
-    def __init__(self, temporal_mapping_dict: Dict, layer_node: LayerNode):
+    def __init__(self, temporal_mapping_dict: TemporalMappingDict, layer_node: LayerNode):
         self.mapping_dic_origin = temporal_mapping_dict
         self.layer_node = layer_node
-        self.operand_list = layer_node.operand_list
+        self.operand_list = layer_node.layer_operands
 
         # Extract memory hierarchy level count for each operand from temporal mapping definition
         self.mem_level = {op: len(tmap) for (op, tmap) in temporal_mapping_dict.items()}
 
         # For each memory level, if the innermost/bottom loop is ir loop, merge it down to the below level
         self.innermost_stationary_loop_merge_down()
 
-        # Calculate the current and below level (cabl) iteration cycle for each memory level, 
+        # Calculate the current and below level (cabl) iteration cycle for each memory level,
         # i.e., each memory level refreshes once, how many cycles it covers
         self.calc_cycle_cabl_level()
 
-        # Calculate the current and below loop (cabl) iteration cycle for each loop,
-        # i.e., each loop iterates once, how many cycles it covers '''
-        # self.calc_cycle_cabl_loop()
-
-        # Calculate the top-ir loop size at each memory level, which will be used 
+        # Calculate the top-ir loop size at each memory level, which will be used
         # to compute instant required memory BW in combined_mapping.py """
         self.calc_top_r_and_ir_loop()
 
     def __str__(self):
         return str(self.mapping_dic_stationary)
 
     def __repr__(self):
         return str(self)
 
-    ## JSON representation of this object to save it to a json file.
     def __jsonrepr__(self):
-        return {"temporal_mapping": self.mapping_dic_stationary}
+        """! JSON representation of this object to save it to a json file."""
+        return json_repr_handler({"temporal_mapping": self.mapping_dic_stationary})
 
-    ## Iteratively merging down the ir loops which located at the bottom position of each memory level.
-    # Also calculate the MAC level data stationary cycle, i,e., the innermost memory level's bottom ir loops.
     def innermost_stationary_loop_merge_down(self):
+        """! Iteratively merging down the ir loops which located at the bottom position of each memory level.
+        Also calculate the MAC level data stationary cycle, i,e., the innermost memory level's bottom ir loops.
+        """
         # Initialization
-        mapping_current = pickle_deepcopy(self.mapping_dic_origin)
-        mapping_previous = pickle_deepcopy(self.mapping_dic_origin)
+        mapping_current: TemporalMappingDict = pickle_deepcopy(self.mapping_dic_origin)
+        mapping_previous: TemporalMappingDict = pickle_deepcopy(self.mapping_dic_origin)
         done = False
 
         while not done:
-            mapping_st = {
-                op: [[] for _ in range(self.mem_level[op])] for op in self.operand_list
-            }
-            MAC_level_st = {op: 1 for op in self.operand_list}
+            mapping_st: TemporalMappingDict = {op: [[] for _ in range(self.mem_level[op])] for op in self.operand_list}
+            MAC_level_st: dict[LayerOperand, UnrollFactor] = {op: 1 for op in self.operand_list}
             for operand in self.mem_level.keys():
                 for level, current_level_loops in enumerate(mapping_previous[operand]):
                     if not current_level_loops:
-                        mapping_st[operand][level] = pickle_deepcopy(
-                            current_level_loops
-                        )
+                        mapping_st[operand][level] = pickle_deepcopy(current_level_loops)
                     else:
                         for loop_type, loop_dim in current_level_loops:
-                            if (
-                                loop_type
-                                in self.layer_node.operand_loop_dim[operand]["ir"]
-                            ):
+                            if loop_type in self.layer_node.loop_relevancy_info.get_ir_layer_dims(operand):
                                 if level == 0:
                                     MAC_level_st[operand] *= loop_dim
-                                    mapping_st[operand][level].append(
-                                        (loop_type, loop_dim)
-                                    )
-                                    mapping_current[operand][level].remove(
-                                        (loop_type, loop_dim)
-                                    )
+                                    mapping_st[operand][level].append((loop_type, loop_dim))
+                                    mapping_current[operand][level].remove((loop_type, loop_dim))
                                 else:
-                                    mapping_st[operand][level - 1].append(
-                                        (loop_type, loop_dim)
-                                    )
-                                    mapping_current[operand][level].remove(
-                                        (loop_type, loop_dim)
-                                    )
+                                    mapping_st[operand][level - 1].append((loop_type, loop_dim))
+                                    mapping_current[operand][level].remove((loop_type, loop_dim))
                             else:
-                                mapping_st[operand][level].extend(
-                                    mapping_current[operand][level]
-                                )
+                                mapping_st[operand][level].extend(mapping_current[operand][level])
                                 break
             if mapping_st != mapping_previous:
                 mapping_previous = pickle_deepcopy(mapping_st)
                 mapping_current = pickle_deepcopy(mapping_st)
                 continue
             else:
                 done = True
 
         self.mapping_dic_stationary = mapping_st
         self.MAC_level_data_stationary_cycle = MAC_level_st
 
-    ## Calculate the iteration cycles that each memory level covers
     def calc_cycle_cabl_level(self):
+        """! Calculate the iteration cycles that each memory level covers"""
         # iteration_each_level only counts for the current level for-loops
         iteration_each_level = {
             op: [
-                prod(
-                    [loop_dim for (_, loop_dim) in self.mapping_dic_stationary[op][lv]]
-                )
+                math.prod([loop_dim for (_, loop_dim) in self.mapping_dic_stationary[op][lv]])
                 for lv in range(self.mem_level[op])
             ]
             for op in self.operand_list
         }
         # cycle_per_level count for current and below levels' for-loops
         cycle_cabl_level = {
-            op: [
-                prod(iteration_each_level[op][0 : lv + 1])
-                for lv in range(self.mem_level[op])
-            ]
+            op: [math.prod(iteration_each_level[op][0 : lv + 1]) for lv in range(self.mem_level[op])]
             for op in self.operand_list
         }
 
         # ASSERT: The total cycle count must be the same for all operand
         total_cycle = [cycle_cabl_level[op][-1] for op in self.operand_list]
         assert all(
             x == total_cycle[0] for x in total_cycle
@@ -126,39 +103,37 @@
 
         self.cycle_cabl_level = cycle_cabl_level
         self.total_cycle = total_cycle[0]
 
     def calc_top_r_and_ir_loop(self):
         # top_ir_loop_size: For each memory level, from top to bottom, the product of top few irrelevant loops.
         # top_ir is used for later required instant memory bandwidth calculation.
-    
+
         # Initialization
         # self.mem_level[op] + 1 to add the placeholder for operational array level
-        top_r_loop_size = {
+        top_r_loop_size: dict[LayerOperand, list[UnrollFactor]] = {
             op: [1 for _ in range(self.mem_level[op] + 1)] for op in self.operand_list
         }
 
-        top_ir_loop_size = {
+        top_ir_loop_size: dict[LayerOperand, list[UnrollFactor]] = {
             op: [1 for _ in range(self.mem_level[op] + 1)] for op in self.operand_list
         }
 
         # Check and extract the top ir loops
         for operand in self.operand_list:
-            for level, current_level_loops in enumerate(
-                self.mapping_dic_stationary[operand]
-            ):
+            for level, current_level_loops in enumerate(self.mapping_dic_stationary[operand]):
                 if not current_level_loops:
                     continue
                 else:
                     for loop_type, loop_dim in reversed(current_level_loops):
-                        if loop_type in self.layer_node.operand_loop_dim[operand]["r"]:
+                        if loop_type in self.layer_node.loop_relevancy_info.get_r_layer_dims(operand):
                             top_r_loop_size[operand][level + 1] *= loop_dim
                         else:
                             break
                     for loop_type, loop_dim in reversed(current_level_loops):
-                        if loop_type in self.layer_node.operand_loop_dim[operand]["ir"]:
+                        if loop_type in self.layer_node.loop_relevancy_info.get_ir_layer_dims(operand):
                             top_ir_loop_size[operand][level + 1] *= loop_dim
                         else:
                             break
 
         self.top_r_loop_size = top_r_loop_size
         self.top_ir_loop_size = top_ir_loop_size
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/opt/temporal/loma/engine.py` & `zigzag_dse-3.1.1/zigzag/opt/loma/LomaEngine.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,225 +1,220 @@
 from math import factorial
 import operator
+from typing import Any, Generator
 from tqdm import tqdm
 import numpy as np
 from sympy.ntheory import factorint
 import logging
 
-from zigzag.classes.hardware.architecture.memory_hierarchy import MemoryHierarchy
-from zigzag.classes.opt.temporal.loma.multipermute import permutations
-from zigzag.classes.opt.temporal.loma.memory_allocator import (
+
+from zigzag.datatypes import LayerDim
+from zigzag.hardware.architecture.Accelerator import Accelerator
+from zigzag.hardware.architecture.MemoryHierarchy import MemoryHierarchy
+from zigzag.mapping.SpatialMappingInternal import SpatialMappingInternal
+from zigzag.opt.loma.multipermute import permutations
+from zigzag.opt.loma.MemoryAllocator import (
     MemoryHierarchyTooSmallException,
     MemoryTooSmallException,
     MemoryAllocator,
 )
+from zigzag.workload.layer_node import LayerNode
 
 logger = logging.getLogger(__name__)
 
-## Description missing
+
 class NoValidLoopOrderingFoundException(Exception):
+
     pass
 
 
-## Class that handles optimization of temporal mapping given a:
-# - layer
-# - spatial mapping
-# - a memory hierarchy
-#
-# This optimization is carried out through loop order based memory allocation.
-# For each ordering of the temporal loops, they are allocated bottom-up to the
-# levels in the memory hierarchy.
-#
-# See https://ieeexplore.ieee.org/document/9458493 for more details.
 class LomaEngine:
+    """! Class that handles optimization of temporal mapping given a:
+    - layer
+    - spatial mapping
+    - a memory hierarchy
+
+    This optimization is carried out through loop order based memory allocation.
+    For each ordering of the temporal loops, they are allocated bottom-up to the
+    levels in the memory hierarchy.
+
+    See https://ieeexplore.ieee.org/document/9458493 for more details.
+    """
 
-    ## The class constructor
-    # Initialize the engine with the given:
-    # - Accelerator
-    # - LayerNode
-    # - SpatialMapping
-    #
-    # The memory hierarchy from the correct core is extracted from the accelerator.
-    #
-    # param accelerator: accelerator to use the memory hierarchy of
-    # param layer: layer to generate temporal mappings for
-    # param spatial_mapping: SpatialMapping to use
-    # param loma_lpf_limit:
-    # param kwargs: further unused, for ease of calling only
     def __init__(
-        self, *, accelerator, layer, spatial_mapping, loma_lpf_limit=np.inf, **kwargs
+        self,
+        *,
+        accelerator: Accelerator,
+        layer: LayerNode,
+        spatial_mapping: SpatialMappingInternal,
+        loma_lpf_limit: int | None = None,
+        **kwargs: Any,
     ):
+        """
+        The memory hierarchy from the correct core is extracted from the accelerator.
+
+        @param accelerator: accelerator to use the memory hierarchy of
+        @param layer: layer to generate temporal mappings for
+        @param spatial_mapping: SpatialMapping to use
+        @param loma_lpf_limit:
+        @param kwargs: further unused, for ease of calling only
+        """
         self.lpf_limit = loma_lpf_limit
 
         self.accelerator = accelerator
         self.layer = layer
         self.spatial_mapping = spatial_mapping
 
         # Extract the memory hierarchy from the accelerator
         # TODO: Take into account that data might be stored in lower level,
         # TODO: thus adapt the memory hierarchy.
         # TODO: The fact that there is a global buffer above the cores requires attention.
-        core_id = layer.core_allocation
-        self.memory_hierarchy: MemoryHierarchy = accelerator.get_core(
-            core_id
-        ).memory_hierarchy
+        core_id = layer.core_allocation[0]
+        self.memory_hierarchy: MemoryHierarchy = accelerator.get_core(core_id).memory_hierarchy
 
         self.show_progress_bar = kwargs.get("loma_show_progress_bar", False)
 
-    ## Runs the LomaEngine
-    # @return Generator that yields all temporal mappings
     def run(self):
+        """! Runs the LomaEngine
+        @return Generator that yields all temporal mappings
+        """
         # TODO: add the criterion(s) as inputs to this function.
-        logger.info("Running temporal mapping search engine...")
-
         self.get_temporal_loops()  # get all the temporal loops
         self.get_prime_factors()  # convert these to LPFs (loop prime factors)
 
-        if self.show_progress_bar:
-            pbar = tqdm(total=self.nb_permutations)
-        else:
-            pbar = None
+        pbar = tqdm(total=self.nb_permutations) if self.show_progress_bar else None
 
         yielded = False
-        for ordering in self.og():  # ordering generator
-            allocator = MemoryAllocator(
-                self.accelerator, self.layer, self.spatial_mapping, ordering
-            )
+        for ordering in self.ordering_generator():
+            allocator = MemoryAllocator(self.accelerator, self.layer, self.spatial_mapping, ordering)
             # using try catch here because in the depth-first mode the highest level might not be big enough
             try:
-                temporal_mapping = (
-                    allocator.run()
-                )  # allocate this ordering to the memories
+                temporal_mapping = allocator.run()  # allocate this ordering to the memories
                 yielded = True
                 yield temporal_mapping
             except MemoryHierarchyTooSmallException:
                 pass
             except MemoryTooSmallException:
                 pass  # Skip the ordering that crashed due to ordering (+su) not fitting in memory
-            if self.show_progress_bar:
+            if pbar is not None:
                 pbar.update(1)
 
-        if self.show_progress_bar:
+        if pbar is not None:
             pbar.close()
 
         if not yielded:
+            # TODO this warning is unclear: an invalid spatial mapping is not necessarily its cause
             raise NoValidLoopOrderingFoundException(
-                f"No valid loop ordering was found for layer {self.layer}. Please make sure the spatial mapping is compatible with the architecture."
+                f"No valid loop ordering was found for layer {self.layer}. Please make sure the spatial mapping is "
+                f"compatible with the architecture."
             )
 
-    ## Get all loops that have to be temporally scheduled given layer and spatial mapping.
-    def get_temporal_loops(self):
-        temporal_loop_dim_size = (
-            self.layer.loop_dim_size.copy()
-        )  # init with all loop sizes
+    def get_temporal_loops(self) -> None:
+        """! Get all loops that have to be temporally scheduled given layer and spatial mapping.
+        # TODO clean up (and make use of `LayerDimSizes` methods)
+        """
+        layer_dim_sizes = self.layer.layer_dim_sizes.copy()  # init with all loop sizes
         for spatial_loop in self.spatial_mapping.spatial_loop_dim_size:
             (spatial_loop_dim, spatial_loop_size) = spatial_loop
             # Allow greedy mapping. If the spatial unrolling is not a multiple of the layer dimension size,
             # we take the ceil of the division, so there can be one extra temporal iteration.
-            q = int(
-                np.ceil(temporal_loop_dim_size[spatial_loop_dim] / spatial_loop_size)
-            )
-            # q, rem = divmod(temporal_loop_dim_size[spatial_loop_dim], spatial_loop_size)
+            q = int(np.ceil(layer_dim_sizes[spatial_loop_dim] / spatial_loop_size))
+            # q, rem = divmod(layer_dim_sizes[spatial_loop_dim], spatial_loop_size)
             # assert rem == 0, "Division of dimension size by spatial unrolling size is not an integer"
             if q == 1:
-                del temporal_loop_dim_size[spatial_loop_dim]
+                del layer_dim_sizes[spatial_loop_dim]
             else:
-                temporal_loop_dim_size[spatial_loop_dim] = q
+                layer_dim_sizes[spatial_loop_dim] = q
 
         # Remove all dimensions with a temporal loop size of 1
-        temporal_loop_dim_size_no_1s = {
-            key: val for (key, val) in temporal_loop_dim_size.items() if val > 1
-        }
+        temporal_loop_dim_size_no_1s = {key: val for key, val in layer_dim_sizes.items() if val > 1}
 
         self.temporal_loop_dim_size = temporal_loop_dim_size_no_1s
         min_nb_temporal_loops = len(self.temporal_loop_dim_size)
-        if self.lpf_limit < min_nb_temporal_loops:
+        if self.lpf_limit is not None and self.lpf_limit < min_nb_temporal_loops:
             logger.debug(
                 f"Updated layer {self.layer}'s lpf limit from {self.lpf_limit} to {min_nb_temporal_loops} lpfs."
             )
             self.lpf_limit = min_nb_temporal_loops
 
-    ## Get the prime factors for all temporal loops.
-    # This is saved in three separate class attributes (temporal_loop_pfs, temporal_loop_pf_counts, temporal_loop_pf_count_sums)
-    def get_prime_factors(self):
+    def get_prime_factors(self) -> None:
+        """! Get the prime factors for all temporal loops.
+        This is saved in three separate class attributes (temporal_loop_pfs, temporal_loop_pf_counts,
+        temporal_loop_pf_count_sums)
+        # TODO clean up (functions should not change class state variables...)
+        """
         # temporal_loop_pfs: a dict that for each temporal loop dimension contains the prime factors
         # temporal_loop_pf_counts: a dict that for each temporal loop dimension contains the prime factor multiplicities
         # temporal_loop_pf_count_sums: a dict that for each temporal loop dimension contains the total amount of prime factors
 
-        temporal_loop_pfs = {}
-        temporal_loop_pf_counts = {}
-        temporal_loop_pf_count_sums = {}
+        temporal_loop_pfs: dict[LayerDim, tuple[int, ...]] = {}
+        temporal_loop_pf_counts: dict[LayerDim, tuple[int, ...]] = {}
+        temporal_loop_pf_count_sums: dict[LayerDim, int] = {}
         lpfs = []
-        for (
-            tl_dim,
-            tl_size,
-        ) in self.temporal_loop_dim_size.items():  # tl = temporal loop
-            factors = factorint(tl_size)
+        for tl_dim, tl_size in self.temporal_loop_dim_size.items():  # tl = temporal loop
+            factors: dict[int, int] = factorint(tl_size)
             pfs = []
             counts = []
             for pf, multiplicity in factors.items():
                 pfs.append(pf)
                 counts.append(multiplicity)
-                for i in range(multiplicity):
+                for _ in range(multiplicity):
                     lpfs.append((tl_dim, pf))
             temporal_loop_pfs[tl_dim] = tuple(pfs)
             temporal_loop_pf_counts[tl_dim] = tuple(counts)
             temporal_loop_pf_count_sums[tl_dim] = sum(counts)
 
         # If there are no temporal LPFs generated, i.e. all loops are unrolled spatially,
         # we manually insert a loop of size 1
         if lpfs == []:
-            loop_dim = self.layer.loop_dim_list[0]
+            loop_dim = self.layer.layer_dims[0]
             temporal_loop_pfs = {loop_dim: (1,)}
             temporal_loop_pf_counts = {loop_dim: (1,)}
             temporal_loop_pf_count_sums = {loop_dim: 1}
             lpfs = [(loop_dim, 1)]
 
         logger.debug(f"Generated {len(lpfs)} LPFs for layer {self.layer}.")
 
-        self.temporal_loop_pfs = temporal_loop_pfs
+        self.temporal_loop_pfs: dict[LayerDim, tuple[int, ...]] = temporal_loop_pfs
         self.temporal_loop_pf_counts = temporal_loop_pf_counts
         self.temporal_loop_pf_count_sums = temporal_loop_pf_count_sums
         self.lpfs = lpfs
 
         # Limit the number of lpfs (if this is set in the settings)
         self.limit_lpfs()
 
         # Compute how many total permuatations we will have to consider
         self.compute_nb_permutations()
 
-    ## Compute the number of permutations that will have to be considered given the LPF distribution
     def compute_nb_permutations(self):
+        """! Compute the number of permutations that will have to be considered given the LPF distribution"""
         nb_permutations = factorial(sum(self.temporal_loop_pf_count_sums.values()))
         for nb_duplicated_pfs in self.temporal_loop_pf_counts.values():
             for nb_duplicated_pf in nb_duplicated_pfs:
                 nb_permutations = int(nb_permutations / factorial(nb_duplicated_pf))
         self.nb_permutations = nb_permutations
-        logger.debug(
-            f"Launching {self.nb_permutations:,} temporal loop order permutations."
-        )
-
-    ## Function to limit the total number of loop prime factors present in this instance.
-    # This function scans the lpfs and while the number of lpfs is greater than self.lpf_limit it:
-    # - picks the loop dimension that has the most lpfs
-    # - merges the smallest two lpfs of that loop dimension (multiplying their values)
-    def limit_lpfs(self):
+        logger.debug(f"Launching {self.nb_permutations:,} temporal loop order permutations.")
+
+    def limit_lpfs(self) -> None:
+        """! Function to limit the total number of loop prime factors present in this instance.
+        This function scans the lpfs and while the number of lpfs is greater than self.lpf_limit it:
+        - picks the loop dimension that has the most lpfs
+        - merges the smallest two lpfs of that loop dimension (multiplying their values)
+        """
         n_pf = sum(self.temporal_loop_pf_count_sums.values())
-        if n_pf <= self.lpf_limit:
+        if self.lpf_limit is None or n_pf <= self.lpf_limit:
             logger.debug(f"No lpf limiting performed for layer {self.layer}")
             return
         while n_pf > self.lpf_limit:
             # Find the loop dimension with the most lpfs
-            max_ld = max(
-                self.temporal_loop_pf_count_sums.items(), key=operator.itemgetter(1)
-            )[0]
+            max_ld = max(self.temporal_loop_pf_count_sums.items(), key=operator.itemgetter(1))[0]
             # Get the prime factors of this loop dimension
-            max_pfs = list(self.temporal_loop_pfs[max_ld])
+            max_pfs: list[int] = list(self.temporal_loop_pfs[max_ld])
             # Get the multiplicity of these prime factors
-            max_counts = list(self.temporal_loop_pf_counts[max_ld])
+            max_counts: list[int] = list(self.temporal_loop_pf_counts[max_ld])
 
             if max_counts[0] == 1:  # multiplicity of smallest pf is 1
                 new_factor = max_pfs[0] * max_pfs[1]
                 max_counts[0] -= 1
                 max_counts[1] -= 1
             else:  # multiplicity of smalles pf is > 1
                 new_factor = max_pfs[0] * max_pfs[0]
@@ -227,17 +222,15 @@
 
             if new_factor in max_pfs:  # possible if not first iteration of while loop
                 new_factor_idx = max_pfs.index(new_factor)
                 max_counts[new_factor_idx] += 1
             else:  # the new factor is not yet present in the factors, insert so list remains sorted
                 new_factor_idx = len([pf for pf in max_pfs if pf < new_factor])
                 max_pfs.insert(new_factor_idx, new_factor)
-                max_counts.insert(
-                    new_factor_idx, 1
-                )  # first time this factor occured, count = 1
+                max_counts.insert(new_factor_idx, 1)  # first time this factor occured, count = 1
 
             # Sanitize max_pfs and max_counts to remove all elements with multiplicity 0
             non_zero_idxs = [idx for idx, count in enumerate(max_counts) if count != 0]
             max_pfs = [max_pfs[non_zero_idx] for non_zero_idx in non_zero_idxs]
             max_counts = [max_counts[non_zero_idx] for non_zero_idx in non_zero_idxs]
 
             # Update the appropriate variables with these new factors and multiplicities
@@ -245,22 +238,19 @@
             self.temporal_loop_pf_counts[max_ld] = tuple(max_counts)
             self.temporal_loop_pf_count_sums[max_ld] -= 1
 
             # Decrease the total number of factors by 1
             n_pf -= 1
 
         # Update self.lpfs for these new factors
-        lpfs = []
-        for dim in self.temporal_loop_pfs.keys():
-            for (pf, count) in zip(
-                self.temporal_loop_pfs[dim], self.temporal_loop_pf_counts[dim]
-            ):
-                lpfs += list(((dim, pf),) * count)
+        lpfs: list[tuple[LayerDim, int]] = []
+        for layer_dim, loop in self.temporal_loop_pfs.items():
+            for pf, count in zip(loop, self.temporal_loop_pf_counts[layer_dim]):
+                lpfs += list(((layer_dim, pf),) * count)
         self.lpfs = lpfs
 
         logger.debug(f"Limited layer {self.layer} to {len(self.lpfs)} lpfs.")
         return
 
-    ## Generator that yields all orderings of the temporal loops.
-    def og(self):
-        # The lpfs are stored in self.lpfs
-        return permutations(self.lpfs)
+    def ordering_generator(self) -> Generator[list[tuple[LayerDim, int]], None, None]:
+        """! Generator that yields all orderings of the temporal loops."""
+        return permutations(self.lpfs)  # type:ignore
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/opt/temporal/loma/memory_allocator.py` & `zigzag_dse-3.1.1/zigzag/opt/loma/MemoryAllocator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,337 +1,317 @@
-from typing import List
 import numpy as np
 from math import prod
 
-from zigzag.classes.hardware.architecture.memory_hierarchy import MemoryHierarchy
-from zigzag.classes.hardware.architecture.memory_level import MemoryLevel
-from zigzag.classes.mapping.temporal.temporal_mapping import TemporalMapping
-from zigzag.classes.opt.temporal.loma.loop import Loop
 
-## Missing description
+from zigzag.datatypes import Constants, LayerDim, LayerOperand, MemoryOperand, UnrollFactor, UnrollFactorInt
+from zigzag.hardware.architecture.Accelerator import Accelerator
+from zigzag.hardware.architecture.MemoryHierarchy import MemoryHierarchy
+from zigzag.hardware.architecture.memory_level import MemoryLevel
+from zigzag.mapping.SpatialMappingInternal import SpatialMappingInternal
+from zigzag.mapping.TemporalMapping import TemporalMapping, TemporalMappingDict
+from zigzag.opt.loma.Loop import Loop
+from zigzag.workload.layer_attributes import LayerDimSizes
+from zigzag.workload.layer_node import LayerNode
+
+
 class MemoryHierarchyTooSmallException(Exception):
+    """! Missing description"""
+
     pass
 
-## Missing description
+
 class MemoryTooSmallException(Exception):
+    """! Missing description"""
+
     pass
 
-## Class that handles allocation of a loop ordering to the memories in the hierarchy.
+
 class MemoryAllocator:
+    """! Class that handles allocation of a loop ordering to the memories in the hierarchy."""
 
-    ## The class constructor
-    # 
-    # Initialize the class with:
-    # - the layer
-    # - the memory hierarchy parameters
-    # - the spatial mapping
-    # 
-    # through main_inputs and
-    # - ordering
-    # 
-    # @param accelerator
-    # @param layer
-    # @param spatial_mapping
-    # @param ordering
-    def __init__(self, accelerator, layer, spatial_mapping, ordering: List):
+    def __init__(
+        self,
+        accelerator: Accelerator,
+        layer: LayerNode,
+        spatial_mapping: SpatialMappingInternal,
+        ordering: list[tuple[LayerDim, UnrollFactorInt]],
+    ):
         self.accelerator = accelerator
         self.layer = layer
         self.spatial_mapping = spatial_mapping
         self.ordering = ordering
 
         # Initialize the different operands
-        # On the HW side, these are always called 'I1' 'I2' and 'O',
-        # but on the layer side, they can be anything.
-        layer_ops = self.layer.operand_list
-        self.mem_ops = [
-            self.layer.memory_operand_links[layer_op] for layer_op in layer_ops
-        ]
-        # Translation dict from layer op to mem op
-        self.layer_to_mem_op = self.layer.memory_operand_links.copy()
-        # Translation dict from mem op to layer op
-        self.mem_to_layer_op = {
-            mem_op: layer_op for (layer_op, mem_op) in self.layer_to_mem_op.items()
+        # On the HW side, these are always called 'I1' 'I2' and 'O', but on the layer side, they can be anything.
+        layer_ops = self.layer.layer_operands
+        self.mem_ops: list[MemoryOperand] = [self.layer.memory_operand_links[layer_op] for layer_op in layer_ops]
+        self.layer_to_mem_op: dict[LayerOperand, MemoryOperand] = {
+            layer_op: self.layer.memory_operand_links.layer_to_mem_op(layer_op)
+            for layer_op in self.layer.memory_operand_links.layer_operands
+        }
+        self.mem_to_layer_op: dict[MemoryOperand, LayerOperand] = {
+            mem_op: self.layer.memory_operand_links.mem_to_layer_op(mem_op)
+            for mem_op in self.layer.memory_operand_links.mem_operands
         }
+
         # Bit precision for the different mem ops
-        self.precision = {
-            mem_op: self.layer.operand_precision[layer_op]
-            for (layer_op, mem_op) in self.layer_to_mem_op.items()
+        self.precision: dict[MemoryOperand, int] = {
+            mem_op: self.layer.operand_precision[layer_op] for layer_op, mem_op in self.layer_to_mem_op.items()
         }
-        self.precision["O_final"] = self.layer.operand_precision.get(
-            "O_final", self.precision["O"]
-        )  # Final output precision
+        # Final output precision
+        self.precision[Constants.FINAL_OUTPUT_MEM_OP] = self.layer.operand_precision.final_output_precision
         # Initialize the unallocated loops with the ordering for each operand
-        self.unallocated = {}
+        self.unallocated: dict[MemoryOperand, list[Loop]] = {}
         for mem_op in self.mem_ops:
-            self.unallocated[mem_op] = [
-                Loop(dim, size) for (dim, size) in self.ordering
-            ]
+            self.unallocated[mem_op] = [Loop(dim, size) for (dim, size) in self.ordering]
 
         # Initialize the allocated loops with the spatial mapping at the operand level for each operand
-        self.allocated = {}
-        for (layer_op, mem_op) in self.layer_to_mem_op.items():
+        self.allocated: dict[MemoryOperand, list[Loop]] = {}
+        for layer_op, mem_op in self.layer_to_mem_op.items():
             self.allocated[mem_op] = [
-                Loop(dim, size, "spatial")
-                for (dim, size) in self.spatial_mapping.get_unrolling(
-                    op=layer_op, level=0
-                )
+                Loop(dim, size, "spatial") for (dim, size) in self.spatial_mapping.get_unrolling(op=layer_op, level=0)
             ]
 
         # Initialize the level of memory hierarchy for each layer operand at 1 (first memory level).
         # This information is required to fetch the correct spatial loops after we have allocated temporal loops.
         self.mem_level = {layer_op: 1 for layer_op in layer_ops}
 
         # Initialize the temporal mapping dict, which is appended to throughout the allocation process.
         # It is a dictionary with keys the different layer operands and values a list of lists.
         # The sublists represent the memory levels for that operand and contain the loops allocated to that level.
-        self.temporal_mapping_dict = {layer_op: [] for layer_op in layer_ops}
+        self.temporal_mapping_dict: TemporalMappingDict = {layer_op: [] for layer_op in layer_ops}
 
-    ## Run the memory allocation process.
-    # Start by the lowest memory hierarchy level and allocate as much loops as possible
-    # for the different operands. The spatial unrolling has to be taken into account at
-    # each memory level in the hierarchy.
     def run(self):
+        """! Run the memory allocation process.
+        Start by the lowest memory hierarchy level and allocate as much loops as possible
+        for the different operands. The spatial unrolling has to be taken into account at
+        each memory level in the hierarchy.
+        """
 
         # self.nodes contains the different memory nodes in bottom-up fashion
-        core_id = self.layer.core_allocation
-        memory_hierarchy: MemoryHierarchy = self.accelerator.get_core(
-            core_id
-        ).memory_hierarchy
-        top_levels = {
-            mem_op: memory_hierarchy.get_operand_top_level(mem_op)
-            for mem_op in self.mem_ops
-        }
+        core_id = self.layer.core_allocation[0]
+        memory_hierarchy: MemoryHierarchy = self.accelerator.get_core(core_id).memory_hierarchy
+        top_levels = {mem_op: memory_hierarchy.get_operand_top_level(mem_op) for mem_op in self.mem_ops}
         nodes = memory_hierarchy.nodes
         for node in nodes:
             self.allocate_node(node, top_levels)
 
-        # After all the nodes have been allocated, we can creat the TemporalMapping
+        # After all the nodes have been allocated, we can create the TemporalMapping
         # object from the dictionary we have built
         temporal_mapping = TemporalMapping(self.temporal_mapping_dict, self.layer)
-
         return temporal_mapping
 
-    ## Allocate a single memory node with the best loops that remain in the unallocated loop ordering.
-    # @param node: The MemoryLevel to which we will allocate loops.
-    # @param top_levels: A list of MemoryLevels for each mem_op that is the highest MemoryLevel that stores that mem_op.
-    def allocate_node(self, node: MemoryLevel, top_levels: List[MemoryLevel]):
+    def allocate_node(self, node: MemoryLevel, top_levels: dict[MemoryOperand, MemoryLevel]):
+        """! Allocate a single memory node with the best loops that remain in the unallocated loop ordering.
+        @param node: The MemoryLevel to which we will allocate loops.
+        @param top_levels: A list of MemoryLevels for each mem_op that is the highest MemoryLevel that stores that mem_op.
+        #TODO cleanup
+        """
 
         # Find out which mem operands this node stores
         mem_ops = node.operands
-        # Then select only the mem operands that are required for this layer (e.g. pooling has no weights so one mem op less)
+        # Then select only the mem operands that are required for this layer (e.g. pooling has no weights so one mem
+        # op less)
         mem_ops = [mem_op for mem_op in mem_ops if mem_op in self.mem_ops]
-        # Does this node support double buffering
-        db_support=node.memory_instance.double_buffering_support
+        # Does this node support double buffering # TODO this is not used
+        db_support = node.memory_instance.double_buffering_support
         # Get the capacity of this memory node (in bits)
         mem_capacity = node.memory_instance.size
 
         # For all the mem_ops, find the max amount of unallocated loops we could allocate
-        all_sizes = {}
+        all_sizes: dict[MemoryOperand, list[UnrollFactor]] = {}
         for mem_op in mem_ops:
             sizes = self.calc_size_slices(mem_op, mem_capacity)
             all_sizes[mem_op] = sizes
 
         # Now that we have this for all the mem_ops, call function that finds the best
         # combination of loops to minimize the number of accesses to the level above
-        best_loop_idxs = self.find_best_loop_combination(
-            mem_ops, all_sizes, node, top_levels
-        )
+        best_loop_idxs = self.find_best_loop_combination(mem_ops, all_sizes, node, top_levels)
 
-        for (best_loop_idx, mem_op) in zip(best_loop_idxs, mem_ops):
+        for best_loop_idx, mem_op in zip(best_loop_idxs, mem_ops):
             # Now that we have the combination of loop_idx for each mem_op, add them
             # to the allocated loops and remove them from the unallocated loops
             loops_to_allocate = self.unallocated[mem_op][:best_loop_idx].copy()
             self.allocated[mem_op] += loops_to_allocate
             del self.unallocated[mem_op][:best_loop_idx]
 
             # Add the loops to allocate to the level-by-level temporal_mapping_dict
             # The key of this dict is the layer_op and not the mem_op
             layer_op = self.mem_to_layer_op[mem_op]
-            self.temporal_mapping_dict[layer_op].append(
-                [(loop.dimension, loop.size) for loop in loops_to_allocate]
-            )
+            self.temporal_mapping_dict[layer_op].append([(loop.layer_dim, loop.size) for loop in loops_to_allocate])
 
             # This memory node that stores one or more mem_ops might be
             # spatially unrolled, add these spatially unrolled loops to
             # the list of allocated loops now, so that the next memory nodes
             # correctly see this spatial unrolling.
             # For this we require the level of memory we are evaluating for this op.
             mem_level_op = self.mem_level[layer_op]
-            spatial_loops = self.spatial_mapping.get_unrolling(
-                op=layer_op, level=mem_level_op
-            )
-            for (loop_dim, loop_size) in spatial_loops:
-                spatial_loop = Loop(dimension=loop_dim, size=loop_size, type="spatial")
+            spatial_loops = self.spatial_mapping.get_unrolling(op=layer_op, level=mem_level_op)
+            for loop_dim, loop_size in spatial_loops:
+                spatial_loop = Loop(layer_dim=loop_dim, size=loop_size, type="spatial")
                 self.allocated[mem_op].append(spatial_loop)
 
             # Check if this node (i.e. MemoryLevel) is the highest level of memory hierarchy.
             # If this is the case and we haven't allocated all loops, raise an exception.
-            if (
-                node == top_levels[mem_op] and self.unallocated[mem_op]
-            ):  # if top level and unallocated not empty
+            if node == top_levels[mem_op] and self.unallocated[mem_op]:  # if top level and unallocated not empty
                 raise MemoryHierarchyTooSmallException(
                     f"Highest MemoryLevel for {mem_op} = {node} too small to store all loops."
                 )
 
             # Increment the mem_level we are currently at for this layer_op by 1
             self.mem_level[layer_op] += 1
 
-    ## Calculate the required memory size to store different
-    # slices of the unallocated loops, with 'mem_capacity' as an upper bound.
-    # @param mem_op
-    # @param mem_capacity Capacity of the memory node in bits.
-    # @param db_support Double buffering support of this node
-    def calc_size_slices(self, mem_op: str, mem_capacity: int, db_support: bool=False):
+    def calc_size_slices(
+        self, mem_op: MemoryOperand, mem_capacity: int, db_support: bool = False
+    ) -> list[UnrollFactor]:
+        """! Calculate the required memory size to store different slices of the unallocated loops, with 'mem_capacity'
+        as an upper bound.
+        @param mem_capacity Capacity of the memory node in bits.
+        @param db_support Double buffering support of this node
+        """
 
         # Already allocated loops for this mem_op
         allocated_loops = self.allocated[mem_op]
 
         # Unallocated loops for this mem_op
         unallocated_loops = self.unallocated[mem_op]
-        sizes = []
+        sizes: list[UnrollFactor] = []
 
         # If this memory supports double buffering get the size it would take to allocate everything
         if db_support:
-            all_loops=(allocated_loops+unallocated_loops[:len(unallocated_loops)+1])
-            all_loops_size=self.calc_loops_size(all_loops,mem_op,unallocated_loops)
+            all_loops = allocated_loops + unallocated_loops[: len(unallocated_loops) + 1]
+            all_loops_size = self.calc_loops_size(all_loops, mem_op, unallocated_loops)
 
-        for i in range(
-            len(unallocated_loops) + 1
-        ):  # Go through all slices (includes empty slice)
-            unallocated_slice = unallocated_loops[
-                :i
-            ]  # Grab a slice of the unallocated loops
-            loops = (
-                allocated_loops + unallocated_slice
-            )  # Join them with already allocated loops
+        for i in range(len(unallocated_loops) + 1):  # Go through all slices (includes empty slice)
+            unallocated_slice = unallocated_loops[:i]  # Grab a slice of the unallocated loops
+            loops = allocated_loops + unallocated_slice  # Join them with already allocated loops
             size = self.calc_loops_size(loops, mem_op, unallocated_loops)
             # double size allocated if the node uses double buffering
             if db_support:
-                if len(unallocated_loops[i:])>0 and size<all_loops_size:
-                    size*=2
+                if len(unallocated_loops[i:]) > 0 and size < all_loops_size:
+                    size *= 2
             if size <= mem_capacity:
                 sizes.append(size)
             else:
                 if i == 0:  # This means we can't even store the already allocated loops
                     raise MemoryTooSmallException(
                         f"Memory capacity overflow for mem_op {mem_op}. loops={loops} size={size} mem_capacity={mem_capacity}"
                     )
                 break  # Stop as soon as we have added a loop that overflows the memory
         return sizes
 
-    ## Calculate the 'mem_op' tensor size required for all the loops in 'loops'.
-    # @param loops: The loops we want to calculate the size for.
-    # @para mmem_op: The memory operand we are calculating the size for.
-    # @param all_unallocated_loops: All unallocated loops for this MemoryLevel node. Needed for output precision calculation.
-    def calc_loops_size(self, loops: List, mem_op: str, all_unallocated_loops: List):
+    def calc_loops_size(
+        self, loops: list[Loop], mem_op: MemoryOperand, all_unallocated_loops: list[Loop]
+    ) -> UnrollFactor:
+        """! Calculate the 'mem_op' tensor size required for all the loops in 'loops'.
+        @param loops: The loops we want to calculate the size for.
+        @para mem_op: The memory operand we are calculating the size for.
+        @param all_unallocated_loops: All unallocated loops for this MemoryLevel node. Needed for output precision calculation.
+        """
 
         # First we compute the size of all loop dimensions present in this layer given the loops in 'loops'.
-        all_dimensions = self.layer.loop_dim_list
-        all_dim_sizes = {dim: 1 for dim in all_dimensions}
+        all_dimensions = self.layer.layer_dims
+        all_dim_sizes: dict[LayerDim, UnrollFactor] = {dim: 1 for dim in all_dimensions}
         for loop in loops:
-            all_dim_sizes[loop.dimension] *= loop.size
+            all_dim_sizes[loop.layer_dim] *= loop.size
 
-        op_dimensions = self.layer.operand_loop_dim[self.mem_to_layer_op[mem_op]]
+        corresponding_layer_op = self.mem_to_layer_op[mem_op]
 
         layer_op = self.mem_to_layer_op[mem_op]
-        tensor_size = self.layer.calc_tensor_size(layer_op, all_dim_sizes)
+        tensor_size = self.layer.calc_tensor_size(layer_op, LayerDimSizes(all_dim_sizes))
 
         # Get the precision at which this tensor will have to be stored in the MemoryLevel node.
         # For output it can be either the partial sum precision, or the final sum precision.
         # This depends on if all the irrelevant loops were allocated in a previous MemoryLevel.
         # Which in turn means all remaining unallocated loops for this MemoryLevel must not contain any ir loops.
         # Moreover, there might be unallocated spatial loops.
-        if mem_op == "O":
-            ir_dims = op_dimensions["ir"]  # Irrelevant dimensions
+        if mem_op == Constants.OUTPUT_MEM_OP:
+            ir_dims = self.layer.loop_relevancy_info.get_ir_layer_dims(corresponding_layer_op)
             layer_op = self.mem_to_layer_op[mem_op]
-            unallocated_spatial_dims = [dim for (dim, size) in self.spatial_mapping.get_unrolling_all(layer_op, self.mem_level[layer_op])]
-            unallocated_temporal_dims = [
-                unallocated_loop.dimension for unallocated_loop in all_unallocated_loops
+            unallocated_spatial_dims: list[LayerDim] = [
+                dim for dim, _ in self.spatial_mapping.get_unrolling_all(layer_op, self.mem_level[layer_op])
             ]
+            unallocated_temporal_dims = [unallocated_loop.layer_dim for unallocated_loop in all_unallocated_loops]
             unallocated_dims = unallocated_spatial_dims + unallocated_temporal_dims
             # If there is still an irrelevant unallocated loop dimension, pick the full precision
             if any([dim in ir_dims for dim in unallocated_dims]):
-                precision = self.precision["O"]
+                precision = self.precision[Constants.OUTPUT_MEM_OP]
             else:
-                precision = self.precision["O_final"]
+                precision = self.precision[Constants.FINAL_OUTPUT_MEM_OP]
         else:
             precision = self.precision[mem_op]
 
         tensor_size_bits = tensor_size * precision
 
         return tensor_size_bits
 
-
-    ## Find the best combination of loops from different mem_ops.
-    # Best is defined as the combination that minimizes the number of accesses
-    # to the memory level above.
-    # @param mem_ops
-    # @param all_sizes
-    # @param node
-    # @param top_levels
-    def find_best_loop_combination(self, mem_ops, all_sizes, node, top_levels):
+    def find_best_loop_combination(
+        self,
+        mem_ops: list[MemoryOperand],
+        all_sizes: dict[MemoryOperand, list[UnrollFactor]],
+        node: MemoryLevel,
+        top_levels: dict[MemoryOperand, MemoryLevel],
+    ) -> list[int]:
+        """! Find the best combination of loops from different mem_ops. Best is defined as the combination that
+        minimizes the number of accesses to the memory level above.
+        # TODO cleanup
+        """
         # TODO: Take into account the operand precision which can change based on the loops picked
         mem_capacity = node.memory_instance.size
 
         # nb_operations = self.__main_inputs.layer.total_MAC_count
         # all_accesses = {mem_op: [nb_operations//size for size in all_sizes[mem_op]] for mem_op in mem_ops}
 
         # If for one of the mem_ops this is the top level memory, we have to enforce that all unallocated loops
         # will be allocated for this operand. We do this by changing the sizes for this mem_op to only include
         # the last number (which represents the size to store all the ops).
         # Because we modify the sizes, we add an offset to the loop_idx for this mem_op.
         loop_idx_offsets = {mem_op: 0 for mem_op in mem_ops}
         for mem_op, sizes in all_sizes.items():
             if node == top_levels[mem_op]:
-                loop_idx_offsets[mem_op] = (
-                    len(sizes) - 1
-                )  # offset is number of original sizes - 1
+                loop_idx_offsets[mem_op] = len(sizes) - 1  # offset is number of original sizes - 1
                 all_sizes[mem_op] = [sizes[-1]]
 
-        all_accesses = {mem_op: [] for mem_op in mem_ops}
+        all_accesses: dict[MemoryOperand, list[float]] = {mem_op: [] for mem_op in mem_ops}
         for mem_op in mem_ops:
             # The number of accesses to the level above is determined through the reuse we have for the different
             # choices of temporal loops. accesses = # total temporal loop iterations / temporal reuse
             # The temporal reuse = # allocated loop iterations / operand size
             # Thus: accesses = # total iterations / (# allocated iterations / size)
             # Thus: accesses = (# total iterations / # allocated iterations) * size
             # Thus: accesses = # unallocated iterations * size
             for i, size in enumerate(all_sizes[mem_op]):
-                unallocated_loops = self.unallocated[mem_op][
-                    (i + loop_idx_offsets[mem_op]) :
-                ]  # slice of unallocated loops for this operand size
-                unallocated_iterations = prod(
-                    (unallocated_loop.size for unallocated_loop in unallocated_loops)
-                )
+                # slice of unallocated loops for this operand size
+                unallocated_loops = self.unallocated[mem_op][(i + loop_idx_offsets[mem_op]) :]
+                unallocated_iterations = prod((unallocated_loop.size for unallocated_loop in unallocated_loops))
                 if node == top_levels[mem_op]:
                     accesses = 0
                 else:
                     accesses = unallocated_iterations * size
                 all_accesses[mem_op].append(accesses)
 
         all_max_nb_loops = {mem_op: len(all_sizes[mem_op]) for mem_op in mem_ops}
         all_max_nb_loops_list = list(all_max_nb_loops.values())
-        best_loop_idxs = [0 for mem_op in mem_ops]
+        best_loop_idxs = [0 for _ in mem_ops]
         best_accesses = np.inf
         nb_combinations = prod(len(sizes) for sizes in all_sizes.values())
         for i in range(nb_combinations):
             size_comb = 0
             accesses_comb = 0
-            current_loop_idxs = []
+            current_loop_idxs: list[int] = []
             for mem_op_idx, mem_op in enumerate(mem_ops):
                 this_max_nb_loops = all_max_nb_loops_list[mem_op_idx]
-                current_loop_idx = (
-                    i // prod(all_max_nb_loops_list[mem_op_idx + 1 :])
-                ) % this_max_nb_loops
+                current_loop_idx = (i // prod(all_max_nb_loops_list[mem_op_idx + 1 :])) % this_max_nb_loops
                 current_loop_idxs.append(current_loop_idx + loop_idx_offsets[mem_op])
                 size_comb += all_sizes[mem_op][current_loop_idx]
                 accesses_comb += all_accesses[mem_op][current_loop_idx]
             if size_comb > mem_capacity:
                 if i == 0:
                     raise MemoryTooSmallException(
-                        "The memory can't store all loops assigned to lower level memories. Likely due to spatial unrolling."
+                        """The memory can't store all loops assigned to lower level memories. Likely due to spatial 
+                        unrolling."""
                     )
                 continue
             if accesses_comb <= best_accesses:
                 best_accesses = accesses_comb
                 best_loop_idxs = current_loop_idxs
         return best_loop_idxs
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/opt/temporal/salsa/engine.py` & `zigzag_dse-3.1.1/zigzag/opt/salsa/SalsaEngine.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,89 +23,83 @@
 #   distributed under the License is distributed on an AS IS BASIS, WITHOUT
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
 from copy import deepcopy
+from multiprocessing_on_dill import Queue
+from typing import Any
 from sympy.ntheory import factorint
 import numpy as np
 import logging
 import random
 
-from zigzag.classes.hardware.architecture.accelerator import Accelerator
-from zigzag.classes.workload.layer_node import LayerNode
-from zigzag.classes.mapping.spatial.spatial_mapping import SpatialMapping
-from zigzag.classes.hardware.architecture.memory_hierarchy import MemoryHierarchy
-from zigzag.classes.opt.temporal.loma.multipermute import permutations
-from zigzag.classes.opt.temporal.loma.memory_allocator import MemoryAllocator
-from zigzag.classes.opt.temporal.salsa.state import SalsaState
+
+from zigzag.hardware.architecture.Accelerator import Accelerator
+from zigzag.workload.layer_node import LayerNode
+from zigzag.mapping.SpatialMappingInternal import SpatialMappingInternal
+from zigzag.opt.salsa.SalsaState import SalsaState
 
 logger = logging.getLogger(__name__)
 
-## Class that handles optimization of temporal mapping given a:
-# - layer
-# - spatial mapping
-# - memory hierarchy
-# - number of iterations
-# - start temperature
-# This optimization is carried out through simulated annealing loop order based.
-# Each loop is broken down to the smallest possible part (prime factors), then a runtime
-# estimation is performed to choose the fastest engine to use (LOMA or SALSA).
+
 class SalsaEngine:
+    """! Class that handles optimization of temporal mapping given a:
+    - layer
+    - spatial mapping
+    - memory hierarchy
+    - number of iterations
+    - start temperature
+    This optimization is carried out through simulated annealing loop order based.
+    Each loop is broken down to the smallest possible part (prime factors), then a runtime estimation is performed to
+    choose the fastest engine to use (LOMA or SALSA).
+    # TODO cleanup
+    """
 
-    ## The class constructor
-    # @param acceleartor
-    # @param layer
-    # @param spatial mapping
-    # @param kwargs
     def __init__(
         self,
         *,
         accelerator: Accelerator,
         layer: LayerNode,
-        spatial_mapping: SpatialMapping,
-        **kwargs,
+        spatial_mapping: SpatialMappingInternal,
+        **kwargs: Any,
     ):
-
-        # iteration_number, start_temperature, opt_criterion_name
-
-        # Initialize the engine with the given:
-        # - LayerNode
-        # - SpatialMapping
-        # - Accelerator
-        # - Number of iterations
-        # - Start temperature
-        # The memory hierarchy from the correct core is extracted from the accelerator.
+        """! Initialize the engine with the given:
+        - LayerNode
+        - SpatialMapping
+        - Accelerator
+        - Number of iterations
+        - Start temperature
+        The memory hierarchy from the correct core is extracted from the accelerator.
+        """
 
         # Hardware and mapping related inputs
         self.accelerator = accelerator
         self.layer = layer
         self.spatial_mapping = spatial_mapping
-        # self.memory_hierarchy: MemoryHierarchy = self.accelerator.get_core(layer.core_allocation).memory_hierarchy
 
         # Algorithm related inputs
         self.iteration_number = kwargs.get("salsa_iteration_number", 1000)
         self.start_temperature = kwargs.get("salsa_start_temperature", 0.05)
         self.opt_criterion_name = kwargs.get("salsa_opt_criterion", "energy")
         self.lpf_limit = kwargs.get("loma_lpf_limit", 4)
 
-    ## Call the necessary methods, start the processes and collect the best temporal mapping found during the run.
-    def run(self, cme_queue):
+    def run(self, cme_queue: Queue):
+        """! Call the necessary methods, start the processes and collect the best temporal mapping found during the
+        run."""
         self.cme_queue = cme_queue
         self.get_temporal_loops()
         self.get_prime_factors()
         self.run_simulated_annealing_opt(self.cme_queue)
 
-    ## Run a simulated annealing optimiation on the loop ordering using a loma memory allocation strategy.
     def run_simulated_annealing_opt(self, cme_queue):
+        """! Run a simulated annealing optimization on the loop ordering using a loma memory allocation strategy."""
         temperature = self.start_temperature
-        start_ordering = (
-            self.temporal_mapping_lpf
-        )  # tmo stands for temporal mapping ordering
+        start_ordering = self.temporal_mapping_lpf  # tmo stands for temporal mapping ordering
 
         # Initialize the algorithm with a random starting point
         random.shuffle(start_ordering)
 
         # Initialize variables to store current, next and best state
         best_state = SalsaState(
             self.accelerator,
@@ -130,58 +124,50 @@
         )
 
         for it in range(self.iteration_number):
 
             temperature = self.start_temperature * (0.995**it)
 
             # Get the index of the loop to swap
-            i = np.random.randint(0, len(current_state.ordering))
-            j = np.random.randint(0, len(current_state.ordering))
+            i = int(np.random.randint(0, len(current_state.ordering)))
+            j = int(np.random.randint(0, len(current_state.ordering)))
 
             # Swap the loops
             next_state = current_state.swap(i, j)
 
             x = np.random.rand()  # x belongs to [0, 1]
-            p = np.exp(
-                ((current_state.opt_criterion / next_state.opt_criterion) - 1)
-                / temperature
-            )  # probability of accepting the next state
+            # probability of accepting the next state
+            p = np.exp(((current_state.opt_criterion / next_state.opt_criterion) - 1) / temperature)
 
             if x < p:
                 # Replace the current state by the next state and compare the energy with the best state
                 current_state = deepcopy(next_state)
 
                 if current_state.opt_criterion < best_state.opt_criterion:
                     best_state = deepcopy(current_state)
 
         cme_queue.put(best_state.cme)
 
-    ## Get all loops that have to be temporally scheduled given layer and spatial mapping.
     def get_temporal_loops(self):
-        temporal_loop_dim_size = (
-            self.layer.loop_dim_size.copy()
-        )  # init with all loop sizes
+        """! Get all loops that have to be temporally scheduled given layer and spatial mapping."""
+        temporal_loop_dim_size = self.layer.layer_dim_sizes.copy()  # init with all loop sizes
         for spatial_loop in self.spatial_mapping.spatial_loop_dim_size:
             (spatial_loop_dim, spatial_loop_size) = spatial_loop
             # Allow greedy mapping. If the spatial unrolling is not a multiple of the layer dimension size,
             # we take the ceil of the division, so there can be one extra temporal iteration.
-            q = int(
-                np.ceil(temporal_loop_dim_size[spatial_loop_dim] / spatial_loop_size)
-            )
+            q = int(np.ceil(temporal_loop_dim_size[spatial_loop_dim] / spatial_loop_size))
             # q, rem = divmod(temporal_loop_dim_size[spatial_loop_dim], spatial_loop_size)
             # assert rem == 0, "Division of dimension size by spatial unrolling size is not an integer"
             if q == 1:
                 del temporal_loop_dim_size[spatial_loop_dim]
             else:
                 temporal_loop_dim_size[spatial_loop_dim] = q
 
         # Remove all dimensions with a temporal loop size of 1
-        temporal_loop_dim_size_no_1s = {
-            key: val for (key, val) in temporal_loop_dim_size.items() if val > 1
-        }
+        temporal_loop_dim_size_no_1s = {key: val for (key, val) in temporal_loop_dim_size.items() if val > 1}
 
         self.temporal_loop_dim_size = temporal_loop_dim_size_no_1s
         min_nb_temporal_loops = len(self.temporal_loop_dim_size)
         if self.lpf_limit < min_nb_temporal_loops:
             logger.debug(
                 f"Updated layer {self.layer}'s lpf limit from {self.lpf_limit} to {min_nb_temporal_loops} lpfs."
             )
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/opt/temporal/salsa/state.py` & `zigzag_dse-3.1.1/zigzag/opt/salsa/SalsaState.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,72 +23,63 @@
 #   distributed under the License is distributed on an AS IS BASIS, WITHOUT
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
 from copy import deepcopy
-from zigzag.classes.opt.temporal.loma.memory_allocator import MemoryAllocator
-from zigzag.classes.cost_model.cost_model import CostModelEvaluation
+from zigzag.datatypes import LayerDim, UnrollFactorInt
+from zigzag.opt.loma.MemoryAllocator import MemoryAllocator
+from zigzag.cost_model.cost_model import CostModelEvaluation
+
+from zigzag.hardware.architecture.Accelerator import Accelerator
+from zigzag.workload.layer_node import LayerNode
+from zigzag.mapping.SpatialMappingInternal import SpatialMappingInternal
+from zigzag.hardware.architecture.MemoryHierarchy import MemoryHierarchy
 
-from zigzag.classes.hardware.architecture.accelerator import Accelerator
-from zigzag.classes.workload.layer_node import LayerNode
-from zigzag.classes.mapping.spatial.spatial_mapping import SpatialMapping
-from zigzag.classes.hardware.architecture.memory_hierarchy import MemoryHierarchy
 
-## State of SALSA, storing an ordering, his temporal mapping and his energy value.
 class SalsaState:
+    """! State of SALSA, storing an ordering, his temporal mapping and his energy value."""
 
     def __init__(
         self,
         accelerator: Accelerator,
         layer: LayerNode,
-        spatial_mapping: SpatialMapping,
-        ordering,
-        opt_criterion_name,
+        spatial_mapping: SpatialMappingInternal,
+        ordering: list[tuple[LayerDim, UnrollFactorInt]],
+        opt_criterion_name: str,
     ):
+        assert opt_criterion_name in ("energy", "latency")  # TODO make this an enum?
         self.ordering = ordering
         self.accelerator = accelerator
         self.layer = layer
         self.spatial_mapping = spatial_mapping
-        self.memory_hierarchy: MemoryHierarchy = self.accelerator.get_core(
-            layer.core_allocation
-        ).memory_hierarchy
+        self.memory_hierarchy: MemoryHierarchy = self.accelerator.get_core(layer.core_allocation[0]).memory_hierarchy
         self.opt_criterion_name = opt_criterion_name
 
-        allocator = MemoryAllocator(
-            self.accelerator, self.layer, self.spatial_mapping, ordering
-        )
+        allocator = MemoryAllocator(self.accelerator, self.layer, self.spatial_mapping, ordering)
 
-        # allocator = MemoryAllocator(layer=self.layer,
-        #                                 ordering=ordering,
-        #                                 spatial_mapping=self.spatial_mapping)
-
-        self.temporal_mapping = (
-            allocator.run()
-        )  # allocate this ordering to the memories
+        self.temporal_mapping = allocator.run()  # allocate this ordering to the memories
 
         self.cme = CostModelEvaluation(
             accelerator=self.accelerator,
             layer=self.layer,
             spatial_mapping=self.spatial_mapping,
+            spatial_mapping_int=self.spatial_mapping,  # TODO the int version is missing?
             temporal_mapping=self.temporal_mapping,
         )
 
         # The optimization criterion will be minimized
         if self.opt_criterion_name == "energy":
             self.opt_criterion = self.cme.energy_total
         elif self.opt_criterion_name == "latency":
             self.opt_criterion = self.cme.latency_total0
-        else:
-            self.opt_criterion = None
 
-    ## Swap between the element at positon i and j in the ordering
-    # and return the new resulting state.
-    def swap(self, i, j):
+    def swap(self, i: int, j: int) -> "SalsaState":
+        """! Swap between the element at position i and j in the ordering and return the new resulting state."""
 
         swapped_ordering = deepcopy(self.ordering)
         temp = swapped_ordering[i]
         swapped_ordering[i] = swapped_ordering[j]
         swapped_ordering[j] = temp
 
         return SalsaState(
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/stages/CostModelStage.py` & `zigzag_dse-3.1.1/zigzag/stages/CostModelStage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,85 +1,68 @@
-from typing import Generator, Callable, List, Tuple, Any
+from typing import Any
 
-from zigzag.classes.stages.Stage import Stage
-from zigzag.classes.cost_model.cost_model import CostModelEvaluation
-from zigzag.classes.cost_model.cost_model_for_sram_imc import CostModelEvaluationForIMC
-from zigzag.classes.hardware.architecture.accelerator import Accelerator
-from zigzag.classes.mapping.spatial.spatial_mapping import SpatialMapping
-from zigzag.classes.mapping.temporal.temporal_mapping import TemporalMapping
-from zigzag.classes.workload.layer_node import LayerNode
+
+from zigzag.stages.Stage import Stage, StageCallable
+from zigzag.cost_model.cost_model import CostModelEvaluation
+from zigzag.cost_model.CostModelEvaluationForIMC import CostModelEvaluationForIMC
+from zigzag.hardware.architecture.Accelerator import Accelerator
+from zigzag.mapping.SpatialMappingInternal import SpatialMappingInternal
+from zigzag.mapping.TemporalMapping import TemporalMapping
+from zigzag.workload.layer_node import LayerNode
 
 import logging
 
 logger = logging.getLogger(__name__)
 
-##  Pipeline stage that calls a cost model to evaluate a mapping on a HW config.
+
 class CostModelStage(Stage):
+    """!  Pipeline stage that calls a cost model to evaluate a mapping on a HW config."""
 
-    ## The class constructor 
-    # Initializes the cost model stage given main inputs
-    # @param list_of_callables
-    # @param accelerator
-    # @param layer
-    # @param spatial_mapping
-    # @param temporal_mapping
-    # @param access_same_data_considered_as_no_access
-    # @param kwargs
     def __init__(
         self,
-        list_of_callables: List[Callable],
+        list_of_callables: list[StageCallable],
         *,
-        accelerator,
-        layer,
-        spatial_mapping,
-        spatial_mapping_int,
-        temporal_mapping,
-        access_same_data_considered_as_no_access=True,
-        **kwargs
+        accelerator: Accelerator,
+        layer: LayerNode,
+        spatial_mapping: SpatialMappingInternal,
+        spatial_mapping_int: SpatialMappingInternal,
+        temporal_mapping: TemporalMapping,
+        access_same_data_considered_as_no_access: bool = True,
+        **kwargs: Any,
     ):
         super().__init__(list_of_callables, **kwargs)
-        (
-            self.accelerator,
-            self.layer,
-            self.spatial_mapping,
-            self.spatial_mapping_int,
-            self.temporal_mapping,
-            self.access_same_data_considered_as_no_access,
-        ) = (
-            accelerator,
-            layer,
-            spatial_mapping,
-            spatial_mapping_int,
-            temporal_mapping,
-            access_same_data_considered_as_no_access,
-        )
-
-    ## Run the cost model stage by calling the internal zigzag cost model with the correct inputs.
-    def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
-        core_id = self.layer.core_allocation
+
+        self.accelerator = accelerator
+        self.layer = layer
+        self.spatial_mapping = spatial_mapping
+        self.spatial_mapping_int = spatial_mapping_int
+        self.temporal_mapping = temporal_mapping
+        self.access_same_data_considered_as_no_access = access_same_data_considered_as_no_access
+
+    def run(self):
+        """! Run the cost model stage by calling the internal zigzag cost model with the correct inputs."""
+        core_id = self.layer.core_allocation[0]
         core = self.accelerator.get_core(core_id)
         operational_array = core.operational_array
-        pe_type = getattr(operational_array, "pe_type", None) # return None if it does not exist
-        if pe_type is not None and pe_type in ["in_sram_computing"]: # if pe_type exists and in the list
-            self.cme = CostModelEvaluationForIMC(
+        pe_type = getattr(operational_array, "pe_type", None)
+        if pe_type is not None and pe_type == "in_sram_computing":
+            cme = CostModelEvaluationForIMC(
                 accelerator=self.accelerator,
                 layer=self.layer,
                 spatial_mapping=self.spatial_mapping,
                 spatial_mapping_int=self.spatial_mapping_int,
                 temporal_mapping=self.temporal_mapping,
-                # the below parameter is optional
                 access_same_data_considered_as_no_access=self.access_same_data_considered_as_no_access,
             )
         else:
-            self.cme = CostModelEvaluation(
+            cme = CostModelEvaluation(
                 accelerator=self.accelerator,
                 layer=self.layer,
                 spatial_mapping=self.spatial_mapping,
                 spatial_mapping_int=self.spatial_mapping_int,
                 temporal_mapping=self.temporal_mapping,
-                # the below parameter is optional
                 access_same_data_considered_as_no_access=self.access_same_data_considered_as_no_access,
             )
-        yield (self.cme, None)
+        yield cme, None
 
     def is_leaf(self) -> bool:
         return True
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/stages/DumpStage.py` & `zigzag_dse-3.1.1/zigzag/stages/DumpStage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 import pickle
-from typing import Generator, Any, Tuple
-from zigzag.classes.stages.Stage import Stage
-from zigzag.classes.cost_model.cost_model import CostModelEvaluation
+from typing import Any
+
+
+from zigzag.stages.Stage import Stage, StageCallable
+from zigzag.cost_model.cost_model import CostModelEvaluation
 import os
 
-## Class that passes through all results yielded by substages, but dumps the results as a pickled list to a file
-# at the end of the iteration
+
 class DumpStage(Stage):
+    """! Class that passes through all results yielded by substages, but dumps the results as a pickled list to a file
+    at the end of the iteration
+    """
 
-    ## The class constructor
-    # @param list_of_callables: see Stage
-    # @param dump_filename_pattern: filename string formatting pattern, which can use named field whose values will be
-    # in kwargs (thus supplied by higher level runnables)
-    # @param kwargs: any kwargs, passed on to substages and can be used in dump_filename_pattern
-    def __init__(self, list_of_callables, *, dump_filename_pattern, **kwargs):
+    def __init__(self, list_of_callables: list[StageCallable], *, dump_filename_pattern: str, **kwargs: Any):
+        """
+        @param list_of_callables: see Stage
+        @param dump_filename_pattern: filename string formatting pattern, which can use named field whose values will be
+        in kwargs (thus supplied by higher level runnables)
+        @param kwargs: any kwargs, passed on to substages and can be used in dump_filename_pattern
+        """
         super().__init__(list_of_callables, **kwargs)
         self.dump_filename_pattern = dump_filename_pattern
 
-    ## Run the compare stage by comparing a new cost model output with the current best found result.
-    def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
+    def run(self):
+        """! Run the compare stage by comparing a new cost model output with the current best found result."""
         substage = self.list_of_callables[0](self.list_of_callables[1:], **self.kwargs)
-        list = []
+        dump_list: list[tuple[CostModelEvaluation, Any]] = []
         filename = self.dump_filename_pattern.format(**self.kwargs)
         for cme, extra_info in substage.run():
-            list.append((cme, extra_info))
+            dump_list.append((cme, extra_info))
             yield cme, extra_info
         os.makedirs(os.path.dirname(filename), exist_ok=True)
         with open(filename, "wb") as f:
-            pickle.dump(list, f, -1)
+            pickle.dump(dump_list, f, -1)
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/stages/LomaStage.py` & `zigzag_dse-3.1.1/zigzag/stages/LomaStage.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,49 @@
-from zigzag.classes.hardware.architecture.accelerator import Accelerator
-from zigzag.classes.mapping.spatial.spatial_mapping import SpatialMapping
-from zigzag.classes.opt.temporal.loma.engine import LomaEngine
-from zigzag.classes.workload.layer_node import LayerNode
-from typing import Generator, Callable, List, Tuple, Any
-from zigzag.classes.stages.Stage import Stage
-from zigzag.classes.cost_model.cost_model import CostModelEvaluation
+from zigzag.hardware.architecture.Accelerator import Accelerator
+from zigzag.mapping.SpatialMappingInternal import SpatialMappingInternal
+from zigzag.opt.loma.LomaEngine import LomaEngine
+from zigzag.workload.layer_node import LayerNode
+from typing import Any
+from zigzag.stages.Stage import Stage, StageCallable
+
 
-## Class that iterates through the different temporal mappings generated through
-# the loop order based memory allocation (loma) engine
 class LomaStage(Stage):
+    """! Class that iterates through the different temporal mappings generated through
+    the loop order based memory allocation (loma) engine
+    """
 
-    ## The class constructor
-    # Initialize the LomaStage by setting the accelerator, layer, and spatial mapping.
-    # @param list_of_callables (List[Callable]): List of substages to call with each generated temporal mapping.
-    # @param accelerator (Accelerator): The accelerator object.
-    # @param layer (Layer): The layer object.
-    # @param spatial_mapping (SpatialMapping): The spatial mapping object.
     def __init__(
         self,
-        list_of_callables: List[Callable],
+        list_of_callables: list[StageCallable],
         *,
-        accelerator,
-        layer,
-        spatial_mapping,
-        **kwargs
+        accelerator: Accelerator,
+        layer: LayerNode,
+        spatial_mapping: SpatialMappingInternal,
+        **kwargs: Any,
     ):
+        """
+        Initialize the LomaStage by setting the accelerator, layer, and spatial mapping.
+        @param list_of_callables (List[Callable]): List of substages to call with each generated temporal mapping.
+        """
         super().__init__(list_of_callables, **kwargs)
-        self.accelerator, self.layer, self.spatial_mapping = (
-            accelerator,
-            layer,
-            spatial_mapping,
-        )
-        self.engine = None
+        self.accelerator = accelerator
+        self.layer = layer
+        self.spatial_mapping = spatial_mapping
 
     def run(self):
-        self.engine = LomaEngine(
+        engine = LomaEngine(
             accelerator=self.accelerator,
             layer=self.layer,
             spatial_mapping=self.spatial_mapping,
-            **self.kwargs
+            **self.kwargs,
         )
 
-        for tm in self.engine.run():
+        for temporal_mapping in engine.run():
 
             kwargs = self.kwargs.copy()
             kwargs["accelerator"] = self.accelerator
             kwargs["layer"] = self.layer
             kwargs["spatial_mapping"] = self.spatial_mapping
-            kwargs["temporal_mapping"] = tm
-            sub_stage = self.list_of_callables[0](self.list_of_callables[1:], **kwargs)
+            kwargs["temporal_mapping"] = temporal_mapping
+            sub_stage: Stage = self.list_of_callables[0](self.list_of_callables[1:], **kwargs)
             for cme, extra_info in sub_stage.run():
-                yield cme, (tm, extra_info)
+                yield cme, (temporal_mapping, extra_info)
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/stages/ONNXModelParserStage.py` & `zigzag_dse-3.1.1/zigzag/stages/ONNXModelParserStage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,29 @@
-from typing import Generator
+from typing import Any
 
-from zigzag.classes.io.onnx.model import ONNXModelParser
-from zigzag.classes.stages.Stage import Stage
+
+from zigzag.parser.onnx.ONNXModelParser import ONNXModelParser
+from zigzag.stages.Stage import Stage, StageCallable
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 
-## Description missing
 class ONNXModelParserStage(Stage):
-    def __init__(self, list_of_callables, *, workload, mapping, **kwargs):
+
+    def __init__(self, list_of_callables: list[StageCallable], *, workload: str, mapping: str, **kwargs: Any):
         super().__init__(list_of_callables, **kwargs)
         self.onnx_model_parser = ONNXModelParser(workload, mapping)
 
-    def run(self) -> Generator:
-        self.onnx_model_parser.run()
-        onnx_model = self.onnx_model_parser.get_onnx_model()
-        workload = self.onnx_model_parser.get_workload()
+    def run(self):
+        workload = self.onnx_model_parser.run()
+        onnx_model = self.onnx_model_parser.onnx_model
 
         sub_stage = self.list_of_callables[0](
             self.list_of_callables[1:],
             onnx_model=onnx_model,
             workload=workload,
-            **self.kwargs
+            **self.kwargs,
         )
         for cme, extra_info in sub_stage.run():
             yield cme, extra_info
-
-    # # For testing purposes
-    # def is_leaf(self) -> bool:
-    #     return True
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/stages/PEArrayScalingStage.py` & `zigzag_dse-3.1.1/zigzag/stages/PEArrayScalingStage.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,48 @@
+"""
+# TODO this file needs to be reworked
+"""
+
 from math import ceil
-from zigzag.classes.hardware.architecture.accelerator import Accelerator
-from zigzag.classes.hardware.architecture.core import Core
-from zigzag.classes.hardware.architecture.memory_hierarchy import MemoryHierarchy
-from zigzag.classes.hardware.architecture.operational_array import OperationalArray
+from typing import Any
+
+from zigzag.cost_model.cost_model import CostModelEvaluation
+from zigzag.hardware.architecture.Accelerator import Accelerator
+from zigzag.hardware.architecture.Core import Core
+from zigzag.hardware.architecture.MemoryHierarchy import MemoryHierarchy
+from zigzag.hardware.architecture.MemoryInstance import MemoryInstance
+from zigzag.hardware.architecture.memory_port import PortAllocation
+from zigzag.hardware.architecture.operational_array import OperationalArray
+from zigzag.hardware.architecture.operational_unit import OperationalUnit
 from zigzag.utils import pickle_deepcopy
-from zigzag.classes.stages.Stage import Stage
+from zigzag.stages.Stage import Stage, StageCallable
 
 import logging
 
 logger = logging.getLogger(__name__)
 
-## This stage scales the PE array of the given accelerator.
-## Because the user-defined spatial mapping resides in the different workload layer nodes,
-## We also have to modify those to scale accordingly
+
 class PEArrayScalingStage(Stage):
+    """! This stage scales the PE array of the given accelerator.
+    Because the user-defined spatial mapping resides in the different workload layer nodes,
+    We also have to modify those to scale accordingly
+    """
+
     def __init__(
-        self, list_of_callables, *, workload, accelerator, pe_array_scaling, **kwargs
+        self,
+        list_of_callables: list[StageCallable],
+        *,
+        workload,
+        accelerator: Accelerator,
+        pe_array_scaling: int,
+        **kwargs: Any,
     ):
         super().__init__(list_of_callables, **kwargs)
 
-        ## SANITY CHECKS
+        # SANITY CHECKS
         # Only allow scaling factors that are a power of 2
         assert pe_array_scaling in [2**i for i in range(-3, 3)]
         # Make sure there's only one core so that the correct one is scaled
         # If your accelerator has more cores, modify the function below
         assert len(accelerator.cores) == 1
 
         self.workload = workload
@@ -58,28 +77,23 @@
                         - memory instance
                         - operands
                         - port allocation
                         - served dimensions
         """
         # Get the relevant accelerator attributes
         core = next(iter(self.accelerator.cores))
-        operational_array = core.operational_array
+        operational_array: OperationalArray = core.operational_array
         operational_unit = operational_array.unit
-        dimension_sizes = operational_array.dimension_sizes
+        dimension_sizes = operational_array.oa_dim_sizes
         memory_hierarchy = core.memory_hierarchy
 
         # Create new operational array
-        new_operational_unit = pickle_deepcopy(operational_unit)
-        new_dimension_sizes = [
-            ceil(self.pe_array_scaling * dim_size) for dim_size in dimension_sizes
-        ]
-        new_dimensions = {
-            f"D{i}": new_dim_size
-            for i, new_dim_size in enumerate(new_dimension_sizes, start=1)
-        }
+        new_operational_unit: OperationalUnit = pickle_deepcopy(operational_unit)
+        new_dimension_sizes = [ceil(self.pe_array_scaling * dim_size) for dim_size in dimension_sizes]
+        new_dimensions = {f"D{i}": new_dim_size for i, new_dim_size in enumerate(new_dimension_sizes, start=1)}
         new_operational_array = OperationalArray(new_operational_unit, new_dimensions)
 
         # Initialize the new memory hierarchy
         mh_name = memory_hierarchy.name
         new_mh_name = mh_name + "-scaled"
         new_memory_hierarchy = MemoryHierarchy(new_operational_array, new_mh_name)
 
@@ -88,40 +102,32 @@
             memory_instance = memory_level.memory_instance
             operands = tuple(memory_level.operands)
             port_alloc = memory_level.port_alloc_raw
             served_dimensions_vec = memory_level.served_dimensions_vec
             assert len(served_dimensions_vec) >= 1
             served_dimensions = served_dimensions_vec[0]
 
-            new_memory_instance = pickle_deepcopy(memory_instance)
-            new_operands = pickle_deepcopy(operands)
-            new_port_alloc = pickle_deepcopy(port_alloc)
+            new_memory_instance: MemoryInstance = pickle_deepcopy(memory_instance)
+            new_operands: tuple[str] = pickle_deepcopy(operands)
+            new_port_alloc: PortAllocation = pickle_deepcopy(port_alloc)
             new_served_dimensions = pickle_deepcopy(served_dimensions)
             new_memory_hierarchy.add_memory(
                 memory_instance=new_memory_instance,
                 operands=new_operands,
                 port_alloc=new_port_alloc,
                 served_dimensions=new_served_dimensions,
             )
 
         # Create the new core
         id = core.id
-        dataflows = core.dataflows
-        if dataflows is not None:
-            raise NotImplementedError(
-                "Scale your core-defined dataflows accordingly here."
-            )
-
         new_id = id
-        new_dataflows = pickle_deepcopy(dataflows)
         new_core = Core(
             id=new_id,
             operational_array=new_operational_array,
             memory_hierarchy=new_memory_hierarchy,
-            dataflows=new_dataflows,
         )
 
         # Create the new accelerator
         name = self.accelerator.name
         new_name = name + "-scaled"
         new_cores = {new_core}
         new_accelerator = Accelerator(
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/stages/PlotTemporalMappingsStage.py` & `zigzag_dse-3.1.1/zigzag/stages/PlotTemporalMappingsStage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,40 @@
+"""
+# TODO this file needs to be reworked
+"""
+
 import os
 
-from typing import Generator, Any, Tuple
-from zigzag.classes.stages.Stage import Stage
-from zigzag.classes.cost_model.cost_model import CostModelEvaluation
+from typing import Any
+
+
+from zigzag.stages.Stage import Stage, StageCallable
+from zigzag.cost_model.cost_model import CostModelEvaluation
 from zigzag.visualization.results.plot_cme import (
     bar_plot_cost_model_evaluations_breakdown,
 )
 
-## Class that passes through all results yielded by substages, but keeps the TMs cme's and saves a plot.
+
 class PlotTemporalMappingsStage(Stage):
+    """! Class that passes through all results yielded by substages, but keeps the TMs cme's and saves a plot."""
 
-    ## The class constructor
-    # @param list_of_callables: see Stage
-    # @param dump_filename_pattern: filename string formatting pattern, which can use named field whose values will be
-    # in kwargs (thus supplied by higher level runnables)
-    # @param kwargs: any kwargs, passed on to substages and can be used in dump_filename_pattern
-    def __init__(self, list_of_callables, *, plot_filename_pattern, **kwargs):
+    def __init__(self, list_of_callables: list[StageCallable], *, plot_filename_pattern: str, **kwargs: Any):
+        """
+        @param list_of_callables: see Stage
+        @param dump_filename_pattern: filename string formatting pattern, which can use named field whose values will be
+        in kwargs (thus supplied by higher level runnables)
+        @param kwargs: any kwargs, passed on to substages and can be used in dump_filename_pattern
+        """
         super().__init__(list_of_callables, **kwargs)
         self.plot_filename_pattern = plot_filename_pattern
 
-    ## Run the compare stage by comparing a new cost model output with the current best found result.
-    def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
+    def run(self):
+        """! Run the compare stage by comparing a new cost model output with the current best found result."""
         substage = self.list_of_callables[0](self.list_of_callables[1:], **self.kwargs)
-        cmes = []
+        cmes: list[CostModelEvaluation] = []
         filename = self.plot_filename_pattern
         for cme, extra_info in substage.run():
+            assert isinstance(cme, CostModelEvaluation)
             cmes.append(cme)
             yield cme, extra_info
         os.makedirs(os.path.dirname(filename), exist_ok=True)
         bar_plot_cost_model_evaluations_breakdown(cmes, filename)
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/stages/ReduceStages.py` & `zigzag_dse-3.1.1/zigzag/stages/reduce_stages.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,145 +1,136 @@
 import logging
 
-from typing import Generator, Tuple, Any
-from zigzag.classes.stages.Stage import Stage
-from zigzag.classes.cost_model.cost_model import CostModelEvaluation
+from typing import Any
+
+
+from zigzag.stages.Stage import Stage, StageCallable
+from zigzag.cost_model.cost_model import CostModelEvaluation, CumulativeCME
 
 logger = logging.getLogger(__name__)
 
-## Class that keeps yields only the cost model evaluation that has minimal energy of all cost model evaluations
-# generated by it's substages created by list_of_callables
+
 class MinimalEnergyStage(Stage):
+    """! Class that keeps yields only the cost model evaluation that has minimal energy of all cost model evaluations
+    generated by it's substages created by list_of_callables
+    """
 
-    ## The class constructor
-    # Initialize the compare stage.
     def __init__(
-        self, list_of_callables, *, reduce_minimal_keep_others=False, **kwargs
+        self, list_of_callables: list[StageCallable], *, reduce_minimal_keep_others: bool = False, **kwargs: Any
     ):
+        """
+        Initialize the compare stage.
+        """
         super().__init__(list_of_callables, **kwargs)
-        self.best_cme = None
         # Visualization stuff
-        self.energies = []
+        self.energies: list[float] = []
         self.keep_others = reduce_minimal_keep_others
 
-    ## Run the compare stage by comparing a new cost model output with the current best found result.
-    def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
+    def run(self):
+        """! Run the compare stage by comparing a new cost model output with the current best found result."""
         sub_list_of_callables = self.list_of_callables[1:]
-        substage = self.list_of_callables[0](sub_list_of_callables, **self.kwargs)
+        substage: Stage = self.list_of_callables[0](sub_list_of_callables, **self.kwargs)
 
-        other_cmes = []
+        other_cmes: list[tuple[CostModelEvaluation, Any]] = []
+        best_cme: CostModelEvaluation | None = None
         for cme, extra_info in substage.run():
+            assert isinstance(cme, CostModelEvaluation)
             self.energies.append(cme.energy_total)
             if (
-                self.best_cme is None
-                or cme.energy_total < self.best_cme.energy_total
-                or (
-                    cme.energy_total == self.best_cme.energy_total
-                    and cme.latency_total2 < self.best_cme.latency_total2
-                )
+                best_cme is None
+                or cme.energy_total < best_cme.energy_total
+                or (cme.energy_total == best_cme.energy_total and cme.latency_total2 < best_cme.latency_total2)
             ):
-                self.best_cme = cme
+                best_cme = cme
             if self.keep_others:
                 other_cmes.append((cme, extra_info))
-        yield (self.best_cme, other_cmes)
 
-## Class that keeps yields only the cost model evaluation that has minimal latency of all cost model evaluations
-# generated by it's substages created by list_of_callables
+        assert best_cme is not None
+        yield best_cme, other_cmes
+
+
 class MinimalLatencyStage(Stage):
+    """! Class that keeps yields only the cost model evaluation that has minimal latency of all cost model evaluations
+    generated by it's substages created by list_of_callables
+    """
 
-    ## The class constructor
-    # Initialize the compare stage.
     def __init__(
-        self, list_of_callables, *, reduce_minimal_keep_others=False, **kwargs
+        self, list_of_callables: list[StageCallable], *, reduce_minimal_keep_others: bool = False, **kwargs: Any
     ):
+        """
+        Initialize the compare stage.
+        """
         super().__init__(list_of_callables, **kwargs)
-        self.best_cme = None
         self.keep_others = reduce_minimal_keep_others
 
-    ## Run the compare stage by comparing a new cost model output with the current best found result.
-    def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
+    def run(self):
+        """! Run the compare stage by comparing a new cost model output with the current best found result."""
         sub_list_of_callables = self.list_of_callables[1:]
-        substage = self.list_of_callables[0](sub_list_of_callables, **self.kwargs)
+        substage: Stage = self.list_of_callables[0](sub_list_of_callables, **self.kwargs)
 
-        other_cmes = []
+        other_cmes: list[tuple[CostModelEvaluation, Any]] = []
+        best_cme: CostModelEvaluation | None = None
         for cme, extra_info in substage.run():
+            assert isinstance(cme, CostModelEvaluation)
             if (
-                self.best_cme is None
-                or cme.latency_total2 < self.best_cme.latency_total2
-                or (
-                    cme.latency_total2 == self.best_cme.latency_total2
-                    and cme.energy_total < self.best_cme.energy_total
-                )
+                best_cme is None
+                or cme.latency_total2 < best_cme.latency_total2
+                or (cme.latency_total2 == best_cme.latency_total2 and cme.energy_total < best_cme.energy_total)
             ):
-                self.best_cme = cme
+                best_cme = cme
             if self.keep_others:
                 other_cmes.append((cme, extra_info))
-        yield (self.best_cme, other_cmes)
 
-## Class that keeps yields only the cost model evaluation that has minimal EDP of all cost model evaluations
-# generated by it's substages created by list_of_callables
+        assert best_cme is not None
+        yield best_cme, other_cmes
+
+
 class MinimalEDPStage(Stage):
+    """! Class that keeps yields only the cost model evaluation that has minimal EDP of all cost model evaluations
+    generated by it's substages created by list_of_callables
+    """
 
-    ## The class constructor
-    # Initialize the compare stage.
     def __init__(
-        self, list_of_callables, *, reduce_minimal_keep_others=False, **kwargs
-    ):
+        self, list_of_callables: list[StageCallable], *, reduce_minimal_keep_others: bool = False, **kwargs: Any
+    ) -> None:
+        """
+        Initialize the compare stage.
+        """
         super().__init__(list_of_callables, **kwargs)
-        self.best_cme = None
         self.keep_others = reduce_minimal_keep_others
 
-    ## Run the compare stage by comparing a new cost model output with the current best found result.
-    def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
+    def run(self):
+        """! Run the compare stage by comparing a new cost model output with the current best found result."""
         sub_list_of_callables = self.list_of_callables[1:]
-        substage = self.list_of_callables[0](sub_list_of_callables, **self.kwargs)
+        substage: Stage = self.list_of_callables[0](sub_list_of_callables, **self.kwargs)
 
-        other_cmes = []
+        other_cmes: list[tuple[CostModelEvaluation, Any]] = []
+        best_cme: CostModelEvaluation | None = None
         for cme, extra_info in substage.run():
+            assert isinstance(cme, CostModelEvaluation)
             if (
-                self.best_cme is None
-                or cme.latency_total2 * cme.energy_total
-                < self.best_cme.latency_total2 * self.best_cme.energy_total
+                best_cme is None
+                or cme.latency_total2 * cme.energy_total < best_cme.latency_total2 * best_cme.energy_total
             ):
-                self.best_cme = cme
+                best_cme = cme
             if self.keep_others:
                 other_cmes.append((cme, extra_info))
-        yield (self.best_cme, other_cmes)
 
-## Class that keeps yields only the sum of all cost model evaluations generated by its
-# substages created by list_of_callables
-class SumStage(Stage):
+        assert best_cme is not None
+        yield best_cme, other_cmes
 
-    ## Initialize the compare stage.
-    def __init__(self, list_of_callables, **kwargs):
-        super().__init__(list_of_callables, **kwargs)
-        self.total_cme = None
 
-    ## Run the compare stage by comparing a new cost model output with the current best found result.
-    def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
-        substage = self.list_of_callables[0](self.list_of_callables[1:], **self.kwargs)
-
-        all_cmes = []
-        for cme, extra_info in substage.run():
-            if self.total_cme is None:
-                self.total_cme = cme
-            else:
-                self.total_cme += cme
-            all_cmes.append((cme, extra_info))
-        yield self.total_cme, all_cmes
-
-
-## Class yields all the cost model evaluations yielded by its substages as a single list instead of as a generator.
-class ListifyStage(Stage):
-
-    ## Initialize the compare stage.
-    def __init__(self, list_of_callables, **kwargs):
-        super().__init__(list_of_callables, **kwargs)
-        self.list = []
+class SumStage(Stage):
+    """! Class that keeps yields only the sum of all cost model evaluations generated by its substages created by
+    list_of_callables.
+    """
 
-    ## Run the compare stage by comparing a new cost model output with the current best found result.
-    def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
-        substage = self.list_of_callables[0](self.list_of_callables[1:], **self.kwargs)
+    def run(self):
+        substage: Stage = self.list_of_callables[0](self.list_of_callables[1:], **self.kwargs)
 
+        all_cmes: list[tuple[CostModelEvaluation, Any]] = []
+        total_cme = CumulativeCME()
         for cme, extra_info in substage.run():
-            self.list.append((cme, extra_info))
-        yield self.list, None
+            assert isinstance(cme, CostModelEvaluation)
+            total_cme += cme
+            all_cmes.append((cme, extra_info))
+        yield total_cme, all_cmes
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/stages/RemoveUnusedMemoryStage.py` & `zigzag_dse-3.1.1/zigzag/stages/RemoveUnusedMemoryStage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,216 +1,198 @@
-from zigzag.classes.hardware.architecture.accelerator import Accelerator
-from zigzag.classes.hardware.architecture.core import Core
-from zigzag.classes.hardware.architecture.memory_hierarchy import MemoryHierarchy
-from zigzag.utils import pickle_deepcopy
-from zigzag.classes.stages.Stage import Stage
-from typing import Generator
+"""
+# TODO this file needs to be reworked
+"""
 
+from typing import Any
 import logging
 
-logger = logging.getLogger(__name__)
 
-#################### Description ####################
-## This stage must be processed behind WorkloadStage.
-## This stage removes unused memory level found by SearchUnusedMemoryStage.
-################### Pseudo-code ####################
-## Initialization:
-##  target_act_mem_level, target_output_mem_level: get from mem_update_list
-##  target_const_mem_level = mem_udpate_weight
-## 1. Modify mem structure:
-## for mem in mem_levels(sort_order: from bottom to top):
-##   if ['I'] in mem.served_operand and mem.mem_level > target_act_mem_level:
-##     remove ['I'] in mem.served_operand, mem_port_alloc
-##   if ['O'] in mem.served_operand and mem.mem_level > target_output_mem_level:
-##     remove ['O'] in mem.served_operand, mem_port_alloc
-##   if ['W'] in mem.served_operand and mem.mem_level > target_const_mem_level:
-##     remove ['W'] in mem.served_operand, mem_port_alloc
-## 2. Remove unused memory
-## for mem in mem_levels(sort_order: from top to bottom):
-##   if mem.served_operand == empty:
-##     do not add the current mem into the modified architecture
-#####################################################
+from zigzag.datatypes import LayerOperand
+from zigzag.hardware.architecture.Accelerator import Accelerator
+from zigzag.hardware.architecture.Core import Core
+from zigzag.hardware.architecture.MemoryHierarchy import MemoryHierarchy
+from zigzag.hardware.architecture.MemoryInstance import MemoryInstance
+from zigzag.hardware.architecture.memory_level import ServedMemDimensions
+from zigzag.workload.layer_node import LayerNode
+from zigzag.utils import pickle_deepcopy
+from zigzag.stages.Stage import Stage, StageCallable
+
+logger = logging.getLogger(__name__)
 
 
 class RemoveUnusedMemoryStage(Stage):
+    """! # ########## Description ##########
+    # # This stage must be processed behind WorkloadStage.
+    # # This stage removes unused memory level found by SearchUnusedMemoryStage.
+    # ######### Pseudo-code ##########
+    # # Initialization:
+    # #  target_act_mem_level, target_output_mem_level: get from mem_update_list
+    # #  target_const_mem_level = mem_udpate_weight
+    # # 1. Modify mem structure:
+    # # for mem in mem_levels(sort_order: from bottom to top):
+    # #   if ['I'] in mem.served_operand and mem.mem_level > target_act_mem_level:
+    # #     remove ['I'] in mem.served_operand, mem_port_alloc
+    # #   if ['O'] in mem.served_operand and mem.mem_level > target_output_mem_level:
+    # #     remove ['O'] in mem.served_operand, mem_port_alloc
+    # #   if ['W'] in mem.served_operand and mem.mem_level > target_const_mem_level:
+    # #     remove ['W'] in mem.served_operand, mem_port_alloc
+    # # 2. Remove unused memory
+    # # for mem in mem_levels(sort_order: from top to bottom):
+    # #   if mem.served_operand == empty:
+    # #     do not add the current mem into the modified architecture
+    # TODO requires cleanup
+    """
+
     def __init__(
         self,
-        list_of_callables,
+        list_of_callables: list[StageCallable],
         *,
-        accelerator,
-        layer,
+        accelerator: Accelerator,
+        layer: LayerNode,
         mem_update_list,
         mem_update_weight,
-        layer_list,
-        **kwargs,
+        layer_list: dict[LayerNode, int],
+        **kwargs: Any,
     ):
         super().__init__(list_of_callables, **kwargs)
         self.accelerator = accelerator
         self.layer = layer
         self.layer_list = layer_list
         self.mem_update_list = mem_update_list
         self.mem_update_weight = mem_update_weight
 
-    def run(self) -> Generator:
+    def run(self):
         modified_accelerator = self.generate_accelerator_with_removing_unused_memory()
         sub_stage = self.list_of_callables[0](
             self.list_of_callables[1:],
             accelerator=modified_accelerator,
             layer=self.layer,
             **self.kwargs,
         )
         for cme, extra_info in sub_stage.run():
             yield cme, extra_info
 
-    def generate_accelerator_with_removing_unused_memory(self):
-        ## Remove nouse memory level according to update_mem_list and mem_update_weight
-        curr_id = self.layer_list[
-            self.layer
-        ]  # current layer id (key) in mem_udpate_list
-        curr_id = str(curr_id)
-        output_operand = self.layer.memory_operand_links[
-            self.layer.output_operand
-        ]  # output representation in memory
+    def generate_accelerator_with_removing_unused_memory(self) -> Accelerator:
+        """
+        # Todo cleanup
+        """
+        # Remove no-use memory level according to update_mem_list and mem_update_weight
+        curr_id: int = self.layer_list[self.layer]
+        output_operand = self.layer.memory_operand_links[self.layer.output_operand]
         core = next(iter(self.accelerator.cores))
         operational_array = core.operational_array
         memory_hierarchy = core.memory_hierarchy
 
         if len(self.layer.constant_operands) == 1:
+            # act representation in memory
             act_operand = self.layer.memory_operand_links[
-                [
-                    operand
-                    for operand in self.layer.input_operands
-                    if operand not in self.layer.constant_operands
-                ][0]
-            ]  # act representation in memory
+                [operand for operand in self.layer.input_operands if operand not in self.layer.constant_operands][0]
+            ]
             const_operand = self.layer.memory_operand_links[
                 self.layer.constant_operands[0]
             ]  # weight representation in memory
         elif len(self.layer.constant_operands) == 0:
             # special case when defining workload manually:
             # the constant operands list is empty for such as "Adder" layers
-            # for input operand, we will represent all inputs as one input, since only their data size is used for required mem size calculation.
-            act_operand = self.layer.memory_operand_links[
-                self.layer.input_operands[0]
-            ]  # act representation in memory
+            # for input operand, we will represent all inputs as one input, since only their data size is used for
+            # required mem size calculation.
+            act_operand = self.layer.memory_operand_links[self.layer.input_operands[0]]  # act representation in memory
             const_operand = self.layer.memory_operand_links[
                 self.layer.input_operands[1]
             ]  # weight representation in memory
         else:
             # special case when defining workload manually:
             # both I and W are considered as constant operands for the first layer
             pr_loop_keys = tuple(self.layer.pr_loop.keys())
-            for (
-                operand,
-                related_loop,
-            ) in self.layer.operand_dimensionality_order.items():
+            related_loop_dict = {
+                layer_op: self.layer.equation.get_r_layer_dims(layer_op)
+                for layer_op in self.layer.equation.get_contained_operands()
+            }
+            act_operand: LayerOperand | None = None
+            for operand, related_loop in related_loop_dict.items():
                 if pr_loop_keys[0] in related_loop:
                     act_operand = operand
-            weight_operand: list = [
-                x for x in self.layer.constant_operands if x != act_operand
-            ]  # weight representation in layer
-            assert len(weight_operand) == 1
-            weight_operand: str = weight_operand[0]
-            act_operand = self.layer.memory_operand_links[
-                act_operand
-            ]  # map from layer representation to hardware memory representation
-            const_operand = self.layer.memory_operand_links[
-                weight_operand
-            ]  # weight representation in memory
+            # weight representation in layer
+            assert act_operand is not None
+            weight_operand_temp: list[LayerOperand] = [x for x in self.layer.constant_operands if x != act_operand]
+            assert len(weight_operand_temp) == 1
+            weight_operand: LayerOperand = weight_operand_temp[0]
+            # map from layer representation to hardware memory representation
+            act_operand = self.layer.memory_operand_links[act_operand]
+            # weight representation in memory
+            const_operand = self.layer.memory_operand_links[weight_operand]
 
         # Find target_act/const/output_mem_level
         for pos, ele in enumerate(self.mem_update_list[curr_id]):
             if list(ele.keys())[0] == act_operand:
                 target_act_mem_level = self.mem_update_list[curr_id][pos][act_operand]
             if list(ele.keys())[0] == output_operand:
-                target_output_mem_level = self.mem_update_list[curr_id][pos][
-                    output_operand
-                ]
-        if len(self.layer.constant_operands) == 0:
+                target_output_mem_level = self.mem_update_list[curr_id][pos][output_operand]
+        if self.layer.constant_operands is None or len(self.layer.constant_operands) == 0:
             # special case when defining workload manually:
             # the constant operands list is empty for such as "Adder" layers
             # Here we make a trick: treating the other input as const_operand
             for pos, ele in enumerate(self.mem_update_list[curr_id]):
                 if list(ele.keys())[0] == act_operand:
-                    target_const_mem_level = self.mem_update_list[curr_id][pos][
-                        act_operand
-                    ]
+                    target_const_mem_level = self.mem_update_list[curr_id][pos][act_operand]
         else:
             target_const_mem_level = self.mem_update_weight
 
         # Initialize the new memory hierarchy
         mh_name = memory_hierarchy.name
         new_mh_name = mh_name + "-without-unused-memory"
         new_memory_hierarchy = MemoryHierarchy(operational_array, new_mh_name)
 
         # Add memories to the new memory hierarchy with the correct attributes
         for curr_mem_level, memory_level in enumerate(memory_hierarchy.mem_level_list):
             memory_instance = memory_level.memory_instance
             operands = tuple(memory_level.operands)
             port_alloc = memory_level.port_alloc_raw
-            served_dimensions_vec = memory_level.served_dimensions_vec
-            assert len(served_dimensions_vec) >= 1
-            served_dimensions = served_dimensions_vec[0]
+            served_dimensions = memory_level.served_dimensions
 
-            new_memory_instance = pickle_deepcopy(memory_instance)
+            new_memory_instance: MemoryInstance = pickle_deepcopy(memory_instance)  # type: ignore
             new_operands = []
             new_port_alloc = []
             if (act_operand in operands) and curr_mem_level <= target_act_mem_level:
                 new_operands.append(act_operand)
                 index_in_operands = operands.index(act_operand)
                 new_port_alloc.append(port_alloc[index_in_operands])
             if (const_operand in operands) and curr_mem_level <= target_const_mem_level:
                 new_operands.append(const_operand)
                 index_in_operands = operands.index(const_operand)
                 new_port_alloc.append(port_alloc[index_in_operands])
-            if (
-                output_operand in operands
-            ) and curr_mem_level <= target_output_mem_level:
+            if (output_operand in operands) and curr_mem_level <= target_output_mem_level:
                 new_operands.append(output_operand)
                 index_in_operands = operands.index(output_operand)
                 new_port_alloc.append(port_alloc[index_in_operands])
             new_operands = tuple(new_operands)
             new_port_alloc = tuple(new_port_alloc)
-            new_served_dimensions = pickle_deepcopy(served_dimensions)
+            new_served_dimensions: ServedMemDimensions = pickle_deepcopy(served_dimensions)
             if len(new_operands) > 0:
                 new_memory_hierarchy.add_memory(
                     memory_instance=new_memory_instance,
                     operands=new_operands,
                     port_alloc=new_port_alloc,
-                    served_dimensions=new_served_dimensions,
+                    served_dimensions=new_served_dimensions.to_user_format(),
                 )
 
         # Create the new core
         id = core.id
-        dataflows = core.dataflows
         new_id = id
-        new_dataflows = pickle_deepcopy(dataflows)
         new_core = Core(
             id=new_id,
             operational_array=operational_array,
             memory_hierarchy=new_memory_hierarchy,
-            dataflows=new_dataflows,
         )
 
         # Create the new accelerator
         name = self.accelerator.name
         new_name = name + "-removing-nouse-mem"
         new_cores = {new_core}
         new_accelerator = Accelerator(
             name=new_name,
             core_set=new_cores,
         )
 
         logger.info(f"Update mem architecture for layer {self.layer}...")
 
-        # RemoveUnusedMemoryStage.visulize_modified_memory_structure(new_memory_hierarchy)
-
         return new_accelerator
-
-    @staticmethod
-    def visulize_modified_memory_structure(new_memory_hierarchy):
-        # Visualization for debugging
-        from zigzag.visualization.graph.memory_hierarchy import (
-            visualize_memory_hierarchy_graph,
-        )
-
-        visualize_memory_hierarchy_graph(new_memory_hierarchy)
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/stages/RunOptStages.py` & `zigzag_dse-3.1.1/zigzag/stages/run_opt_stages.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,65 @@
-from typing import Generator, Tuple, Any
-from zigzag.classes.stages.Stage import Stage
-from zigzag.classes.cost_model.cost_model import CostModelEvaluation
+from typing import Any, Callable
+
+
+from zigzag.cost_model.cost_model import CostModelEvaluationABC
+from zigzag.stages.Stage import Stage, StageCallable
 
 import logging
 import os
 
 logger = logging.getLogger(__name__)
 
-## Strips extra info for subcallables to save memory
+
 class RemoveExtraInfoStage(Stage):
+    """! Strips extra info for subcallables to save memory"""
 
-    ## The class constructor
-    # Initialize the remove extra info stage.
-    def __init__(self, list_of_callables, **kwargs):
+    def __init__(self, list_of_callables: list[StageCallable], **kwargs: Any):
+        """
+        Initialize the remove extra info stage.
+        """
         super().__init__(list_of_callables, **kwargs)
 
-    ## Run the remove extra info stage by running the substage and discarding the extra_info.
-    def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
+    def run(self):
+        """! Run the remove extra info stage by running the substage and discarding the extra_info."""
         sub_list_of_callables = self.list_of_callables[1:]
         substage = self.list_of_callables[0](sub_list_of_callables, **self.kwargs)
 
-        for cme, extra_info in substage.run():
+        for cme, _ in substage.run():
             yield cme, None
 
 
-## Caches results in a list and then yields them.
-# This breaks the yield flow from top to bottom.
 class CacheBeforeYieldStage(Stage):
-
-    ## The class constructor
-    # Initialize the cache before yield stage.
-    def __init__(self, list_of_callables, **kwargs):
+    """! Caches results in a list and then yields them.
+    This breaks the yield flow from top to bottom.
+    """
+
+    def __init__(self, list_of_callables: list[StageCallable], **kwargs: Any):
+        """
+        Initialize the cache before yield stage.
+        """
         super().__init__(list_of_callables, **kwargs)
 
-    ## Run the cache before yield stage by running the substage and caching everything it yields, then yielding everything.
-    def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
+    def run(self):
+        """! Run the cache before yield stage by running the substage and caching everything it yields, then yielding everything."""
         sub_list_of_callables = self.list_of_callables[1:]
         substage = self.list_of_callables[0](sub_list_of_callables, **self.kwargs)
 
-        to_yield = []
+        to_yield: list[tuple[CostModelEvaluationABC, Any]] = []
         for ty in substage.run():
             to_yield.append(ty)
         for ty in to_yield:
             yield ty
 
 
-## Check if the output file is already generated, skip the run if so.
 class SkipIfDumpExistsStage(Stage):
+    """! Check if the output file is already generated, skip the run if so."""
 
-    ## The class constructor
-    def __init__(self, list_of_callables, *, dump_filename_pattern, **kwargs):
+    def __init__(self, list_of_callables: list[StageCallable], *, dump_filename_pattern: str, **kwargs: Any):
+        """"""
         super().__init__(list_of_callables, **kwargs)
         self.dump_filename_pattern = dump_filename_pattern
 
     def run(self):
         filename = self.dump_filename_pattern.format(**self.kwargs)
         if os.path.isfile(filename):
             print(
@@ -71,109 +77,110 @@
 
 import multiprocessing
 
 
 threadpool = None
 
 
-def get_threadpool(nb_threads_if_non_existent):
+def get_threadpool(nb_threads_if_non_existent: int | None):
     global threadpool
     if threadpool is None:
         threadpool = multiprocessing.Pool(nb_threads_if_non_existent)
     return threadpool
 
 
 def close_threadpool():
     global threadpool
-    threadpool.close()
+    if threadpool is not None:
+        threadpool.close()
     threadpool = None
 
 
 def terminate_threadpool():
     global threadpool
-    threadpool.terminate()
+    if threadpool is not None:
+        threadpool.terminate()
     threadpool = None
 
 
 def raise_exception(e):
     terminate_threadpool()
     raise e
 
 
-## Multiprocessing support stage.
-# 
-# Warning: does not yield (CostModelEvaluation, extra_info) pairs.
-#
-# Use as follows in a list_of_callables:
-# - [..., ..., MultiProcessingGatherStage, some stage(s) that loop over stuff and just yield (cme, extra_info) pairs
-#     every iteration without postprocessing it, MultiProcessingSpawnStage, ..., ...]
-# 
-# Note: list of callables may not contain lambda functions, as this will break pickling which is required for
-#         by multiprocessing
-# 
-# Note: there is quite some overhead in spawning these parallel processes (python...; it needs to copy through pickle
-#         all variables), so best to do this at some high level loop (early in list of callables)
 class MultiProcessingSpawnStage(Stage):
+    """! Multiprocessing support stage.
+
+    Warning: does not yield (CostModelEvaluation, extra_info) pairs.
+
+    Use as follows in a list_of_callables:
+    - [..., ..., MultiProcessingGatherStage, some stage(s) that loop over stuff and just yield (cme, extra_info) pairs
+        every iteration without postprocessing it, MultiProcessingSpawnStage, ..., ...]
+
+    Note: list of callables may not contain lambda functions, as this will break pickling which is required for
+            by multiprocessing
+
+    Note: there is quite some overhead in spawning these parallel processes (python...; it needs to copy through pickle
+            all variables), so best to do this at some high level loop (early in list of callables)
+    """
 
-    ## The class constructor
-    # @param list_of_callables: may not contain lambda functions, as this will break pickling which is required for
-    # by multiprocessing.
-    # @param multiprocessing_callback: intended to be set by MultiProcessingGatherStage
-    # @param kwargs:
     def __init__(
         self,
-        list_of_callables,
+        list_of_callables: list[StageCallable],
         *,
-        multiprocessing_callback,
-        nb_multiprocessing_threads=multiprocessing.cpu_count(),
-        **kwargs,
+        multiprocessing_callback: Callable[[object], None],
+        nb_multiprocessing_threads: int = multiprocessing.cpu_count(),
+        **kwargs: Any,
     ):
+        """
+        @param list_of_callables: may not contain lambda functions, as this will break pickling which is required for
+        by multiprocessing.
+        @param multiprocessing_callback: intended to be set by MultiProcessingGatherStage
+        @param kwargs:
+        """
         super().__init__(list_of_callables, **kwargs)
         self.nb_multiprocessing_threads = nb_multiprocessing_threads
         self.callback = multiprocessing_callback
 
     def _to_run(self):
         return list(self.sub_stage.run())
 
     def run(self):
-        self.sub_stage = self.list_of_callables[0](
-            self.list_of_callables[1:], **self.kwargs
-        )
+        self.sub_stage = self.list_of_callables[0](self.list_of_callables[1:], **self.kwargs)
         get_threadpool(self.nb_multiprocessing_threads).apply_async(
             self._to_run, callback=self.callback, error_callback=raise_exception
         )
         yield None, None
 
 
-## Multiprocessing support stage.
-# 
-# Use as follows in a list_of_callables:
-# - [..., ..., MultiProcessingGatherStage, some stage(s) that loop over stuff and just yield (cme, extra_info) pairs
-#     every iteration without postprocessing it, MultiProcessingSpawnStage, ..., ...]
-# 
-# Note: list of callables may not contain lambda functions, as this will break pickling which is required for
-#         by multiprocessing
 class MultiProcessingGatherStage(Stage):
+    """! Multiprocessing support stage.
+
+    Use as follows in a list_of_callables:
+    - [..., ..., MultiProcessingGatherStage, some stage(s) that loop over stuff and just yield (cme, extra_info) pairs
+        every iteration without postprocessing it, MultiProcessingSpawnStage, ..., ...]
+
+    Note: list of callables may not contain lambda functions, as this will break pickling which is required for
+            by multiprocessing
+    """
 
-    def _callback(self, ans):
+    def _callback(self, ans: object):
         self.queue.put(ans)
 
     def run(self):
         self.queue = multiprocessing.Manager().Queue()
         kwargs = self.kwargs.copy()
         kwargs["multiprocessing_callback"] = self._callback
 
         sub_stage = self.list_of_callables[0](self.list_of_callables[1:], **kwargs)
         count_to_get = 0
-        for i in sub_stage.run():
+        for _ in sub_stage.run():
             count_to_get += 1
         logger.info(f"Multiprocessing results to get: {count_to_get}")
         count = 0
         while count < count_to_get:
             for ans in self.queue.get(block=True):
                 yield ans
             count += 1
             if count % (count_to_get // 10) == 0:
-                logger.info(
-                    f"Multiprocessing results received: {count} of {count_to_get}"
-                )
+                logger.info(f"Multiprocessing results received: {count} of {count_to_get}")
         close_threadpool()
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/stages/SalsaStage.py` & `zigzag_dse-3.1.1/zigzag/stages/SalsaStage.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,94 +22,86 @@
 #   distributed under the License is distributed on an AS IS BASIS, WITHOUT
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
 import multiprocessing_on_dill as multiprocessing
-from sympy.ntheory import factorint
-from copy import deepcopy
 import logging
 
-from zigzag.classes.hardware.architecture.accelerator import Accelerator
-from zigzag.classes.mapping.spatial.spatial_mapping import SpatialMapping
-from zigzag.classes.opt.temporal.salsa.engine import SalsaEngine
-from zigzag.classes.workload.layer_node import LayerNode
-from typing import Generator, Callable, List, Tuple, Any
-from zigzag.classes.stages.Stage import Stage
-from zigzag.classes.cost_model.cost_model import CostModelEvaluation
 
-from zigzag.classes.stages.ReduceStages import MinimalEnergyStage
-from zigzag.classes.stages.ReduceStages import MinimalLatencyStage
+from zigzag.cost_model.cost_model import CostModelEvaluation, CostModelEvaluationABC
+
+from zigzag.hardware.architecture.Accelerator import Accelerator
+from zigzag.mapping.SpatialMappingInternal import SpatialMappingInternal
+from zigzag.opt.salsa.SalsaEngine import SalsaEngine
+from typing import Any
+from zigzag.stages.Stage import Stage, StageCallable
+from zigzag.workload.layer_node import LayerNode
+
 
 logger = logging.getLogger(__name__)
 
-## Class that return the best temporal mapping found by the Simulated Annealing
-# Loop-ordering Scheduler for Accelerators (SALSA) for a single layer.
+
 class SalsaStage(Stage):
+    """! Class that return the best temporal mapping found by the Simulated Annealing
+    Loop-ordering Scheduler for Accelerators (SALSA) for a single layer.
+    """
 
-    ## The class constructor
-    # Initialize the SalsaStage by setting the accelerator, layer, and spatial mapping.
-    # @param list_of_callables (List[Callable]): List of substages to call with each generated temporal mapping.
-    # @param accelerator (Accelerator): The accelerator object.
-    # @param layer (Layer): The layer object.
-    # @param spatial_mapping (SpatialMapping): The spatial mapping object.
     def __init__(
         self,
-        list_of_callables: List[Callable],
+        list_of_callables: list[StageCallable],
         *,
-        accelerator,
-        layer,
-        spatial_mapping,
-        **kwargs,
+        accelerator: Accelerator,
+        layer: LayerNode,
+        spatial_mapping: SpatialMappingInternal,
+        **kwargs: Any,
     ):
+        """
+        Initialize the SalsaStage by setting the accelerator, layer, and spatial mapping.
+        @param list_of_callables (List[Callable]): List of substages to call with each generated temporal mapping.
+        """
         super().__init__(list_of_callables, **kwargs)
         self.accelerator, self.layer, self.spatial_mapping = (
             accelerator,
             layer,
             spatial_mapping,
         )
         self.engine = None
-        self.best_cme = None
+        self.best_cme: CostModelEvaluationABC | None = None
 
         self.opt_criterion_name = kwargs.get("salsa_opt_criterion", "energy")
         self.number_of_core_allocated = kwargs.get("salsa_number_of_core", 1)
 
         # Multiprocessing parameters
         self.worker_list = []
         self.cme_queue = multiprocessing.Queue()
 
         if self.opt_criterion_name == "energy":
             self.compare_stage = self.compare_cme_energy
         elif self.opt_criterion_name == "latency":
             self.compare_stage = self.compare_cme_latency
         else:
-            raise Exception(
-                "Invalid optimization criterion for SALSA. Must be either 'energy' or 'latency'."
-            )
+            raise Exception("Invalid optimization criterion for SALSA. Must be either 'energy' or 'latency'.")
 
     ## Set up and start salsa engine, then collect and return the best cost model evaluation
     def run(self):
 
-        logger.info(
-            f"Running SALSA Temporal Mapping Optimizer with {self.number_of_core_allocated} core(s)."
-        )
+        logger.info(f"Running SALSA Temporal Mapping Optimizer with {self.number_of_core_allocated} core(s).")
 
         self.engine = SalsaEngine(
             accelerator=self.accelerator,
             layer=self.layer,
             spatial_mapping=self.spatial_mapping,
             **self.kwargs,
         )
 
-        # self.best_cme = self.engine.run(self.cme_queue)
-
         # Get the number of core the user wants to allocate
         if self.number_of_core_allocated <= multiprocessing.cpu_count():
-            self.number_of_core = self.number_of_core_allocated
+            self.number_of_core: int = self.number_of_core_allocated
         else:
             self.number_of_core = multiprocessing.cpu_count()
 
         # Create processes
         for core_id in range(0, self.number_of_core):
             p = multiprocessing.Process(target=self.engine.run, args=(self.cme_queue,))
             self.worker_list.append(p)
@@ -134,33 +126,27 @@
         kwargs["spatial_mapping"] = self.spatial_mapping
         kwargs["temporal_mapping"] = self.best_cme.mapping.temporal_mapping
         sub_stage = self.list_of_callables[0](self.list_of_callables[1:], **kwargs)
 
         for cme, extra_info in sub_stage.run():
             yield cme, (self.best_cme.mapping.temporal_mapping, extra_info)
 
-    ## Compare the latency of the current cost model evaluation with the best latency found so far.
-    # Then replace the current best cme if the current cme has a lower latency.
-    def compare_cme_latency(self, cme):
+    def compare_cme_latency(self, cme: CostModelEvaluation):
+        """! Compare the latency of the current cost model evaluation with the best latency found so far.
+        Then replace the current best cme if the current cme has a lower latency."""
 
         if self.best_cme is None:
             self.best_cme = cme
-        elif (
-            cme.latency_total2 == self.best_cme.latency_total2
-            and cme.energy_total < self.best_cme.energy_total
-        ):
+        elif cme.latency_total2 == self.best_cme.latency_total2 and cme.energy_total < self.best_cme.energy_total:
             self.best_cme = cme
         elif cme.latency_total2 < self.best_cme.latency_total2:
             self.best_cme = cme
 
-    ## Compare the energy of the current cost model evaluation with the best energy found so far.
-    # Then replace the best cme if the current cme has a lower energy.
-    def compare_cme_energy(self, cme):
+    def compare_cme_energy(self, cme: CostModelEvaluation):
+        """! Compare the energy of the current cost model evaluation with the best energy found so far.
+        # Then replace the best cme if the current cme has a lower energy."""
         if self.best_cme is None:
             self.best_cme = cme
-        elif (
-            cme.energy_total == self.best_cme.energy_total
-            and cme.latency_total2 < self.best_cme.latency_total2
-        ):
+        elif cme.energy_total == self.best_cme.energy_total and cme.latency_total2 < self.best_cme.latency_total2:
             self.best_cme = cme
         elif cme.energy_total < self.best_cme.energy_total:
             self.best_cme = cme
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/stages/SaveStage.py` & `zigzag_dse-3.1.1/zigzag/stages/save_stages.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,159 +1,136 @@
-from typing import Generator, Any, Tuple
-from zigzag.classes.stages.Stage import Stage
-from zigzag.classes.cost_model.cost_model import CostModelEvaluation
+from typing import Any
 import os
 import pickle
 import json
 import yaml
-import re
-import numpy as np
-
 import logging
 
+from zigzag.cost_model.cost_model import CostModelEvaluation, CostModelEvaluationABC, CumulativeCME
+from zigzag.stages.Stage import Stage, StageCallable
+from zigzag.utils import json_repr_handler
+
 logger = logging.getLogger(__name__)
 
 
-## Class that passes through all results yielded by substages, but saves the results as a json list to a file
-# at the end of the iteration.
 class CompleteSaveStage(Stage):
-
-    ## The class constructor
-    # @param list_of_callables: see Stage
-    # @param dump_filename_pattern: filename string formatting pattern, which can use named field whose values will be
-    # in kwargs (thus supplied by higher level runnables)
-    # @param kwargs: any kwargs, passed on to substages and can be used in dump_filename_pattern
-    def __init__(self, list_of_callables, *, dump_filename_pattern, **kwargs):
+    """! Class that passes through all results yielded by substages, but saves the results as a json list to a file
+    at the end of the iteration.
+    """
+
+    def __init__(self, list_of_callables: list[StageCallable], *, dump_filename_pattern: str, **kwargs: Any):
+        """
+        @param dump_filename_pattern: filename string formatting pattern, which can use named field whose values will be
+        in kwargs (thus supplied by higher level runnables). Must contain `?`
+        @param kwargs: any kwargs, passed on to substages and can be used in dump_filename_pattern
+        """
         super().__init__(list_of_callables, **kwargs)
         self.dump_filename_pattern = dump_filename_pattern
 
-    ## Run the complete save stage by running the substage and saving the CostModelEvaluation json representation.
-    def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
+    def run(self):
+        """! Run the complete save stage by running the substage and saving the CostModelEvaluation json
+        representation."""
         self.kwargs["dump_filename_pattern"] = self.dump_filename_pattern
         substage = self.list_of_callables[0](self.list_of_callables[1:], **self.kwargs)
 
-        for id, (cme, extra_info) in enumerate(substage.run()):
-            cme: CostModelEvaluation
-            # filename = self.dump_filename_pattern.format(datetime=datetime.now().isoformat().replace(":", "-"))
-            if type(cme.layer) == list:
-                filename = self.dump_filename_pattern.replace(
-                    "?", "overall_complete"
-                )
+        for cme, extra_info in substage.run():
+            if isinstance(cme, CumulativeCME):
+                filename = self.dump_filename_pattern.replace("?", "overall_complete")
+            elif isinstance(cme, CostModelEvaluation):
+                filename = self.dump_filename_pattern.replace("?", f"{cme.layer}_complete")
             else:
-                filename = self.dump_filename_pattern.replace(
-                    "?", f"{cme.layer}_complete"
-                )
+                raise NotImplementedError
+
             self.save_to_json(cme, filename=filename)
-            yamlname = os.path.join(os.path.splitext(filename)[0], ".yml")
-            self.save_to_yaml(jsonname=filename, yamlname=yamlname)
+            yaml_name = os.path.join(os.path.splitext(filename)[0], ".yml")
+            self.save_to_yaml(json_name=filename, yaml_name=yaml_name)
             logger.info(
                 f"Saved {cme} with energy {cme.energy_total:.3e} and latency {cme.latency_total2:.3e} to {filename}"
             )
             yield cme, extra_info
 
-    def save_to_json(self, obj, filename):
+    def save_to_json(self, obj: object, filename: str):
         os.makedirs(os.path.dirname(filename), exist_ok=True)
         with open(filename, "w") as fp:
-            json.dump(obj, fp, default=self.complexHandler, indent=4)
+            json.dump(obj, fp, default=json_repr_handler, indent=4)
 
-    def save_to_yaml(self, jsonname, yamlname):
-        os.makedirs(os.path.dirname(yamlname), exist_ok=True)
-        with open(jsonname, "r") as fp:
+    def save_to_yaml(self, json_name: str, yaml_name: str):
+        os.makedirs(os.path.dirname(yaml_name), exist_ok=True)
+        with open(json_name, "r") as fp:
             res = json.load(fp)
-        with open(yamlname, "w") as fp:
+        with open(yaml_name, "w") as fp:
             yaml.dump(res, fp, Dumper=yaml.SafeDumper)
 
-    @staticmethod
-    def complexHandler(obj):
-        # print(type(obj))
-        if isinstance(obj, set):
-            return list(obj)
-        if isinstance(obj, np.int32):
-            return int(obj)
-        if hasattr(obj, "__jsonrepr__"):
-            return obj.__jsonrepr__()
-        else:
-            raise TypeError(
-                f"Object of type {type(obj)} is not serializable. Create a __jsonrepr__ method."
-            )
-
 
-## Class that passes through results yielded by substages, but saves the results as a json list to a file
-# at the end of the iteration.
-# In this simple version, only the energy total and latency total are saved.
 class SimpleSaveStage(Stage):
-
-    ## The class constructor
-    # @param list_of_callables: see Stage
-    # @param dump_filename_pattern: filename string formatting pattern, which can use named field whose values will be
-    # in kwargs (thus supplied by higher level runnables)
-    # @param kwargs: any kwargs, passed on to substages and can be used in dump_filename_pattern
-    def __init__(self, list_of_callables, *, dump_filename_pattern, **kwargs):
+    """! Class that passes through results yielded by substages, but saves the results as a json list to a file
+    at the end of the iteration.
+    In this simple version, only the energy total and latency total are saved.
+    """
+
+    def __init__(self, list_of_callables: list[StageCallable], *, dump_filename_pattern: str, **kwargs: Any):
+        """
+        @param list_of_callables: see Stage
+        @param dump_filename_pattern: filename string formatting pattern, which can use named field whose values will be
+        in kwargs (thus supplied by higher level runnables)
+        @param kwargs: any kwargs, passed on to substages and can be used in dump_filename_pattern
+        """
         super().__init__(list_of_callables, **kwargs)
         self.dump_filename_pattern = dump_filename_pattern
 
-    ## Run the simple save stage by running the substage and saving the CostModelEvaluation simple json representation.
-    def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
+    def run(self):
+        """! Run the simple save stage by running the substage and saving the CostModelEvaluation simple json
+        representation."""
         self.kwargs["dump_filename_pattern"] = self.dump_filename_pattern
         substage = self.list_of_callables[0](self.list_of_callables[1:], **self.kwargs)
 
-        for id, (cme, extra_info) in enumerate(substage.run()):
-            cme: CostModelEvaluation
-            # filename = self.dump_filename_pattern.format(datetime=datetime.now().isoformat().replace(":", "-"))
-            if type(cme.layer) == list:
+        for cme, extra_info in substage.run():
+            if isinstance(cme, CumulativeCME):
                 filename = self.dump_filename_pattern.replace("?", "overall_simple")
+            elif isinstance(cme, CostModelEvaluation):
+                filename = self.dump_filename_pattern.replace("?", f"{cme.layer}_simple")
             else:
-                filename = self.dump_filename_pattern.replace(
-                    "?", f"{cme.layer}_simple"
-                )
+                raise NotImplementedError
             self.save_to_json(cme, filename=filename)
             logger.info(
                 f"Saved {cme} with energy {cme.energy_total:.3e} and latency {cme.latency_total2:.3e} to {filename}"
             )
             yield cme, extra_info
 
-    def save_to_json(self, obj, filename):
+    def save_to_json(self, obj: CostModelEvaluationABC, filename: str):
         os.makedirs(os.path.dirname(filename), exist_ok=True)
-        with open(filename, "w") as fp:
-            json.dump(obj, fp, default=self.complexHandler, indent=4)
+        with open(filename, "w", encoding="UTF-8") as fp:
+
+            def handler(obj: object):
+                return json_repr_handler(obj, simple=True)
+
+            json.dump(obj, fp, default=handler, indent=4)
 
-    @staticmethod
-    def complexHandler(obj):
-        # print(type(obj))
-        if isinstance(obj, set):
-            return list(obj)
-        if isinstance(obj, np.int32):
-            return int(obj)
-        if hasattr(obj, "__simplejsonrepr__"):
-            return obj.__simplejsonrepr__()
-        else:
-            raise TypeError(
-                f"Object of type {type(obj)} is not serializable. Create a __simplejsonrepr__ method."
-            )
 
-## Class that dumps all received CMEs into a list and saves that list to a pickle file.
 class PickleSaveStage(Stage):
+    """! Class that dumps all received CMEs into a list and saves that list to a pickle file."""
 
-    ## The class constructor
-    # @param list_of_callables: see Stage
-    # @param pickle_filename: output pickle filename
-    # @param kwargs: any kwargs, passed on to substages and can be used in dump_filename_pattern
-    def __init__(self, list_of_callables, *, pickle_filename, **kwargs):
+    def __init__(self, list_of_callables: list[StageCallable], *, pickle_filename: str, **kwargs: Any):
+        """
+        @param list_of_callables: see Stage
+        @param pickle_filename: output pickle filename
+        @param kwargs: any kwargs, passed on to substages and can be used in dump_filename_pattern
+        """
         super().__init__(list_of_callables, **kwargs)
         self.pickle_filename = pickle_filename
 
-    ## Run the simple save stage by running the substage and saving the CostModelEvaluation simple json representation.
-    # This should be placed above a ReduceStage such as the SumStage, as we assume the list of CMEs is passed as extra_info
-    def run(self) -> Generator[Tuple[CostModelEvaluation, Any], None, None]:
+    def run(self):
+        """! Run the simple save stage by running the substage and saving the CostModelEvaluation simple json representation.
+        This should be placed above a ReduceStage such as the SumStage, as we assume the list of CMEs is passed as extra_info
+        """
         substage = self.list_of_callables[0](self.list_of_callables[1:], **self.kwargs)
-        for id, (cme, extra_info) in enumerate(substage.run()):
-            all_cmes = [cme for (cme, extra) in extra_info]
+        for cme, extra_info in substage.run():
+            all_cmes: list[CostModelEvaluation] = [cme for (cme, _) in extra_info]
             yield cme, extra_info
+
         # After we have received all the CMEs, save them to the specified output location.
         dirname = os.path.dirname(self.pickle_filename)
         if not os.path.exists(dirname):
             os.makedirs(dirname)
         with open(self.pickle_filename, "wb") as handle:
             pickle.dump(all_cmes, handle, protocol=pickle.HIGHEST_PROTOCOL)
-        logger.info(
-            f"Saved pickled list of {len(all_cmes)} CMEs to {self.pickle_filename}."
-        )
+        logger.info(f"Saved pickled list of {len(all_cmes)} CMEs to {self.pickle_filename}.")
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/stages/SearchUnusedMemoryStage.py` & `zigzag_dse-3.1.1/zigzag/stages/SearchUnusedMemoryStage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,525 +1,458 @@
-from zigzag.classes.stages.Stage import Stage
+from typing import Any, Generator
+from zigzag.cost_model.cost_model import CostModelEvaluation
+from zigzag.datatypes import LayerDim, LayerOperand, MemoryOperand
+
+from zigzag.hardware.architecture.Accelerator import Accelerator
+from zigzag.hardware.architecture.memory_level import MemoryLevel
+from zigzag.stages.Stage import Stage, StageCallable
 
 import networkx as nx
-from typing import Generator
-from zigzag.classes.workload.dummy_node import DummyNode
+from zigzag.workload.Workload import Workload
+from zigzag.workload.DummyNode import DummyNode
 
 import logging
 
+from zigzag.workload.layer_node import LayerNode
+
 logger = logging.getLogger(__name__)
 
-#################### Description ####################
-## This stage must be processed before WorkloadStage.
-## This stage figures out the unused memory levels for "I", "W", "O" when the size of lower memory level is enough to hold all data, considering the output data of previous layer can be directly used by next layer. As an impact, the energy / latency related to these memories will be removed.
-## The general criteria is:
-##      If a low-level memory size is big enough to hold both "I" and "O" data of current layer, memory above this one will be labeled as unused.
-##      If a low-level memory size is big enough to hold "W" data of entire workload, memory above this one will be labeled as unused.
-## The above method only applies layers along the same branch, otherwise (for branch starting nodes or branch final nodes) the "O" data will return back to the top possible memory.
-## In RemoveNoUseMemStage, unused mem across all layers, labeled in this stage, will be removed in the memory architecture.
-## For now, the number of cores must be 1.
-#################### Pseudo-code ####################
-## Initialization:
-##   mem_update_list = [layer_ids: {"I" / "O": -1}] ## mem level of different operands of each layer (there should be no -1 after self.update_top_mem_level())
-##   each_layer_IO_data_size = [layer_ids: {"I" / "O": size}] ## input / output data size of each layer
-##   mem_update_weight = top_mem_level ## top mem level to put weight
-##   weight_size_entire_workload = weight_size # weight data size of entire workload
-## Generate:
-##   layer_execution_order = list( topological_sort(layer_gragh) )
-## Locate top mem level for each operand of each layer. Store results in mem_update_list and mem_update_weight.
-##   for layer in all_layers:
-##     if layer.index != 0: ## not the 1st execution layer
-##       mem_udpate_list[layer]["I"] = mem_udpate_list[previous_layer]["O"]
-##     if len(layer.next_node) > 1 or len(next_layer.prevous_node) > 1: ## starting node of branches / final node of branches
-##     | if layer.index == 0:
-##     |   mem_update_list[layer]["I" / "O"] updates to the top input/output mem level
-##     | else:
-##     |   mem_update_list[layer]["O"] updates to the top output mem level
-##     |   mem_update_weight = top weight mem level, if mem_update_weight > top weight mem level
-##     |
-##     else:
-##       for mem in mem_levels(sort_order: from top to bottom):
-##         if sum(layer[operand_size] for operand in mem.operands) <= mem.size:
-##           if ["I", "O"] both in mem.operands:
-##             mem_update_list[layer]["O"] = current_mem_level
-##             if layer.index == 0: ## the 1st execution layer
-##               mem_update_list[layer]["I"] = current_mem_level
-##           if ("W" in mem.operand) and (current_mem_level < mem_update_weight):
-##             mem_update_weight = current_mem_level
-#####################################################
+# ########## Description ##########
+# TODO clean up. Don't think anyone will read this...
+# # This stage must be processed before WorkloadStage.
+# # This stage figures out the unused memory levels for "I", "W", "O" when the size of lower memory
+# # level is enough to hold all data, considering the output data of previous layer can be directly
+# # used by next layer. As an impact, the energy / latency related to these memories will be removed.
+# # The general criteria is:
+# #      If a low-level memory size is big enough to hold both "I" and "O" data of current layer,
+# #      memory above this one will be labeled as unused.
+# #      If a low-level memory size is big enough to hold "W" data of entire workload, memory above
+# #      this one will be labeled as unused.
+# # The above method only applies layers along the same branch, otherwise (for branch starting nodes
+# # or branch final nodes) the "O" data will return back to the top possible memory.
+# # In RemoveNoUseMemStage, unused mem across all layers, labeled in this stage, will be removed in
+# # the memory architecture.
+# # For now, the number of cores must be 1.
+# ########## Pseudo-code ##########
+# # Initialization:
+# #   mem_update_list = [layer_ids: {"I" / "O": -1}] # mem level of different operands of each layer
+# #   (there should be no -1 after self.update_top_mem_level())
+# #   each_layer_IO_data_size = [layer_ids: {"I" / "O": size}] # input / output data size of each layer
+# #   mem_update_weight = top_mem_level # top mem level to put weight
+# #   weight_size_entire_workload = weight_size # weight data size of entire workload
+# # Generate:
+# #   layer_execution_order = list( topological_sort(layer_graph) )
+# # Locate top mem level for each operand of each layer. Store results in mem_update_list and mem_update_weight.
+# #   for layer in all_layers:
+# #     if layer.index != 0: # not the 1st execution layer
+# #       mem_update_list[layer]["I"] = mem_update_list[previous_layer]["O"]
+# #     if len(layer.next_node) > 1 or len(next_layer.previous_node) > 1: # starting node of branches / final node of branches
+# #     | if layer.index == 0:
+# #     |   mem_update_list[layer]["I" / "O"] updates to the top input/output mem level
+# #     | else:
+# #     |   mem_update_list[layer]["O"] updates to the top output mem level
+# #     |   mem_update_weight = top weight mem level, if mem_update_weight > top weight mem level
+# #     |
+# #     else:
+# #       for mem in mem_levels(sort_order: from top to bottom):
+# #         if sum(layer[operand_size] for operand in mem.operands) <= mem.size:
+# #           if ["I", "O"] both in mem.operands:
+# #             mem_update_list[layer]["O"] = current_mem_level
+# #             if layer.index == 0: # the 1st execution layer
+# #               mem_update_list[layer]["I"] = current_mem_level
+# #           if ("W" in mem.operand) and (current_mem_level < mem_update_weight):
+# #             mem_update_weight = current_mem_level
+# ##########################
 #  Special note for Adder layers:
-#   Currently the algorithm is tricky for Adder layers. As for a conv/pool layer, required I, O sizes are put in
-#   each_layer_IO_data_size and the weight data size will be accumulated in weight_size_entire_workload.
-#   But for Adder layers, (1) there is no weight operand (or constant operand); (2) there are two input operands.
-#   (3) the info regarding which of the two operands is represented as I1 or I2 is not saved in self.workload,
-#   though it is defined in the input file.
+#   Currently the algorithm is tricky for Adder layers. As for a conv/pool layer, required I, O
+#   sizes are put in each_layer_IO_data_size and the weight data size will be accumulated in
+#   weight_size_entire_workload.
+#   But for Adder layers, (1) there is no weight operand (or constant operand); (2) there are two
+#   input operands. (3) the info regarding which of the two operands is represented as I1 or I2 is
+#   not saved in self.workload, though it is defined in the input file.
 #   So, the current solution is:
-#   (1) for weight, the data amount is 0, which means weight_size_entire_workload will not consider Adder layers.
-#   (2) for act, we add up the data size of the two (or multiple) inputs and treat the sum as the act data size
-#   for the current layer, which is stored in each_layer_IO_data_size.
+#   (1) for weight, the data amount is 0, which means weight_size_entire_workload will not consider
+#   Adder layers. (2) for act, we add up the data size of the two (or multiple) inputs and treat the
+#   sum as the act data size for the current layer, which is stored in each_layer_IO_data_size.
 #   What does this mean?
-#   This means for Adder layers, the required act data size is over-estimated, because we also include the data amount
-#   of the other operand, which we may have defined separate mem for the other operand.
-#   In other words, for a mem level with enough size to hold both O, I1
-#   (assume I1 is the mem representation for one input),
-#   may be thought by the code that the size is not enough and therefore the output cannot be stored at this level.
+#   This means for Adder layers, the required act data size is over-estimated, because we also
+#   include the data amount of the other operand, which we may have defined separate mem for the
+#   other operand. In other words, for a mem level with enough size to hold both O, I1 (assume I1 is
+#   the mem representation for one input), may be thought by the code that the size is not enough
+#   and therefore the output cannot be stored at this level.
 #   But keep in mind that!!!!!:
-#   this is only a problem when you use manually-defined workload and there are Adder layers.
-#   there is no problem if your workload is an .onnx file, because Adder layers will be skipped by default.
+#   This is only a problem when you use manually-defined workload and there are Adder layers.
+#   There is no problem if your workload is an .onnx file, because Adder layers will be skipped by
+#   default.
 #   Is there a solution?
 #   The reason why it cannot be fixed is we do not know which operand is from which layer.
 #   This problem can be fixed unless this info granularity is saved in the self.workload object,
 #   which is a networkx graph.
 
 
 class SearchUnusedMemoryStage(Stage):
-    def __init__(self, list_of_callables, *, accelerator, workload, **kwargs):
+    def __init__(
+        self, list_of_callables: list[StageCallable], *, accelerator: Accelerator, workload: Workload, **kwargs: Any
+    ):
+        """
+        # TODO needs cleanup
+        """
         super().__init__(list_of_callables, **kwargs)
         self.accelerator = accelerator
         self.workload = workload
-        ## Initialization
-        self.mem_update_list = {}
-        self.each_layer_IO_data_size = {}  # unit: bit
+        # Initialization
+        self.mem_update_list: dict[str, list[dict[MemoryOperand, int]]] = {}
+        self.each_layer_IO_data_size: dict[str, list[dict[MemoryOperand, int]]] = {}  # unit: bit
+
+        # TODO fix this!
         core_id = accelerator.cores[0].id  # correct only for single-core hardware
-        self.core_mem_level_list = accelerator.get_core(
-            core_id=core_id
-        ).memory_hierarchy.mem_level_list
-        self.mem_update_weight = (
-            len(self.core_mem_level_list) - 1
-        )  # index of the top memory
-        self.weight_size_entire_workload = 0  # unit: bit
-        self.layer_list = {}  # layer name and its corresponding id
-        core = accelerator.get_core(core_id=core_id)
-        for id, layer in enumerate(nx.topological_sort(workload)):
-            if (
-                type(layer) != DummyNode
-            ):  # create record on memory level, data size of each operand for un-dummy nodes
-                # identify the weight operand
-                if len(layer.constant_operands) == 1:
-                    weight_operand = layer.constant_operands[0]
-                else:
-                    if len(layer.constant_operands) == 0:
-                        # special case when defining workload manually:
-                        # the constant operands list is empty for such as "Adder" layers
-                        # for input operand, we will represent all inputs as one input, since only their data size is used for required mem size calculation.
-                        input_operand = layer.input_operands[0]
-                        output_operand = layer.output_operand
-                        input_data_size = 0
-                        for operand in layer.input_operands:
-                            input_data_size += layer.operand_size_bit[operand]
-                        self.mem_update_list[f"{id}"] = [
-                            {operand: -1}
-                            for operand in core.mem_hierarchy_dict.keys()
-                            if operand
-                            in [
-                                layer.memory_operand_links[output_operand],
-                                layer.memory_operand_links[input_operand],
-                            ]
-                        ]
-                        self.each_layer_IO_data_size[f"{id}"] = [
-                            {
-                                layer.memory_operand_links[
-                                    output_operand
-                                ]: layer.operand_size_bit[output_operand],
-                                layer.memory_operand_links[
-                                    input_operand
-                                ]: input_data_size,
-                            }
-                        ]
-                        self.layer_list[layer] = id
-                        continue
-                    else:
-                        # special case when defining workload manually:
-                        # both I and W are considered as constant operands for the first layer
-                        pr_loop_keys = tuple(layer.pr_loop.keys())
-                        for (
-                            operand,
-                            related_loop,
-                        ) in layer.operand_dimensionality_order.items():
-                            if pr_loop_keys[0] in related_loop:
-                                act_operand = operand
-                        weight_operand: list = [
-                            x for x in layer.constant_operands if x != act_operand
-                        ]
-                        assert len(weight_operand) == 1
-                        weight_operand: str = weight_operand[0]
-                self.mem_update_list[f"{id}"] = [
+
+        core = accelerator.get_core(core_id)
+        self.core_mem_level_list = core.memory_hierarchy.mem_level_list
+        self.mem_update_weight = len(self.core_mem_level_list) - 1  # index of the top memory
+        self.weight_size_entire_workload: int = 0  # unit: bit
+        self.layer_list: dict[LayerNode, int] = {}  # layer name and its corresponding id
+
+        for idx, layer in enumerate(workload.topological_sort()):
+            if isinstance(layer, DummyNode):
+                continue
+
+            # identify the weight operand
+            if len(layer.constant_operands) == 1:
+                weight_operand: LayerOperand = layer.constant_operands[0]
+            elif len(layer.constant_operands) == 0:
+                # special case when defining workload manually:
+                # the constant operands list is empty for such as "Adder" layers
+                # for input operand, we will represent all inputs as one input, since only their data size is used for required mem size calculation.
+                input_operand = layer.input_operands[0]
+                output_operand = layer.output_operand
+                input_data_size = 0
+                for operand in layer.input_operands:
+                    input_data_size += layer.operand_size_bit[operand]
+                self.mem_update_list[str(idx)] = [
                     {operand: -1}
                     for operand in core.mem_hierarchy_dict.keys()
-                    if operand != layer.memory_operand_links[weight_operand]
+                    if operand
+                    in [
+                        layer.memory_operand_links[output_operand],
+                        layer.memory_operand_links[input_operand],
+                    ]
                 ]
-                self.each_layer_IO_data_size[f"{id}"] = [
+                self.each_layer_IO_data_size[str(idx)] = [
                     {
-                        layer.memory_operand_links[operand]: layer.operand_size_bit[
-                            operand
-                        ]
-                        for operand in layer.memory_operand_links.keys()
-                        if operand != weight_operand
+                        layer.memory_operand_links[output_operand]: layer.operand_size_bit[output_operand],
+                        layer.memory_operand_links[input_operand]: input_data_size,
                     }
                 ]
-                self.weight_size_entire_workload += layer.operand_size_bit[
-                    weight_operand
-                ]
-                self.layer_list[layer] = id
+                self.layer_list[layer] = idx
+                continue
+            # special case when defining workload manually:
+            # both I and W are considered as constant operands for the first layer
+            else:
+                pr_loop_keys = tuple(layer.pr_loop.keys())
+                act_operand: LayerOperand | None = None
+                related_loop_dict = {
+                    layer_op: layer.equation.get_r_layer_dims(layer_op)
+                    for layer_op in layer.equation.get_contained_operands()
+                }
+                for operand, related_loop in related_loop_dict.items():
+                    if pr_loop_keys[0] in related_loop:
+                        act_operand = operand
+                assert act_operand is not None
+                weight_operand_temp: list[LayerOperand] = [x for x in layer.constant_operands if x != act_operand]
+                assert len(weight_operand_temp) == 1
+                weight_operand: LayerOperand = weight_operand_temp[0]
+
+            self.mem_update_list[str(idx)] = [
+                {operand: -1}
+                for operand in core.mem_hierarchy_dict.keys()
+                if operand != layer.memory_operand_links[weight_operand]
+            ]
+            self.each_layer_IO_data_size[str(idx)] = [
+                {
+                    layer.memory_operand_links[operand]: layer.operand_size_bit[operand]
+                    for operand in layer.memory_operand_links
+                    if operand != weight_operand
+                }
+            ]
+            self.weight_size_entire_workload += layer.operand_size_bit[weight_operand]
+            self.layer_list[layer] = idx
 
-    def run(self, workload_data_always_from_top_mem=False) -> Generator:
+    def run(self, workload_data_always_from_top_mem: bool = False):
         self.update_top_mem_level()  # figure out the lowest possible mem level for all operands for all layers
 
         if workload_data_always_from_top_mem:
             # [OPTIONAL] re-define the input/output mem level of first/last layer to the top possible mem level. This
             # is specially designed for the case that workload input and output must be stored in the top mem level.
             self.update_mem_level_for_loading_data()
 
-        sub_stage = self.list_of_callables[0](
+        sub_stage: Stage = self.list_of_callables[0](
             self.list_of_callables[1:],
             accelerator=self.accelerator,
             workload=self.workload,
             mem_update_list=self.mem_update_list,
             mem_update_weight=self.mem_update_weight,
             layer_list=self.layer_list,
             **self.kwargs,
         )
         for cme, (layer, extra_info) in sub_stage.run():
             yield cme, (layer, extra_info)
 
     def update_top_mem_level(self):
         """
         Update mem_update_list and mem_update_weight according to the algorithm description at the file beginning.
+        # TODO cleanup, split into functions
         """
         self.remove_dummy_nodes_in_workload()  # remove dummy nodes for the ease of telling the branch starting or final nodes
 
-        ## Update mem_update_list and mem_update_weight
-        for id, layer in enumerate(nx.topological_sort(self.workload)):
-            branch_starting_node = (
-                True if self.workload.out_degree(layer) > 1 else False
-            )  # starting node of branches
+        # Update mem_update_list and mem_update_weight
+        for id, layer in enumerate(self.workload.topological_sort()):
+            if isinstance(layer, DummyNode):
+                continue
+
+            # starting node of branches
+            branch_starting_node = True if self.workload.out_degree(layer) > 1 else False
             branch_final_node = (
                 True
                 if self.workload.out_degree(layer) == 1
-                and self.workload.in_degree(list(self.workload.successors(layer))[0])
-                > 1
+                and self.workload.in_degree(list(self.workload.successors(layer))[0]) > 1
                 else False
             )
-            output_operand = layer.memory_operand_links[
+            output_operand: MemoryOperand = layer.memory_operand_links[
                 layer.output_operand
             ]  # output representation in memory
-            curr_id = self.layer_list[
-                layer
-            ]  # current layer id (key) in mem_udpate_list
+            curr_id = self.layer_list[layer]  # current layer id (key) in mem_update_list
+            # weight representation in memory
             if len(layer.constant_operands) == 1:
-                const_operand = layer.memory_operand_links[
-                    layer.constant_operands[0]
-                ]  # weight representation in memory
-                act_operand = layer.memory_operand_links[
-                    [
-                        operand
-                        for operand in layer.input_operands
-                        if operand not in layer.constant_operands
-                    ][0]
-                ]  # act representation in memory
+                const_operand = layer.memory_operand_links[layer.constant_operands[0]]
+                # act representation in memory
+                act_operand: MemoryOperand = layer.memory_operand_links[
+                    [operand for operand in layer.input_operands if operand not in layer.constant_operands][0]
+                ]
+            elif len(layer.constant_operands) == 0:
+                # special case when defining workload manually:
+                # the constant operands list is empty for such as "Adder" layers
+                const_operand = None
+                act_operand = layer.memory_operand_links[layer.input_operands[0]]
             else:
-                if len(layer.constant_operands) == 0:
-                    # special case when defining workload manually:
-                    # the constant operands list is empty for such as "Adder" layers
-                    const_operand = None
-                    act_operand = layer.memory_operand_links[layer.input_operands[0]]
-                else:
-                    # special case when defining workload manually:
-                    # both I and W are considered as constant operands for the first layer
-                    pr_loop_keys = tuple(layer.pr_loop.keys())
-                    for (
-                        operand,
-                        related_loop,
-                    ) in layer.operand_dimensionality_order.items():
-                        if pr_loop_keys[0] in related_loop:
-                            act_operand = operand
-                    weight_operand: list = [
-                        x for x in layer.constant_operands if x != act_operand
-                    ]
-                    weight_operand: str = weight_operand[0]
-                    act_operand = layer.memory_operand_links[
-                        act_operand
-                    ]  # map from layer representation to hardware memory representation
-                    const_operand = layer.memory_operand_links[
-                        weight_operand
-                    ]  # weight representation in memory
-            if id != 0:  ## not the first layer
-                ## Assign mem_udpate_list[layer]["I"] = mem_udpate_list[previous_layer]["O"]
-                prev_layer = list(self.workload.predecessors(layer))[
-                    0
-                ]  # previous layer node (object)
+                # special case when defining workload manually:
+                # both I and W are considered as constant operands for the first layer
+                pr_loop_keys = tuple(layer.pr_loop.keys())
+                related_loop_dict: dict[LayerOperand, list[LayerDim]] = {
+                    layer_op: layer.equation.get_r_layer_dims(layer_op)
+                    for layer_op in layer.equation.get_contained_operands()
+                }
+                for operand, related_loop in related_loop_dict.items():
+                    if pr_loop_keys[0] in related_loop:
+                        act_operand = operand
+                weight_operand_temp: list[LayerOperand] = [x for x in layer.constant_operands if x != act_operand]
+                weight_operand: LayerOperand = weight_operand_temp[0]
+                # map from layer representation to hardware memory representation
+                const_operand: MemoryOperand = layer.memory_operand_links.layer_to_mem_op(weight_operand)
+
+            if id != 0:  # not the first layer
+                # Assign mem_udpate_list[layer]["I"] = mem_udpate_list[previous_layer]["O"]
+                prev_layer: LayerNode = list(self.workload.predecessors(layer))[0]  # previous layer node (object)
                 prev_layer_id = self.layer_list[prev_layer]  # previous layer id
-                prev_layer_output_operand = (
-                    prev_layer.output_operand
-                )  # output representation in memory of previous layer
-                for ele in self.mem_update_list[
-                    f"{prev_layer_id}"
-                ]:  # find the output mem level of previous layer
-                    try:
-                        prev_layer_output_level = ele[f"{prev_layer_output_operand}"]
-                    except (
-                        KeyError
-                    ):  # skip if the key is incorrect, as there will only be one that match.
-                        pass
-                self.update_IO_mem_level(
-                    curr_id, act_operand, prev_layer_output_level
-                )  # update the input mem level of current layer
-            if (
-                branch_starting_node or branch_final_node
-            ):  ## branch starting node or branch final node or permited dummy nodes (e.g. Adder layer)
-                ## Update input, weight, output mem level for branch starting node and branch final node
-                ## Find the top mem level for input if it is the first layer, update mem_udpate_list of current layer
-                if id == 0:  ## the first layer
-                    for curr_mem_level, mem in reversed(
-                        list(enumerate(self.core_mem_level_list))
-                    ):
+                # output representation in memory of previous layer
+                prev_layer_output_layer_op = prev_layer.output_operand
+                prev_layer_output_mem_op = prev_layer.memory_operand_links.layer_to_mem_op(prev_layer_output_layer_op)
+                # starting node of branches
+                for ele in self.mem_update_list[f"{prev_layer_id}"]:
+                    if prev_layer_output_mem_op in ele:
+                        prev_layer_output_level = ele[prev_layer_output_mem_op]
+                        self.update_IO_mem_level(curr_id, act_operand, prev_layer_output_level)
+
+            # # branch starting node or branch final node or permited dummy nodes (e.g. Adder layer)
+            # # Update input, weight, output mem level for branch starting node and branch final node
+            # # Find the top mem level for input if it is the first layer, update mem_udpate_list of current layer
+            if branch_starting_node or branch_final_node:
+                if id == 0:  # the first layer
+                    for curr_mem_level, mem in reversed(list(enumerate(self.core_mem_level_list))):
                         served_operands = list(
                             mem.mem_level_of_operands.keys()
                         )  # Check the served operand of current mem
                         if act_operand in served_operands:
-                            self.update_IO_mem_level(
-                                curr_id, act_operand, curr_mem_level
-                            )  # update the input mem level of current layer if it is the first layer
+                            # update the input mem level of current layer if it is the first layer
+                            self.update_IO_mem_level(curr_id, act_operand, curr_mem_level)
                             break
-                ## Find the top mem level for output, update mem_update_list of current layer
-                for curr_mem_level, mem in reversed(
-                    list(enumerate(self.core_mem_level_list))
-                ):
-                    served_operands = list(
-                        mem.mem_level_of_operands.keys()
-                    )  # Check the served operand of current mem
+                # Find the top mem level for output, update mem_update_list of current layer
+                for curr_mem_level, mem in reversed(list(enumerate(self.core_mem_level_list))):
+                    served_operands = list(mem.mem_level_of_operands.keys())  # Check the served operand of current mem
                     if output_operand in served_operands:
-                        self.update_IO_mem_level(
-                            curr_id, output_operand, curr_mem_level
-                        )  # update the output mem level of current layer
+                        # update the output mem level of current layer
+                        self.update_IO_mem_level(curr_id, output_operand, curr_mem_level)
                         break
-                ## Find the top mem level for weight, update mem_update_weight of current layer to the top weight mem level if mem_update_weight is bigger
-                for curr_mem_level, mem in reversed(
-                    list(enumerate(self.core_mem_level_list))
-                ):
-                    served_operands = list(
-                        mem.mem_level_of_operands.keys()
-                    )  # Check the served operand of current mem
-                    if (
-                        const_operand in served_operands
-                    ):  # identify the top weight mem level
+                # Find the top mem level for weight, update mem_update_weight of current layer to the top weight mem level if mem_update_weight is bigger
+                for curr_mem_level, mem in reversed(list(enumerate(self.core_mem_level_list))):
+                    served_operands = list(mem.mem_level_of_operands.keys())  # Check the served operand of current mem
+                    if const_operand in served_operands:  # identify the top weight mem level
                         # We need to check if the current mem serve all oa dims, otherwise we will not decrease
                         # the mem_update_weight.
                         # The reason is if the current mem not serve all oa dims, the mapping will impact the memory
                         # utilization, so solely comparing with total memory size will be incorrect.
-                        mem_serve_all_oa_dims = self.check_if_mem_serve_all_oa_dims(
-                            mem, self.accelerator
-                        )
-                        if (
-                            curr_mem_level < self.mem_update_weight
-                        ) and mem_serve_all_oa_dims:  # mem_update_weight is bigger than the top weight mem level
+                        mem_serve_all_oa_dims = self.check_if_mem_serve_all_oa_dims(mem, self.accelerator)
+                        # mem_update_weight is bigger than the top weight mem level
+                        if (curr_mem_level < self.mem_update_weight) and mem_serve_all_oa_dims:
                             self.mem_update_weight = curr_mem_level
                         break
-            else:  ## node (layer) that is not a branch starting node or a branch final node
-                ## Iterate the memory level and update input, weight, output mem level
-                for curr_mem_level, mem in reversed(
-                    list(enumerate(self.core_mem_level_list))
-                ):
-                    served_operands = list(
-                        mem.mem_level_of_operands.keys()
-                    )  # Check the served operand of current mem
-                    ## Update input, weight, output mem level
-                    avail_mem_size = (
-                        mem.memory_instance.size * mem.unroll_count
-                    )  # available hardware mem size
+            # # node (layer) that is not a branch starting node or a branch final node
+            else:
+                # # Iterate the memory level and update input, weight, output mem level
+                for curr_mem_level, mem in reversed(list(enumerate(self.core_mem_level_list))):
+                    served_operands = list(mem.mem_level_of_operands.keys())  # Check the served operand of current mem
+                    # Update input, weight, output mem level
+                    avail_mem_size = mem.memory_instance.size * mem.unroll_count  # available hardware mem size
 
                     try:
                         # we need to grab the next layer name, which is a non-Adder layer for sure
                         # if next layer is an Adder layer, then branch_final_node=True for the current layer,
                         # so, the simulation will not reach to this "else" branch.
-                        next_layer = list(self.workload.successors(layer))[0]
+                        next_layer: LayerNode = list(self.workload.successors(layer))[0]
                         # next, we find out the layer representation for the act operand of the next layer
-                        const_layer_operand_of_next_layer = (
-                            next_layer.constant_operands[0]
-                        )
+                        const_layer_operand_of_next_layer = next_layer.constant_operands[0]
                         act_layer_operand_of_next_layer = [
                             operand
                             for operand in next_layer.input_operands
                             if operand != const_layer_operand_of_next_layer
                         ][0]
                         # then, we will fetch the mem representation for the act operand of the next layer
-                        act_mem_operand_of_next_layer = next_layer.memory_operand_links[
-                            act_layer_operand_of_next_layer
-                        ]
+                        act_mem_operand_of_next_layer = next_layer.memory_operand_links[act_layer_operand_of_next_layer]
                         # check if the current mem level serve the act operand in the next layer
                         mem_serve_act_in_next_layer = (
-                            True
-                            if (act_mem_operand_of_next_layer in served_operands)
-                            else False
+                            True if (act_mem_operand_of_next_layer in served_operands) else False
                         )
-                    except (
-                        IndexError
-                    ):  # there is no next layer, which means the current layer is the last layer
+                    except IndexError:  # there is no next layer, which means the current layer is the last layer
                         # As for the last layer, we will instead check
                         # if the mem serves act operand of the current layer.
-                        mem_serve_act_in_next_layer = (
-                            True if (act_operand in served_operands) else False
-                        )
+                        mem_serve_act_in_next_layer = True if (act_operand in served_operands) else False
 
+                    # ["I", "O"] both in mem.served_operands
                     mem_serve_io_both = (
-                        True
-                        if mem_serve_act_in_next_layer
-                        and (output_operand in served_operands)
-                        else False
-                    )  # ["I", "O"] both in mem.served_operands
-                    mem_serve_weight = (
-                        True if (const_operand in served_operands) else False
-                    )  # mem.served_operands = ["W"]
+                        True if mem_serve_act_in_next_layer and (output_operand in served_operands) else False
+                    )
+                    # mem.served_operands = ["W"]
+                    mem_serve_weight = True if (const_operand in served_operands) else False
                     # we need to change served_operands if the current layer is an Adder layer,
                     # for the ease of calculation of required input data size.
                     # Since an Adder layer has two inputs,
                     # but in each_layer_IO_data_size, data size of two inputs are put under one key,
                     # so we have to update served_operands to ensure the key used in each_layer_IO_data_size is in it.
-                    if (
-                        len(layer.constant_operands) == 0 and mem_serve_io_both
-                    ):  # the layer type is an Adder layer, which has multiple input operands
+
+                    # the layer type is an Adder layer, which has multiple input operands
+                    if len(layer.constant_operands) == 0 and mem_serve_io_both:
                         served_operands = [
                             output_operand,
                             layer.memory_operand_links[layer.input_operands[0]],
                         ]
 
                     if mem_serve_io_both or mem_serve_weight:
                         required_IO_data_size = sum(
                             [
                                 self.each_layer_IO_data_size[f"{curr_id}"][0][operand]
                                 for operand in served_operands
                                 if operand != const_operand
                             ]
                         )
+                        # required size to put data in current mem level
                         required_weight_size = (
-                            self.weight_size_entire_workload
-                            if const_operand in served_operands
-                            else 0
+                            self.weight_size_entire_workload if const_operand in served_operands else 0
                         )
-                        required_total_size = (
-                            required_IO_data_size + required_weight_size
-                        )  # required size to put data in current mem level
-                        if (
-                            required_total_size <= avail_mem_size
-                        ):  # sum(layer[operand_size] for operand in mem.operands) <= mem.size
+                        required_total_size = required_IO_data_size + required_weight_size
+
+                        # sum(layer[operand_size] for operand in mem.operands) <= mem.size
+                        if required_total_size <= avail_mem_size:
                             if mem_serve_io_both:
                                 if id == 0:
-                                    self.update_IO_mem_level(
-                                        curr_id, act_operand, curr_mem_level
-                                    )  # update input mem level
-                                self.update_IO_mem_level(
-                                    curr_id, output_operand, curr_mem_level
-                                )  # update output mem level
+                                    # update input mem level
+                                    self.update_IO_mem_level(curr_id, act_operand, curr_mem_level)
+                                # update output mem level
+                                self.update_IO_mem_level(curr_id, output_operand, curr_mem_level)
                             # For weight, we need to check if the current mem serve all oa dims, otherwise we will not
                             # decrease the mem_update_weight.
                             # The reason is if the current mem not serve all oa dims, the mapping will impact the memory
                             # utilization, so solely comparing with total memory size will be incorrect.
-                            mem_serve_all_oa_dims = self.check_if_mem_serve_all_oa_dims(
-                                mem, self.accelerator
-                            )
-                            if (
-                                (curr_mem_level < self.mem_update_weight)
-                                and mem_serve_all_oa_dims
-                                and mem_serve_weight
-                            ):  # update weight mem level
+                            mem_serve_all_oa_dims = self.check_if_mem_serve_all_oa_dims(mem, self.accelerator)
+                            # update weight mem level
+                            if (curr_mem_level < self.mem_update_weight) and mem_serve_all_oa_dims and mem_serve_weight:
                                 self.mem_update_weight = curr_mem_level
-        ## [OPTIONAL CHECK] assert check if there is -1 value in mem_update_list
-        ## [NOTE] Until here, if there is still -1 value in mem_update_list, it means the size of top mem level for IO is not big enough.
+        # [OPTIONAL CHECK] assert check if there is -1 value in mem_update_list
+        # [NOTE] Until here, if there is still -1 value in mem_update_list, it means the size of top mem level for IO is not big enough.
         for layer_ele in self.mem_update_list.values():
             for operand_dict in layer_ele:
                 assert (
                     list(operand_dict.values())[0] >= 0
-                ), "SearchUnusedMemoryStage fisnishes abnormally, there are still layers with top mem levels not figured out."
+                ), "SearchUnusedMemoryStage finishes abnormally, there are still layers with top mem levels not figured out."
 
-    def check_if_mem_serve_all_oa_dims(self, mem, accelerator):
+    def check_if_mem_serve_all_oa_dims(self, mem: MemoryLevel, accelerator: Accelerator):
         # check if mem serve all hardare dimensions
         core = accelerator.cores[0]
         operational_array = core.operational_array
-        oa_dim_nb = len(operational_array.dimensions)
-        mem_served_oa_dim_nb = len(mem.served_dimensions)
-        if mem_served_oa_dim_nb == oa_dim_nb:
-            return True
-        else:
-            return False
+        oa_dim_nb = len(operational_array.oa_dim_sizes)
+        mem_served_oa_dim_nb = mem.served_dimensions.nb_dims
+        return mem_served_oa_dim_nb == oa_dim_nb
 
     def update_mem_level_for_loading_data(self):
-        """
+        """!
         [OPTIONAL FUNCTION] This is an optional function.
         Depending on your requirement, sometimes data loading from the top mem level and offloading to the top mem level is a must.
         If that is the your case, add this function to self.run().
         Otherwise, if the input is generated on-chip at the lowest possible input mem level and the output is stored on-chip at the lowest possible output mem level, remove this function from self.run().
         [FUNCTION OBJECT]
         Update mem_update_list of first and last layer, so that the input data of first layer still is loaded from top input mem level and the output of last layer still is offloaded to top output mem level
         """
         self.remove_dummy_nodes_in_workload()  # remove dummy nodes for the ease of telling the branch starting or final nodes
 
-        ## Update mem_update_list and mem_update_weight
-        for id, layer in enumerate(nx.topological_sort(self.workload)):
+        # Update mem_update_list and mem_update_weight
+        for id, layer in enumerate(self.workload.topological_sort()):
+            if isinstance(layer, DummyNode):
+                continue
+
+            # act representation
             act_operand = layer.memory_operand_links[
-                [
-                    operand
-                    for operand in layer.input_operands
-                    if operand not in layer.constant_operands
-                ][0]
-            ]  # act representation
-            output_operand = layer.output_operand  # output representation
-            curr_id = self.layer_list[
-                layer
-            ]  # current layer id (key) in mem_udpate_list
-            if (
-                id == 0
-            ):  # the first layer: update activation mem level to the top possible mem level
-                for curr_mem_level, mem in reversed(
-                    list(enumerate(self.core_mem_level_list))
-                ):
-                    served_operands = list(
-                        mem.mem_level_of_operands.keys()
-                    )  # Check the served operand of current mem
+                [operand for operand in layer.input_operands if operand not in layer.constant_operands][0]
+            ]
+            output_layer_op = layer.output_operand  # output representation
+            output_mem_op = layer.memory_operand_links.layer_to_mem_op(output_layer_op)
+            curr_id = self.layer_list[layer]  # current layer id (key) in mem_udpate_list
+            if id == 0:  # the first layer: update activation mem level to the top possible mem level
+                for curr_mem_level, mem in reversed(list(enumerate(self.core_mem_level_list))):
+                    served_operands = list(mem.mem_level_of_operands.keys())  # Check the served operand of current mem
                     if act_operand in served_operands:
-                        self.update_IO_mem_level(
-                            curr_id, act_operand, curr_mem_level
-                        )  # update the input mem level of current layer if it is the first layer
+                        # update the input mem level of current layer if it is the first layer
+                        self.update_IO_mem_level(curr_id, act_operand, curr_mem_level)
                         break
-            if (
-                id == len(self.layer_list) - 1
-            ):  # the last layer: update output mem level to the top possible mem level
-                for curr_mem_level, mem in reversed(
-                    list(enumerate(self.core_mem_level_list))
-                ):
-                    served_operands = list(
-                        mem.mem_level_of_operands.keys()
-                    )  # Check the served operand of current mem
-                    if output_operand in served_operands:
-                        self.update_IO_mem_level(
-                            curr_id, output_operand, curr_mem_level
-                        )  # update the output mem level of current layer if it is the last layer
+            if id == len(self.layer_list) - 1:  # the last layer: update output mem level to the top possible mem level
+                for curr_mem_level, mem in reversed(list(enumerate(self.core_mem_level_list))):
+                    served_operands = list(mem.mem_level_of_operands.keys())  # Check the served operand of current mem
+                    if output_mem_op in served_operands:
+                        # update the output mem level of current layer if it is the last layer
+                        self.update_IO_mem_level(curr_id, output_mem_op, curr_mem_level)
                         break
 
     def remove_dummy_nodes_in_workload(self):
-        ## Remove dummy nodes (layers) in the graph (assume there is no branch from a non-dummy node to dummy node)
-        ## Redirect the outgoing edges of dummy nodes to non-dummy nodes
-        ## Algorithm:
-        ## for each dummy node, add edges between its predecessor nodes and successor nodes; then remove the dummy node.
-        #############################################
-        ## Comment on the following 4 lines below: visualize the network for debugging
-        ## import matplotlib.pyplot as plt
-        ## pos = nx.spring_layout(self.workload)
-        ## nx.draw(self.workload, pos, with_labels=True, node_color="lightblue", font_weight="bold")
-        ## plt.show()
-        #############################################
-        dummy_nodes = [
-            node for node in self.workload.nodes() if type(node) == DummyNode
-        ]
+        """! Remove dummy nodes (layers) in the graph (assume there is no branch from a non-dummy
+        node to dummy node) Redirect the outgoing edges of dummy nodes to non-dummy nodes
+        Algorithm:
+        for each dummy node, add edges between its predecessor nodes and successor nodes;
+        then remove the dummy node.
+
+        Comment on the following 4 lines below: visualize the network for debugging
+        import matplotlib.pyplot as plt
+        pos = nx.spring_layout(self.workload)
+        nx.draw(self.workload, pos, with_labels=True, node_color="lightblue", font_weight="bold")
+        plt.show()
+        """
+        dummy_nodes = [node for node in self.workload.nodes() if isinstance(node, DummyNode)]
         for dummy_node in dummy_nodes:
             for successor_node in list(self.workload.successors(dummy_node)):
                 for predecessor_node in list(self.workload.predecessors(dummy_node)):
                     self.workload.add_edge(predecessor_node, successor_node)
         self.workload.remove_nodes_from(dummy_nodes)
 
-    def update_IO_mem_level(self, layer_id, operand, target_level):
-        """
-        Update self.mem_update_list as:
+    def update_IO_mem_level(self, layer_id: int, operand: MemoryOperand, target_level: int):
+        """! Update self.mem_update_list as:
         self.mem_update_list[layer_id][operand_index][operand] = target_level
         """
         for pos, ele in enumerate(self.mem_update_list[f"{layer_id}"]):
             if list(ele.keys())[0] == f"{operand}":
-                self.mem_update_list[f"{layer_id}"][pos][f"{operand}"] = target_level
+                self.mem_update_list[f"{layer_id}"][pos][operand] = target_level
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/stages/Stage.py` & `zigzag_dse-3.1.1/zigzag/stages/Stage.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,48 @@
-from typing import Generator, Callable, List
+from abc import ABCMeta, abstractmethod
+from typing import Any, Generator, Protocol, runtime_checkable
 
-## Abstract superclass for Runnables
-class Stage:
 
-    ## The class constructor
-    # @param list_of_callables: a list of callables, that must have a signature compatible with this __init__ function
-    # (list_of_callables, *, required_kwarg1, required_kwarg2, kwarg_with_default=default, **kwargs)
-    # and return a Stage instance. This is used to flexibly build iterators upon other iterators.
-    # @param kwargs: any keyword arguments, irrelevant to the specific class in question but passed on down
-    def __init__(self, list_of_callables: List[Callable], **kwargs):
+from zigzag.cost_model.cost_model import CostModelEvaluationABC
+
+
+class Stage(metaclass=ABCMeta):
+    """! Abstract superclass for Runnables"""
+
+    def __init__(
+        self,
+        list_of_callables: list["StageCallable"],
+        **kwargs: Any,
+    ):
+        """
+        @param list_of_callables: a list of callables, that must have a signature compatible with this __init__ function
+        and return a Stage instance. This is used to flexibly build iterators upon other iterators.
+        @param kwargs: any keyword arguments, irrelevant to the specific class in question but passed on down
+        """
         self.kwargs = kwargs
         self.list_of_callables = list_of_callables
         if self.is_leaf() and list_of_callables not in ([], tuple(), set(), None):
             raise ValueError("Leaf runnable received a non empty list_of_callables")
 
         if list_of_callables in ([], tuple(), set(), None) and not self.is_leaf():
             raise ValueError(
                 "List of callables empty on a non leaf runnable, so nothing can be generated.\
-                              Final callable in list_of_callables must return Stage instances that have is_leaf() == True"
+                    Final callable in list_of_callables must return Stage instances that have is_leaf() == True"
             )
 
-    ## Runs the runnable.
-    # This requires no arguments and returns a generator yielding any amount of tuple, that each have
-    # a CostModelEvaluation as the first element and a second element that can be anything, meant only for manual
-    # inspection.
-    def run(self) -> Generator:
-        raise ImportError("Run function not implemented for runnable")
+    @abstractmethod
+    def run(self) -> Generator[tuple[CostModelEvaluationABC, Any], None, None]: ...
 
     def __iter__(self):
         return self.run()
 
-    ## @return: Returns true if the runnable is a leaf runnable, meaning that it does not use (or thus need) any substages
-    # to be able to yield a result. Final element in list_of_callables must always have is_leaf() == True, except
-    # for that final element that has an empty list_of_callables
     def is_leaf(self) -> bool:
+        """! @return: Returns true if the runnable is a leaf runnable, meaning that it does not use (or thus need)
+        any substages to be able to yield a result. Final element in list_of_callables must always have
+        is_leaf() == True, except for that final element that has an empty list_of_callables
+        """
         return False
 
-## Not actually a Stage, as running it does return (not yields!) a list of results instead of a generator
-# Can be used as the main entry point
-class MainStage:
-
-    def __init__(self, list_of_callables, **kwargs):
-        self.kwargs = kwargs
-        self.list_of_callables = list_of_callables
 
-    def run(self):
-        answers = []
-        for cme, extra_info in self.list_of_callables[0](
-            self.list_of_callables[1:], **self.kwargs
-        ).run():
-            answers.append((cme, extra_info))
-        return answers
+@runtime_checkable
+class StageCallable(Protocol):
+    def __call__(self, list_of_callables: list["StageCallable"], **kwagrs: Any) -> Stage: ...
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/stages/WorkloadStage.py` & `zigzag_dse-3.1.1/zigzag/stages/WorkloadStage.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,51 @@
-import networkx as nx
 import logging
+from typing import Any
 
-from zigzag.classes.stages.Stage import Stage
-from zigzag.classes.workload.dummy_node import DummyNode
+
+from zigzag.hardware.architecture.Accelerator import Accelerator
+from zigzag.stages.Stage import Stage, StageCallable
+from zigzag.workload.Workload import Workload
+from zigzag.workload.DummyNode import DummyNode
 
 
 logger = logging.getLogger(__name__)
 
-## Class that iterates through the nodes in a given workload graph.
+
 class WorkloadStage(Stage):
+    """! Class that iterates through the nodes in a given workload graph."""
 
-    ## The class constructor
-    # Initialization of self.workload.
-    def __init__(self, list_of_callables, *, workload, accelerator, **kwargs):
+    def __init__(
+        self, list_of_callables: list[StageCallable], *, workload: Workload, accelerator: Accelerator, **kwargs: Any
+    ):
+        """
+        Initialization of self.workload.
+        """
         super().__init__(list_of_callables, **kwargs)
         self.workload = workload
         self.accelerator = accelerator
 
     def run(self):
-        for id, layer in enumerate(nx.topological_sort(self.workload)):
-            if type(layer) == DummyNode:
-                continue  # skip the DummyNodes
+        for layer in self.workload.topological_sort():
+            # skip the DummyNodes
+            if isinstance(layer, DummyNode):
+                continue
             # Skip a layer if the layer type is "Pooling" and the hardware template is an IMC core.
             # This wil have impact when the workload is defined manually.
             # If the workload is from onnx, no skipping will be done.
-            core_id = layer.core_allocation
+            core_id: int = layer.core_allocation[0]
             core = self.accelerator.get_core(core_id)
             operational_array = core.operational_array
-            pe_type = getattr(operational_array, "pe_type", None)  # return None if it does not exist
-            try:  # branch if the workload is manually defined
-                layer_type = layer.layer_attrs["operator_type"]
-            except KeyError:  # branch if the workload is from an onnx (key "operator_type" does not exist)
-                layer_type = None
+            pe_type = getattr(operational_array, "pe_type", None)
+            layer_type = layer.type
+
             if (pe_type in ["in_sram_computing"]) and (layer_type in ["Pooling", "Add"]):
                 continue
 
             kwargs = self.kwargs.copy()
             kwargs["layer"] = layer
             kwargs["accelerator"] = self.accelerator
-            if layer.name:
-                layer_name = layer.name
-            else:
-                layer_name = id
-            logger.info(f"Processing layer {layer_name}...")
+
+            logger.info(f"Processing  {layer.name}...")
             sub_stage = self.list_of_callables[0](self.list_of_callables[1:], **kwargs)
             for cme, extra_info in sub_stage.run():
                 yield cme, (layer, extra_info)
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/workload/dummy_node.py` & `zigzag_dse-3.1.1/zigzag/workload/DummyNode.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,61 @@
-
-## A class to represent an ONNX node that is not "accelerateable".
-# This node is created to preserve the original ONNX model graph structure,
-# but will be skipped by the underlying engines, treating it as a 0 HW cost node.
-class DummyNode:
-
-    ## The class constructor
-    # Initialize the DummyNode by setting its id, the node's predecessors and optionally giving it a name.
-    # @param id (int): id for this node
-    # @param preds (list): list of ids of this node's predecessor nodes
-    # @param node_name (str, optional): a name for this node, e.g. the node's name within the onnx model
-    def __init__(self, id, preds, node_name="", type=None) -> None:
-        self.id = id
-        self.input_operand_source = {"I": preds}
-        self.name = node_name
+from zigzag.datatypes import LayerOperand
+from zigzag.workload.LayerNodeABC import LayerNodeABC
+from zigzag.workload.layer_attributes import InputOperandSource
+
+
+class DummyNode(LayerNodeABC):
+    """! A class to represent an ONNX node that is not "accelerateable".
+    This node is created to preserve the original ONNX model graph structure,
+    but will be skipped by the underlying engines, treating it as a 0 HW cost node.
+    """
+
+    def __init__(self, layer_id: int, predecessor: int | None, node_name: str = "", type: str | None = None) -> None:
+        """
+        Initialize the DummyNode by setting its id, the node's predecessors and optionally giving it a name.
+        @param id (int): id for this node
+        @param predecessor (list): list of ids of this node's predecessor nodes
+        @param node_name (str, optional): a name for this node, e.g. the node's name within the onnx model
+        """
+        super().__init__(layer_id, node_name)
+        self.input_operand_source: InputOperandSource = (
+            {LayerOperand("I"): predecessor} if predecessor is not None else {}
+        )
         self.type = type
-        self.core_allocation = (
-            -1
-        )  # We assume these nodes are mapped on a core with id -1
+        # We assume these nodes are mapped on a core with id -1
+        self.core_allocation = -1
         self.runtime = 0
         self.start = None
         self.end = None
 
     def __str__(self):
         return f"DummyNode({self.id})"
 
-    def __repr__(self) -> str:
-        return str(self)
-
-    ## JSON representation used for saving this object to a json file.
-    def __jsonrepr__(self):
-        return {"id": self.id}
-
-    ## Set the start time in ccyles of this node
-    # @param start (int): start time in cycles
-    def set_start(self, start):
+    def set_start(self, start: int):
+        """! Set the start time in ccyles of this node
+        @param start : start time in cycles
+        """
         self.start = start
 
-    ## Set the end time in cycles of this node
-    # @param end (int): end time in cycles
-    def set_end(self, end):
+    def set_end(self, end: int):
+        """! Set the end time in cycles of this node
+        @param end: end time in cycles
+        """
         self.end = end
 
-    ## Get the start time in cycles of this node.
     def get_start(self):
+        """! Get the start time in cycles of this node."""
         return self.start
 
-    ## Get the end time in cycles of this node.
     def get_end(self):
+        """! Get the end time in cycles of this node."""
         return self.end
 
-    ## Return the runtime of running this node.
     def get_runtime(self):
+        """! Return the runtime of running this node."""
         return self.runtime
 
-    ## Check if this node has already been assigned an end time.
-    # @return (bool) True if this node has been assigned an end time
     def has_end(self) -> bool:
+        """! Check if this node has already been assigned an end time.
+        @return (bool) True if this node has been assigned an end time
+        """
         return self.end is not None
```

### Comparing `zigzag_dse-3.1.0/zigzag/classes/workload/onnx_workload.py` & `zigzag_dse-3.1.1/zigzag/workload/ONNXWorkload.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,29 @@
-import networkx as nx
+from typing import Any
 
-from zigzag.classes.workload.layer_node import LayerNode
-from typing import Dict, Any
-from networkx import DiGraph
+from zigzag.workload.LayerNodeABC import LayerNodeABC
+from zigzag.workload.Workload import Workload
 
 
-## Description missing
-class ONNXWorkload(DiGraph):
+class ONNXWorkload(Workload):
 
-    ## Collect all the algorithmic workload information here.
-    def __init__(self, **attr):
+    def __init__(self, **attr: Any):
+        """! Collect all the algorithmic workload information here."""
         super().__init__(**attr)
 
-        self.node_id_to_obj = {}
-        self.node_list = []
+        self.node_id_to_obj: dict[int, LayerNodeABC] = {}
+        self.node_list: list[LayerNodeABC] = []
 
-    ## Add a node object to the ONNX workload graph.
-    # This can be a different object based on if it's an "accelerateable" node or not.
-    def add(self, node_id, node_obj):
+    def add(self, node_id: int, node_obj: LayerNodeABC):
+        """! Add a node object to the ONNX workload graph.
+        This can be a different object based on if it's an "accelerateable" node or not.
+        """
         self.node_list.append(node_obj)
         self.node_id_to_obj[node_id] = node_obj
 
-        self.add_node(node_obj)
-        edges = []
-        for (op, parents) in node_obj.input_operand_source.items():
-            for parent_id in parents:
-                parent_node_obj = self.node_id_to_obj[parent_id]
-                edges.append((parent_node_obj, node_obj))
-                node_obj.input_operand_source[op] = parent_node_obj
-            self.add_edges_from(edges)
-
-    def topological_sort(self):
-        return nx.topological_sort(self)
-
-    def get_node_with_id(self, id):
-        for node in self.nodes:
-            if node.id == id:
-                return node
-        raise ValueError(
-            "DNNWorkload instance does not have a node with the requested id"
-        )
+        self.add_workload_node(node_obj)
+        edges: list[tuple[LayerNodeABC, LayerNodeABC]] = []
+        for _, parent_id in node_obj.input_operand_source.items():
+            # for parent_id in parents:
+            parent_node_obj = self.node_id_to_obj[parent_id]
+            edges.append((parent_node_obj, node_obj))
+            self.add_workload_edges_from(edges)
```

### Comparing `zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc1_validation_subfunc.py` & `zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc1_validation_subfunc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,137 +1,182 @@
-from aimc_cost_model import ADC, DAC
-from dimc_cost_model import UnitDff, MultiplierArray, MemoryInstance
-
-def aimc1_cost_estimation(aimc, cacti_value):
-    unit_reg = UnitDff(aimc['unit_area'], aimc['unit_delay'], aimc['unit_cap'])
-    unit_area = aimc['unit_area']
-    unit_delay = aimc['unit_delay']
-    unit_cap = aimc['unit_cap']
-    input_channel = aimc['input_channel']
-    reg_input_bitwidth = aimc['reg_input_bitwidth']
-    input_bandwidth = input_channel * aimc['input_precision']
-    output_bandwidth_per_channel = aimc['output_precision']
-    """
-    multiplier array for each output channel
-    """
-    mults = MultiplierArray(vdd=aimc['vdd'],input_precision=int(aimc['multiplier_precision']),number_of_multiplier=input_channel, unit_area=unit_area, unit_delay=unit_delay, unit_cap=unit_cap)
-    
-    """
-    adder_tree for each output channel
-    """
-    adder_tree = None
-        
-    """
-    accumulator for each output channel
-    """
-    accumulator = None
-    
-    """
-    ADC cost for each output channel
-    """
-    adc = ADC(resolution=aimc['adc_resolution'], ICH=aimc['input_channel'])
-    
-    """
-    DAC cost for each input channel
-    """
-    dac = DAC(resolution=aimc['dac_resolution'])
-
-    """
-    memory instance (delay unit: ns, energy unit: fJ, area unit: mm2)
-    unitbank: sram bank, data from CACTI
-    regs_input: input register files
-    regs_output: output register files for each output channel
-    regs_accumulator: register files inside accumulator for each output channel (congifuration is same with regs_output)
-    """
-    unitbank = MemoryInstance(name='unitbank', size=aimc['rows']*aimc['cols'], r_bw=aimc['cols'], w_bw=aimc['cols'], delay=cacti_value['delay']*0, r_energy=cacti_value['r_energy'], w_energy=cacti_value['w_energy'], area=cacti_value['area'], r_port=1, w_port=1, rw_port=0, latency=0)
-    energy_wl = 0 # per output channel
-    energy_bl = aimc['input_channel'] * aimc['unit_cap']/2*2 * aimc['vdd']**2 # per output channel (aimc['unit_cap']/2 for bitline cap/cell, *2 for 2 bitline port of 2 cells connecting together)
-    energy_en = aimc['input_channel'] * aimc['unit_cap']/2 * aimc['vdd']**2 # per output channel (energy cost on "csbias" enable signal)
-    
-    
-    """
-    calculate result
-    :predicted_area:                The area cost for entire IMC core (unit: mm2)
-    :predicted_delay:               The minimum delay of single clock period (unit: ns)
-    :predicted_energy_per_cycle:    The energy cost each time the IMC core is activated (unit: fJ)
-    :number_of_cycle: The number of cycle for computing entire input
-    :predicted_energy:              The energy cost for computing entire input (unit: fJ)
-    :number_of_operations:          The number of operations executed when computing entire input
-    :predicted_tops:                Peak TOP/s
-    :predicted_topsw:               Peak TOP/s/W
-    """
-    
-    ## Area cost breakdown
-    area_mults = aimc['banks'] * aimc['output_channel'] * mults.calculate_area()
-    area_adder_tree = 0
-    area_accumulator = 0
-    area_banks = aimc['banks'] * 2*unitbank.area # 2 for pulse generators (repeators in papers) (it's an assumption)
-    area_regs_accumulator = 0
-    area_regs_pipeline = 0
-    area_adc = aimc['banks'] * aimc['output_channel'] * adc.calculate_area()
-    area_dac = aimc['banks'] * aimc['input_channel'] * dac.calculate_area()
-    
-    # (for beyong ADC/DAC part, scale from 28nm -> 22nm, exclude ADC/DAC, which is assumed indepedent from tech.) (assume linear)
-    area_mults = area_mults/28*22
-    area_adder_tree = area_adder_tree/28*22
-    area_accumulator = area_accumulator/28*22
-    area_banks = area_banks # the area is for 22 nm
-    area_regs_accumulator = area_regs_accumulator/28*22
-    area_regs_pipeline = area_regs_pipeline/28*22
-    area_adc = area_adc/28*22
-    area_dac = area_dac/28*22
-    
-    predicted_area = area_mults + area_adder_tree + area_accumulator + area_banks + area_regs_accumulator + area_regs_pipeline + area_adc + area_dac# cost of input/output regs has been taken out #  (scale from 22nm -> 28nm, exclude ADC/DAC, which is assumed indepedent from tech.) (assume linear)
-    
-    ## delay cost
-    predicted_delay = unitbank.delay + mults.calculate_delay() + adc.calculate_delay()
-        
-    ## Energy cost breakdown per cycle 
-    energy_mults = (1-aimc['weight_sparsity']) * aimc['banks'] * aimc['output_channel'] * mults.calculate_energy()
-    energy_adder_tree = 0
-    energy_accumulator = 0
-    energy_banks = (1-aimc['weight_sparsity']) * aimc['banks'] * aimc['output_channel'] * (energy_wl + energy_bl + energy_en)
-    energy_regs_accumulator = 0
-    energy_regs_pipeline = 0
-    energy_adc = (1-aimc['weight_sparsity']) * aimc['banks'] * aimc['output_channel'] * adc.calculate_energy(vdd=aimc['vdd'])
-    energy_dac = aimc['banks'] * aimc['input_channel'] * dac.calculate_energy(vdd=aimc['vdd'], k0=aimc['dac_energy_k0'])
-    
-    # (for beyong ADC/DAC part, scale from 28nm -> 22nm, exclude ADC/DAC, which is assumed indepedent from tech.) (assume linear)
-    energy_mults = energy_mults/28*22
-    energy_adder_tree = energy_adder_tree/28*22
-    energy_accumulator = energy_accumulator/28*22
-    energy_banks = energy_banks/28*22
-    energy_regs_accumulator = energy_regs_accumulator/28*22
-    energy_regs_pipeline = energy_regs_pipeline/28*22
-    
-        
-    predicted_energy_per_cycle = energy_mults + energy_adder_tree + energy_accumulator + energy_banks + energy_regs_accumulator + energy_regs_pipeline + energy_adc + energy_dac 
-    
-    number_of_cycle = aimc['activation_precision']/aimc['input_precision']
-    
-    predicted_energy = predicted_energy_per_cycle * number_of_cycle
-    
-    number_of_operations = 2*aimc['banks']*aimc['output_channel']*aimc['input_channel'] # 1MAC = 2 Operations
-        
-    predicted_tops = number_of_operations/(predicted_delay*number_of_cycle) / (10**3)
-    predicted_topsw = number_of_operations/predicted_energy * 10**3
-    
-    ## Energy breakdown per MAC
-    number_of_mac = number_of_operations/2
-    energy_mults_mac = energy_mults * number_of_cycle/number_of_mac
-    energy_adder_tree_mac = 0
-    energy_accumulator_mac = 0
-    energy_banks_mac = energy_banks * number_of_cycle/number_of_mac
-    energy_regs_accumulator_mac = 0
-    energy_regs_pipeline_mac = 0
-    energy_adc_mac = energy_adc * number_of_cycle/number_of_mac
-    energy_dac_mac = energy_dac * number_of_cycle/number_of_mac
-    energy_estimation_per_mac = predicted_energy/number_of_mac
-    energy_reported_per_mac = 2000/aimc['TOP/s/W']
-    
-    area_mismatch = abs(predicted_area/aimc['area']-1)
-    delay_mismatch = abs(predicted_delay/aimc['tclk']-1)
-    energy_mismatch = abs(energy_estimation_per_mac/energy_reported_per_mac-1)
-    #return predicted_area, predicted_delay, energy_estimation_per_mac
-    #return area_mismatch, delay_mismatch, energy_mismatch
-    #print(area_mults, area_adder_tree, area_accumulator, area_banks, area_regs_accumulator, area_regs_pipeline)
-    #print(energy_mults_mac, energy_adder_tree_mac, energy_accumulator_mac, energy_banks_mac, energy_regs_accumulator_mac, energy_regs_pipeline_mac)
+from aimc_cost_model import ADC, DAC
+from dimc_cost_model import UnitDff, MultiplierArray, MemoryInstance
+
+
+def aimc1_cost_estimation(aimc, cacti_value):
+    unit_reg = UnitDff(aimc["unit_area"], aimc["unit_delay"], aimc["unit_cap"])
+    unit_area = aimc["unit_area"]
+    unit_delay = aimc["unit_delay"]
+    unit_cap = aimc["unit_cap"]
+    input_channel = aimc["input_channel"]
+    reg_input_bitwidth = aimc["reg_input_bitwidth"]
+    input_bandwidth = input_channel * aimc["input_precision"]
+    output_bandwidth_per_channel = aimc["output_precision"]
+    """
+    multiplier array for each output channel
+    """
+    mults = MultiplierArray(
+        vdd=aimc["vdd"],
+        input_precision=int(aimc["multiplier_precision"]),
+        number_of_multiplier=input_channel,
+        unit_area=unit_area,
+        unit_delay=unit_delay,
+        unit_cap=unit_cap,
+    )
+
+    """
+    adder_tree for each output channel
+    """
+    adder_tree = None
+
+    """
+    accumulator for each output channel
+    """
+    accumulator = None
+
+    """
+    ADC cost for each output channel
+    """
+    adc = ADC(resolution=aimc["adc_resolution"], ICH=aimc["input_channel"])
+
+    """
+    DAC cost for each input channel
+    """
+    dac = DAC(resolution=aimc["dac_resolution"])
+
+    """
+    memory instance (delay unit: ns, energy unit: fJ, area unit: mm2)
+    unitbank: sram bank, data from CACTI
+    regs_input: input register files
+    regs_output: output register files for each output channel
+    regs_accumulator: register files inside accumulator for each output channel (congifuration is same with regs_output)
+    """
+    unitbank = MemoryInstance(
+        name="unitbank",
+        size=aimc["rows"] * aimc["cols"],
+        r_bw=aimc["cols"],
+        w_bw=aimc["cols"],
+        delay=cacti_value["delay"] * 0,
+        r_energy=cacti_value["r_energy"],
+        w_energy=cacti_value["w_energy"],
+        area=cacti_value["area"],
+        r_port=1,
+        w_port=1,
+        rw_port=0,
+        latency=0,
+    )
+    energy_wl = 0  # per output channel
+    energy_bl = (
+        aimc["input_channel"] * aimc["unit_cap"] / 2 * 2 * aimc["vdd"] ** 2
+    )  # per output channel (aimc['unit_cap']/2 for bitline cap/cell, *2 for 2 bitline port of 2 cells connecting together)
+    energy_en = (
+        aimc["input_channel"] * aimc["unit_cap"] / 2 * aimc["vdd"] ** 2
+    )  # per output channel (energy cost on "csbias" enable signal)
+
+    """
+    calculate result
+    :predicted_area:                The area cost for entire IMC core (unit: mm2)
+    :predicted_delay:               The minimum delay of single clock period (unit: ns)
+    :predicted_energy_per_cycle:    The energy cost each time the IMC core is activated (unit: fJ)
+    :number_of_cycle: The number of cycle for computing entire input
+    :predicted_energy:              The energy cost for computing entire input (unit: fJ)
+    :number_of_operations:          The number of operations executed when computing entire input
+    :predicted_tops:                Peak TOP/s
+    :predicted_topsw:               Peak TOP/s/W
+    """
+
+    ## Area cost breakdown
+    area_mults = aimc["banks"] * aimc["output_channel"] * mults.calculate_area()
+    area_adder_tree = 0
+    area_accumulator = 0
+    area_banks = aimc["banks"] * 2 * unitbank.area  # 2 for pulse generators (repeators in papers) (it's an assumption)
+    area_regs_accumulator = 0
+    area_regs_pipeline = 0
+    area_adc = aimc["banks"] * aimc["output_channel"] * adc.calculate_area()
+    area_dac = aimc["banks"] * aimc["input_channel"] * dac.calculate_area()
+
+    # (for beyong ADC/DAC part, scale from 28nm -> 22nm, exclude ADC/DAC, which is assumed indepedent from tech.) (assume linear)
+    area_mults = area_mults / 28 * 22
+    area_adder_tree = area_adder_tree / 28 * 22
+    area_accumulator = area_accumulator / 28 * 22
+    area_banks = area_banks  # the area is for 22 nm
+    area_regs_accumulator = area_regs_accumulator / 28 * 22
+    area_regs_pipeline = area_regs_pipeline / 28 * 22
+    area_adc = area_adc / 28 * 22
+    area_dac = area_dac / 28 * 22
+
+    predicted_area = (
+        area_mults
+        + area_adder_tree
+        + area_accumulator
+        + area_banks
+        + area_regs_accumulator
+        + area_regs_pipeline
+        + area_adc
+        + area_dac
+    )  # cost of input/output regs has been taken out #  (scale from 22nm -> 28nm, exclude ADC/DAC, which is assumed indepedent from tech.) (assume linear)
+
+    ## delay cost
+    predicted_delay = unitbank.delay + mults.calculate_delay() + adc.calculate_delay()
+
+    ## Energy cost breakdown per cycle
+    energy_mults = (1 - aimc["weight_sparsity"]) * aimc["banks"] * aimc["output_channel"] * mults.calculate_energy()
+    energy_adder_tree = 0
+    energy_accumulator = 0
+    energy_banks = (
+        (1 - aimc["weight_sparsity"]) * aimc["banks"] * aimc["output_channel"] * (energy_wl + energy_bl + energy_en)
+    )
+    energy_regs_accumulator = 0
+    energy_regs_pipeline = 0
+    energy_adc = (
+        (1 - aimc["weight_sparsity"]) * aimc["banks"] * aimc["output_channel"] * adc.calculate_energy(vdd=aimc["vdd"])
+    )
+    energy_dac = aimc["banks"] * aimc["input_channel"] * dac.calculate_energy(vdd=aimc["vdd"], k0=aimc["dac_energy_k0"])
+
+    # (for beyong ADC/DAC part, scale from 28nm -> 22nm, exclude ADC/DAC, which is assumed indepedent from tech.) (assume linear)
+    energy_mults = energy_mults / 28 * 22
+    energy_adder_tree = energy_adder_tree / 28 * 22
+    energy_accumulator = energy_accumulator / 28 * 22
+    energy_banks = energy_banks / 28 * 22
+    energy_regs_accumulator = energy_regs_accumulator / 28 * 22
+    energy_regs_pipeline = energy_regs_pipeline / 28 * 22
+
+    predicted_energy_per_cycle = (
+        energy_mults
+        + energy_adder_tree
+        + energy_accumulator
+        + energy_banks
+        + energy_regs_accumulator
+        + energy_regs_pipeline
+        + energy_adc
+        + energy_dac
+    )
+
+    number_of_cycle = aimc["activation_precision"] / aimc["input_precision"]
+
+    predicted_energy = predicted_energy_per_cycle * number_of_cycle
+
+    number_of_operations = 2 * aimc["banks"] * aimc["output_channel"] * aimc["input_channel"]  # 1MAC = 2 Operations
+
+    predicted_tops = number_of_operations / (predicted_delay * number_of_cycle) / (10**3)
+    predicted_topsw = number_of_operations / predicted_energy * 10**3
+
+    ## Energy breakdown per MAC
+    number_of_mac = number_of_operations / 2
+    energy_mults_mac = energy_mults * number_of_cycle / number_of_mac
+    energy_adder_tree_mac = 0
+    energy_accumulator_mac = 0
+    energy_banks_mac = energy_banks * number_of_cycle / number_of_mac
+    energy_regs_accumulator_mac = 0
+    energy_regs_pipeline_mac = 0
+    energy_adc_mac = energy_adc * number_of_cycle / number_of_mac
+    energy_dac_mac = energy_dac * number_of_cycle / number_of_mac
+    energy_estimation_per_mac = predicted_energy / number_of_mac
+    energy_reported_per_mac = 2000 / aimc["TOP/s/W"]
+
+    area_mismatch = abs(predicted_area / aimc["area"] - 1)
+    delay_mismatch = abs(predicted_delay / aimc["tclk"] - 1)
+    energy_mismatch = abs(energy_estimation_per_mac / energy_reported_per_mac - 1)
+    # return predicted_area, predicted_delay, energy_estimation_per_mac
+    # return area_mismatch, delay_mismatch, energy_mismatch
+    # print(area_mults, area_adder_tree, area_accumulator, area_banks, area_regs_accumulator, area_regs_pipeline)
+    # print(energy_mults_mac, energy_adder_tree_mac, energy_accumulator_mac, energy_banks_mac, energy_regs_accumulator_mac, energy_regs_pipeline_mac)
```

### Comparing `zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc2_validation_subfunc.py` & `zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc3_validation_subfunc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,142 +1,210 @@
-from aimc_cost_model import ADC, DAC
-from dimc_cost_model import UnitNand2, UnitDff, MultiplierArray, Adder, AdderTree, MemoryInstance
-
-def aimc2_cost_estimation(aimc, cacti_value):
-    unit_reg = UnitDff(aimc['unit_area'], aimc['unit_delay'], aimc['unit_cap'])
-    unit_area = aimc['unit_area']
-    unit_delay = aimc['unit_delay']
-    unit_cap = aimc['unit_cap']
-    input_channel = aimc['input_channel']
-    reg_input_bitwidth = aimc['reg_input_bitwidth']
-    input_bandwidth = input_channel * aimc['input_precision']
-    output_bandwidth_per_channel = aimc['output_precision']
-    """
-    multiplier array for each output channel
-    """
-    col_mux = 2
-    mults = MultiplierArray(vdd=aimc['vdd'],input_precision=int(aimc['multiplier_precision']),number_of_multiplier=col_mux*input_channel, unit_area=unit_area, unit_delay=unit_delay, unit_cap=unit_cap)
-    
-    """
-    adder_tree for each output channel
-    """
-    # adder tree with place value
-    adder1 = Adder(vdd=aimc['vdd'], input_precision=7, unit_area=unit_area, unit_delay=unit_delay, unit_cap=unit_cap) # 8 in total
-    adder2 = Adder(vdd=aimc['vdd'], input_precision=9, unit_area=unit_area, unit_delay=unit_delay, unit_cap=unit_cap) # 4 in total
-    adder3 = Adder(vdd=aimc['vdd'], input_precision=12, unit_area=unit_area, unit_delay=unit_delay, unit_cap=unit_cap) # 2 in total
-    adder4 = Adder(vdd=aimc['vdd'], input_precision=15, unit_area=unit_area, unit_delay=unit_delay, unit_cap=unit_cap) # 1 in total
-    adder_tree = AdderTree(vdd=aimc['vdd'], input_precision=int(aimc['adder_input_precision']), number_of_input=input_channel, unit_area=unit_area, unit_delay=unit_delay, unit_cap=unit_cap)
-        
-    """
-    accumulator for each output channel
-    """
-    accumulator = Adder(vdd=aimc['vdd'], input_precision=int(aimc['accumulator_precision']), unit_area=unit_area, unit_delay=unit_delay, unit_cap=unit_cap)
-    
-    """
-    ADC cost for each ADC
-    """
-    adc = ADC(resolution=aimc['adc_resolution'], ICH=aimc['input_channel'])
-    
-    """
-    DAC cost for each DAC
-    """
-    dac = DAC(resolution=aimc['dac_resolution'])
-
-    """
-    memory instance (delay unit: ns, energy unit: fJ, area unit: mm2)
-    unitbank: sram bank, data from CACTI
-    regs_accumulator: register files inside accumulator for each output channel (congifuration is same with regs_output)
-    """
-    unitbank = MemoryInstance(name='unitbank', size=aimc['rows']*aimc['cols'], r_bw=aimc['cols'], w_bw=aimc['cols'], delay=cacti_value['delay']*0, r_energy=cacti_value['r_energy'], w_energy=cacti_value['w_energy'], area=cacti_value['area'], r_port=1, w_port=1, rw_port=0, latency=0)
-    regs_accumulator = MemoryInstance(name='regs_accumulator', size=aimc['reg_accumulator_precision'], r_bw=aimc['reg_accumulator_precision'], w_bw=aimc['reg_accumulator_precision'], delay=unit_reg.calculate_delay(), r_energy=0, w_energy=unit_reg.calculate_cap() * aimc['vdd']**2 * aimc['reg_accumulator_precision'], area=unit_reg.calculate_area()*aimc['reg_accumulator_precision'], r_port=1, w_port=1, rw_port=0, latency=0)
-    regs_pipeline = MemoryInstance(name='regs_pipeline', size=5*16, r_bw=5*16, w_bw=5*16, delay=0, r_energy=0, w_energy=unit_reg.calculate_cap() * aimc['vdd']**2 * 5 * 16, area=unit_reg.calculate_area()*5*16, r_port=1, w_port=1, rw_port=0, latency=1)
-    
-    energy_wl = aimc['input_channel'] * aimc['unit_cap']/2*2 * aimc['vdd']**2 * aimc['weight_precision'] # per output channel
-    #energy_bl = aimc['rows'] * aimc['unit_cap']/2*2 * aimc['vdd']**2 * aimc['weight_precision'] # per output channel (aimc['unit_cap']/2 for bitline cap/cell, *2 for 2 bitline port of 2 cells connecting together)
-    energy_en = aimc['input_channel'] * aimc['unit_cap']/2*2 * aimc['vdd']**2 # per output channel (energy cost on "en" enable signal)
-    energy_bl = 0 # assume bitline doesn't change during computation
-    
-    """
-    calculate result
-    :predicted_area:                The area cost for entire IMC core (unit: mm2)
-    :predicted_delay:               The minimum delay of single clock period (unit: ns)
-    :predicted_energy_per_cycle:    The energy cost each time the IMC core is activated (unit: fJ)
-    :number_of_cycle: The number of cycle for computing entire input
-    :predicted_energy:              The energy cost for computing entire input (unit: fJ)
-    :number_of_operations:          The number of operations executed when computing entire input
-    :predicted_tops:                Peak TOP/s
-    :predicted_topsw:               Peak TOP/s/W
-    """
-    
-    ## Area cost breakdown
-    area_mults = aimc['banks'] * aimc['output_channel'] * mults.calculate_area()
-    #area_adder_tree = aimc['banks'] * aimc['output_channel'] * adder_tree.calculate_area()
-    area_adder_tree = aimc['banks'] * aimc['output_channel'] * ( 8*adder1.calculate_area() + 4*adder2.calculate_area() + 2*adder3.calculate_area() + 1*adder4.calculate_area() )
-    area_accumulator = aimc['banks'] * aimc['output_channel'] * accumulator.calculate_area()
-    area_banks = aimc['banks'] *unitbank.area
-    area_regs_accumulator = aimc['banks'] * aimc['output_channel'] * regs_accumulator.area
-    area_regs_pipeline = aimc['banks'] * aimc['output_channel'] * regs_pipeline.area
-    area_adc = aimc['banks'] * aimc['output_channel'] * 16 * adc.calculate_area()
-    area_dac = aimc['banks'] * 2 * aimc['input_channel'] * dac.calculate_area()
-    
-    
-    predicted_area = area_mults + area_adder_tree + area_accumulator + area_banks + area_regs_accumulator + area_regs_pipeline + area_adc + area_dac# cost of input/output regs has been taken out
-    
-    ## delay cost (2* for input transfer two times)
-    adder_1b_carry_delay = 2*UnitNand2(unit_area, unit_delay, unit_cap).calculate_delay()
-    accumulator_delay = accumulator.calculate_delay_lsb()+adder_1b_carry_delay * (aimc['reg_accumulator_precision']-aimc['accumulator_input_precision'])
-    predicted_delay = max(2* (unitbank.delay + mults.calculate_delay() + adc.calculate_delay()), 2*(adder_tree.calculate_delay() + accumulator_delay))
-        
-    ## Energy cost breakdown per input transfer
-    energy_mults = (1-aimc['weight_sparsity']) * aimc['banks'] * aimc['output_channel'] * mults.calculate_energy()
-    #energy_adder_tree = (1-aimc['weight_sparsity']) * aimc['banks'] * aimc['output_channel'] * adder_tree.calculate_energy()
-    energy_adder_tree = (1 - aimc['weight_sparsity']) * aimc['banks'] * aimc[
-        'output_channel'] * ( 8*adder1.calculate_energy() + 4*adder2.calculate_energy() + 2*adder3.calculate_energy() + 1*adder4.calculate_energy() )
-    energy_accumulator = aimc['banks'] * aimc['output_channel'] * accumulator.calculate_energy()
-    energy_banks = (1-aimc['weight_sparsity']) * aimc['banks'] * aimc['output_channel'] * (energy_wl + energy_bl + energy_en)
-    energy_regs_accumulator = aimc['banks'] * aimc['output_channel'] * regs_accumulator.w_energy
-    energy_regs_pipeline = aimc['banks'] * aimc['output_channel'] * regs_pipeline.w_energy
-    energy_adc = (1-aimc['weight_sparsity']) * aimc['banks'] * aimc['output_channel'] * 16 * adc.calculate_energy(vdd=aimc['vdd'])
-    energy_dac = aimc['banks'] * 2 * aimc['input_channel'] * dac.calculate_energy(vdd=aimc['vdd'], k0=aimc['dac_energy_k0'])
-    
-    ## 2* for input transfer two times
-    energy_mults *= 2
-    energy_adder_tree *= 2
-    energy_accumulator *= 2
-    energy_banks *= 2
-    energy_regs_accumulator *= 2
-    energy_regs_pipeline *= 2
-    energy_adc *= 2
-    energy_dac *= 2
-    
-        
-    predicted_energy_per_cycle = energy_mults + energy_adder_tree + energy_accumulator + energy_banks + energy_regs_accumulator + energy_regs_pipeline + energy_adc + energy_dac
-    
-    number_of_cycle = aimc['activation_precision']/aimc['input_precision']
-    
-    predicted_energy = predicted_energy_per_cycle * number_of_cycle
-    
-    number_of_operations = 2*aimc['banks']*aimc['output_channel']*aimc['input_channel'] # 1MAC = 2 Operations
-        
-    predicted_tops = number_of_operations/(predicted_delay*number_of_cycle) / (10**3)
-    predicted_topsw = number_of_operations/predicted_energy * 10**3
-    
-    ## Energy breakdown per MAC
-    number_of_mac = number_of_operations/2
-    energy_mults_mac = energy_mults * number_of_cycle/number_of_mac
-    energy_adder_tree_mac = energy_adder_tree * number_of_cycle/number_of_mac
-    energy_accumulator_mac = energy_accumulator * number_of_cycle/number_of_mac
-    energy_banks_mac = energy_banks * number_of_cycle/number_of_mac
-    energy_regs_accumulator_mac = energy_regs_accumulator * number_of_cycle/number_of_mac
-    energy_regs_pipeline_mac = energy_regs_pipeline * number_of_cycle/number_of_mac
-    energy_adc_mac = energy_adc * number_of_cycle/number_of_mac
-    energy_dac_mac = energy_dac * number_of_cycle/number_of_mac
-    energy_estimation_per_mac = predicted_energy/number_of_mac
-    energy_reported_per_mac = 2000/aimc['TOP/s/W']
-    
-    area_mismatch = abs(predicted_area/aimc['area']-1)
-    delay_mismatch = abs(predicted_delay/aimc['tclk']-1)
-    energy_mismatch = abs(energy_estimation_per_mac/energy_reported_per_mac-1)
-    #return predicted_area, predicted_delay, energy_estimation_per_mac
-    #return area_mismatch, delay_mismatch, energy_mismatch
-    #print(area_mults, area_adder_tree, area_accumulator, area_banks, area_regs_accumulator, area_regs_pipeline)
-    #print(energy_mults_mac, energy_adder_tree_mac, energy_accumulator_mac, energy_banks_mac, energy_regs_accumulator_mac, energy_regs_pipeline_mac)
+from aimc_cost_model import ADC, DAC
+from dimc_cost_model import UnitDff, MultiplierArray, Adder, MemoryInstance
+
+
+def aimc3_cost_estimation(aimc, cacti_value):
+    unit_reg = UnitDff(aimc["unit_area"], aimc["unit_delay"], aimc["unit_cap"])
+    unit_area = aimc["unit_area"]
+    unit_delay = aimc["unit_delay"]
+    unit_cap = aimc["unit_cap"]
+    input_channel = aimc["input_channel"]
+    reg_input_bitwidth = aimc["reg_input_bitwidth"]
+    input_bandwidth = input_channel * aimc["input_precision"]
+    output_bandwidth_per_channel = aimc["output_precision"]
+    """
+    multiplier array for each output channel
+    """
+    mults = MultiplierArray(
+        vdd=aimc["vdd"],
+        input_precision=int(aimc["multiplier_precision"]),
+        number_of_multiplier=64,
+        unit_area=unit_area,
+        unit_delay=unit_delay,
+        unit_cap=unit_cap,
+    )
+    mults_energy = MultiplierArray(
+        vdd=aimc["vdd"],
+        input_precision=int(aimc["multiplier_precision"]),
+        number_of_multiplier=16,
+        unit_area=unit_area,
+        unit_delay=unit_delay,
+        unit_cap=unit_cap,
+    )  # mapped multipliers
+
+    """
+    adder_tree for each output channel
+    """
+    adder_tree = Adder(
+        vdd=aimc["vdd"],
+        input_precision=6,
+        unit_area=unit_area,
+        unit_delay=unit_delay,
+        unit_cap=unit_cap,
+    )
+
+    """
+    accumulator for each output channel
+    """
+    accumulator = None
+
+    """
+    ADC cost for each ADC
+    """
+    adc = ADC(resolution=aimc["adc_resolution"], ICH=aimc["input_channel"])
+    adc_area = ADC(resolution=7, ICH=64)  # for estimating area
+
+    """
+    DAC cost for each DAC
+    """
+    dac = None
+
+    """
+    memory instance (delay unit: ns, energy unit: fJ, area unit: mm2)
+    unitbank: sram bank, data from CACTI
+    regs_accumulator: register files inside accumulator for each output channel (congifuration is same with regs_output)
+    """
+    unitbank = MemoryInstance(
+        name="unitbank",
+        size=aimc["rows"] * aimc["cols"],
+        r_bw=aimc["cols"],
+        w_bw=aimc["cols"],
+        delay=cacti_value["delay"] * 0,
+        r_energy=cacti_value["r_energy"],
+        w_energy=cacti_value["w_energy"],
+        area=cacti_value["area"],
+        r_port=1,
+        w_port=1,
+        rw_port=0,
+        latency=0,
+    )
+    regs_accumulator = None
+    regs_pipeline = None
+
+    energy_wl = 0  # per output channel
+    # for energy_bl, there are 64 rows in total, but only 8 are used.
+    energy_bl = (
+        aimc["input_channel"] * aimc["unit_cap"] / 2 * aimc["vdd"] ** 2 * aimc["weight_precision"]
+    )  # per output channel (aimc['unit_cap']/2 for bitline cap/cell, *2 for 2 bitline port of 2 cells connecting together)
+    energy_en = 0  # per output channel (no enable signal) (for cap couplling-based AIMC, no enable signal is required, as long as the input sequence timing is gated when not under computation.)
+
+    """
+    calculate result
+    :predicted_area:                The area cost for entire IMC core (unit: mm2)
+    :predicted_delay:               The minimum delay of single clock period (unit: ns)
+    :predicted_energy_per_cycle:    The energy cost each time the IMC core is activated (unit: fJ)
+    :number_of_cycle: The number of cycle for computing entire input
+    :predicted_energy:              The energy cost for computing entire input (unit: fJ)
+    :number_of_operations:          The number of operations executed when computing entire input
+    :predicted_tops:                Peak TOP/s
+    :predicted_topsw:               Peak TOP/s/W
+    """
+
+    ## Area cost breakdown
+    area_mults = aimc["banks"] * aimc["output_channel"] * mults.calculate_area()
+    area_adder_tree = aimc["banks"] * aimc["output_channel"] * adder_tree.calculate_area()
+    area_accumulator = 0
+    if aimc["compact_rule"] == False:
+        area_banks = aimc["banks"] * 3 * unitbank.area  # 2 for non-compact rule scaling
+    else:
+        area_banks = aimc["banks"] * unitbank.area
+    area_regs_accumulator = 0
+    area_regs_pipeline = 0
+    area_adc = aimc["banks"] * aimc["output_channel"] * adc_area.calculate_area()
+    area_dac = 0  # =0
+
+    # (for beyong ADC/DAC part, scale from 28nm -> 22nm, exclude ADC/DAC, which is assumed indepedent from tech.) (assume linear)
+    area_mults = area_mults / 28 * 22
+    area_adder_tree = area_adder_tree / 28 * 22
+    area_accumulator = area_accumulator / 28 * 22
+    area_banks = area_banks / 28 * 22
+    area_regs_accumulator = area_regs_accumulator / 28 * 22
+    area_regs_pipeline = area_regs_pipeline / 28 * 22
+    area_adc = area_adc / 28 * 22
+    area_dac = area_dac / 28 * 22
+
+    predicted_area = (
+        area_mults
+        + area_adder_tree
+        + area_accumulator
+        + area_banks
+        + area_regs_accumulator
+        + area_regs_pipeline
+        + area_adc
+        + area_dac
+    )  # cost of input/output regs has been taken out
+
+    ## delay cost
+    predicted_delay = (
+        unitbank.delay + mults.calculate_delay() + adder_tree.calculate_delay_msb() + adc.calculate_delay()
+    )
+
+    ## Energy cost breakdown per input transfer
+    energy_mults = (
+        aimc["input_toggle_rate"]
+        * (1 - aimc["weight_sparsity"])
+        * aimc["banks"]
+        * aimc["output_channel"]
+        * mults_energy.calculate_energy()
+    )
+    energy_adder_tree = (
+        (1 - aimc["weight_sparsity"]) * aimc["banks"] * aimc["output_channel"] * adder_tree.calculate_energy()
+    )
+    energy_accumulator = 0
+    energy_banks = (
+        (1 - aimc["weight_sparsity"]) * aimc["banks"] * aimc["output_channel"] * (energy_wl + energy_bl + energy_en)
+    )
+    energy_regs_accumulator = 0
+    energy_regs_pipeline = 0
+    energy_adc = (
+        (1 - aimc["weight_sparsity"]) * aimc["banks"] * aimc["output_channel"] * adc.calculate_energy(vdd=aimc["vdd"])
+    )
+    energy_dac = 0
+
+    # (for beyong ADC/DAC part, scale from 28nm -> 22nm, exclude ADC/DAC, which is assumed indepedent from tech.) (assume linear)
+    energy_mults = energy_mults / 28 * 22
+    energy_adder_tree = energy_adder_tree / 28 * 22
+    energy_accumulator = energy_accumulator / 28 * 22
+    energy_banks = energy_banks / 28 * 22
+    energy_regs_accumulator = energy_regs_accumulator / 28 * 22
+    energy_regs_pipeline = energy_regs_pipeline / 28 * 22
+
+    predicted_energy_per_cycle = (
+        energy_mults
+        + energy_adder_tree
+        + energy_accumulator
+        + energy_banks
+        + energy_regs_accumulator
+        + energy_regs_pipeline
+        + energy_adc
+        + energy_dac
+    )
+
+    number_of_cycle = aimc["activation_precision"] / aimc["input_precision"]
+
+    predicted_energy = predicted_energy_per_cycle * number_of_cycle
+
+    number_of_operations = 2 * aimc["banks"] * aimc["output_channel"] * aimc["rows"] / 8  # 1MAC = 2 Operations
+
+    predicted_tops = number_of_operations / (predicted_delay * number_of_cycle) / (10**3)
+    predicted_topsw = number_of_operations / predicted_energy * 10**3
+
+    ## Energy breakdown per MAC
+    number_of_mac = number_of_operations / 2
+    energy_mults_mac = energy_mults * number_of_cycle / number_of_mac
+    energy_adder_tree_mac = energy_adder_tree * number_of_cycle / number_of_mac
+    energy_accumulator_mac = energy_accumulator * number_of_cycle / number_of_mac
+    energy_banks_mac = energy_banks * number_of_cycle / number_of_mac
+    energy_regs_accumulator_mac = energy_regs_accumulator * number_of_cycle / number_of_mac
+    energy_regs_pipeline_mac = 0
+    energy_adc_mac = energy_adc * number_of_cycle / number_of_mac
+    energy_dac_mac = energy_dac * number_of_cycle / number_of_mac
+    energy_estimation_per_mac = predicted_energy / number_of_mac
+    energy_reported_per_mac = 2000 / aimc["TOP/s/W"]
+
+    area_mismatch = abs(predicted_area / aimc["area"] - 1)
+    delay_mismatch = abs(predicted_delay / aimc["tclk"] - 1)
+    energy_mismatch = abs(energy_estimation_per_mac / energy_reported_per_mac - 1)
+    # return predicted_area, predicted_delay, energy_estimation_per_mac
+    # return area_mismatch, delay_mismatch, energy_mismatch
+    # print(area_mults, area_adder_tree, area_accumulator, area_banks, area_regs_accumulator, area_regs_pipeline)
+    # print(energy_mults_mac, energy_adder_tree_mac, energy_accumulator_mac, energy_banks_mac, energy_regs_accumulator_mac, energy_regs_pipeline_mac)
```

### Comparing `zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_cost_model.py` & `zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_cost_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,55 @@
-import math
-
-class ADC:
-    """
-    Class for a single ADC.
-    :param resolution: ADC resolution
-    :param vdd: The supply vdd (unit: V)
-    :param ICH: The number of input channels on bitline (ADC input node)
-    """
-    def __init__(self, resolution: int, ICH: int):
-        self.resolution = resolution
-        self.ICH = ICH
-    def calculate_area(self):
-        if self.resolution < 12:
-            #self.area = 10 ** (-0.25 * self.resolution-3.3) * 2**self.resolution # unit: mm2
-            self.area = (10**-6) * 10 ** (-0.0369 * self.resolution+1.206) * 2**self.resolution # unit: mm2
-        else:
-            self.area = 5 * 10**-7 * 2**self.resolution # unit: mm2
-        return self.area
-    def calculate_delay(self):
-        self.delay = self.resolution * (0.00653*self.ICH+0.640) # ns
-        return self.delay
-    def calculate_energy(self, vdd): # unit: fJ
-        k1 = 100 # fF
-        k2 = 0.001 # fF
-        self.energy = (k1 * self.resolution + k2 * 4**self.resolution) * vdd**2
-        return self.energy
-        
-class DAC:
-    """
-    Class for a single DAC.
-    :param resolution: DAC resolution
-    :param vdd: The supply vdd (unit: V)
-    """
-    def __init__(self, resolution: int):
-        self.resolution = resolution
-    def calculate_area(self):
-        self.area = 0
-        return self.area
-    def calculate_delay(self):
-        self.delay = 0
-        return self.delay
-    def calculate_energy(self, vdd, k0): # unit: fF
-        self.energy = (k0 * self.resolution) * vdd**2
-        return self.energy
+import math
+
+
+class ADC:
+    """
+    Class for a single ADC.
+    :param resolution: ADC resolution
+    :param vdd: The supply vdd (unit: V)
+    :param ICH: The number of input channels on bitline (ADC input node)
+    """
+
+    def __init__(self, resolution: int, ICH: int):
+        self.resolution = resolution
+        self.ICH = ICH
+
+    def calculate_area(self):
+        if self.resolution < 12:
+            # self.area = 10 ** (-0.25 * self.resolution-3.3) * 2**self.resolution # unit: mm2
+            self.area = (10**-6) * 10 ** (-0.0369 * self.resolution + 1.206) * 2**self.resolution  # unit: mm2
+        else:
+            self.area = 5 * 10**-7 * 2**self.resolution  # unit: mm2
+        return self.area
+
+    def calculate_delay(self):
+        self.delay = self.resolution * (0.00653 * self.ICH + 0.640)  # ns
+        return self.delay
+
+    def calculate_energy(self, vdd):
+        k1 = 100  # fF
+        k2 = 0.001  # fF
+        self.energy = (k1 * self.resolution + k2 * 4**self.resolution) * vdd**2
+        return self.energy  # unit: fJ
+
+
+class DAC:
+    """
+    Class for a single DAC.
+    :param resolution: DAC resolution
+    :param vdd: The supply vdd (unit: V)
+    """
+
+    def __init__(self, resolution: int):
+        self.resolution = resolution
+
+    def calculate_area(self):
+        self.area = 0
+        return self.area
+
+    def calculate_delay(self):
+        self.delay = 0
+        return self.delay
+
+    def calculate_energy(self, vdd, k0):  # unit: fF
+        self.energy = (k0 * self.resolution) * vdd**2
+        return self.energy
```

### Comparing `zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/model_extration_28nm.py` & `zigzag_dse-3.1.1/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/model_extration_28nm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,79 @@
-from dimc_validation import dimc_ISSCC2022_15_5, cacti_ISSCC2022_15_5, dimc_ISSCC2022_11_7, cacti_ISSCC2022_11_7, dimc_ISSCC2023_7_2, cacti_value_ISSCC2023_7_2
-from dimc_validation4 import dimc_ISSCC2023_16_3, cacti_value_ISSCC2023_16_3
-from dimc_validation_subfunc4 import dimc_cost_estimation4
-from dimc_validation_subfunc import dimc_cost_estimation
-
-def area_fitting():
-    mismatch = 1
-    for area in range(294, 1000, 1):
-        dimc_ISSCC2022_15_5['unit_area'] = area/1000 #um2
-        dimc_ISSCC2022_11_7['unit_area'] = area/1000 #um2
-        dimc_ISSCC2023_7_2['unit_area'] = area/1000 #um2
-        dimc_ISSCC2023_16_3['unit_area'] = area/1000 #um2
-        a1, d1, e1 = dimc_cost_estimation(dimc_ISSCC2022_15_5, cacti_ISSCC2022_15_5)
-        a2, d2, e2 = dimc_cost_estimation(dimc_ISSCC2022_11_7, cacti_ISSCC2022_11_7)
-        a3, d3, e3 = dimc_cost_estimation(dimc_ISSCC2023_7_2, cacti_value_ISSCC2023_7_2)
-        a4, d4, e4 = dimc_cost_estimation4(dimc_ISSCC2023_16_3, cacti_value_ISSCC2023_16_3)
-        at = (a1+a2+a3+a4)/4 # average area mismatch
-        dt = (d1+d2+d3+d4)/4 # average delay mismatch
-        et = (e1+e3)/2 # average energy mismatch (peak energy is not reported in paper2)
-        if at < mismatch:
-            mismatch = at
-            fitted_unit_area = area/1000
-    print(f"fitted_unit_area: {fitted_unit_area}, average_mismatch: {mismatch}")
-    return mismatch, fitted_unit_area
-
-def delay_fitting():
-    mismatch = 1
-    for delay in range(150, 500, 1):
-        dimc_ISSCC2022_15_5['unit_delay'] = delay/10000 #ns
-        dimc_ISSCC2022_11_7['unit_delay'] = delay/10000 #ns
-        dimc_ISSCC2023_7_2['unit_delay'] = delay/10000 #ns
-        dimc_ISSCC2023_16_3['unit_delay'] = delay/10000 #ns
-        a1, d1, e1 = dimc_cost_estimation(dimc_ISSCC2022_15_5, cacti_ISSCC2022_15_5)
-        a2, d2, e2 = dimc_cost_estimation(dimc_ISSCC2022_11_7, cacti_ISSCC2022_11_7)
-        a3, d3, e3 = dimc_cost_estimation(dimc_ISSCC2023_7_2, cacti_value_ISSCC2023_7_2)
-        a4, d4, e4 = dimc_cost_estimation4(dimc_ISSCC2023_16_3, cacti_value_ISSCC2023_16_3)
-        at = (a1+a2+a3+a4)/4 # average area mismatch
-        dt = (d1+d2+d3+d4)/4 # average delay mismatch
-        et = (e1+e3)/2 # average energy mismatch (peak energy is not reported in paper2)
-        if dt < mismatch:
-            mismatch = dt
-            dlist = [d1,d2,d3,d4]
-            fitted_unit_delay = delay/10000
-    print(f"fitted_unit_delay: {fitted_unit_delay}, average_mismatch: {mismatch}")
-    return mismatch, fitted_unit_delay
-
-def cap_fitting():
-    mismatch = 1
-    for cap in range(1, 50, 1):
-        dimc_ISSCC2022_15_5['unit_cap'] = cap/10 #fF
-        dimc_ISSCC2022_11_7['unit_cap'] = cap/10 #fF
-        dimc_ISSCC2023_7_2['unit_cap'] = cap/10 #fF
-        a1, d1, e1 = dimc_cost_estimation(dimc_ISSCC2022_15_5, cacti_ISSCC2022_15_5)
-        a2, d2, e2 = dimc_cost_estimation(dimc_ISSCC2022_11_7, cacti_ISSCC2022_11_7)
-        a3, d3, e3 = dimc_cost_estimation(dimc_ISSCC2023_7_2, cacti_value_ISSCC2023_7_2)
-        at = (a1+a2+a3)/3 # average area mismatch
-        dt = (d1+d2+d3)/3 # average delay mismatch
-        et = (e1+e3)/2 # average energy mismatch (peak energy is not reported in paper2)
-        if et < mismatch:
-            mismatch = et
-            fitted_unit_cap = cap/10
-    print(f"fitted_unit_cap: {fitted_unit_cap}, average_mismatch: {mismatch}")
-    return mismatch, fitted_unit_cap
-
-if __name__ == '__main__':
-    area_fitting()
-    delay_fitting()
-    cap_fitting()
+from dimc_validation import (
+    dimc_ISSCC2022_15_5,
+    cacti_ISSCC2022_15_5,
+    dimc_ISSCC2022_11_7,
+    cacti_ISSCC2022_11_7,
+    dimc_ISSCC2023_7_2,
+    cacti_value_ISSCC2023_7_2,
+)
+from dimc_validation4 import dimc_ISSCC2023_16_3, cacti_value_ISSCC2023_16_3
+from dimc_validation_subfunc4 import dimc_cost_estimation4
+from dimc_validation_subfunc import dimc_cost_estimation
+
+
+def area_fitting():
+    mismatch = 1
+    for area in range(294, 1000, 1):
+        dimc_ISSCC2022_15_5["unit_area"] = area / 1000  # um2
+        dimc_ISSCC2022_11_7["unit_area"] = area / 1000  # um2
+        dimc_ISSCC2023_7_2["unit_area"] = area / 1000  # um2
+        dimc_ISSCC2023_16_3["unit_area"] = area / 1000  # um2
+        a1, d1, e1 = dimc_cost_estimation(dimc_ISSCC2022_15_5, cacti_ISSCC2022_15_5)
+        a2, d2, e2 = dimc_cost_estimation(dimc_ISSCC2022_11_7, cacti_ISSCC2022_11_7)
+        a3, d3, e3 = dimc_cost_estimation(dimc_ISSCC2023_7_2, cacti_value_ISSCC2023_7_2)
+        a4, d4, e4 = dimc_cost_estimation4(dimc_ISSCC2023_16_3, cacti_value_ISSCC2023_16_3)
+        at = (a1 + a2 + a3 + a4) / 4  # average area mismatch
+        dt = (d1 + d2 + d3 + d4) / 4  # average delay mismatch
+        et = (e1 + e3) / 2  # average energy mismatch (peak energy is not reported in paper2)
+        if at < mismatch:
+            mismatch = at
+            fitted_unit_area = area / 1000
+    print(f"fitted_unit_area: {fitted_unit_area}, average_mismatch: {mismatch}")
+    return mismatch, fitted_unit_area
+
+
+def delay_fitting():
+    mismatch = 1
+    for delay in range(150, 500, 1):
+        dimc_ISSCC2022_15_5["unit_delay"] = delay / 10000  # ns
+        dimc_ISSCC2022_11_7["unit_delay"] = delay / 10000  # ns
+        dimc_ISSCC2023_7_2["unit_delay"] = delay / 10000  # ns
+        dimc_ISSCC2023_16_3["unit_delay"] = delay / 10000  # ns
+        a1, d1, e1 = dimc_cost_estimation(dimc_ISSCC2022_15_5, cacti_ISSCC2022_15_5)
+        a2, d2, e2 = dimc_cost_estimation(dimc_ISSCC2022_11_7, cacti_ISSCC2022_11_7)
+        a3, d3, e3 = dimc_cost_estimation(dimc_ISSCC2023_7_2, cacti_value_ISSCC2023_7_2)
+        a4, d4, e4 = dimc_cost_estimation4(dimc_ISSCC2023_16_3, cacti_value_ISSCC2023_16_3)
+        at = (a1 + a2 + a3 + a4) / 4  # average area mismatch
+        dt = (d1 + d2 + d3 + d4) / 4  # average delay mismatch
+        et = (e1 + e3) / 2  # average energy mismatch (peak energy is not reported in paper2)
+        if dt < mismatch:
+            mismatch = dt
+            dlist = [d1, d2, d3, d4]
+            fitted_unit_delay = delay / 10000
+    print(f"fitted_unit_delay: {fitted_unit_delay}, average_mismatch: {mismatch}")
+    return mismatch, fitted_unit_delay
+
+
+def cap_fitting():
+    mismatch = 1
+    for cap in range(1, 50, 1):
+        dimc_ISSCC2022_15_5["unit_cap"] = cap / 10  # fF
+        dimc_ISSCC2022_11_7["unit_cap"] = cap / 10  # fF
+        dimc_ISSCC2023_7_2["unit_cap"] = cap / 10  # fF
+        a1, d1, e1 = dimc_cost_estimation(dimc_ISSCC2022_15_5, cacti_ISSCC2022_15_5)
+        a2, d2, e2 = dimc_cost_estimation(dimc_ISSCC2022_11_7, cacti_ISSCC2022_11_7)
+        a3, d3, e3 = dimc_cost_estimation(dimc_ISSCC2023_7_2, cacti_value_ISSCC2023_7_2)
+        at = (a1 + a2 + a3) / 3  # average area mismatch
+        dt = (d1 + d2 + d3) / 3  # average delay mismatch
+        et = (e1 + e3) / 2  # average energy mismatch (peak energy is not reported in paper2)
+        if et < mismatch:
+            mismatch = et
+            fitted_unit_cap = cap / 10
+    print(f"fitted_unit_cap: {fitted_unit_cap}, average_mismatch: {mismatch}")
+    return mismatch, fitted_unit_cap
+
+
+if __name__ == "__main__":
+    area_fitting()
+    delay_fitting()
+    cap_fitting()
```

### Comparing `zigzag_dse-3.1.0/zigzag/visualization/graph/memory_hierarchy.py` & `zigzag_dse-3.1.1/zigzag/visualization/graph/memory_hierarchy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 import matplotlib.pyplot as plt
 import networkx as nx
 import matplotlib.pyplot as plt
+from networkx import Graph
 
-from zigzag.classes.hardware.architecture.memory_hierarchy import MemoryHierarchy
+from zigzag.hardware.architecture.memory_level import MemoryLevel
 
 
-def visualize_memory_hierarchy_graph(G: MemoryHierarchy):
+def visualize_memory_hierarchy_graph(G: Graph, save_path: str = ""):
     """
     Visualizes a memory hierarchy graph.
     """
 
     generations = list(nx.topological_generations(G))
     max_nodes_gen = max((len(generation) for generation in generations))
     pos = {}
     node_list = []
     node_size_list = []
     node_label_dict = {}
+    node: MemoryLevel
     for gen_idx, generation in enumerate(generations):
         y = gen_idx
         node_size = (gen_idx + 1) * 2000
         for node_idx, node in enumerate(generation):
             if len(generation) == max_nodes_gen:
                 x = node_idx
             else:
                 x = (node_idx + 1) * (max_nodes_gen - 1) / (len(generation) + 1)
             pos[node] = (x, y)
             node_list.append(node)
             node_size_list.append(node_size)
-            node_label_dict[
-                node
-            ] = f"{node.name}\n{node.operands}\nx{node.unroll_count}"
+            node_label_dict[node] = f"{node.name}\n{node.operands}\nx{node.unroll_count}"
 
     nx.draw(
         G,
         pos=pos,
         node_shape="s",
         nodelist=node_list,
         node_size=node_size_list,
         labels=node_label_dict,
     )
     plt.title(G.name)
-    plt.show()
+    if save_path == "":
+        plt.show()
+    else:
+        plt.savefig(save_path)
+    plt.close()
 
 
 if __name__ == "__main__":
     import pickle
 
     with open("../list_of_cmes.pickle", "rb") as handle:
         list_of_cme = pickle.load(handle)
```

### Comparing `zigzag_dse-3.1.0/zigzag/visualization/graph/workload.py` & `zigzag_dse-3.1.1/zigzag/visualization/graph/workload.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,17 +27,7 @@
                 linewidth=5,
             ),
         )
     nx.draw_networkx_nodes(G, pos=pos, node_size=100, node_color="black")
     nx.draw_networkx_labels(G, pos=pos_lb, font_color="black")
     plt.box(False)
     plt.show()
-
-
-if __name__ == "__main__":
-    import zigzag.classes.stages.MainInputParserStages as MainInputParserStages
-
-    workload = "zigzag.inputs.examples.workload.resnet18"
-    parsed_workload = MainInputParserStages.parse_workload_from_path_or_from_module(
-        workload
-    )
-    visualize_dnn_graph(parsed_workload)
```

### Comparing `zigzag_dse-3.1.0/zigzag/visualization/results/plot_cme.py` & `zigzag_dse-3.1.1/zigzag/visualization/results/plot_cme.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-from typing import Dict, List, Tuple
-from typing import TYPE_CHECKING
 from collections import defaultdict
+from typing import Any
 import matplotlib.pyplot as plt
 from matplotlib.colors import hsv_to_rgb
 import numpy as np
-from zigzag.classes.mapping.combined_mapping import FourWayDataMoving
-from zigzag.classes.cost_model.cost_model import CostModelEvaluation
+from zigzag.cost_model.cost_model import CostModelEvaluation, CostModelEvaluationABC, CumulativeCME
+from zigzag.datatypes import LayerOperand
+from zigzag.hardware.architecture.MemoryInstance import MemoryInstance
+from zigzag.hardware.architecture.memory_level import MemoryLevel
+from zigzag.hardware.architecture.memory_port import DataDirection
+from zigzag.mapping.data_movement import FourWayDataMoving
 
 # MPL FONT SIZES
 SMALLEST_SIZE = 10
 SMALLER_SIZE = 12
 SMALL_SIZE = 14
 MEDIUM_SIZE = 16
 BIG_SIZE = 18
@@ -20,46 +23,40 @@
 plt.rc("xtick", labelsize=SMALLER_SIZE)  # fontsize of the tick labels
 plt.rc("ytick", labelsize=SMALLER_SIZE)  # fontsize of the tick labels
 plt.rc("legend", fontsize=SMALL_SIZE)  # legend fontsize
 plt.rc("figure", titlesize=MEDIUM_SIZE)  # fontsize of the figure title
 
 
 def bar_plot_cost_model_evaluations_total(
-    cmes: List[CostModelEvaluation],
-    labels,
+    cmes: list[CostModelEvaluation],
+    labels: list[str],
     save_path: str = "plot.png",
 ):
     """Plot total energy and latency of each cost model evaluation in a bar chart.
 
     Args:
         cmes (List[CostModelEvaluation]): List of CostModelEvaluations to compare.
         save_path (str): Path to save the plot to.
     """
-    assert len(cmes) == len(
-        labels
-    ), "Please match a label for each cost model evaluation."
+    assert len(cmes) == len(labels), "Please match a label for each cost model evaluation."
     energies = [cme.energy_total for cme in cmes]
     latencies = [cme.latency_total2 for cme in cmes]
 
     x = np.arange(len(labels))  # the label locations
     width = 0.35  # the width of the bars
 
     fig, ax1 = plt.subplots()
     ax2 = ax1.twinx()
 
     colormap = plt.get_cmap("Set1")
-    color_energy = colormap.colors[0]
-    color_latency = colormap.colors[1]
+    color_energy = colormap.colors[0]  # type: ignore
+    color_latency = colormap.colors[1]  # type: ignore
 
-    h1 = rects1 = ax1.bar(
-        x - width / 2, energies, width, label="Energy", color=color_energy
-    )
-    h2 = rects2 = ax2.bar(
-        x + width / 2, latencies, width, label="Latency", color=color_latency
-    )
+    h1 = rects1 = ax1.bar(x - width / 2, energies, width, label="Energy", color=color_energy)
+    h2 = rects2 = ax2.bar(x + width / 2, latencies, width, label="Latency", color=color_latency)
 
     # Add some text for labels, title and custom x-axis tick labels, etc.
     ax1.set_ylabel("Energy [pJ]", fontsize=15)
     ax2.set_ylabel("Latency [cycle]", fontsize=15)
     ax1.set_xticks(x, labels)
     handles1, labels1 = ax1.get_legend_handles_labels()
     handles2, labels2 = ax2.get_legend_handles_labels()
@@ -79,138 +76,136 @@
 
     # ax1.set_title(fig_title)
     fig.tight_layout()
     plt.savefig(save_path)
 
 
 def bar_plot_cost_model_evaluations_breakdown(
-    cmes: List[CostModelEvaluation], save_path: str, xtick_rotation=90
+    cmes: list[CostModelEvaluationABC], save_path: str, xtick_rotation: int = 90
 ):
-    memory_word_access_summed = {
-        d: defaultdict(lambda: defaultdict(lambda: FourWayDataMoving(0, 0, 0, 0)))
-        for d in range(len(cmes))
+    memory_word_access_summed: dict[int, defaultdict[LayerOperand, defaultdict[str, FourWayDataMoving]]] = {
+        idx: defaultdict(lambda: defaultdict(lambda: FourWayDataMoving(0, 0, 0, 0))) for idx in range(len(cmes))
     }
-    mac_costs = defaultdict(lambda: 0)
-    memory_instances = {}
-    la_break_down = {
-        d: {
+    mac_costs: defaultdict[int, float] = defaultdict(lambda: 0.0)
+    memory_instances: dict[str, MemoryLevel] = {}
+    la_break_down: dict[int, dict[str, float]] = {
+        idx: {
             "Ideal computation": 0,
             "Spatial stall": 0,
             "Temporal stall": 0,
             "Data loading": 0,
             "Data off-loading": 0,
         }
-        for d in range(len(cmes))
+        for idx in range(len(cmes))
     }
-    la_tot = {d: 0 for d in range(len(cmes))}
+    la_tot: dict[int, float] = {idx: 0 for idx in range(len(cmes))}
 
-    for d, cme in enumerate(cmes):
-        mh = cme.accelerator.get_core(cme.layer.core_allocation).memory_hierarchy
-        mac_costs[d] = cme.MAC_energy
-        la_break_down[d]["Ideal computation"] = cme.ideal_cycle
-        la_break_down[d]["Spatial stall"] = cme.ideal_temporal_cycle - cme.ideal_cycle
-        la_break_down[d]["Temporal stall"] = (
-            cme.latency_total0 - cme.ideal_temporal_cycle
-        )
-        la_break_down[d]["Data loading"] = cme.latency_total1 - cme.latency_total0
-        la_break_down[d]["Data off-loading"] = cme.latency_total2 - cme.latency_total1
-        la_tot[d] = cme.latency_total2
+    for idx, cme in enumerate(cmes):
+        if isinstance(cme, CumulativeCME):
+            continue
+        assert isinstance(cme, CostModelEvaluation)
+
+        mem_hierarchy = cme.accelerator.get_core(cme.layer.core_allocation[0]).memory_hierarchy
+        mac_costs[idx] = cme.MAC_energy
+        la_break_down[idx]["Ideal computation"] = cme.ideal_cycle
+        la_break_down[idx]["Spatial stall"] = cme.ideal_temporal_cycle - cme.ideal_cycle
+        la_break_down[idx]["Temporal stall"] = cme.latency_total0 - cme.ideal_temporal_cycle
+        la_break_down[idx]["Data loading"] = cme.latency_total1 - cme.latency_total0
+        la_break_down[idx]["Data off-loading"] = cme.latency_total2 - cme.latency_total1
+        la_tot[idx] = cme.latency_total2
         for operand in cme.mem_energy_breakdown_further:
             mem_op = cme.layer.memory_operand_links[operand]
-            operand_memory_levels = mh.get_memory_levels(mem_op)
+            operand_memory_levels = mem_hierarchy.get_memory_levels(mem_op)
             for j in range(len(cme.mem_energy_breakdown_further[operand])):
                 mem = operand_memory_levels[j].name
                 memory_instances[mem] = operand_memory_levels[j]
-                memory_word_access_summed[d][operand][
-                    mem
-                ] += cme.mem_energy_breakdown_further[operand][j]
+                memory_word_access_summed[idx][operand][mem] += cme.mem_energy_breakdown_further[operand][j]
 
-    all_mems = set()
+    all_mems_set: set[str] = set()
     for v in memory_word_access_summed.values():
         for vv in v.values():
             for vvv in vv.keys():
-                all_mems.add(vvv)
-    all_mems = sorted(
-        list(all_mems), key=lambda m: memory_instances[m].memory_instance.size
-    )
-    all_ops = set()
+                all_mems_set.add(vvv)
+    all_mems = sorted(list(all_mems_set), key=lambda m: memory_instances[m].memory_instance.size)
+    all_ops_set: set[LayerOperand] = set()
     for v in memory_word_access_summed.values():
         for vv in v.keys():
-            all_ops.add(vv)
-    all_ops = sorted(list(all_ops))
+            all_ops_set.add(vv)
+    all_ops = sorted(list(all_ops_set))
 
-    """ plotting start """
-    """ Energy part """
+    # plotting start
+    # Energy part
 
     fig, (ax1, ax2) = plt.subplots(nrows=2, figsize=(10, 8))
     hues = np.linspace(0, 1, len(all_ops) + 1)[:-1]
     hatches = ["////", "\\\\\\\\", "xxxx", "++++"]
     x = 0
     xticks = {}
-    for d, cme in enumerate(cmes):
+    for idx, cme in enumerate(cmes):
         total_energy = 0
         startx_of_layer = x
         # mac
-        ax1.bar([x], [mac_costs[d]], width=1, bottom=0, facecolor="k")
-        total_energy += mac_costs[d]
-        highest_bar = mac_costs[d]
+        ax1.bar([x], [mac_costs[idx]], width=1, bottom=0, facecolor="k")
+        total_energy += mac_costs[idx]
+        highest_bar = mac_costs[idx]
         xticks[x] = "MAC"
         x += 1
         # mems
         for mem in all_mems:
             bottom = 0
             for op_i, operand in enumerate(all_ops):
-                for dir_i, dir in enumerate(memory_word_access_summed[d][operand][mem]):
-                    height = memory_word_access_summed[d][operand][mem][dir]
+                for dir_idx, direction in enumerate(DataDirection):
+                    data_movement = memory_word_access_summed[idx][operand][mem]
+                    height = data_movement.get_single_dir_data(direction)
                     ax1.bar(
                         [x],
                         [height],
                         width=1,
                         bottom=[bottom],
                         facecolor=hsv_to_rgb((hues[op_i], 1, 1)),
-                        hatch=hatches[dir_i],
+                        hatch=hatches[dir_idx],
                     )
 
                     bottom += height
             xticks[x] = mem
             total_energy += bottom
             x += 1
             highest_bar = max(bottom, highest_bar)
-        x
+
         ax1.text(
             x * 0.5 + startx_of_layer * 0.5,
             1.05 * highest_bar,
             "tot:{:,d}".format(int(total_energy)),
             horizontalalignment="center",
             verticalalignment="bottom",
             weight="bold",
         )
         x += len(all_mems) / 4
 
     for op, h in zip(all_ops, hues):
         ax1.bar(0, 0, width=1, facecolor=hsv_to_rgb((h, 1, 1)), label=op)
 
-    for dir_i, dir in enumerate(memory_word_access_summed[d][operand][mem]):
+    for idx, direction in enumerate(DataDirection):
         ax1.bar(
             [0],
             [0],
             width=1,
             bottom=0,
             facecolor=(1, 1, 1),
-            hatch=hatches[dir_i],
-            label=dir,
+            hatch=hatches[idx],
+            label=str(direction),
         )
 
     ax1.legend(loc="upper left")
     ax1.set_xticks(list(xticks.keys()), list(xticks.values()), rotation=xtick_rotation)
     ax1.set_ylim(0, 1.1 * ax1.get_ylim()[1])
 
     ax1.set_ylabel("Energy (pJ)", fontsize=15)
 
-    """ Latency part """
+    # Latency part
     x2 = list(range(len(la_break_down)))
 
     y2 = {ky: [] for ky in la_break_down[0].keys()}
     for _, design_point in la_break_down.items():
         for ky, val in design_point.items():
             y2[ky].append(val)
 
@@ -250,14 +245,15 @@
     ax2.set_xticks(x2, x2, rotation=xtick_rotation)
     ax2.set_ylim(0, 1.1 * ax2.get_ylim()[1])
     ax2.set_xlabel("Layers", fontsize=15)
     ax2.set_ylabel("Latency (cycle)", fontsize=15)
 
     fig.tight_layout()
     plt.savefig(save_path)
+    plt.close()
 
 
 if __name__ == "__main__":
     import pickle
 
     with open("../list_of_cmes.pickle", "rb") as handle:
         list_of_cme = pickle.load(handle)
```

### Comparing `zigzag_dse-3.1.0/zigzag_dse.egg-info/PKG-INFO` & `zigzag_dse-3.1.1/zigzag_dse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigzag-dse
-Version: 3.1.0
+Version: 3.1.1
 Summary: ZigZag - Deep Learning Hardware Design Space Exploration
 Author-email: Arne Symons <arne.symons@kuleuven.be>, Linyan Mei <linyan.mei@kuleuven.be>
 License: MIT License
         
         Copyright (c) 2021 MICAS (KU Leuven)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,26 +25,26 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/ZigZag-Project/zigzag
 Keywords: zigzag,dse,design-space-exploration,machine-learning,deep-learning,mapping
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: networkx
 Requires-Dist: sympy
 Requires-Dist: matplotlib
 Requires-Dist: onnx
 Requires-Dist: tqdm
 Requires-Dist: multiprocessing_on_dill
 Requires-Dist: pyyaml
-Requires-Dist: tomli; python_version < "3.11"
+Requires-Dist: tomli
 Provides-Extra: dev
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # ZigZag [Documentation](https://kuleuven-micas.github.io/zigzag/) [Tutorial](https://www.youtube.com/watch?v=VgUuG4QaSQQ&list=PLUi74Rw4uFDIuK_6FCF9Bv7SMJlHfG4l3&index=1)
```

