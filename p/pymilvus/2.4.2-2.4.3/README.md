# Comparing `tmp/pymilvus-2.4.2.tar.gz` & `tmp/pymilvus-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymilvus-2.4.2.tar", last modified: Tue May 14 12:59:56 2024, max compression
+gzip compressed data, was "pymilvus-2.4.3.tar", last modified: Fri May 17 04:01:40 2024, max compression
```

## Comparing `pymilvus-2.4.2.tar` & `pymilvus-2.4.3.tar`

### file list

```diff
@@ -1,225 +1,227 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.998082 pymilvus-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.962081 pymilvus-2.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.962081 pymilvus-2.4.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/ISSUE_TEMPLATE/enhancement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/ISSUE_TEMPLATE/general-question.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/mergify.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.962081 pymilvus-2.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/workflows/check_milvus_proto.yml
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/workflows/code_checker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/workflows/doc_update_event.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/workflows/nightly_ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/workflows/publish_dev_package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/workflows/publish_on_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/workflows/release_event.yml
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-14 12:59:47.000000 pymilvus-2.4.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-14 12:59:47.000000 pymilvus-2.4.2/CONTRIBUTING_CN.md
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 12:59:47.000000 pymilvus-2.4.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-05-14 12:59:47.000000 pymilvus-2.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-14 12:59:47.000000 pymilvus-2.4.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-14 12:59:47.000000 pymilvus-2.4.2/OWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-14 12:59:55.998082 pymilvus-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-14 12:59:47.000000 pymilvus-2.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-14 12:59:47.000000 pymilvus-2.4.2/_version_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1306 2024-05-14 12:59:47.000000 pymilvus-2.4.2/check_proto_product.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.958081 pymilvus-2.4.2/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.958081 pymilvus-2.4.2/ci/docker/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.962081 pymilvus-2.4.2/ci/docker/milvus/
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-14 12:59:47.000000 pymilvus-2.4.2/ci/docker/milvus/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.966081 pymilvus-2.4.2/ci/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7597 2024-05-14 12:59:47.000000 pymilvus-2.4.2/ci/scripts/docker_image_find_tag.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.966081 pymilvus-2.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.966081 pymilvus-2.4.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.966081 pymilvus-2.4.2/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/_templates/autosummaryclass.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/about.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.970081 pymilvus-2.4.2/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/api/collection.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/api/connections.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/api/future.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/api/milvus_index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/api/partition.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/api/schema.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/api/search.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/api/utility.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/param.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.970081 pymilvus-2.4.2/docs/source/res/
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/res/Intro_to_Indexes.md
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/res/about_documentation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/results.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.978081 pymilvus-2.4.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/bfloat16_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/binary_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.978081 pymilvus-2.4.2/examples/cert/
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/cert/ca.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/cert/client.key
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/cert/client.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/cert/server.pem
--rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.978081 pymilvus-2.4.2/examples/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1139866 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/data/train_embeddings.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/dynamic_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example.py
--rw-r--r--   0 runner    (1001) docker     (127)    18184 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example_bulkinsert_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    17421 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example_bulkinsert_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    16018 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example_bulkwriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example_gpu_brute_force.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example_gpu_cagra.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example_group_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example_tls1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example_tls2.py
--rw-r--r--   0 runner    (1001) docker     (127)  1070736 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/films.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/float16_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/fuzzy_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/hello_hybrid_sparse_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    12007 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/hello_milvus.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/hello_milvus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/hello_milvus_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/hello_milvus_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/hello_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/hello_sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/hybrid_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/inverted_index_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.982082 pymilvus-2.4.2/examples/milvus_client/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/customize_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/customize_schema_auto_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/index.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/index_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/non_ascii_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/rbac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/simple_auto_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/multithreading_hello_milvus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/old_style_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/old_style_example_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/old_style_example_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/old_style_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/resource_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/resource_group_declarative_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/role_and_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.982082 pymilvus-2.4.2/pymilvus/
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.982082 pymilvus-2.4.2/pymilvus/bulk_writer/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/bulk_writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/bulk_writer/buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/bulk_writer/bulk_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/bulk_writer/bulk_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/bulk_writer/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/bulk_writer/local_bulk_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13461 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/bulk_writer/remote_bulk_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.986081 pymilvus-2.4.2/pymilvus/client/
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/asynch.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/blob.py
--rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/check.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    20429 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/entity_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    72991 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/grpc_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (127)    47348 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/singleton_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    59505 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/ts_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24250 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.990082 pymilvus-2.4.2/pymilvus/grpc_gen/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19238 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    29021 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/feder_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/feder_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    91367 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/milvus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)   104621 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/milvus_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   138400 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/milvus_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/msg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10071 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/msg_pb2.pyi
--rwxr-xr-x   0 runner    (1001) docker     (127)     2208 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/python_gen.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/rg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/rg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/schema_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14384 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/schema_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.990082 pymilvus-2.4.2/pymilvus/milvus_client/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/milvus_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/milvus_client/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/milvus_client/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    35578 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/milvus_client/milvus_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.990082 pymilvus-2.4.2/pymilvus/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.994082 pymilvus-2.4.2/pymilvus/orm/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    66019 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    21066 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/future.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    23291 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)    31276 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    23015 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    50438 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.998082 pymilvus-2.4.2/pymilvus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-14 12:59:55.000000 pymilvus-2.4.2/pymilvus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-14 12:59:55.000000 pymilvus-2.4.2/pymilvus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:59:55.000000 pymilvus-2.4.2/pymilvus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-14 12:59:55.000000 pymilvus-2.4.2/pymilvus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 12:59:55.000000 pymilvus-2.4.2/pymilvus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-14 12:59:47.000000 pymilvus-2.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:59:55.998082 pymilvus-2.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.998082 pymilvus-2.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/mock_milvus.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/mock_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    14886 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_create_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_grpc_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_milvus_lite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_ts_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.633430 pymilvus-2.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-17 04:01:30.000000 pymilvus-2.4.3/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.597430 pymilvus-2.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.597430 pymilvus-2.4.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-17 04:01:30.000000 pymilvus-2.4.3/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-17 04:01:30.000000 pymilvus-2.4.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-17 04:01:30.000000 pymilvus-2.4.3/.github/ISSUE_TEMPLATE/enhancement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-17 04:01:30.000000 pymilvus-2.4.3/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-17 04:01:30.000000 pymilvus-2.4.3/.github/ISSUE_TEMPLATE/general-question.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-17 04:01:30.000000 pymilvus-2.4.3/.github/mergify.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.601430 pymilvus-2.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-17 04:01:30.000000 pymilvus-2.4.3/.github/workflows/check_milvus_proto.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-17 04:01:30.000000 pymilvus-2.4.3/.github/workflows/code_checker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-17 04:01:30.000000 pymilvus-2.4.3/.github/workflows/doc_update_event.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-17 04:01:30.000000 pymilvus-2.4.3/.github/workflows/nightly_ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 04:01:30.000000 pymilvus-2.4.3/.github/workflows/publish_dev_package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-17 04:01:30.000000 pymilvus-2.4.3/.github/workflows/publish_on_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-17 04:01:30.000000 pymilvus-2.4.3/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-17 04:01:30.000000 pymilvus-2.4.3/.github/workflows/release_event.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-17 04:01:30.000000 pymilvus-2.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-17 04:01:30.000000 pymilvus-2.4.3/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-17 04:01:30.000000 pymilvus-2.4.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-17 04:01:30.000000 pymilvus-2.4.3/CONTRIBUTING_CN.md
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-17 04:01:30.000000 pymilvus-2.4.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-05-17 04:01:30.000000 pymilvus-2.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-17 04:01:30.000000 pymilvus-2.4.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-17 04:01:30.000000 pymilvus-2.4.3/OWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-05-17 04:01:40.633430 pymilvus-2.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-17 04:01:30.000000 pymilvus-2.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-17 04:01:30.000000 pymilvus-2.4.3/_version_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1306 2024-05-17 04:01:30.000000 pymilvus-2.4.3/check_proto_product.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.593430 pymilvus-2.4.3/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.593430 pymilvus-2.4.3/ci/docker/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.601430 pymilvus-2.4.3/ci/docker/milvus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-17 04:01:30.000000 pymilvus-2.4.3/ci/docker/milvus/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.601430 pymilvus-2.4.3/ci/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7597 2024-05-17 04:01:30.000000 pymilvus-2.4.3/ci/scripts/docker_image_find_tag.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.601430 pymilvus-2.4.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.601430 pymilvus-2.4.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.601430 pymilvus-2.4.3/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/_templates/autosummaryclass.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/about.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.605430 pymilvus-2.4.3/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/api/collection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/api/connections.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/api/future.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/api/milvus_index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/api/partition.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/api/schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/api/search.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/api/utility.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/param.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.605430 pymilvus-2.4.3/docs/source/res/
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/res/Intro_to_Indexes.md
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/res/about_documentation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-05-17 04:01:30.000000 pymilvus-2.4.3/docs/source/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.613430 pymilvus-2.4.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/bfloat16_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/binary_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.613430 pymilvus-2.4.3/examples/cert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/cert/ca.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/cert/client.key
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/cert/client.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/cert/server.pem
+-rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.613430 pymilvus-2.4.3/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1139866 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/data/train_embeddings.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/dynamic_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18184 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/example_bulkinsert_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17421 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/example_bulkinsert_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16018 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/example_bulkwriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/example_gpu_brute_force.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/example_gpu_cagra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/example_group_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/example_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/example_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/example_tls1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/example_tls2.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1070736 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/films.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/float16_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/fuzzy_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/hello_cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/hello_hybrid_sparse_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12007 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/hello_milvus.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/hello_milvus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/hello_milvus_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/hello_milvus_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/hello_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/hello_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/hybrid_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/inverted_index_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.617430 pymilvus-2.4.3/examples/milvus_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/milvus_client/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/milvus_client/customize_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/milvus_client/customize_schema_auto_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/milvus_client/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/milvus_client/index_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/milvus_client/non_ascii_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/milvus_client/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/milvus_client/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/milvus_client/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/milvus_client/simple_auto_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/milvus_client/simple_cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/milvus_client/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/multithreading_hello_milvus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/old_style_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/old_style_example_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/old_style_example_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/old_style_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/resource_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/resource_group_declarative_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/role_and_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-17 04:01:30.000000 pymilvus-2.4.3/examples/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.617430 pymilvus-2.4.3/pymilvus/
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.621430 pymilvus-2.4.3/pymilvus/bulk_writer/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/bulk_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/bulk_writer/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/bulk_writer/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/bulk_writer/bulk_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/bulk_writer/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/bulk_writer/local_bulk_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13461 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/bulk_writer/remote_bulk_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.621430 pymilvus-2.4.3/pymilvus/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20863 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/client/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/client/asynch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/client/blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/client/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20441 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/client/entity_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73124 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/client/grpc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/client/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47348 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/client/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/client/singleton_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59505 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/client/stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/client/ts_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25270 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.625430 pymilvus-2.4.3/pymilvus/grpc_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/grpc_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19238 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/grpc_gen/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29021 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/grpc_gen/common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/grpc_gen/feder_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/grpc_gen/feder_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    91367 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/grpc_gen/milvus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104621 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/grpc_gen/milvus_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   138400 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/grpc_gen/milvus_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/grpc_gen/msg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10071 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/grpc_gen/msg_pb2.pyi
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2116 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/grpc_gen/python_gen.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/grpc_gen/rg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/grpc_gen/rg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/grpc_gen/schema_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14384 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/grpc_gen/schema_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.625430 pymilvus-2.4.3/pymilvus/milvus_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/milvus_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/milvus_client/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/milvus_client/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35817 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/milvus_client/milvus_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.625430 pymilvus-2.4.3/pymilvus/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.629430 pymilvus-2.4.3/pymilvus/orm/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66019 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/orm/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21066 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/orm/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/orm/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/orm/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/orm/future.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/orm/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23291 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/orm/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/orm/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31276 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/orm/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/orm/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/orm/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23015 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/orm/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/orm/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50438 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/orm/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pymilvus/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.633430 pymilvus-2.4.3/pymilvus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-05-17 04:01:40.000000 pymilvus-2.4.3/pymilvus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-05-17 04:01:40.000000 pymilvus-2.4.3/pymilvus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 04:01:40.000000 pymilvus-2.4.3/pymilvus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-17 04:01:40.000000 pymilvus-2.4.3/pymilvus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 04:01:40.000000 pymilvus-2.4.3/pymilvus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-17 04:01:30.000000 pymilvus-2.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-17 04:01:30.000000 pymilvus-2.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 04:01:40.633430 pymilvus-2.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:01:40.633430 pymilvus-2.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-17 04:01:30.000000 pymilvus-2.4.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-05-17 04:01:30.000000 pymilvus-2.4.3/tests/mock_milvus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-17 04:01:30.000000 pymilvus-2.4.3/tests/mock_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-17 04:01:30.000000 pymilvus-2.4.3/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-05-17 04:01:30.000000 pymilvus-2.4.3/tests/test_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-17 04:01:30.000000 pymilvus-2.4.3/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-05-17 04:01:30.000000 pymilvus-2.4.3/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14886 2024-05-17 04:01:30.000000 pymilvus-2.4.3/tests/test_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-17 04:01:30.000000 pymilvus-2.4.3/tests/test_create_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-05-17 04:01:30.000000 pymilvus-2.4.3/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-17 04:01:30.000000 pymilvus-2.4.3/tests/test_grpc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-17 04:01:30.000000 pymilvus-2.4.3/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-17 04:01:30.000000 pymilvus-2.4.3/tests/test_milvus_lite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-17 04:01:30.000000 pymilvus-2.4.3/tests/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-05-17 04:01:30.000000 pymilvus-2.4.3/tests/test_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-05-17 04:01:30.000000 pymilvus-2.4.3/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-17 04:01:30.000000 pymilvus-2.4.3/tests/test_ts_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-17 04:01:30.000000 pymilvus-2.4.3/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-17 04:01:30.000000 pymilvus-2.4.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-17 04:01:30.000000 pymilvus-2.4.3/tests/utils.py
```

### Comparing `pymilvus-2.4.2/.github/ISSUE_TEMPLATE/bug_report.yaml` & `pymilvus-2.4.3/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/.github/ISSUE_TEMPLATE/enhancement.yaml` & `pymilvus-2.4.3/.github/ISSUE_TEMPLATE/enhancement.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/.github/ISSUE_TEMPLATE/feature_request.yaml` & `pymilvus-2.4.3/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/.github/ISSUE_TEMPLATE/general-question.yaml` & `pymilvus-2.4.3/.github/ISSUE_TEMPLATE/general-question.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/.github/mergify.yml` & `pymilvus-2.4.3/.github/mergify.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/.github/workflows/check_milvus_proto.yml` & `pymilvus-2.4.3/.github/workflows/check_milvus_proto.yml`

 * *Files 12% similar despite different names*

```diff
@@ -27,9 +27,10 @@
       run: |
         python -m pip install --upgrade pip
         pip install -e .
 
     - name: Try generate proto
       run: |
         git submodule update --init
