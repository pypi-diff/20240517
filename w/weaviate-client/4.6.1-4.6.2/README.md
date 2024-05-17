# Comparing `tmp/weaviate_client-4.6.1.tar.gz` & `tmp/weaviate_client-4.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weaviate_client-4.6.1.tar", last modified: Tue May 14 18:53:52 2024, max compression
+gzip compressed data, was "weaviate_client-4.6.2.tar", last modified: Fri May 17 20:11:04 2024, max compression
```

## Comparing `weaviate_client-4.6.1.tar` & `weaviate_client-4.6.2.tar`

### file list

```diff
@@ -1,425 +1,425 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.507894 weaviate_client-4.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.443894 weaviate_client-4.6.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.443894 weaviate_client-4.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/.github/workflows/main.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    19131 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-14 18:53:52.507894 weaviate_client-4.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.447894 weaviate_client-4.6.1/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/compose.sh
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/docker-compose-async.yml
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/docker-compose-azure.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/docker-compose-cluster.yml
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/docker-compose-generative.yml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/docker-compose-okta-cc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/docker-compose-okta-users.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/docker-compose-proxy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/docker-compose-rerank.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/docker-compose-wcs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.447894 weaviate_client-4.6.1/ci/proxy/
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/proxy/envoy.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      922 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/start_weaviate.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/stop_weaviate.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.451894 weaviate_client-4.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    56915 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.auth.rst
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.backup.rst
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.batch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.classification.rst
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.client.rst
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.cluster.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.collections.aggregations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.collections.batch.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.collections.classes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.collections.grpc.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.collections.queries.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.collections.rst
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.connect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.contextionary.rst
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.data.references.rst
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.data.replication.rst
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.gql.rst
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.proto.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.proto.v1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.rst
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.schema.properties.rst
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.schema.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.util.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.459894 weaviate_client-4.6.1/integration/
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/1234.3gp
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)   172641 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/hobbits.mp4
--rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    19306 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_batch_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    78596 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    31180 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    21235 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_batch_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    34333 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27875 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_geo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_get.py
--rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_multi_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    18946 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)    25027 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    41744 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_references.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_rerank.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_gql_raw_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21762 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_named_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/weaviate-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.459894 weaviate_client-4.6.1/integration_embedded/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_embedded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_embedded/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.459894 weaviate_client-4.6.1/integration_v3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/people_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_backup_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)    20525 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    31522 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    24351 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_grcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_stress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_timeout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.463894 weaviate_client-4.6.1/mock_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/test_automatic_retries.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/test_batching_manual.py
--rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/test_resend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.463894 weaviate_client-4.6.1/profiling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/profiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/profiling/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/profiling/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/profiling/test_import_and_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/profiling/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/profiling/test_refs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/profiling/test_sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/publishing.md
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/run-mypy.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-14 18:53:52.507894 weaviate_client-4.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.463894 weaviate_client-4.6.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.467894 weaviate_client-4.6.1/test/batch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/batch/test_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.467894 weaviate_client-4.6.1/test/classification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19246 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/classification/test_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.467894 weaviate_client-4.6.1/test/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/cluster/test_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.467894 weaviate_client-4.6.1/test/collection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/collection/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/collection/test_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/collection/test_byteops.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/collection/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/collection/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/collection/test_collection_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    37924 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/collection/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/collection/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/collection/test_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.467894 weaviate_client-4.6.1/test/connection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/connection/test_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.467894 weaviate_client-4.6.1/test/contextionary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/contextionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/contextionary/test_text2vec_contextionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.467894 weaviate_client-4.6.1/test/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.467894 weaviate_client-4.6.1/test/data/references/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/data/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/data/references/test_crud_references.py
--rw-r--r--   0 runner    (1001) docker     (127)    31268 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/data/test_crud_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.471894 weaviate_client-4.6.1/test/gql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/gql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/gql/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)    46096 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/gql/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    33189 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/gql/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/gql/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.471894 weaviate_client-4.6.1/test/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.471894 weaviate_client-4.6.1/test/schema/properties/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/schema/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/schema/properties/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/schema/schema_company.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/schema/tenants.json
--rw-r--r--   0 runner    (1001) docker     (127)    25534 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/schema/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/test_embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/test_server_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    57211 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.471894 weaviate_client-4.6.1/weaviate/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.475894 weaviate_client-4.6.1/weaviate/backup/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26299 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/backup/backup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.475894 weaviate_client-4.6.1/weaviate/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74441 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/batch/crud_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/batch/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.475894 weaviate_client-4.6.1/weaviate/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classes/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classes/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classes/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classes/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classes/generics.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classes/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classes/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classes/tenants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.475894 weaviate_client-4.6.1/weaviate/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classification/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classification/config_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    22119 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.475894 weaviate_client-4.6.1/weaviate/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/cluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/cluster/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.479894 weaviate_client-4.6.1/weaviate/collections/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/aggregate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.479894 weaviate_client-4.6.1/weaviate/collections/aggregations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/aggregations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/aggregations/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/aggregations/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/aggregations/near_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/aggregations/near_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/aggregations/near_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/aggregations/near_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/aggregations/over_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/backups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.483894 weaviate_client-4.6.1/weaviate/collections/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27776 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/batch/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/batch/batch_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/batch/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/batch/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/batch/grpc_batch_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    15748 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/batch/grpc_batch_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/batch/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.487894 weaviate_client-4.6.1/weaviate/collections/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15550 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    70969 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/config_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13424 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/config_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    41098 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/config_named_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/config_vector_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    40780 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/config_vectorizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    21511 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19528 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/orm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    12632 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27210 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.487894 weaviate_client-4.6.1/weaviate/collections/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28488 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/grpc/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/grpc/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/grpc/tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.487894 weaviate_client-4.6.1/weaviate/collections/queries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24324 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.487894 weaviate_client-4.6.1/weaviate/collections/queries/bm25/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/bm25/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/bm25/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/bm25/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/bm25/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/bm25/query.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/byteops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.487894 weaviate_client-4.6.1/weaviate/collections/queries/fetch_object_by_id/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/fetch_object_by_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/fetch_object_by_id/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/fetch_object_by_id/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.487894 weaviate_client-4.6.1/weaviate/collections/queries/fetch_objects/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/fetch_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/fetch_objects/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/fetch_objects/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/fetch_objects/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/fetch_objects/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.491894 weaviate_client-4.6.1/weaviate/collections/queries/hybrid/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/hybrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/hybrid/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12154 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/hybrid/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/hybrid/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/hybrid/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.491894 weaviate_client-4.6.1/weaviate/collections/queries/near_image/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_image/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_image/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_image/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_image/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.491894 weaviate_client-4.6.1/weaviate/collections/queries/near_media/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_media/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_media/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_media/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_media/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.491894 weaviate_client-4.6.1/weaviate/collections/queries/near_object/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_object/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10965 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_object/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_object/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_object/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.495894 weaviate_client-4.6.1/weaviate/collections/queries/near_text/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_text/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_text/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_text/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_text/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.495894 weaviate_client-4.6.1/weaviate/collections/queries/near_vector/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_vector/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_vector/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_vector/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_vector/query.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.495894 weaviate_client-4.6.1/weaviate/connect/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/connect/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/connect/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15187 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/connect/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/connect/integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)    24958 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/connect/v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    26677 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/connect/v4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.495894 weaviate_client-4.6.1/weaviate/contextionary/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/contextionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/contextionary/crud_contextionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.495894 weaviate_client-4.6.1/weaviate/data/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38789 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/data/crud_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.495894 weaviate_client-4.6.1/weaviate/data/references/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/data/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27102 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/data/references/crud_references.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.495894 weaviate_client-4.6.1/weaviate/data/replication/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/data/replication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/data/replication/replication.py
--rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/error_msgs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.499894 weaviate_client-4.6.1/weaviate/gql/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/gql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42084 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/gql/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)    36163 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/gql/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    75456 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/gql/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/gql/multi_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/gql/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.499894 weaviate_client-4.6.1/weaviate/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/outputs/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/outputs/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/outputs/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/outputs/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/outputs/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/outputs/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/outputs/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/outputs/tenants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.499894 weaviate_client-4.6.1/weaviate/proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.503894 weaviate_client-4.6.1/weaviate/proto/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/base_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/base_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/base_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/batch_delete_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/batch_delete_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/batch_delete_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/batch_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/batch_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/batch_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/properties_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/properties_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/properties_pb2_grpc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      391 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/regen.sh
--rw-r--r--   0 runner    (1001) docker     (127)    18051 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/search_get_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    29649 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/search_get_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/search_get_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/tenants_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/tenants_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/tenants_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/weaviate_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/weaviate_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/weaviate_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.503894 weaviate_client-4.6.1/weaviate/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34232 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/schema/crud_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.503894 weaviate_client-4.6.1/weaviate/schema/properties/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/schema/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/schema/properties/crud_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28584 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11919 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.507894 weaviate_client-4.6.1/weaviate_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-14 18:53:52.000000 weaviate_client-4.6.1/weaviate_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-14 18:53:52.000000 weaviate_client-4.6.1/weaviate_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:53:52.000000 weaviate_client-4.6.1/weaviate_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:53:52.000000 weaviate_client-4.6.1/weaviate_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-14 18:53:52.000000 weaviate_client-4.6.1/weaviate_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 18:53:52.000000 weaviate_client-4.6.1/weaviate_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.783228 weaviate_client-4.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.727228 weaviate_client-4.6.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.727228 weaviate_client-4.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    19131 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-17 20:11:04.783228 weaviate_client-4.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.731228 weaviate_client-4.6.2/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/ci/compose.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/ci/docker-compose-async.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/ci/docker-compose-azure.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/ci/docker-compose-cluster.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/ci/docker-compose-generative.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/ci/docker-compose-okta-cc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/ci/docker-compose-okta-users.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/ci/docker-compose-proxy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/ci/docker-compose-rerank.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/ci/docker-compose-wcs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/ci/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.731228 weaviate_client-4.6.2/ci/proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/ci/proxy/envoy.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      922 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/ci/start_weaviate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/ci/stop_weaviate.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.735228 weaviate_client-4.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    57214 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.auth.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.backup.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.batch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.classification.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.client.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.cluster.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.collections.aggregations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.collections.batch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.collections.classes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.collections.grpc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.collections.queries.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.collections.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.connect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.contextionary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.data.references.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.data.replication.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.gql.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.proto.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.proto.v1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.schema.properties.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/docs/weaviate.util.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.739228 weaviate_client-4.6.2/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/1234.3gp
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)   172641 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/hobbits.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19365 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_batch_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17338 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78596 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31180 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_collection_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_collection_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21235 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_collection_batch_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34388 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_collection_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27875 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_collection_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_collection_geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_collection_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_collection_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_collection_multi_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18946 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_collection_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25135 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_collection_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41744 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_collection_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_collection_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_gql_raw_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21762 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_named_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/test_tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration/weaviate-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.739228 weaviate_client-4.6.2/integration_embedded/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration_embedded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration_embedded/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.743228 weaviate_client-4.6.2/integration_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration_v3/people_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration_v3/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration_v3/test_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration_v3/test_backup_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20525 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration_v3/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration_v3/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration_v3/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31522 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration_v3/test_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24351 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration_v3/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration_v3/test_grcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration_v3/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration_v3/test_stress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/integration_v3/test_timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.743228 weaviate_client-4.6.2/mock_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/mock_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/mock_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/mock_tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/mock_tests/test_automatic_retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/mock_tests/test_batching_manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/mock_tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/mock_tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/mock_tests/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/mock_tests/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/mock_tests/test_resend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/mock_tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.743228 weaviate_client-4.6.2/profiling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/profiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/profiling/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/profiling/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/profiling/test_import_and_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/profiling/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/profiling/test_refs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/profiling/test_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/publishing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/run-mypy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-17 20:11:04.783228 weaviate_client-4.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.747228 weaviate_client-4.6.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.747228 weaviate_client-4.6.2/test/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/batch/test_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.747228 weaviate_client-4.6.2/test/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19246 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/classification/test_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.747228 weaviate_client-4.6.2/test/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/cluster/test_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.747228 weaviate_client-4.6.2/test/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/collection/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/collection/test_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/collection/test_byteops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/collection/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/collection/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/collection/test_collection_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37924 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/collection/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/collection/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/collection/test_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.747228 weaviate_client-4.6.2/test/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/connection/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.747228 weaviate_client-4.6.2/test/contextionary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/contextionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/contextionary/test_text2vec_contextionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.747228 weaviate_client-4.6.2/test/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.747228 weaviate_client-4.6.2/test/data/references/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/data/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/data/references/test_crud_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31268 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/data/test_crud_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.751228 weaviate_client-4.6.2/test/gql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/gql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/gql/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46096 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/gql/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33189 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/gql/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/gql/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.751228 weaviate_client-4.6.2/test/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.751228 weaviate_client-4.6.2/test/schema/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/schema/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/schema/properties/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/schema/schema_company.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/schema/tenants.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25534 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/schema/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/test_embedded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/test_server_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57211 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/test/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.751228 weaviate_client-4.6.2/weaviate/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.751228 weaviate_client-4.6.2/weaviate/backup/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26299 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/backup/backup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.755228 weaviate_client-4.6.2/weaviate/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74441 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/batch/crud_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/batch/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.755228 weaviate_client-4.6.2/weaviate/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/classes/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/classes/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/classes/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/classes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/classes/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/classes/generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/classes/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/classes/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/classes/tenants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.755228 weaviate_client-4.6.2/weaviate/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/classification/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/classification/config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22104 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.755228 weaviate_client-4.6.2/weaviate/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/cluster/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/cluster/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.759228 weaviate_client-4.6.2/weaviate/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/aggregate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.759228 weaviate_client-4.6.2/weaviate/collections/aggregations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/aggregations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/aggregations/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/aggregations/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/aggregations/near_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/aggregations/near_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/aggregations/near_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/aggregations/near_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/aggregations/over_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/backups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.759228 weaviate_client-4.6.2/weaviate/collections/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27776 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/batch/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/batch/batch_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/batch/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/batch/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/batch/grpc_batch_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15748 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/batch/grpc_batch_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/batch/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.763228 weaviate_client-4.6.2/weaviate/collections/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15550 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/classes/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/classes/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/classes/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70969 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/classes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/classes/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13424 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/classes/config_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41098 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/classes/config_named_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/classes/config_vector_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40850 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/classes/config_vectorizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/classes/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21511 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/classes/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/classes/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19528 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/classes/internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/classes/orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/classes/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/classes/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15295 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12632 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27210 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.763228 weaviate_client-4.6.2/weaviate/collections/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28488 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/grpc/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/grpc/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/grpc/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.763228 weaviate_client-4.6.2/weaviate/collections/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24324 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.763228 weaviate_client-4.6.2/weaviate/collections/queries/bm25/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/bm25/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/bm25/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/bm25/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/bm25/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/bm25/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/byteops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.767228 weaviate_client-4.6.2/weaviate/collections/queries/fetch_object_by_id/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/fetch_object_by_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/fetch_object_by_id/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/fetch_object_by_id/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.767228 weaviate_client-4.6.2/weaviate/collections/queries/fetch_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/fetch_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/fetch_objects/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/fetch_objects/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/fetch_objects/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/fetch_objects/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.767228 weaviate_client-4.6.2/weaviate/collections/queries/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/hybrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/hybrid/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12154 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/hybrid/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/hybrid/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/hybrid/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.767228 weaviate_client-4.6.2/weaviate/collections/queries/near_image/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_image/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_image/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_image/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_image/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.767228 weaviate_client-4.6.2/weaviate/collections/queries/near_media/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_media/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_media/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_media/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_media/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.771228 weaviate_client-4.6.2/weaviate/collections/queries/near_object/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_object/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10965 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_object/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_object/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_object/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.771228 weaviate_client-4.6.2/weaviate/collections/queries/near_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_text/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_text/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_text/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_text/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.771228 weaviate_client-4.6.2/weaviate/collections/queries/near_vector/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_vector/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_vector/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_vector/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/queries/near_vector/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/collections/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.771228 weaviate_client-4.6.2/weaviate/connect/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/connect/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/connect/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/connect/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/connect/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24991 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/connect/v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28105 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/connect/v4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.771228 weaviate_client-4.6.2/weaviate/contextionary/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/contextionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/contextionary/crud_contextionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.771228 weaviate_client-4.6.2/weaviate/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38789 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/data/crud_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.775228 weaviate_client-4.6.2/weaviate/data/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/data/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27102 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/data/references/crud_references.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.775228 weaviate_client-4.6.2/weaviate/data/replication/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/data/replication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/data/replication/replication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12458 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/embedded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/error_msgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.775228 weaviate_client-4.6.2/weaviate/gql/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/gql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42084 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/gql/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36163 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/gql/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75456 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/gql/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/gql/multi_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/gql/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.775228 weaviate_client-4.6.2/weaviate/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/outputs/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/outputs/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/outputs/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/outputs/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/outputs/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/outputs/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/outputs/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/outputs/tenants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.775228 weaviate_client-4.6.2/weaviate/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.779228 weaviate_client-4.6.2/weaviate/proto/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/base_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/base_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/base_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/batch_delete_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/batch_delete_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/batch_delete_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/batch_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/batch_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/batch_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/properties_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/properties_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/properties_pb2_grpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      391 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/regen.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    18051 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/search_get_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29649 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/search_get_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/search_get_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/tenants_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/tenants_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/tenants_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/weaviate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/weaviate_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/proto/v1/weaviate_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.779228 weaviate_client-4.6.2/weaviate/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34232 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/schema/crud_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.779228 weaviate_client-4.6.2/weaviate/schema/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/schema/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/schema/properties/crud_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28584 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11696 2024-05-17 20:10:42.000000 weaviate_client-4.6.2/weaviate/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:11:04.783228 weaviate_client-4.6.2/weaviate_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-17 20:11:04.000000 weaviate_client-4.6.2/weaviate_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-17 20:11:04.000000 weaviate_client-4.6.2/weaviate_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 20:11:04.000000 weaviate_client-4.6.2/weaviate_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 20:11:04.000000 weaviate_client-4.6.2/weaviate_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-17 20:11:04.000000 weaviate_client-4.6.2/weaviate_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 20:11:04.000000 weaviate_client-4.6.2/weaviate_client.egg-info/top_level.txt
```

### Comparing `weaviate_client-4.6.1/.flake8` & `weaviate_client-4.6.2/.flake8`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/.github/workflows/main.yaml` & `weaviate_client-4.6.2/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/.pre-commit-config.yaml` & `weaviate_client-4.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/.pylintrc` & `weaviate_client-4.6.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/CONTRIBUTING.md` & `weaviate_client-4.6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/LICENSE` & `weaviate_client-4.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/PKG-INFO` & `weaviate_client-4.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weaviate-client
-Version: 4.6.1
+Version: 4.6.2
 Summary: A python native Weaviate client
 Home-page: https://github.com/weaviate/weaviate-python-client
 Author: Weaviate
 Author-email: hello@weaviate.io,
 License: BSD 3-clause
 Project-URL: Documentation, https://weaviate-python-client.readthedocs.io
 Project-URL: Source, https://github.com/weaviate/weaviate-python-client
```

