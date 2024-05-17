# Comparing `tmp/x10_python_trading-0.1.3.tar.gz` & `tmp/x10_python_trading-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x10_python_trading-0.1.3.tar", max compression
+gzip compressed data, was "x10_python_trading-0.2.0.tar", max compression
```

## Comparing `x10_python_trading-0.1.3.tar` & `x10_python_trading-0.2.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0     5537 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/README.md
--rw-r--r--   0        0        0     1541 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/__init__.py
--rw-r--r--   0        0        0     3945 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/signature/README.md
--rw-r--r--   0        0        0        0 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/signature/__init__.py
--rw-r--r--   0        0        0     1840 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/signature/fast_pedersen_hash.py
--rw-r--r--   0        0        0     3627 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/signature/math_utils.py
--rw-r--r--   0        0        0     6074 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/signature/nothing_up_my_sleeve_gen.py
--rw-r--r--   0        0        0   102708 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/signature/pedersen_params.json
--rw-r--r--   0        0        0    11728 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/signature/signature.py
--rw-r--r--   0        0        0     3759 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/signature/src/config/assets_precomputed.json
--rw-r--r--   0        0        0    70705 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/signature/src/config/constant_points.json
--rw-r--r--   0        0        0     3701 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/crypto/signature/src/config/keys_precomputed.json
--rw-r--r--   0        0        0     1955 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/BUILD
--rw-r--r--   0        0        0       31 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/CMakeLists.txt
--rw-r--r--   0        0        0     1254 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/CMakeLists_common.txt
--rw-r--r--   0        0        0        0 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/__init__.py
--rw-r--r--   0        0        0     1522 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/async_subprocess.py
--rw-r--r--   0        0        0     5946 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/expression_string.py
--rw-r--r--   0        0        0     1883 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/expression_string_test.py
--rw-r--r--   0        0        0     3938 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/fixed_point.py
--rw-r--r--   0        0        0      675 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/json_rpc/BUILD
--rw-r--r--   0        0        0      359 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/json_rpc/CMakeLists.txt
--rw-r--r--   0        0        0      812 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/json_rpc/client.py
--rw-r--r--   0        0        0      681 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/json_rpc/client_test.py
--rw-r--r--   0        0        0     8881 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/math_utils.py
--rw-r--r--   0        0        0     5102 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/math_utils_test.py
--rw-r--r--   0        0        0     1614 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/merkle_tree.py
--rw-r--r--   0        0        0     1796 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/object_utils.py
--rw-r--r--   0        0        0     1545 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/python_dependencies.py
--rw-r--r--   0        0        0     6247 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/random_test.py
--rw-r--r--   0        0        0     6247 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/random_test_utils.py
--rw-r--r--   0        0        0     3460 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/test_utils.py
--rw-r--r--   0        0        0     2783 2024-05-15 16:59:29.254255 x10_python_trading-0.1.3/starkware/python/test_utils_test.py
--rw-r--r--   0        0        0    19817 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/starkware/python/utils.py
--rw-r--r--   0        0        0      599 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/starkware/python/utils_stub_module.py
--rw-r--r--   0        0        0     1554 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/starkware/python/utils_stub_module.pyi
--rw-r--r--   0        0        0     7959 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/starkware/python/utils_test.py
--rw-r--r--   0        0        0        0 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/__init__.py
--rw-r--r--   0        0        0      429 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/config.py
--rw-r--r--   0        0        0       36 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/errors.py
--rw-r--r--   0        0        0        0 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/__init__.py
--rw-r--r--   0        0        0     1575 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/accounts.py
--rw-r--r--   0        0        0     1618 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/amounts.py
--rw-r--r--   0        0        0     1120 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/assets.py
--rw-r--r--   0        0        0      347 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/balances.py
--rw-r--r--   0        0        0      427 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/configuration.py
--rw-r--r--   0        0        0      327 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/fees.py
--rw-r--r--   0        0        0      459 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/funding_rates.py
--rw-r--r--   0        0        0     2744 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/markets.py
--rw-r--r--   0        0        0     4461 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/order_object.py
--rw-r--r--   0        0        0      739 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/orderbooks.py
--rw-r--r--   0        0        0     2207 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/orders.py
--rw-r--r--   0        0        0     1069 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/positions.py
--rw-r--r--   0        0        0     4227 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/simple_client/simple_trading_client.py
--rw-r--r--   0        0        0       99 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/stream_client/__init__.py
--rw-r--r--   0        0        0     2974 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/stream_client/perpetual_stream_connection.py
--rw-r--r--   0        0        0     2497 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/stream_client/stream_client.py
--rw-r--r--   0        0        0     1241 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/trades.py
--rw-r--r--   0        0        0      102 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/trading_client/__init__.py
--rw-r--r--   0        0        0     4996 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/trading_client/account_module.py
--rw-r--r--   0        0        0      636 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/trading_client/base_module.py
--rw-r--r--   0        0        0     1499 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/trading_client/markets_information_module.py
--rw-r--r--   0        0        0     2353 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/trading_client/order_management_module.py
--rw-r--r--   0        0        0     2953 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/perpetual/trading_client/trading_client.py
--rw-r--r--   0        0        0        0 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/utils/__init__.py
--rw-r--r--   0        0        0      246 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/utils/date.py
--rw-r--r--   0        0        0     5981 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/utils/http.py
--rw-r--r--   0        0        0       79 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/utils/log.py
--rw-r--r--   0        0        0     2336 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/utils/model.py
--rw-r--r--   0        0        0    14980 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/utils/starkex.py
--rw-r--r--   0        0        0      275 2024-05-15 16:59:29.258255 x10_python_trading-0.1.3/x10/utils/string.py
--rw-r--r--   0        0        0     6491 1970-01-01 00:00:00.000000 x10_python_trading-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     7819 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/README.md
+-rw-r--r--   0        0        0     1541 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/__init__.py
+-rw-r--r--   0        0        0     3945 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/signature/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/signature/__init__.py
+-rw-r--r--   0        0        0     1840 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/signature/fast_pedersen_hash.py
+-rw-r--r--   0        0        0     3627 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/signature/math_utils.py
+-rw-r--r--   0        0        0     6074 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/signature/nothing_up_my_sleeve_gen.py
+-rw-r--r--   0        0        0   102708 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/signature/pedersen_params.json
+-rw-r--r--   0        0        0    11728 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/signature/signature.py
+-rw-r--r--   0        0        0     3759 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/signature/src/config/assets_precomputed.json
+-rw-r--r--   0        0        0    70705 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/signature/src/config/constant_points.json
+-rw-r--r--   0        0        0     3701 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/signature/src/config/keys_precomputed.json
+-rw-r--r--   0        0        0     1955 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/python/BUILD
+-rw-r--r--   0        0        0       31 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/python/CMakeLists.txt
+-rw-r--r--   0        0        0     1254 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/python/CMakeLists_common.txt
+-rw-r--r--   0        0        0        0 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/python/__init__.py
+-rw-r--r--   0        0        0     1522 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/python/async_subprocess.py
+-rw-r--r--   0        0        0     5946 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/expression_string.py
+-rw-r--r--   0        0        0     1883 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/expression_string_test.py
+-rw-r--r--   0        0        0     3938 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/fixed_point.py
+-rw-r--r--   0        0        0      675 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/json_rpc/BUILD
+-rw-r--r--   0        0        0      359 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/json_rpc/CMakeLists.txt
+-rw-r--r--   0        0        0      812 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/json_rpc/client.py
+-rw-r--r--   0        0        0      681 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/json_rpc/client_test.py
+-rw-r--r--   0        0        0     8881 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/math_utils.py
+-rw-r--r--   0        0        0     5102 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/math_utils_test.py
+-rw-r--r--   0        0        0     1614 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/merkle_tree.py
+-rw-r--r--   0        0        0     1796 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/object_utils.py
+-rw-r--r--   0        0        0     1545 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/python_dependencies.py
+-rw-r--r--   0        0        0     6247 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/random_test.py
+-rw-r--r--   0        0        0     6247 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/random_test_utils.py
+-rw-r--r--   0        0        0     3460 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/test_utils.py
+-rw-r--r--   0        0        0     2783 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/test_utils_test.py
+-rw-r--r--   0        0        0    19817 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/utils.py
+-rw-r--r--   0        0        0      599 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/utils_stub_module.py
+-rw-r--r--   0        0        0     1554 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/utils_stub_module.pyi
+-rw-r--r--   0        0        0     7959 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/utils_test.py
+-rw-r--r--   0        0        0        0 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/__init__.py
+-rw-r--r--   0        0        0      429 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/config.py
+-rw-r--r--   0        0        0       36 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/errors.py
+-rw-r--r--   0        0        0        0 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/__init__.py
+-rw-r--r--   0        0        0     1575 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/accounts.py
+-rw-r--r--   0        0        0     1618 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/amounts.py
+-rw-r--r--   0        0        0     1120 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/assets.py
+-rw-r--r--   0        0        0      347 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/balances.py
+-rw-r--r--   0        0        0      427 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/configuration.py
+-rw-r--r--   0        0        0      327 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/fees.py
+-rw-r--r--   0        0        0      459 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/funding_rates.py
+-rw-r--r--   0        0        0     2744 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/markets.py
+-rw-r--r--   0        0        0     4461 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/order_object.py
+-rw-r--r--   0        0        0      739 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/orderbooks.py
+-rw-r--r--   0        0        0     3058 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/orders.py
+-rw-r--r--   0        0        0     1069 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/positions.py
+-rw-r--r--   0        0        0     4227 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/simple_client/simple_trading_client.py
+-rw-r--r--   0        0        0       99 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/stream_client/__init__.py
+-rw-r--r--   0        0        0     2974 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/stream_client/perpetual_stream_connection.py
+-rw-r--r--   0        0        0     2497 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/stream_client/stream_client.py
+-rw-r--r--   0        0        0     1271 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/trades.py
+-rw-r--r--   0        0        0      102 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/trading_client/__init__.py
+-rw-r--r--   0        0        0     5214 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/trading_client/account_module.py
+-rw-r--r--   0        0        0      636 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/trading_client/base_module.py
+-rw-r--r--   0        0        0     1499 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/trading_client/markets_information_module.py
+-rw-r--r--   0        0        0     2353 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/trading_client/order_management_module.py
+-rw-r--r--   0        0        0     2953 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/trading_client/trading_client.py
+-rw-r--r--   0        0        0        0 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/utils/__init__.py
+-rw-r--r--   0        0        0      246 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/utils/date.py
+-rw-r--r--   0        0        0     5981 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/utils/http.py
+-rw-r--r--   0        0        0       79 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/utils/log.py
+-rw-r--r--   0        0        0     2336 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/utils/model.py
+-rw-r--r--   0        0        0    14980 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/utils/starkex.py
+-rw-r--r--   0        0        0      275 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/utils/string.py
+-rw-r--r--   0        0        0     8773 1970-01-01 00:00:00.000000 x10_python_trading-0.2.0/PKG-INFO
```

### Comparing `x10_python_trading-0.1.3/pyproject.toml` & `x10_python_trading-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "x10-python-trading"
-version = "0.1.3"
+version = "0.2.0"
 description = "Python client for X10 API"
 authors = ["X10 <tech@ex10.org>"]
 packages = [
     { include = "starkware" },
     { include = "x10" },
 ]
 readme = "README.md"
