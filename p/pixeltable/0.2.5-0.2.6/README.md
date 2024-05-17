# Comparing `tmp/pixeltable-0.2.5.tar.gz` & `tmp/pixeltable-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixeltable-0.2.5.tar", max compression
+gzip compressed data, was "pixeltable-0.2.6.tar", max compression
```

## Comparing `pixeltable-0.2.5.tar` & `pixeltable-0.2.6.tar`

### file list

```diff
@@ -1,139 +1,119 @@
--rw-r--r--   0        0        0      746 2024-03-22 03:20:30.000000 pixeltable-0.2.5/LICENSE
--rw-r--r--   0        0        0     4778 2024-04-26 23:52:15.843337 pixeltable-0.2.5/README.md
--rw-r--r--   0        0        0      959 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/__init__.py
--rw-r--r--   0        0        0      453 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/catalog/__init__.py
--rw-r--r--   0        0        0     7908 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/catalog/catalog.py
--rw-r--r--   0        0        0     7887 2024-04-26 23:52:15.860281 pixeltable-0.2.5/pixeltable/catalog/column.py
--rw-r--r--   0        0        0      919 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/catalog/dir.py
--rw-r--r--   0        0        0      943 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/catalog/globals.py
--rw-r--r--   0        0        0     8303 2024-04-26 23:52:15.860489 pixeltable-0.2.5/pixeltable/catalog/insertable_table.py
--rw-r--r--   0        0        0     1147 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/catalog/named_function.py
--rw-r--r--   0        0        0     1677 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/catalog/path.py
--rw-r--r--   0        0        0     5941 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/catalog/path_dict.py
--rw-r--r--   0        0        0     1059 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/catalog/schema_object.py
--rw-r--r--   0        0        0    30675 2024-04-26 23:52:15.860760 pixeltable-0.2.5/pixeltable/catalog/table.py
--rw-r--r--   0        0        0    48818 2024-04-26 23:52:15.861070 pixeltable-0.2.5/pixeltable/catalog/table_version.py
--rw-r--r--   0        0        0     5482 2024-04-26 23:52:15.861379 pixeltable-0.2.5/pixeltable/catalog/table_version_path.py
--rw-r--r--   0        0        0     9734 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/catalog/view.py
--rw-r--r--   0        0        0    23442 2024-04-26 23:52:15.861740 pixeltable-0.2.5/pixeltable/client.py
--rw-r--r--   0        0        0    30014 2024-04-26 23:52:15.862042 pixeltable-0.2.5/pixeltable/dataframe.py
--rw-r--r--   0        0        0    16303 2024-04-26 23:52:15.862207 pixeltable-0.2.5/pixeltable/env.py
--rw-r--r--   0        0        0      376 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exceptions.py
--rw-r--r--   0        0        0      412 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exec/__init__.py
--rw-r--r--   0        0        0     3321 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/exec/aggregation_node.py
--rw-r--r--   0        0        0     5241 2024-04-26 23:52:15.862576 pixeltable-0.2.5/pixeltable/exec/cache_prefetch_node.py
--rw-r--r--   0        0        0     4069 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exec/component_iteration_node.py
--rw-r--r--   0        0        0     3505 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exec/data_row_batch.py
--rw-r--r--   0        0        0      924 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exec/exec_context.py
--rw-r--r--   0        0        0     2170 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exec/exec_node.py
--rw-r--r--   0        0        0    10810 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/exec/expr_eval_node.py
--rw-r--r--   0        0        0     3171 2024-04-26 23:52:15.862984 pixeltable-0.2.5/pixeltable/exec/in_memory_data_node.py
--rw-r--r--   0        0        0     1514 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exec/media_validation_node.py
--rw-r--r--   0        0        0    10318 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exec/sql_scan_node.py
--rw-r--r--   0        0        0      935 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/exprs/__init__.py
--rw-r--r--   0        0        0     4386 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/arithmetic_expr.py
--rw-r--r--   0        0        0     2131 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/array_slice.py
--rw-r--r--   0        0        0     2706 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/column_property_ref.py
--rw-r--r--   0        0        0     4794 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/column_ref.py
--rw-r--r--   0        0        0     2964 2024-04-26 23:52:15.863463 pixeltable-0.2.5/pixeltable/exprs/comparison.py
--rw-r--r--   0        0        0     3830 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/compound_predicate.py
--rw-r--r--   0        0        0     8278 2024-04-26 23:52:15.863796 pixeltable-0.2.5/pixeltable/exprs/data_row.py
--rw-r--r--   0        0        0    23748 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/exprs/expr.py
--rw-r--r--   0        0        0     1222 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/expr_set.py
--rw-r--r--   0        0        0    16961 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/exprs/function_call.py
--rw-r--r--   0        0        0     1537 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/globals.py
--rw-r--r--   0        0        0     4663 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/image_member_access.py
--rw-r--r--   0        0        0     1906 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/image_similarity_predicate.py
--rw-r--r--   0        0        0     4312 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/inline_array.py
--rw-r--r--   0        0        0     3695 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/inline_dict.py
--rw-r--r--   0        0        0     1041 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/is_null.py
--rw-r--r--   0        0        0     4559 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/json_mapper.py
--rw-r--r--   0        0        0     6526 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/json_path.py
--rw-r--r--   0        0        0     2396 2024-04-26 23:52:15.864641 pixeltable-0.2.5/pixeltable/exprs/literal.py
--rw-r--r--   0        0        0     1250 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/object_ref.py
--rw-r--r--   0        0        0     1859 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/predicate.py
--rw-r--r--   0        0        0    15321 2024-04-26 23:52:15.864817 pixeltable-0.2.5/pixeltable/exprs/row_builder.py
--rw-r--r--   0        0        0     4268 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/rowid_ref.py
--rw-r--r--   0        0        0     1793 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/exprs/type_cast.py
--rw-r--r--   0        0        0     1361 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/exprs/variable.py
--rw-r--r--   0        0        0      269 2024-04-26 23:52:15.864917 pixeltable-0.2.5/pixeltable/ext/__init__.py
--rw-r--r--   0        0        0     3131 2024-04-26 23:52:15.865002 pixeltable-0.2.5/pixeltable/ext/functions/yolox.py
--rw-r--r--   0        0        0      457 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/func/__init__.py
--rw-r--r--   0        0        0     9267 2024-04-26 23:52:15.865380 pixeltable-0.2.5/pixeltable/func/aggregate_function.py
--rw-r--r--   0        0        0     2350 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/func/batched_function.py
--rw-r--r--   0        0        0     2357 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/func/callable_function.py
--rw-r--r--   0        0        0     3807 2024-04-26 23:52:15.865719 pixeltable-0.2.5/pixeltable/func/expr_template_function.py
--rw-r--r--   0        0        0     4023 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/func/function.py
--rw-r--r--   0        0        0    11456 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/func/function_registry.py
--rw-r--r--   0        0        0     1483 2024-04-26 23:52:15.866057 pixeltable-0.2.5/pixeltable/func/globals.py
--rw-r--r--   0        0        0     9650 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/func/nos_function.py
--rw-r--r--   0        0        0     7343 2024-04-26 23:52:15.866428 pixeltable-0.2.5/pixeltable/func/signature.py
--rw-r--r--   0        0        0     6711 2024-04-26 23:52:15.866878 pixeltable-0.2.5/pixeltable/func/udf.py
--rw-r--r--   0        0        0     3297 2024-04-26 23:52:15.866971 pixeltable-0.2.5/pixeltable/functions/__init__.py
--rw-r--r--   0        0        0     8404 2024-04-26 23:52:15.867168 pixeltable-0.2.5/pixeltable/functions/eval.py
--rw-r--r--   0        0        0      908 2024-04-17 01:12:13.000000 pixeltable-0.2.5/pixeltable/functions/fireworks.py
--rw-r--r--   0        0        0     5693 2024-04-26 23:52:15.867554 pixeltable-0.2.5/pixeltable/functions/huggingface.py
--rw-r--r--   0        0        0      431 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/functions/image.py
--rw-r--r--   0        0        0     6870 2024-04-26 23:52:15.867781 pixeltable-0.2.5/pixeltable/functions/openai.py
--rw-r--r--   0        0        0     6217 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/functions/pil/image.py
--rw-r--r--   0        0        0      516 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/functions/string.py
--rw-r--r--   0        0        0     3423 2024-04-17 01:12:13.000000 pixeltable-0.2.5/pixeltable/functions/together.py
--rw-r--r--   0        0        0     1860 2024-04-26 23:52:15.868147 pixeltable-0.2.5/pixeltable/functions/util.py
--rw-r--r--   0        0        0     2403 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/functions/video.py
--rw-r--r--   0        0        0       72 2024-04-26 23:52:15.868217 pixeltable-0.2.5/pixeltable/index/__init__.py
--rw-r--r--   0        0        0     1362 2024-04-26 23:52:15.868269 pixeltable-0.2.5/pixeltable/index/base.py
--rw-r--r--   0        0        0     4372 2024-04-26 23:52:15.868362 pixeltable-0.2.5/pixeltable/index/embedding_index.py
--rw-r--r--   0        0        0       70 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/iterators/__init__.py
--rw-r--r--   0        0        0     1545 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/iterators/base.py
--rw-r--r--   0        0        0    13105 2024-04-08 22:50:04.000000 pixeltable-0.2.5/pixeltable/iterators/document.py
--rw-r--r--   0        0        0     3444 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/iterators/video.py
--rw-r--r--   0        0        0     2083 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/metadata/__init__.py
--rw-r--r--   0        0        0      733 2024-03-22 03:20:30.000000 pixeltable-0.2.5/pixeltable/metadata/converters/convert_10.py
--rw-r--r--   0        0        0     8335 2024-04-26 23:52:15.868900 pixeltable-0.2.5/pixeltable/metadata/schema.py
--rw-r--r--   0        0        0    33549 2024-04-26 23:52:15.869190 pixeltable-0.2.5/pixeltable/plan.py
--rw-r--r--   0        0        0    19426 2024-04-26 23:52:15.869492 pixeltable-0.2.5/pixeltable/store.py
--rw-r--r--   0        0        0     6339 2024-04-26 23:52:15.879933 pixeltable-0.2.5/pixeltable/tests/conftest.py
--rw-r--r--   0        0        0     1085 2024-04-26 23:52:15.883996 pixeltable-0.2.5/pixeltable/tests/ext/test_yolox.py
--rw-r--r--   0        0        0     1690 2024-04-26 23:52:15.884519 pixeltable-0.2.5/pixeltable/tests/functions/test_fireworks.py
--rw-r--r--   0        0        0     2884 2024-04-17 01:12:13.000000 pixeltable-0.2.5/pixeltable/tests/functions/test_functions.py
--rw-r--r--   0        0        0     7657 2024-04-26 23:52:15.884812 pixeltable-0.2.5/pixeltable/tests/functions/test_huggingface.py
--rw-r--r--   0        0        0     8659 2024-04-26 23:52:15.885170 pixeltable-0.2.5/pixeltable/tests/functions/test_openai.py
--rw-r--r--   0        0        0     4812 2024-04-26 23:52:15.885535 pixeltable-0.2.5/pixeltable/tests/functions/test_together.py
--rw-r--r--   0        0        0     3186 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/tests/test_audio.py
--rw-r--r--   0        0        0     1189 2024-03-22 03:20:31.000000 pixeltable-0.2.5/pixeltable/tests/test_catalog.py
--rw-r--r--   0        0        0      531 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/tests/test_client.py
--rw-r--r--   0        0        0    18221 2024-04-26 23:52:15.885726 pixeltable-0.2.5/pixeltable/tests/test_component_view.py
--rw-r--r--   0        0        0    17906 2024-04-26 23:52:15.885857 pixeltable-0.2.5/pixeltable/tests/test_dataframe.py
--rw-r--r--   0        0        0     3611 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/tests/test_dirs.py
--rw-r--r--   0        0        0     5810 2024-04-06 17:38:32.000000 pixeltable-0.2.5/pixeltable/tests/test_document.py
--rw-r--r--   0        0        0    32181 2024-04-26 23:52:15.886175 pixeltable-0.2.5/pixeltable/tests/test_exprs.py
--rw-r--r--   0        0        0    12987 2024-04-26 23:52:15.886344 pixeltable-0.2.5/pixeltable/tests/test_function.py
--rw-r--r--   0        0        0     5410 2024-04-26 23:52:15.886438 pixeltable-0.2.5/pixeltable/tests/test_index.py
--rw-r--r--   0        0        0     1599 2024-04-26 23:52:15.886763 pixeltable-0.2.5/pixeltable/tests/test_migration.py
--rw-r--r--   0        0        0     2649 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/tests/test_nos.py
--rw-r--r--   0        0        0    10331 2024-04-26 23:52:15.887131 pixeltable-0.2.5/pixeltable/tests/test_snapshot.py
--rw-r--r--   0        0        0    56557 2024-04-26 23:52:15.887436 pixeltable-0.2.5/pixeltable/tests/test_table.py
--rw-r--r--   0        0        0     1308 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/tests/test_transactional_directory.py
--rw-r--r--   0        0        0     2045 2024-04-26 23:52:15.887779 pixeltable-0.2.5/pixeltable/tests/test_types.py
--rw-r--r--   0        0        0     7740 2024-04-26 23:52:15.887909 pixeltable-0.2.5/pixeltable/tests/test_video.py
--rw-r--r--   0        0        0    22108 2024-04-26 23:52:15.888166 pixeltable-0.2.5/pixeltable/tests/test_view.py
--rw-r--r--   0        0        0    15106 2024-04-26 23:52:15.888400 pixeltable-0.2.5/pixeltable/tests/utils.py
--rw-r--r--   0        0        0     5842 2024-04-26 23:52:15.888794 pixeltable-0.2.5/pixeltable/tool/create_test_db_dump.py
--rw-r--r--   0        0        0     2899 2024-04-06 17:38:28.000000 pixeltable-0.2.5/pixeltable/tool/create_test_video.py
--rw-r--r--   0        0        0    29929 2024-04-26 23:52:15.888989 pixeltable-0.2.5/pixeltable/type_system.py
--rw-r--r--   0        0        0      439 2024-03-22 03:20:31.000000 pixeltable-0.2.5/pixeltable/utils/__init__.py
--rw-r--r--   0        0        0     3692 2024-04-17 01:12:13.000000 pixeltable-0.2.5/pixeltable/utils/arrow.py
--rw-r--r--   0        0        0      720 2024-03-22 03:20:31.000000 pixeltable-0.2.5/pixeltable/utils/clip.py
--rw-r--r--   0        0        0     5604 2024-03-22 03:20:31.000000 pixeltable-0.2.5/pixeltable/utils/coco.py
--rw-r--r--   0        0        0     1094 2024-03-22 03:20:31.000000 pixeltable-0.2.5/pixeltable/utils/documents.py
--rw-r--r--   0        0        0     7839 2024-03-22 03:20:31.000000 pixeltable-0.2.5/pixeltable/utils/filecache.py
--rw-r--r--   0        0        0      252 2024-03-22 03:20:31.000000 pixeltable-0.2.5/pixeltable/utils/help.py
--rw-r--r--   0        0        0     7005 2024-04-17 01:12:13.000000 pixeltable-0.2.5/pixeltable/utils/hf_datasets.py
--rw-r--r--   0        0        0     3116 2024-03-22 03:20:31.000000 pixeltable-0.2.5/pixeltable/utils/media_store.py
--rw-r--r--   0        0        0     7120 2024-04-17 01:12:13.000000 pixeltable-0.2.5/pixeltable/utils/parquet.py
--rw-r--r--   0        0        0     3483 2024-04-17 01:12:13.000000 pixeltable-0.2.5/pixeltable/utils/pytorch.py
--rw-r--r--   0        0        0      432 2024-03-22 03:20:31.000000 pixeltable-0.2.5/pixeltable/utils/s3.py
--rw-r--r--   0        0        0      765 2024-03-22 03:20:31.000000 pixeltable-0.2.5/pixeltable/utils/sql.py
--rw-r--r--   0        0        0     1349 2024-04-04 00:11:47.000000 pixeltable-0.2.5/pixeltable/utils/transactional_directory.py
--rw-r--r--   0        0        0     3481 2024-04-26 23:52:15.890789 pixeltable-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     6081 1970-01-01 00:00:00.000000 pixeltable-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      746 2024-03-22 03:20:30.000000 pixeltable-0.2.6/LICENSE
+-rw-r--r--   0        0        0     4904 2024-05-17 02:13:16.858634 pixeltable-0.2.6/README.md
+-rw-r--r--   0        0        0     1040 2024-05-17 02:13:16.886391 pixeltable-0.2.6/pixeltable/__init__.py
+-rw-r--r--   0        0        0      112 2024-05-17 02:31:16.433929 pixeltable-0.2.6/pixeltable/__version__.py
+-rw-r--r--   0        0        0      453 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/catalog/__init__.py
+-rw-r--r--   0        0        0     7908 2024-04-04 00:11:47.000000 pixeltable-0.2.6/pixeltable/catalog/catalog.py
+-rw-r--r--   0        0        0     8088 2024-05-07 19:43:59.355517 pixeltable-0.2.6/pixeltable/catalog/column.py
+-rw-r--r--   0        0        0      919 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/catalog/dir.py
+-rw-r--r--   0        0        0      943 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/catalog/globals.py
+-rw-r--r--   0        0        0     8168 2024-05-07 19:43:59.355707 pixeltable-0.2.6/pixeltable/catalog/insertable_table.py
+-rw-r--r--   0        0        0     1147 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/catalog/named_function.py
+-rw-r--r--   0        0        0     1677 2024-04-04 00:11:47.000000 pixeltable-0.2.6/pixeltable/catalog/path.py
+-rw-r--r--   0        0        0     5941 2024-04-04 00:11:47.000000 pixeltable-0.2.6/pixeltable/catalog/path_dict.py
+-rw-r--r--   0        0        0     1059 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/catalog/schema_object.py
+-rw-r--r--   0        0        0    31252 2024-05-16 01:04:50.721865 pixeltable-0.2.6/pixeltable/catalog/table.py
+-rw-r--r--   0        0        0    48865 2024-05-07 19:43:59.356192 pixeltable-0.2.6/pixeltable/catalog/table_version.py
+-rw-r--r--   0        0        0     5482 2024-04-26 23:52:15.861379 pixeltable-0.2.6/pixeltable/catalog/table_version_path.py
+-rw-r--r--   0        0        0     9734 2024-04-04 00:11:47.000000 pixeltable-0.2.6/pixeltable/catalog/view.py
+-rw-r--r--   0        0        0    31922 2024-05-17 02:13:16.887470 pixeltable-0.2.6/pixeltable/dataframe.py
+-rw-r--r--   0        0        0    17971 2024-05-17 02:13:16.888197 pixeltable-0.2.6/pixeltable/env.py
+-rw-r--r--   0        0        0      376 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/exceptions.py
+-rw-r--r--   0        0        0      454 2024-05-07 19:43:59.356809 pixeltable-0.2.6/pixeltable/exec/__init__.py
+-rw-r--r--   0        0        0     3321 2024-04-04 00:11:47.000000 pixeltable-0.2.6/pixeltable/exec/aggregation_node.py
+-rw-r--r--   0        0        0     5241 2024-04-26 23:52:15.862576 pixeltable-0.2.6/pixeltable/exec/cache_prefetch_node.py
+-rw-r--r--   0        0        0     4069 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/exec/component_iteration_node.py
+-rw-r--r--   0        0        0     3392 2024-05-07 19:43:59.356939 pixeltable-0.2.6/pixeltable/exec/data_row_batch.py
+-rw-r--r--   0        0        0      924 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/exec/exec_context.py
+-rw-r--r--   0        0        0     2170 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/exec/exec_node.py
+-rw-r--r--   0        0        0    10856 2024-05-16 01:04:50.729118 pixeltable-0.2.6/pixeltable/exec/expr_eval_node.py
+-rw-r--r--   0        0        0     3171 2024-04-26 23:52:15.862984 pixeltable-0.2.6/pixeltable/exec/in_memory_data_node.py
+-rw-r--r--   0        0        0     1514 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/exec/media_validation_node.py
+-rw-r--r--   0        0        0    10250 2024-05-16 01:04:50.729737 pixeltable-0.2.6/pixeltable/exec/sql_scan_node.py
+-rw-r--r--   0        0        0      951 2024-05-16 01:04:50.729880 pixeltable-0.2.6/pixeltable/exprs/__init__.py
+-rw-r--r--   0        0        0     4386 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/exprs/arithmetic_expr.py
+-rw-r--r--   0        0        0     2131 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/exprs/array_slice.py
+-rw-r--r--   0        0        0     2706 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/exprs/column_property_ref.py
+-rw-r--r--   0        0        0     5333 2024-05-07 19:43:59.357453 pixeltable-0.2.6/pixeltable/exprs/column_ref.py
+-rw-r--r--   0        0        0     2964 2024-04-26 23:52:15.863463 pixeltable-0.2.6/pixeltable/exprs/comparison.py
+-rw-r--r--   0        0        0     3830 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/exprs/compound_predicate.py
+-rw-r--r--   0        0        0     8278 2024-04-26 23:52:15.863796 pixeltable-0.2.6/pixeltable/exprs/data_row.py
+-rw-r--r--   0        0        0    24190 2024-05-16 01:04:50.730131 pixeltable-0.2.6/pixeltable/exprs/expr.py
+-rw-r--r--   0        0        0     1222 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/exprs/expr_set.py
+-rw-r--r--   0        0        0    17207 2024-05-16 01:04:50.730549 pixeltable-0.2.6/pixeltable/exprs/function_call.py
+-rw-r--r--   0        0        0     1537 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/exprs/globals.py
+-rw-r--r--   0        0        0     3547 2024-05-07 19:43:59.358010 pixeltable-0.2.6/pixeltable/exprs/image_member_access.py
+-rw-r--r--   0        0        0     3696 2024-05-16 01:04:50.730652 pixeltable-0.2.6/pixeltable/exprs/in_predicate.py
+-rw-r--r--   0        0        0     4499 2024-05-07 19:43:59.358187 pixeltable-0.2.6/pixeltable/exprs/inline_array.py
+-rw-r--r--   0        0        0     3885 2024-05-07 19:43:59.358321 pixeltable-0.2.6/pixeltable/exprs/inline_dict.py
+-rw-r--r--   0        0        0     1041 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/exprs/is_null.py
+-rw-r--r--   0        0        0     4559 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/exprs/json_mapper.py
+-rw-r--r--   0        0        0     6526 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/exprs/json_path.py
+-rw-r--r--   0        0        0     2396 2024-04-26 23:52:15.864641 pixeltable-0.2.6/pixeltable/exprs/literal.py
+-rw-r--r--   0        0        0     1250 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/exprs/object_ref.py
+-rw-r--r--   0        0        0     1859 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/exprs/predicate.py
+-rw-r--r--   0        0        0    15662 2024-05-07 19:43:59.358548 pixeltable-0.2.6/pixeltable/exprs/row_builder.py
+-rw-r--r--   0        0        0     4268 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/exprs/rowid_ref.py
+-rw-r--r--   0        0        0     2664 2024-05-07 19:43:59.358644 pixeltable-0.2.6/pixeltable/exprs/similarity_expr.py
+-rw-r--r--   0        0        0     1793 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/exprs/type_cast.py
+-rw-r--r--   0        0        0     1361 2024-04-04 00:11:47.000000 pixeltable-0.2.6/pixeltable/exprs/variable.py
+-rw-r--r--   0        0        0      269 2024-04-26 23:52:15.864917 pixeltable-0.2.6/pixeltable/ext/__init__.py
+-rw-r--r--   0        0        0     3131 2024-04-26 23:52:15.865002 pixeltable-0.2.6/pixeltable/ext/functions/yolox.py
+-rw-r--r--   0        0        0      348 2024-05-16 01:04:50.731216 pixeltable-0.2.6/pixeltable/func/__init__.py
+-rw-r--r--   0        0        0     9356 2024-05-07 19:43:59.358828 pixeltable-0.2.6/pixeltable/func/aggregate_function.py
+-rw-r--r--   0        0        0     4612 2024-05-16 01:04:50.731351 pixeltable-0.2.6/pixeltable/func/callable_function.py
+-rw-r--r--   0        0        0     4266 2024-05-07 19:43:59.359292 pixeltable-0.2.6/pixeltable/func/expr_template_function.py
+-rw-r--r--   0        0        0     5611 2024-05-16 01:04:50.731617 pixeltable-0.2.6/pixeltable/func/function.py
+-rw-r--r--   0        0        0    11456 2024-04-04 00:11:47.000000 pixeltable-0.2.6/pixeltable/func/function_registry.py
+-rw-r--r--   0        0        0     1483 2024-04-26 23:52:15.866057 pixeltable-0.2.6/pixeltable/func/globals.py
+-rw-r--r--   0        0        0     9650 2024-04-04 00:11:47.000000 pixeltable-0.2.6/pixeltable/func/nos_function.py
+-rw-r--r--   0        0        0     6697 2024-05-07 19:43:59.359623 pixeltable-0.2.6/pixeltable/func/signature.py
+-rw-r--r--   0        0        0     6484 2024-05-16 01:04:50.731811 pixeltable-0.2.6/pixeltable/func/udf.py
+-rw-r--r--   0        0        0     3297 2024-04-26 23:52:15.866971 pixeltable-0.2.6/pixeltable/functions/__init__.py
+-rw-r--r--   0        0        0     8404 2024-04-26 23:52:15.867168 pixeltable-0.2.6/pixeltable/functions/eval.py
+-rw-r--r--   0        0        0      908 2024-04-17 01:12:13.000000 pixeltable-0.2.6/pixeltable/functions/fireworks.py
+-rw-r--r--   0        0        0     6458 2024-05-16 01:04:50.731955 pixeltable-0.2.6/pixeltable/functions/huggingface.py
+-rw-r--r--   0        0        0      431 2024-04-04 00:11:47.000000 pixeltable-0.2.6/pixeltable/functions/image.py
+-rw-r--r--   0        0        0     7972 2024-05-16 01:04:50.732101 pixeltable-0.2.6/pixeltable/functions/openai.py
+-rw-r--r--   0        0        0     5992 2024-05-16 01:04:50.732257 pixeltable-0.2.6/pixeltable/functions/pil/image.py
+-rw-r--r--   0        0        0      516 2024-04-04 00:11:47.000000 pixeltable-0.2.6/pixeltable/functions/string.py
+-rw-r--r--   0        0        0     4173 2024-05-16 01:04:50.732536 pixeltable-0.2.6/pixeltable/functions/together.py
+-rw-r--r--   0        0        0     1860 2024-04-26 23:52:15.868147 pixeltable-0.2.6/pixeltable/functions/util.py
+-rw-r--r--   0        0        0     2403 2024-04-04 00:11:47.000000 pixeltable-0.2.6/pixeltable/functions/video.py
+-rw-r--r--   0        0        0    13606 2024-05-17 02:13:16.888463 pixeltable-0.2.6/pixeltable/globals.py
+-rw-r--r--   0        0        0       72 2024-04-26 23:52:15.868217 pixeltable-0.2.6/pixeltable/index/__init__.py
+-rw-r--r--   0        0        0     1431 2024-05-07 19:43:59.360549 pixeltable-0.2.6/pixeltable/index/base.py
+-rw-r--r--   0        0        0     7565 2024-05-07 19:43:59.360688 pixeltable-0.2.6/pixeltable/index/embedding_index.py
+-rw-r--r--   0        0        0      148 2024-05-17 02:13:16.888548 pixeltable-0.2.6/pixeltable/io/__init__.py
+-rw-r--r--   0        0        0     8004 2024-05-17 02:13:16.888631 pixeltable-0.2.6/pixeltable/io/hf_datasets.py
+-rw-r--r--   0        0        0     6478 2024-05-17 02:13:16.888692 pixeltable-0.2.6/pixeltable/io/pandas.py
+-rw-r--r--   0        0        0     8150 2024-05-17 02:13:16.888760 pixeltable-0.2.6/pixeltable/io/parquet.py
+-rw-r--r--   0        0        0      108 2024-05-17 02:13:16.890972 pixeltable-0.2.6/pixeltable/iterators/__init__.py
+-rw-r--r--   0        0        0     1676 2024-05-17 02:13:16.891872 pixeltable-0.2.6/pixeltable/iterators/base.py
+-rw-r--r--   0        0        0    19318 2024-05-17 02:13:16.891996 pixeltable-0.2.6/pixeltable/iterators/document.py
+-rw-r--r--   0        0        0     3474 2024-05-17 02:13:16.892721 pixeltable-0.2.6/pixeltable/iterators/video.py
+-rw-r--r--   0        0        0     2227 2024-05-16 01:04:50.732917 pixeltable-0.2.6/pixeltable/metadata/__init__.py
+-rw-r--r--   0        0        0      733 2024-03-22 03:20:30.000000 pixeltable-0.2.6/pixeltable/metadata/converters/convert_10.py
+-rw-r--r--   0        0        0      107 2024-05-16 01:04:50.733029 pixeltable-0.2.6/pixeltable/metadata/converters/convert_12.py
+-rw-r--r--   0        0        0     1366 2024-05-16 01:04:50.733088 pixeltable-0.2.6/pixeltable/metadata/converters/convert_13.py
+-rw-r--r--   0        0        0     8335 2024-04-26 23:52:15.868900 pixeltable-0.2.6/pixeltable/metadata/schema.py
+-rw-r--r--   0        0        0    32342 2024-05-07 19:43:59.361515 pixeltable-0.2.6/pixeltable/plan.py
+-rw-r--r--   0        0        0    19394 2024-05-16 01:04:50.733331 pixeltable-0.2.6/pixeltable/store.py
+-rw-r--r--   0        0        0     6847 2024-05-16 01:04:50.733646 pixeltable-0.2.6/pixeltable/tool/create_test_db_dump.py
+-rw-r--r--   0        0        0     2899 2024-04-06 17:38:28.000000 pixeltable-0.2.6/pixeltable/tool/create_test_video.py
+-rw-r--r--   0        0        0    29224 2024-05-16 01:04:50.733857 pixeltable-0.2.6/pixeltable/type_system.py
+-rw-r--r--   0        0        0      439 2024-03-22 03:20:31.000000 pixeltable-0.2.6/pixeltable/utils/__init__.py
+-rw-r--r--   0        0        0     3692 2024-04-17 01:12:13.000000 pixeltable-0.2.6/pixeltable/utils/arrow.py
+-rw-r--r--   0        0        0      720 2024-03-22 03:20:31.000000 pixeltable-0.2.6/pixeltable/utils/clip.py
+-rw-r--r--   0        0        0     5604 2024-03-22 03:20:31.000000 pixeltable-0.2.6/pixeltable/utils/coco.py
+-rw-r--r--   0        0        0     2213 2024-05-17 02:13:16.893072 pixeltable-0.2.6/pixeltable/utils/documents.py
+-rw-r--r--   0        0        0     7839 2024-03-22 03:20:31.000000 pixeltable-0.2.6/pixeltable/utils/filecache.py
+-rw-r--r--   0        0        0      252 2024-03-22 03:20:31.000000 pixeltable-0.2.6/pixeltable/utils/help.py
+-rw-r--r--   0        0        0     2422 2024-05-07 19:43:59.385376 pixeltable-0.2.6/pixeltable/utils/http_server.py
+-rw-r--r--   0        0        0     3116 2024-03-22 03:20:31.000000 pixeltable-0.2.6/pixeltable/utils/media_store.py
+-rw-r--r--   0        0        0     3483 2024-04-17 01:12:13.000000 pixeltable-0.2.6/pixeltable/utils/pytorch.py
+-rw-r--r--   0        0        0      432 2024-03-22 03:20:31.000000 pixeltable-0.2.6/pixeltable/utils/s3.py
+-rw-r--r--   0        0        0      765 2024-03-22 03:20:31.000000 pixeltable-0.2.6/pixeltable/utils/sql.py
+-rw-r--r--   0        0        0     1349 2024-04-04 00:11:47.000000 pixeltable-0.2.6/pixeltable/utils/transactional_directory.py
+-rw-r--r--   0        0        0     4061 2024-05-17 02:31:16.433471 pixeltable-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     6317 1970-01-01 00:00:00.000000 pixeltable-0.2.6/PKG-INFO
```

### Comparing `pixeltable-0.2.5/LICENSE` & `pixeltable-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/README.md` & `pixeltable-0.2.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <div align="center">
-<img src="docs/pixeltable-banner.png" width="45%"/>
+<img src="https://raw.githubusercontent.com/pixeltable/pixeltable/master/docs/pixeltable-banner.png" alt="Pixeltable" width="45%" />
 
 # Unifying Data, Models, and Orchestration for AI Products
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 &nbsp;&nbsp;
-![pytest status](https://github.com/pixeltable/pixeltable/actions/workflows/pytest.yml/badge.svg)
+[![pytest status](https://github.com/pixeltable/pixeltable/actions/workflows/pytest.yml/badge.svg)](https://github.com/pixeltable/pixeltable/actions)
 
 [Installation](https://pixeltable.github.io/pixeltable/getting-started/) | [Documentation](https://pixeltable.github.io/pixeltable/)
 </div>
 
 Pixeltable is a Python library that lets AI engineers and data scientists focus on exploration, modeling, and app development without dealing with the customary data plumbing.
 
 ## What problems does Pixeltable solve?
@@ -37,15 +37,15 @@
 pip install pixeltable
 ```
 
 To verify that it's working:
 
 ```
 import pixeltable as pxt
-cl = pxt.Client()
+pxt.init()
 ```
 
 For more detailed installation instructions, see the
 [Getting Started with Pixeltable](https://pixeltable.github.io/pixeltable/getting-started/)
 guide. Then, check out the
 [Pixeltable Basics](https://pixeltable.github.io/pixeltable/tutorials/pixeltable-basics/)
 tutorial for a tour of its most important features.
```

### Comparing `pixeltable-0.2.5/pixeltable/__init__.py` & `pixeltable-0.2.6/pixeltable/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 from .catalog import Column, Table, InsertableTable, View
-from .client import Client
 from .dataframe import DataFrame
 from .exceptions import Error, Error
 from .exprs import RELATIVE_PATH_ROOT
 from .func import Function, udf, uda, Aggregator, expr_udf
-from .type_system import \
-    ColumnType, StringType, IntType, FloatType, BoolType, TimestampType, JsonType, ArrayType, ImageType, VideoType, \
-    AudioType, DocumentType
+from .globals import *
+from .type_system import (
+    ColumnType,
+    StringType,
+    IntType,
+    FloatType,
+    BoolType,
+    TimestampType,
+    JsonType,
+    ArrayType,
+    ImageType,
+    VideoType,
+    AudioType,
+    DocumentType,
+)
 from .utils.help import help
+
 # noinspection PyUnresolvedReferences
-from . import functions
+from . import functions, io
+from .__version__ import __version__, __version_tuple__
 
 __all__ = [
-    'Client',
     'DataFrame',
     'Column',
     'Table',
     'InsertableTable',
     'View',
     'Error',
     'ColumnType',
@@ -35,10 +47,7 @@
     'Function',
     'help',
     'udf',
     'Aggregator',
     'uda',
     'expr_udf',
 ]
-
-
-
```

### Comparing `pixeltable-0.2.5/pixeltable/catalog/catalog.py` & `pixeltable-0.2.6/pixeltable/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/catalog/column.py` & `pixeltable-0.2.6/pixeltable/catalog/column.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from __future__ import annotations
 
 import logging
 from typing import Optional, Union, Callable, Set
 
 import sqlalchemy as sql
 
-from pixeltable import exceptions as excs
-from pixeltable.type_system import ColumnType, StringType
+import pixeltable.exceptions as excs
+import pixeltable.type_system as ts
 from .globals import is_valid_identifier
 
 _logger = logging.getLogger('pixeltable')
 
 class Column:
     """Representation of a column in the schema of a Table/DataFrame.
 
     A Column contains all the metadata necessary for executing queries and updates against a particular version of a
     table/view.
     """
     def __init__(
-            self, name: Optional[str], col_type: Optional[ColumnType] = None,
+            self, name: Optional[str], col_type: Optional[ts.ColumnType] = None,
             computed_with: Optional[Union['Expr', Callable]] = None,
             is_pk: bool = False, stored: Optional[bool] = None,
             col_id: Optional[int] = None, schema_version_add: Optional[int] = None,
             schema_version_drop: Optional[int] = None, sa_col_type: Optional[sql.sqltypes.TypeEngine] = None
     ):
         """Column constructor.
 
@@ -110,14 +110,18 @@
     def has_window_fn_call(self) -> bool:
         if self.value_expr is None:
             return False
         from pixeltable import exprs
         l = list(self.value_expr.subexprs(filter=lambda e: isinstance(e, exprs.FunctionCall) and e.is_window_fn_call))
         return len(l) > 0
 
+    def get_idx_info(self) -> dict[str, 'pixeltable.catalog.TableVersion.IndexInfo']:
+        assert self.tbl is not None
+        return {name: info for name, info in self.tbl.idxs_by_name.items() if info.col == self}
+
     @property
     def is_computed(self) -> bool:
         return self.compute_func is not None or self.value_expr is not None
 
     @property
     def is_stored(self) -> bool:
         """Returns True if column is materialized in the stored table."""
@@ -144,16 +148,16 @@
         """
         assert self.is_stored
         # all storage columns are nullable (we deal with null errors in Pixeltable directly)
         self.sa_col = sql.Column(
             self.store_name(), self.col_type.to_sa_type() if self.sa_col_type is None else self.sa_col_type,
             nullable=True)
         if self.is_computed or self.col_type.is_media_type():
-            self.sa_errormsg_col = sql.Column(self.errormsg_store_name(), StringType().to_sa_type(), nullable=True)
-            self.sa_errortype_col = sql.Column(self.errortype_store_name(), StringType().to_sa_type(), nullable=True)
+            self.sa_errormsg_col = sql.Column(self.errormsg_store_name(), ts.StringType().to_sa_type(), nullable=True)
+            self.sa_errortype_col = sql.Column(self.errortype_store_name(), ts.StringType().to_sa_type(), nullable=True)
 
     def get_sa_col_type(self) -> sql.sqltypes.TypeEngine:
         return self.col_type.to_sa_type() if self.sa_col_type is None else self.sa_col_type
 
     def store_name(self) -> str:
         assert self.id is not None
         assert self.is_stored
```

### Comparing `pixeltable-0.2.5/pixeltable/catalog/dir.py` & `pixeltable-0.2.6/pixeltable/catalog/dir.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/catalog/globals.py` & `pixeltable-0.2.6/pixeltable/catalog/globals.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/catalog/insertable_table.py` & `pixeltable-0.2.6/pixeltable/catalog/insertable_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,12 @@
         """
         from pixeltable.exprs import Predicate
         from pixeltable.plan import Planner
         if where is not None:
             if not isinstance(where, Predicate):
                 raise excs.Error(f"'where' argument must be a Predicate, got {type(where)}")
             analysis_info = Planner.analyze(self.tbl_version_path, where)
-            if analysis_info.similarity_clause is not None:
-                raise excs.Error('nearest() cannot be used with delete()')
             # for now we require that the updated rows can be identified via SQL, rather than via a Python filter
             if analysis_info.filter is not None:
                 raise excs.Error(f'Filter {analysis_info.filter} not expressible in SQL')
 
         return self.tbl_version.delete(where)
```

### Comparing `pixeltable-0.2.5/pixeltable/catalog/named_function.py` & `pixeltable-0.2.6/pixeltable/catalog/named_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/catalog/path.py` & `pixeltable-0.2.6/pixeltable/catalog/path.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/catalog/path_dict.py` & `pixeltable-0.2.6/pixeltable/catalog/path_dict.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/catalog/schema_object.py` & `pixeltable-0.2.6/pixeltable/catalog/schema_object.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/catalog/table.py` & `pixeltable-0.2.6/pixeltable/catalog/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,14 +93,19 @@
     def order_by(self, *items: 'exprs.Expr', asc: bool = True) -> 'pixeltable.dataframe.DataFrame':
         """Return a DataFrame for this table.
         """
         # local import: avoid circular imports
         from pixeltable.dataframe import DataFrame
         return DataFrame(self.tbl_version_path).order_by(*items, asc=asc)
 
+    def group_by(self, *items: 'exprs.Expr') -> 'pixeltable.dataframe.DataFrame':
+        """Return a DataFrame for this table."""
+        from pixeltable.dataframe import DataFrame
+        return DataFrame(self.tbl_version_path).group_by(*items)
+
     def collect(self) -> 'pixeltable.dataframe.DataFrameResultSet':  # type: ignore[name-defined, no-untyped-def]
         """Return rows from this table.
         """
         return self.df().collect()
 
     def show(
             self, *args, **kwargs
@@ -466,45 +471,50 @@
             >>> tbl.rename_column('factorial', 'fac')
         """
         self._check_is_dropped()
         self.tbl_version_path.tbl_version.rename_column(old_name, new_name)
 
     def add_embedding_index(
             self, col_name: str, *, idx_name: Optional[str] = None,
-            text_embed: Optional[pixeltable.Function] = None, img_embed: Optional[pixeltable.Function] = None
+            text_embed: Optional[pixeltable.Function] = None, img_embed: Optional[pixeltable.Function] = None,
+            metric: str = 'cosine'
     ) -> None:
         """Add an index to the table.
         Args:
             col_name: name of column to index
             idx_name: name of index, which needs to be unique for the table; if not provided, a name will be generated
-            idx_type: type of index (one of 'embedding')
+            text_embed: function to embed text; required if the column is a text column
+            img_embed: function to embed images; required if the column is an image column
+            metric: distance metric to use for the index; one of 'cosine', 'ip', 'l2'; default is 'cosine'
 
         Raises:
             Error: If an index with that name already exists for the table or if the column does not exist.
 
         Examples:
             Add an index to the ``img`` column:
 
-            >>> tbl.add_embedding_index('img', text_embed=...)
+            >>> tbl.add_embedding_index('img', img_embed=...)
 
-            Add another index to the ``img`` column, with a specific name:
+            Add another index to the ``img`` column, using the inner product as the distance metric,
+            and with a specific name; ``text_embed`` is also specified in order to search with text:
 
-            >>> tbl.add_embedding_index('img', idx_name='clip_idx', text_embed=...)
+            >>> tbl.add_embedding_index(
+                'img', idx_name='clip_idx', img_embed=..., text_embed=...text_embed..., metric='ip')
         """
         if self.tbl_version_path.is_snapshot():
             raise excs.Error('Cannot add an index to a snapshot')
         self._check_is_dropped()
         col = self.tbl_version_path.get_column(col_name, include_bases=True)
         if col is None:
             raise excs.Error(f'Column {col_name} unknown')
         if idx_name is not None and idx_name in self.tbl_version_path.tbl_version.idxs_by_name:
             raise excs.Error(f'Duplicate index name: {idx_name}')
         from pixeltable.index import EmbeddingIndex
         # create the EmbeddingIndex instance to verify args
-        idx = EmbeddingIndex(col, text_embed=text_embed, img_embed=img_embed)
+        idx = EmbeddingIndex(col, metric=metric, text_embed=text_embed, img_embed=img_embed)
         status = self.tbl_version_path.tbl_version.add_index(col, idx_name=idx_name, idx=idx)
         # TODO: how to deal with exceptions here? drop the index and raise?
 
     def drop_index(self, *, column_name: Optional[str] = None, idx_name: Optional[str] = None) -> None:
         """Drop an index from the table.
 
         Args:
@@ -578,16 +588,14 @@
 
         update_spec = self._validate_update_spec(value_spec, allow_pk=False, allow_exprs=True)
         from pixeltable.plan import Planner
         if where is not None:
             if not isinstance(where, exprs.Predicate):
                 raise excs.Error(f"'where' argument must be a Predicate, got {type(where)}")
             analysis_info = Planner.analyze(self.tbl_version_path, where)
-            if analysis_info.similarity_clause is not None:
-                raise excs.Error('nearest() cannot be used with update()')
             # for now we require that the updated rows can be identified via SQL, rather than via a Python filter
             if analysis_info.filter is not None:
                 raise excs.Error(f'Filter {analysis_info.filter} not expressible in SQL')
 
         return self.tbl_version_path.tbl_version.update(update_spec, where, cascade)
 
     def batch_update(self, rows: Iterable[dict[str, Any]], cascade: bool = True) -> UpdateStatus:
```

### Comparing `pixeltable-0.2.5/pixeltable/catalog/table_version.py` & `pixeltable-0.2.6/pixeltable/catalog/table_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
       * TODO: create a separate hierarchy of objects that records the version-independent tree of tables/views, and
         have TableVersions reference those
     - mutable TableVersions record their TableVersionPath, which is needed for expr evaluation in updates
     """
     @dataclasses.dataclass
     class IndexInfo:
         id: int
+        name: str
         idx: index.IndexBase
         col: Column
         val_col: Column
         undo_col: Column
 
 
     def __init__(
@@ -268,15 +269,15 @@
             idx = cls.from_dict(idx_col, md.init_args)
 
             # fix up the sa column type of the index value and undo columns
             val_col = self.cols_by_id[md.index_val_col_id]
             val_col.sa_col_type = idx.index_sa_type()
             undo_col = self.cols_by_id[md.index_val_undo_col_id]
             undo_col.sa_col_type = idx.index_sa_type()
-            idx_info = self.IndexInfo(id=md.id, idx=idx, col=idx_col, val_col=val_col, undo_col=undo_col)
+            idx_info = self.IndexInfo(id=md.id, name=md.name, idx=idx, col=idx_col, val_col=val_col, undo_col=undo_col)
             self.idxs_by_name[md.name] = idx_info
 
     def _init_sa_schema(self) -> None:
         # create the sqlalchemy schema; do this after instantiating columns, in order to determine whether they
         # need to record errors
         from pixeltable.store import StoreBase, StoreTable, StoreView, StoreComponentView
         if self.is_component_view():
@@ -349,15 +350,15 @@
             # create and register the index metadata
             idx_cls = type(idx)
             idx_md = schema.IndexMd(
                 id=idx_id, name=idx_name,
                 indexed_col_id=col.id, index_val_col_id=val_col.id, index_val_undo_col_id=undo_col.id,
                 schema_version_add=self.schema_version, schema_version_drop=None,
                 class_fqn=idx_cls.__module__ + '.' + idx_cls.__name__, init_args=idx.as_dict())
-            idx_info = self.IndexInfo(id=idx_id, idx=idx, col=col, val_col=val_col, undo_col=undo_col)
+            idx_info = self.IndexInfo(id=idx_id, name=idx_name, idx=idx, col=col, val_col=val_col, undo_col=undo_col)
             self.idx_md[idx_id] = idx_md
             self.idxs_by_name[idx_name] = idx_info
 
             # add the columns and update the metadata
             status = self._add_columns([val_col, undo_col], conn, preceding_schema_version=preceding_schema_version)
             # now create the index structure
             idx.create_index(self._store_idx_name(idx_id), val_col, conn)
```

### Comparing `pixeltable-0.2.5/pixeltable/catalog/table_version_path.py` & `pixeltable-0.2.6/pixeltable/catalog/table_version_path.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/catalog/view.py` & `pixeltable-0.2.6/pixeltable/catalog/view.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/dataframe.py` & `pixeltable-0.2.6/pixeltable/dataframe.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,42 +22,39 @@
 import pixeltable.exceptions as excs
 import pixeltable.exprs as exprs
 import pixeltable.type_system as ts
 from pixeltable.catalog import is_valid_identifier
 from pixeltable.env import Env
 from pixeltable.plan import Planner
 from pixeltable.type_system import ColumnType
+from pixeltable.utils.http_server import get_file_uri
 
-__all__ = [
-    'DataFrame'
-]
+__all__ = ['DataFrame']
 
 _logger = logging.getLogger('pixeltable')
 
 
 def _create_source_tag(file_path: str) -> str:
-    abs_path = Path(file_path)
-    assert abs_path.is_absolute()
-    src_url = f'{Env.get().http_address}/{abs_path}'
+    src_url = get_file_uri(Env.get().http_address, file_path)
     mime = mimetypes.guess_type(src_url)[0]
     # if mime is None, the attribute string would not be valid html.
     mime_attr = f'type="{mime}"' if mime is not None else ''
     return f'<source src="{src_url}" {mime_attr} />'
 
 
 class DataFrameResultSet:
-
     def __init__(self, rows: List[List[Any]], col_names: List[str], col_types: List[ColumnType]):
         self._rows = rows
         self._col_names = col_names
         self._col_types = col_types
         self._formatters = {
             ts.ImageType: self._format_img,
             ts.VideoType: self._format_video,
             ts.AudioType: self._format_audio,
+            ts.DocumentType: self._format_document,
         }
 
     def __len__(self) -> int:
         return len(self._rows)
 
     def column_names(self) -> List[str]:
         return self._col_names
@@ -86,15 +83,14 @@
     def to_pandas(self) -> pd.DataFrame:
         return pd.DataFrame.from_records(self._rows, columns=self._col_names)
 
     def _row_to_dict(self, row_idx: int) -> Dict[str, Any]:
         return {self._col_names[i]: self._rows[row_idx][i] for i in range(len(self._col_names))}
 
     # Formatters
-
     def _format_img(self, img: Image.Image) -> str:
         """
         Create <img> tag for Image object.
         """
         assert isinstance(img, Image.Image), f'Wrong type: {type(img)}'
         # Try to make it look decent in a variety of display scenarios
         if len(self._rows) > 1:
@@ -102,22 +98,22 @@
         elif len(self._col_names) > 1:
             width = 480  # Multiple columns: display medium images
         else:
             width = 640  # A single image: larger display
         with io.BytesIO() as buffer:
             img.save(buffer, 'jpeg')
             img_base64 = base64.b64encode(buffer.getvalue()).decode()
-            return f'''
-            <div style="width:{width}px;">
+            return f"""
+            <div class="pxt_image" style="width:{width}px;">
                 <img src="data:image/jpeg;base64,{img_base64}" width="{width}" />
             </div>
-            '''
+            """
 
     def _format_video(self, file_path: str) -> str:
-        thumb_tag = ""
+        thumb_tag = ''
         # Attempt to extract the first frame of the video to use as a thumbnail,
         # so that the notebook can be exported as HTML and viewed in contexts where
         # the video itself is not accessible.
         # TODO(aaron-siegel): If the video is backed by a concrete external URL,
         # should we link to that instead?
         video_reader = cv2.VideoCapture(str(file_path))
         if video_reader.isOpened():
@@ -132,24 +128,61 @@
             video_reader.release()
         if len(self._rows) > 1:
             width = 320
         elif len(self._col_names) > 1:
             width = 480
         else:
             width = 800
-        return f'''
-        <div style="width:{width}px;">
+        return f"""
+        <div class="pxt_video" style="width:{width}px;">
             <video controls width="{width}" {thumb_tag}>
                 {_create_source_tag(file_path)}
             </video>
         </div>
-        '''
+        """
+
+    def _format_document(self, file_path: str) -> str:
+        max_width = max_height = 320
+        # by default, file path will be shown as a link
+        inner_element = file_path
+        # try generating a thumbnail for different types and use that if successful
+        if file_path.lower().endswith('.pdf'):
+            try:
+                import fitz
+
+                doc = fitz.open(file_path)
+                p = doc.get_page_pixmap(0)
+                while p.width > max_width or p.height > max_height:
+                    # shrink(1) will halve each dimension
+                    p.shrink(1)
+                data = p.tobytes(output='jpeg')
+                thumb_base64 = base64.b64encode(data).decode()
+                img_src = f'data:image/jpeg;base64,{thumb_base64}'
+                inner_element = f"""
+                    <img style="object-fit: contain; border: 1px solid black;" src="{img_src}" />
+                """
+            except:
+                logging.warning(f'Failed to produce PDF thumbnail {file_path}. Make sure you have PyMuPDF installed.')
+
+        return f"""
+        <div class="pxt_document" style="width:{max_width}px;">
+            <a href="{get_file_uri(Env.get().http_address, file_path)}">
+                {inner_element}
+            </a>
+        </div>
+        """
 
     def _format_audio(self, file_path: str) -> str:
-        return f'<audio controls>{_create_source_tag(file_path)}</audio>'
+        return f"""
+        <div class="pxt_audio">
+            <audio controls>
+                {_create_source_tag(file_path)}
+            </audio>
+        </div>
+        """
 
     def __getitem__(self, index: Any) -> Any:
         if isinstance(index, str):
             if index not in self._col_names:
                 raise excs.Error(f'Invalid column name: {index}')
             col_idx = self._col_names.index(index)
             return [row[col_idx] for row in self._rows]
@@ -182,59 +215,61 @@
         if self._idx >= len(self._result_set):
             raise StopIteration
         row = self._result_set._row_to_dict(self._idx)
         self._idx += 1
         return row
 
 
-# TODO: remove this; it's only here as a reminder that we still need to call release() in the current implementation
-class AnalysisInfo:
-    def __init__(self, tbl: catalog.TableVersion):
-        self.tbl = tbl
-        # output of the SQL scan stage
-        self.sql_scan_output_exprs: List[exprs.Expr] = []
-        # output of the agg stage
-        self.agg_output_exprs: List[exprs.Expr] = []
-        # Where clause of the Select stmt of the SQL scan stage
-        self.sql_where_clause: Optional[sql.ClauseElement] = None
-        # filter predicate applied to input rows of the SQL scan stage
-        self.filter: Optional[exprs.Predicate] = None
-        self.similarity_clause: Optional[exprs.ImageSimilarityPredicate] = None
-        self.agg_fn_calls: List[exprs.FunctionCall] = []  # derived from unique_exprs
-        self.has_frame_col: bool = False  # True if we're referencing the frame col
-
-        self.evaluator: Optional[exprs.Evaluator] = None
-        self.sql_scan_eval_ctx: List[exprs.Expr] = []  # needed to materialize output of SQL scan stage
-        self.agg_eval_ctx: List[exprs.Expr] = []  # needed to materialize output of agg stage
-        self.filter_eval_ctx: List[exprs.Expr] = []
-        self.group_by_eval_ctx: List[exprs.Expr] = []
-
-    def finalize_exec(self) -> None:
-        """
-        Call release() on all collected Exprs.
-        """
-        exprs.Expr.release_list(self.sql_scan_output_exprs)
-        exprs.Expr.release_list(self.agg_output_exprs)
-        if self.filter is not None:
-            self.filter.release()
+# # TODO: remove this; it's only here as a reminder that we still need to call release() in the current implementation
+# class AnalysisInfo:
+#     def __init__(self, tbl: catalog.TableVersion):
+#         self.tbl = tbl
+#         # output of the SQL scan stage
+#         self.sql_scan_output_exprs: List[exprs.Expr] = []
+#         # output of the agg stage
+#         self.agg_output_exprs: List[exprs.Expr] = []
+#         # Where clause of the Select stmt of the SQL scan stage
+#         self.sql_where_clause: Optional[sql.ClauseElement] = None
+#         # filter predicate applied to input rows of the SQL scan stage
+#         self.filter: Optional[exprs.Predicate] = None
+#         self.similarity_clause: Optional[exprs.ImageSimilarityPredicate] = None
+#         self.agg_fn_calls: List[exprs.FunctionCall] = []  # derived from unique_exprs
+#         self.has_frame_col: bool = False  # True if we're referencing the frame col
+#
+#         self.evaluator: Optional[exprs.Evaluator] = None
+#         self.sql_scan_eval_ctx: List[exprs.Expr] = []  # needed to materialize output of SQL scan stage
+#         self.agg_eval_ctx: List[exprs.Expr] = []  # needed to materialize output of agg stage
+#         self.filter_eval_ctx: List[exprs.Expr] = []
+#         self.group_by_eval_ctx: List[exprs.Expr] = []
+#
+#     def finalize_exec(self) -> None:
+#         """
+#         Call release() on all collected Exprs.
+#         """
+#         exprs.Expr.release_list(self.sql_scan_output_exprs)
+#         exprs.Expr.release_list(self.agg_output_exprs)
+#         if self.filter is not None:
+#             self.filter.release()
 
 
 class DataFrame:
     def __init__(
-            self, tbl: catalog.TableVersionPath,
-            select_list: Optional[List[Tuple[exprs.Expr, Optional[str]]]] = None,
-            where_clause: Optional[exprs.Predicate] = None,
-            group_by_clause: Optional[List[exprs.Expr]] = None,
-            grouping_tbl: Optional[catalog.TableVersion] = None,
-            order_by_clause: Optional[List[Tuple[exprs.Expr, bool]]] = None,  # List[(expr, asc)]
-            limit: Optional[int] = None):
+        self,
+        tbl: catalog.TableVersionPath,
+        select_list: Optional[List[Tuple[exprs.Expr, Optional[str]]]] = None,
+        where_clause: Optional[exprs.Predicate] = None,
+        group_by_clause: Optional[List[exprs.Expr]] = None,
+        grouping_tbl: Optional[catalog.TableVersion] = None,
+        order_by_clause: Optional[List[Tuple[exprs.Expr, bool]]] = None,  # List[(expr, asc)]
+        limit: Optional[int] = None,
+    ):
         self.tbl = tbl
 
         # select list logic
-        DataFrame._select_list_check_rep(select_list) # check select list without expansion
+        DataFrame._select_list_check_rep(select_list)  # check select list without expansion
         # exprs contain execution state and therefore cannot be shared
         select_list = copy.deepcopy(select_list)
         select_list_exprs, column_names = DataFrame._normalize_select_list(tbl, select_list)
         DataFrame._select_list_check_rep(list(zip(select_list_exprs, column_names)))
         # check select list after expansion to catch early
         # the following two lists are always non empty, even if select list is None.
         self._select_list_exprs = select_list_exprs
@@ -245,64 +280,65 @@
         assert group_by_clause is None or grouping_tbl is None
         self.group_by_clause = copy.deepcopy(group_by_clause)
         self.grouping_tbl = grouping_tbl
         self.order_by_clause = copy.deepcopy(order_by_clause)
         self.limit_val = limit
 
     @classmethod
-    def _select_list_check_rep(cls,
+    def _select_list_check_rep(
+        cls,
         select_list: Optional[List[Tuple[exprs.Expr, Optional[str]]]],
     ) -> None:
-        """Validate basic select list types. 
-        """
-        if select_list is None: # basic check for valid select list
+        """Validate basic select list types."""
+        if select_list is None:  # basic check for valid select list
             return
 
         assert len(select_list) > 0
         for ent in select_list:
             assert isinstance(ent, tuple)
             assert len(ent) == 2
             assert isinstance(ent[0], exprs.Expr)
             assert ent[1] is None or isinstance(ent[1], str)
             if isinstance(ent[1], str):
                 assert is_valid_identifier(ent[1])
 
     @classmethod
-    def _normalize_select_list(cls,
+    def _normalize_select_list(
+        cls,
         tbl: catalog.TableVersionPath,
         select_list: Optional[List[Tuple[exprs.Expr, Optional[str]]]],
     ) -> Tuple[List[exprs.Expr], List[str]]:
         """
         Expand select list information with all columns and their names
-        Returns: 
+        Returns:
             a pair composed of the list of expressions and the list of corresponding names
         """
         if select_list is None:
             expanded_list = [(exprs.ColumnRef(col), None) for col in tbl.columns()]
         else:
             expanded_list = select_list
 
-        out_exprs : List[exprs.Expr] = []
-        out_names : List[str] = [] # keep track of order
-        seen_out_names : set[str] = set() # use to check for duplicates in loop, avoid square complexity
+        out_exprs: List[exprs.Expr] = []
+        out_names: List[str] = []  # keep track of order
+        seen_out_names: set[str] = set()  # use to check for duplicates in loop, avoid square complexity
         for i, (expr, name) in enumerate(expanded_list):
             if name is None:
                 # use default, add suffix if needed so default adds no duplicates
                 default_name = expr.default_column_name()
                 if default_name is not None:
                     column_name = default_name
                     if default_name in seen_out_names:
                         # already used, then add suffix until unique name is found
-                        for j in range(1, len(out_names)+1):
+                        for j in range(1, len(out_names) + 1):
                             column_name = f'{default_name}_{j}'
                             if column_name not in seen_out_names:
                                 break
-                else: # no default name, eg some expressions
+                else:  # no default name, eg some expressions
                     column_name = f'col_{i}'
-            else: # user provided name, no attempt to rename
+            else:  # user provided name, no attempt to rename
                 column_name = name
 
             out_exprs.append(expr)
             out_names.append(column_name)
             seen_out_names.add(column_name)
         assert len(out_exprs) == len(out_names)
         assert set(out_names) == seen_out_names
@@ -322,17 +358,21 @@
             group_by_clause = [exprs.RowidRef(self.tbl.tbl_version, idx) for idx in range(num_rowid_cols)]
         elif self.group_by_clause is not None:
             group_by_clause = self.group_by_clause
 
         for item in self._select_list_exprs:
             item.bind_rel_paths(None)
         plan = Planner.create_query_plan(
-            self.tbl, self._select_list_exprs, where_clause=self.where_clause, group_by_clause=group_by_clause,
+            self.tbl,
+            self._select_list_exprs,
+            where_clause=self.where_clause,
+            group_by_clause=group_by_clause,
             order_by_clause=self.order_by_clause if self.order_by_clause is not None else [],
-            limit=self.limit_val if self.limit_val is not None else 0)  # limit_val == 0: no limit_val
+            limit=self.limit_val if self.limit_val is not None else 0,
+        )  # limit_val == 0: no limit_val
 
         with Env.get().engine.begin() as conn:
             plan.ctx.conn = conn
             plan.open()
             try:
                 for row_batch in plan:
                     for data_row in row_batch:
@@ -370,20 +410,18 @@
     def collect(self) -> DataFrameResultSet:
         try:
             result_rows = []
             for data_row in self._exec():
                 result_row = [data_row[e.slot_idx] for e in self._select_list_exprs]
                 result_rows.append(result_row)
         except excs.ExprEvalError as e:
-            msg = (f'In row {e.row_num} the {e.expr_msg} encountered exception '
-                   f'{type(e.exc).__name__}:\n{str(e.exc)}')
+            msg = f'In row {e.row_num} the {e.expr_msg} encountered exception ' f'{type(e.exc).__name__}:\n{str(e.exc)}'
             if len(e.input_vals) > 0:
                 input_msgs = [
-                    f"'{d}' = {d.col_type.print_value(e.input_vals[i])}"
-                    for i, d in enumerate(e.expr.dependencies())
+                    f"'{d}' = {d.col_type.print_value(e.input_vals[i])}" for i, d in enumerate(e.expr.dependencies())
                 ]
                 msg += f'\nwith {", ".join(input_msgs)}'
             assert e.exc_tb is not None
             stack_trace = traceback.format_tb(e.exc_tb)
             if len(stack_trace) > 2:
                 # append a stack trace if the exception happened in user code
                 # (frame 0 is ExprEvaluator and frame 1 is some expr's eval()
@@ -395,14 +433,15 @@
             raise excs.Error(f'Error during SQL execution:\n{e}')
 
         col_types = self.get_column_types()
         return DataFrameResultSet(result_rows, self._column_names, col_types)
 
     def count(self) -> int:
         from pixeltable.plan import Planner
+
         stmt = Planner.create_count_stmt(self.tbl, self.where_clause)
         with Env.get().engine.connect() as conn:
             result: int = conn.execute(stmt).scalar_one()
             assert isinstance(result, int)
             return result
 
     def _description(self) -> pd.DataFrame:
@@ -420,63 +459,67 @@
         if self.group_by_clause is not None:
             heading_vals.append('Group By')
             heading_vals.extend([''] * (len(self.group_by_clause) - 1))
             info_vals.extend([e.display_str(inline=False) for e in self.group_by_clause])
         if self.order_by_clause is not None:
             heading_vals.append('Order By')
             heading_vals.extend([''] * (len(self.order_by_clause) - 1))
-            info_vals.extend([
-                f'{e[0].display_str(inline=False)} {"asc" if e[1] else "desc"}' for e in self.order_by_clause
-            ])
+            info_vals.extend(
+                [f'{e[0].display_str(inline=False)} {"asc" if e[1] else "desc"}' for e in self.order_by_clause]
+            )
         if self.limit_val is not None:
             heading_vals.append('Limit')
             info_vals.append(str(self.limit_val))
         assert len(heading_vals) > 0
         assert len(info_vals) > 0
         assert len(heading_vals) == len(info_vals)
         return pd.DataFrame({'Heading': heading_vals, 'Info': info_vals})
 
     def _description_html(self) -> pandas.io.formats.style.Styler:
         """Return the description in an ipython-friendly manner."""
         pd_df = self._description()
         # white-space: pre-wrap: print \n as newline
         # th: center-align headings
-        return pd_df.style.set_properties(**{'white-space': 'pre-wrap', 'text-align': 'left'}) \
-            .set_table_styles([dict(selector='th', props=[('text-align', 'center')])]) \
-            .hide(axis='index').hide(axis='columns')
+        return (
+            pd_df.style.set_properties(**{'white-space': 'pre-wrap', 'text-align': 'left'})
+            .set_table_styles([dict(selector='th', props=[('text-align', 'center')])])
+            .hide(axis='index')
+            .hide(axis='columns')
+        )
 
     def describe(self) -> None:
         """
         Prints a tabular description of this DataFrame.
         The description has two columns, heading and info, which list the contents of each 'component'
                 (select list, where clause, ...) vertically.
         """
         try:
             __IPYTHON__
             from IPython.display import display
+
             display(self._description_html())
         except NameError:
             print(self.__repr__())
 
     def __repr__(self) -> str:
         return self._description().to_string(header=False, index=False)
 
     def _repr_html_(self) -> str:
         return self._description_html()._repr_html_()
 
-    def select(self, *items: Any, **named_items : Any) -> DataFrame:
+    def select(self, *items: Any, **named_items: Any) -> DataFrame:
         if self.select_list is not None:
             raise excs.Error(f'Select list already specified')
-        for (name, _) in named_items.items():
+        for name, _ in named_items.items():
             if not isinstance(name, str) or not is_valid_identifier(name):
                 raise excs.Error(f'Invalid name: {name}')
         base_list = [(expr, None) for expr in items] + [(expr, k) for (k, expr) in named_items.items()]
         if len(base_list) == 0:
             raise excs.Error(f'Empty select list')
-        
+
         # analyze select list; wrap literals with the corresponding expressions
         select_list = []
         for raw_expr, name in base_list:
             if isinstance(raw_expr, exprs.Expr):
                 select_list.append((raw_expr, name))
             elif isinstance(raw_expr, dict):
                 select_list.append((exprs.InlineDict(raw_expr), name))
@@ -497,21 +540,33 @@
             if name in seen:
                 repeated_names = [j for j, x in enumerate(names) if x == name]
                 pretty = ', '.join(map(str, repeated_names))
                 raise excs.Error(f'Repeated column name "{name}" in select() at positions: {pretty}')
             seen.add(name)
 
         return DataFrame(
-            self.tbl, select_list=select_list, where_clause=self.where_clause, group_by_clause=self.group_by_clause,
-            grouping_tbl=self.grouping_tbl, order_by_clause=self.order_by_clause, limit=self.limit_val)
+            self.tbl,
+            select_list=select_list,
+            where_clause=self.where_clause,
+            group_by_clause=self.group_by_clause,
+            grouping_tbl=self.grouping_tbl,
+            order_by_clause=self.order_by_clause,
+            limit=self.limit_val,
+        )
 
     def where(self, pred: exprs.Predicate) -> DataFrame:
         return DataFrame(
-            self.tbl, select_list=self.select_list, where_clause=pred, group_by_clause=self.group_by_clause,
-            grouping_tbl=self.grouping_tbl, order_by_clause=self.order_by_clause, limit=self.limit_val)
+            self.tbl,
+            select_list=self.select_list,
+            where_clause=pred,
+            group_by_clause=self.group_by_clause,
+            grouping_tbl=self.grouping_tbl,
+            order_by_clause=self.order_by_clause,
+            limit=self.limit_val,
+        )
 
     def group_by(self, *grouping_items: Any) -> DataFrame:
         """Add a group-by clause to this DataFrame.
         Variants:
         - group_by(<base table>): group a component view by their respective base table rows
         - group_by(<expr>, ...): group by the given expressions
         """
@@ -530,34 +585,50 @@
                 grouping_tbl = item.tbl_version_path.tbl_version
                 break
             if not isinstance(item, exprs.Expr):
                 raise excs.Error(f'Invalid expression in group_by(): {item}')
         if grouping_tbl is None:
             group_by_clause = list(grouping_items)
         return DataFrame(
-            self.tbl, select_list=self.select_list, where_clause=self.where_clause, group_by_clause=group_by_clause,
-            grouping_tbl=grouping_tbl, order_by_clause=self.order_by_clause, limit=self.limit_val)
+            self.tbl,
+            select_list=self.select_list,
+            where_clause=self.where_clause,
+            group_by_clause=group_by_clause,
+            grouping_tbl=grouping_tbl,
+            order_by_clause=self.order_by_clause,
+            limit=self.limit_val,
+        )
 
     def order_by(self, *expr_list: exprs.Expr, asc: bool = True) -> DataFrame:
         for e in expr_list:
             if not isinstance(e, exprs.Expr):
                 raise excs.Error(f'Invalid expression in order_by(): {e}')
         order_by_clause = self.order_by_clause if self.order_by_clause is not None else []
         order_by_clause.extend([(e.copy(), asc) for e in expr_list])
         return DataFrame(
-            self.tbl, select_list=self.select_list, where_clause=self.where_clause,
-            group_by_clause=self.group_by_clause, grouping_tbl=self.grouping_tbl, order_by_clause=order_by_clause,
-            limit=self.limit_val)
+            self.tbl,
+            select_list=self.select_list,
+            where_clause=self.where_clause,
+            group_by_clause=self.group_by_clause,
+            grouping_tbl=self.grouping_tbl,
+            order_by_clause=order_by_clause,
+            limit=self.limit_val,
+        )
 
     def limit(self, n: int) -> DataFrame:
         assert n is not None and isinstance(n, int)
         return DataFrame(
-            self.tbl, select_list=self.select_list, where_clause=self.where_clause,
-            group_by_clause=self.group_by_clause, grouping_tbl=self.grouping_tbl, order_by_clause=self.order_by_clause,
-            limit=n)
+            self.tbl,
+            select_list=self.select_list,
+            where_clause=self.where_clause,
+            group_by_clause=self.group_by_clause,
+            grouping_tbl=self.grouping_tbl,
+            order_by_clause=self.order_by_clause,
+            limit=n,
+        )
 
     def __getitem__(self, index: object) -> DataFrame:
         """
         Allowed:
         - [<Predicate>]: filter operation
         - [List[Expr]]/[Tuple[Expr]]: setting the select list
         - [Expr]: setting a single-col select list
@@ -567,32 +638,35 @@
         if isinstance(index, tuple):
             index = list(index)
         if isinstance(index, exprs.Expr):
             index = [index]
         if isinstance(index, list):
             return self.select(*index)
         raise TypeError(f'Invalid index type: {type(index)}')
-    
+
     def _as_dict(self) -> Dict[str, Any]:
-        """ 
-            Returns:
-                Dictionary representing this dataframe.
+        """
+        Returns:
+            Dictionary representing this dataframe.
         """
         tbl_versions = self.tbl.get_tbl_versions()
         d = {
             '_classname': 'DataFrame',
             'tbl_ids': [str(t.id) for t in tbl_versions],
             'tbl_versions': [t.version for t in tbl_versions],
-            'select_list':
-                [(e.as_dict(), name) for (e, name) in self.select_list] if self.select_list is not None else None,
+            'select_list': [(e.as_dict(), name) for (e, name) in self.select_list]
+            if self.select_list is not None
+            else None,
             'where_clause': self.where_clause.as_dict() if self.where_clause is not None else None,
-            'group_by_clause':
-                [e.as_dict() for e in self.group_by_clause] if self.group_by_clause is not None else None,
-            'order_by_clause':
-                [(e.as_dict(), asc) for (e,asc) in self.order_by_clause] if self.order_by_clause is not None else None,
+            'group_by_clause': [e.as_dict() for e in self.group_by_clause]
+            if self.group_by_clause is not None
+            else None,
+            'order_by_clause': [(e.as_dict(), asc) for (e, asc) in self.order_by_clause]
+            if self.order_by_clause is not None
+            else None,
             'limit_val': self.limit_val,
         }
         return d
 
     def to_coco_dataset(self) -> Path:
         """Convert the dataframe to a COCO dataset.
         This dataframe must return a single json-typed output column in the following format:
@@ -611,15 +685,15 @@
             Path to the COCO dataset file.
         """
         from pixeltable.utils.coco import write_coco_dataset
 
         summary_string = json.dumps(self._as_dict())
         cache_key = hashlib.sha256(summary_string.encode()).hexdigest()
 
-        dest_path = (Env.get().dataset_cache_dir / f'coco_{cache_key}')
+        dest_path = Env.get().dataset_cache_dir / f'coco_{cache_key}'
         if dest_path.exists():
             assert dest_path.is_dir()
             data_file_path = dest_path / 'data.json'
             assert data_file_path.exists()
             assert data_file_path.is_file()
             return data_file_path
         else:
@@ -656,20 +730,20 @@
             modify or remove any such values through selections and filters prior to calling to_pytorch_dataset().
         """
         # check dependencies
         Env.get().require_package('pyarrow', [13])
         Env.get().require_package('torch')
         Env.get().require_package('torchvision')
 
-        from pixeltable.utils.parquet import save_parquet # pylint: disable=import-outside-toplevel
-        from pixeltable.utils.pytorch import PixeltablePytorchDataset # pylint: disable=import-outside-toplevel
+        from pixeltable.io.parquet import save_parquet  # pylint: disable=import-outside-toplevel
+        from pixeltable.utils.pytorch import PixeltablePytorchDataset  # pylint: disable=import-outside-toplevel
 
-        summary_string = json.dumps(self._as_dict()) 
+        summary_string = json.dumps(self._as_dict())
         cache_key = hashlib.sha256(summary_string.encode()).hexdigest()
-    
-        dest_path = (Env.get().dataset_cache_dir / f'df_{cache_key}').with_suffix('.parquet') # pylint: disable = protected-access
-        if dest_path.exists(): # fast path: use cache
+
+        dest_path = (Env.get().dataset_cache_dir / f'df_{cache_key}').with_suffix('.parquet')  # pylint: disable = protected-access
+        if dest_path.exists():  # fast path: use cache
             assert dest_path.is_dir()
         else:
             save_parquet(self, dest_path)
 
         return PixeltablePytorchDataset(path=dest_path, image_format=image_format)
```

### Comparing `pixeltable-0.2.5/pixeltable/env.py` & `pixeltable-0.2.6/pixeltable/env.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,48 +19,53 @@
 import sqlalchemy as sql
 import yaml
 from sqlalchemy_utils.functions import database_exists, create_database, drop_database
 from tqdm import TqdmWarning
 
 import pixeltable.exceptions as excs
 from pixeltable import metadata
+from pixeltable.utils.http_server import make_server
 
 
 class Env:
     """
     Store for runtime globals.
     """
+
     _instance: Optional[Env] = None
     _log_fmt_str = '%(asctime)s %(levelname)s %(name)s %(filename)s:%(lineno)d: %(message)s'
 
     @classmethod
     def get(cls) -> Env:
         if cls._instance is None:
-            cls._instance = Env()
+            env = Env()
+            env._set_up()
+            env._upgrade_metadata()
+            cls._instance = env
         return cls._instance
 
     def __init__(self):
         self._home: Optional[Path] = None
         self._media_dir: Optional[Path] = None  # computed media files
         self._file_cache_dir: Optional[Path] = None  # cached media files with external URL
         self._dataset_cache_dir: Optional[Path] = None  # cached datasets (eg, pytorch or COCO)
         self._log_dir: Optional[Path] = None  # log files
         self._tmp_dir: Optional[Path] = None  # any tmp files
         self._sa_engine: Optional[sql.engine.base.Engine] = None
-        self._pgdata_dir : Optional[Path] = None
+        self._pgdata_dir: Optional[Path] = None
         self._db_name: Optional[str] = None
         self._db_server: Optional[pgserver.PostgresServer] = None
         self._db_url: Optional[str] = None
 
         # info about installed packages that are utilized by some parts of the code;
         # package name -> version; version == []: package is installed, but we haven't determined the version yet
         self._installed_packages: Dict[str, Optional[List[int]]] = {}
         self._nos_client: Optional[Any] = None
         self._spacy_nlp: Optional[Any] = None  # spacy.Language
-        self._httpd: Optional[socketserver.TCPServer] = None
+        self._httpd: Optional[http.server.ThreadingHTTPServer] = None
         self._http_address: Optional[str] = None
 
         self._registered_clients: dict[str, Any] = {}
 
         # logging-related state
         self._logger = logging.getLogger('pixeltable')
         self._logger.setLevel(logging.DEBUG)  # allow everything to pass, we filter in _log_filter()
@@ -90,21 +95,51 @@
         return self._db_url
 
     @property
     def http_address(self) -> str:
         assert self._http_address is not None
         return self._http_address
 
+    def configure_logging(
+        self,
+        *,
+        to_stdout: Optional[bool] = None,
+        level: Optional[int] = None,
+        add: Optional[str] = None,
+        remove: Optional[str] = None,
+    ) -> None:
+        """Configure logging.
+
+        Args:
+            to_stdout: if True, also log to stdout
+            level: default log level
+            add: comma-separated list of 'module name:log level' pairs; ex.: add='video:10'
+            remove: comma-separated list of module names
+        """
+        if to_stdout is not None:
+            self.log_to_stdout(to_stdout)
+        if level is not None:
+            self.set_log_level(level)
+        if add is not None:
+            for module, level in [t.split(':') for t in add.split(',')]:
+                self.set_module_log_level(module, int(level))
+        if remove is not None:
+            for module in remove.split(','):
+                self.set_module_log_level(module, None)
+        if to_stdout is None and level is None and add is None and remove is None:
+            self.print_log_config()
+
     def print_log_config(self) -> None:
         print(f'logging to {self._logfilename}')
         print(f'{"" if self._log_to_stdout else "not "}logging to stdout')
         print(f'default log level: {logging.getLevelName(self._default_log_level)}')
         print(
             f'module log levels: '
-            f'{",".join([name + ":" + logging.getLevelName(val) for name, val in self._module_log_level.items()])}')
+            f'{",".join([name + ":" + logging.getLevelName(val) for name, val in self._module_log_level.items()])}'
+        )
 
     def log_to_stdout(self, enable: bool = True) -> None:
         self._log_to_stdout = enable
         if enable:
             self._logger.addHandler(self._stdout_handler)
         else:
             self._logger.removeHandler(self._stdout_handler)
@@ -131,18 +166,22 @@
                 if module_name in self._module_log_level and record.levelno >= self._module_log_level[module_name]:
                     return True
         if record.levelno >= self._default_log_level:
             return True
         else:
             return False
 
-    def set_up(self, echo: bool = False, reinit_db: bool = False) -> None:
+    def _set_up(self, echo: bool = False, reinit_db: bool = False) -> None:
         if self._initialized:
             return
 
+        # Disable spurious warnings
+        warnings.simplefilter('ignore', category=TqdmWarning)
+        os.environ['TOKENIZERS_PARALLELISM'] = 'false'
+
         self._initialized = True
         home = Path(os.environ.get('PIXELTABLE_HOME', str(Path.home() / '.pixeltable')))
         assert self._home is None or self._home == home
         self._home = home
         self._config_file = Path(os.environ.get('PIXELTABLE_CONFIG', str(self._home / 'config.yaml')))
         self._media_dir = self._home / 'media'
         self._file_cache_dir = self._home / 'file_cache'
@@ -200,14 +239,22 @@
         av_logfilename = self._logfilename.replace('.log', '_av.log')
         av_fh = logging.FileHandler(self._log_dir / av_logfilename, mode='w')
         av_fh.setFormatter(logging.Formatter(self._log_fmt_str))
         av_logger = logging.getLogger('libav')
         av_logger.addHandler(av_fh)
         av_logger.propagate = False
 
+        # configure web-server logging
+        http_logfilename = self._logfilename.replace('.log', '_http.log')
+        http_fh = logging.FileHandler(self._log_dir / http_logfilename, mode='w')
+        http_fh.setFormatter(logging.Formatter(self._log_fmt_str))
+        http_logger = logging.getLogger('pixeltable.http.server')
+        http_logger.addHandler(http_fh)
+        http_logger.propagate = False
+
         # empty tmp dir
         for path in glob.glob(f'{self._tmp_dir}/*'):
             os.remove(path)
 
         self._db_name = os.environ.get('PIXELTABLE_DB', 'pixeltable')
         self._pgdata_dir = Path(os.environ.get('PIXELTABLE_PGDATA', str(self._home / 'pgdata')))
 
@@ -220,14 +267,15 @@
                 drop_database(self.db_url)
 
         if not database_exists(self.db_url):
             self._logger.info(f'creating database at {self.db_url}')
             create_database(self.db_url)
             self._sa_engine = sql.create_engine(self.db_url, echo=echo, future=True)
             from pixeltable.metadata import schema
+
             schema.Base.metadata.create_all(self._sa_engine)
             metadata.create_system_info(self._sa_engine)
             # enable pgvector
             with self._sa_engine.begin() as conn:
                 conn.execute(sql.text('CREATE EXTENSION vector'))
         else:
             self._logger.info(f'found database {self.db_url}')
@@ -236,37 +284,37 @@
 
         print(f'Connected to Pixeltable database at: {self.db_url}')
 
         # we now have a home directory and db; start other services
         self._set_up_runtime()
         self.log_to_stdout(False)
 
-        # Disable spurious warnings
-        warnings.simplefilter("ignore", category=TqdmWarning)
-
-    def upgrade_metadata(self) -> None:
+    def _upgrade_metadata(self) -> None:
         metadata.upgrade_md(self._sa_engine)
 
     def _create_nos_client(self) -> None:
         import nos
+
         self._logger.info('connecting to NOS')
         nos.init(logging_level=logging.DEBUG)
         self._nos_client = nos.client.InferenceClient()
         self._logger.info('waiting for NOS')
         self._nos_client.WaitForServer()
 
         # now that we have a client, we can create the module
         import importlib
+
         try:
             importlib.import_module('pixeltable.functions.nos')
             # it's already been created
             return
         except ImportError:
             pass
         from pixeltable.functions.util import create_nos_modules
+
         _ = create_nos_modules()
 
     def get_client(self, name: str, init: Callable, environ: Optional[str] = None) -> Any:
         """
         Gets the client with the specified name, using `init` to construct one if necessary.
 
         - name: The name of the client
@@ -292,24 +340,21 @@
         self._logger.info(f'Initialized `{name}` client.')
         return client
 
     def _start_web_server(self) -> None:
         """
         The http server root is the file system root.
         eg: /home/media/foo.mp4 is located at http://127.0.0.1:{port}/home/media/foo.mp4
+        in windows, the server will translate paths like http://127.0.0.1:{port}/c:/media/foo.mp4
         This arrangement enables serving media hosted within _home,
         as well as external media inserted into pixeltable or produced by pixeltable.
         The port is chosen dynamically to prevent conflicts.
         """
         # Port 0 means OS picks one for us.
-        address = ("127.0.0.1", 0)
-        class FixedRootHandler(http.server.SimpleHTTPRequestHandler):
-            def __init__(self, *args, **kwargs):
-                super().__init__(*args, directory='/', **kwargs)
-        self._httpd = socketserver.TCPServer(address, FixedRootHandler)
+        self._httpd = make_server('127.0.0.1', 0)
         port = self._httpd.server_address[1]
         self._http_address = f'http://127.0.0.1:{port}'
 
         def run_server():
             logging.log(logging.INFO, f'running web server at {self._http_address}')
             self._httpd.serve_forever()
 
@@ -332,26 +377,29 @@
         check('datasets')
         check('torch')
         check('torchvision')
         check('transformers')
         check('sentence_transformers')
         check('yolox')
         check('boto3')
+        check('fitz')  # pymupdf
         check('pyarrow')
         check('spacy')  # TODO: deal with en-core-web-sm
         if self.is_installed_package('spacy'):
             import spacy
+
             self._spacy_nlp = spacy.load('en_core_web_sm')
         check('tiktoken')
         check('openai')
         check('together')
         check('fireworks')
         check('nos')
         if self.is_installed_package('nos'):
             self._create_nos_client()
+        check('openpyxl')
 
     def require_package(self, package: str, min_version: Optional[List[int]] = None) -> None:
         assert package in self._installed_packages
         if self._installed_packages[package] is None:
             raise excs.Error(f'Package {package} is not installed')
         if min_version is None:
             return
@@ -361,17 +409,20 @@
             m = importlib.import_module(package)
             module_version = [int(x) for x in m.__version__.split('.')]
             self._installed_packages[package] = module_version
         installed_version = self._installed_packages[package]
         if len(min_version) < len(installed_version):
             normalized_min_version = min_version + [0] * (len(installed_version) - len(min_version))
         if any([a < b for a, b in zip(installed_version, normalized_min_version)]):
-            raise excs.Error((
-                f'The installed version of package {package} is {".".join([str[v] for v in installed_version])}, '
-                f'but version  >={".".join([str[v] for v in min_version])} is required'))
+            raise excs.Error(
+                (
+                    f'The installed version of package {package} is {".".join([str[v] for v in installed_version])}, '
+                    f'but version  >={".".join([str[v] for v in min_version])} is required'
+                )
+            )
 
     def num_tmp_files(self) -> int:
         return len(glob.glob(f'{self._tmp_dir}/*'))
 
     def create_tmp_path(self, extension: str = '') -> Path:
         return self._tmp_dir / f'{uuid.uuid4()}{extension}'
 
@@ -408,8 +459,8 @@
     @property
     def nos_client(self) -> Any:
         return self._nos_client
 
     @property
     def spacy_nlp(self) -> Any:
         assert self._spacy_nlp is not None
-        return self._spacy_nlp
+        return self._spacy_nlp
```

### Comparing `pixeltable-0.2.5/pixeltable/exec/aggregation_node.py` & `pixeltable-0.2.6/pixeltable/exec/aggregation_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exec/cache_prefetch_node.py` & `pixeltable-0.2.6/pixeltable/exec/cache_prefetch_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exec/component_iteration_node.py` & `pixeltable-0.2.6/pixeltable/exec/component_iteration_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exec/data_row_batch.py` & `pixeltable-0.2.6/pixeltable/exec/data_row_batch.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 _logger = logging.getLogger('pixeltable')
 
 class DataRowBatch:
     """Set of DataRows, indexed by rowid.
 
     Contains the metadata needed to initialize DataRows.
     """
-    def __init__(self, tbl: catalog.TableVersion, row_builder: exprs.RowBuilder, len: int = 0):
-        self.tbl_id = tbl.id
-        self.tbl_version = tbl.version
+    def __init__(self, tbl: Optional[catalog.TableVersion], row_builder: exprs.RowBuilder, len: int = 0):
+        self.tbl = tbl
         self.row_builder = row_builder
         self.img_slot_idxs = [e.slot_idx for e in row_builder.unique_exprs if e.col_type.is_image_type()]
         # non-image media slots
         self.media_slot_idxs = [
             e.slot_idx for e in row_builder.unique_exprs
             if e.col_type.is_media_type() and not e.col_type.is_image_type()
         ]
@@ -38,45 +37,45 @@
         return row
 
     def pop_row(self) -> exprs.DataRow:
         return self.rows.pop()
 
     def set_row_ids(self, row_ids: List[int]) -> None:
         """Sets pks for rows in batch"""
+        assert self.tbl is not None
         assert len(row_ids) == len(self.rows)
         for row, row_id in zip(self.rows, row_ids):
-            row.set_pk((row_id, self.tbl_version))
+            row.set_pk((row_id, self.tbl))
 
     def __len__(self) -> int:
         return len(self.rows)
 
     def __getitem__(self, index: object) -> exprs.DataRow:
         return self.rows[index]
 
     def flush_imgs(
             self, idx_range: Optional[slice] = None, stored_img_info: Optional[List[exprs.ColumnSlotIdx]] = None,
             flushed_slot_idxs: Optional[List[int]] = None
     ) -> None:
         """Flushes images in the given range of rows."""
+        assert self.tbl is not None
         if stored_img_info is None:
             stored_img_info = []
         if flushed_slot_idxs is None:
             flushed_slot_idxs = []
         if len(stored_img_info) == 0 and len(flushed_slot_idxs) == 0:
             return
         if idx_range is None:
             idx_range = slice(0, len(self.rows))
         for row in self.rows[idx_range]:
             for info in stored_img_info:
-                filepath = str(MediaStore.prepare_media_path(self.tbl_id, info.col.id, self.tbl_version))
+                filepath = str(MediaStore.prepare_media_path(self.tbl.id, info.col.id, self.tbl.version))
                 row.flush_img(info.slot_idx, filepath)
             for slot_idx in flushed_slot_idxs:
                 row.flush_img(slot_idx)
-        #_logger.debug(
-            #f'flushed images in range {idx_range}: slot_idxs={flushed_slot_idxs} stored_img_info={stored_img_info}')
 
     def __iter__(self) -> Iterator[exprs.DataRow]:
         return DataRowBatchIterator(self)
 
 
 class DataRowBatchIterator:
     """
```

### Comparing `pixeltable-0.2.5/pixeltable/exec/exec_context.py` & `pixeltable-0.2.6/pixeltable/exec/exec_context.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exec/exec_node.py` & `pixeltable-0.2.6/pixeltable/exec/exec_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exec/expr_eval_node.py` & `pixeltable-0.2.6/pixeltable/exec/expr_eval_node.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import sys
-import warnings
-from typing import List, Optional, Tuple
-from dataclasses import dataclass, field
 import logging
+import sys
 import time
+import warnings
+from dataclasses import dataclass
+from typing import List, Optional
 
 from tqdm import tqdm, TqdmWarning
 
+import pixeltable.exprs as exprs
+from pixeltable.func import CallableFunction
 from .data_row_batch import DataRowBatch
 from .exec_node import ExecNode
-import pixeltable.exprs as exprs
-import pixeltable.func as func
-
 
 _logger = logging.getLogger('pixeltable')
 
+
 class ExprEvalNode(ExecNode):
     """Materializes expressions
     """
     @dataclass
     class Cohort:
         """List of exprs that form an evaluation context and contain calls to at most one external function"""
         exprs: List[exprs.Expr]
-        ext_function: Optional[func.BatchedFunction]
+        batched_fn: Optional[CallableFunction]
         segment_ctxs: List[exprs.RowBuilder.EvalCtx]
         target_slot_idxs: List[int]
         batch_size: int = 8
 
     def __init__(
             self, row_builder: exprs.RowBuilder, output_exprs: List[exprs.Expr], input_exprs: List[exprs.Expr],
             input: ExecNode
@@ -59,35 +59,35 @@
                 file=sys.stdout
             )
 
     def _close(self) -> None:
         if self.pbar is not None:
             self.pbar.close()
 
-    def _get_batched_fn(self, expr: exprs.Expr) -> Optional[func.BatchedFunction]:
-        if not isinstance(expr, exprs.FunctionCall):
-            return None
-        return expr.fn if isinstance(expr.fn, func.BatchedFunction) else None
+    def _get_batched_fn(self, expr: exprs.Expr) -> Optional[CallableFunction]:
+        if isinstance(expr, exprs.FunctionCall) and isinstance(expr.fn, CallableFunction) and expr.fn.is_batched:
+            return expr.fn
+        return None
 
-    def _is_ext_call(self, expr: exprs.Expr) -> bool:
+    def _is_batched_fn_call(self, expr: exprs.Expr) -> bool:
         return self._get_batched_fn(expr) is not None
 
     def _create_cohorts(self) -> None:
         all_exprs = self.row_builder.get_dependencies(self.target_exprs)
         # break up all_exprs into cohorts such that each cohort contains calls to at most one external function;
         # seed the cohorts with only the ext fn calls
         cohorts: List[List[exprs.Expr]] = []
-        current_ext_function: Optional[func.BatchedFunction] = None
+        current_batched_fn: Optional[CallableFunction] = None
         for e in all_exprs:
-            if not self._is_ext_call(e):
+            if not self._is_batched_fn_call(e):
                 continue
-            if current_ext_function is None or current_ext_function != e.fn:
+            if current_batched_fn is None or current_batched_fn != e.fn:
                 # create a new cohort
                 cohorts.append([])
-                current_ext_function = e.fn
+                current_batched_fn = e.fn
             cohorts[-1].append(e)
 
         # expand the cohorts to include all exprs that are in the same evaluation context as the external calls;
         # cohorts are evaluated in order, so we can exclude the target slots from preceding cohorts and input slots
         exclude = set([e.slot_idx for e in self.input_exprs])
         all_target_slot_idxs = set([e.slot_idx for e in self.target_exprs])
         target_slot_idxs: List[List[int]] = []  # the ones materialized by each cohort
@@ -111,49 +111,49 @@
         for i in range(len(cohorts)):
             cohort = cohorts[i]
             # segment the cohort into sublists that contain either a single ext. function call or no ext. function calls
             # (i.e., only computed cols)
             assert len(cohort) > 0
             # create the first segment here, so we can avoid checking for an empty list in the loop
             segments = [[cohort[0]]]
-            is_ext_segment = self._is_ext_call(cohort[0])
-            ext_fn: Optional[func.BatchedFunction] = self._get_batched_fn(cohort[0])
+            is_batched_segment = self._is_batched_fn_call(cohort[0])
+            batched_fn: Optional[CallableFunction] = self._get_batched_fn(cohort[0])
             for e in cohort[1:]:
-                if self._is_ext_call(e):
+                if self._is_batched_fn_call(e):
                     segments.append([e])
-                    is_ext_segment = True
-                    ext_fn = self._get_batched_fn(e)
+                    is_batched_segment = True
+                    batched_fn = self._get_batched_fn(e)
                 else:
-                    if is_ext_segment:
+                    if is_batched_segment:
                         # start a new segment
                         segments.append([])
-                        is_ext_segment = False
+                        is_batched_segment = False
                     segments[-1].append(e)
 
             # we create the EvalCtxs manually because create_eval_ctx() would repeat the dependencies of each segment
             segment_ctxs = [
                 exprs.RowBuilder.EvalCtx(
                     slot_idxs=[e.slot_idx for e in s], exprs=s, target_slot_idxs=[], target_exprs=[])
                 for s in segments
             ]
-            cohort_info = self.Cohort(cohort, ext_fn, segment_ctxs, target_slot_idxs[i])
+            cohort_info = self.Cohort(cohort, batched_fn, segment_ctxs, target_slot_idxs[i])
             self.cohorts.append(cohort_info)
 
     def _exec_cohort(self, cohort: Cohort, rows: DataRowBatch) -> None:
         """Compute the cohort for the entire input batch by dividing it up into sub-batches"""
         batch_start_idx = 0  # start row of the current sub-batch
         # for multi-resolution models, we re-assess the correct ext fn batch size for each input batch
-        ext_batch_size = cohort.ext_function.get_batch_size() if cohort.ext_function is not None else None
+        ext_batch_size = cohort.batched_fn.get_batch_size() if cohort.batched_fn is not None else None
         if ext_batch_size is not None:
             cohort.batch_size = ext_batch_size
 
         while batch_start_idx < len(rows):
             num_batch_rows = min(cohort.batch_size, len(rows) - batch_start_idx)
             for segment_ctx in cohort.segment_ctxs:
-                if not self._is_ext_call(segment_ctx.exprs[0]):
+                if not self._is_batched_fn_call(segment_ctx.exprs[0]):
                     # compute batch row-wise
                     for row_idx in range(batch_start_idx, batch_start_idx + num_batch_rows):
                         self.row_builder.eval(
                             rows[row_idx], segment_ctx, self.ctx.profile, ignore_errors=self.ctx.ignore_errors)
                 else:
                     fn_call = segment_ctx.exprs[0]
                     # make a batched external function call
@@ -189,15 +189,15 @@
                             for i in range(len(arg_batches))
                         ]
                         call_kwargs = {
                             k: kwarg_batches[k][ext_batch_offset:ext_batch_offset + num_ext_batch_rows]
                             for k in kwarg_batches.keys()
                         }
                         start_ts = time.perf_counter()
-                        result_batch = fn_call.fn.invoke(call_args, call_kwargs)
+                        result_batch = fn_call.fn.exec_batch(*call_args, **call_kwargs)
                         self.ctx.profile.eval_time[fn_call.slot_idx] += time.perf_counter() - start_ts
                         self.ctx.profile.eval_count[fn_call.slot_idx] += num_ext_batch_rows
 
                         # move the result into the row batch
                         for result_idx in range(len(result_batch)):
                             row_idx = valid_batch_idxs[ext_batch_offset + result_idx]
                             row = rows[row_idx]
```

### Comparing `pixeltable-0.2.5/pixeltable/exec/in_memory_data_node.py` & `pixeltable-0.2.6/pixeltable/exec/in_memory_data_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exec/media_validation_node.py` & `pixeltable-0.2.6/pixeltable/exec/media_validation_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exec/sql_scan_node.py` & `pixeltable-0.2.6/pixeltable/exec/sql_scan_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     """Materializes data from the store via SQL
     """
     def __init__(
             self, tbl: catalog.TableVersionPath, row_builder: exprs.RowBuilder,
             select_list: Iterable[exprs.Expr],
             where_clause: Optional[exprs.Expr] = None, filter: Optional[exprs.Predicate] = None,
             order_by_items: Optional[List[Tuple[exprs.Expr, bool]]] = None,
-            similarity_clause: Optional[exprs.ImageSimilarityPredicate] = None,
             limit: int = 0, set_pk: bool = False, exact_version_only: Optional[List[catalog.TableVersion]] = None
     ):
         """
         Args:
             select_list: output of the query
             sql_where_clause: SQL Where clause
             filter: additional Where-clause predicate that can't be evaluated via SQL
@@ -73,23 +72,25 @@
         self.stmt = self.create_from_clause(
             tbl, self.stmt, refd_tbl_ids, exact_version_only={t.id for t in exact_version_only})
 
         # change rowid refs against a base table to rowid refs against the target table, so that we minimize
         # the number of tables that need to be joined to the target table
         for rowid_ref in [e for e, _ in order_by_items if isinstance(e, exprs.RowidRef)]:
             rowid_ref.set_tbl(tbl)
-        order_by_clause = [e.sql_expr().desc() if not asc else e.sql_expr() for e, asc in order_by_items]
+        order_by_clause: List[sql.ClauseElement] = []
+        for e, asc in order_by_items:
+            if isinstance(e, exprs.SimilarityExpr):
+                order_by_clause.append(e.as_order_by_clause(asc))
+            else:
+                order_by_clause.append(e.sql_expr().desc() if not asc else e.sql_expr())
 
         if where_clause is not None:
             sql_where_clause = where_clause.sql_expr()
             assert sql_where_clause is not None
             self.stmt = self.stmt.where(sql_where_clause)
-        if similarity_clause is not None:
-            self.stmt = self.stmt.order_by(
-                similarity_clause.img_col_ref.col.sa_idx_col.l2_distance(similarity_clause.embedding()))
         if len(order_by_clause) > 0:
             self.stmt = self.stmt.order_by(*order_by_clause)
         elif target.id in row_builder.unstored_iter_args:
             # we are referencing unstored iter columns from this view and try to order by our primary key,
             # which ensures that iterators will see monotonically increasing pos values
             self.stmt = self.stmt.order_by(*self.tbl.store_tbl.rowid_columns())
         if limit != 0 and self.filter is None:
@@ -197,15 +198,15 @@
             for i, e in enumerate(self.sql_exprs):
                 slot_idx = e.slot_idx
                 output_row[slot_idx] = sql_row[i]
             if self.filter is not None:
                 self.row_builder.eval(output_row, self.filter_eval_ctx, profile=self.ctx.profile)
                 if output_row[self.filter.slot_idx]:
                     needs_row = True
-                    if self.limit is not None and len(output_batch) >= self.limit:
+                    if self.limit > 0 and len(output_batch) >= self.limit:
                         self.has_more_rows = False
                         break
                 else:
                     # we re-use this row for the next sql row if it didn't pass the filter
                     needs_row = False
                     output_row.clear()
```

### Comparing `pixeltable-0.2.5/pixeltable/exprs/__init__.py` & `pixeltable-0.2.6/pixeltable/exprs/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 from .array_slice import ArraySlice
 from .column_property_ref import ColumnPropertyRef
 from .column_ref import ColumnRef
 from .comparison import Comparison
 from .compound_predicate import CompoundPredicate
 from .data_row import DataRow
 from .expr import Expr
+from .expr_set import ExprSet
 from .function_call import FunctionCall
 from .image_member_access import ImageMemberAccess
-from .image_similarity_predicate import ImageSimilarityPredicate
+from .in_predicate import InPredicate
 from .inline_array import InlineArray
 from .inline_dict import InlineDict
 from .is_null import IsNull
 from .json_mapper import JsonMapper
 from .json_path import RELATIVE_PATH_ROOT, JsonPath
 from .literal import Literal
 from .object_ref import ObjectRef
-from  .variable import Variable
 from .predicate import Predicate
 from .row_builder import RowBuilder, ColumnSlotIdx, ExecProfile
 from .rowid_ref import RowidRef
-from .expr_set import ExprSet
+from .similarity_expr import SimilarityExpr
 from .type_cast import TypeCast
+from .variable import Variable
```

### Comparing `pixeltable-0.2.5/pixeltable/exprs/arithmetic_expr.py` & `pixeltable-0.2.6/pixeltable/exprs/arithmetic_expr.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exprs/array_slice.py` & `pixeltable-0.2.6/pixeltable/exprs/array_slice.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exprs/column_property_ref.py` & `pixeltable-0.2.6/pixeltable/exprs/column_property_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exprs/column_ref.py` & `pixeltable-0.2.6/pixeltable/exprs/column_ref.py`

 * *Files 14% similar despite different names*

```diff
@@ -59,14 +59,23 @@
 
         if self.col_type.is_json_type():
             from .json_path import JsonPath
             return JsonPath(self, [name])
 
         return super().__getattr__(name)
 
+    def similarity(self, other: Any) -> Expr:
+        if isinstance(other, Expr):
+            raise excs.Error(f'similarity(): requires a string or a PIL.Image.Image object, not an expression')
+        item = Expr.from_object(other)
+        if item is None or not(item.col_type.is_string_type() or item.col_type.is_image_type()):
+            raise excs.Error(f'similarity(): requires a string or a PIL.Image.Image object, not a {type(other)}')
+        from .similarity_expr import SimilarityExpr
+        return SimilarityExpr(self, item)
+
     def default_column_name(self) -> Optional[str]:
         return str(self)
 
     def _equals(self, other: ColumnRef) -> bool:
         return self.col == other.col
 
     def __str__(self) -> str:
```

### Comparing `pixeltable-0.2.5/pixeltable/exprs/comparison.py` & `pixeltable-0.2.6/pixeltable/exprs/comparison.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exprs/compound_predicate.py` & `pixeltable-0.2.6/pixeltable/exprs/compound_predicate.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exprs/data_row.py` & `pixeltable-0.2.6/pixeltable/exprs/data_row.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exprs/expr.py` & `pixeltable-0.2.6/pixeltable/exprs/expr.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,17 @@
         # - set by the subclass's __init__()
         # - produced by _create_id()
         # - not expected to survive a serialize()/deserialize() roundtrip
         self.id: Optional[int] = None
 
         # index of the expr's value in the data row:
         # - set for all materialized exprs
-        # - -1: not executable
+        # - None: not executable
         # - not set for subexprs that don't need to be materialized because the parent can be materialized via SQL
-        self.slot_idx = -1
+        self.slot_idx: Optional[int] = None
         self.components: List[Expr] = []  # the subexprs that are needed to construct this expr
 
     def dependencies(self) -> List[Expr]:
         """
         Returns all exprs that need to have been evaluated before eval() can be called on this one.
         """
         return self.components
@@ -106,14 +106,19 @@
         if len(self.components) != len(other.components):
             return False
         for i in range(len(self.components)):
             if not self.components[i].equals(other.components[i]):
                 return False
         return self._equals(other)
 
+    def _equals(self, other: Expr) -> bool:
+        # we already compared the type and components in equals(); subclasses that require additional comparisons
+        # override this
+        return True
+
     def _id_attrs(self) -> List[Tuple[str, Any]]:
         """Returns attribute name/value pairs that are used to construct the instance id.
 
         Attribute values must be immutable and have str() defined.
         """
         return [('classname', self.__class__.__name__)]
 
@@ -144,15 +149,15 @@
         """
         Creates a copy that can be evaluated separately: it doesn't share any eval context (slot_idx)
         but shares everything else (catalog objects, etc.)
         """
         cls = self.__class__
         result = cls.__new__(cls)
         result.__dict__.update(self.__dict__)
-        result.slot_idx = -1
+        result.slot_idx = None
         result.components = [c.copy() for c in self.components]
         return result
 
     @classmethod
     def copy_list(cls, expr_list: List[Expr]) -> List[Expr]:
         return [e.copy() for e in expr_list]
 
@@ -310,18 +315,14 @@
             return InlineDict(o)
         elif isinstance(o, list):
             from .inline_array import InlineArray
             return InlineArray(tuple(o))
         return None
 
     @abc.abstractmethod
-    def _equals(self, other: Expr) -> bool:
-        pass
-
-    @abc.abstractmethod
     def sql_expr(self) -> Optional[sql.ClauseElement]:
         """
         If this expr can be materialized directly in SQL:
         - returns a ClauseElement
         - eval() will not be called (exception: Literal)
         Otherwise
         - returns None
@@ -392,14 +393,21 @@
     def from_dict_list(cls, dict_list: List[Dict]) -> List[Expr]:
         return [cls.from_dict(d) for d in dict_list]
 
     @classmethod
     def _from_dict(cls, d: Dict, components: List[Expr]) -> Expr:
         assert False, 'not implemented'
 
+    def isin(self, value_set: Any) -> 'pixeltable.exprs.InPredicate':
+        from .in_predicate import InPredicate
+        if isinstance(value_set, Expr):
+            return InPredicate(self, value_set_expr=value_set)
+        else:
+            return InPredicate(self, value_set_literal=value_set)
+
     def astype(self, new_type: ts.ColumnType) -> 'pixeltable.exprs.TypeCast':
         from pixeltable.exprs import TypeCast
         return TypeCast(self, new_type)
 
     def apply(self, fn: Callable, *, col_type: Optional[ts.ColumnType] = None) -> 'pixeltable.exprs.FunctionCall':
         function = self._make_applicator_function(fn, col_type)
         # Return a `FunctionCall` obtained by passing this `Expr` to the new `function`.
```

### Comparing `pixeltable-0.2.5/pixeltable/exprs/expr_set.py` & `pixeltable-0.2.6/pixeltable/exprs/expr_set.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exprs/function_call.py` & `pixeltable-0.2.6/pixeltable/exprs/function_call.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             self, fn: func.Function, bound_args: Dict[str, Any], order_by_clause: Optional[List[Any]] = None,
             group_by_clause: Optional[List[Any]] = None, is_method_call: bool = False):
         if order_by_clause is None:
             order_by_clause = []
         if group_by_clause is None:
             group_by_clause = []
         signature = fn.signature
-        super().__init__(signature.get_return_type(bound_args))
+        super().__init__(fn.call_return_type(bound_args))
         self.fn = fn
         self.is_method_call = is_method_call
         self.check_args(signature, bound_args)
 
         self.agg_init_args: Dict[str, Any] = {}
         if self.is_agg_fn_call:
             # we separate out the init args for the aggregator
@@ -42,43 +42,43 @@
             bound_args = {arg_name: arg for arg_name, arg in bound_args.items() if arg_name not in fn.init_param_names}
 
         # construct components, args, kwargs
         self.components: List[Expr] = []
 
         # Tuple[int, Any]:
         # - for Exprs: (index into components, None)
-        # - otherwise: (-1, val)
-        self.args: List[Tuple[int, Any]] = []
-        self.kwargs: Dict[str, Tuple[int, Any]] = {}
+        # - otherwise: (None, val)
+        self.args: List[Tuple[Optional[int], Optional[Any]]] = []
+        self.kwargs: Dict[str, Tuple[Optional[int], Optional[Any]]] = {}
 
         # we record the types of non-variable parameters for runtime type checks
         self.arg_types: List[ts.ColumnType] = []
         self.kwarg_types: Dict[str, ts.ColumnType] = {}
         # the prefix of parameters that are bound can be passed by position
         for param in fn.py_signature.parameters.values():
             if param.name not in bound_args or param.kind == inspect.Parameter.KEYWORD_ONLY:
                 break
             arg = bound_args[param.name]
             if isinstance(arg, Expr):
                 self.args.append((len(self.components), None))
                 self.components.append(arg.copy())
             else:
-                self.args.append((-1, arg))
+                self.args.append((None, arg))
             if param.kind != inspect.Parameter.VAR_POSITIONAL and param.kind != inspect.Parameter.VAR_KEYWORD:
                 self.arg_types.append(signature.parameters[param.name].col_type)
 
         # the remaining args are passed as keywords
         kw_param_names = set(bound_args.keys()) - set(list(fn.py_signature.parameters.keys())[:len(self.args)])
         for param_name in kw_param_names:
             arg = bound_args[param_name]
             if isinstance(arg, Expr):
                 self.kwargs[param_name] = (len(self.components), None)
                 self.components.append(arg.copy())
             else:
-                self.kwargs[param_name] = (-1, arg)
+                self.kwargs[param_name] = (None, arg)
             if fn.py_signature.parameters[param_name].kind != inspect.Parameter.VAR_KEYWORD:
                 self.kwarg_types[param_name] = signature.parameters[param_name].col_type
 
         # window function state:
         # self.components[self.group_by_start_idx:self.group_by_stop_idx] contains group_by exprs
         self.group_by_start_idx, self.group_by_stop_idx = 0, 0
         if len(group_by_clause) > 0:
@@ -211,20 +211,20 @@
             return f'{self.components[0]}.{self.fn.name}({self._print_args(1, inline)})'
         else:
             fn_name = self.fn.display_name if self.fn.display_name != '' else 'anonymous_fn'
             return f'{fn_name}({self._print_args()})'
 
     def _print_args(self, start_idx: int = 0, inline: bool = True) -> str:
         arg_strs = [
-            str(arg) if idx == -1 else str(self.components[idx]) for idx, arg in self.args[start_idx:]
+            str(arg) if idx is None else str(self.components[idx]) for idx, arg in self.args[start_idx:]
         ]
         def print_arg(arg: Any) -> str:
             return f"'{arg}'" if isinstance(arg, str) else str(arg)
         arg_strs.extend([
-            f'{param_name}={print_arg(arg) if idx == -1 else str(self.components[idx])}'
+            f'{param_name}={print_arg(arg) if idx is None else str(self.components[idx])}'
             for param_name, (idx, arg) in self.kwargs.items()
         ])
         if len(self.order_by) > 0:
             if self.fn.requires_order_by:
                 arg_strs.insert(0, Expr.print_list(self.order_by))
             else:
                 arg_strs.append(f'order_by={Expr.print_list(self.order_by)}')
@@ -283,26 +283,26 @@
         args, kwargs = self._make_args(data_row)
         self.aggregator.update(*args, **kwargs)
 
     def _make_args(self, data_row: DataRow) -> Tuple[List[Any], Dict[str, Any]]:
         """Return args and kwargs, constructed for data_row"""
         kwargs: Dict[str, Any] = {}
         for param_name, (component_idx, arg) in self.kwargs.items():
-            val = arg if component_idx == -1 else data_row[self.components[component_idx].slot_idx]
+            val = arg if component_idx is None else data_row[self.components[component_idx].slot_idx]
             param = self.fn.signature.parameters[param_name]
             if param.kind == inspect.Parameter.VAR_KEYWORD:
                 # expand **kwargs parameter
                 kwargs.update(val)
             else:
                 assert param.kind != inspect.Parameter.VAR_POSITIONAL
                 kwargs[param_name] = val
 
         args: List[Any] = []
         for param_idx, (component_idx, arg) in enumerate(self.args):
-            val = arg if component_idx == -1 else data_row[self.components[component_idx].slot_idx]
+            val = arg if component_idx is None else data_row[self.components[component_idx].slot_idx]
             param = self.fn.signature.parameters_by_pos[param_idx]
             if param.kind == inspect.Parameter.VAR_POSITIONAL:
                 # expand *args parameter
                 assert isinstance(val, list)
                 args.extend(val)
             elif param.kind == inspect.Parameter.VAR_KEYWORD:
                 # expand **kwargs parameter
@@ -329,32 +329,34 @@
                     return
 
         if isinstance(self.fn, func.ExprTemplateFunction):
             # we need to evaluate the template
             # TODO: can we get rid of this extra copy?
             fn_expr = self.components[self.fn_expr_idx]
             data_row[self.slot_idx] = data_row[fn_expr.slot_idx]
-        elif isinstance(self.fn, func.CallableFunction):
+        elif isinstance(self.fn, func.CallableFunction) and not self.fn.is_batched:
+            # optimization: avoid additional level of indirection we'd get from calling Function.exec()
             data_row[self.slot_idx] = self.fn.py_fn(*args, **kwargs)
         elif self.is_window_fn_call:
             if self.has_group_by():
                 if self.current_partition_vals is None:
                     self.current_partition_vals = [None] * len(self.group_by)
                 partition_vals = [data_row[e.slot_idx] for e in self.group_by]
                 if partition_vals != self.current_partition_vals:
                     # new partition
                     self.aggregator = self.fn.agg_cls(**self.agg_init_args)
                     self.current_partition_vals = partition_vals
             elif self.aggregator is None:
                 self.aggregator = self.fn.agg_cls(**self.agg_init_args)
             self.aggregator.update(*args)
             data_row[self.slot_idx] = self.aggregator.value()
-        else:
-            assert self.is_agg_fn_call
+        elif self.is_agg_fn_call:
             data_row[self.slot_idx] = self.aggregator.value()
+        else:
+            data_row[self.slot_idx] = self.fn.exec(*args, **kwargs)
 
     def _as_dict(self) -> Dict:
         result = {
             'fn': self.fn.as_dict(), 'args': self.args, 'kwargs': self.kwargs,
             'group_by_start_idx': self.group_by_start_idx, 'group_by_stop_idx': self.group_by_stop_idx,
             'order_by_start_idx': self.order_by_start_idx,
             **super()._as_dict()
@@ -365,16 +367,16 @@
     def _from_dict(cls, d: Dict, components: List[Expr]) -> Expr:
         assert 'fn' in d
         assert 'args' in d
         assert 'kwargs' in d
         # reassemble bound args
         fn = func.Function.from_dict(d['fn'])
         param_names = list(fn.signature.parameters.keys())
-        bound_args = {param_names[i]: arg if idx == -1 else components[idx] for i, (idx, arg) in enumerate(d['args'])}
+        bound_args = {param_names[i]: arg if idx is None else components[idx] for i, (idx, arg) in enumerate(d['args'])}
         bound_args.update(
-            {param_name: val if idx == -1 else components[idx] for param_name, (idx, val) in d['kwargs'].items()})
+            {param_name: val if idx is None else components[idx] for param_name, (idx, val) in d['kwargs'].items()})
         group_by_exprs = components[d['group_by_start_idx']:d['group_by_stop_idx']]
         order_by_exprs = components[d['order_by_start_idx']:]
         fn_call = cls(
             func.Function.from_dict(d['fn']), bound_args, group_by_clause=group_by_exprs,
             order_by_clause=order_by_exprs)
         return fn_call
```

### Comparing `pixeltable-0.2.5/pixeltable/exprs/globals.py` & `pixeltable-0.2.6/pixeltable/exprs/globals.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exprs/image_member_access.py` & `pixeltable-0.2.6/pixeltable/exprs/image_member_access.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from __future__ import annotations
-from typing import Optional, List, Any, Dict, Tuple, Union
+
+from typing import Optional, List, Any, Dict, Tuple
 
 import PIL
 import sqlalchemy as sql
 
+import pixeltable.exceptions as excs
+import pixeltable.func as func
+import pixeltable.type_system as ts
+from .data_row import DataRow
 from .expr import Expr
-from .column_ref import ColumnRef
 from .function_call import FunctionCall
-from .image_similarity_predicate import ImageSimilarityPredicate
-from .data_row import DataRow
 from .row_builder import RowBuilder
-import pixeltable.catalog as catalog
-import pixeltable.func as func
-import pixeltable.exceptions as excs
-import pixeltable.type_system as ts
 
 
 # TODO: this doesn't dig up all attrs for actual jpeg images
 def _create_pil_attr_info() -> Dict[str, ts.ColumnType]:
     # create random Image to inspect for attrs
     img = PIL.Image.new('RGB', (100, 100))
     # we're only interested in public attrs (including properties)
@@ -39,17 +37,15 @@
     Access of either an attribute or function member of PIL.Image.Image.
     Ex.: tbl.img_col_ref.rotate(90), tbl.img_col_ref.width
     TODO: remove this class and use FunctionCall instead (attributes to be replaced by functions)
     """
     attr_info = _create_pil_attr_info()
 
     def __init__(self, member_name: str, caller: Expr):
-        if member_name == 'nearest':
-            super().__init__(ts.InvalidType())  # requires FunctionCall to return value
-        elif member_name in self.attr_info:
+        if member_name in self.attr_info:
             super().__init__(self.attr_info[member_name])
         else:
             candidates = func.FunctionRegistry.get().get_type_methods(member_name, ts.ColumnType.Type.IMAGE)
             if len(candidates) == 0:
                 raise excs.Error(f'Unknown Image member: {member_name}')
             if len(candidates) > 1:
                 raise excs.Error(f'Ambiguous Image method: {member_name}')
@@ -74,30 +70,16 @@
 
     @classmethod
     def _from_dict(cls, d: Dict, components: List[Expr]) -> Expr:
         assert 'member_name' in d
         assert len(components) == 1
         return cls(d['member_name'], components[0])
 
-    def __call__(self, *args, **kwargs) -> Union[FunctionCall, ImageSimilarityPredicate]:
-        caller = self._caller
-        call_signature = f'({",".join([type(arg).__name__ for arg in args])})'
-        if self.member_name == 'nearest':
-            # - caller must be ColumnRef
-            # - signature is (Union[PIL.Image.Image, str])
-            if not isinstance(caller, ColumnRef):
-                raise excs.Error(f'nearest(): caller must be an image column')
-            if len(args) != 1 or (not isinstance(args[0], PIL.Image.Image) and not isinstance(args[0], str)):
-                raise excs.Error(f'nearest(): requires a PIL.Image.Image or str, got {call_signature} instead')
-            return ImageSimilarityPredicate(
-                caller,
-                img=args[0] if isinstance(args[0], PIL.Image.Image) else None,
-                text=args[0] if isinstance(args[0], str) else None)
-
-        result = self.img_method(*[caller, *args], **kwargs)
+    def __call__(self, *args, **kwargs) -> FunctionCall:
+        result = self.img_method(*[self._caller, *args], **kwargs)
         result.is_method_call = True
         return result
 
     def _equals(self, other: ImageMemberAccess) -> bool:
         return self.member_name == other.member_name
 
     def _id_attrs(self) -> List[Tuple[str, Any]]:
@@ -108,8 +90,7 @@
 
     def eval(self, data_row: DataRow, row_builder: RowBuilder) -> None:
         caller_val = data_row[self._caller.slot_idx]
         try:
             data_row[self.slot_idx] = getattr(caller_val, self.member_name)
         except AttributeError:
             data_row[self.slot_idx] = None
-
```

### Comparing `pixeltable-0.2.5/pixeltable/exprs/inline_array.py` & `pixeltable-0.2.6/pixeltable/exprs/inline_array.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
-from typing import Optional, List, Any, Dict, Tuple
+
 import copy
+from typing import Optional, List, Any, Dict, Tuple
 
-import sqlalchemy as sql
 import numpy as np
+import sqlalchemy as sql
 
-from .expr import Expr
+import pixeltable.type_system as ts
 from .data_row import DataRow
+from .expr import Expr
 from .inline_dict import InlineDict
 from .row_builder import RowBuilder
-import pixeltable.catalog as catalog
-import pixeltable.type_system as ts
 
 
 class InlineArray(Expr):
     """
     Array 'literal' which can use Exprs as values.
 
     The literal can be cast as either a pixeltable `ArrayType` or `JsonType`. If `force_json`
@@ -23,33 +23,33 @@
     """
     def __init__(self, elements: Tuple, force_json: bool = False):
         # we need to call this in order to populate self.components
         super().__init__(ts.ArrayType((len(elements),), ts.IntType()))
 
         # elements contains
         # - for Expr elements: (index into components, None)
-        # - for non-Expr elements: (-1, value)
-        self.elements: List[Tuple[int, Any]] = []
+        # - for non-Expr elements: (None, value)
+        self.elements: List[Tuple[Optional[int], Any]] = []
         for el in elements:
             el = copy.deepcopy(el)
             if isinstance(el, list):
                 # If col_type is an ArrayType, we'll require it to be a multidimensional array
                 # of the specified underlying type
                 el = InlineArray(tuple(el), force_json)
             if isinstance(el, dict):
                 el = InlineDict(el)
             if isinstance(el, Expr):
                 self.elements.append((len(self.components), None))
                 self.components.append(el)
             else:
-                self.elements.append((-1, el))
+                self.elements.append((None, el))
 
         inferred_element_type = ts.InvalidType()
         for idx, val in self.elements:
-            if idx >= 0:
+            if idx is not None:
                 inferred_element_type = ts.ColumnType.supertype(inferred_element_type, self.components[idx].col_type)
             else:
                 inferred_element_type = ts.ColumnType.supertype(inferred_element_type, ts.ColumnType.infer_literal_type(val))
             if inferred_element_type is None:
                 break
 
         if force_json or inferred_element_type is None:
@@ -79,15 +79,15 @@
 
     def sql_expr(self) -> Optional[sql.ClauseElement]:
         return None
 
     def eval(self, data_row: DataRow, row_builder: RowBuilder) -> None:
         result = [None] * len(self.elements)
         for i, (child_idx, val) in enumerate(self.elements):
-            if child_idx >= 0:
+            if child_idx is not None:
                 result[i] = data_row[self.components[child_idx].slot_idx]
             else:
                 result[i] = copy.deepcopy(val)
         if self.col_type.is_array_type():
             data_row[self.slot_idx] = np.array(result)
         else:
             data_row[self.slot_idx] = result
@@ -96,12 +96,14 @@
         return {'elements': self.elements, **super()._as_dict()}
 
     @classmethod
     def _from_dict(cls, d: Dict, components: List[Expr]) -> Expr:
         assert 'elements' in d
         arg: List[Any] = []
         for idx, val in d['elements']:
-            if idx >= 0:
+            # TODO Normalize idx -1 to None via schema migrations.
+            # Long-term we should not be allowing idx == -1.
+            if idx is not None and idx >= 0:  # Older schemas might have -1 instead of None
                 arg.append(components[idx])
             else:
                 arg.append(val)
         return cls(tuple(arg))
```

### Comparing `pixeltable-0.2.5/pixeltable/exprs/inline_dict.py` & `pixeltable-0.2.6/pixeltable/exprs/inline_dict.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 from __future__ import annotations
-from typing import Optional, List, Any, Dict, Tuple
+
 import copy
+from typing import Optional, List, Any, Dict, Tuple
 
 import sqlalchemy as sql
 
-from .expr import Expr
-from .data_row import DataRow
-from .row_builder import RowBuilder
 import pixeltable.exceptions as excs
-import pixeltable.catalog as catalog
 import pixeltable.type_system as ts
+from .data_row import DataRow
+from .expr import Expr
+from .row_builder import RowBuilder
 
 
 class InlineDict(Expr):
     """
     Dictionary 'literal' which can use Exprs as values.
     """
     def __init__(self, d: Dict):
         from .inline_array import InlineArray
         super().__init__(ts.JsonType())  # we need to call this in order to populate self.components
         # dict_items contains
         # - for Expr fields: (key, index into components, None)
-        # - for non-Expr fields: (key, -1, value)
-        self.dict_items: List[Tuple[str, int, Any]] = []
+        # - for non-Expr fields: (key, None, value)
+        self.dict_items: List[Tuple[str, Optional[int], Any]] = []
         for key, val in d.items():
             if not isinstance(key, str):
                 raise excs.Error(f'Dictionary requires string keys, {key} has type {type(key)}')
             val = copy.deepcopy(val)
             if isinstance(val, dict):
                 val = InlineDict(val)
             if isinstance(val, list) or isinstance(val, tuple):
                 val = InlineArray(tuple(val), force_json=True)
             if isinstance(val, Expr):
                 self.dict_items.append((key, len(self.components), None))
                 self.components.append(val)
             else:
-                self.dict_items.append((key, -1, val))
+                self.dict_items.append((key, None, val))
 
         self.type_spec: Optional[Dict[str, ts.ColumnType]] = {}
         for key, idx, _ in self.dict_items:
-            if idx == -1:
+            if idx is None:
                 # TODO: implement type inference for values
                 self.type_spec = None
                 break
             self.type_spec[key] = self.components[idx].col_type
         self.col_type = ts.JsonType(self.type_spec)
 
         self.id = self._create_id()
@@ -52,50 +52,52 @@
         item_strs: List[str] = []
         i = 0
         def print_val(val: Any) -> str:
             if isinstance(val, str):
                 return f"'{val}'"
             return str(val)
         for key, idx, val in self.dict_items:
-            if idx != -1:
+            if idx is not None:
                 item_strs.append(f"'{key}': {str(self.components[i])}")
                 i += 1
             else:
                 item_strs.append(f"'{key}': {print_val(val)}")
         return '{' + ', '.join(item_strs) + '}'
 
     def _equals(self, other: InlineDict) -> bool:
         return self.dict_items == other.dict_items
 
     def _id_attrs(self) -> List[Tuple[str, Any]]:
         return super()._id_attrs() + [('dict_items', self.dict_items)]
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the original dict used to construct this"""
-        return {key: val if idx == -1 else self.components[idx] for key, idx, val in self.dict_items}
+        return {key: val if idx is None else self.components[idx] for key, idx, val in self.dict_items}
 
     def sql_expr(self) -> Optional[sql.ClauseElement]:
         return None
 
     def eval(self, data_row: DataRow, row_builder: RowBuilder) -> None:
         result = {}
         for key, idx, val in self.dict_items:
             assert isinstance(key, str)
-            if idx >= 0:
+            if idx is not None:
                 result[key] = data_row[self.components[idx].slot_idx]
             else:
                 result[key] = copy.deepcopy(val)
         data_row[self.slot_idx] = result
 
     def _as_dict(self) -> Dict:
         return {'dict_items': self.dict_items, **super()._as_dict()}
 
     @classmethod
     def _from_dict(cls, d: Dict, components: List[Expr]) -> Expr:
         assert 'dict_items' in d
         arg: Dict[str, Any] = {}
         for key, idx, val in d['dict_items']:
-            if idx >= 0:
+            # TODO Normalize idx -1 to None via schema migrations.
+            # Long-term we should not be allowing idx == -1.
+            if idx is not None and idx >= 0:  # Older schemas might have -1 instead of None
                 arg[key] = components[idx]
             else:
                 arg[key] = val
         return cls(arg)
```

### Comparing `pixeltable-0.2.5/pixeltable/exprs/is_null.py` & `pixeltable-0.2.6/pixeltable/exprs/is_null.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exprs/json_mapper.py` & `pixeltable-0.2.6/pixeltable/exprs/json_mapper.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exprs/json_path.py` & `pixeltable-0.2.6/pixeltable/exprs/json_path.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exprs/literal.py` & `pixeltable-0.2.6/pixeltable/exprs/literal.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exprs/object_ref.py` & `pixeltable-0.2.6/pixeltable/exprs/object_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exprs/predicate.py` & `pixeltable-0.2.6/pixeltable/exprs/predicate.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exprs/row_builder.py` & `pixeltable-0.2.6/pixeltable/exprs/row_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,16 @@
     def __init__(
             self, output_exprs: List[Expr], columns: List[catalog.Column], input_exprs: List[Expr]
     ):
         """
         Args:
             output_exprs: list of Exprs to be evaluated
             columns: list of columns to be materialized
+            input_exprs: list of Exprs that are excluded from evaluation (because they're already materialized)
+        TODO: enforce that output_exprs doesn't overlap with input_exprs?
         """
         self.unique_exprs = ExprSet()  # dependencies precede their dependents
         self.next_slot_idx = 0
 
         # record input and output exprs; make copies to avoid reusing execution state
         unique_input_exprs = [self._record_unique_expr(e.copy(), recursive=False) for e in input_exprs]
         self.input_expr_slot_idxs = {e.slot_idx for e in unique_input_exprs}
@@ -175,20 +177,24 @@
             return self.unique_exprs[expr]
 
         # expr value needs to be computed via Expr.eval()
         if recursive:
             for i, c in enumerate(expr.components):
                 # make sure we only refer to components that have themselves been recorded
                 expr.components[i] = self._record_unique_expr(c, True)
-        assert expr.slot_idx < 0
+        assert expr.slot_idx is None
         expr.slot_idx = self._next_slot_idx()
         self.unique_exprs.append(expr)
         return expr
 
     def _record_output_expr_id(self, e: Expr, output_expr_id: int) -> None:
+        assert e.slot_idx is not None
+        assert output_expr_id is not None
+        if e.slot_idx in self.input_expr_slot_idxs:
+            return
         self.output_expr_ids[e.slot_idx].add(output_expr_id)
         for d in e.dependencies():
             self._record_output_expr_id(d, output_expr_id)
 
     def _compute_dependencies(self, target_slot_idxs: List[int], excluded_slot_idxs: List[int]) -> List[int]:
         """Compute exprs needed to materialize the given target slots, excluding 'excluded_slot_idxs'"""
         dependencies = [set() for _ in range(self.num_materialized)]  # indexed by slot_idx
```

### Comparing `pixeltable-0.2.5/pixeltable/exprs/rowid_ref.py` & `pixeltable-0.2.6/pixeltable/exprs/rowid_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exprs/type_cast.py` & `pixeltable-0.2.6/pixeltable/exprs/type_cast.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/exprs/variable.py` & `pixeltable-0.2.6/pixeltable/exprs/variable.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/ext/functions/yolox.py` & `pixeltable-0.2.6/pixeltable/ext/functions/yolox.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/func/aggregate_function.py` & `pixeltable-0.2.6/pixeltable/func/aggregate_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,17 @@
 
         # make sure the signature doesn't contain reserved parameter names;
         # do this after super().__init__(), otherwise self.name is invalid
         for param in signature.parameters:
             if param.lower() in self.RESERVED_PARAMS:
                 raise excs.Error(f'{self.name}(): parameter name {param} is reserved')
 
+    def exec(self, *args: Any, **kwargs: Any) -> Any:
+        raise NotImplementedError
+
     def help_str(self) -> str:
         res = super().help_str()
         res += '\n\n' + inspect.getdoc(self.agg_cls.update)
         return res
 
     def __call__(self, *args: object, **kwargs: object) -> 'pixeltable.exprs.Expr':
         from pixeltable import exprs
```

### Comparing `pixeltable-0.2.5/pixeltable/func/expr_template_function.py` & `pixeltable-0.2.6/pixeltable/func/expr_template_function.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import inspect
-from typing import Dict, Optional, Callable, List
+from typing import Dict, Optional, Any
 
 import pixeltable
 import pixeltable.exceptions as excs
-import pixeltable.type_system as ts
 from .function import Function
 from .signature import Signature, Parameter
 
 
 class ExprTemplateFunction(Function):
     """A parameterized expression from which an executable Expr is created with a function call."""
 
@@ -61,14 +60,24 @@
             else:
                 arg_expr = arg
             result = result.substitute(param_expr, arg_expr)
         import pixeltable.exprs as exprs
         assert not result.contains(exprs.Variable)
         return result
 
+    def exec(self, *args: Any, **kwargs: Any) -> Any:
+        expr = self.instantiate(*args, **kwargs)
+        import pixeltable.exprs as exprs
+        row_builder = exprs.RowBuilder(output_exprs=[expr], columns=[], input_exprs=[])
+        import pixeltable.exec as exec
+        row_batch = exec.DataRowBatch(tbl=None, row_builder=row_builder, len=1)
+        row = row_batch[0]
+        row_builder.eval(row, ctx=row_builder.default_eval_ctx)
+        return row[row_builder.get_output_exprs()[0].slot_idx]
+
     @property
     def display_name(self) -> str:
         return self.self_name
 
     @property
     def name(self) -> str:
         return self.self_name
```

### Comparing `pixeltable-0.2.5/pixeltable/func/function.py` & `pixeltable-0.2.6/pixeltable/func/function.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from __future__ import annotations
 
 import abc
 import importlib
 import inspect
-import pixeltable
-from typing import Optional, Dict, Any, Tuple
+from typing import Optional, Dict, Any, Tuple, Callable
 
+import pixeltable
+import pixeltable.type_system as ts
 from .globals import resolve_symbol
 from .signature import Signature
 
 
 class Function(abc.ABC):
     """Base class for Pixeltable's function interface.
 
     A function in Pixeltable is an object that has a signature and implements __call__().
     This base class provides a default serialization mechanism for Function instances provided by Python modules,
     via the member self_path.
     """
 
-    def __init__(self, signature: Signature, py_signature: inspect.Signature, self_path: Optional[str] = None):
+    def __init__(
+            self, signature: Signature, py_signature: inspect.Signature, self_path: Optional[str] = None
+    ):
         self.signature = signature
         self.py_signature = py_signature
         self.self_path = self_path  # fully-qualified path to self
+        self._conditional_return_type: Optional[Callable[..., ts.ColumnType]] = None
 
     @property
     def name(self) -> str:
         assert self.self_path is not None
         return self.self_path.split('.')[-1]
 
     @property
@@ -36,24 +40,51 @@
         if self.self_path.startswith(ptf_prefix):
             return self.self_path[len(ptf_prefix):]
         return self.self_path
 
     def help_str(self) -> str:
         return self.display_name + str(self.signature)
 
-    def __call__(self, *args: object, **kwargs: object) -> 'pixeltable.exprs.Expr':
+    def __call__(self, *args: Any, **kwargs: Any) -> 'pixeltable.exprs.Expr':
         from pixeltable import exprs
         bound_args = self.py_signature.bind(*args, **kwargs)
         self.validate_call(bound_args.arguments)
         return exprs.FunctionCall(self, bound_args.arguments)
 
     def validate_call(self, bound_args: Dict[str, Any]) -> None:
         """Override this to do custom validation of the arguments"""
         pass
 
+    def call_return_type(self, kwargs: dict[str, Any]) -> ts.ColumnType:
+        """Return the type of the value returned by calling this function with the given arguments"""
+        if self._conditional_return_type is None:
+            return self.signature.return_type
+        bound_args = self.py_signature.bind(**kwargs)
+        kw_args: dict[str, Any] = {}
+        sig = inspect.signature(self._conditional_return_type)
+        for param in sig.parameters.values():
+            if param.name in bound_args.arguments:
+                kw_args[param.name] = bound_args.arguments[param.name]
+        return self._conditional_return_type(**kw_args)
+
+    def conditional_return_type(self, fn: Callable[..., ts.ColumnType]) -> Callable[..., ts.ColumnType]:
+        """Instance decorator for specifying a conditional return type for this function"""
+        # verify that call_return_type only has parameters that are also present in the signature
+        sig = inspect.signature(fn)
+        for param in sig.parameters.values():
+            if param.name not in self.signature.parameters:
+                raise ValueError(f'`conditional_return_type` has parameter `{param.name}` that is not in the signature')
+        self._conditional_return_type = fn
+        return fn
+
+    @abc.abstractmethod
+    def exec(self, *args: Any, **kwargs: Any) -> Any:
+        """Execute the function with the given arguments and return the result."""
+        pass
+
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, self.__class__):
             return False
         return self.self_path == other.self_path
 
     def source(self) -> None:
         """Print source code"""
```

### Comparing `pixeltable-0.2.5/pixeltable/func/function_registry.py` & `pixeltable-0.2.6/pixeltable/func/function_registry.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/func/globals.py` & `pixeltable-0.2.6/pixeltable/func/globals.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/func/nos_function.py` & `pixeltable-0.2.6/pixeltable/func/nos_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/func/signature.py` & `pixeltable-0.2.6/pixeltable/func/signature.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,41 +25,31 @@
 Batch = typing.Annotated[list[T], 'pxt-batch']
 
 
 class Signature:
     """
     Represents the signature of a Pixeltable function.
 
-    Regarding return type:
-    - most functions will have a fixed return type, which is specified directly
-    - some functions will have a return type that depends on the argument values;
-      ex.: PIL.Image.Image.resize() returns an image with dimensions specified as a parameter
-    - in the latter case, the 'return_type' field is a function that takes the bound arguments and returns the
-      return type; if no bound arguments are specified, a generic return type is returned (eg, ImageType() without a
-      size)
     - self.is_batched: return type is a Batch[...] type
     """
     SPECIAL_PARAM_NAMES = ['group_by', 'order_by']
 
-    def __init__(
-            self,
-            return_type: Union[ts.ColumnType, Callable[[Dict[str, Any]], ts.ColumnType]],
-            parameters: List[Parameter], is_batched: bool = False):
+    def __init__(self, return_type: ts.ColumnType, parameters: List[Parameter], is_batched: bool = False):
+        assert isinstance(return_type, ts.ColumnType)
         self.return_type = return_type
         self.is_batched = is_batched
         # we rely on the ordering guarantee of dicts in Python >=3.7
         self.parameters = {p.name: p for p in parameters}
         self.parameters_by_pos = parameters.copy()
         self.constant_parameters = [p for p in parameters if not p.is_batched]
         self.batched_parameters = [p for p in parameters if p.is_batched]
 
-    def get_return_type(self, bound_args: Optional[Dict[str, Any]] = None) -> ts.ColumnType:
-        if isinstance(self.return_type, ts.ColumnType):
-            return self.return_type
-        return self.return_type(bound_args)
+    def get_return_type(self) -> ts.ColumnType:
+        assert isinstance(self.return_type, ts.ColumnType)
+        return self.return_type
 
     def as_dict(self) -> Dict[str, Any]:
         result = {
             'return_type': self.get_return_type().as_dict(),
             'parameters': [
                 [p.name, p.col_type.as_dict() if p.col_type is not None else None, p.kind, p.is_batched]
                 for p in self.parameters.values()
```

### Comparing `pixeltable-0.2.5/pixeltable/func/udf.py` & `pixeltable-0.2.6/pixeltable/func/udf.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import inspect
 from typing import List, Callable, Optional, overload, Any
 
 import pixeltable as pxt
 import pixeltable.exceptions as excs
 import pixeltable.type_system as ts
-from .batched_function import ExplicitBatchedFunction
 from .callable_function import CallableFunction
 from .expr_template_function import ExprTemplateFunction
 from .function import Function
 from .function_registry import FunctionRegistry
 from .globals import validate_symbol_path
 from .signature import Signature
 
@@ -58,32 +57,32 @@
         param_types = kwargs.pop('param_types', None)
         batch_size = kwargs.pop('batch_size', None)
         substitute_fn = kwargs.pop('py_fn', None)
         force_stored = kwargs.pop('_force_stored', False)
 
         def decorator(decorated_fn: Callable):
             return make_function(
-                decorated_fn, return_type, param_types, batch_size, substitute_fn=substitute_fn,
-                force_stored=force_stored)
+                decorated_fn, return_type, param_types, batch_size,
+                substitute_fn=substitute_fn, force_stored=force_stored)
 
         return decorator
 
 
 def make_function(
     decorated_fn: Callable,
     return_type: Optional[ts.ColumnType] = None,
     param_types: Optional[List[ts.ColumnType]] = None,
     batch_size: Optional[int] = None,
     substitute_fn: Optional[Callable] = None,
     function_name: Optional[str] = None,
     force_stored: bool = False
 ) -> Function:
     """
-    Constructs a `CallableFunction` or `BatchedFunction`, depending on the
-    supplied parameters. If `substitute_fn` is specified, then `decorated_fn`
+    Constructs a `CallableFunction` from the specified parameters.
+    If `substitute_fn` is specified, then `decorated_fn`
     will be used only for its signature, with execution delegated to
     `substitute_fn`.
     """
     # Obtain function_path from decorated_fn when appropriate
     if force_stored:
         # force storing the function in the db
         function_path = None
@@ -113,19 +112,16 @@
     if substitute_fn is None:
         py_fn = decorated_fn
     else:
         if function_path is None:
             raise excs.Error(f'{errmsg_name}(): @udf decorator with a `substitute_fn` can only be used in a module')
         py_fn = substitute_fn
 
-    if batch_size is None:
-        result = CallableFunction(signature=sig, py_fn=py_fn, self_path=function_path, self_name=function_name)
-    else:
-        result = ExplicitBatchedFunction(
-            signature=sig, batch_size=batch_size, invoker_fn=py_fn, self_path=function_path)
+    result = CallableFunction(
+        signature=sig, py_fn=py_fn, self_path=function_path, self_name=function_name, batch_size=batch_size)
 
     # If this function is part of a module, register it
     if function_path is not None:
         # do the validation at the very end, so it's easier to write tests for other failure scenarios
         validate_symbol_path(function_path)
         FunctionRegistry.get().register_function(function_path, result)
```

### Comparing `pixeltable-0.2.5/pixeltable/functions/__init__.py` & `pixeltable-0.2.6/pixeltable/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/functions/eval.py` & `pixeltable-0.2.6/pixeltable/functions/eval.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/functions/fireworks.py` & `pixeltable-0.2.6/pixeltable/functions/fireworks.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/functions/huggingface.py` & `pixeltable-0.2.6/pixeltable/functions/huggingface.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,24 @@
 
     model = _lookup_model(model_id, SentenceTransformer)
 
     array = model.encode(sentences, normalize_embeddings=normalize_embeddings)
     return [array[i] for i in range(array.shape[0])]
 
 
+@sentence_transformer.conditional_return_type
+def _(model_id: str) -> ts.ArrayType:
+    try:
+        from sentence_transformers import SentenceTransformer
+        model = _lookup_model(model_id, SentenceTransformer)
+        return ts.ArrayType((model.get_sentence_embedding_dimension(),), dtype=ts.FloatType(), nullable=False)
+    except ImportError:
+        return ts.ArrayType((None,), dtype=ts.FloatType(), nullable=False)
+
+
 @pxt.udf
 def sentence_transformer_list(sentences: list, *, model_id: str, normalize_embeddings: bool = False) -> list:
     env.Env.get().require_package('sentence_transformers')
     from sentence_transformers import SentenceTransformer
 
     model = _lookup_model(model_id, SentenceTransformer)
 
@@ -52,50 +62,59 @@
 
     model = _lookup_model(model_id, CrossEncoder)
 
     array = model.predict([[sentence1, s2] for s2 in sentences2], convert_to_numpy=True)
     return array.tolist()
 
 
-@pxt.udf(batch_size=32, return_type=ts.ArrayType((512,), dtype=ts.FloatType(), nullable=False))
+@pxt.udf(batch_size=32, return_type=ts.ArrayType((None,), dtype=ts.FloatType(), nullable=False))
 def clip_text(text: Batch[str], *, model_id: str) -> Batch[np.ndarray]:
     env.Env.get().require_package('transformers')
     device = resolve_torch_device('auto')
     import torch
     from transformers import CLIPModel, CLIPProcessor
 
     model = _lookup_model(model_id, CLIPModel.from_pretrained, device=device)
-    assert model.config.projection_dim == 512
     processor = _lookup_processor(model_id, CLIPProcessor.from_pretrained)
 
     with torch.no_grad():
         inputs = processor(text=text, return_tensors='pt', padding=True, truncation=True)
         embeddings = model.get_text_features(**inputs.to(device)).detach().to('cpu').numpy()
 
     return [embeddings[i] for i in range(embeddings.shape[0])]
 
 
-@pxt.udf(batch_size=32, return_type=ts.ArrayType((512,), dtype=ts.FloatType(), nullable=False))
+@pxt.udf(batch_size=32, return_type=ts.ArrayType((None,), dtype=ts.FloatType(), nullable=False))
 def clip_image(image: Batch[PIL.Image.Image], *, model_id: str) -> Batch[np.ndarray]:
     env.Env.get().require_package('transformers')
     device = resolve_torch_device('auto')
     import torch
     from transformers import CLIPModel, CLIPProcessor
 
     model = _lookup_model(model_id, CLIPModel.from_pretrained, device=device)
-    assert model.config.projection_dim == 512
     processor = _lookup_processor(model_id, CLIPProcessor.from_pretrained)
 
     with torch.no_grad():
         inputs = processor(images=image, return_tensors='pt', padding=True)
         embeddings = model.get_image_features(**inputs.to(device)).detach().to('cpu').numpy()
 
     return [embeddings[i] for i in range(embeddings.shape[0])]
 
 
+@clip_text.conditional_return_type
+@clip_image.conditional_return_type
+def _(model_id: str) -> ts.ArrayType:
+    try:
+        from transformers import CLIPModel
+        model = _lookup_model(model_id, CLIPModel.from_pretrained)
+        return ts.ArrayType((model.config.projection_dim,), dtype=ts.FloatType(), nullable=False)
+    except ImportError:
+        return ts.ArrayType((None,), dtype=ts.FloatType(), nullable=False)
+
+
 @pxt.udf(batch_size=4)
 def detr_for_object_detection(image: Batch[PIL.Image.Image], *, model_id: str, threshold: float = 0.5) -> Batch[dict]:
     env.Env.get().require_package('transformers')
     device = resolve_torch_device('auto')
     import torch
     from transformers import DetrImageProcessor, DetrForObjectDetection
```

### Comparing `pixeltable-0.2.5/pixeltable/functions/openai.py` & `pixeltable-0.2.6/pixeltable/functions/openai.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         model=model,
         voice=voice,
         response_format=_opt(response_format),
         speed=_opt(speed)
     )
     ext = response_format or 'mp3'
     output_filename = str(env.Env.get().tmp_dir / f"{uuid.uuid4()}.{ext}")
-    content.stream_to_file(output_filename, chunk_size=1 << 20)
+    content.write_to_file(output_filename)
     return output_filename
 
 
 @pxt.udf(
     param_types=[ts.AudioType(), ts.StringType(), ts.StringType(nullable=True),
                  ts.StringType(nullable=True), ts.FloatType(nullable=True)]
 )
@@ -177,34 +177,53 @@
     )
     return result.choices[0].message.content
 
 
 #####################################
 # Embeddings Endpoints
 
+_embedding_dimensions_cache: dict[str, int] = {
+    'text-embedding-ada-002': 1536,
+    'text-embedding-3-small': 1536,
+    'text-embedding-3-large': 3072,
+}
+
+
 @pxt.udf(batch_size=32, return_type=ts.ArrayType((None,), dtype=ts.FloatType()))
 @_retry
 def embeddings(
         input: Batch[str],
         *,
         model: str,
+        dimensions: Optional[int] = None,
         user: Optional[str] = None
 ) -> Batch[np.ndarray]:
     result = openai_client().embeddings.create(
         input=input,
         model=model,
+        dimensions=_opt(dimensions),
         user=_opt(user),
         encoding_format='float'
     )
     return [
         np.array(data.embedding, dtype=np.float64)
         for data in result.data
     ]
 
 
+@embeddings.conditional_return_type
+def _(model: str, dimensions: Optional[int] = None) -> ts.ArrayType:
+    if dimensions is None:
+        if model not in _embedding_dimensions_cache:
+            # TODO: find some other way to retrieve a sample
+            return ts.ArrayType((None,), dtype=ts.FloatType(), nullable=False)
+        dimensions = _embedding_dimensions_cache.get(model, None)
+    return ts.ArrayType((dimensions,), dtype=ts.FloatType(), nullable=False)
+
+
 #####################################
 # Images Endpoints
 
 @pxt.udf
 @_retry
 def image_generations(
         prompt: str,
@@ -228,14 +247,28 @@
     b64_str = result.data[0].b64_json
     b64_bytes = base64.b64decode(b64_str)
     img = PIL.Image.open(io.BytesIO(b64_bytes))
     img.load()
     return img
 
 
+@image_generations.conditional_return_type
+def _(size: Optional[str] = None) -> ts.ImageType:
+    if size is None:
+        return ts.ImageType(size=(1024, 1024))
+    x_pos = size.find('x')
+    if x_pos == -1:
+        return ts.ImageType()
+    try:
+        width, height = int(size[:x_pos]), int(size[x_pos + 1:])
+    except ValueError:
+        return ts.ImageType()
+    return ts.ImageType(size=(width, height))
+
+
 #####################################
 # Moderations Endpoints
 
 @pxt.udf
 @_retry
 def moderations(
         input: str,
```

### Comparing `pixeltable-0.2.5/pixeltable/functions/pil/image.py` & `pixeltable-0.2.6/pixeltable/functions/pil/image.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-from typing import Dict, Any, Tuple, Optional
+from typing import Tuple, Optional
 
 import PIL.Image
+from PIL.Image import Dither
 
-from pixeltable.type_system import FloatType, ImageType, IntType, ArrayType, ColumnType, StringType, JsonType, BoolType
 import pixeltable.func as func
+from pixeltable.type_system import FloatType, ImageType, IntType, ArrayType, ColumnType, StringType, JsonType
 
 
-def _caller_return_type(bound_args: Optional[Dict[str, Any]]) -> ColumnType:
-    if bound_args is None:
-        return ImageType()
-    return bound_args['self'].col_type
-
 @func.udf(
     py_fn=PIL.Image.alpha_composite, return_type=ImageType(), param_types=[ImageType(), ImageType()])
 def alpha_composite(im1: PIL.Image.Image, im2: PIL.Image.Image) -> PIL.Image.Image:
     pass
 @func.udf(
     py_fn=PIL.Image.blend, return_type=ImageType(), param_types=[ImageType(), ImageType(), FloatType()])
 def blend(im1: PIL.Image.Image, im2: PIL.Image.Image, alpha: float) -> PIL.Image.Image:
@@ -24,127 +20,128 @@
 def composite(image1: PIL.Image.Image, image2: PIL.Image.Image, mask: PIL.Image.Image) -> PIL.Image.Image:
     pass
 
 
 # PIL.Image.Image methods
 
 # Image.convert()
-def _convert_return_type(bound_args: Dict[str, Any]) -> ColumnType:
-    if bound_args is None:
-        return ImageType()
-    assert 'self' in bound_args
-    assert 'mode' in bound_args
-    img_type = bound_args['self'].col_type
-    return ImageType(size=img_type.size, mode=bound_args['mode'])
-@func.udf(return_type=_convert_return_type, param_types=[ImageType(), StringType()])
+@func.udf(param_types=[ImageType(), StringType()])
 def convert(self: PIL.Image.Image, mode: str) -> PIL.Image.Image:
     return self.convert(mode)
 
+
+@convert.conditional_return_type
+def _(self: PIL.Image.Image, mode: str) -> ColumnType:
+    input_type = self.col_type
+    assert input_type.is_image_type()
+    return ImageType(size=input_type.size, mode=mode, nullable=input_type.nullable)
+
+
 # Image.crop()
-def _crop_return_type(bound_args: Dict[str, Any]) -> ColumnType:
-    if bound_args is None:
-        return ImageType()
-    img_type = bound_args['self'].col_type
-    box = bound_args['box']
-    if isinstance(box, list) and all(isinstance(x, int) for x in box):
-        return ImageType(size=(box[2] - box[0], box[3] - box[1]), mode=img_type.mode)
-    return ImageType()  # we can't compute the size statically
 @func.udf(
-    py_fn=PIL.Image.Image.crop, return_type=_crop_return_type,
+    py_fn=PIL.Image.Image.crop,
     param_types=[ImageType(), ArrayType((4,), dtype=IntType())])
 def crop(self: PIL.Image.Image, box: Tuple[int, int, int, int]) -> PIL.Image.Image:
     pass
 
+@crop.conditional_return_type
+def _(self: PIL.Image.Image, box: Tuple[int, int, int, int]) -> ColumnType:
+    input_type = self.col_type
+    assert input_type.is_image_type()
+    if isinstance(box, list) and all(isinstance(x, int) for x in box):
+        return ImageType(size=(box[2] - box[0], box[3] - box[1]), mode=input_type.mode, nullable=input_type.nullable)
+    return ImageType(mode=input_type.mode, nullable=input_type.nullable)  # we can't compute the size statically
+
 # Image.getchannel()
-def _getchannel_return_type(bound_args: Dict[str, Any]) -> ColumnType:
-    if bound_args is None:
-        return ImageType()
-    img_type = bound_args['self'].col_type
-    return ImageType(size=img_type.size, mode='L')
-@func.udf(
-    py_fn=PIL.Image.Image.getchannel, return_type=_getchannel_return_type, param_types=[ImageType(), IntType()])
+@func.udf(py_fn=PIL.Image.Image.getchannel, param_types=[ImageType(), IntType()])
 def getchannel(self: PIL.Image.Image, channel: int) -> PIL.Image.Image:
     pass
 
+@getchannel.conditional_return_type
+def _(self: PIL.Image.Image) -> ColumnType:
+    input_type = self.col_type
+    assert input_type.is_image_type()
+    return ImageType(size=input_type.size, mode='L', nullable=input_type.nullable)
+
+
 # Image.resize()
-def resize_return_type(bound_args: Dict[str, Any]) -> ColumnType:
-    if bound_args is None:
-        return ImageType()
-    assert 'size' in bound_args
-    return ImageType(size=bound_args['size'])
-@func.udf(return_type=resize_return_type, param_types=[ImageType(), ArrayType((2, ), dtype=IntType())])
+@func.udf(param_types=[ImageType(), ArrayType((2, ), dtype=IntType())])
 def resize(self: PIL.Image.Image, size: Tuple[int, int]) -> PIL.Image.Image:
     return self.resize(size)
 
+@resize.conditional_return_type
+def _(self: PIL.Image.Image, size: Tuple[int, int]) -> ColumnType:
+    input_type = self.col_type
+    assert input_type.is_image_type()
+    return ImageType(size=size, mode=input_type.mode, nullable=input_type.nullable)
+
 # Image.rotate()
-@func.udf(return_type=ImageType(), param_types=[ImageType(), IntType()])
+@func.udf(param_types=[ImageType(), IntType()])
 def rotate(self: PIL.Image.Image, angle: int) -> PIL.Image.Image:
     return self.rotate(angle)
 
-# Image.transform()
-@func.udf(return_type= _caller_return_type, param_types=[ImageType(), ArrayType((2,), dtype=IntType()), IntType()])
-def transform(self: PIL.Image.Image, size: Tuple[int, int], method: int) -> PIL.Image.Image:
-    return self.transform(size, method)
+@func.udf(py_fn=PIL.Image.Image.effect_spread, param_types=[ImageType(), IntType()])
+def effect_spread(self: PIL.Image.Image, distance: int) -> PIL.Image.Image:
+    pass
 
-@func.udf(
-    py_fn=PIL.Image.Image.effect_spread, return_type=_caller_return_type, param_types=[ImageType(), FloatType()])
-def effect_spread(self: PIL.Image.Image, distance: float) -> PIL.Image.Image:
+@func.udf(py_fn=PIL.Image.Image.transpose, param_types=[ImageType(), IntType()])
+def transpose(self: PIL.Image.Image, method: int) -> PIL.Image.Image:
     pass
 
+@rotate.conditional_return_type
+@effect_spread.conditional_return_type
+@transpose.conditional_return_type
+def _(self: PIL.Image.Image) -> ColumnType:
+    return self.col_type
+
 @func.udf(
     py_fn=PIL.Image.Image.entropy, return_type=FloatType(), param_types=[ImageType(), ImageType(), JsonType()])
-def entropy(self: PIL.Image.Image, mask: PIL.Image.Image, histogram: Dict) -> float:
+def entropy(self: PIL.Image.Image, mask: PIL.Image.Image, extrema: Optional[list] = None) -> float:
     pass
 
 @func.udf(py_fn=PIL.Image.Image.getbands, return_type=JsonType(), param_types=[ImageType()])
 def getbands(self: PIL.Image.Image) -> Tuple[str]:
     pass
 
 @func.udf(py_fn=PIL.Image.Image.getbbox, return_type=JsonType(), param_types=[ImageType()])
 def getbbox(self: PIL.Image.Image) -> Tuple[int, int, int, int]:
     pass
 
-@func.udf(
-    py_fn=PIL.Image.Image.getcolors, return_type=JsonType(), param_types=[ImageType(), IntType()])
+@func.udf(py_fn=PIL.Image.Image.getcolors, return_type=JsonType(), param_types=[ImageType(), IntType()])
 def getcolors(self: PIL.Image.Image, maxcolors: int) -> Tuple[Tuple[int, int, int], int]:
     pass
 
 @func.udf(py_fn=PIL.Image.Image.getextrema, return_type=JsonType(), param_types=[ImageType()])
 def getextrema(self: PIL.Image.Image) -> Tuple[int, int]:
     pass
 
 @func.udf(
     py_fn=PIL.Image.Image.getpalette, return_type=JsonType(), param_types=[ImageType(), StringType()])
-def getpalette(self: PIL.Image.Image, mode: str) -> Tuple[int]:
+def getpalette(self: PIL.Image.Image, mode: Optional[str] = None) -> Tuple[int]:
     pass
 
 @func.udf(
-    py_fn=PIL.Image.Image.getpixel, return_type=JsonType(), param_types=[ImageType(), ArrayType((2,), dtype=IntType())])
-def getpixel(self: PIL.Image.Image, xy: Tuple[int, int]) -> Tuple[int]:
-    pass
+    return_type=JsonType(), param_types=[ImageType(), ArrayType((2,), dtype=IntType())])
+def getpixel(self: PIL.Image.Image, xy: tuple[int, int]) -> Tuple[int]:
+    # `xy` will be a list; `tuple(xy)` is necessary for pillow 9 compatibility
+    return self.getpixel(tuple(xy))
 
-@func.udf(
-    py_fn=PIL.Image.Image.getprojection, return_type=JsonType(), param_types=[ImageType()])
+@func.udf(py_fn=PIL.Image.Image.getprojection, return_type=JsonType(), param_types=[ImageType()])
 def getprojection(self: PIL.Image.Image) -> Tuple[int]:
     pass
 
-@func.udf(
-    py_fn=PIL.Image.Image.histogram, return_type=JsonType(), param_types=[ImageType(), ImageType(), JsonType()])
-def histogram(self: PIL.Image.Image, mask: PIL.Image.Image, histogram: Dict) -> Tuple[int]:
+@func.udf(py_fn=PIL.Image.Image.histogram, return_type=JsonType(), param_types=[ImageType(), ImageType(), JsonType()])
+def histogram(self: PIL.Image.Image, mask: PIL.Image.Image, extrema: Optional[list] = None) -> Tuple[int]:
     pass
 
 @func.udf(
     py_fn=PIL.Image.Image.quantize, return_type=ImageType(),
     param_types=[ImageType(), IntType(), IntType(nullable=True), IntType(), IntType(nullable=True), IntType()])
 def quantize(
-        self: PIL.Image.Image, colors: int, method: int, kmeans: int, palette: int, dither: int) -> PIL.Image.Image:
+        self: PIL.Image.Image, colors: int = 256, method: Optional[int] = None, kmeans: int = 0,
+        palette: Optional[int] = None, dither: int = Dither.FLOYDSTEINBERG) -> PIL.Image.Image:
     pass
 
 @func.udf(
     py_fn=PIL.Image.Image.reduce, return_type=ImageType(), param_types=[ImageType(), IntType(), JsonType()])
-def reduce(self: PIL.Image.Image, factor: int, filter: Tuple[int]) -> PIL.Image.Image:
-    pass
-
-@func.udf(
-    py_fn=PIL.Image.Image.transpose, return_type=_caller_return_type, param_types=[ImageType(), IntType()])
-def transpose(self: PIL.Image.Image, method: int) -> PIL.Image.Image:
+def reduce(self: PIL.Image.Image, factor: int, box: Optional[Tuple[int]]) -> PIL.Image.Image:
     pass
```

### Comparing `pixeltable-0.2.5/pixeltable/functions/string.py` & `pixeltable-0.2.6/pixeltable/functions/string.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/functions/util.py` & `pixeltable-0.2.6/pixeltable/functions/util.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/functions/video.py` & `pixeltable-0.2.6/pixeltable/functions/video.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/index/base.py` & `pixeltable-0.2.6/pixeltable/index/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 
 
 class IndexBase(abc.ABC):
     """
     Internal interface used by the catalog and runtime system to interact with indices:
     - types and expressions needed to create and populate the index value column
     - creating/dropping the index
-    - TODO: translating queries into sqlalchemy predicates
+    This doesn't cover querying the index, which is dependent on the index semantics and handled by
+    the specific subclass.
     """
+
     @abc.abstractmethod
     def __init__(self, c: catalog.Column, **kwargs: Any):
         pass
 
     @abc.abstractmethod
     def index_value_expr(self) -> 'pixeltable.exprs.Expr':
         """Return expression that computes the value that goes into the index"""
```

### Comparing `pixeltable-0.2.5/pixeltable/iterators/base.py` & `pixeltable-0.2.6/pixeltable/iterators/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,7 +42,11 @@
         """Close the iterator and release all resources"""
         raise NotImplementedError
 
     @abstractmethod
     def set_pos(self, pos: int) -> None:
         """Set the iterator position to pos"""
         raise NotImplementedError
+
+    @classmethod
+    def create(cls, **kwargs: Any) -> tuple[type[ComponentIterator], dict[str, Any]]:
+        return cls, kwargs
```

### Comparing `pixeltable-0.2.5/pixeltable/iterators/video.py` & `pixeltable-0.2.6/pixeltable/iterators/video.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-from typing import Dict, Any, List, Tuple
-from pathlib import Path
-import math
 import logging
+import math
+from pathlib import Path
+from typing import Dict, Any, List, Tuple
 
-import cv2
 import PIL.Image
+import cv2
 
-from .base import ComponentIterator
-
-from pixeltable.type_system import ColumnType, VideoType, ImageType, IntType, FloatType
+from pixeltable import exprs
 from pixeltable.exceptions import Error
-
+from pixeltable.type_system import ColumnType, VideoType, ImageType, IntType, FloatType
+from .base import ComponentIterator
 
 _logger = logging.getLogger('pixeltable')
 
 class FrameIterator(ComponentIterator):
-    def __init__(self, video: str, fps: float = 0.0):
+    def __init__(self, video: str, *, fps: float = 0.0):
         video_path = Path(video)
         assert video_path.exists() and video_path.is_file()
         self.video_path = video_path
         self.fps = fps
         self.video_reader = cv2.VideoCapture(str(video_path))
         if not self.video_reader.isOpened():
             raise Error(f'Failed to open video: {video}')
```

### Comparing `pixeltable-0.2.5/pixeltable/metadata/__init__.py` & `pixeltable-0.2.6/pixeltable/metadata/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import sqlalchemy as sql
 import sqlalchemy.orm as orm
 
 from .schema import SystemInfo, SystemInfoMd
 
 # current version of the metadata; this is incremented whenever the metadata schema changes
-VERSION = 12
+VERSION = 14
 
 
 def create_system_info(engine: sql.engine.Engine) -> None:
     """Create the systemmetadata record"""
     system_md = SystemInfoMd(schema_version=VERSION)
     record = SystemInfo(md=dataclasses.asdict(system_md))
     with orm.Session(engine, future=True) as session:
@@ -26,25 +26,29 @@
 # key: old schema version
 converter_cbs: Dict[int, Callable[[sql.engine.Engine], None]] = {}
 
 def register_converter(version: int, cb: Callable[[sql.engine.Engine], None]) -> None:
     global converter_cbs
     converter_cbs[version] = cb
 
+def noop_converter(engine: sql.engine.Engine) -> None:
+    # Converter to use when incrementing the schema version, but without any functional changes
+    pass
+
 # load all converter modules
 for _, modname, _ in pkgutil.iter_modules([os.path.dirname(__file__) + '/converters']):
     importlib.import_module('pixeltable.metadata.converters.' + modname)
 
 def upgrade_md(engine: sql.engine.Engine) -> None:
     """Upgrade the metadata schema to the current version"""
-    with orm.Session(engine, future=True) as session:
+    with orm.Session(engine) as session:
         system_info = session.query(SystemInfo).one().md
         md_version = system_info['schema_version']
         if md_version == VERSION:
-                return
+            return
         while md_version < VERSION:
             if md_version not in converter_cbs:
                 raise RuntimeError(f'No metadata converter for version {md_version}')
             print(f'Converting metadata from version {md_version} to {md_version + 1}')
             converter_cbs[md_version](engine)
             md_version += 1
         # update system info
```

### Comparing `pixeltable-0.2.5/pixeltable/metadata/converters/convert_10.py` & `pixeltable-0.2.6/pixeltable/metadata/converters/convert_10.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/metadata/schema.py` & `pixeltable-0.2.6/pixeltable/metadata/schema.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/plan.py` & `pixeltable-0.2.6/pixeltable/plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,33 +56,18 @@
         self.order_by_clause = [(e.resolve_computed_cols(), asc) for e, asc in order_by_clause]
 
         # Where clause of the Select stmt of the SQL scan
         self.sql_where_clause: Optional[exprs.Expr] = None
         # filter predicate applied to output rows of the SQL scan
         self.filter: Optional[exprs.Predicate] = None
         # not executable
-        self.similarity_clause: Optional[exprs.ImageSimilarityPredicate] = None
+        #self.similarity_clause: Optional[exprs.ImageSimilarityPredicate] = None
         if where_clause is not None:
             where_clause_conjuncts, self.filter = where_clause.split_conjuncts(lambda e: e.sql_expr() is not None)
             self.sql_where_clause = exprs.CompoundPredicate.make_conjunction(where_clause_conjuncts)
-            if self.filter is not None:
-                similarity_clauses, self.filter = self.filter.split_conjuncts(
-                    lambda e: isinstance(e, exprs.ImageSimilarityPredicate))
-                if len(similarity_clauses) > 1:
-                    raise excs.Error(f'More than one nearest() not supported')
-                if len(similarity_clauses) == 1:
-                    if len(self.order_by_clause) > 0:
-                        raise excs.Error((
-                            f'nearest() returns results in order of proximity and cannot be used in conjunction with '
-                            f'order_by()'))
-                    self.similarity_clause = similarity_clauses[0]
-                    img_col = self.similarity_clause.img_col_ref.col
-                    indexed_col_ids = {info.col.id for info in tbl.tbl_version.idxs_by_name.values()}
-                    if img_col.id not in indexed_col_ids:
-                        raise excs.Error(f'nearest() not available for unindexed column {img_col.name}')
 
         # all exprs that are evaluated in Python; not executable
         self.all_exprs = self.select_list.copy()
         self.all_exprs.extend(self.group_by_clause)
         self.all_exprs.extend([e for e, _ in self.order_by_clause])
         if self.filter is not None:
             self.all_exprs.append(self.filter)
@@ -200,16 +185,14 @@
     def create_count_stmt(
             cls, tbl: catalog.TableVersionPath, where_clause: Optional[exprs.Predicate] = None
     ) -> sql.Select:
         stmt = sql.select(sql.func.count('*'))
         refd_tbl_ids: Set[UUID] = set()
         if where_clause is not None:
             analyzer = cls.analyze(tbl, where_clause)
-            if analyzer.similarity_clause is not None:
-                raise excs.Error('nearest() cannot be used with count()')
             if analyzer.filter is not None:
                 raise excs.Error(f'Filter {analyzer.filter} not expressible in SQL')
             clause_element = analyzer.sql_where_clause.sql_expr()
             assert clause_element is not None
             stmt = stmt.where(clause_element)
             refd_tbl_ids = where_clause.tbl_ids()
         stmt = exec.SqlScanNode.create_from_clause(tbl, stmt, refd_tbl_ids)
@@ -566,15 +549,15 @@
         ctx = exec.ExecContext(row_builder)
 
         order_by_items = cls._determine_ordering(analyzer)
         sql_limit = 0 if is_agg_query else limit  # if we're aggregating, the limit applies to the agg output
         sql_select_list = analyzer.sql_exprs.copy()
         plan = exec.SqlScanNode(
             tbl, row_builder, select_list=sql_select_list, where_clause=analyzer.sql_where_clause,
-            filter=analyzer.filter, similarity_clause=analyzer.similarity_clause, order_by_items=order_by_items,
+            filter=analyzer.filter, order_by_items=order_by_items,
             limit=sql_limit, set_pk=with_pk, exact_version_only=exact_version_only)
         plan = cls._insert_prefetch_node(tbl.tbl_version.id, analyzer.select_list, row_builder, plan)
 
         if len(analyzer.group_by_clause) > 0 or len(analyzer.agg_fn_calls) > 0:
             # we're doing aggregation; the input of the AggregateNode are the grouping exprs plus the
             # args of the agg fn calls
             agg_input = exprs.ExprSet(analyzer.group_by_clause.copy())
```

### Comparing `pixeltable-0.2.5/pixeltable/store.py` & `pixeltable-0.2.6/pixeltable/store.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,18 +197,18 @@
         stmt = sql.text(f'ALTER TABLE {self._storage_name()} ADD COLUMN {col.store_name()} {col_type_str} NULL')
         log_stmt(_logger, stmt)
         conn.execute(stmt)
         added_storage_cols = [col.store_name()]
         if col.records_errors:
             # we also need to create the errormsg and errortype storage cols
             stmt = (f'ALTER TABLE {self._storage_name()} '
-                    f'ADD COLUMN {col.errormsg_store_name()} {StringType().to_sql()} DEFAULT NULL')
+                    f'ADD COLUMN {col.errormsg_store_name()} VARCHAR DEFAULT NULL')
             conn.execute(sql.text(stmt))
             stmt = (f'ALTER TABLE {self._storage_name()} '
-                    f'ADD COLUMN {col.errortype_store_name()} {StringType().to_sql()} DEFAULT NULL')
+                    f'ADD COLUMN {col.errortype_store_name()} VARCHAR DEFAULT NULL')
             conn.execute(sql.text(stmt))
             added_storage_cols.extend([col.errormsg_store_name(), col.errortype_store_name()])
         self.create_sa_tbl()
         _logger.info(f'Added columns {added_storage_cols} to storage table {self._storage_name()}')
 
     def drop_column(self, col: catalog.Column, conn: sql.engine.Connection) -> None:
         """Execute Alter Table Drop Column statement"""
```

### Comparing `pixeltable-0.2.5/pixeltable/tool/create_test_db_dump.py` & `pixeltable-0.2.6/pixeltable/tool/create_test_db_dump.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import pgserver
 import toml
 
 import pixeltable as pxt
 import pixeltable.metadata as metadata
 from pixeltable.env import Env
+from pixeltable.func import Batch
 from pixeltable.type_system import \
     StringType, IntType, FloatType, BoolType, TimestampType, JsonType
 
 _logger = logging.getLogger('pixeltable')
 
 
 class Dumper:
@@ -25,17 +26,15 @@
         mock_home_dir = self.output_dir / '.pixeltable'
         mock_home_dir.mkdir(parents=True, exist_ok=True)
         os.environ['PIXELTABLE_HOME'] = str(mock_home_dir)
         os.environ['PIXELTABLE_CONFIG'] = str(shared_home / 'config.yaml')
         os.environ['PIXELTABLE_DB'] = db_name
         os.environ['PIXELTABLE_PGDATA'] = str(shared_home / 'pgdata')
 
-        Env.get().set_up(reinit_db=True)
-        self.cl = pxt.Client()
-        self.cl.logging(level=logging.DEBUG, to_stdout=True)
+        Env.get().configure_logging(level=logging.DEBUG, to_stdout=True)
 
     def dump_db(self) -> None:
         md_version = metadata.VERSION
         dump_file = self.output_dir / f'pixeltable-v{md_version:03d}-test.dump.gz'
         _logger.info(f'Creating database dump at: {dump_file}')
         pg_package_dir = os.path.dirname(pgserver.__file__)
         pg_dump_binary = f'{pg_package_dir}/pginstall/bin/pg_dump'
@@ -72,16 +71,26 @@
             'c2': IntType(nullable=False),
             'c3': FloatType(nullable=False),
             'c4': BoolType(nullable=False),
             'c5': TimestampType(nullable=False),
             'c6': JsonType(nullable=False),
             'c7': JsonType(nullable=False),
         }
-        t = self.cl.create_table('sample_table', schema, primary_key='c2')
+        t = pxt.create_table('sample_table', schema, primary_key='c2')
+
+        # Add columns for InlineArray and InlineDict
         t.add_column(c8=[[1, 2, 3], [4, 5, 6]])
+        t.add_column(c9=[['a', 'b', 'c'], ['d', 'e', 'f']])
+        t.add_column(c10=[t.c1, [t.c1n, t.c2]])
+        t.add_column(c11={'int': 22, 'dict': {'key': 'val'}, 'expr': t.c1})
+
+        # InPredicate
+        t.add_column(isin_1=t.c1.isin(['test string 1', 'test string 2', 'test string 3']))
+        t.add_column(isin_2=t.c2.isin([1, 2, 3, 4, 5]))
+        t.add_column(isin_3=t.c2.isin(t.c6.f5))
 
         # Add columns for .astype converters to ensure they're persisted properly
         t.add_column(c2_as_float=t.c2.astype(FloatType()))
 
         # Add columns for .apply
         t.add_column(c2_to_string=t.c2.apply(str))
         t.add_column(c6_to_string=t.c6.apply(json.dumps))
@@ -132,32 +141,42 @@
                 'c5': c5_data[i],
                 'c6': c6_data[i],
                 'c7': c7_data[i],
             }
             for i in range(num_rows)
         ]
         t.insert(rows)
-        self.cl.create_dir('views')
-        v = self.cl.create_view('views.sample_view', t, filter=(t.c2 < 50))
-        _ = self.cl.create_view('views.sample_snapshot', t, filter=(t.c2 >= 75), is_snapshot=True)
+        pxt.create_dir('views')
+        v = pxt.create_view('views.sample_view', t, filter=(t.c2 < 50))
+        _ = pxt.create_view('views.sample_snapshot', t, filter=(t.c2 >= 75), is_snapshot=True)
+        e = pxt.create_view('views.empty_view', t, filter=t.c2 == 4171780)
+        assert e.count() == 0
         # Computed column using a library function
         v['str_format'] = pxt.functions.string.str_format('{0} {key}', t.c1, key=t.c1)
-        # Computed column using a bespoke udf
-        v['test_udf'] = test_udf(t.c2)
+        # Computed column using a bespoke stored udf
+        v['test_udf'] = test_udf_stored(t.c2)
+        # Computed column using a batched function
+        # (apply this to the empty view, since it's a "heavyweight" function)
+        e['batched'] = pxt.functions.huggingface.clip_text(t.c1, model_id='openai/clip-vit-base-patch32')
+        # computed column using a stored batched function
+        v['test_udf_batched'] = test_udf_stored_batched(t.c1, upper=False)
         # astype
         v['astype'] = t.c1.astype(pxt.FloatType())
-        # computed column using a stored function
-        v['stored'] = t.c1.apply(lambda x: f'Hello, {x}', col_type=pxt.StringType())
 
 
-@pxt.udf
-def test_udf(n: int) -> int:
+@pxt.udf(_force_stored=True)
+def test_udf_stored(n: int) -> int:
     return n + 1
 
 
+@pxt.udf(batch_size=4, _force_stored=True)
+def test_udf_stored_batched(strings: Batch[str], *, upper: bool = True) -> Batch[str]:
+    return [string.upper() if upper else string.lower() for string in strings]
+
+
 def main() -> None:
     _logger.info("Creating pixeltable test artifact.")
     dumper = Dumper()
     dumper.create_tables()
     dumper.dump_db()
```

### Comparing `pixeltable-0.2.5/pixeltable/tool/create_test_video.py` & `pixeltable-0.2.6/pixeltable/tool/create_test_video.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/type_system.py` & `pixeltable-0.2.6/pixeltable/type_system.py`

 * *Files 4% similar despite different names*

```diff
@@ -221,14 +221,16 @@
             return IntType()
         if isinstance(val, float):
             return FloatType()
         if isinstance(val, bool):
             return BoolType()
         if isinstance(val, datetime.datetime) or isinstance(val, datetime.date):
             return TimestampType()
+        if isinstance(val, PIL.Image.Image):
+            return ImageType(width=val.width, height=val.height)
         if isinstance(val, np.ndarray):
             col_type = ArrayType.from_literal(val)
             if col_type is not None:
                 return col_type
             # this could still be json-serializable
         if isinstance(val, dict) or isinstance(val, np.ndarray):
             try:
@@ -367,21 +369,14 @@
         return self._type == self.Type.DOCUMENT
 
     def is_media_type(self) -> bool:
         # types that refer to external media files
         return self.is_image_type() or self.is_video_type() or self.is_audio_type() or self.is_document_type()
 
     @abc.abstractmethod
-    def to_sql(self) -> str:
-        """
-        Return corresponding Postgres type.
-        """
-        pass
-
-    @abc.abstractmethod
     def to_sa_type(self) -> sql.types.TypeEngine:
         """
         Return corresponding SQLAlchemy type.
         """
         pass
 
     @staticmethod
@@ -400,17 +395,14 @@
         return None
 
 
 class InvalidType(ColumnType):
     def __init__(self, nullable: bool = False):
         super().__init__(self.Type.INVALID, nullable=nullable)
 
-    def to_sql(self) -> str:
-        assert False
-
     def to_sa_type(self) -> sql.types.TypeEngine:
         assert False
 
     def print_value(self, val: Any) -> str:
         assert False
 
     def _validate_literal(self, val: Any) -> None:
@@ -428,17 +420,14 @@
             try:
                 dt = datetime.datetime.fromisoformat(val)
                 return dt
             except ValueError:
                 return None
         return convert
 
-    def to_sql(self) -> str:
-        return 'VARCHAR'
-
     def to_sa_type(self) -> sql.types.TypeEngine:
         return sql.String()
 
     def print_value(self, val: Any) -> str:
         return f"'{val}'"
 
     def _validate_literal(self, val: Any) -> None:
@@ -454,32 +443,26 @@
         return val
 
 
 class IntType(ColumnType):
     def __init__(self, nullable: bool = False):
         super().__init__(self.Type.INT, nullable=nullable)
 
-    def to_sql(self) -> str:
-        return 'BIGINT'
-
     def to_sa_type(self) -> sql.types.TypeEngine:
         return sql.BigInteger()
 
     def _validate_literal(self, val: Any) -> None:
         if not isinstance(val, int):
             raise TypeError(f'Expected int, got {val.__class__.__name__}')
 
 
 class FloatType(ColumnType):
     def __init__(self, nullable: bool = False):
         super().__init__(self.Type.FLOAT, nullable=nullable)
 
-    def to_sql(self) -> str:
-        return 'FLOAT'
-
     def to_sa_type(self) -> sql.types.TypeEngine:
         return sql.Float()
 
     def _validate_literal(self, val: Any) -> None:
         if not isinstance(val, float):
             raise TypeError(f'Expected float, got {val.__class__.__name__}')
 
@@ -489,17 +472,14 @@
         return val
 
 
 class BoolType(ColumnType):
     def __init__(self, nullable: bool = False):
         super().__init__(self.Type.BOOL, nullable=nullable)
 
-    def to_sql(self) -> str:
-        return 'BOOLEAN'
-
     def to_sa_type(self) -> sql.types.TypeEngine:
         return sql.Boolean()
 
     def _validate_literal(self, val: Any) -> None:
         if not isinstance(val, bool):
             raise TypeError(f'Expected bool, got {val.__class__.__name__}')
 
@@ -509,17 +489,14 @@
         return val
 
 
 class TimestampType(ColumnType):
     def __init__(self, nullable: bool = False):
         super().__init__(self.Type.TIMESTAMP, nullable=nullable)
 
-    def to_sql(self) -> str:
-        return 'INTEGER'
-
     def to_sa_type(self) -> sql.types.TypeEngine:
         return sql.TIMESTAMP()
 
     def _validate_literal(self, val: Any) -> None:
         if not isinstance(val, datetime.datetime) and not isinstance(val, datetime.date):
             raise TypeError(f'Expected datetime.datetime or datetime.date, got {val.__class__.__name__}')
 
@@ -547,22 +524,21 @@
         type_spec = None
         if 'type_spec' in d:
             type_spec = {
                 field_name: cls.deserialize(field_type_dict) for field_name, field_type_dict in d['type_spec'].items()
             }
         return cls(type_spec, nullable=d['nullable'])
 
-    def to_sql(self) -> str:
-        return 'JSONB'
-
     def to_sa_type(self) -> sql.types.TypeEngine:
         return sql.dialects.postgresql.JSONB()
 
     def print_value(self, val: Any) -> str:
         val_type = self.infer_literal_type(val)
+        if val_type is None:
+            return super().print_value(val)
         if val_type == self:
             return str(val)
         return val_type.print_value(val)
 
     def _validate_literal(self, val: Any) -> None:
         if not isinstance(val, dict) and not isinstance(val, list):
             raise TypeError(f'Expected dict or list, got {val.__class__.__name__}')
@@ -653,17 +629,14 @@
     def _create_literal(self, val: Any) -> Any:
         if isinstance(val, (list,tuple)):
             # map python float to whichever numpy float is
             # declared for this type, rather than assume float64
             return np.array(val, dtype=self.numpy_dtype())
         return val
 
-    def to_sql(self) -> str:
-        return 'BYTEA'
-
     def to_sa_type(self) -> sql.types.TypeEngine:
         return sql.LargeBinary()
 
     def numpy_dtype(self) -> np.dtype:
         if self.dtype == self.Type.INT:
             return np.dtype(np.int64)
         if self.dtype == self.Type.FLOAT:
@@ -758,17 +731,14 @@
             if self.width != target.width or self.height != target.height:
                 img = img.resize((target.width, target.height))
             if self.mode != target.mode:
                 img = img.convert(target.mode.to_pil())
             return img
         return convert
 
-    def to_sql(self) -> str:
-        return 'VARCHAR'
-
     def to_sa_type(self) -> sql.types.TypeEngine:
         return sql.String()
 
     def _validate_literal(self, val: Any) -> None:
         if isinstance(val, PIL.Image.Image):
             return
         self._validate_file_path(val)
@@ -781,19 +751,16 @@
             raise excs.Error(f'Not a valid image: {val}') from None
 
 
 class VideoType(ColumnType):
     def __init__(self, nullable: bool = False):
         super().__init__(self.Type.VIDEO, nullable=nullable)
 
-    def to_sql(self) -> str:
-        # stored as a file path
-        return 'VARCHAR'
-
     def to_sa_type(self) -> sql.types.TypeEngine:
+        # stored as a file path
         return sql.String()
 
     def _validate_literal(self, val: Any) -> None:
         self._validate_file_path(val)
 
     def validate_media(self, val: Any) -> None:
         assert isinstance(val, str)
@@ -816,19 +783,16 @@
             raise excs.Error(f'Not a valid video: {val}') from None
 
 
 class AudioType(ColumnType):
     def __init__(self, nullable: bool = False):
         super().__init__(self.Type.AUDIO, nullable=nullable)
 
-    def to_sql(self) -> str:
-        # stored as a file path
-        return 'VARCHAR'
-
     def to_sa_type(self) -> sql.types.TypeEngine:
+        # stored as a file path
         return sql.String()
 
     def _validate_literal(self, val: Any) -> None:
         self._validate_file_path(val)
 
     def validate_media(self, val: Any) -> None:
         try:
@@ -860,28 +824,23 @@
             for type_str in type_strs:
                 if not hasattr(self.DocumentFormat, type_str):
                     raise ValueError(f'Invalid document type: {type_str}')
             self._doc_formats = [self.DocumentFormat[type_str.upper()] for type_str in type_strs]
         else:
             self._doc_formats = [t for t in self.DocumentFormat]
 
-    def to_sql(self) -> str:
-        # stored as a file path
-        return 'VARCHAR'
-
     def to_sa_type(self) -> sql.types.TypeEngine:
+        # stored as a file path
         return sql.String()
 
     def _validate_literal(self, val: Any) -> None:
         self._validate_file_path(val)
 
     def validate_media(self, val: Any) -> None:
         assert isinstance(val, str)
         from pixeltable.utils.documents import get_document_handle
-        with open(val, 'r', encoding='utf8') as fh:
-            try:
-                s = fh.read()
-                dh = get_document_handle(s)
-                if dh is None:
-                    raise excs.Error(f'Not a recognized document format: {val}')
-            except Exception as e:
-                raise excs.Error(f'Not a recognized document format: {val}') from None
+        try:
+            dh = get_document_handle(val)
+            if dh is None:
+                raise excs.Error(f'Not a recognized document format: {val}')
+        except Exception as e:
+            raise excs.Error(f'Not a recognized document format: {val}') from None
```

### Comparing `pixeltable-0.2.5/pixeltable/utils/arrow.py` & `pixeltable-0.2.6/pixeltable/utils/arrow.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/utils/clip.py` & `pixeltable-0.2.6/pixeltable/utils/clip.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/utils/coco.py` & `pixeltable-0.2.6/pixeltable/utils/coco.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/utils/filecache.py` & `pixeltable-0.2.6/pixeltable/utils/filecache.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/utils/hf_datasets.py` & `pixeltable-0.2.6/pixeltable/io/hf_datasets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,82 +1,113 @@
-import datasets
-from typing import Union, Optional, List, Dict, Any
-import pixeltable.type_system as ts
-from pixeltable import exceptions as excs
-import math
+from __future__ import annotations
+
 import logging
-import pixeltable
+import math
 import random
+import typing
+from typing import Union, Optional, Any
+
+import pixeltable
+import pixeltable.type_system as ts
+from pixeltable import exceptions as excs
+
+if typing.TYPE_CHECKING:
+    import datasets
 
 _logger = logging.getLogger(__name__)
 
 # use 100MB as the batch size limit for loading a huggingface dataset into pixeltable.
 # The primary goal is to bound memory use, regardless of dataset size.
 # Second goal is to limit overhead. 100MB is presumed to be reasonable for a lot of storage systems.
 _K_BATCH_SIZE_BYTES = 100_000_000
 
 # note, there are many more types. we allow overrides in the schema_override parameter
 # to handle cases where the appropriate type is not yet mapped, or to override this mapping.
 # https://huggingface.co/docs/datasets/v2.17.0/en/package_reference/main_classes#datasets.Value
-_hf_to_pxt: Dict[str, ts.ColumnType] = {
+_hf_to_pxt: dict[str, ts.ColumnType] = {
     'int32': ts.IntType(nullable=True),  # pixeltable widens to big int
     'int64': ts.IntType(nullable=True),
     'bool': ts.BoolType(nullable=True),
     'float32': ts.FloatType(nullable=True),
     'string': ts.StringType(nullable=True),
     'timestamp[s]': ts.TimestampType(nullable=True),
     'timestamp[ms]': ts.TimestampType(nullable=True),  # HF dataset iterator converts timestamps to datetime.datetime
 }
 
+
 def _to_pixeltable_type(
     feature_type: Union[datasets.ClassLabel, datasets.Value, datasets.Sequence],
 ) -> Optional[ts.ColumnType]:
     """Convert a huggingface feature type to a pixeltable ColumnType if one is defined."""
+    import datasets
+
     if isinstance(feature_type, datasets.ClassLabel):
         # enum, example: ClassLabel(names=['neg', 'pos'], id=None)
         return ts.StringType(nullable=True)
     elif isinstance(feature_type, datasets.Value):
         # example: Value(dtype='int64', id=None)
         return _hf_to_pxt.get(feature_type.dtype, None)
     elif isinstance(feature_type, datasets.Sequence):
         # example: cohere wiki. Sequence(feature=Value(dtype='float32', id=None), length=-1, id=None)
         dtype = _to_pixeltable_type(feature_type.feature)
         length = feature_type.length if feature_type.length != -1 else None
         return ts.ArrayType(shape=(length,), dtype=dtype)
     else:
         return None
 
+
 def _get_hf_schema(dataset: Union[datasets.Dataset, datasets.DatasetDict]) -> datasets.Features:
     """Get the schema of a huggingface dataset as a dictionary."""
+    import datasets
+
     first_dataset = dataset if isinstance(dataset, datasets.Dataset) else next(iter(dataset.values()))
     return first_dataset.features
 
+
 def huggingface_schema_to_pixeltable_schema(
     hf_dataset: Union[datasets.Dataset, datasets.DatasetDict],
-) -> Dict[str, Optional[ts.ColumnType]]:
+) -> dict[str, Optional[ts.ColumnType]]:
     """Generate a pixeltable schema from a huggingface dataset schema.
     Columns without a known mapping are mapped to None
     """
     hf_schema = _get_hf_schema(hf_dataset)
     pixeltable_schema = {
         column_name: _to_pixeltable_type(feature_type) for column_name, feature_type in hf_schema.items()
     }
     return pixeltable_schema
 
+
 def import_huggingface_dataset(
-    cl: 'pixeltable.Client',
     table_path: str,
     dataset: Union[datasets.Dataset, datasets.DatasetDict],
     *,
-    column_name_for_split: Optional[str],
-    schema_override: Optional[Dict[str, Any]],
+    column_name_for_split: Optional[str] = None,
+    schema_override: Optional[dict[str, Any]] = None,
     **kwargs,
 ) -> 'pixeltable.InsertableTable':
-    """See `pixeltable.Client.import_huggingface_dataset` for documentation"""
-    if table_path in cl.list_tables():
+    """Create a new `Table` from a Huggingface dataset, or dataset dict with multiple splits.
+        Requires datasets library to be installed.
+
+    Args:
+        path_str: Path to the table.
+        dataset: Huggingface datasets.Dataset or datasets.DatasetDict to insert into the table.
+        column_name_for_split: column name to use for split information. If None, no split information will be stored.
+        schema_override: Optional dictionary mapping column names to column type to override the corresponding defaults from
+        `pixeltable.utils.hf_datasets.huggingface_schema_to_pixeltable_schema`. The column type should be a pixeltable ColumnType.
+        For example, {'col_vid': VideoType()}, rather than {'col_vid': StringType()}.
+
+        kwargs: Additional arguments to pass to `create_table`.
+
+    Returns:
+        The newly created table. The table will have loaded the data from the dataset.
+    """
+    import datasets
+    import pixeltable as pxt
+
+    if table_path in pxt.list_tables():
         raise excs.Error(f'table {table_path} already exists')
 
     if not isinstance(dataset, (datasets.Dataset, datasets.DatasetDict)):
         raise excs.Error(f'`type(dataset)` must be `datasets.Dataset` or `datasets.DatasetDict`. Got {type(dataset)=}')
 
     if isinstance(dataset, datasets.Dataset):
         # when loading an hf dataset partially, dataset.split._name is sometimes the form "train[0:1000]"
@@ -118,17 +149,17 @@
         for (feature_name, feature_type) in hf_schema.items()
         if isinstance(feature_type, datasets.ClassLabel)
     }
 
     try:
         # random tmp name
         tmp_name = f'{table_path}_tmp_{random.randint(0, 100000000)}'
-        tab = cl.create_table(tmp_name, pixeltable_schema, **kwargs)
+        tab = pxt.create_table(tmp_name, pixeltable_schema, **kwargs)
 
-        def _translate_row(row: Dict[str, Any], split_name: str) -> Dict[str, Any]:
+        def _translate_row(row: dict[str, Any], split_name: str) -> dict[str, Any]:
             output_row = row.copy()
             # map all class labels to strings
             for field, values in categorical_features.items():
                 output_row[field] = values[row[field]]
             # add split name to row
             if column_name_for_split is not None:
                 output_row[column_name_for_split] = split_name
@@ -149,9 +180,9 @@
             if len(batch) > 0:
                 tab.insert(batch)
 
     except Exception as e:
         _logger.error(f'Error while inserting dataset into table: {tmp_name}')
         raise e
 
-    cl.move(tmp_name, table_path)
-    return cl.get_table(table_path)
+    pxt.move(tmp_name, table_path)
+    return pxt.get_table(table_path)
```

### Comparing `pixeltable-0.2.5/pixeltable/utils/media_store.py` & `pixeltable-0.2.6/pixeltable/utils/media_store.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/utils/parquet.py` & `pixeltable-0.2.6/pixeltable/io/parquet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,81 @@
+from __future__ import annotations
+
 import io
 import json
 import logging
+import random
+import typing
 from collections import deque
 from pathlib import Path
-from typing import Dict, List, Optional, Union
+from typing import Dict, Optional
 
-import numpy as np
 import PIL.Image
-import pyarrow as pa
-import pyarrow.parquet
+import numpy as np
 
+import pixeltable.exceptions as exc
 import pixeltable.type_system as ts
-from pixeltable.utils.arrow import iter_tuples, to_arrow_schema, to_pixeltable_schema
 from pixeltable.utils.transactional_directory import transactional_directory
-import pixeltable.exceptions as exc
 
-import random
+if typing.TYPE_CHECKING:
+    import pixeltable as pxt
+    import pyarrow as pa
 
 _logger = logging.getLogger(__name__)
 
 
-def _write_batch(value_batch : Dict[str, deque], schema : pa.Schema, output_path : Path) -> None:
+def _write_batch(value_batch: Dict[str, deque], schema: pa.Schema, output_path: Path) -> None:
+    import pyarrow as pa
+
     pydict = {}
     for field in schema:
         if isinstance(field.type, pa.FixedShapeTensorType):
             stacked_arr = np.stack(value_batch[field.name])
             pydict[field.name] = pa.FixedShapeTensorArray.from_numpy_ndarray(stacked_arr)
         else:
             pydict[field.name] = value_batch[field.name]
 
     tab = pa.Table.from_pydict(pydict, schema=schema)
     pa.parquet.write_table(tab, output_path)
 
-def save_parquet(df: 'pixeltable.DataFrame', dest_path: Path, partition_size_bytes: int = 100_000_000) -> None:
+
+def save_parquet(df: pxt.DataFrame, dest_path: Path, partition_size_bytes: int = 100_000_000) -> None:
     """
-        Internal method to stream dataframe data to parquet format.
-        Does not materialize the dataset to memory.
+    Internal method to stream dataframe data to parquet format.
+    Does not materialize the dataset to memory.
 
-        It preserves pixeltable type metadata in a json file, which would otherwise
-        not be available in the parquet format.
+    It preserves pixeltable type metadata in a json file, which would otherwise
+    not be available in the parquet format.
 
-        Images are stored inline in a compressed format in their parquet file.
+    Images are stored inline in a compressed format in their parquet file.
 
-        Args:
-            df : dataframe to save.
-            dest_path : path to directory to save the parquet files to.
-            partition_size_bytes : maximum target size for each chunk. Default 100_000_000 bytes.
+    Args:
+        df : dataframe to save.
+        dest_path : path to directory to save the parquet files to.
+        partition_size_bytes : maximum target size for each chunk. Default 100_000_000 bytes.
     """
+    from pixeltable.utils.arrow import to_arrow_schema
+
     column_names = df.get_column_names()
     column_types = df.get_column_types()
     type_dict = {k: v.as_dict() for k, v in zip(column_names, column_types)}
     arrow_schema = to_arrow_schema(dict(zip(column_names, column_types)))
 
     # store the changes atomically
     with transactional_directory(dest_path) as temp_path:
         # dump metadata json file so we can inspect what was the source of the parquet file later on.
-        json.dump(df._as_dict(), (temp_path / '.pixeltable.json').open('w')) # pylint: disable=protected-access
-        json.dump(type_dict, (temp_path / '.pixeltable.column_types.json').open('w')) # keep type metadata
+        json.dump(df._as_dict(), (temp_path / '.pixeltable.json').open('w'))  # pylint: disable=protected-access
+        json.dump(type_dict, (temp_path / '.pixeltable.column_types.json').open('w'))  # keep type metadata
 
         batch_num = 0
-        current_value_batch : Dict[str, deque] = {k:deque() for k in column_names}
+        current_value_batch: Dict[str, deque] = {k: deque() for k in column_names}
         current_byte_estimate = 0
 
-        for data_row in df._exec(): # pylint: disable=protected-access
-            for (col_name, col_type, e) in zip(column_names, column_types, df._select_list_exprs): # pylint: disable=protected-access
+        for data_row in df._exec():  # pylint: disable=protected-access
+            for col_name, col_type, e in zip(column_names, column_types, df._select_list_exprs):  # pylint: disable=protected-access
                 val = data_row[e.slot_idx]
                 if val is None:
                     current_value_batch[col_name].append(val)
                     continue
 
                 assert val is not None
                 if col_type.is_image_type():
@@ -108,60 +116,77 @@
                 else:
                     assert False, f'unknown type {col_type} for {col_name}'
 
                 current_value_batch[col_name].append(val)
                 current_byte_estimate += length
             if current_byte_estimate > partition_size_bytes:
                 assert batch_num < 100_000, 'wrote too many parquet files, unclear ordering'
-                _write_batch(current_value_batch, arrow_schema,  temp_path / f'part-{batch_num:05d}.parquet')
+                _write_batch(current_value_batch, arrow_schema, temp_path / f'part-{batch_num:05d}.parquet')
                 batch_num += 1
-                current_value_batch = {k:deque() for k in column_names}
+                current_value_batch = {k: deque() for k in column_names}
                 current_byte_estimate = 0
 
         _write_batch(current_value_batch, arrow_schema, temp_path / f'part-{batch_num:05d}.parquet')
 
 
 def parquet_schema_to_pixeltable_schema(parquet_path: str) -> Dict[str, Optional[ts.ColumnType]]:
     """Generate a default pixeltable schema for the given parquet file. Returns None for unknown types."""
+    import pyarrow as pa
+    from pixeltable.utils.arrow import to_pixeltable_schema
 
     input_path = Path(parquet_path).expanduser()
     parquet_dataset = pa.parquet.ParquetDataset(input_path)
     return to_pixeltable_schema(parquet_dataset.schema)
 
 
 def import_parquet(
-    cl: 'pixeltable.Client',
     table_path: str,
     *,
     parquet_path: str,
-    schema_override: Optional[Dict[str, ts.ColumnType]],
+    schema_override: Optional[Dict[str, ts.ColumnType]] = None,
     **kwargs,
-) -> 'catalog.InsertableTable':
-    """See `pixeltable.Client.import_parquet` for documentation"""
+) -> pxt.catalog.InsertableTable:
+    """Create a new `Table` from a Parquet file or set of files. Requires pyarrow to be installed.
+    Args:
+        path_str: Path to the table within pixeltable.
+        parquet_path: Path to an individual Parquet file or directory of Parquet files.
+        schema_override: Optional dictionary mapping column names to column type to override the default
+                        schema inferred from the Parquet file. The column type should be a pixeltable ColumnType.
+                        For example, {'col_vid': VideoType()}, rather than {'col_vid': StringType()}.
+                        Any fields not provided explicitly will map to types with `pixeltable.utils.parquet.parquet_schema_to_pixeltable_schema`
+        kwargs: Additional arguments to pass to `create_table`.
+
+    Returns:
+        The newly created table. The table will have loaded the data from the Parquet file(s).
+    """
+    import pixeltable as pxt
+    import pyarrow as pa
+    from pixeltable.utils.arrow import iter_tuples
+
     input_path = Path(parquet_path).expanduser()
     parquet_dataset = pa.parquet.ParquetDataset(input_path)
 
     schema = parquet_schema_to_pixeltable_schema(parquet_path)
     if schema_override is None:
         schema_override = {}
 
     schema.update(schema_override)
     for k, v in schema.items():
         if v is None:
             raise exc.Error(f'Could not infer pixeltable type for column {k} from parquet file')
 
-    if table_path in cl.list_tables():
+    if table_path in pxt.list_tables():
         raise exc.Error(f'Table {table_path} already exists')
 
     try:
         tmp_name = f'{table_path}_tmp_{random.randint(0, 100000000)}'
-        tab = cl.create_table(tmp_name, schema, **kwargs)
+        tab = pxt.create_table(tmp_name, schema, **kwargs)
         for fragment in parquet_dataset.fragments:
             for batch in fragment.to_batches():
                 dict_batch = list(iter_tuples(batch))
                 tab.insert(dict_batch)
     except Exception as e:
         _logger.error(f'Error while inserting Parquet file into table: {e}')
         raise e
 
-    cl.move(tmp_name, table_path)
-    return cl.get_table(table_path)
+    pxt.move(tmp_name, table_path)
+    return pxt.get_table(table_path)
```

### Comparing `pixeltable-0.2.5/pixeltable/utils/pytorch.py` & `pixeltable-0.2.6/pixeltable/utils/pytorch.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/utils/sql.py` & `pixeltable-0.2.6/pixeltable/utils/sql.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pixeltable/utils/transactional_directory.py` & `pixeltable-0.2.6/pixeltable/utils/transactional_directory.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.5/pyproject.toml` & `pixeltable-0.2.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core", "poetry-dynamic-versioning>=1.3.0,<2.0.0"]
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "pixeltable"
-version = "0.2.5"
+version = "0.2.6"
 description = "Pixeltable: The Multimodal AI Data Plane"
 authors = ["Marcel Kornacker <marcelk@gmail.com>"]
 readme = "README.md"
 exclude = [
     ".pytype",
     ".pytest_cache",
-    "pixeltable/.pytest_cache",
-    "pixeltable/tests/data"
+    "tests",
+    "docs",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-numpy = ">=1.26"
+setuptools = "69.1.1"  # setuptools >= 69.2 has known issues with Github Actions
+numpy = ">=1.25"
 pandas = ">=2.0,<3.0"
-pillow = ">=10.0"
+pillow = ">=9.3.0"
 opencv-python-headless = "^4.7.0.68"
 tqdm = "^4.64.1"
 jmespath = "^1.0.1"
-regex = "^2022.10.31"
 cloudpickle = "^2.2.1"
 psycopg2-binary = "^2.9.5"
 psutil = "^5.9.5"
 sqlalchemy = {extras = ["mypy"], version = "^2.0.23"}
 sqlalchemy-utils = "^0.41.1"
 pgvector = "^0.2.1"
 av = ">=10.0.0"
 beautifulsoup4 = "^4.0.0"
 requests = "^2.31.0"
 pyyaml = "^6.0.1"
 jinja2 = "^3.1.3"
 tenacity = "^8.2"
 pgserver = "0.1.2"
+mistune = "^3.0.2"
+pymupdf = "^1.24.1"
+ftfy = "^6.2.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 # pytest-related
 pytest = "^7.2.1"
@@ -65,24 +68,33 @@
 pycocotools = "^2.0.7"
 ipykernel = "^6.27.1"
 nbmake = "^1.4.6"
 # packages required by various optional pieces of the codebase
 torch = "^2.2"
 torchvision = "^0.17"
 pyarrow = ">=13.0.0"
-openai = "^1.0.0"
-together = "^1.0.1"
+openai = "^1.10.0"
+together = "^1.1"
 fireworks-ai = "^0.13.0"
 boto3 = "^1.17"
 spacy = "^3.0"
 en-core-web-sm = {url = "https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.7.1/en_core_web_sm-3.7.1-py3-none-any.whl"}
 tiktoken = ">=0.3"
 sentence-transformers = "^2.0.0"
 transformers = "^4.20"
 datasets = ">=2.15.0"
+openpyxl = ">=3.1"  # Excel (.xlsx) support
+
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = "git"
+dirty = true
+
+[tool.poetry-dynamic-versioning.substitution]
+files = ["pixeltable/__version__.py"]
 
 [tool.mypy]
 plugins = "sqlalchemy.ext.mypy.plugin"
 disallow_untyped_defs = true
 disallow_any_unimported = true
 no_implicit_optional = true
 check_untyped_defs = true
@@ -110,21 +122,25 @@
 disable = ["C0114","C0116","C0415","E1121","R0401","R0801","R0902","R0913","R0914","W0511"]
 
 [tool.pytest.ini_options]
 addopts = "-v -m \"not remote_api\""
 markers = [
     "remote_api: marks tests as calling a remote API (such as OpenAI)"
 ]
+filterwarnings = [
+    "ignore:The `dict` method is deprecated; use `model_dump` instead.:DeprecationWarning",
+    "ignore:Pydantic V1 style `@validator` validators are deprecated.:DeprecationWarning"
+]
 
 [tool.ruff]
 line-length = 120
 
 [tool.ruff.lint]
 select = ["F", "E", "W", "C", "I", "N", "B", "A", "ICN", "PYI", "SIM", "TD002", "PL", "RUF"]
 ignore = ["PLC0415", "PLR0904", "PLR0912", "PLR0913", "PLR0914", "PLR0915", "PLR2004"]
 preview = true
 
 [tool.ruff.lint.isort]
 known-first-party = ["pixeltable"]
 
 [tool.ruff.format]
-quote-style = "preserve"
+quote-style = "single"  # can be "single", "double", or "preserve"
```

### Comparing `pixeltable-0.2.5/PKG-INFO` & `pixeltable-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 Metadata-Version: 2.1
 Name: pixeltable
-Version: 0.2.5
+Version: 0.2.6
 Summary: Pixeltable: The Multimodal AI Data Plane
 Author: Marcel Kornacker
 Author-email: marcelk@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: av (>=10.0.0)
 Requires-Dist: beautifulsoup4 (>=4.0.0,<5.0.0)
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
+Requires-Dist: ftfy (>=6.2.0,<7.0.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
-Requires-Dist: numpy (>=1.26)
+Requires-Dist: mistune (>=3.0.2,<4.0.0)
+Requires-Dist: numpy (>=1.25)
 Requires-Dist: opencv-python-headless (>=4.7.0.68,<5.0.0.0)
 Requires-Dist: pandas (>=2.0,<3.0)
 Requires-Dist: pgserver (==0.1.2)
 Requires-Dist: pgvector (>=0.2.1,<0.3.0)
-Requires-Dist: pillow (>=10.0)
+Requires-Dist: pillow (>=9.3.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
+Requires-Dist: pymupdf (>=1.24.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: regex (>=2022.10.31,<2023.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: setuptools (==69.1.1)
 Requires-Dist: sqlalchemy-utils (>=0.41.1,<0.42.0)
 Requires-Dist: sqlalchemy[mypy] (>=2.0.23,<3.0.0)
 Requires-Dist: tenacity (>=8.2,<9.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
-<img src="docs/pixeltable-banner.png" width="45%"/>
+<img src="https://raw.githubusercontent.com/pixeltable/pixeltable/master/docs/pixeltable-banner.png" alt="Pixeltable" width="45%" />
 
 # Unifying Data, Models, and Orchestration for AI Products
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 &nbsp;&nbsp;
-![pytest status](https://github.com/pixeltable/pixeltable/actions/workflows/pytest.yml/badge.svg)
+[![pytest status](https://github.com/pixeltable/pixeltable/actions/workflows/pytest.yml/badge.svg)](https://github.com/pixeltable/pixeltable/actions)
 
 [Installation](https://pixeltable.github.io/pixeltable/getting-started/) | [Documentation](https://pixeltable.github.io/pixeltable/)
 </div>
 
 Pixeltable is a Python library that lets AI engineers and data scientists focus on exploration, modeling, and app development without dealing with the customary data plumbing.
 
 ## What problems does Pixeltable solve?
@@ -71,15 +74,15 @@
 pip install pixeltable
 ```
 
 To verify that it's working:
 
 ```
 import pixeltable as pxt
-cl = pxt.Client()
+pxt.init()
 ```
 
 For more detailed installation instructions, see the
 [Getting Started with Pixeltable](https://pixeltable.github.io/pixeltable/getting-started/)
 guide. Then, check out the
 [Pixeltable Basics](https://pixeltable.github.io/pixeltable/tutorials/pixeltable-basics/)
 tutorial for a tour of its most important features.
```