### Comparing `weaviate_client-4.6.1/README.rst` & `weaviate_client-4.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/ci/docker-compose-async.yml` & `weaviate_client-4.6.2/ci/docker-compose-async.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/ci/docker-compose-azure.yml` & `weaviate_client-4.6.2/ci/docker-compose-azure.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/ci/docker-compose-cluster.yml` & `weaviate_client-4.6.2/ci/docker-compose-cluster.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/ci/docker-compose-generative.yml` & `weaviate_client-4.6.2/ci/docker-compose-generative.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/ci/docker-compose-okta-cc.yml` & `weaviate_client-4.6.2/ci/docker-compose-okta-cc.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/ci/docker-compose-okta-users.yml` & `weaviate_client-4.6.2/ci/docker-compose-okta-users.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/ci/docker-compose-proxy.yml` & `weaviate_client-4.6.2/ci/docker-compose-proxy.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/ci/docker-compose-rerank.yml` & `weaviate_client-4.6.2/ci/docker-compose-rerank.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/ci/docker-compose-wcs.yml` & `weaviate_client-4.6.2/ci/docker-compose-wcs.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/ci/docker-compose.yml` & `weaviate_client-4.6.2/ci/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/ci/proxy/envoy.yaml` & `weaviate_client-4.6.2/ci/proxy/envoy.yaml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/ci/start_weaviate.sh` & `weaviate_client-4.6.2/ci/start_weaviate.sh`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/docs/Makefile` & `weaviate_client-4.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/docs/README.rst` & `weaviate_client-4.6.2/docs/README.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/docs/changelog.rst` & `weaviate_client-4.6.2/docs/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+Version 4.6.2
+--------------
+This patch version includes:
+  - Respect default vectorizer
+  - Wait for Weaviate 1.25 to be ready before starting the embedded client
+  - Add missing models for voyageai
+  - Rename WCS to Weaviate Cloud and add new helper function `weaviate.connect_to_weaviate_cloud`
+
 Version 4.6.1
 --------------
 This patch version includes:
   - Fixes for ``client.integrations.configure``
 
 Version 4.6.0
 --------------
```

### Comparing `weaviate_client-4.6.1/docs/conf.py` & `weaviate_client-4.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/docs/index.rst` & `weaviate_client-4.6.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/docs/make.bat` & `weaviate_client-4.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/docs/weaviate.classification.rst` & `weaviate_client-4.6.2/docs/weaviate.classification.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/docs/weaviate.collections.aggregations.rst` & `weaviate_client-4.6.2/docs/weaviate.collections.aggregations.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/docs/weaviate.collections.batch.rst` & `weaviate_client-4.6.2/docs/weaviate.collections.batch.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/docs/weaviate.collections.classes.rst` & `weaviate_client-4.6.2/docs/weaviate.collections.classes.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/docs/weaviate.collections.grpc.rst` & `weaviate_client-4.6.2/docs/weaviate.collections.grpc.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/docs/weaviate.collections.queries.rst` & `weaviate_client-4.6.2/docs/weaviate.collections.queries.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/docs/weaviate.collections.rst` & `weaviate_client-4.6.2/docs/weaviate.collections.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/docs/weaviate.connect.rst` & `weaviate_client-4.6.2/docs/weaviate.connect.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/docs/weaviate.gql.rst` & `weaviate_client-4.6.2/docs/weaviate.gql.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/docs/weaviate.proto.v1.rst` & `weaviate_client-4.6.2/docs/weaviate.proto.v1.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/docs/weaviate.rst` & `weaviate_client-4.6.2/docs/weaviate.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration/1234.3gp` & `weaviate_client-4.6.2/integration/1234.3gp`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration/conftest.py` & `weaviate_client-4.6.2/integration/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             additional_config=AdditionalConfig(timeout=(60, 120)),  # for image tests
         )
         client_fixture.collections.delete(name_fixture)
 
         collection: Collection[Any, Any] = client_fixture.collections.create(
             name=name_fixture,
             description=description,
-            vectorizer_config=vectorizer_config,
+            vectorizer_config=vectorizer_config or Configure.Vectorizer.none(),
             properties=properties,
             references=references,
             inverted_index_config=inverted_index_config,
             multi_tenancy_config=multi_tenancy_config,
             generative_config=generative_config,
             data_model_properties=data_model_properties,
             data_model_references=data_model_refs,
@@ -140,15 +140,15 @@
             pytest.skip("No OpenAI API key found.")
 
         if vectorizer_config is None:
             vectorizer_config = Configure.Vectorizer.none()
 
         collection = collection_factory(
             name=name,
-            vectorizer_config=vectorizer_config,
+            vectorizer_config=vectorizer_config or Configure.Vectorizer.none(),
             properties=[
                 Property(name="text", data_type=DataType.TEXT),
                 Property(name="content", data_type=DataType.TEXT),
                 Property(name="extra", data_type=DataType.TEXT),
             ],
             generative_config=Configure.Generative.openai(),
             ports=(8086, 50057),
```

