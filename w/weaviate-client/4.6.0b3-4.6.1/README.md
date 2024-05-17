# Comparing `tmp/weaviate_client-4.6.0b3.tar.gz` & `tmp/weaviate_client-4.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weaviate_client-4.6.0b3.tar", last modified: Thu May  9 03:59:19 2024, max compression
+gzip compressed data, was "weaviate_client-4.6.1.tar", last modified: Tue May 14 18:53:52 2024, max compression
```

## Comparing `weaviate_client-4.6.0b3.tar` & `weaviate_client-4.6.1.tar`

### file list

```diff
@@ -1,425 +1,425 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.258886 weaviate_client-4.6.0b3/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.198886 weaviate_client-4.6.0b3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.198886 weaviate_client-4.6.0b3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/.github/workflows/main.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    19131 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-09 03:59:19.258886 weaviate_client-4.6.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.202886 weaviate_client-4.6.0b3/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/ci/compose.sh
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/ci/docker-compose-async.yml
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/ci/docker-compose-azure.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/ci/docker-compose-cluster.yml
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/ci/docker-compose-generative.yml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/ci/docker-compose-okta-cc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/ci/docker-compose-okta-users.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/ci/docker-compose-proxy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/ci/docker-compose-rerank.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/ci/docker-compose-wcs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/ci/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.202886 weaviate_client-4.6.0b3/ci/proxy/
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/ci/proxy/envoy.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      922 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/ci/start_weaviate.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/ci/stop_weaviate.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.206886 weaviate_client-4.6.0b3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    56116 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.auth.rst
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.backup.rst
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.batch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.classification.rst
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.client.rst
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.cluster.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.collections.aggregations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.collections.batch.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.collections.classes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.collections.grpc.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.collections.queries.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.collections.rst
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.connect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.contextionary.rst
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.data.references.rst
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.data.replication.rst
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.gql.rst
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.proto.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.proto.v1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.rst
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.schema.properties.rst
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.schema.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/docs/weaviate.util.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.210886 weaviate_client-4.6.0b3/integration/
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/1234.3gp
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)   172641 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/hobbits.mp4
--rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    19306 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_batch_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    78596 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    31180 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_collection_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_collection_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    21235 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_collection_batch_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    34333 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_collection_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27875 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_collection_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_collection_geo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_collection_get.py
--rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_collection_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_collection_multi_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    18946 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_collection_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)    25027 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_collection_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    41744 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_collection_references.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_collection_rerank.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_gql_raw_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21762 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_named_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/test_tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration/weaviate-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.210886 weaviate_client-4.6.0b3/integration_embedded/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration_embedded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration_embedded/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.214886 weaviate_client-4.6.0b3/integration_v3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration_v3/people_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration_v3/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration_v3/test_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration_v3/test_backup_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)    20525 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration_v3/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration_v3/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration_v3/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    31522 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration_v3/test_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    24351 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration_v3/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration_v3/test_grcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration_v3/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration_v3/test_stress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/integration_v3/test_timeout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.214886 weaviate_client-4.6.0b3/mock_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/mock_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/mock_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/mock_tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/mock_tests/test_automatic_retries.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/mock_tests/test_batching_manual.py
--rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/mock_tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/mock_tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/mock_tests/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/mock_tests/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/mock_tests/test_resend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/mock_tests/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.218886 weaviate_client-4.6.0b3/profiling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/profiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/profiling/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/profiling/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/profiling/test_import_and_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/profiling/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/profiling/test_refs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/profiling/test_sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/publishing.md
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/run-mypy.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-09 03:59:19.258886 weaviate_client-4.6.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.218886 weaviate_client-4.6.0b3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.218886 weaviate_client-4.6.0b3/test/batch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/batch/test_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.218886 weaviate_client-4.6.0b3/test/classification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19246 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/classification/test_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.218886 weaviate_client-4.6.0b3/test/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/cluster/test_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.222886 weaviate_client-4.6.0b3/test/collection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/collection/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/collection/test_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/collection/test_byteops.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/collection/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/collection/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/collection/test_collection_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    37924 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/collection/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/collection/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/collection/test_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.222886 weaviate_client-4.6.0b3/test/connection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/connection/test_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.222886 weaviate_client-4.6.0b3/test/contextionary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/contextionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/contextionary/test_text2vec_contextionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.222886 weaviate_client-4.6.0b3/test/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.222886 weaviate_client-4.6.0b3/test/data/references/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/data/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/data/references/test_crud_references.py
--rw-r--r--   0 runner    (1001) docker     (127)    31268 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/data/test_crud_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.222886 weaviate_client-4.6.0b3/test/gql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/gql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/gql/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)    46096 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/gql/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    33189 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/gql/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/gql/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.222886 weaviate_client-4.6.0b3/test/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.222886 weaviate_client-4.6.0b3/test/schema/properties/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/schema/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/schema/properties/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/schema/schema_company.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/schema/tenants.json
--rw-r--r--   0 runner    (1001) docker     (127)    25534 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/schema/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/test_embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/test_server_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    57211 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/test/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.226886 weaviate_client-4.6.0b3/weaviate/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.226886 weaviate_client-4.6.0b3/weaviate/backup/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26299 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/backup/backup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.226886 weaviate_client-4.6.0b3/weaviate/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74441 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/batch/crud_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/batch/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.230886 weaviate_client-4.6.0b3/weaviate/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/classes/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/classes/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/classes/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/classes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/classes/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/classes/generics.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/classes/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/classes/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/classes/tenants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.230886 weaviate_client-4.6.0b3/weaviate/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/classification/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/classification/config_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    22119 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.230886 weaviate_client-4.6.0b3/weaviate/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/cluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/cluster/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.230886 weaviate_client-4.6.0b3/weaviate/collections/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/aggregate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.234886 weaviate_client-4.6.0b3/weaviate/collections/aggregations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/aggregations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/aggregations/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/aggregations/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/aggregations/near_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/aggregations/near_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/aggregations/near_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/aggregations/near_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/aggregations/over_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/backups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.234886 weaviate_client-4.6.0b3/weaviate/collections/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27776 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/batch/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/batch/batch_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/batch/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/batch/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/batch/grpc_batch_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    15748 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/batch/grpc_batch_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/batch/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.238886 weaviate_client-4.6.0b3/weaviate/collections/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15550 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/classes/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/classes/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/classes/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    70969 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/classes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/classes/config_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13424 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/classes/config_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    41098 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/classes/config_named_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/classes/config_vector_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    40780 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/classes/config_vectorizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/classes/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    21511 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/classes/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/classes/grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19528 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/classes/internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/classes/orm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/classes/tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/classes/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    12632 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27210 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.238886 weaviate_client-4.6.0b3/weaviate/collections/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28488 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/grpc/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/grpc/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/grpc/tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.238886 weaviate_client-4.6.0b3/weaviate/collections/queries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24324 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.238886 weaviate_client-4.6.0b3/weaviate/collections/queries/bm25/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/bm25/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/bm25/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/bm25/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/bm25/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/bm25/query.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/byteops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.238886 weaviate_client-4.6.0b3/weaviate/collections/queries/fetch_object_by_id/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/fetch_object_by_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/fetch_object_by_id/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/fetch_object_by_id/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.242886 weaviate_client-4.6.0b3/weaviate/collections/queries/fetch_objects/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/fetch_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/fetch_objects/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/fetch_objects/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/fetch_objects/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/fetch_objects/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.242886 weaviate_client-4.6.0b3/weaviate/collections/queries/hybrid/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/hybrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/hybrid/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12154 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/hybrid/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/hybrid/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/hybrid/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.242886 weaviate_client-4.6.0b3/weaviate/collections/queries/near_image/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_image/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_image/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_image/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_image/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.242886 weaviate_client-4.6.0b3/weaviate/collections/queries/near_media/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_media/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_media/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_media/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_media/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.246886 weaviate_client-4.6.0b3/weaviate/collections/queries/near_object/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_object/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10965 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_object/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_object/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_object/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.246886 weaviate_client-4.6.0b3/weaviate/collections/queries/near_text/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_text/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_text/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_text/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_text/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.246886 weaviate_client-4.6.0b3/weaviate/collections/queries/near_vector/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_vector/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_vector/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_vector/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/queries/near_vector/query.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/collections/tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.246886 weaviate_client-4.6.0b3/weaviate/connect/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/connect/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/connect/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15187 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/connect/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/connect/integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)    24958 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/connect/v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    26680 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/connect/v4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.246886 weaviate_client-4.6.0b3/weaviate/contextionary/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/contextionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/contextionary/crud_contextionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.246886 weaviate_client-4.6.0b3/weaviate/data/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38789 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/data/crud_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.246886 weaviate_client-4.6.0b3/weaviate/data/references/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/data/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27102 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/data/references/crud_references.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.250886 weaviate_client-4.6.0b3/weaviate/data/replication/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/data/replication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/data/replication/replication.py
--rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/error_msgs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.250886 weaviate_client-4.6.0b3/weaviate/gql/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/gql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42084 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/gql/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)    36163 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/gql/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    75456 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/gql/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/gql/multi_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/gql/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.250886 weaviate_client-4.6.0b3/weaviate/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/outputs/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/outputs/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/outputs/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/outputs/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/outputs/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/outputs/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/outputs/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/outputs/tenants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.250886 weaviate_client-4.6.0b3/weaviate/proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.254886 weaviate_client-4.6.0b3/weaviate/proto/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/base_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/base_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/base_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/batch_delete_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/batch_delete_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/batch_delete_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/batch_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/batch_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/batch_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/properties_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/properties_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/properties_pb2_grpc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      391 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/regen.sh
--rw-r--r--   0 runner    (1001) docker     (127)    18051 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/search_get_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    29649 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/search_get_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/search_get_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/tenants_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/tenants_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/tenants_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/weaviate_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/weaviate_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/proto/v1/weaviate_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.254886 weaviate_client-4.6.0b3/weaviate/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34232 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/schema/crud_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.254886 weaviate_client-4.6.0b3/weaviate/schema/properties/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/schema/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/schema/properties/crud_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28584 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11662 2024-05-09 03:58:55.000000 weaviate_client-4.6.0b3/weaviate/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:59:19.258886 weaviate_client-4.6.0b3/weaviate_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-09 03:59:19.000000 weaviate_client-4.6.0b3/weaviate_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-09 03:59:19.000000 weaviate_client-4.6.0b3/weaviate_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 03:59:19.000000 weaviate_client-4.6.0b3/weaviate_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 03:59:18.000000 weaviate_client-4.6.0b3/weaviate_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-09 03:59:19.000000 weaviate_client-4.6.0b3/weaviate_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 03:59:19.000000 weaviate_client-4.6.0b3/weaviate_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.507894 weaviate_client-4.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.443894 weaviate_client-4.6.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.443894 weaviate_client-4.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    19131 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-14 18:53:52.507894 weaviate_client-4.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.447894 weaviate_client-4.6.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/compose.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/docker-compose-async.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/docker-compose-azure.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/docker-compose-cluster.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/docker-compose-generative.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/docker-compose-okta-cc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/docker-compose-okta-users.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/docker-compose-proxy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/docker-compose-rerank.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/docker-compose-wcs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.447894 weaviate_client-4.6.1/ci/proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/proxy/envoy.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      922 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/start_weaviate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/ci/stop_weaviate.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.451894 weaviate_client-4.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    56915 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.auth.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.backup.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.batch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.classification.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.client.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.cluster.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.collections.aggregations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.collections.batch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.collections.classes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.collections.grpc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.collections.queries.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.collections.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.connect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.contextionary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.data.references.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.data.replication.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.gql.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.proto.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.proto.v1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.schema.properties.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/docs/weaviate.util.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.459894 weaviate_client-4.6.1/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/1234.3gp
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)   172641 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/hobbits.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19306 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_batch_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78596 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31180 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21235 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_batch_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34333 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27875 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_multi_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18946 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25027 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41744 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_collection_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_gql_raw_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21762 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_named_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/test_tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration/weaviate-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.459894 weaviate_client-4.6.1/integration_embedded/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_embedded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_embedded/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.459894 weaviate_client-4.6.1/integration_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/people_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_backup_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20525 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31522 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24351 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_grcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_stress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/integration_v3/test_timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.463894 weaviate_client-4.6.1/mock_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/test_automatic_retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/test_batching_manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/test_resend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/mock_tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.463894 weaviate_client-4.6.1/profiling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/profiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/profiling/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/profiling/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/profiling/test_import_and_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/profiling/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/profiling/test_refs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/profiling/test_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/publishing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/run-mypy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-14 18:53:52.507894 weaviate_client-4.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.463894 weaviate_client-4.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.467894 weaviate_client-4.6.1/test/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/batch/test_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.467894 weaviate_client-4.6.1/test/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19246 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/classification/test_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.467894 weaviate_client-4.6.1/test/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/cluster/test_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.467894 weaviate_client-4.6.1/test/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/collection/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/collection/test_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/collection/test_byteops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/collection/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/collection/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/collection/test_collection_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37924 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/collection/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/collection/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/collection/test_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.467894 weaviate_client-4.6.1/test/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/connection/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.467894 weaviate_client-4.6.1/test/contextionary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/contextionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/contextionary/test_text2vec_contextionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.467894 weaviate_client-4.6.1/test/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.467894 weaviate_client-4.6.1/test/data/references/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/data/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/data/references/test_crud_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31268 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/data/test_crud_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.471894 weaviate_client-4.6.1/test/gql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/gql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/gql/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46096 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/gql/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33189 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/gql/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/gql/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.471894 weaviate_client-4.6.1/test/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.471894 weaviate_client-4.6.1/test/schema/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/schema/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/schema/properties/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/schema/schema_company.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/schema/tenants.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25534 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/schema/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/test_embedded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/test_server_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57211 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/test/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.471894 weaviate_client-4.6.1/weaviate/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.475894 weaviate_client-4.6.1/weaviate/backup/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26299 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/backup/backup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.475894 weaviate_client-4.6.1/weaviate/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74441 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/batch/crud_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/batch/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.475894 weaviate_client-4.6.1/weaviate/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classes/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classes/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classes/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classes/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classes/generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classes/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classes/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classes/tenants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.475894 weaviate_client-4.6.1/weaviate/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classification/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/classification/config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22119 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.475894 weaviate_client-4.6.1/weaviate/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/cluster/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/cluster/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.479894 weaviate_client-4.6.1/weaviate/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/aggregate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.479894 weaviate_client-4.6.1/weaviate/collections/aggregations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/aggregations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/aggregations/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/aggregations/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/aggregations/near_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/aggregations/near_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/aggregations/near_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/aggregations/near_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/aggregations/over_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/backups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.483894 weaviate_client-4.6.1/weaviate/collections/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27776 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/batch/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/batch/batch_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/batch/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/batch/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/batch/grpc_batch_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15748 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/batch/grpc_batch_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/batch/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.487894 weaviate_client-4.6.1/weaviate/collections/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15550 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70969 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13424 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/config_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41098 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/config_named_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/config_vector_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40780 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/config_vectorizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21511 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19528 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/classes/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12632 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27210 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.487894 weaviate_client-4.6.1/weaviate/collections/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28488 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/grpc/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/grpc/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/grpc/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.487894 weaviate_client-4.6.1/weaviate/collections/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24324 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.487894 weaviate_client-4.6.1/weaviate/collections/queries/bm25/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/bm25/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/bm25/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/bm25/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/bm25/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/bm25/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/byteops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.487894 weaviate_client-4.6.1/weaviate/collections/queries/fetch_object_by_id/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/fetch_object_by_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/fetch_object_by_id/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/fetch_object_by_id/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.487894 weaviate_client-4.6.1/weaviate/collections/queries/fetch_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/fetch_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/fetch_objects/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/fetch_objects/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/fetch_objects/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/fetch_objects/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.491894 weaviate_client-4.6.1/weaviate/collections/queries/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/hybrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/hybrid/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12154 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/hybrid/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/hybrid/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/hybrid/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.491894 weaviate_client-4.6.1/weaviate/collections/queries/near_image/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_image/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_image/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_image/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_image/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.491894 weaviate_client-4.6.1/weaviate/collections/queries/near_media/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_media/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_media/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_media/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_media/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.491894 weaviate_client-4.6.1/weaviate/collections/queries/near_object/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_object/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10965 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_object/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_object/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_object/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.495894 weaviate_client-4.6.1/weaviate/collections/queries/near_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_text/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_text/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_text/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_text/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.495894 weaviate_client-4.6.1/weaviate/collections/queries/near_vector/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_vector/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_vector/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_vector/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/queries/near_vector/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/collections/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.495894 weaviate_client-4.6.1/weaviate/connect/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/connect/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/connect/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15187 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/connect/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/connect/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24958 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/connect/v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26677 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/connect/v4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.495894 weaviate_client-4.6.1/weaviate/contextionary/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/contextionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/contextionary/crud_contextionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.495894 weaviate_client-4.6.1/weaviate/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38789 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/data/crud_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.495894 weaviate_client-4.6.1/weaviate/data/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/data/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27102 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/data/references/crud_references.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.495894 weaviate_client-4.6.1/weaviate/data/replication/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/data/replication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/data/replication/replication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/embedded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/error_msgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.499894 weaviate_client-4.6.1/weaviate/gql/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/gql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42084 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/gql/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36163 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/gql/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75456 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/gql/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/gql/multi_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/gql/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.499894 weaviate_client-4.6.1/weaviate/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/outputs/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/outputs/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/outputs/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/outputs/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/outputs/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/outputs/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/outputs/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/outputs/tenants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.499894 weaviate_client-4.6.1/weaviate/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.503894 weaviate_client-4.6.1/weaviate/proto/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/base_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/base_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/base_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/batch_delete_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/batch_delete_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/batch_delete_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/batch_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/batch_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/batch_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/properties_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/properties_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/properties_pb2_grpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      391 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/regen.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    18051 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/search_get_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29649 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/search_get_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/search_get_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/tenants_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/tenants_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/tenants_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/weaviate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/weaviate_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/proto/v1/weaviate_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.503894 weaviate_client-4.6.1/weaviate/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34232 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/schema/crud_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.503894 weaviate_client-4.6.1/weaviate/schema/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/schema/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/schema/properties/crud_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28584 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11919 2024-05-14 18:53:21.000000 weaviate_client-4.6.1/weaviate/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:53:52.507894 weaviate_client-4.6.1/weaviate_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-14 18:53:52.000000 weaviate_client-4.6.1/weaviate_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-14 18:53:52.000000 weaviate_client-4.6.1/weaviate_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:53:52.000000 weaviate_client-4.6.1/weaviate_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:53:52.000000 weaviate_client-4.6.1/weaviate_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-14 18:53:52.000000 weaviate_client-4.6.1/weaviate_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 18:53:52.000000 weaviate_client-4.6.1/weaviate_client.egg-info/top_level.txt
```

### Comparing `weaviate_client-4.6.0b3/.flake8` & `weaviate_client-4.6.1/.flake8`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/.github/workflows/main.yaml` & `weaviate_client-4.6.1/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/.pre-commit-config.yaml` & `weaviate_client-4.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/.pylintrc` & `weaviate_client-4.6.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/CONTRIBUTING.md` & `weaviate_client-4.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/LICENSE` & `weaviate_client-4.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/PKG-INFO` & `weaviate_client-4.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weaviate-client
-Version: 4.6.0b3
+Version: 4.6.1
 Summary: A python native Weaviate client
 Home-page: https://github.com/weaviate/weaviate-python-client
 Author: Weaviate
 Author-email: hello@weaviate.io,
 License: BSD 3-clause
 Project-URL: Documentation, https://weaviate-python-client.readthedocs.io
 Project-URL: Source, https://github.com/weaviate/weaviate-python-client
```