```

### Comparing `x10_python_trading-0.1.3/starkware/crypto/signature/README.md` & `x10_python_trading-0.2.0/starkware/crypto/signature/README.md`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/crypto/signature/fast_pedersen_hash.py` & `x10_python_trading-0.2.0/starkware/crypto/signature/fast_pedersen_hash.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/crypto/signature/math_utils.py` & `x10_python_trading-0.2.0/starkware/crypto/signature/math_utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/crypto/signature/nothing_up_my_sleeve_gen.py` & `x10_python_trading-0.2.0/starkware/crypto/signature/nothing_up_my_sleeve_gen.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/crypto/signature/pedersen_params.json` & `x10_python_trading-0.2.0/starkware/crypto/signature/pedersen_params.json`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/crypto/signature/signature.py` & `x10_python_trading-0.2.0/starkware/crypto/signature/signature.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/crypto/signature/src/config/assets_precomputed.json` & `x10_python_trading-0.2.0/starkware/crypto/signature/src/config/assets_precomputed.json`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/crypto/signature/src/config/constant_points.json` & `x10_python_trading-0.2.0/starkware/crypto/signature/src/config/constant_points.json`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/crypto/signature/src/config/keys_precomputed.json` & `x10_python_trading-0.2.0/starkware/crypto/signature/src/config/keys_precomputed.json`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/BUILD` & `x10_python_trading-0.2.0/starkware/python/BUILD`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/CMakeLists_common.txt` & `x10_python_trading-0.2.0/starkware/python/CMakeLists_common.txt`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/async_subprocess.py` & `x10_python_trading-0.2.0/starkware/python/async_subprocess.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/expression_string.py` & `x10_python_trading-0.2.0/starkware/python/expression_string.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/expression_string_test.py` & `x10_python_trading-0.2.0/starkware/python/expression_string_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/fixed_point.py` & `x10_python_trading-0.2.0/starkware/python/fixed_point.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/json_rpc/BUILD` & `x10_python_trading-0.2.0/starkware/python/json_rpc/BUILD`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/json_rpc/client.py` & `x10_python_trading-0.2.0/starkware/python/json_rpc/client.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/json_rpc/client_test.py` & `x10_python_trading-0.2.0/starkware/python/json_rpc/client_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/math_utils.py` & `x10_python_trading-0.2.0/starkware/python/math_utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/math_utils_test.py` & `x10_python_trading-0.2.0/starkware/python/math_utils_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/merkle_tree.py` & `x10_python_trading-0.2.0/starkware/python/merkle_tree.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/object_utils.py` & `x10_python_trading-0.2.0/starkware/python/object_utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/python_dependencies.py` & `x10_python_trading-0.2.0/starkware/python/python_dependencies.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/random_test.py` & `x10_python_trading-0.2.0/starkware/python/random_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/random_test_utils.py` & `x10_python_trading-0.2.0/starkware/python/random_test_utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/test_utils.py` & `x10_python_trading-0.2.0/starkware/python/test_utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/test_utils_test.py` & `x10_python_trading-0.2.0/starkware/python/test_utils_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/utils.py` & `x10_python_trading-0.2.0/starkware/python/utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/utils_stub_module.py` & `x10_python_trading-0.2.0/starkware/python/utils_stub_module.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/utils_stub_module.pyi` & `x10_python_trading-0.2.0/starkware/python/utils_stub_module.pyi`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/starkware/python/utils_test.py` & `x10_python_trading-0.2.0/starkware/python/utils_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/x10/perpetual/accounts.py` & `x10_python_trading-0.2.0/x10/perpetual/accounts.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/x10/perpetual/amounts.py` & `x10_python_trading-0.2.0/x10/perpetual/amounts.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/x10/perpetual/assets.py` & `x10_python_trading-0.2.0/x10/perpetual/assets.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/x10/perpetual/markets.py` & `x10_python_trading-0.2.0/x10/perpetual/markets.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/x10/perpetual/order_object.py` & `x10_python_trading-0.2.0/x10/perpetual/order_object.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/x10/perpetual/orderbooks.py` & `x10_python_trading-0.2.0/x10/perpetual/orderbooks.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/x10/perpetual/orders.py` & `x10_python_trading-0.2.0/x10/perpetual/orders.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,22 +22,44 @@
     TPSL = "TPSL"
     MARKET = "MARKET"
 
 
 class OrderStatus(Enum):
     UNKNOWN = "UNKNOWN"
     NEW = "NEW"
-    PENDING = "PENDING"
+    UNTRIGGERED = "UNTRIGGERED"
     PARTIALLY_FILLED = "PARTIALLY_FILLED"
     FILLED = "FILLED"
     CANCELLED = "CANCELLED"
     EXPIRED = "EXPIRED"
     REJECTED = "REJECTED"
 
 
+class OrderStatusReason(Enum):
+    NONE = "NONE"
+    UNKNOWN = "UNKNOWN"
+    UNKNOWN_MARKET = "UNKNOWN_MARKET"
+    DISABLED_MARKET = "DISABLED_MARKET"
+    NOT_ENOUGH_FUNDS = "NOT_ENOUGH_FUNDS"
+    NO_LIQUIDITY = "NO_LIQUIDITY"
+    INVALID_FEE = "INVALID_FEE"
+    INVALID_QTY = "INVALID_QTY"
+    INVALID_PRICE = "INVALID_PRICE"
+    INVALID_VALUE = "INVALID_VALUE"
+    UNKNOWN_ACCOUNT = "UNKNOWN_ACCOUNT"
+    SELF_TRADE_PROTECTION = "SELF_TRADE_PROTECTION"
+    POST_ONLY_FAILED = "POST_ONLY_FAILED"
+    REDUCE_ONLY_FAILED = "REDUCE_ONLY_FAILED"
+    INVALID_EXPIRE_TIME = "INVALID_EXPIRE_TIME"
+    POSITION_TPSL_CONFLICT = "POSITION_TPSL_CONFLICT"
+    INVALID_LEVERAGE = "INVALID_LEVERAGE"
+    PREV_ORDER_NOT_FOUND = "PREV_ORDER_NOT_FOUND"
+    PREV_ORDER_TRIGGERED = "PREV_ORDER_TRIGGERED"
+
+
 class SignatureModel(X10BaseModel):
     r: HexValue
     s: HexValue
 
 
 class StarkSettlementModel(X10BaseModel):
     signature: SignatureModel
@@ -85,14 +107,15 @@
     id: int
     account_id: int
     external_id: str
     market: str
     type: OrderType
     side: OrderSide
     status: OrderStatus
+    status_reason: Optional[OrderStatusReason] = None
     price: Decimal
     average_price: Optional[Decimal] = None
     qty: Decimal
     filled_qty: Optional[Decimal] = None
     reduce_only: bool
     post_only: bool
     created_time: int
```