### Comparing `weaviate_client-4.6.1/integration/constants.py` & `weaviate_client-4.6.2/integration/constants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration/hobbits.mp4` & `weaviate_client-4.6.2/integration/hobbits.mp4`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration/test_auth.py` & `weaviate_client-4.6.2/integration/test_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pytest
 from _pytest.fixtures import SubRequest
 
 import weaviate
 import weaviate.classes as wvc
 from integration.conftest import _sanitize_collection_name
 from weaviate import util
-from weaviate.collections.classes.config import DataType, Property
+from weaviate.collections.classes.config import Configure, DataType, Property
 from weaviate.collections.classes.filters import Filter
 from weaviate.exceptions import AuthenticationFailedError, UnexpectedStatusCodeError
 
 ANON_PORT = 8080
 AZURE_PORT = 8081
 OKTA_PORT_CC = 8082
 OKTA_PORT_USERS = 8083
@@ -261,14 +261,15 @@
         client.collections.delete(name)
         col = client.collections.create(
             name=name,
             description="test",
             properties=[
                 Property(name="name", data_type=DataType.TEXT),
             ],
+            vectorizer_config=Configure.Vectorizer.none(),
         )
         col.data.insert({"name": "test"})
         col.data.insert_many([{"name": "test2"}])
         assert len(col.query.fetch_objects().objects) == 2
 
         col.data.delete_many(Filter.by_property("name").equal("test"))
         assert len(col.query.fetch_objects().objects) == 1
```

### Comparing `weaviate_client-4.6.1/integration/test_batch_v4.py` & `weaviate_client-4.6.2/integration/test_batch_v4.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
             name=name_fixture,
             properties=[
                 Property(name="name", data_type=DataType.TEXT),
                 Property(name="age", data_type=DataType.INT),
             ],
             references=[ReferenceProperty(name="test", target_collection=name_fixture)],
             multi_tenancy_config=Configure.multi_tenancy(multi_tenant),
+            vectorizer_config=Configure.Vectorizer.none(),
         )
         return client_fixture, name_fixture
 
     yield _factory
     if client_fixture is not None and name_fixture is not None:
         client_fixture.collections.delete(name_fixture)
```

### Comparing `weaviate_client-4.6.1/integration/test_client.py` & `weaviate_client-4.6.2/integration/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     client.get_meta()
 
 
 def test_create_get_and_delete(client: weaviate.WeaviateClient, request: SubRequest) -> None:
     name = request.node.name
     client.collections.delete(name)
 
-    col = client.collections.create(name=name)
+    col = client.collections.create(name=name, vectorizer_config=Configure.Vectorizer.none())
     assert client.collections.exists(name)
     assert isinstance(col, Collection)
 
     col = client.collections.get(name)
     assert isinstance(col, Collection)
 
     client.collections.delete(name)
@@ -320,15 +320,17 @@
     client.collections.delete(name_small)
     assert not client.collections.exists(name_small)
     assert not client.collections.exists(name_big)
 
 
 def test_client_cluster(client: weaviate.WeaviateClient, request: SubRequest) -> None:
     client.collections.delete(request.node.name)
-    collection = client.collections.create(name=request.node.name)
+    collection = client.collections.create(
+        name=request.node.name, vectorizer_config=Configure.Vectorizer.none()
+    )
 
     nodes = client.cluster.nodes(collection.name, output="verbose")
     assert len(nodes) == 1
     assert len(nodes[0].shards) == 1
     assert nodes[0].shards[0].collection == collection.name
     assert nodes[0].shards[0].object_count == 0
     assert nodes[0].shards[0].vector_indexing_status == "READY"
@@ -341,24 +343,27 @@
 
 
 def test_client_cluster_multitenant(client: weaviate.WeaviateClient, request: SubRequest) -> None:
     client.collections.delete(request.node.name)
     collection = client.collections.create(
         name=request.node.name,
         multi_tenancy_config=Configure.multi_tenancy(enabled=True),
+        vectorizer_config=Configure.Vectorizer.none(),
     )
 
     nodes = client.cluster.nodes(collection.name, output="verbose")
     assert len(nodes) == 1
     assert len(nodes[0].shards) == 0
 
 
 def test_client_cluster_minimal(client: weaviate.WeaviateClient, request: SubRequest) -> None:
     client.collections.delete(request.node.name)
-    collection = client.collections.create(name=request.node.name)
+    collection = client.collections.create(
+        name=request.node.name, vectorizer_config=Configure.Vectorizer.none()
+    )
 
     nodes = client.cluster.nodes(collection.name, output="minimal")
     assert len(nodes) == 1
     assert nodes[0].shards is None
 
 
 def test_client_connect_and_close() -> None:
@@ -456,14 +461,17 @@
 def test_client_with_extra_options(timeout: Union[Tuple[int, int], Timeout]) -> None:
     additional_config = wvc.init.AdditionalConfig(timeout=timeout, trust_env=True)
 
     for client in [
         weaviate.connect_to_wcs(
             cluster_url=WCS_URL, auth_credentials=WCS_CREDS, additional_config=additional_config
         ),
+        weaviate.connect_to_weaviate_cloud(
+            cluster_url=WCS_URL, auth_credentials=WCS_CREDS, additional_config=additional_config
+        ),
         weaviate.connect_to_local(additional_config=additional_config),
         weaviate.connect_to_custom(
             http_secure=True,
             http_host=WCS_HOST,
             http_port=443,
             grpc_secure=True,
             grpc_host=WCS_GRPC_HOST,
@@ -505,10 +513,11 @@
             )
         )
     ) as client:
         client.collections.delete("TestLocalProxies")
         collection = client.collections.create(
             "TestLocalProxies",
             properties=[wvc.config.Property(name="name", data_type=wvc.config.DataType.TEXT)],
+            vectorizer_config=Configure.Vectorizer.none(),
         )
         collection.data.insert({"name": "Test"})
         assert collection.query.fetch_objects().objects[0].properties["name"] == "Test"
```

### Comparing `weaviate_client-4.6.1/integration/test_collection.py` & `weaviate_client-4.6.2/integration/test_collection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration/test_collection_aggregate.py` & `weaviate_client-4.6.2/integration/test_collection_aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration/test_collection_batch.py` & `weaviate_client-4.6.2/integration/test_collection_batch.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration/test_collection_batch_delete.py` & `weaviate_client-4.6.2/integration/test_collection_batch_delete.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration/test_collection_config.py` & `weaviate_client-4.6.2/integration/test_collection_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -617,14 +617,15 @@
     expected_reranker: Rerankers,
     expected_model: dict,
 ) -> None:
     client.collections.delete("TestCollectionConfigRerankerModule")
     collection = client.collections.create(
         name="TestCollectionConfigRerankerModule",
         reranker_config=reranker_config,
+        vectorizer_config=Configure.Vectorizer.none(),
     )
     conf = collection.config.get()
     assert conf.reranker_config is not None
     assert conf.reranker_config.reranker == expected_reranker
     assert conf.reranker_config.model == expected_model
```

### Comparing `weaviate_client-4.6.1/integration/test_collection_filter.py` & `weaviate_client-4.6.2/integration/test_collection_filter.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration/test_collection_geo.py` & `weaviate_client-4.6.2/integration/test_collection_geo.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration/test_collection_get.py` & `weaviate_client-4.6.2/integration/test_collection_get.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration/test_collection_model.py` & `weaviate_client-4.6.2/integration/test_collection_model.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration/test_collection_multi_node.py` & `weaviate_client-4.6.2/integration/test_collection_multi_node.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration/test_collection_nested.py` & `weaviate_client-4.6.2/integration/test_collection_nested.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration/test_collection_openai.py` & `weaviate_client-4.6.2/integration/test_collection_openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -521,40 +521,42 @@
     )
     assert res.generated == "apples bananas"
     assert len(res.groups) == 2
     assert list(res.groups.values())[0].generated == "Yes"
     assert list(res.groups.values())[1].generated == "No"
 
 
-def test_openapi_invalid_key(request: SubRequest) -> None:
+def test_openai_invalid_key(request: SubRequest) -> None:
     local_client = weaviate.connect_to_local(
         port=8086, grpc_port=50057, headers={"X-OpenAI-Api-Key": "IamNotValid"}
     )
 
     local_client.collections.delete(request.node.name)
     collection = local_client.collections.create(
         name=request.node.name,
         properties=[Property(name="text", data_type=DataType.TEXT)],
         generative_config=Configure.Generative.openai(),
+        vectorizer_config=Configure.Vectorizer.none(),
     )
     collection.data.insert(properties={"text": "test"})
     with pytest.raises(WeaviateQueryError):
         collection.generate.fetch_objects(single_prompt="tell a joke based on {text}")
 
 
-def test_openapi_no_module(request: SubRequest) -> None:
+def test_openai_no_module(request: SubRequest) -> None:
     local_client = weaviate.connect_to_local(
         port=8080, grpc_port=50051, headers={"X-OpenAI-Api-Key": "doesnt matter"}
     )
 
     local_client.collections.delete(request.node.name)
     collection = local_client.collections.create(
         name=request.node.name,
         properties=[Property(name="text", data_type=DataType.TEXT)],
         generative_config=Configure.Generative.openai(),
+        vectorizer_config=Configure.Vectorizer.none(),
     )
     collection.data.insert(properties={"text": "test"})
     with pytest.raises(WeaviateQueryError):
         collection.generate.fetch_objects(single_prompt="tell a joke based on {text}")
 
 
 def test_openai_batch_upload(openai_collection: OpenAICollection, request: SubRequest) -> None:
```

### Comparing `weaviate_client-4.6.1/integration/test_collection_references.py` & `weaviate_client-4.6.2/integration/test_collection_references.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration/test_collection_rerank.py` & `weaviate_client-4.6.2/integration/test_collection_rerank.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration/test_gql_raw_v4.py` & `weaviate_client-4.6.2/integration/test_gql_raw_v4.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration/test_iterator.py` & `weaviate_client-4.6.2/integration/test_iterator.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration/test_named_vectors.py` & `weaviate_client-4.6.2/integration/test_named_vectors.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration/test_tenants.py` & `weaviate_client-4.6.2/integration/test_tenants.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
     uuid = tenant1.data.insert(properties={"name": "some name"})
     tenant1.data.replace(properties={"name": "other name"}, uuid=uuid)
     assert tenant1.query.fetch_object_by_id(uuid).properties["name"] == "other name"
     assert tenant2.query.fetch_object_by_id(uuid) is None
 
 
-def test_update(collection_factory: CollectionFactory) -> None:
+def test_tenants_update(collection_factory: CollectionFactory) -> None:
     collection = collection_factory(
         properties=[Property(name="Name", data_type=DataType.TEXT)],
         vectorizer_config=Configure.Vectorizer.none(),
     )
     uuid = collection.data.insert(properties={"name": "some name"})
     collection.data.update(properties={"name": "other name"}, uuid=uuid, vector=[1, 2, 3])
     obj = collection.query.fetch_object_by_id(uuid, include_vector=True)