### Comparing `weaviate_client-4.6.0b3/README.rst` & `weaviate_client-4.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/ci/docker-compose-async.yml` & `weaviate_client-4.6.1/ci/docker-compose-async.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/ci/docker-compose-azure.yml` & `weaviate_client-4.6.1/ci/docker-compose-azure.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/ci/docker-compose-cluster.yml` & `weaviate_client-4.6.1/ci/docker-compose-cluster.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/ci/docker-compose-generative.yml` & `weaviate_client-4.6.1/ci/docker-compose-generative.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/ci/docker-compose-okta-cc.yml` & `weaviate_client-4.6.1/ci/docker-compose-okta-cc.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/ci/docker-compose-okta-users.yml` & `weaviate_client-4.6.1/ci/docker-compose-okta-users.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/ci/docker-compose-proxy.yml` & `weaviate_client-4.6.1/ci/docker-compose-proxy.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/ci/docker-compose-rerank.yml` & `weaviate_client-4.6.1/ci/docker-compose-rerank.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/ci/docker-compose-wcs.yml` & `weaviate_client-4.6.1/ci/docker-compose-wcs.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/ci/docker-compose.yml` & `weaviate_client-4.6.1/ci/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/ci/proxy/envoy.yaml` & `weaviate_client-4.6.1/ci/proxy/envoy.yaml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/ci/start_weaviate.sh` & `weaviate_client-4.6.1/ci/start_weaviate.sh`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/docs/Makefile` & `weaviate_client-4.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/docs/README.rst` & `weaviate_client-4.6.1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/docs/changelog.rst` & `weaviate_client-4.6.1/docs/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,35 @@
 Changelog
 =========