+        make gen_proto
         make check_proto_product
```

### Comparing `pymilvus-2.4.2/.github/workflows/code_checker.yml` & `pymilvus-2.4.3/.github/workflows/code_checker.yml`

 * *Files 25% similar despite different names*

```diff
@@ -20,12 +20,12 @@
         with:
           python-version: ${{ matrix.python-version }}
       - name: check pyproject.toml install
         run: |
           pip install -e .
       - name: Install requirements
         run: |
-          pip install -r requirements.txt
+          pip install -e ".[dev]"
       - name: Run pylint
         shell: bash
         run: |
           make lint
```

### Comparing `pymilvus-2.4.2/.github/workflows/doc_update_event.yml` & `pymilvus-2.4.3/.github/workflows/doc_update_event.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/.github/workflows/nightly_ci.yml` & `pymilvus-2.4.3/.github/workflows/nightly_ci.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/.github/workflows/publish_dev_package.yml` & `pymilvus-2.4.3/.github/workflows/publish_dev_package.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/.github/workflows/publish_on_release.yml` & `pymilvus-2.4.3/.github/workflows/publish_on_release.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/.github/workflows/pull_request.yml` & `pymilvus-2.4.3/.github/workflows/pull_request.yml`

 * *Files 1% similar despite different names*

```diff
@@ -24,12 +24,12 @@
       - name: Fetch tags
         run: |
           git fetch --prune --unshallow --tags
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install -e ".[test]"
+          pip install -e ".[dev]"
 
       - name: Test with pytest
         run: |
           make unittest