```

### Comparing `weaviate_client-4.6.1/integration/weaviate-logo.png` & `weaviate_client-4.6.2/integration/weaviate-logo.png`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration_embedded/test_client.py` & `weaviate_client-4.6.2/integration_embedded/test_client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration_v3/people_schema.json` & `weaviate_client-4.6.2/integration_v3/people_schema.json`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration_v3/test_authentication.py` & `weaviate_client-4.6.2/integration_v3/test_authentication.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration_v3/test_backup.py` & `weaviate_client-4.6.2/integration_v3/test_backup.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration_v3/test_backup_v4.py` & `weaviate_client-4.6.2/integration_v3/test_backup_v4.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration_v3/test_batch.py` & `weaviate_client-4.6.2/integration_v3/test_batch.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration_v3/test_classification.py` & `weaviate_client-4.6.2/integration_v3/test_classification.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration_v3/test_cluster.py` & `weaviate_client-4.6.2/integration_v3/test_cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration_v3/test_crud.py` & `weaviate_client-4.6.2/integration_v3/test_crud.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration_v3/test_graphql.py` & `weaviate_client-4.6.2/integration_v3/test_graphql.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration_v3/test_grcp.py` & `weaviate_client-4.6.2/integration_v3/test_grcp.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration_v3/test_schema.py` & `weaviate_client-4.6.2/integration_v3/test_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration_v3/test_stress.py` & `weaviate_client-4.6.2/integration_v3/test_stress.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/integration_v3/test_timeout.py` & `weaviate_client-4.6.2/integration_v3/test_timeout.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/mock_tests/conftest.py` & `weaviate_client-4.6.2/mock_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/mock_tests/test_auth.py` & `weaviate_client-4.6.2/mock_tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/mock_tests/test_automatic_retries.py` & `weaviate_client-4.6.2/mock_tests/test_automatic_retries.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/mock_tests/test_batching_manual.py` & `weaviate_client-4.6.2/mock_tests/test_batching_manual.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/mock_tests/test_collection.py` & `weaviate_client-4.6.2/mock_tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/mock_tests/test_connection.py` & `weaviate_client-4.6.2/mock_tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/mock_tests/test_exception.py` & `weaviate_client-4.6.2/mock_tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/mock_tests/test_graphql.py` & `weaviate_client-4.6.2/mock_tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/mock_tests/test_resend.py` & `weaviate_client-4.6.2/mock_tests/test_resend.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/mock_tests/test_schema.py` & `weaviate_client-4.6.2/mock_tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/profiling/conftest.py` & `weaviate_client-4.6.2/profiling/conftest.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/profiling/constants.py` & `weaviate_client-4.6.2/profiling/constants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/profiling/test_import_and_query.py` & `weaviate_client-4.6.2/profiling/test_import_and_query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/profiling/test_profiling.py` & `weaviate_client-4.6.2/profiling/test_profiling.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/profiling/test_refs.py` & `weaviate_client-4.6.2/profiling/test_refs.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/profiling/test_sphere.py` & `weaviate_client-4.6.2/profiling/test_sphere.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/publishing.md` & `weaviate_client-4.6.2/publishing.md`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/pyproject.toml` & `weaviate_client-4.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/requirements-devel.txt` & `weaviate_client-4.6.2/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/setup.cfg` & `weaviate_client-4.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/README.md` & `weaviate_client-4.6.2/test/README.md`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/batch/test_requests.py` & `weaviate_client-4.6.2/test/batch/test_requests.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/classification/test_classification.py` & `weaviate_client-4.6.2/test/classification/test_classification.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/cluster/test_cluster.py` & `weaviate_client-4.6.2/test/cluster/test_cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/collection/test_aggregates.py` & `weaviate_client-4.6.2/test/collection/test_aggregates.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/collection/test_byteops.py` & `weaviate_client-4.6.2/test/collection/test_byteops.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/collection/test_classes.py` & `weaviate_client-4.6.2/test/collection/test_classes.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/collection/test_client.py` & `weaviate_client-4.6.2/test/collection/test_client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/collection/test_collection_model.py` & `weaviate_client-4.6.2/test/collection/test_collection_model.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/collection/test_config.py` & `weaviate_client-4.6.2/test/collection/test_config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/collection/test_filter.py` & `weaviate_client-4.6.2/test/collection/test_filter.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/collection/test_queries.py` & `weaviate_client-4.6.2/test/collection/test_queries.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/connection/test_connection.py` & `weaviate_client-4.6.2/test/connection/test_connection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/contextionary/test_text2vec_contextionary.py` & `weaviate_client-4.6.2/test/contextionary/test_text2vec_contextionary.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/data/references/test_crud_references.py` & `weaviate_client-4.6.2/test/data/references/test_crud_references.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/data/test_crud_data.py` & `weaviate_client-4.6.2/test/data/test_crud_data.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/gql/test_aggregate.py` & `weaviate_client-4.6.2/test/gql/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/gql/test_filter.py` & `weaviate_client-4.6.2/test/gql/test_filter.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/gql/test_get.py` & `weaviate_client-4.6.2/test/gql/test_get.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/gql/test_query.py` & `weaviate_client-4.6.2/test/gql/test_query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/schema/properties/test_properties.py` & `weaviate_client-4.6.2/test/schema/properties/test_properties.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/schema/schema_company.json` & `weaviate_client-4.6.2/test/schema/schema_company.json`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/schema/test_schema.py` & `weaviate_client-4.6.2/test/schema/test_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/test_auth.py` & `weaviate_client-4.6.2/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/test_client.py` & `weaviate_client-4.6.2/test/test_client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/test_embedded.py` & `weaviate_client-4.6.2/test/test_embedded.py`

 * *Files 11% similar despite different names*

```diff
@@ -102,38 +102,40 @@
     )
 
 
 @pytest.mark.parametrize(
     "options", [EmbeddedOptions(), EmbeddedOptions(port=30666, grpc_port=50046)]
 )
 def test_embedded_end_to_end(options: EmbeddedDB, tmp_path):
-    options.binary_path = tmp_path
-    options.persistence_data_path = tmp_path
-    embedded_db = EmbeddedDB(options=options)
-    assert embedded_db.is_listening() is False
-    with pytest.raises(WeaviateStartUpError):
-        with patch("time.sleep") as mocked_sleep:
-            embedded_db.wait_till_listening()
-            mocked_sleep.assert_has_calls([0.1] * 300)
-
-    embedded_db.ensure_running()
-    assert embedded_db.is_listening() is True
-    with patch("builtins.print") as mocked_print:
-        embedded_db.start()
-        mocked_print.assert_called_once_with(
-            f"embedded weaviate is already listening on port {options.port}"
-        )
-
-    # killing the process should restart it again when ensure running is called
-    os.kill(embedded_db.process.pid, signal.SIGTERM)
-    time.sleep(0.2)
-    assert embedded_db.is_listening() is False
-    embedded_db.ensure_running()
-    assert embedded_db.is_listening() is True
-    embedded_db.stop()
+    try:
+        options.binary_path = tmp_path
+        options.persistence_data_path = tmp_path
+        embedded_db = EmbeddedDB(options=options)
+        assert embedded_db.is_listening() is False
+        with pytest.raises(WeaviateStartUpError):
+            with patch("time.sleep") as mocked_sleep:
+                embedded_db.wait_till_listening()
+                mocked_sleep.assert_has_calls([0.1] * 300)
+
+        embedded_db.ensure_running()
+        assert embedded_db.is_listening() is True
+        with patch("builtins.print") as mocked_print:
+            embedded_db.start()
+            mocked_print.assert_called_once_with(
+                f"embedded weaviate is already listening on port {options.port}"
+            )
+
+        # killing the process should restart it again when ensure running is called
+        os.kill(embedded_db.process.pid, signal.SIGTERM)
+        time.sleep(0.2)
+        assert embedded_db.is_listening() is False
+        embedded_db.ensure_running()
+        assert embedded_db.is_listening() is True
+    finally:
+        embedded_db.stop()
 
 
 def test_embedded_multiple_instances(tmp_path_factory: pytest.TempPathFactory):
     embedded_db = EmbeddedDB(
         EmbeddedOptions(
             port=30662,
             persistence_data_path=tmp_path_factory.mktemp("data"),
@@ -147,18 +149,22 @@
             port=30663,
             persistence_data_path=tmp_path_factory.mktemp("data"),
             binary_path=tmp_path_factory.mktemp("bin"),
             additional_env_vars={"GRPC_PORT": "50054"},
             grpc_port=50054,
         )
     )
-    embedded_db.ensure_running()
-    assert embedded_db.is_listening() is True
-    embedded_db2.ensure_running()
-    assert embedded_db2.is_listening() is True
+    try:
+        embedded_db.ensure_running()
+        assert embedded_db.is_listening() is True
+        embedded_db2.ensure_running()
+        assert embedded_db2.is_listening() is True
+    finally:
+        embedded_db.stop()
+        embedded_db2.stop()
 
 
 def test_embedded_different_versions(tmp_path_factory: pytest.TempPathFactory):
     client1 = weaviate.Client(
         embedded_options=EmbeddedOptions(
             port=30664,
             persistence_data_path=tmp_path_factory.mktemp("data"),
@@ -170,31 +176,38 @@
         embedded_options=EmbeddedOptions(
             port=30665,
             persistence_data_path=tmp_path_factory.mktemp("data"),
             binary_path=tmp_path_factory.mktemp("bin"),
             version="https://github.com/weaviate/weaviate/releases/download/v1.18.0/weaviate-v1.18.0-linux-amd64.tar.gz",
         )
     )
-    meta1 = client1.get_meta()
-    assert meta1["version"] == "1.18.1"
-    meta2 = client2.get_meta()
-    assert meta2["version"] == "1.18.0"
+    try:
+        meta1 = client1.get_meta()
+        assert meta1["version"] == "1.18.1"
+        meta2 = client2.get_meta()
+        assert meta2["version"] == "1.18.0"
+    finally:
+        client1._connection.embedded_db.stop()
+        client2._connection.embedded_db.stop()
 
 
 def test_custom_env_vars(tmp_path_factory: pytest.TempPathFactory):
     client = weaviate.Client(
         embedded_options=EmbeddedOptions(
             binary_path=tmp_path_factory.mktemp("bin"),
             additional_env_vars={"ENABLE_MODULES": "", "GRPC_PORT": "50057"},
             persistence_data_path=tmp_path_factory.mktemp("data"),
             port=30666,
         )
     )
-    meta = client.get_meta()
-    assert len(meta["modules"]) == 0
+    try:
+        meta = client.get_meta()
+        assert len(meta["modules"]) == 0
+    finally:
+        client._connection.embedded_db.stop()
 
 
 def test_weaviate_state(tmp_path_factory: pytest.TempPathFactory) -> None:
     """Test that weaviate keeps the state between different runs."""
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     port = 36545
     data_path = tmp_path_factory.mktemp("data")
@@ -224,42 +237,52 @@
             additional_env_vars={"GRPC_PORT": "50059"},
             grpc_port=50059,
         )
     )
     count = client.query.aggregate("Person").with_meta_count().do()
     assert count["data"]["Aggregate"]["Person"][0]["meta"]["count"] == 1
 
+    client._connection.embedded_db.stop()
+
 
 def test_version(tmp_path_factory: pytest.TempPathFactory):
     client = weaviate.Client(
         embedded_options=EmbeddedOptions(
             persistence_data_path=tmp_path_factory.mktemp("data"),
             binary_path=tmp_path_factory.mktemp("bin"),
             version="1.18.2",
             port=30667,
         )
     )
-    meta = client.get_meta()
-    assert meta["version"] == "1.18.2"
+    try:
+        meta = client.get_meta()
+        assert meta["version"] == "1.18.2"
+    finally:
+        client._connection.embedded_db.stop()
 
 
 def test_latest(tmp_path_factory: pytest.TempPathFactory):
     client = weaviate.Client(
         embedded_options=EmbeddedOptions(
             persistence_data_path=tmp_path_factory.mktemp("data"),
             binary_path=tmp_path_factory.mktemp("bin"),
             version="latest",
             port=30668,
             additional_env_vars={"GRPC_PORT": "50060"},
             grpc_port=50060,
         )
     )
-    meta = client.get_meta()
-    latest = requests.get("https://api.github.com/repos/weaviate/weaviate/releases/latest").json()
-    assert "v" + meta["version"] == latest["tag_name"]
+    try:
+        meta = client.get_meta()
+        latest = requests.get(
+            "https://api.github.com/repos/weaviate/weaviate/releases/latest"
+        ).json()
+        assert "v" + meta["version"] == latest["tag_name"]
+    finally:
+        client._connection.embedded_db.stop()
 
 
 @pytest.mark.parametrize(
     "version",
     [
         "v1.16.6",
         "sdgfsdfposdfjpsdf",
@@ -284,50 +307,77 @@
             persistence_data_path=tmp_path_factory.mktemp("data"),
             binary_path=tmp_path_factory.mktemp("bin"),
             version="latest",
             port=30668,
             grpc_port=50061,
         ),
     )
+    try:
+        assert client.is_ready()
+        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        sock.settimeout(1.0)  # we're only pinging the port, 1s is plenty
+
+        assert sock.connect_ex(("127.0.0.1", 50061)) == 0  # running
+    finally:
+        client._connection.embedded_db.stop()
 
-    assert client.is_ready()
-    sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    sock.settimeout(1.0)  # we're only pinging the port, 1s is plenty
 
-    assert sock.connect_ex(("127.0.0.1", 50061)) == 0  # running
+def test_embedded_v4_with_grpc_port(tmp_path_factory: pytest.TempPathFactory):
+    client = weaviate.WeaviateClient(
+        embedded_options=EmbeddedOptions(
+            persistence_data_path=tmp_path_factory.mktemp("data"),
+            binary_path=tmp_path_factory.mktemp("bin"),
+            version="latest",
+            port=30668,
+            grpc_port=50061,
+        ),
+    )
+    try:
+        client.connect()
+        assert client.is_ready()
+        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        sock.settimeout(1.0)  # we're only pinging the port, 1s is plenty
+
+        assert sock.connect_ex(("127.0.0.1", 50061)) == 0  # running
+    finally:
+        client._connection.embedded_db.stop()
 
 
 def test_embedded_with_grpc_port_default(tmp_path_factory: pytest.TempPathFactory):
     client = weaviate.Client(
         embedded_options=EmbeddedOptions(
             persistence_data_path=tmp_path_factory.mktemp("data"),
             binary_path=tmp_path_factory.mktemp("bin"),
             version="latest",
             port=30669,
         )
     )
-
-    assert client.is_ready()
-    sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    sock.settimeout(1.0)  # we're only pinging the port, 1s is plenty
-
-    assert sock.connect_ex(("127.0.0.1", 50060)) == 0  # running
+    try:
+        assert client.is_ready()
+        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        sock.settimeout(1.0)  # we're only pinging the port, 1s is plenty
+
+        assert sock.connect_ex(("127.0.0.1", 50060)) == 0  # running
+    finally:
+        client._connection.embedded_db.stop()
 
 
 def test_embedded_stop(tmp_path_factory: pytest.TempPathFactory):
     client = weaviate.Client(
         embedded_options=EmbeddedOptions(
             persistence_data_path=tmp_path_factory.mktemp("data"),
             binary_path=tmp_path_factory.mktemp("bin"),
             version="latest",
             port=30668,
-            grpc_port=50061,
+            grpc_port=50060,
         ),
     )
+    try:
+        assert client.is_ready()
 
-    assert client.is_ready()
-
-    assert client._connection.embedded_db.process is not None
-    client._connection.embedded_db.stop()
-    assert client._connection.embedded_db.process is None
-    client._connection.embedded_db.stop()
-    assert client._connection.embedded_db.process is None
+        assert client._connection.embedded_db.process is not None
+        client._connection.embedded_db.stop()
+        assert client._connection.embedded_db.process is None
+        client._connection.embedded_db.stop()
+        assert client._connection.embedded_db.process is None
+    finally:
+        client._connection.embedded_db.stop()
```