+
+Version 4.6.1
+--------------
+This patch version includes:
+  - Fixes for ``client.integrations.configure``
+
+Version 4.6.0
+--------------
+This minor version includes:
+
+- Support for Weaviate 1.25.0:
+
+  - BM25/Hybrid support groupBy parameter
+  - Hybrid supports MoveTo/MoveAwayFrom in near_vector and near_text through HybridVector class
+  - Ollama text2vec and generative module
+  - Octoai text2vec and generative module
+  - multi2vev-palm module
+  - dynamic vector index type
+  - auto tenant creation
+  - improved batching with vectorization
+  - tenant exists endpoint
+  - get tenant by name
+
+- Added ``client.integrations.configure`` to configure api-keys and model provider parameters for integration/module-providers without setting headers.
+- Improved error messages and deprecation warnings.
+
 Version 4.5.7
 --------------
 This patch version includes:
 
 - Deprecation of the ``bit_compression`` field in the ``PQConfig`` class
 - Improvements to closing possibly open objects and connections
 - Enhances the ``WeaviateGRPCUnavailableError`` message with added context relevant to the user's environment
```

### Comparing `weaviate_client-4.6.0b3/docs/conf.py` & `weaviate_client-4.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/docs/index.rst` & `weaviate_client-4.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/docs/make.bat` & `weaviate_client-4.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/docs/weaviate.classification.rst` & `weaviate_client-4.6.1/docs/weaviate.classification.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/docs/weaviate.collections.aggregations.rst` & `weaviate_client-4.6.1/docs/weaviate.collections.aggregations.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/docs/weaviate.collections.batch.rst` & `weaviate_client-4.6.1/docs/weaviate.collections.batch.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/docs/weaviate.collections.classes.rst` & `weaviate_client-4.6.1/docs/weaviate.collections.classes.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/docs/weaviate.collections.grpc.rst` & `weaviate_client-4.6.1/docs/weaviate.collections.grpc.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/docs/weaviate.collections.queries.rst` & `weaviate_client-4.6.1/docs/weaviate.collections.queries.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/docs/weaviate.collections.rst` & `weaviate_client-4.6.1/docs/weaviate.collections.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/docs/weaviate.connect.rst` & `weaviate_client-4.6.1/docs/weaviate.connect.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/docs/weaviate.gql.rst` & `weaviate_client-4.6.1/docs/weaviate.gql.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/docs/weaviate.proto.v1.rst` & `weaviate_client-4.6.1/docs/weaviate.proto.v1.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/docs/weaviate.rst` & `weaviate_client-4.6.1/docs/weaviate.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/1234.3gp` & `weaviate_client-4.6.1/integration/1234.3gp`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/conftest.py` & `weaviate_client-4.6.1/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/constants.py` & `weaviate_client-4.6.1/integration/constants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/hobbits.mp4` & `weaviate_client-4.6.1/integration/hobbits.mp4`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_auth.py` & `weaviate_client-4.6.1/integration/test_auth.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_batch_v4.py` & `weaviate_client-4.6.1/integration/test_batch_v4.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_client.py` & `weaviate_client-4.6.1/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_collection.py` & `weaviate_client-4.6.1/integration/test_collection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_collection_aggregate.py` & `weaviate_client-4.6.1/integration/test_collection_aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_collection_batch.py` & `weaviate_client-4.6.1/integration/test_collection_batch.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_collection_batch_delete.py` & `weaviate_client-4.6.1/integration/test_collection_batch_delete.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_collection_config.py` & `weaviate_client-4.6.1/integration/test_collection_config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_collection_filter.py` & `weaviate_client-4.6.1/integration/test_collection_filter.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_collection_geo.py` & `weaviate_client-4.6.1/integration/test_collection_geo.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_collection_get.py` & `weaviate_client-4.6.1/integration/test_collection_get.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_collection_model.py` & `weaviate_client-4.6.1/integration/test_collection_model.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_collection_multi_node.py` & `weaviate_client-4.6.1/integration/test_collection_multi_node.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_collection_nested.py` & `weaviate_client-4.6.1/integration/test_collection_nested.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_collection_openai.py` & `weaviate_client-4.6.1/integration/test_collection_openai.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_collection_references.py` & `weaviate_client-4.6.1/integration/test_collection_references.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_collection_rerank.py` & `weaviate_client-4.6.1/integration/test_collection_rerank.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_gql_raw_v4.py` & `weaviate_client-4.6.1/integration/test_gql_raw_v4.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_iterator.py` & `weaviate_client-4.6.1/integration/test_iterator.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_named_vectors.py` & `weaviate_client-4.6.1/integration/test_named_vectors.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/test_tenants.py` & `weaviate_client-4.6.1/integration/test_tenants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration/weaviate-logo.png` & `weaviate_client-4.6.1/integration/weaviate-logo.png`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration_embedded/test_client.py` & `weaviate_client-4.6.1/integration_embedded/test_client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration_v3/people_schema.json` & `weaviate_client-4.6.1/integration_v3/people_schema.json`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration_v3/test_authentication.py` & `weaviate_client-4.6.1/integration_v3/test_authentication.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration_v3/test_backup.py` & `weaviate_client-4.6.1/integration_v3/test_backup.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration_v3/test_backup_v4.py` & `weaviate_client-4.6.1/integration_v3/test_backup_v4.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration_v3/test_batch.py` & `weaviate_client-4.6.1/integration_v3/test_batch.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration_v3/test_classification.py` & `weaviate_client-4.6.1/integration_v3/test_classification.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration_v3/test_cluster.py` & `weaviate_client-4.6.1/integration_v3/test_cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration_v3/test_crud.py` & `weaviate_client-4.6.1/integration_v3/test_crud.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration_v3/test_graphql.py` & `weaviate_client-4.6.1/integration_v3/test_graphql.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration_v3/test_grcp.py` & `weaviate_client-4.6.1/integration_v3/test_grcp.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration_v3/test_schema.py` & `weaviate_client-4.6.1/integration_v3/test_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration_v3/test_stress.py` & `weaviate_client-4.6.1/integration_v3/test_stress.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/integration_v3/test_timeout.py` & `weaviate_client-4.6.1/integration_v3/test_timeout.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/mock_tests/conftest.py` & `weaviate_client-4.6.1/mock_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/mock_tests/test_auth.py` & `weaviate_client-4.6.1/mock_tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/mock_tests/test_automatic_retries.py` & `weaviate_client-4.6.1/mock_tests/test_automatic_retries.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/mock_tests/test_batching_manual.py` & `weaviate_client-4.6.1/mock_tests/test_batching_manual.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/mock_tests/test_collection.py` & `weaviate_client-4.6.1/mock_tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/mock_tests/test_connection.py` & `weaviate_client-4.6.1/mock_tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/mock_tests/test_exception.py` & `weaviate_client-4.6.1/mock_tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/mock_tests/test_graphql.py` & `weaviate_client-4.6.1/mock_tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/mock_tests/test_resend.py` & `weaviate_client-4.6.1/mock_tests/test_resend.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/mock_tests/test_schema.py` & `weaviate_client-4.6.1/mock_tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/profiling/conftest.py` & `weaviate_client-4.6.1/profiling/conftest.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/profiling/constants.py` & `weaviate_client-4.6.1/profiling/constants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/profiling/test_import_and_query.py` & `weaviate_client-4.6.1/profiling/test_import_and_query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/profiling/test_profiling.py` & `weaviate_client-4.6.1/profiling/test_profiling.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/profiling/test_refs.py` & `weaviate_client-4.6.1/profiling/test_refs.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/profiling/test_sphere.py` & `weaviate_client-4.6.1/profiling/test_sphere.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/publishing.md` & `weaviate_client-4.6.1/publishing.md`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/pyproject.toml` & `weaviate_client-4.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/requirements-devel.txt` & `weaviate_client-4.6.1/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/setup.cfg` & `weaviate_client-4.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/README.md` & `weaviate_client-4.6.1/test/README.md`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/batch/test_requests.py` & `weaviate_client-4.6.1/test/batch/test_requests.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/classification/test_classification.py` & `weaviate_client-4.6.1/test/classification/test_classification.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/cluster/test_cluster.py` & `weaviate_client-4.6.1/test/cluster/test_cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/collection/test_aggregates.py` & `weaviate_client-4.6.1/test/collection/test_aggregates.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/collection/test_byteops.py` & `weaviate_client-4.6.1/test/collection/test_byteops.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/collection/test_classes.py` & `weaviate_client-4.6.1/test/collection/test_classes.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/collection/test_client.py` & `weaviate_client-4.6.1/test/collection/test_client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/collection/test_collection_model.py` & `weaviate_client-4.6.1/test/collection/test_collection_model.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/collection/test_config.py` & `weaviate_client-4.6.1/test/collection/test_config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/collection/test_filter.py` & `weaviate_client-4.6.1/test/collection/test_filter.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/collection/test_queries.py` & `weaviate_client-4.6.1/test/collection/test_queries.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/connection/test_connection.py` & `weaviate_client-4.6.1/test/connection/test_connection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/contextionary/test_text2vec_contextionary.py` & `weaviate_client-4.6.1/test/contextionary/test_text2vec_contextionary.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/data/references/test_crud_references.py` & `weaviate_client-4.6.1/test/data/references/test_crud_references.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/data/test_crud_data.py` & `weaviate_client-4.6.1/test/data/test_crud_data.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/gql/test_aggregate.py` & `weaviate_client-4.6.1/test/gql/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/gql/test_filter.py` & `weaviate_client-4.6.1/test/gql/test_filter.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/gql/test_get.py` & `weaviate_client-4.6.1/test/gql/test_get.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/gql/test_query.py` & `weaviate_client-4.6.1/test/gql/test_query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/schema/properties/test_properties.py` & `weaviate_client-4.6.1/test/schema/properties/test_properties.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/schema/schema_company.json` & `weaviate_client-4.6.1/test/schema/schema_company.json`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/schema/test_schema.py` & `weaviate_client-4.6.1/test/schema/test_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/test_auth.py` & `weaviate_client-4.6.1/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/test_client.py` & `weaviate_client-4.6.1/test/test_client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/test_embedded.py` & `weaviate_client-4.6.1/test/test_embedded.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/test_exceptions.py` & `weaviate_client-4.6.1/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/test_server_version.py` & `weaviate_client-4.6.1/test/test_server_version.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/test_util.py` & `weaviate_client-4.6.1/test/test_util.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/test/util.py` & `weaviate_client-4.6.1/test/util.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/__init__.py` & `weaviate_client-4.6.1/weaviate/__init__.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/auth.py` & `weaviate_client-4.6.1/weaviate/auth.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/backup/backup.py` & `weaviate_client-4.6.1/weaviate/backup/backup.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/batch/crud_batch.py` & `weaviate_client-4.6.1/weaviate/batch/crud_batch.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/batch/requests.py` & `weaviate_client-4.6.1/weaviate/batch/requests.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/classes/config.py` & `weaviate_client-4.6.1/weaviate/classes/config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/classes/query.py` & `weaviate_client-4.6.1/weaviate/classes/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/classification/classification.py` & `weaviate_client-4.6.1/weaviate/classification/classification.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/classification/config_builder.py` & `weaviate_client-4.6.1/weaviate/classification/config_builder.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/client.py` & `weaviate_client-4.6.1/weaviate/client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/cluster/cluster.py` & `weaviate_client-4.6.1/weaviate/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/cluster/types.py` & `weaviate_client-4.6.1/weaviate/cluster/types.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/aggregations/base.py` & `weaviate_client-4.6.1/weaviate/collections/aggregations/base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/aggregations/hybrid.py` & `weaviate_client-4.6.1/weaviate/collections/aggregations/hybrid.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/aggregations/near_image.py` & `weaviate_client-4.6.1/weaviate/collections/aggregations/near_image.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/aggregations/near_object.py` & `weaviate_client-4.6.1/weaviate/collections/aggregations/near_object.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/aggregations/near_text.py` & `weaviate_client-4.6.1/weaviate/collections/aggregations/near_text.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/aggregations/near_vector.py` & `weaviate_client-4.6.1/weaviate/collections/aggregations/near_vector.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/aggregations/over_all.py` & `weaviate_client-4.6.1/weaviate/collections/aggregations/over_all.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/backups.py` & `weaviate_client-4.6.1/weaviate/collections/backups.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/base.py` & `weaviate_client-4.6.1/weaviate/collections/base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/batch/base.py` & `weaviate_client-4.6.1/weaviate/collections/batch/base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/batch/batch_wrapper.py` & `weaviate_client-4.6.1/weaviate/collections/batch/batch_wrapper.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/batch/client.py` & `weaviate_client-4.6.1/weaviate/collections/batch/client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/batch/collection.py` & `weaviate_client-4.6.1/weaviate/collections/batch/collection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/batch/grpc_batch_delete.py` & `weaviate_client-4.6.1/weaviate/collections/batch/grpc_batch_delete.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/batch/grpc_batch_objects.py` & `weaviate_client-4.6.1/weaviate/collections/batch/grpc_batch_objects.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/batch/rest.py` & `weaviate_client-4.6.1/weaviate/collections/batch/rest.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/classes/aggregate.py` & `weaviate_client-4.6.1/weaviate/collections/classes/aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/classes/batch.py` & `weaviate_client-4.6.1/weaviate/collections/classes/batch.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/classes/cluster.py` & `weaviate_client-4.6.1/weaviate/collections/classes/cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/classes/config.py` & `weaviate_client-4.6.1/weaviate/collections/classes/config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/classes/config_base.py` & `weaviate_client-4.6.1/weaviate/collections/classes/config_base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/classes/config_methods.py` & `weaviate_client-4.6.1/weaviate/collections/classes/config_methods.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/classes/config_named_vectors.py` & `weaviate_client-4.6.1/weaviate/collections/classes/config_named_vectors.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/classes/config_vector_index.py` & `weaviate_client-4.6.1/weaviate/collections/classes/config_vector_index.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/classes/config_vectorizers.py` & `weaviate_client-4.6.1/weaviate/collections/classes/config_vectorizers.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/classes/data.py` & `weaviate_client-4.6.1/weaviate/collections/classes/data.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/classes/filters.py` & `weaviate_client-4.6.1/weaviate/collections/classes/filters.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/classes/grpc.py` & `weaviate_client-4.6.1/weaviate/collections/classes/grpc.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/classes/internal.py` & `weaviate_client-4.6.1/weaviate/collections/classes/internal.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/classes/orm.py` & `weaviate_client-4.6.1/weaviate/collections/classes/orm.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/classes/tenants.py` & `weaviate_client-4.6.1/weaviate/collections/classes/tenants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/classes/types.py` & `weaviate_client-4.6.1/weaviate/collections/classes/types.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/cluster.py` & `weaviate_client-4.6.1/weaviate/collections/cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/collection.py` & `weaviate_client-4.6.1/weaviate/collections/collection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/collections.py` & `weaviate_client-4.6.1/weaviate/collections/collections.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/config.py` & `weaviate_client-4.6.1/weaviate/collections/config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/data.py` & `weaviate_client-4.6.1/weaviate/collections/data.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/filters.py` & `weaviate_client-4.6.1/weaviate/collections/filters.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/grpc/query.py` & `weaviate_client-4.6.1/weaviate/collections/grpc/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/grpc/shared.py` & `weaviate_client-4.6.1/weaviate/collections/grpc/shared.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/grpc/tenants.py` & `weaviate_client-4.6.1/weaviate/collections/grpc/tenants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/iterator.py` & `weaviate_client-4.6.1/weaviate/collections/iterator.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/orm.py` & `weaviate_client-4.6.1/weaviate/collections/orm.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/base.py` & `weaviate_client-4.6.1/weaviate/collections/queries/base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/bm25/generate.py` & `weaviate_client-4.6.1/weaviate/collections/queries/bm25/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/bm25/generate.pyi` & `weaviate_client-4.6.1/weaviate/collections/queries/bm25/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/bm25/query.py` & `weaviate_client-4.6.1/weaviate/collections/queries/bm25/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/bm25/query.pyi` & `weaviate_client-4.6.1/weaviate/collections/queries/bm25/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/byteops.py` & `weaviate_client-4.6.1/weaviate/collections/queries/byteops.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/fetch_object_by_id/query.py` & `weaviate_client-4.6.1/weaviate/collections/queries/fetch_object_by_id/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/fetch_object_by_id/query.pyi` & `weaviate_client-4.6.1/weaviate/collections/queries/fetch_object_by_id/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/fetch_objects/generate.py` & `weaviate_client-4.6.1/weaviate/collections/queries/fetch_objects/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/fetch_objects/generate.pyi` & `weaviate_client-4.6.1/weaviate/collections/queries/fetch_objects/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/fetch_objects/query.py` & `weaviate_client-4.6.1/weaviate/collections/queries/fetch_objects/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/fetch_objects/query.pyi` & `weaviate_client-4.6.1/weaviate/collections/queries/fetch_objects/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/hybrid/generate.py` & `weaviate_client-4.6.1/weaviate/collections/queries/hybrid/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/hybrid/generate.pyi` & `weaviate_client-4.6.1/weaviate/collections/queries/hybrid/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/hybrid/query.py` & `weaviate_client-4.6.1/weaviate/collections/queries/hybrid/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/hybrid/query.pyi` & `weaviate_client-4.6.1/weaviate/collections/queries/hybrid/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/near_image/generate.py` & `weaviate_client-4.6.1/weaviate/collections/queries/near_image/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/near_image/generate.pyi` & `weaviate_client-4.6.1/weaviate/collections/queries/near_image/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/near_image/query.py` & `weaviate_client-4.6.1/weaviate/collections/queries/near_image/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/near_image/query.pyi` & `weaviate_client-4.6.1/weaviate/collections/queries/near_image/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/near_media/generate.py` & `weaviate_client-4.6.1/weaviate/collections/queries/near_media/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/near_media/generate.pyi` & `weaviate_client-4.6.1/weaviate/collections/queries/near_media/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/near_media/query.py` & `weaviate_client-4.6.1/weaviate/collections/queries/near_media/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/near_media/query.pyi` & `weaviate_client-4.6.1/weaviate/collections/queries/near_media/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/near_object/generate.py` & `weaviate_client-4.6.1/weaviate/collections/queries/near_object/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/near_object/generate.pyi` & `weaviate_client-4.6.1/weaviate/collections/queries/near_object/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/near_object/query.py` & `weaviate_client-4.6.1/weaviate/collections/queries/near_object/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/near_object/query.pyi` & `weaviate_client-4.6.1/weaviate/collections/queries/near_object/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/near_text/generate.py` & `weaviate_client-4.6.1/weaviate/collections/queries/near_text/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/near_text/generate.pyi` & `weaviate_client-4.6.1/weaviate/collections/queries/near_text/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/near_text/query.py` & `weaviate_client-4.6.1/weaviate/collections/queries/near_text/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/near_text/query.pyi` & `weaviate_client-4.6.1/weaviate/collections/queries/near_text/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/near_vector/generate.py` & `weaviate_client-4.6.1/weaviate/collections/queries/near_vector/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/near_vector/generate.pyi` & `weaviate_client-4.6.1/weaviate/collections/queries/near_vector/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/near_vector/query.py` & `weaviate_client-4.6.1/weaviate/collections/queries/near_vector/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/queries/near_vector/query.pyi` & `weaviate_client-4.6.1/weaviate/collections/queries/near_vector/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/query.py` & `weaviate_client-4.6.1/weaviate/collections/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/collections/tenants.py` & `weaviate_client-4.6.1/weaviate/collections/tenants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/config.py` & `weaviate_client-4.6.1/weaviate/config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/connect/authentication.py` & `weaviate_client-4.6.1/weaviate/connect/authentication.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/connect/base.py` & `weaviate_client-4.6.1/weaviate/connect/base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/connect/helpers.py` & `weaviate_client-4.6.1/weaviate/connect/helpers.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/connect/integrations.py` & `weaviate_client-4.6.1/weaviate/connect/integrations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Dict, Optional, cast
+
 from pydantic import BaseModel, ConfigDict, Field
 
 
 class _IntegrationConfig(BaseModel):
     model_config = ConfigDict(strict=True)
 
     def _to_header(self) -> Dict[str, str]:
@@ -61,19 +62,19 @@
     requests_per_minute_embeddings: Optional[int] = Field(
         serialization_alias="X-Jinaai-Ratelimit-RequestPM-Embedding"
     )
     base_url: Optional[str] = Field(serialization_alias="X-Jinaai-Baseurl")
 
 
 class _IntegrationConfigOcto(_IntegrationConfig):
-    api_key: str = Field(serialization_alias="X-Octoai-Api-Key")
+    api_key: str = Field(serialization_alias="X-OctoAI-Api-Key")
     requests_per_minute_embeddings: Optional[int] = Field(
-        serialization_alias="X-Octoai-Ratelimit-RequestPM-Embedding"
+        serialization_alias="X-OctoAI-Ratelimit-RequestPM-Embedding"
     )
-    base_url: Optional[str] = Field(serialization_alias="X-Octoai-Baseurl")
+    base_url: Optional[str] = Field(serialization_alias="X-OctoAI-Baseurl")
 
 
 class Integrations:
     @staticmethod
     def cohere(
         *,
         api_key: str,
```