```

### Comparing `pymilvus-2.4.2/.github/workflows/release_event.yml` & `pymilvus-2.4.3/.github/workflows/release_event.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/CONTRIBUTING.md` & `pymilvus-2.4.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/CONTRIBUTING_CN.md` & `pymilvus-2.4.3/CONTRIBUTING_CN.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/LICENSE` & `pymilvus-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/Makefile` & `pymilvus-2.4.3/Makefile`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 unittest:
 	PYTHONPATH=`pwd` python3 -m pytest tests --cov=pymilvus -v
 
 lint:
-	PYTHONPATH=`pwd` black pymilvus --check
-	PYTHONPATH=`pwd` ruff check pymilvus
+	PYTHONPATH=`pwd` python3 -m black pymilvus --check
+	PYTHONPATH=`pwd` python3 -m ruff check pymilvus
 
 format:
-	PYTHONPATH=`pwd` black pymilvus
-	PYTHONPATH=`pwd` ruff check pymilvus --fix
+	PYTHONPATH=`pwd` python3 -m black pymilvus
+	PYTHONPATH=`pwd` python3 -m ruff check pymilvus --fix
 
 codecov:
 	PYTHONPATH=`pwd` pytest --cov=pymilvus --cov-report=xml tests -x -v -rxXs
 
 example:
 	PYTHONPATH=`pwd` python examples/example.py
 
@@ -21,14 +21,15 @@
 package:
 	python3 -m build --sdist --wheel --outdir dist/ .
 
 get_proto:
 	git submodule update --init
 
 gen_proto:
+	python3 -m pip install -e ".[dev]"
 	cd pymilvus/grpc_gen && ./python_gen.sh
 
 check_proto_product: gen_proto
 	./check_proto_product.sh
 
 version:
 	python -m setuptools_scm
```

### Comparing `pymilvus-2.4.2/PKG-INFO` & `pymilvus-2.4.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: pymilvus
-Version: 2.4.2
+Version: 2.4.3
 Summary: Python Sdk for Milvus
 Author-email: Milvus Team <milvus-team@zilliz.com>
 Project-URL: repository, https://github.com/milvus-io/pymilvus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools>=67
-Requires-Dist: grpcio<=1.60.0,>=1.49.1
+Requires-Dist: grpcio<=1.63.0,>=1.49.1
 Requires-Dist: protobuf>=3.20.0
 Requires-Dist: environs<=9.5.0
 Requires-Dist: ujson>=2.0.0
 Requires-Dist: pandas>=1.2.4
 Requires-Dist: numpy<1.25.0; python_version <= "3.8"
 Requires-Dist: milvus_lite<2.5.0,>=2.4.0
 Provides-Extra: bulk-writer
 Requires-Dist: requests; extra == "bulk-writer"
 Requires-Dist: minio>=7.0.0; extra == "bulk-writer"
 Requires-Dist: pyarrow>=12.0.0; extra == "bulk-writer"
 Requires-Dist: azure-storage-blob; extra == "bulk-writer"
 Provides-Extra: model
 Requires-Dist: milvus-model>=0.1.0; extra == "model"