### Comparing `weaviate_client-4.6.1/test/test_exceptions.py` & `weaviate_client-4.6.2/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/test_server_version.py` & `weaviate_client-4.6.2/test/test_server_version.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/test_util.py` & `weaviate_client-4.6.2/test/test_util.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/test/util.py` & `weaviate_client-4.6.2/test/util.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/__init__.py` & `weaviate_client-4.6.2/weaviate/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from .client import Client, WeaviateClient
 from .connect.helpers import (
     connect_to_custom,
     connect_to_embedded,
     connect_to_local,
     connect_to_wcs,
+    connect_to_weaviate_cloud,
 )
 
 from . import (
     auth,
     backup,
     batch,
     classes,
@@ -47,14 +48,15 @@
 __all__ = [
     "Client",
     "WeaviateClient",
     "connect_to_custom",
     "connect_to_embedded",
     "connect_to_local",
     "connect_to_wcs",
+    "connect_to_weaviate_cloud",
     "auth",
     "backup",
     "batch",
     "classes",
     "cluster",
     "collections",
     "config",
```

### Comparing `weaviate_client-4.6.1/weaviate/auth.py` & `weaviate_client-4.6.2/weaviate/auth.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/backup/backup.py` & `weaviate_client-4.6.2/weaviate/backup/backup.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/batch/crud_batch.py` & `weaviate_client-4.6.2/weaviate/batch/crud_batch.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/batch/requests.py` & `weaviate_client-4.6.2/weaviate/batch/requests.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/classes/config.py` & `weaviate_client-4.6.2/weaviate/classes/config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/classes/query.py` & `weaviate_client-4.6.2/weaviate/classes/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/classification/classification.py` & `weaviate_client-4.6.2/weaviate/classification/classification.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/classification/config_builder.py` & `weaviate_client-4.6.2/weaviate/classification/config_builder.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/client.py` & `weaviate_client-4.6.2/weaviate/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,16 +158,16 @@
         additional_config: Optional[AdditionalConfig] = None,
         skip_init_checks: bool = False,
     ) -> None:
         """Initialise a WeaviateClient class instance to use when interacting with Weaviate.
 
         Use this specific initializer when you want to create a custom Client specific to your Weaviate setup.
 
-        If you want to get going quickly connecting to WCS or a local instance then use the `weaviate.connect_to_wcs` or
-        `weaviate.connect_to_local` helper functions instead.
+        To simplify connections to Weaviate Cloud or local instances, use the weaviate.connect_to_weaviate_cloud
+        or weaviate.connect_to_local helper functions.
 
         Arguments:
             - `connection_params`: `weaviate.connect.ConnectionParams` or None, optional
                 - The connection parameters to use for the underlying HTTP requests.
             - `embedded_options`: `weaviate.EmbeddedOptions` or None, optional
                 - The options to use when provisioning an embedded Weaviate instance.
             - `auth_client_secret`: `weaviate.AuthCredentials` or None, optional
```

### Comparing `weaviate_client-4.6.1/weaviate/cluster/cluster.py` & `weaviate_client-4.6.2/weaviate/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/cluster/types.py` & `weaviate_client-4.6.2/weaviate/cluster/types.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/aggregations/base.py` & `weaviate_client-4.6.2/weaviate/collections/aggregations/base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/aggregations/hybrid.py` & `weaviate_client-4.6.2/weaviate/collections/aggregations/hybrid.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/aggregations/near_image.py` & `weaviate_client-4.6.2/weaviate/collections/aggregations/near_image.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/aggregations/near_object.py` & `weaviate_client-4.6.2/weaviate/collections/aggregations/near_object.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/aggregations/near_text.py` & `weaviate_client-4.6.2/weaviate/collections/aggregations/near_text.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/aggregations/near_vector.py` & `weaviate_client-4.6.2/weaviate/collections/aggregations/near_vector.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/aggregations/over_all.py` & `weaviate_client-4.6.2/weaviate/collections/aggregations/over_all.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/backups.py` & `weaviate_client-4.6.2/weaviate/collections/backups.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/base.py` & `weaviate_client-4.6.2/weaviate/collections/base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/batch/base.py` & `weaviate_client-4.6.2/weaviate/collections/batch/base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/batch/batch_wrapper.py` & `weaviate_client-4.6.2/weaviate/collections/batch/batch_wrapper.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/batch/client.py` & `weaviate_client-4.6.2/weaviate/collections/batch/client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/batch/collection.py` & `weaviate_client-4.6.2/weaviate/collections/batch/collection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/batch/grpc_batch_delete.py` & `weaviate_client-4.6.2/weaviate/collections/batch/grpc_batch_delete.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/batch/grpc_batch_objects.py` & `weaviate_client-4.6.2/weaviate/collections/batch/grpc_batch_objects.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/batch/rest.py` & `weaviate_client-4.6.2/weaviate/collections/batch/rest.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/classes/aggregate.py` & `weaviate_client-4.6.2/weaviate/collections/classes/aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/classes/batch.py` & `weaviate_client-4.6.2/weaviate/collections/classes/batch.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/classes/cluster.py` & `weaviate_client-4.6.2/weaviate/collections/classes/cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/classes/config.py` & `weaviate_client-4.6.2/weaviate/collections/classes/config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/classes/config_base.py` & `weaviate_client-4.6.2/weaviate/collections/classes/config_base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/classes/config_methods.py` & `weaviate_client-4.6.2/weaviate/collections/classes/config_methods.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/classes/config_named_vectors.py` & `weaviate_client-4.6.2/weaviate/collections/classes/config_named_vectors.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/classes/config_vector_index.py` & `weaviate_client-4.6.2/weaviate/collections/classes/config_vector_index.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/classes/config_vectorizers.py` & `weaviate_client-4.6.2/weaviate/collections/classes/config_vectorizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,21 @@
     "embed-english-light-v3.0",
 ]
 CohereTruncation: TypeAlias = Literal["NONE", "START", "END", "LEFT", "RIGHT"]
 OpenAIModel: TypeAlias = Literal[
     "text-embedding-3-small", "text-embedding-3-large", "text-embedding-ada-002"
 ]
 JinaModel: TypeAlias = Literal["jina-embeddings-v2-base-en", "jina-embeddings-v2-small-en"]
-VoyageModel: TypeAlias = Literal["voyage-large-2, voyage-code-2, voyage-2"]
+VoyageModel: TypeAlias = Literal[
+    "voyage-large-2",
+    "voyage-code-2",
+    "voyage-2",
+    "voyage-law-2",
+    "voyage-large-2-instruct",
+]
 AWSModel: TypeAlias = Literal[
     "amazon.titan-embed-text-v1",
     "cohere.embed-english-v3",
     "cohere.embed-multilingual-v3",
 ]
 AWSService: TypeAlias = Literal[
     "bedrock",
```

### Comparing `weaviate_client-4.6.1/weaviate/collections/classes/data.py` & `weaviate_client-4.6.2/weaviate/collections/classes/data.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/classes/filters.py` & `weaviate_client-4.6.2/weaviate/collections/classes/filters.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/classes/grpc.py` & `weaviate_client-4.6.2/weaviate/collections/classes/grpc.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/classes/internal.py` & `weaviate_client-4.6.2/weaviate/collections/classes/internal.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/classes/orm.py` & `weaviate_client-4.6.2/weaviate/collections/classes/orm.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/classes/tenants.py` & `weaviate_client-4.6.2/weaviate/collections/classes/tenants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/classes/types.py` & `weaviate_client-4.6.2/weaviate/collections/classes/types.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/cluster.py` & `weaviate_client-4.6.2/weaviate/collections/cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/collection.py` & `weaviate_client-4.6.2/weaviate/collections/collection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/collections.py` & `weaviate_client-4.6.2/weaviate/collections/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     _VectorIndexConfigCreate,
     Property,
     _ShardingConfigCreate,
     _ReferencePropertyBase,
     _ReplicationConfigCreate,
     _RerankerConfigCreate,
     _VectorizerConfigCreate,
-    _Vectorizer,
 )
 from weaviate.collections.classes.internal import References
 from weaviate.collections.classes.types import (
     Properties,
     _check_properties_generic,
     _check_references_generic,
 )
@@ -118,15 +117,15 @@
             multi_tenancy_config=multi_tenancy_config,
             name=name,
             properties=properties,
             references=references,
             replication_config=replication_config,
             reranker_config=reranker_config,
             sharding_config=sharding_config,
-            vectorizer_config=vectorizer_config or _Vectorizer.none(),
+            vectorizer_config=vectorizer_config,
             vector_index_config=vector_index_config,
         )
 
         name = super()._create(config._to_dict())
         assert (
             config.name == name
         ), f"Name of created collection ({name}) does not match given name ({config.name})"
```

### Comparing `weaviate_client-4.6.1/weaviate/collections/config.py` & `weaviate_client-4.6.2/weaviate/collections/config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/data.py` & `weaviate_client-4.6.2/weaviate/collections/data.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/filters.py` & `weaviate_client-4.6.2/weaviate/collections/filters.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/grpc/query.py` & `weaviate_client-4.6.2/weaviate/collections/grpc/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/grpc/shared.py` & `weaviate_client-4.6.2/weaviate/collections/grpc/shared.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/grpc/tenants.py` & `weaviate_client-4.6.2/weaviate/collections/grpc/tenants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/iterator.py` & `weaviate_client-4.6.2/weaviate/collections/iterator.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/orm.py` & `weaviate_client-4.6.2/weaviate/collections/orm.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/base.py` & `weaviate_client-4.6.2/weaviate/collections/queries/base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/bm25/generate.py` & `weaviate_client-4.6.2/weaviate/collections/queries/bm25/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/bm25/generate.pyi` & `weaviate_client-4.6.2/weaviate/collections/queries/bm25/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/bm25/query.py` & `weaviate_client-4.6.2/weaviate/collections/queries/bm25/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/bm25/query.pyi` & `weaviate_client-4.6.2/weaviate/collections/queries/bm25/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/byteops.py` & `weaviate_client-4.6.2/weaviate/collections/queries/byteops.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/fetch_object_by_id/query.py` & `weaviate_client-4.6.2/weaviate/collections/queries/fetch_object_by_id/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/fetch_object_by_id/query.pyi` & `weaviate_client-4.6.2/weaviate/collections/queries/fetch_object_by_id/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/fetch_objects/generate.py` & `weaviate_client-4.6.2/weaviate/collections/queries/fetch_objects/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/fetch_objects/generate.pyi` & `weaviate_client-4.6.2/weaviate/collections/queries/fetch_objects/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/fetch_objects/query.py` & `weaviate_client-4.6.2/weaviate/collections/queries/fetch_objects/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/fetch_objects/query.pyi` & `weaviate_client-4.6.2/weaviate/collections/queries/fetch_objects/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/hybrid/generate.py` & `weaviate_client-4.6.2/weaviate/collections/queries/hybrid/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/hybrid/generate.pyi` & `weaviate_client-4.6.2/weaviate/collections/queries/hybrid/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/hybrid/query.py` & `weaviate_client-4.6.2/weaviate/collections/queries/hybrid/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/hybrid/query.pyi` & `weaviate_client-4.6.2/weaviate/collections/queries/hybrid/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/near_image/generate.py` & `weaviate_client-4.6.2/weaviate/collections/queries/near_image/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/near_image/generate.pyi` & `weaviate_client-4.6.2/weaviate/collections/queries/near_image/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/near_image/query.py` & `weaviate_client-4.6.2/weaviate/collections/queries/near_image/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/near_image/query.pyi` & `weaviate_client-4.6.2/weaviate/collections/queries/near_image/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/near_media/generate.py` & `weaviate_client-4.6.2/weaviate/collections/queries/near_media/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/near_media/generate.pyi` & `weaviate_client-4.6.2/weaviate/collections/queries/near_media/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/near_media/query.py` & `weaviate_client-4.6.2/weaviate/collections/queries/near_media/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/near_media/query.pyi` & `weaviate_client-4.6.2/weaviate/collections/queries/near_media/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/near_object/generate.py` & `weaviate_client-4.6.2/weaviate/collections/queries/near_object/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/near_object/generate.pyi` & `weaviate_client-4.6.2/weaviate/collections/queries/near_object/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/near_object/query.py` & `weaviate_client-4.6.2/weaviate/collections/queries/near_object/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/near_object/query.pyi` & `weaviate_client-4.6.2/weaviate/collections/queries/near_object/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/near_text/generate.py` & `weaviate_client-4.6.2/weaviate/collections/queries/near_text/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/near_text/generate.pyi` & `weaviate_client-4.6.2/weaviate/collections/queries/near_text/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/near_text/query.py` & `weaviate_client-4.6.2/weaviate/collections/queries/near_text/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/near_text/query.pyi` & `weaviate_client-4.6.2/weaviate/collections/queries/near_text/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/near_vector/generate.py` & `weaviate_client-4.6.2/weaviate/collections/queries/near_vector/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/near_vector/generate.pyi` & `weaviate_client-4.6.2/weaviate/collections/queries/near_vector/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/near_vector/query.py` & `weaviate_client-4.6.2/weaviate/collections/queries/near_vector/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/queries/near_vector/query.pyi` & `weaviate_client-4.6.2/weaviate/collections/queries/near_vector/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/query.py` & `weaviate_client-4.6.2/weaviate/collections/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/collections/tenants.py` & `weaviate_client-4.6.2/weaviate/collections/tenants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/config.py` & `weaviate_client-4.6.2/weaviate/config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/connect/authentication.py` & `weaviate_client-4.6.2/weaviate/connect/authentication.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/connect/base.py` & `weaviate_client-4.6.2/weaviate/connect/base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/connect/helpers.py` & `weaviate_client-4.6.2/weaviate/connect/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 from weaviate.client import WeaviateClient
 from weaviate.config import AdditionalConfig
 from weaviate.connect.base import ConnectionParams, ProtocolParams
 from weaviate.embedded import EmbeddedOptions
 from weaviate.validator import _validate_input, _ValidateArgument
 
 
-def connect_to_wcs(
+def connect_to_weaviate_cloud(
     cluster_url: str,
     auth_credentials: Optional[AuthCredentials],
     headers: Optional[Dict[str, str]] = None,
     additional_config: Optional[AdditionalConfig] = None,
     skip_init_checks: bool = False,
 ) -> WeaviateClient:
     """
-    Connect to your own Weaviate Cloud Service (WCS) instance.
+    Connect to a Weaviate Cloud (WCD) instance.
 
     This method handles automatically connecting to Weaviate but not automatically closing the connection. Once you are done with the client
     you should call `client.close()` to close the connection and free up resources. Alternatively, you can use the client as a context manager
     in a `with` statement, which will automatically close the connection when the context is exited. See the examples below for details.
 
     Arguments:
         `cluster_url`
-            The WCS cluster URL or hostname to connect to. Usually in the form rAnD0mD1g1t5.something.weaviate.cloud
+            The WCD cluster URL or hostname to connect to. Usually in the form: rAnD0mD1g1t5.something.weaviate.cloud
         `auth_credentials`
             The credentials to use for authentication with your Weaviate instance. This can be an API key, in which case use `weaviate.classes.init.Auth.api_key()`,
             a bearer token, in which case use `weaviate.classes.init.Auth.bearer_token()`, a client secret, in which case use `weaviate.classes.init.Auth.client_credentials()`
             or a username and password, in which case use `weaviate.classes.init.Auth.client_password()`.
         `headers`
             Additional headers to include in the requests, e.g. API keys for third-party Cloud vectorization.
         `additional_config`
@@ -81,14 +81,70 @@
         additional_headers=headers,
         additional_config=additional_config,
         skip_init_checks=skip_init_checks,
     )
     return __connect(client)
 
 