### Comparing `weaviate_client-4.6.0b3/weaviate/connect/v3.py` & `weaviate_client-4.6.1/weaviate/connect/v3.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/connect/v4.py` & `weaviate_client-4.6.1/weaviate/connect/v4.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from weaviate.connect.authentication import _Auth
 from weaviate.connect.base import (
     _ConnectionBase,
     ConnectionParams,
     JSONPayload,
     _get_proxies,
 )
+from weaviate.connect.integrations import _IntegrationConfig
 from weaviate.embedded import EmbeddedV4
 from weaviate.exceptions import (
     AuthenticationFailedError,
     UnexpectedStatusCodeError,
     WeaviateGRPCUnavailableError,
     WeaviateStartUpError,
     WeaviateClosedClientError,
@@ -56,16 +57,14 @@
     PYPI_PACKAGE_URL,
     _decode_json_response_dict,
     _ServerVersion,
 )
 from weaviate.validator import _ValidateArgument, _validate_input
 from weaviate.warnings import _Warnings
 
-from weaviate.connect.integrations import _IntegrationConfig
-
 Session = Union[Client, OAuth2Client]
 AsyncSession = Union[AsyncClient, AsyncOAuth2Client]
 
 
 @dataclass
 class _ExpectedStatusCodes:
     ok_in: Union[List[int], int]