-Provides-Extra: test
-Requires-Dist: pytest>=5.3.4; extra == "test"
-Requires-Dist: pytest-cov>=2.8.1; extra == "test"
-Requires-Dist: pytest-timeout>=1.3.4; extra == "test"
-Requires-Dist: grpcio-testing; extra == "test"
-Requires-Dist: ruff>0.4.0; extra == "test"
-Requires-Dist: black; extra == "test"
+Provides-Extra: dev
+Requires-Dist: grpcio==1.62.2; extra == "dev"
+Requires-Dist: grpcio-tools==1.62.2; extra == "dev"
+Requires-Dist: grpcio-testing==1.62.2; extra == "dev"
+Requires-Dist: pytest>=5.3.4; extra == "dev"
+Requires-Dist: pytest-cov>=2.8.1; extra == "dev"
+Requires-Dist: pytest-timeout>=1.3.4; extra == "dev"
+Requires-Dist: ruff>0.4.0; extra == "dev"
+Requires-Dist: black; extra == "dev"
 
 # Milvus Python SDK
 
 [![version](https://img.shields.io/pypi/v/pymilvus.svg?color=blue)](https://pypi.org/project/pymilvus/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/pymilvus?logo=python&logoColor=blue)](https://pypi.org/project/pymilvus/)
 [![Downloads](https://static.pepy.tech/badge/pymilvus)](https://pepy.tech/project/pymilvus)
 [![Downloads](https://static.pepy.tech/badge/pymilvus/month)](https://pepy.tech/project/pymilvus)
@@ -67,14 +69,15 @@
 ## Installation
 
 You can install PyMilvus via `pip` or `pip3` for Python 3.8+:
 
 ```shell
 $ pip3 install pymilvus
 $ pip3 install pymilvus[model] # for milvus-model
+$ pip3 install pymilvus[bulk_writer] # for bulk_writer
 ```
 
 You can install a specific version of PyMilvus by:
 
 ```shell
 $ pip3 install pymilvus==2.3.7
 ```
@@ -92,16 +95,14 @@
 [milvus-proto](https://github.com/milvus-io/milvus-proto#usage) for details.
 ```shell
 $ git submodule update --init
 ```
 
 Q2. How to generate python files from milvus-proto?
 
-**Before generating python files, please install requirements in `requirements.txt`**
-
 A2.
 ```shell
 $ make gen_proto
 ```
 
 Q3. How to use the local PyMilvus repository for Milvus server?
 
@@ -124,18 +125,18 @@
 make format
 ```
 
 Q6. How to run unittests?
 
 A6
 ```shell
-$ pip install ".[test]"
+$ pip install ".[dev]"
 $ make unittest
 ```
-Q7. `zsh: no matches found: pymilvus[model]` in mac, how do I solve this?
+Q7. `zsh: no matches found: pymilvus[model]`, how do I solve this?
 
 A7
 ```shell
 $ pip install "pymilvus[model]"
 ```
 
 ## Documentation
```

### Comparing `pymilvus-2.4.2/README.md` & `pymilvus-2.4.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 ## Installation
 
 You can install PyMilvus via `pip` or `pip3` for Python 3.8+:
 
 ```shell
 $ pip3 install pymilvus
 $ pip3 install pymilvus[model] # for milvus-model
+$ pip3 install pymilvus[bulk_writer] # for bulk_writer
 ```
 
 You can install a specific version of PyMilvus by:
 
 ```shell
 $ pip3 install pymilvus==2.3.7
 ```
@@ -58,16 +59,14 @@
 [milvus-proto](https://github.com/milvus-io/milvus-proto#usage) for details.
 ```shell
 $ git submodule update --init
 ```
 
 Q2. How to generate python files from milvus-proto?
 
-**Before generating python files, please install requirements in `requirements.txt`**
-
 A2.
 ```shell
 $ make gen_proto
 ```
 
 Q3. How to use the local PyMilvus repository for Milvus server?
 
@@ -90,18 +89,18 @@
 make format
 ```
 
 Q6. How to run unittests?
 
 A6
 ```shell
-$ pip install ".[test]"
+$ pip install ".[dev]"
 $ make unittest
 ```
-Q7. `zsh: no matches found: pymilvus[model]` in mac, how do I solve this?
+Q7. `zsh: no matches found: pymilvus[model]`, how do I solve this?
 
 A7
 ```shell
 $ pip install "pymilvus[model]"
 ```
 
 ## Documentation
```

### Comparing `pymilvus-2.4.2/_version_helper.py` & `pymilvus-2.4.3/_version_helper.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/check_proto_product.sh` & `pymilvus-2.4.3/check_proto_product.sh`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/ci/docker/milvus/docker-compose.yml` & `pymilvus-2.4.3/ci/docker/milvus/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/ci/scripts/docker_image_find_tag.sh` & `pymilvus-2.4.3/ci/scripts/docker_image_find_tag.sh`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/docs/Makefile` & `pymilvus-2.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/docs/README.md` & `pymilvus-2.4.3/docs/README.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/docs/make.bat` & `pymilvus-2.4.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/docs/source/api/collection.rst` & `pymilvus-2.4.3/docs/source/api/collection.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/docs/source/api/connections.rst` & `pymilvus-2.4.3/docs/source/api/connections.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/docs/source/api/future.rst` & `pymilvus-2.4.3/docs/source/api/future.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/docs/source/api/milvus_index.rst` & `pymilvus-2.4.3/docs/source/api/milvus_index.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/docs/source/api/partition.rst` & `pymilvus-2.4.3/docs/source/api/partition.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/docs/source/api/schema.rst` & `pymilvus-2.4.3/docs/source/api/schema.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/docs/source/api/search.rst` & `pymilvus-2.4.3/docs/source/api/search.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/docs/source/api/utility.rst` & `pymilvus-2.4.3/docs/source/api/utility.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/docs/source/conf.py` & `pymilvus-2.4.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/docs/source/contribute.rst` & `pymilvus-2.4.3/docs/source/contribute.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/docs/source/faq.rst` & `pymilvus-2.4.3/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/docs/source/index.rst` & `pymilvus-2.4.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/docs/source/install.rst` & `pymilvus-2.4.3/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/docs/source/res/Intro_to_Indexes.md` & `pymilvus-2.4.3/docs/source/res/Intro_to_Indexes.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/docs/source/res/about_documentation.md` & `pymilvus-2.4.3/docs/source/res/about_documentation.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/docs/source/results.rst` & `pymilvus-2.4.3/docs/source/results.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/docs/source/tutorial.rst` & `pymilvus-2.4.3/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/bfloat16_example.py` & `pymilvus-2.4.3/examples/bfloat16_example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/binary_example.py` & `pymilvus-2.4.3/examples/binary_example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/cert/ca.pem` & `pymilvus-2.4.3/examples/cert/ca.pem`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/cert/client.key` & `pymilvus-2.4.3/examples/cert/client.key`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/cert/client.pem` & `pymilvus-2.4.3/examples/cert/client.pem`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/cert/server.pem` & `pymilvus-2.4.3/examples/cert/server.pem`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/collection.py` & `pymilvus-2.4.3/examples/collection.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/data/train_embeddings.csv` & `pymilvus-2.4.3/examples/data/train_embeddings.csv`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/database.py` & `pymilvus-2.4.3/examples/database.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/dynamic_field.py` & `pymilvus-2.4.3/examples/dynamic_field.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/example.py` & `pymilvus-2.4.3/examples/example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/example_bulkinsert_json.py` & `pymilvus-2.4.3/examples/example_bulkinsert_json.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/example_bulkinsert_numpy.py` & `pymilvus-2.4.3/examples/example_bulkinsert_numpy.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/example_bulkwriter.py` & `pymilvus-2.4.3/examples/example_bulkwriter.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/example_gpu_brute_force.py` & `pymilvus-2.4.3/examples/example_gpu_brute_force.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/example_gpu_cagra.py` & `pymilvus-2.4.3/examples/example_gpu_cagra.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/example_group_by.py` & `pymilvus-2.4.3/examples/example_group_by.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/example_index.py` & `pymilvus-2.4.3/examples/example_index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/example_str.py` & `pymilvus-2.4.3/examples/example_str.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/example_tls1.py` & `pymilvus-2.4.3/examples/example_tls1.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/example_tls2.py` & `pymilvus-2.4.3/examples/example_tls2.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/films.csv` & `pymilvus-2.4.3/examples/films.csv`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/float16_example.py` & `pymilvus-2.4.3/examples/float16_example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/fuzzy_match.py` & `pymilvus-2.4.3/examples/fuzzy_match.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/hello_hybrid_sparse_dense.py` & `pymilvus-2.4.3/examples/hello_hybrid_sparse_dense.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/hello_milvus.ipynb` & `pymilvus-2.4.3/examples/hello_milvus.ipynb`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/hello_milvus.py` & `pymilvus-2.4.3/examples/hello_milvus.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/hello_milvus_array.py` & `pymilvus-2.4.3/examples/hello_milvus_array.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/hello_milvus_delete.py` & `pymilvus-2.4.3/examples/hello_milvus_delete.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/hello_model.py` & `pymilvus-2.4.3/examples/hello_model.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/hello_sparse.py` & `pymilvus-2.4.3/examples/hello_sparse.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/hybrid_search.py` & `pymilvus-2.4.3/examples/hybrid_search.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/inverted_index_example.py` & `pymilvus-2.4.3/examples/inverted_index_example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/iterator.py` & `pymilvus-2.4.3/examples/iterator.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/milvus_client/alias.py` & `pymilvus-2.4.3/examples/milvus_client/alias.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/milvus_client/customize_schema.py` & `pymilvus-2.4.3/examples/milvus_client/customize_schema.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/milvus_client/customize_schema_auto_id.py` & `pymilvus-2.4.3/examples/milvus_client/customize_schema_auto_id.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/milvus_client/index.py` & `pymilvus-2.4.3/examples/milvus_client/index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/milvus_client/index_params.py` & `pymilvus-2.4.3/examples/milvus_client/index_params.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/milvus_client/non_ascii_encode.py` & `pymilvus-2.4.3/examples/milvus_client/non_ascii_encode.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/milvus_client/partition.py` & `pymilvus-2.4.3/examples/milvus_client/partition.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/milvus_client/rbac.py` & `pymilvus-2.4.3/examples/milvus_client/rbac.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/milvus_client/simple.py` & `pymilvus-2.4.3/examples/milvus_client/simple.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/milvus_client/simple_auto_id.py` & `pymilvus-2.4.3/examples/milvus_client/simple_auto_id.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/milvus_client/sparse.py` & `pymilvus-2.4.3/examples/milvus_client/sparse.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/multithreading_hello_milvus.py` & `pymilvus-2.4.3/examples/multithreading_hello_milvus.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/old_style_example.py` & `pymilvus-2.4.3/examples/old_style_example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/old_style_example_index.py` & `pymilvus-2.4.3/examples/old_style_example_index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/old_style_example_str.py` & `pymilvus-2.4.3/examples/old_style_example_str.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/old_style_query.py` & `pymilvus-2.4.3/examples/old_style_query.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/partition.py` & `pymilvus-2.4.3/examples/partition.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/resource_group.py` & `pymilvus-2.4.3/examples/resource_group.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/resource_group_declarative_api.py` & `pymilvus-2.4.3/examples/resource_group_declarative_api.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/role_and_privilege.py` & `pymilvus-2.4.3/examples/role_and_privilege.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/examples/user.py` & `pymilvus-2.4.3/examples/user.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/__init__.py` & `pymilvus-2.4.3/pymilvus/__init__.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/bulk_writer/__init__.py` & `pymilvus-2.4.3/pymilvus/bulk_writer/__init__.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/bulk_writer/buffer.py` & `pymilvus-2.4.3/pymilvus/bulk_writer/buffer.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/bulk_writer/bulk_import.py` & `pymilvus-2.4.3/pymilvus/bulk_writer/bulk_import.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/bulk_writer/bulk_writer.py` & `pymilvus-2.4.3/pymilvus/bulk_writer/bulk_writer.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/bulk_writer/constants.py` & `pymilvus-2.4.3/pymilvus/bulk_writer/constants.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/bulk_writer/local_bulk_writer.py` & `pymilvus-2.4.3/pymilvus/bulk_writer/local_bulk_writer.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/bulk_writer/remote_bulk_writer.py` & `pymilvus-2.4.3/pymilvus/bulk_writer/remote_bulk_writer.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/client/__init__.py` & `pymilvus-2.4.3/pymilvus/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/client/abstract.py` & `pymilvus-2.4.3/pymilvus/client/abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import abc
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 import ujson
 
 from pymilvus.exceptions import DataTypeNotMatchException, ExceptionsMessage, MilvusException
-from pymilvus.grpc_gen import schema_pb2
+from pymilvus.grpc_gen import common_pb2, schema_pb2
 from pymilvus.settings import Config
 
 from . import entity_helper, utils
 from .constants import DEFAULT_CONSISTENCY_LEVEL, RANKER_TYPE_RRF, RANKER_TYPE_WEIGHTED
 from .types import DataType
 
 
@@ -191,14 +191,15 @@
         self._primary_keys = []
         self._insert_cnt = 0
         self._delete_cnt = 0
         self._upsert_cnt = 0
         self._timestamp = 0
         self._succ_index = []
         self._err_index = []
+        self._cost = 0
 
         self._pack(raw)
 
     @property
     def primary_keys(self):
         return self._primary_keys
 
@@ -230,18 +231,24 @@
     def succ_index(self):
         return self._succ_index
 
     @property
     def err_index(self):
         return self._err_index
 
+    # The unit of this cost is vcu, similar to token
+    @property
+    def cost(self):
+        return self._cost
+
     def __str__(self):
         return (
             f"(insert count: {self._insert_cnt}, delete count: {self._delete_cnt}, upsert count: {self._upsert_cnt}, "
-            f"timestamp: {self._timestamp}, success count: {self.succ_count}, err count: {self.err_count})"
+            f"timestamp: {self._timestamp}, success count: {self.succ_count}, err count: {self.err_count}, "
+            f"cost: {self._cost})"
         )
 
     __repr__ = __str__
 
     # TODO
     # def error_code(self):
     #     pass
@@ -258,14 +265,17 @@
 
         self._insert_cnt = raw.insert_cnt
         self._delete_cnt = raw.delete_cnt
         self._upsert_cnt = raw.upsert_cnt
         self._timestamp = raw.timestamp
         self._succ_index = raw.succ_index
         self._err_index = raw.err_index
+        self._cost = int(
+            raw.status.extra_info["report_value"] if raw.status and raw.status.extra_info else "0"
+        )
 
 
 class SequenceIterator:
     def __init__(self, seq: Sequence[Any]):
         self._seq = seq
         self._idx = 0
 
@@ -370,18 +380,25 @@
             "expr": self.expr,
         }.__str__()
 
 
 class SearchResult(list):
     """nq results: List[Hits]"""
 
-    def __init__(self, res: schema_pb2.SearchResultData, round_decimal: Optional[int] = None):
+    def __init__(
+        self,
+        res: schema_pb2.SearchResultData,
+        round_decimal: Optional[int] = None,
+        status: Optional[common_pb2.Status] = None,
+    ):
         self._nq = res.num_queries
         all_topks = res.topks
 
+        self.cost = int(status.extra_info["report_value"] if status and status.extra_info else "0")
+
         output_fields = res.output_fields
         fields_data = res.fields_data
 
         all_pks: List[Union[str, int]] = []
         all_scores: List[float] = []
 
         if res.ids.HasField("int_id"):
@@ -493,15 +510,15 @@
         return field2data
 
     def __iter__(self) -> SequenceIterator:
         return SequenceIterator(self)
 
     def __str__(self) -> str:
         """Only print at most 10 query results"""
-        return str(list(map(str, self[:10])))
+        return f"data: {list(map(str, self[:10]))} {'...' if len(self) > 10 else ''}, cost: {self.cost}"
 
     __repr__ = __str__
 
 
 class Hits(list):
     ids: List[Union[str, int]]
     distances: List[float]
```

### Comparing `pymilvus-2.4.2/pymilvus/client/asynch.py` & `pymilvus-2.4.3/pymilvus/client/asynch.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         if self._future:
             self._future.exception()
 
 
 class SearchFuture(Future):
     def on_response(self, response: milvus_pb2.SearchResults):
         check_status(response.status)
-        return SearchResult(response.results)
+        return SearchResult(response.results, status=response.status)
 
 
 class MutationFuture(Future):
     def on_response(self, response: Any):
         check_status(response.status)
         return MutationResult(response)
```

### Comparing `pymilvus-2.4.2/pymilvus/client/check.py` & `pymilvus-2.4.3/pymilvus/client/check.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/client/entity_helper.py` & `pymilvus-2.4.3/pymilvus/client/entity_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,16 +103,16 @@
     else:
         dim = 0
         for _, row_data in enumerate(data):
             indices = []
             values = []
             row = row_data.items() if isinstance(row_data, dict) else row_data
             for index, value in row:
-                indices.append(index)
-                values.append(value)
+                indices.append(int(index))
+                values.append(float(value))
             result.contents.append(sparse_float_row_to_bytes(indices, values))
             dim = max(dim, indices[-1] + 1)
         result.dim = dim
     return result
 
 
 # converts schema_types.SparseFloatArray proto to Iterable[SparseRowOutputType]
```

### Comparing `pymilvus-2.4.2/pymilvus/client/grpc_handler.py` & `pymilvus-2.4.3/pymilvus/client/grpc_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,27 +40,29 @@
 from .prepare import Prepare
 from .types import (
     BulkInsertState,
     CompactionPlans,
     CompactionState,
     DatabaseInfo,
     DataType,
+    ExtraList,
     GrantInfo,
     Group,
     IndexState,
     LoadState,
     Plan,
     Replica,
     ResourceGroupConfig,
     ResourceGroupInfo,
     RoleInfo,
     Shard,
     State,
     Status,
     UserInfo,
+    get_cost_extra,
 )
 from .utils import (
     check_invalid_binary_vector,
     check_status,
     get_server_type,
     is_successful,
     len_of,
@@ -728,15 +730,15 @@
                 future = self._stub.Search.future(request, timeout=timeout)
                 func = kwargs.get("_callback", None)
                 return SearchFuture(future, func)
 
             response = self._stub.Search(request, timeout=timeout)
             check_status(response.status)
             round_decimal = kwargs.get("round_decimal", -1)
-            return SearchResult(response.results, round_decimal)
+            return SearchResult(response.results, round_decimal, status=response.status)
 
         except Exception as e:
             if kwargs.get("_async", False):
                 return SearchFuture(None, None, e)
             raise e from e
 
     def _execute_hybrid_search(
@@ -747,15 +749,15 @@
                 future = self._stub.HybridSearch.future(request, timeout=timeout)
                 func = kwargs.get("_callback", None)
                 return SearchFuture(future, func)
 
             response = self._stub.HybridSearch(request, timeout=timeout)
             check_status(response.status)
             round_decimal = kwargs.get("round_decimal", -1)
-            return SearchResult(response.results, round_decimal)
+            return SearchResult(response.results, round_decimal, status=response.status)
 
         except Exception as e:
             if kwargs.get("_async", False):
                 return SearchFuture(None, None, e)
             raise e from e
 
     @retry_on_rpc_failure(retry_on_inconsistent_requery=True)
@@ -1515,15 +1517,15 @@
 
         results = []
         for index in range(num_entities):
             entity_row_data = entity_helper.extract_row_data_from_fields_data(
                 response.fields_data, index, dynamic_fields
             )
             results.append(entity_row_data)
-        return results
+        return ExtraList(results, extra=get_cost_extra(response.status))
 
     @retry_on_rpc_failure()
     def load_balance(
         self,
         collection_name: str,
         src_node_id: int,
         dst_node_ids: List[int],
```

### Comparing `pymilvus-2.4.2/pymilvus/client/interceptor.py` & `pymilvus-2.4.3/pymilvus/client/interceptor.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/client/prepare.py` & `pymilvus-2.4.3/pymilvus/client/prepare.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/client/stub.py` & `pymilvus-2.4.3/pymilvus/client/stub.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/client/ts_utils.py` & `pymilvus-2.4.3/pymilvus/client/ts_utils.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/client/types.py` & `pymilvus-2.4.3/pymilvus/client/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 from enum import IntEnum
-from typing import Any, ClassVar, Dict, List, TypeVar, Union
+from typing import Any, ClassVar, Dict, List, Optional, TypeVar, Union
 
 from pymilvus.exceptions import (
     AutoIDException,
     ExceptionsMessage,
     InvalidConsistencyLevel,
 )
 from pymilvus.grpc_gen import common_pb2, rg_pb2
@@ -759,15 +759,14 @@
     @property
     def groups(self):
         return self._groups
 
 
 class ResourceGroupInfo:
     def __init__(self, resource_group: Any) -> None:
-
         self._name = resource_group.name
         self._capacity = resource_group.capacity
         self._num_available_node = resource_group.num_available_node
         self._num_loaded_replica = resource_group.num_loaded_replica
         self._num_outgoing_node = resource_group.num_outgoing_node
         self._num_incoming_node = resource_group.num_incoming_node
         self._config = resource_group.config
@@ -913,7 +912,40 @@
         self._properties = {}
 
         for p in info.properties:
             self.properties[p.key] = p.value
 
     def __str__(self) -> str:
         return f"DatabaseInfo(name={self.name}, properties={self.properties})"
+
+
+class ExtraList(list):
+    """
+    A list that can hold extra information.
+    Attributes:
+        extra (dict): The extra information of the list.
+    Example:
+        ExtraList([1, 2, 3], extra={"total": 3})
+    """
+
+    def __init__(self, *args, extra: Optional[Dict] = None, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self.extra = extra or {}
+
+    def __str__(self) -> str:
+        """Only print at most 10 query results"""
+        return f"data: {list(map(str, self[:10]))} {'...' if len(self) > 10 else ''}, extra_info: {self.extra}"
+
+    __repr__ = __str__
+
+
+def get_cost_from_status(status: Optional[common_pb2.Status] = None):
+    return int(status.extra_info["report_value"] if status and status.extra_info else "0")
+
+
+def get_cost_extra(status: Optional[common_pb2.Status] = None):
+    return {"cost": get_cost_from_status(status)}
+
+
+# Construct extra dict, the cost unit is the vcu, similar to tokenlike the
+def construct_cost_extra(cost: int):
+    return {"cost": cost}
```

### Comparing `pymilvus-2.4.2/pymilvus/client/utils.py` & `pymilvus-2.4.3/pymilvus/client/utils.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/decorators.py` & `pymilvus-2.4.3/pymilvus/decorators.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/exceptions.py` & `pymilvus-2.4.3/pymilvus/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/grpc_gen/common_pb2.py` & `pymilvus-2.4.3/pymilvus/grpc_gen/common_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: common.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `pymilvus-2.4.2/pymilvus/grpc_gen/common_pb2.pyi` & `pymilvus-2.4.3/pymilvus/grpc_gen/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/grpc_gen/feder_pb2.py` & `pymilvus-2.4.3/pymilvus/grpc_gen/feder_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: feder.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `pymilvus-2.4.2/pymilvus/grpc_gen/feder_pb2.pyi` & `pymilvus-2.4.3/pymilvus/grpc_gen/feder_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/grpc_gen/milvus_pb2.py` & `pymilvus-2.4.3/pymilvus/grpc_gen/milvus_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: milvus.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `pymilvus-2.4.2/pymilvus/grpc_gen/milvus_pb2.pyi` & `pymilvus-2.4.3/pymilvus/grpc_gen/milvus_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/grpc_gen/milvus_pb2_grpc.py` & `pymilvus-2.4.3/pymilvus/grpc_gen/milvus_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/grpc_gen/msg_pb2.py` & `pymilvus-2.4.3/pymilvus/grpc_gen/msg_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: msg.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `pymilvus-2.4.2/pymilvus/grpc_gen/msg_pb2.pyi` & `pymilvus-2.4.3/pymilvus/grpc_gen/msg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/grpc_gen/python_gen.sh` & `pymilvus-2.4.3/pymilvus/grpc_gen/python_gen.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 #!/bin/bash
 
 OUTDIR=.
 PROTO_DIR="milvus-proto/proto"
 
-python -m pip install "grpcio-tools==$(python3 -c 'import grpc; print(grpc.__version__)')"
-
 python -m grpc_tools.protoc -I ${PROTO_DIR} --python_out=${OUTDIR} --pyi_out=${OUTDIR} ${PROTO_DIR}/common.proto
 python -m grpc_tools.protoc -I ${PROTO_DIR} --python_out=${OUTDIR} --pyi_out=${OUTDIR} ${PROTO_DIR}/schema.proto
 python -m grpc_tools.protoc -I ${PROTO_DIR} --python_out=${OUTDIR} --pyi_out=${OUTDIR} ${PROTO_DIR}/feder.proto
 python -m grpc_tools.protoc -I ${PROTO_DIR} --python_out=${OUTDIR} --pyi_out=${OUTDIR} ${PROTO_DIR}/msg.proto
 python -m grpc_tools.protoc -I ${PROTO_DIR} --python_out=${OUTDIR} --pyi_out=${OUTDIR} ${PROTO_DIR}/rg.proto
 python -m grpc_tools.protoc -I ${PROTO_DIR} --python_out=${OUTDIR} --pyi_out=${OUTDIR} --grpc_python_out=${OUTDIR}  ${PROTO_DIR}/milvus.proto
```

### Comparing `pymilvus-2.4.2/pymilvus/grpc_gen/rg_pb2.py` & `pymilvus-2.4.3/pymilvus/grpc_gen/rg_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: rg.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `pymilvus-2.4.2/pymilvus/grpc_gen/rg_pb2.pyi` & `pymilvus-2.4.3/pymilvus/grpc_gen/rg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/grpc_gen/schema_pb2.py` & `pymilvus-2.4.3/pymilvus/grpc_gen/schema_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: schema.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `pymilvus-2.4.2/pymilvus/grpc_gen/schema_pb2.pyi` & `pymilvus-2.4.3/pymilvus/grpc_gen/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/milvus_client/index.py` & `pymilvus-2.4.3/pymilvus/milvus_client/index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/milvus_client/milvus_client.py` & `pymilvus-2.4.3/pymilvus/milvus_client/milvus_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 """MilvusClient for dealing with simple workflows."""
 
 import logging
 from typing import Dict, List, Optional, Union
 from uuid import uuid4
 
 from pymilvus.client.constants import DEFAULT_CONSISTENCY_LEVEL
-from pymilvus.client.types import ExceptionsMessage, LoadState
+from pymilvus.client.types import (
+    ExceptionsMessage,
+    ExtraList,
+    LoadState,
+    construct_cost_extra,
+)
 from pymilvus.exceptions import (
     DataTypeNotMatchException,
     MilvusException,
     ParamError,
     PrimaryKeyException,
 )
 from pymilvus.orm import utility
@@ -212,15 +217,19 @@
         # Insert into the collection.
         try:
             res = conn.insert_rows(
                 collection_name, data, partition_name=partition_name, timeout=timeout
             )
         except Exception as ex:
             raise ex from ex
-        return {"insert_count": res.insert_count, "ids": res.primary_keys}
+        return {
+            "insert_count": res.insert_count,
+            "ids": res.primary_keys,
+            "cost": res.cost,
+        }
 
     def upsert(
         self,
         collection_name: str,
         data: Union[Dict, List[Dict]],
         timeout: Optional[float] = None,
         partition_name: Optional[str] = "",
@@ -259,15 +268,18 @@
         try:
             res = conn.upsert_rows(
                 collection_name, data, partition_name=partition_name, timeout=timeout, **kwargs
             )
         except Exception as ex:
             raise ex from ex
 
-        return {"upsert_count": res.upsert_count}
+        return {
+            "upsert_count": res.upsert_count,
+            "cost": res.cost,
+        }
 
     def search(
         self,
         collection_name: str,
         data: Union[List[list], list],
         filter: str = "",
         limit: int = 10,
@@ -321,15 +333,15 @@
         ret = []
         for hits in res:
             query_result = []
             for hit in hits:
                 query_result.append(hit.to_dict())
             ret.append(query_result)
 
-        return ret
+        return ExtraList(ret, extra=construct_cost_extra(res.cost))
 
     def query(
         self,
         collection_name: str,
         filter: str = "",
         output_fields: Optional[List[str]] = None,
         timeout: Optional[float] = None,
@@ -539,15 +551,15 @@
         except Exception as ex:
             logger.error("Failed to delete primary keys in collection: %s", collection_name)
             raise ex from ex
 
         if ret_pks:
             return ret_pks
 
-        return {"delete_count": res.delete_count}
+        return {"delete_count": res.delete_count, "cost": res.cost}
 
     def get_collection_stats(self, collection_name: str, timeout: Optional[float] = None) -> Dict:
         conn = self._get_connection()
         stats = conn.get_collection_stats(collection_name, timeout=timeout)
         result = {stat.key: stat.value for stat in stats}
         if "row_count" in result:
             result["row_count"] = int(result["row_count"])
```

### Comparing `pymilvus-2.4.2/pymilvus/model/__init__.py` & `pymilvus-2.4.3/pymilvus/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/orm/__init__.py` & `pymilvus-2.4.3/pymilvus/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/orm/collection.py` & `pymilvus-2.4.3/pymilvus/orm/collection.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/orm/connections.py` & `pymilvus-2.4.3/pymilvus/orm/connections.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/orm/constants.py` & `pymilvus-2.4.3/pymilvus/orm/constants.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/orm/db.py` & `pymilvus-2.4.3/pymilvus/orm/db.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/orm/future.py` & `pymilvus-2.4.3/pymilvus/orm/future.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/orm/index.py` & `pymilvus-2.4.3/pymilvus/orm/index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/orm/iterator.py` & `pymilvus-2.4.3/pymilvus/orm/iterator.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/orm/mutation.py` & `pymilvus-2.4.3/pymilvus/orm/mutation.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,19 @@
     def succ_index(self):
         return self._mr.succ_index if self._mr else []
 
     @property
     def err_index(self):
         return self._mr.err_index if self._mr else []
 
+    # The unit of this cost is vcu, similar to token
+    @property
+    def cost(self):
+        return self._mr.cost if self._mr else 0
+
     def __str__(self) -> str:
         """
         Return the information of mutation result
 
         :return str:
             The information of mutation result.
         """
```

### Comparing `pymilvus-2.4.2/pymilvus/orm/partition.py` & `pymilvus-2.4.3/pymilvus/orm/partition.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/orm/prepare.py` & `pymilvus-2.4.3/pymilvus/orm/prepare.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/orm/role.py` & `pymilvus-2.4.3/pymilvus/orm/role.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/orm/schema.py` & `pymilvus-2.4.3/pymilvus/orm/schema.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/orm/types.py` & `pymilvus-2.4.3/pymilvus/orm/types.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/orm/utility.py` & `pymilvus-2.4.3/pymilvus/orm/utility.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus/settings.py` & `pymilvus-2.4.3/pymilvus/settings.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/pymilvus.egg-info/PKG-INFO` & `pymilvus-2.4.3/pymilvus.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: pymilvus
-Version: 2.4.2
+Version: 2.4.3
 Summary: Python Sdk for Milvus
 Author-email: Milvus Team <milvus-team@zilliz.com>
 Project-URL: repository, https://github.com/milvus-io/pymilvus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools>=67
-Requires-Dist: grpcio<=1.60.0,>=1.49.1
+Requires-Dist: grpcio<=1.63.0,>=1.49.1
 Requires-Dist: protobuf>=3.20.0
 Requires-Dist: environs<=9.5.0
 Requires-Dist: ujson>=2.0.0
 Requires-Dist: pandas>=1.2.4
 Requires-Dist: numpy<1.25.0; python_version <= "3.8"
 Requires-Dist: milvus_lite<2.5.0,>=2.4.0
 Provides-Extra: bulk-writer
 Requires-Dist: requests; extra == "bulk-writer"
 Requires-Dist: minio>=7.0.0; extra == "bulk-writer"
 Requires-Dist: pyarrow>=12.0.0; extra == "bulk-writer"
 Requires-Dist: azure-storage-blob; extra == "bulk-writer"
 Provides-Extra: model
 Requires-Dist: milvus-model>=0.1.0; extra == "model"
-Provides-Extra: test
-Requires-Dist: pytest>=5.3.4; extra == "test"
-Requires-Dist: pytest-cov>=2.8.1; extra == "test"
-Requires-Dist: pytest-timeout>=1.3.4; extra == "test"
-Requires-Dist: grpcio-testing; extra == "test"
-Requires-Dist: ruff>0.4.0; extra == "test"
-Requires-Dist: black; extra == "test"
+Provides-Extra: dev
+Requires-Dist: grpcio==1.62.2; extra == "dev"
+Requires-Dist: grpcio-tools==1.62.2; extra == "dev"
+Requires-Dist: grpcio-testing==1.62.2; extra == "dev"
+Requires-Dist: pytest>=5.3.4; extra == "dev"
+Requires-Dist: pytest-cov>=2.8.1; extra == "dev"
+Requires-Dist: pytest-timeout>=1.3.4; extra == "dev"
+Requires-Dist: ruff>0.4.0; extra == "dev"
+Requires-Dist: black; extra == "dev"
 
 # Milvus Python SDK
 
 [![version](https://img.shields.io/pypi/v/pymilvus.svg?color=blue)](https://pypi.org/project/pymilvus/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/pymilvus?logo=python&logoColor=blue)](https://pypi.org/project/pymilvus/)
 [![Downloads](https://static.pepy.tech/badge/pymilvus)](https://pepy.tech/project/pymilvus)
 [![Downloads](https://static.pepy.tech/badge/pymilvus/month)](https://pepy.tech/project/pymilvus)
@@ -67,14 +69,15 @@
 ## Installation
 
 You can install PyMilvus via `pip` or `pip3` for Python 3.8+:
 
 ```shell
 $ pip3 install pymilvus
 $ pip3 install pymilvus[model] # for milvus-model
+$ pip3 install pymilvus[bulk_writer] # for bulk_writer
 ```
 
 You can install a specific version of PyMilvus by:
 
 ```shell
 $ pip3 install pymilvus==2.3.7
 ```
@@ -92,16 +95,14 @@
 [milvus-proto](https://github.com/milvus-io/milvus-proto#usage) for details.
 ```shell
 $ git submodule update --init
 ```
 
 Q2. How to generate python files from milvus-proto?
 
-**Before generating python files, please install requirements in `requirements.txt`**
-
 A2.
 ```shell
 $ make gen_proto
 ```
 
 Q3. How to use the local PyMilvus repository for Milvus server?
 
@@ -124,18 +125,18 @@
 make format
 ```
 
 Q6. How to run unittests?
 
 A6
 ```shell
-$ pip install ".[test]"
+$ pip install ".[dev]"
 $ make unittest
 ```
-Q7. `zsh: no matches found: pymilvus[model]` in mac, how do I solve this?
+Q7. `zsh: no matches found: pymilvus[model]`, how do I solve this?
 
 A7
 ```shell
 $ pip install "pymilvus[model]"
 ```
 
 ## Documentation
```

### Comparing `pymilvus-2.4.2/pymilvus.egg-info/SOURCES.txt` & `pymilvus-2.4.3/pymilvus.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 examples/example_index.py
 examples/example_str.py
 examples/example_tls1.py
 examples/example_tls2.py
 examples/films.csv
 examples/float16_example.py
 examples/fuzzy_match.py
+examples/hello_cost.py
 examples/hello_hybrid_sparse_dense.py
 examples/hello_milvus.ipynb
 examples/hello_milvus.py
 examples/hello_milvus_array.py
 examples/hello_milvus_delete.py
 examples/hello_model.py
 examples/hello_sparse.py
@@ -104,14 +105,15 @@
 examples/milvus_client/index.py
 examples/milvus_client/index_params.py
 examples/milvus_client/non_ascii_encode.py
 examples/milvus_client/partition.py
 examples/milvus_client/rbac.py
 examples/milvus_client/simple.py
 examples/milvus_client/simple_auto_id.py
+examples/milvus_client/simple_cost.py
 examples/milvus_client/sparse.py
 pymilvus/__init__.py
 pymilvus/decorators.py
 pymilvus/exceptions.py
 pymilvus/settings.py
 pymilvus.egg-info/PKG-INFO
 pymilvus.egg-info/SOURCES.txt
```

### Comparing `pymilvus-2.4.2/pyproject.toml` & `pymilvus-2.4.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   {name='Milvus Team', email="milvus-team@zilliz.com"},
 ]
 requires-python = '>=3.8'
 description = "Python Sdk for Milvus"
 readme = "README.md"
 dependencies=[
     "setuptools >= 67", # python3.12 pkg_resources
-    "grpcio>=1.49.1,<=1.60.0",
+    "grpcio>=1.49.1, <=1.63.0",
     "protobuf>=3.20.0",
     "environs<=9.5.0",
     "ujson>=2.0.0",
     "pandas>=1.2.4",
     "numpy<1.25.0;python_version<='3.8'",
     "milvus_lite>=2.4.0,<2.5.0",
 ]
@@ -45,19 +45,23 @@
     "azure-storage-blob",
 ]
 
 model = [
     "milvus-model>=0.1.0",
 ]
 
-test = [
+dev = [
+    # The generated codes of 1.63.0 is incompatible with versions < 1.63.0,
+    # so we use fixed grpcio version to develop.
+    "grpcio==1.62.2",
+    "grpcio-tools==1.62.2",
+    "grpcio-testing==1.62.2",
     "pytest>=5.3.4",
     "pytest-cov>=2.8.1",
     "pytest-timeout>=1.3.4",
-    "grpcio-testing",
     "ruff>0.4.0",
     "black",
 ]
 
 [tool.setuptools.dynamic]
 version = { attr = "_version_helper.version"}
```

### Comparing `pymilvus-2.4.2/requirements.txt` & `pymilvus-2.4.3/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 build==0.4.0
 certifi==2023.7.22
 chardet==4.0.0
 environs==9.5.0
-grpcio==1.60.0
-grpcio-testing==1.60.0
-grpcio-tools==1.60.0
+grpcio==1.62.2
+grpcio-testing==1.62.2
+grpcio-tools==1.62.2
 protobuf==4.25.2
 idna==2.10
 packaging==20.9
 pep517==0.10.0
 pyparsing==2.4.7
 six==1.16.0
 toml==0.10.2
```

### Comparing `pymilvus-2.4.2/tests/conftest.py` & `pymilvus-2.4.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/tests/mock_milvus.py` & `pymilvus-2.4.3/tests/mock_milvus.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/tests/mock_result.py` & `pymilvus-2.4.3/tests/mock_result.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/tests/test_abstract.py` & `pymilvus-2.4.3/tests/test_abstract.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/tests/test_check.py` & `pymilvus-2.4.3/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/tests/test_collection.py` & `pymilvus-2.4.3/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/tests/test_connections.py` & `pymilvus-2.4.3/tests/test_connections.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/tests/test_create_collection.py` & `pymilvus-2.4.3/tests/test_create_collection.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/tests/test_decorators.py` & `pymilvus-2.4.3/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/tests/test_grpc_handler.py` & `pymilvus-2.4.3/tests/test_grpc_handler.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/tests/test_index.py` & `pymilvus-2.4.3/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/tests/test_milvus_lite.py` & `pymilvus-2.4.3/tests/test_milvus_lite.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/tests/test_partition.py` & `pymilvus-2.4.3/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/tests/test_prepare.py` & `pymilvus-2.4.3/tests/test_prepare.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/tests/test_schema.py` & `pymilvus-2.4.3/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/tests/test_ts_utils.py` & `pymilvus-2.4.3/tests/test_ts_utils.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/tests/test_types.py` & `pymilvus-2.4.3/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.2/tests/utils.py` & `pymilvus-2.4.3/tests/utils.py`

 * *Files identical despite different names*