+def connect_to_wcs(
+    cluster_url: str,
+    auth_credentials: Optional[AuthCredentials],
+    headers: Optional[Dict[str, str]] = None,
+    additional_config: Optional[AdditionalConfig] = None,
+    skip_init_checks: bool = False,
+) -> WeaviateClient:
+    """
+    Connect to a Weaviate Cloud (WCD) instance.
+
+    This method handles automatically connecting to Weaviate but not automatically closing the connection. Once you are done with the client
+    you should call `client.close()` to close the connection and free up resources. Alternatively, you can use the client as a context manager
+    in a `with` statement, which will automatically close the connection when the context is exited. See the examples below for details.
+
+    Arguments:
+        `cluster_url`
+            The WCD cluster URL or hostname to connect to. Usually in the form: rAnD0mD1g1t5.something.weaviate.cloud
+        `auth_credentials`
+            The credentials to use for authentication with your Weaviate instance. This can be an API key, in which case use `weaviate.classes.init.Auth.api_key()`,
+            a bearer token, in which case use `weaviate.classes.init.Auth.bearer_token()`, a client secret, in which case use `weaviate.classes.init.Auth.client_credentials()`
+            or a username and password, in which case use `weaviate.classes.init.Auth.client_password()`.
+        `headers`
+            Additional headers to include in the requests, e.g. API keys for third-party Cloud vectorization.
+        `additional_config`
+            This includes many additional, rarely used config options. use wvc.init.AdditionalConfig() to configure.
+        `skip_init_checks`
+            Whether to skip the initialization checks when connecting to Weaviate.
+
+    Returns
+        `weaviate.WeaviateClient`
+            The client connected to the cluster with the required parameters set appropriately.
+
+    Examples:
+        >>> import weaviate
+        >>> client = weaviate.connect_to_wcs(
+        ...     cluster_url="rAnD0mD1g1t5.something.weaviate.cloud",
+        ...     auth_credentials=weaviate.classes.init.Auth.api_key("my-api-key"),
+        ... )
+        >>> client.is_ready()
+        True
+        >>> client.close() # Close the connection when you are done with it.
+        ################## With Context Manager #############################
+        >>> import weaviate
+        >>> with weaviate.connect_to_wcs(
+        ...     cluster_url="rAnD0mD1g1t5.something.weaviate.cloud",
+        ...     auth_credentials=weaviate.classes.init.Auth.api_key("my-api-key"),
+        ... ) as client:
+        ...     client.is_ready()
+        True
+        >>> # The connection is automatically closed when the context is exited.
+    """
+    return connect_to_weaviate_cloud(
+        cluster_url, auth_credentials, headers, additional_config, skip_init_checks
+    )
+
+
 def connect_to_local(
     host: str = "localhost",
     port: int = 8080,
     grpc_port: int = 50051,
     headers: Optional[Dict[str, str]] = None,
     additional_config: Optional[AdditionalConfig] = None,
     skip_init_checks: bool = False,
```

### Comparing `weaviate_client-4.6.1/weaviate/connect/integrations.py` & `weaviate_client-4.6.2/weaviate/connect/integrations.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/connect/v3.py` & `weaviate_client-4.6.2/weaviate/connect/v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,17 @@
             pkg_info = pkg_info.get("info", {})
             latest_version = pkg_info.get("version", "unknown version")
             if is_weaviate_client_too_old(client_version, latest_version):
                 _Warnings.weaviate_client_too_old_vs_latest(client_version, latest_version)
         except requests.exceptions.RequestException:
             pass  # ignore any errors related to requests, it is a best-effort warning
 
+        if embedded_db is not None:
+            self.wait_for_weaviate(10)
+
     def _create_sessions(self, auth_client_secret: Optional[AuthCredentials]) -> None:
         """Creates a async httpx session and a sync request session.
 
         Either through authlib.oauth2 if authentication is enabled or a normal request session otherwise.
 
         Raises
         ------
@@ -233,21 +236,20 @@
                 msg = f""""No login credentials provided. The weaviate instance at {self.url} requires login credentials.
 
                     For more information, see: https://weaviate.io/developers/weaviate/client-libraries/python#authentication"""
 
                 if is_weaviate_domain(self.url):
                     msg += """
 
-                    You can instantiate the client with login credentials for WCS using
+                    You can instantiate the client with login credentials for Weaviate Cloud using
 
                     client = weaviate.Client(
                       url=YOUR_WEAVIATE_URL,
-                      auth_client_secret=weaviate.AuthClientPassword(
-                        username = YOUR_WCS_USER,
-                        password = YOUR_WCS_PW,
+                      auth_client_secret=weaviate.AuthApiKey(
+                        api_key = YOUR_WCD_API_KEY,
                       ))
                     """
                 raise AuthenticationFailedException(msg)
         elif response.status_code == 404 and auth_client_secret is not None:
             _Warnings.auth_with_anon_weaviate()
             self._session = requests.Session()
         else:
```

### Comparing `weaviate_client-4.6.1/weaviate/connect/v4.py` & `weaviate_client-4.6.2/weaviate/connect/v4.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from grpc_health.v1 import health_pb2  # type: ignore
 from httpx import (
     AsyncClient,
     AsyncHTTPTransport,
     Client,
     ConnectError,
     HTTPError,
+    HTTPStatusError,
     Limits,
     ReadError,
     RemoteProtocolError,
     RequestError,
     Response,
     HTTPTransport,
     get,
@@ -132,14 +133,21 @@
             self._headers["authorization"] = "Bearer " + auth_client_secret.api_key
 
     def connect(self, skip_init_checks: bool) -> None:
         if self.embedded_db is not None:
             self.embedded_db.start()
         self._create_clients(self._auth, skip_init_checks)
         self.__connected = True
+        if self.embedded_db is not None:
+            try:
+                self.wait_for_weaviate(10)
+            except WeaviateStartUpError as e:
+                self.embedded_db.stop()
+                self.__connected = False
+                raise e
 
         # need this to get the version of weaviate for version checks
         try:
             self._weaviate_version = _ServerVersion.from_string(self.get_meta()["version"])
         except (WeaviateConnectionError, ReadError, RemoteProtocolError) as e:
             raise WeaviateStartUpError(f"Could not connect to Weaviate:{e}.") from e
 
@@ -287,17 +295,17 @@
 
                     Please check our documentation at https://weaviate.io/developers/weaviate/client-libraries/python#authentication
                     for more information about how to use authentication."""
 
                 if is_weaviate_domain(self.url):
                     msg += """
 
-                    You can instantiate the client with login credentials for WCS using
+                    You can instantiate the client with login credentials for Weaviate Cloud using
 
-                    client = weaviate.connect_to_wcs(
+                    client = weaviate.connect_to_weaviate_cloud(
                       url=YOUR_WEAVIATE_URL,
                       auth_client_secret=wvc.init.Auth.api_key("YOUR_API_KEY")
                     )
                     """
                 raise AuthenticationFailedError(msg)
         elif response.status_code == 404 and auth_client_secret is not None:
             _Warnings.auth_with_anon_weaviate()
@@ -591,14 +599,43 @@
         res = _decode_json_response_dict(response, "Meta endpoint")
         assert res is not None
         return res
 
     def supports_groupby_in_bm25_and_hybrid(self) -> bool:
         return self._weaviate_version.is_at_least(1, 25, 0)
 
+    def wait_for_weaviate(self, startup_period: int) -> None:
+        """
+        Waits until weaviate is ready or the time limit given in 'startup_period' has passed.
+
+        Parameters
+        ----------
+        startup_period : int
+            Describes how long the client will wait for weaviate to start in seconds.
+
+        Raises
+        ------
+        WeaviateStartUpError
+            If weaviate takes longer than the time limit to respond.
+        """
+        for _i in range(startup_period):
+            try:
+                self.get("/.well-known/ready").raise_for_status()
+                return
+            except (ConnectError, ReadError, TimeoutError, HTTPStatusError):
+                time.sleep(1)
+
+        try:
+            self.get("/.well-known/ready").raise_for_status()
+            return
+        except (ConnectError, ReadError, TimeoutError) as error:
+            raise WeaviateStartUpError(
+                f"Weaviate did not start up in {startup_period} seconds. Either the Weaviate URL {self.url} is wrong or Weaviate did not start up in the interval given in 'startup_period'."
+            ) from error
+
 
 class ConnectionV4(_Connection):
     def __init__(
         self,
         connection_params: ConnectionParams,
         auth_client_secret: Optional[AuthCredentials],
         timeout_config: TimeoutConfig,
```

### Comparing `weaviate_client-4.6.1/weaviate/contextionary/crud_contextionary.py` & `weaviate_client-4.6.2/weaviate/contextionary/crud_contextionary.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/data/crud_data.py` & `weaviate_client-4.6.2/weaviate/data/crud_data.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/data/references/crud_references.py` & `weaviate_client-4.6.2/weaviate/data/references/crud_references.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/embedded.py` & `weaviate_client-4.6.2/weaviate/embedded.py`

 * *Files 3% similar despite different names*

```diff
@@ -204,14 +204,19 @@
 
         my_env.setdefault("AUTHENTICATION_ANONYMOUS_ACCESS_ENABLED", "true")
         my_env.setdefault("QUERY_DEFAULTS_LIMIT", "20")
         my_env.setdefault("PERSISTENCE_DATA_PATH", self.options.persistence_data_path)
         # Bug with weaviate requires setting gossip and data bind port
         my_env.setdefault("CLUSTER_GOSSIP_BIND_PORT", str(get_random_port()))
         my_env.setdefault("GRPC_PORT", str(self.grpc_port))
+        my_env.setdefault("RAFT_BOOTSTRAP_EXPECT", str(1))
+        my_env.setdefault("CLUSTER_IN_LOCALHOST", str(True))
+        my_env.setdefault("RAFT_PORT", str(get_random_port()))
+        my_env.setdefault("RAFT_INTERNAL_RPC_PORT", str(get_random_port()))
+        my_env.setdefault("PROFILING_PORT", str(get_random_port()))
 
         my_env.setdefault(
             "ENABLE_MODULES",
             "text2vec-openai,text2vec-cohere,text2vec-huggingface,ref2vec-centroid,generative-openai,qna-openai,"
             "reranker-cohere",
         )
```

### Comparing `weaviate_client-4.6.1/weaviate/error_msgs.py` & `weaviate_client-4.6.2/weaviate/error_msgs.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/exceptions.py` & `weaviate_client-4.6.2/weaviate/exceptions.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/gql/aggregate.py` & `weaviate_client-4.6.2/weaviate/gql/aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/gql/filter.py` & `weaviate_client-4.6.2/weaviate/gql/filter.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/gql/get.py` & `weaviate_client-4.6.2/weaviate/gql/get.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/gql/multi_get.py` & `weaviate_client-4.6.2/weaviate/gql/multi_get.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/gql/query.py` & `weaviate_client-4.6.2/weaviate/gql/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/integrations.py` & `weaviate_client-4.6.2/weaviate/integrations.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/outputs/aggregate.py` & `weaviate_client-4.6.2/weaviate/outputs/aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/outputs/config.py` & `weaviate_client-4.6.2/weaviate/outputs/config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/outputs/query.py` & `weaviate_client-4.6.2/weaviate/outputs/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/proto/v1/base_pb2.py` & `weaviate_client-4.6.2/weaviate/proto/v1/base_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/proto/v1/base_pb2.pyi` & `weaviate_client-4.6.2/weaviate/proto/v1/base_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/proto/v1/batch_delete_pb2.py` & `weaviate_client-4.6.2/weaviate/proto/v1/batch_delete_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/proto/v1/batch_delete_pb2.pyi` & `weaviate_client-4.6.2/weaviate/proto/v1/batch_delete_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/proto/v1/batch_pb2.py` & `weaviate_client-4.6.2/weaviate/proto/v1/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/proto/v1/batch_pb2.pyi` & `weaviate_client-4.6.2/weaviate/proto/v1/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/proto/v1/properties_pb2.py` & `weaviate_client-4.6.2/weaviate/proto/v1/properties_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/proto/v1/properties_pb2.pyi` & `weaviate_client-4.6.2/weaviate/proto/v1/properties_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/proto/v1/search_get_pb2.py` & `weaviate_client-4.6.2/weaviate/proto/v1/search_get_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/proto/v1/search_get_pb2.pyi` & `weaviate_client-4.6.2/weaviate/proto/v1/search_get_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/proto/v1/tenants_pb2.py` & `weaviate_client-4.6.2/weaviate/proto/v1/tenants_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/proto/v1/tenants_pb2.pyi` & `weaviate_client-4.6.2/weaviate/proto/v1/tenants_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/proto/v1/weaviate_pb2.py` & `weaviate_client-4.6.2/weaviate/proto/v1/weaviate_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/proto/v1/weaviate_pb2_grpc.py` & `weaviate_client-4.6.2/weaviate/proto/v1/weaviate_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/schema/crud_schema.py` & `weaviate_client-4.6.2/weaviate/schema/crud_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/schema/properties/crud_properties.py` & `weaviate_client-4.6.2/weaviate/schema/properties/crud_properties.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/types.py` & `weaviate_client-4.6.2/weaviate/types.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/util.py` & `weaviate_client-4.6.2/weaviate/util.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/validator.py` & `weaviate_client-4.6.2/weaviate/validator.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.1/weaviate/warnings.py` & `weaviate_client-4.6.2/weaviate/warnings.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,36 +9,36 @@
     __version__ = "unknown version"
 
 
 class _Warnings:
     @staticmethod
     def auth_with_anon_weaviate() -> None:
         warnings.warn(
-            message="""Auth001: The client was configured to use authentication, but weaviate is configured without
+            message="""Auth001: The client is configured to use authentication, but weaviate is configured without
                     authentication. Are you sure this is correct?""",
             category=UserWarning,
             stacklevel=1,
         )
 
     @staticmethod
     def auth_no_refresh_token(auth_len: Optional[int] = None) -> None:
         if auth_len is not None:
             msg = f"The current access token is only valid for {auth_len}s."
         else:
             msg = "Also, no expiration time was given."
 
         warnings.warn(
-            message=f"""Auth002: The token returned from you identity provider does not contain a refresh token. {msg}
+            message=f"""Auth002: The token your identity provider returned does not contain a refresh token. {msg}
 
-            Access to your weaviate instance is not possible after expiration and this client will return an
+            Access to your weaviate instance is not possible after the token expires. This client returns an
             authentication exception.
 
             Things to try:
-            - You might need to enable refresh tokens in the settings of your authentication provider
-            - You might need to send the correct scope. For some providers it needs to include "offline_access"
+            - You might need to enable refresh tokens in your authentication provider settings.
+            - You might need to send the correct scope. For some providers, the scope needs to include "offline_access".
             """,
             category=UserWarning,
             stacklevel=1,
         )
 
     @staticmethod
     def auth_negative_expiration_time(expires_in: int) -> None:
@@ -46,45 +46,47 @@
 
         warnings.warn(message=msg, category=UserWarning, stacklevel=1)
 
     @staticmethod
     def auth_header_and_auth_secret() -> None:
         msg = """Auth004: Received an authentication header and an auth_client_secret parameter.
 
-         The auth_client_secret takes precedence over the header and the authentication header will be ignored. Use
-         weaviate.auth.AuthBearerToken(..) to supply an access token via auth_client_secret parameter and (if available)
-         also supply refresh tokens and token lifetimes.
-         """
+        The auth_client_secret takes precedence over the header. The authentication header will be ignored.
+
+        Use weaviate.auth.AuthBearerToken(..) to supply an access token via auth_client_secret parameter and,
+        if available with your provider, to supply refresh tokens and token lifetimes.
+        """
         warnings.warn(message=msg, category=UserWarning, stacklevel=1)
 
     @staticmethod
     def auth_cannot_parse_oidc_config(url: str) -> None:
         msg = f"""Auth005: Could not parse Weaviate's OIDC configuration, using unauthenticated access. If you added
         an authorization header yourself it will be unaffected.
 
-        This can happen if weaviate is miss-configured or you have a proxy between the client and weaviate.
+        This can happen if weaviate is miss-configured or if you have a proxy between the client and weaviate.
         You can test this by visiting {url}."""
         warnings.warn(message=msg, category=UserWarning, stacklevel=1)
 
     @staticmethod
     def weaviate_server_older_than_1_14(server_version: str) -> None:
         warnings.warn(
-            message=f"""Dep001: You are using the Weaviate Python Client version {__version__} which supports
+            message=f"""Dep001: You are using Weaviate Python Client version {__version__}. This version supports
             changes and features of Weaviate >=1.14.x, but you are connected to Weaviate {server_version}.
-            If you want to make use of these new changes/features using this Python Client version, upgrade your
+
+            To use this Python Client with the new features, upgrade your
             Weaviate instance.""",
             category=DeprecationWarning,
             stacklevel=1,
         )
 
     @staticmethod
     def manual_batching() -> None:
         warnings.warn(
-            message="""Dep002: You are batching manually. This means you are NOT using the client's built-in
-            multi-threading. Setting `batch_size` in `client.batch.configure()`  to an int value will enabled automatic
+            message="""Dep002: Manual batching does NOT use the client's built-in multi-threading. Set
+            `batch_size` in `client.batch.configure()` to an integer value to enabled automatic
             batching. See:
             https://weaviate.io/developers/weaviate/current/restful-api-references/batch.html#example-request-1""",
             category=DeprecationWarning,
             stacklevel=1,
         )
 
     @staticmethod
@@ -95,137 +97,139 @@
             category=DeprecationWarning,
             stacklevel=1,
         )
 
     @staticmethod
     def startup_period_deprecated() -> None:
         warnings.warn(
-            message="""Dep004: startup_period is deprecated and has no effect. Please remove it from your code.""",
+            message="""Dep004: startup_period is deprecated and has no effect.""",
             category=DeprecationWarning,
             stacklevel=1,
         )
 
     @staticmethod
     def token_refresh_failed(exc: Exception) -> None:
         warnings.warn(
             message=f"""Con001: Could not reach token issuer for the periodic refresh. This client will automatically
-            retry to refresh. If this does not succeed, the client will become unauthenticated.
-            Causes might be an unstable internet connection or a problem with your authentication provider.
+            retry to refresh. If the retry does not succeed, the client will become unauthenticated.
+
+            The cause might be an unstable internet connection or a problem with your authentication provider.
             Exception: {exc}
             """,
             category=UserWarning,
             stacklevel=1,
         )
 
     @staticmethod
     def weaviate_too_old_vs_latest(server_version: str) -> None:
         warnings.warn(
             message=f"""Dep004: You are connected to Weaviate {server_version}.
-            Please consider upgrading to the latest version. See https://www.weaviate.io/developers/weaviate for details.""",
+            Consider upgrading to the latest version. See https://www.weaviate.io/developers/weaviate for details.""",
             category=DeprecationWarning,
             stacklevel=1,
         )
 
     @staticmethod
     def weaviate_client_too_old_vs_latest(client_version: str, latest_version: str) -> None:
         warnings.warn(
             message=f"""Dep005: You are using weaviate-client version {client_version}. The latest version is {latest_version}.
-            Please consider upgrading to the latest version. See https://weaviate.io/developers/weaviate/client-libraries/python for details.""",
+            Consider upgrading to the latest version. See https://weaviate.io/developers/weaviate/client-libraries/python for details.""",
             category=DeprecationWarning,
             stacklevel=1,
         )
 
     @staticmethod
     def use_of_client_batch_will_be_removed_in_next_major_release() -> None:
         warnings.warn(
-            message="""Dep006: You are using the `client.batch()` method, which will be removed in the next major release.
-            Please instead use the `client.batch.configure()` method to configure your batch and `client.batch` to enter the context manager.
+            message="""Dep006: You are using the `client.batch()` method. This method will be removed in the next major release.
+            Use the `client.batch.configure()` method to configure your batch process, and `client.batch` to enter the context manager.
+
             See https://weaviate.io/developers/weaviate/client-libraries/python for details.""",
             category=DeprecationWarning,
             stacklevel=1,
         )
 
     @staticmethod
     def root_module_import(name: str, loc: str) -> None:
         warnings.warn(
             f"Dep010: Importing {name} from weaviate is deprecated. "
-            f"Please import it from its specific module: weaviate.{loc}",
+            f"Import {name} from its module: weaviate.{loc}",
             DeprecationWarning,
             stacklevel=2,  # don't increase stacklevel, as this otherwise writes the auth-secrets into the log
         )
 
     @staticmethod
     def weaviate_v3_client_is_deprecated() -> None:
         warnings.warn(
-            message="""Dep016: You are creating a Weaviate v3 client using `client =  weaviate.Client(...)`, which is
-            deprecated. Consider creating a v4 (`weaviate.WeaviateClient`) client, using a `weaviate.connect_to_<method>`
-            helper function.
-            See here for
-                - migrating from v3 to v4: https://weaviate.io/developers/weaviate/client-libraries/python/v3_v4_migration
-                - general v4 usage: https://weaviate.io/developers/weaviate/client-libraries/python
+            message="""Dep016: Python client v3 `weaviate.Client(...)` connections and methods are deprecated. Update
+            your code to use Python client v4 `weaviate.WeaviateClient` connections and methods.
+
+            For Python Client v4 usage, see: https://weaviate.io/developers/weaviate/client-libraries/python
+            For code migration, see: https://weaviate.io/developers/weaviate/client-libraries/python/v3_v4_migration
             """,
             category=DeprecationWarning,
             stacklevel=1,
         )
 
     @staticmethod
     def vector_index_config_in_config_update() -> None:
         warnings.warn(
             message="""Dep017: You are using the `vector_index_config` argument in the `collection.config.update()` method, which is deprecated.
-            Please instead use the `vectorizer_config` argument instead.
+            Use the `vectorizer_config` argument instead.
             """,
             category=DeprecationWarning,
             stacklevel=1,
         )
 
     @staticmethod
     def sharding_actual_count_is_deprecated(argument: str) -> None:
         warnings.warn(
             message=f"""Dep018: You are using the {argument} argument in the `Configure.sharding` method, which is deprecated.
-            This field is read-only so has no effect and as such is deprecated. It will be removed in a future release.""",
+            This field is read-only, the argument has no effect. It will be removed in a future release.""",
             category=DeprecationWarning,
             stacklevel=1,
         )
 
     @staticmethod
     def bit_compression_in_pq_config() -> None:
         warnings.warn(
-            message="""Dep018: The `bit_compression` argument in `PQConfig` is deprecated and will be removed by Q4 2024.""",
+            message="""Dep019: The `bit_compression` argument in `PQConfig` is deprecated and will be removed by Q4 2024.""",
             category=DeprecationWarning,
             stacklevel=1,
         )
 
     @staticmethod
     def datetime_insertion_with_no_specified_timezone(date: datetime) -> None:
         warnings.warn(
             message=f"""Con002: You are inserting the datetime object {date} without a timezone. The timezone will be set to UTC.
-            If you want to use a different timezone, please specify it in the datetime object. For example:
+            To use a different timezone, specify it in the datetime object. For example:
             datetime.datetime(2021, 1, 1, 0, 0, 0, tzinfo=datetime.timezone(-datetime.timedelta(hours=2))).isoformat() = 2021-01-01T00:00:00-02:00
             """,
             category=UserWarning,
             stacklevel=1,
         )
 
     @staticmethod
     def text2vec_huggingface_endpoint_url_and_model_set_together() -> None:
         warnings.warn(
-            message="""Con003: You are setting the endpoint_url alongside model or passage_model and query_model in your Text2Vec-HuggingFace module configuration.
-            The model definitions will be ignored in favour of endpoint_url.
+            message="""Con003: You are setting the endpoint_url alongside model or passage_model and
+            query_model in your Text2Vec-HuggingFace module configuration. The model definitions will
+            be ignored in favour of endpoint_url.
             """,
             category=UserWarning,
             stacklevel=1,
         )
 
     @staticmethod
     def batch_executor_is_shutdown() -> None:
         warnings.warn(
             message="""Bat001: The BatchExecutor was shutdown, most probably when it exited the `with` statement.
-                It will be initialized again. If you are not `batch` in the `with client.batch as batch`
-                please make sure to shut it down when done importing data: `client.batch.shutdown()`.
-                You can start it again using the `client.batch.start()` method.""",
+                It will be initialized again. If you use `batch` outside the `with client.batch as batch` context,
+                shut down `batch` when the data import finishes: `client.batch.shutdown()`.
+                To start `batch` again, use the `client.batch.start()` method.""",
             category=UserWarning,
             stacklevel=1,
         )
 
     @staticmethod
     def batch_weaviate_overloaded_sleeping(sleep: int) -> None:
         warnings.warn(
@@ -233,24 +237,24 @@
             category=UserWarning,
             stacklevel=1,
         )
 
     @staticmethod
     def batch_refresh_failed(err: str) -> None:
         warnings.warn(
-            message=f"""Bat003: The dynamic batch-size could not be refreshed successfully with error {err}""",
+            message=f"""Bat003: The dynamic batch-size could not be refreshed successfully: error {err}""",
             category=UserWarning,
             stacklevel=1,
         )
 
     @staticmethod
     def batch_retrying_failed_batches_hit_hard_limit(limit: int) -> None:
         warnings.warn(
-            message=f"""Bat004: Attempts to retry failed objects and/or references have hit the hard limit of {limit}.
-            The failed objects and references can be accessed in client.collections.batch.failed_objects and client.collections.batch.failed_references.""",
+            message=f"""Bat004: Attempts to retry failed objects or references have hit the hard limit of {limit}.
+            The failed objects or references can be accessed in client.collections.batch.failed_objects and client.collections.batch.failed_references.""",
             category=UserWarning,
             stacklevel=1,
         )
 
     @staticmethod
     def batch_rate_limit_reached(msg: str, seconds: int) -> None:
         warnings.warn(
```

### Comparing `weaviate_client-4.6.1/weaviate_client.egg-info/PKG-INFO` & `weaviate_client-4.6.2/weaviate_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weaviate-client
-Version: 4.6.1
+Version: 4.6.2
 Summary: A python native Weaviate client
 Home-page: https://github.com/weaviate/weaviate-python-client
 Author: Weaviate
 Author-email: hello@weaviate.io,
 License: BSD 3-clause
 Project-URL: Documentation, https://weaviate-python-client.readthedocs.io
 Project-URL: Source, https://github.com/weaviate/weaviate-python-client
```

### Comparing `weaviate_client-4.6.1/weaviate_client.egg-info/SOURCES.txt` & `weaviate_client-4.6.2/weaviate_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