@@ -615,17 +614,17 @@
             timeout_config,
             proxies,
             trust_env,
             additional_headers,
             connection_config,
             embedded_db,
         )
-        self.__prepare_grpc_headers()
+        self._prepare_grpc_headers()
 
-    def __prepare_grpc_headers(self) -> None:
+    def _prepare_grpc_headers(self) -> None:
         self.__metadata_list: List[Tuple[str, str]] = []
         if len(self.additional_headers):
             for key, val in self.additional_headers.items():
                 if val is not None:
                     self.__metadata_list.append((key.lower(), val))
 
         if self._auth is not None:
```

### Comparing `weaviate_client-4.6.0b3/weaviate/contextionary/crud_contextionary.py` & `weaviate_client-4.6.1/weaviate/contextionary/crud_contextionary.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/data/crud_data.py` & `weaviate_client-4.6.1/weaviate/data/crud_data.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/data/references/crud_references.py` & `weaviate_client-4.6.1/weaviate/data/references/crud_references.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/embedded.py` & `weaviate_client-4.6.1/weaviate/embedded.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/error_msgs.py` & `weaviate_client-4.6.1/weaviate/error_msgs.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/exceptions.py` & `weaviate_client-4.6.1/weaviate/exceptions.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/gql/aggregate.py` & `weaviate_client-4.6.1/weaviate/gql/aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/gql/filter.py` & `weaviate_client-4.6.1/weaviate/gql/filter.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/gql/get.py` & `weaviate_client-4.6.1/weaviate/gql/get.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/gql/multi_get.py` & `weaviate_client-4.6.1/weaviate/gql/multi_get.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/gql/query.py` & `weaviate_client-4.6.1/weaviate/gql/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/integrations.py` & `weaviate_client-4.6.1/weaviate/integrations.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,7 +10,8 @@
 
     def configure(
         self, integrations_config: Union[_IntegrationConfig, List[_IntegrationConfig]]
     ) -> None:
         if isinstance(integrations_config, _IntegrationConfig):
             integrations_config = [integrations_config]
         self.__connection.set_integrations(integrations_config)