### Comparing `x10_python_trading-0.1.3/x10/perpetual/positions.py` & `x10_python_trading-0.2.0/x10/perpetual/positions.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/x10/perpetual/simple_client/simple_trading_client.py` & `x10_python_trading-0.2.0/x10/perpetual/simple_client/simple_trading_client.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/x10/perpetual/stream_client/perpetual_stream_connection.py` & `x10_python_trading-0.2.0/x10/perpetual/stream_client/perpetual_stream_connection.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/x10/perpetual/stream_client/stream_client.py` & `x10_python_trading-0.2.0/x10/perpetual/stream_client/stream_client.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/x10/perpetual/trades.py` & `x10_python_trading-0.2.0/x10/perpetual/trades.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from x10.perpetual.orders import OrderSide
 from x10.utils.model import X10BaseModel
 
 
 class TradeType(Enum):
     TRADE = "TRADE"
     LIQUIDATION = "LIQUIDATION"
+    DELEVERAGE = "DELEVERAGE"
 
 
 class PublicTradeModel(X10BaseModel):
     id: int = Field(validation_alias=AliasChoices("id", "i"), serialization_alias="i")
     market: str = Field(validation_alias=AliasChoices("market", "m"), serialization_alias="m")
     side: OrderSide = Field(validation_alias=AliasChoices("side", "S"), serialization_alias="S")
     trade_type: TradeType = Field(validation_alias=AliasChoices("trade_type", "tT"), serialization_alias="tT")