+        self.__connection._prepare_grpc_headers()
```

### Comparing `weaviate_client-4.6.0b3/weaviate/outputs/aggregate.py` & `weaviate_client-4.6.1/weaviate/outputs/aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/outputs/config.py` & `weaviate_client-4.6.1/weaviate/outputs/config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/outputs/query.py` & `weaviate_client-4.6.1/weaviate/outputs/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/proto/v1/base_pb2.py` & `weaviate_client-4.6.1/weaviate/proto/v1/base_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/proto/v1/base_pb2.pyi` & `weaviate_client-4.6.1/weaviate/proto/v1/base_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/proto/v1/batch_delete_pb2.py` & `weaviate_client-4.6.1/weaviate/proto/v1/batch_delete_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/proto/v1/batch_delete_pb2.pyi` & `weaviate_client-4.6.1/weaviate/proto/v1/batch_delete_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/proto/v1/batch_pb2.py` & `weaviate_client-4.6.1/weaviate/proto/v1/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/proto/v1/batch_pb2.pyi` & `weaviate_client-4.6.1/weaviate/proto/v1/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/proto/v1/properties_pb2.py` & `weaviate_client-4.6.1/weaviate/proto/v1/properties_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/proto/v1/properties_pb2.pyi` & `weaviate_client-4.6.1/weaviate/proto/v1/properties_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/proto/v1/search_get_pb2.py` & `weaviate_client-4.6.1/weaviate/proto/v1/search_get_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/proto/v1/search_get_pb2.pyi` & `weaviate_client-4.6.1/weaviate/proto/v1/search_get_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/proto/v1/tenants_pb2.py` & `weaviate_client-4.6.1/weaviate/proto/v1/tenants_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/proto/v1/tenants_pb2.pyi` & `weaviate_client-4.6.1/weaviate/proto/v1/tenants_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/proto/v1/weaviate_pb2.py` & `weaviate_client-4.6.1/weaviate/proto/v1/weaviate_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/proto/v1/weaviate_pb2_grpc.py` & `weaviate_client-4.6.1/weaviate/proto/v1/weaviate_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/schema/crud_schema.py` & `weaviate_client-4.6.1/weaviate/schema/crud_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/schema/properties/crud_properties.py` & `weaviate_client-4.6.1/weaviate/schema/properties/crud_properties.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/types.py` & `weaviate_client-4.6.1/weaviate/types.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/util.py` & `weaviate_client-4.6.1/weaviate/util.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/validator.py` & `weaviate_client-4.6.1/weaviate/validator.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b3/weaviate/warnings.py` & `weaviate_client-4.6.1/weaviate/warnings.py`

 * *Files 6% similar despite different names*

```diff
@@ -152,17 +152,20 @@
             DeprecationWarning,
             stacklevel=2,  # don't increase stacklevel, as this otherwise writes the auth-secrets into the log
         )
 
     @staticmethod
     def weaviate_v3_client_is_deprecated() -> None:
         warnings.warn(
-            message="""Dep016: You are using the Weaviate v3 client, which is deprecated.
-            Consider upgrading to the new and improved v4 client instead!
-            See here for usage: https://weaviate.io/developers/weaviate/client-libraries/python
+            message="""Dep016: You are creating a Weaviate v3 client using `client =  weaviate.Client(...)`, which is
+            deprecated. Consider creating a v4 (`weaviate.WeaviateClient`) client, using a `weaviate.connect_to_<method>`
+            helper function.
+            See here for
+                - migrating from v3 to v4: https://weaviate.io/developers/weaviate/client-libraries/python/v3_v4_migration
+                - general v4 usage: https://weaviate.io/developers/weaviate/client-libraries/python
             """,
             category=DeprecationWarning,
             stacklevel=1,
         )
 
     @staticmethod
     def vector_index_config_in_config_update() -> None:
```

### Comparing `weaviate_client-4.6.0b3/weaviate_client.egg-info/PKG-INFO` & `weaviate_client-4.6.1/weaviate_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weaviate-client
-Version: 4.6.0b3
+Version: 4.6.1
 Summary: A python native Weaviate client
 Home-page: https://github.com/weaviate/weaviate-python-client
 Author: Weaviate
 Author-email: hello@weaviate.io,
 License: BSD 3-clause
 Project-URL: Documentation, https://weaviate-python-client.readthedocs.io
 Project-URL: Source, https://github.com/weaviate/weaviate-python-client
```

### Comparing `weaviate_client-4.6.0b3/weaviate_client.egg-info/SOURCES.txt` & `weaviate_client-4.6.1/weaviate_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