```

### Comparing `x10_python_trading-0.1.3/x10/perpetual/trading_client/account_module.py` & `x10_python_trading-0.2.0/x10/perpetual/trading_client/account_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,22 +31,24 @@
         url = self._get_url("/user/positions", query={"market": market_names, "side": position_side})
         return await send_get_request(url, List[PositionModel], api_key=self._get_api_key())
 
     async def get_positions_history(
         self,
         market_names: Optional[List[str]] = None,
         position_side: Optional[PositionSide] = None,
+        cursor: Optional[int] = None,
+        limit: Optional[int] = None,
     ) -> WrappedApiResponse[List[PositionHistoryModel]]:
         """
         https://x101.docs.apiary.io/#reference/0/account/get-positions-history
         """
 
         url = self._get_url(
             "/user/positions/history",
-            query={"market": market_names, "side": position_side},
+            query={"market": market_names, "side": position_side, "cursor": cursor, "limit": limit},
         )
         return await send_get_request(url, List[PositionHistoryModel], api_key=self._get_api_key())
 
     async def get_open_orders(
         self,
         market_names: Optional[List[str]] = None,
         order_type: Optional[OrderType] = None,
@@ -63,22 +65,24 @@
         return await send_get_request(url, List[OpenOrderModel], api_key=self._get_api_key())
 
     async def get_orders_history(
         self,
         market_names: Optional[List[str]] = None,
         order_type: Optional[OrderType] = None,
         order_side: Optional[OrderSide] = None,
+        cursor: Optional[int] = None,
+        limit: Optional[int] = None,
     ) -> WrappedApiResponse[List[OpenOrderModel]]:
         """
         https://x101.docs.apiary.io/#reference/0/account/get-orders-history
         """
 
         url = self._get_url(
             "/user/orders/history",
-            query={"market": market_names, "type": order_type, "side": order_side},
+            query={"market": market_names, "type": order_type, "side": order_side, "cursor": cursor, "limit": limit},
         )
         return await send_get_request(url, List[OpenOrderModel], api_key=self._get_api_key())
 
     async def get_trades(
         self,
         market_names: List[str],
         trade_side: Optional[OrderSide] = None,
```

### Comparing `x10_python_trading-0.1.3/x10/perpetual/trading_client/base_module.py` & `x10_python_trading-0.2.0/x10/perpetual/trading_client/base_module.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/x10/perpetual/trading_client/markets_information_module.py` & `x10_python_trading-0.2.0/x10/perpetual/trading_client/markets_information_module.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/x10/perpetual/trading_client/order_management_module.py` & `x10_python_trading-0.2.0/x10/perpetual/trading_client/order_management_module.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/x10/perpetual/trading_client/trading_client.py` & `x10_python_trading-0.2.0/x10/perpetual/trading_client/trading_client.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/x10/utils/http.py` & `x10_python_trading-0.2.0/x10/utils/http.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/x10/utils/model.py` & `x10_python_trading-0.2.0/x10/utils/model.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/x10/utils/starkex.py` & `x10_python_trading-0.2.0/x10/utils/starkex.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.1.3/PKG-INFO` & `x10_python_trading-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x10-python-trading
-Version: 0.1.3
+Version: 0.2.0
 Summary: Python client for X10 API
 Author: X10
 Author-email: tech@ex10.org
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -90,15 +90,17 @@
     price=Decimal("63000.1"),
     side=OrderSide.SELL,
 )
 await trading_client.orders.cancel_order(order_id=placed_order.id)
 print(placed_order)
 ```
 
-for more information see [placing an order example](examples/placed_order_example_simple.py)
+for more information see [placing an order example](examples/placed_order_example_simple.py).
+
+There is also a skeleton implementation of a [blocking client](examples/simple_client_example.py).
 
 ## Modules
 
 The SDK currently provides functionality across three main modules
 
 ### Order Management Module 
 The order module is accessed using the `orders` property of the trading client
@@ -129,41 +131,113 @@
 
 ```python
     logger = logging.getLogger("demo_logger")
     positions = await trading_client.account.get_positions()
     logger.info("Positions: %s", positions.to_pretty_json())
 ```
 
+returns a list of
+```python
+class PositionModel(X10BaseModel):
+    id: int
+    account_id: int
+    market: str
+    side: PositionSide
+    leverage: Decimal
+    size: Decimal
+    value: Decimal
+    open_price: Decimal
+    mark_price: Decimal
+    liquidation_price: Optional[Decimal] = None
+    unrealised_pnl: Decimal
+    realised_pnl: Decimal
+    tp_price: Optional[Decimal] = None
+    sl_price: Optional[Decimal] = None
+    adl: Optional[int] = None
+    created_at: int
+    updated_at: int
+```
+
 #### `get_positions_history`
 Fetches the historical positions of the user's account. It can filter the positions based on market names and position side.
 
 ```python
-pass
+    logger = logging.getLogger("demo_logger")
+    positions = await trading_client.account.get_positions_history()
+    logger.info("Positions: %s", positions.to_pretty_json())
+```
+
+returns a list of 
+```python
+class PositionHistoryModel(X10BaseModel):
+    id: int
+    account_id: int
+    market: str
+    side: PositionSide
+    leverage: Decimal
+    size: Decimal
+    open_price: Decimal
+    exit_type: Optional[ExitType]
+    exit_price: Optional[Decimal]
+    realised_pnl: Decimal
+    created_time: int
+    closed_time: Optional[int]
 ```
 
 #### `get_open_orders`
 Fetches the open orders of the user's account. It can filter the orders based on market names, order type, and order side.
 
 ```python
     open_orders = await trading_client.account.get_open_orders()
     await trading_client.orders.mass_cancel(order_ids=[order.id for order in open_orders.data])
 ```
+returns a list of
+```python 
+class OpenOrderModel(X10BaseModel):
+    id: int
+    account_id: int
+    external_id: str
+    market: str
+    type: OrderType
+    side: OrderSide
+    status: OrderStatus
+    status_reason: Optional[OrderStatusReason] = None
+    price: Decimal
+    average_price: Optional[Decimal] = None
+    qty: Decimal
+    filled_qty: Optional[Decimal] = None
+    reduce_only: bool
+    post_only: bool
+    created_time: int
+    expiry_time: Optional[int] = None
+```
 
 #### `get_orders_history`
-Fetches the historical orders of the user's account. It can filter the orders based on market names, order type, and order side.
+Fetches the historical orders of the user's account. It can filter the orders based on market names, order type, and order side
 
 ```python
-pass
+    market_names: Optional[List[str]] = None, #parameter to filter by market
+    order_type: Optional[OrderType] = None, #parameter to filter by order type (IOC, GTT etc)
+    order_side: Optional[OrderSide] = None, #parameter to filter by side (BUY/SELL)
+    cursor: Optional[int] = None, #pagination cursor
+    limit: Optional[int] = None, #limit the number of returned orders per page
+```
+
+```python
+    open_orders = await trading_client.account.get_orders_history(
+        market_names=["BTC-USD", "SOL-USD"],
+        order_side=OrderSide.BUY
+    )
 ```
+returns a list of `OpenOrderModel`
 
 #### `get_trades`
 Fetches the trades of the user's account. It can filter the trades based on market names, trade side, and trade type.
 
 ```python
-pass
 ```
 
 #### `get_fees`
 Fetches the trading fees for the specified markets.
 
 ```python
 pass
@@ -173,14 +247,21 @@
 Fetches the leverage for the specified markets.
 
 ```python
    leverage = await trading_client.account.get_leverage(market_names=list("BTC-USD"))
    print(leverage)
 ```
 
+returns a list of
+```python
+class AccountLeverage(X10BaseModel):
+    market: str
+    leverage: Decimal
+```
+
 #### `update_leverage`
 Updates the leverage for a specific market.
 
 ```python
     await trading_client.account.update_leverage(market_name="BTC-USD", leverage=Decimal("20.0"))
 ```
 
@@ -191,16 +272,16 @@
 ```
 TODO
 
 ## Contribution
 
 Make sure you have [poetry](https://python-poetry.org/) installed.
 
-- Clone the repository: `git@github.com:x10xchange/python-trading.git`
-- Navigate to the project directory: `cd python-trading`
+- Clone the repository: `git@github.com:x10xchange/python_sdk.git`
+- Navigate to the project directory: `cd python_sdk`
 - Create a virtual environment: `poetry shell`
 - Install dependencies: `poetry install`
 - Update `examples/placed_order_example.py` with your credentials
 - Run it: `python -m examples.placed_order_example`
 
 Custom commands:
 - `make format` - format code with `black`
```

