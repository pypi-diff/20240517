# Comparing `tmp/gfx_perp_sdk-0.0.6.tar.gz` & `tmp/gfx_perp_sdk-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfx_perp_sdk-0.0.6.tar", last modified: Thu Nov 16 20:56:00 2023, max compression
+gzip compressed data, was "gfx_perp_sdk-0.0.8.tar", last modified: Fri Jan 26 15:11:02 2024, max compression
```

## Comparing `gfx_perp_sdk-0.0.6.tar` & `gfx_perp_sdk-0.0.8.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-11-16 20:56:00.309989 gfx_perp_sdk-0.0.6/
--rw-r--r--   0 shashank   (501) staff       (20)     1064 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/LICENSE
--rw-r--r--   0 shashank   (501) staff       (20)     7482 2023-11-16 20:56:00.309692 gfx_perp_sdk-0.0.6/PKG-INFO
--rw-r--r--   0 shashank   (501) staff       (20)     7197 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/README.md
-drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-11-16 20:56:00.278828 gfx_perp_sdk-0.0.6/gfx_perp_sdk/
--rw-r--r--   0 shashank   (501) staff       (20)      480 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/Slabs.py
--rw-r--r--   0 shashank   (501) staff       (20)      151 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/__init__.py
-drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-11-16 20:56:00.280421 gfx_perp_sdk-0.0.6/gfx_perp_sdk/agnostic/
--rw-r--r--   0 shashank   (501) staff       (20)     5853 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/agnostic/EventQueue.py
--rw-r--r--   0 shashank   (501) staff       (20)     6677 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/agnostic/Slabs.py
--rw-r--r--   0 shashank   (501) staff       (20)      198 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/agnostic/__init__.py
-drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-11-16 20:56:00.280672 gfx_perp_sdk-0.0.6/gfx_perp_sdk/constant_instructions/
--rw-r--r--   0 shashank   (501) staff       (20)        0 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/constant_instructions/__init__.py
--rw-r--r--   0 shashank   (501) staff       (20)     2408 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/constant_instructions/instructions.py
-drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-11-16 20:56:00.280941 gfx_perp_sdk-0.0.6/gfx_perp_sdk/constants/
--rw-r--r--   0 shashank   (501) staff       (20)        0 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/constants/__init__.py
--rw-r--r--   0 shashank   (501) staff       (20)     3870 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/constants/perps_constants.py
-drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-11-16 20:56:00.284297 gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/
--rw-r--r--   0 shashank   (501) staff       (20)     1685 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/__init__.py
--rw-r--r--   0 shashank   (501) staff       (20)     7249 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/cancel_order.py
--rw-r--r--   0 shashank   (501) staff       (20)     2584 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/choose_successor.py
--rw-r--r--   0 shashank   (501) staff       (20)     2256 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/claim_authority.py
--rw-r--r--   0 shashank   (501) staff       (20)     4450 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/clear_expired_orderbook.py
--rw-r--r--   0 shashank   (501) staff       (20)     5909 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/consume_orderbook_events.py
--rw-r--r--   0 shashank   (501) staff       (20)     3860 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/deposit_funds.py
--rw-r--r--   0 shashank   (501) staff       (20)     2801 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/initialize_combo.py
--rw-r--r--   0 shashank   (501) staff       (20)     3216 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/initialize_market_product.py
--rw-r--r--   0 shashank   (501) staff       (20)     7612 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/initialize_market_product_group.py
--rw-r--r--   0 shashank   (501) staff       (20)     5016 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/initialize_trader_risk_group.py
--rw-r--r--   0 shashank   (501) staff       (20)     1125 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/instruction_tag.py
--rw-r--r--   0 shashank   (501) staff       (20)     8956 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/new_order.py
--rw-r--r--   0 shashank   (501) staff       (20)     4490 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/remove_market_product.py
--rw-r--r--   0 shashank   (501) staff       (20)     3580 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/sweep_fees.py
--rw-r--r--   0 shashank   (501) staff       (20)     5784 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/transfer_full_position.py
--rw-r--r--   0 shashank   (501) staff       (20)     2544 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/update_product_funding.py
--rw-r--r--   0 shashank   (501) staff       (20)     2335 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/update_trader_funding.py
--rw-r--r--   0 shashank   (501) staff       (20)     6694 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/withdraw_funds.py
--rw-r--r--   0 shashank   (501) staff       (20)     3754 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/perp.py
--rw-r--r--   0 shashank   (501) staff       (20)    12609 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/product.py
--rw-r--r--   0 shashank   (501) staff       (20)    15462 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/trader.py
-drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-11-16 20:56:00.293821 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/
--rw-r--r--   0 shashank   (501) staff       (20)     2064 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/__init__.py
--rw-r--r--   0 shashank   (501) staff       (20)     1031 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/account_tag.py
--rw-r--r--   0 shashank   (501) staff       (20)      858 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/action_status.py
--rw-r--r--   0 shashank   (501) staff       (20)      648 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/average_position.py
--rw-r--r--   0 shashank   (501) staff       (20)      530 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/base.py
--rw-r--r--   0 shashank   (501) staff       (20)      453 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/bitset.py
--rw-r--r--   0 shashank   (501) staff       (20)      499 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/call_back_info.py
--rw-r--r--   0 shashank   (501) staff       (20)      441 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/cancel_order_params.py
--rw-r--r--   0 shashank   (501) staff       (20)      469 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/clear_expired_orderbook_params.py
--rw-r--r--   0 shashank   (501) staff       (20)      618 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/combo.py
--rw-r--r--   0 shashank   (501) staff       (20)      467 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/consume_orderbook_events_params.py
--rw-r--r--   0 shashank   (501) staff       (20)      472 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/deposit_funds_params.py
--rw-r--r--   0 shashank   (501) staff       (20)     2282 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/dex_error.py
--rw-r--r--   0 shashank   (501) staff       (20)     3154 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/fractional.py
--rw-r--r--   0 shashank   (501) staff       (20)      577 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/health_info.py
--rw-r--r--   0 shashank   (501) staff       (20)      788 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/health_result.py
--rw-r--r--   0 shashank   (501) staff       (20)      906 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/health_status.py
--rw-r--r--   0 shashank   (501) staff       (20)      665 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/initialize_combo_params.py
--rw-r--r--   0 shashank   (501) staff       (20)      955 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/initialize_market_product_group_params.py
--rw-r--r--   0 shashank   (501) staff       (20)      644 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/initialize_market_product_params.py
--rw-r--r--   0 shashank   (501) staff       (20)      514 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/leg.py
--rw-r--r--   0 shashank   (501) staff       (20)      863 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/liquidation_info.py
--rw-r--r--   0 shashank   (501) staff       (20)     4496 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/market_product_group.py
--rw-r--r--   0 shashank   (501) staff       (20)      717 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/new_order_params.py
--rw-r--r--   0 shashank   (501) staff       (20)     1102 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/open_orders.py
--rw-r--r--   0 shashank   (501) staff       (20)      859 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/open_orders_metadata.py
--rw-r--r--   0 shashank   (501) staff       (20)      684 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/open_orders_node.py
--rw-r--r--   0 shashank   (501) staff       (20)      940 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/operation_type.py
--rw-r--r--   0 shashank   (501) staff       (20)      812 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/order_info.py
--rw-r--r--   0 shashank   (501) staff       (20)      919 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/order_type.py
--rw-r--r--   0 shashank   (501) staff       (20)     1432 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/outright.py
--rw-r--r--   0 shashank   (501) staff       (20)      470 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/params.py
--rw-r--r--   0 shashank   (501) staff       (20)     1093 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/price_ewma.py
--rw-r--r--   0 shashank   (501) staff       (20)     1229 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/product.py
--rw-r--r--   0 shashank   (501) staff       (20)      876 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/product_array.py
--rw-r--r--   0 shashank   (501) staff       (20)     1410 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/product_metadata.py
--rw-r--r--   0 shashank   (501) staff       (20)      883 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/product_status.py
--rw-r--r--   0 shashank   (501) staff       (20)      509 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/risk_output_register.py
--rw-r--r--   0 shashank   (501) staff       (20)      506 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/social_loss.py
--rw-r--r--   0 shashank   (501) staff       (20)      351 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/solana_pubkey.py
--rw-r--r--   0 shashank   (501) staff       (20)      869 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/trade_history.py
--rw-r--r--   0 shashank   (501) staff       (20)      688 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/trader_fee_params.py
--rw-r--r--   0 shashank   (501) staff       (20)      512 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/trader_fees.py
--rw-r--r--   0 shashank   (501) staff       (20)     1292 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/trader_position.py
--rw-r--r--   0 shashank   (501) staff       (20)     3382 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/trader_risk_group.py
--rw-r--r--   0 shashank   (501) staff       (20)      524 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/update_product_funding_params.py
--rw-r--r--   0 shashank   (501) staff       (20)     1385 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/util_error.py
--rw-r--r--   0 shashank   (501) staff       (20)      474 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/withdraw_funds_params.py
--rw-r--r--   0 shashank   (501) staff       (20)    26447 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk/utils.py
-drwxr-xr-x   0 shashank   (501) staff       (20)        0 2023-11-16 20:56:00.279705 gfx_perp_sdk-0.0.6/gfx_perp_sdk.egg-info/
--rw-r--r--   0 shashank   (501) staff       (20)     7482 2023-11-16 20:56:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk.egg-info/PKG-INFO
--rw-r--r--   0 shashank   (501) staff       (20)     3365 2023-11-16 20:56:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 shashank   (501) staff       (20)        1 2023-11-16 20:56:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 shashank   (501) staff       (20)        7 2023-11-16 20:56:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk.egg-info/requires.txt
--rw-r--r--   0 shashank   (501) staff       (20)       13 2023-11-16 20:56:00.000000 gfx_perp_sdk-0.0.6/gfx_perp_sdk.egg-info/top_level.txt
--rw-r--r--   0 shashank   (501) staff       (20)      384 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.6/pyproject.toml
--rw-r--r--   0 shashank   (501) staff       (20)       38 2023-11-16 20:56:00.310036 gfx_perp_sdk-0.0.6/setup.cfg
--rw-r--r--   0 shashank   (501) staff       (20)      520 2023-11-16 20:54:34.000000 gfx_perp_sdk-0.0.6/setup.py
+drwxr-xr-x   0 shashank   (501) staff       (20)        0 2024-01-26 15:11:02.245135 gfx_perp_sdk-0.0.8/
+-rw-r--r--   0 shashank   (501) staff       (20)     1064 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/LICENSE
+-rw-r--r--   0 shashank   (501) staff       (20)     7482 2024-01-26 15:11:02.244655 gfx_perp_sdk-0.0.8/PKG-INFO
+-rw-r--r--   0 shashank   (501) staff       (20)     7197 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/README.md
+drwxr-xr-x   0 shashank   (501) staff       (20)        0 2024-01-26 15:11:02.228184 gfx_perp_sdk-0.0.8/gfx_perp_sdk/
+-rw-r--r--   0 shashank   (501) staff       (20)      480 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/Slabs.py
+-rw-r--r--   0 shashank   (501) staff       (20)      151 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/__init__.py
+drwxr-xr-x   0 shashank   (501) staff       (20)        0 2024-01-26 15:11:02.230019 gfx_perp_sdk-0.0.8/gfx_perp_sdk/agnostic/
+-rw-r--r--   0 shashank   (501) staff       (20)     5853 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/agnostic/EventQueue.py
+-rw-r--r--   0 shashank   (501) staff       (20)     6677 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/agnostic/Slabs.py
+-rw-r--r--   0 shashank   (501) staff       (20)      198 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/agnostic/__init__.py
+drwxr-xr-x   0 shashank   (501) staff       (20)        0 2024-01-26 15:11:02.230337 gfx_perp_sdk-0.0.8/gfx_perp_sdk/constant_instructions/
+-rw-r--r--   0 shashank   (501) staff       (20)        0 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/constant_instructions/__init__.py
+-rw-r--r--   0 shashank   (501) staff       (20)     2408 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/constant_instructions/instructions.py
+drwxr-xr-x   0 shashank   (501) staff       (20)        0 2024-01-26 15:11:02.230613 gfx_perp_sdk-0.0.8/gfx_perp_sdk/constants/
+-rw-r--r--   0 shashank   (501) staff       (20)        0 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/constants/__init__.py
+-rw-r--r--   0 shashank   (501) staff       (20)     3870 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/constants/perps_constants.py
+drwxr-xr-x   0 shashank   (501) staff       (20)        0 2024-01-26 15:11:02.233894 gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/
+-rw-r--r--   0 shashank   (501) staff       (20)     1685 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/__init__.py
+-rw-r--r--   0 shashank   (501) staff       (20)     7249 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/cancel_order.py
+-rw-r--r--   0 shashank   (501) staff       (20)     2584 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/choose_successor.py
+-rw-r--r--   0 shashank   (501) staff       (20)     2256 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/claim_authority.py
+-rw-r--r--   0 shashank   (501) staff       (20)     4450 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/clear_expired_orderbook.py
+-rw-r--r--   0 shashank   (501) staff       (20)     5909 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/consume_orderbook_events.py
+-rw-r--r--   0 shashank   (501) staff       (20)     3860 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/deposit_funds.py
+-rw-r--r--   0 shashank   (501) staff       (20)     2801 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/initialize_combo.py
+-rw-r--r--   0 shashank   (501) staff       (20)     3216 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/initialize_market_product.py
+-rw-r--r--   0 shashank   (501) staff       (20)     7612 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/initialize_market_product_group.py
+-rw-r--r--   0 shashank   (501) staff       (20)     5016 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/initialize_trader_risk_group.py
+-rw-r--r--   0 shashank   (501) staff       (20)     1125 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/instruction_tag.py
+-rw-r--r--   0 shashank   (501) staff       (20)     8956 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/new_order.py
+-rw-r--r--   0 shashank   (501) staff       (20)     4490 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/remove_market_product.py
+-rw-r--r--   0 shashank   (501) staff       (20)     3580 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/sweep_fees.py
+-rw-r--r--   0 shashank   (501) staff       (20)     5784 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/transfer_full_position.py
+-rw-r--r--   0 shashank   (501) staff       (20)     2544 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/update_product_funding.py
+-rw-r--r--   0 shashank   (501) staff       (20)     2335 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/update_trader_funding.py
+-rw-r--r--   0 shashank   (501) staff       (20)     6694 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/withdraw_funds.py
+-rw-r--r--   0 shashank   (501) staff       (20)     3754 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/perp.py
+-rw-r--r--   0 shashank   (501) staff       (20)    12609 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/product.py
+-rw-r--r--   0 shashank   (501) staff       (20)    15462 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/trader.py
+drwxr-xr-x   0 shashank   (501) staff       (20)        0 2024-01-26 15:11:02.243937 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/
+-rw-r--r--   0 shashank   (501) staff       (20)     2064 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/__init__.py
+-rw-r--r--   0 shashank   (501) staff       (20)     1031 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/account_tag.py
+-rw-r--r--   0 shashank   (501) staff       (20)      858 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/action_status.py
+-rw-r--r--   0 shashank   (501) staff       (20)      648 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/average_position.py
+-rw-r--r--   0 shashank   (501) staff       (20)      530 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/base.py
+-rw-r--r--   0 shashank   (501) staff       (20)      453 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/bitset.py
+-rw-r--r--   0 shashank   (501) staff       (20)      499 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/call_back_info.py
+-rw-r--r--   0 shashank   (501) staff       (20)      441 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/cancel_order_params.py
+-rw-r--r--   0 shashank   (501) staff       (20)      469 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/clear_expired_orderbook_params.py
+-rw-r--r--   0 shashank   (501) staff       (20)      618 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/combo.py
+-rw-r--r--   0 shashank   (501) staff       (20)      467 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/consume_orderbook_events_params.py
+-rw-r--r--   0 shashank   (501) staff       (20)      472 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/deposit_funds_params.py
+-rw-r--r--   0 shashank   (501) staff       (20)     2282 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/dex_error.py
+-rw-r--r--   0 shashank   (501) staff       (20)     3154 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/fractional.py
+-rw-r--r--   0 shashank   (501) staff       (20)      577 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/health_info.py
+-rw-r--r--   0 shashank   (501) staff       (20)      788 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/health_result.py
+-rw-r--r--   0 shashank   (501) staff       (20)      906 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/health_status.py
+-rw-r--r--   0 shashank   (501) staff       (20)      665 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/initialize_combo_params.py
+-rw-r--r--   0 shashank   (501) staff       (20)      955 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/initialize_market_product_group_params.py
+-rw-r--r--   0 shashank   (501) staff       (20)      644 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/initialize_market_product_params.py
+-rw-r--r--   0 shashank   (501) staff       (20)      514 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/leg.py
+-rw-r--r--   0 shashank   (501) staff       (20)      863 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/liquidation_info.py
+-rw-r--r--   0 shashank   (501) staff       (20)     4496 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/market_product_group.py
+-rw-r--r--   0 shashank   (501) staff       (20)      717 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/new_order_params.py
+-rw-r--r--   0 shashank   (501) staff       (20)     1102 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/open_orders.py
+-rw-r--r--   0 shashank   (501) staff       (20)      859 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/open_orders_metadata.py
+-rw-r--r--   0 shashank   (501) staff       (20)      684 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/open_orders_node.py
+-rw-r--r--   0 shashank   (501) staff       (20)      940 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/operation_type.py
+-rw-r--r--   0 shashank   (501) staff       (20)      812 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/order_info.py
+-rw-r--r--   0 shashank   (501) staff       (20)      919 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/order_type.py
+-rw-r--r--   0 shashank   (501) staff       (20)     1432 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/outright.py
+-rw-r--r--   0 shashank   (501) staff       (20)      470 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/params.py
+-rw-r--r--   0 shashank   (501) staff       (20)     1093 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/price_ewma.py
+-rw-r--r--   0 shashank   (501) staff       (20)     1229 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/product.py
+-rw-r--r--   0 shashank   (501) staff       (20)      876 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/product_array.py
+-rw-r--r--   0 shashank   (501) staff       (20)     1410 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/product_metadata.py
+-rw-r--r--   0 shashank   (501) staff       (20)      883 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/product_status.py
+-rw-r--r--   0 shashank   (501) staff       (20)      509 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/risk_output_register.py
+-rw-r--r--   0 shashank   (501) staff       (20)      506 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/social_loss.py
+-rw-r--r--   0 shashank   (501) staff       (20)      351 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/solana_pubkey.py
+-rw-r--r--   0 shashank   (501) staff       (20)      869 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/trade_history.py
+-rw-r--r--   0 shashank   (501) staff       (20)      688 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/trader_fee_params.py
+-rw-r--r--   0 shashank   (501) staff       (20)      512 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/trader_fees.py
+-rw-r--r--   0 shashank   (501) staff       (20)     1292 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/trader_position.py
+-rw-r--r--   0 shashank   (501) staff       (20)     3382 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/trader_risk_group.py
+-rw-r--r--   0 shashank   (501) staff       (20)      524 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/update_product_funding_params.py
+-rw-r--r--   0 shashank   (501) staff       (20)     1385 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/util_error.py
+-rw-r--r--   0 shashank   (501) staff       (20)      474 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/withdraw_funds_params.py
+-rw-r--r--   0 shashank   (501) staff       (20)    26447 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk/utils.py
+drwxr-xr-x   0 shashank   (501) staff       (20)        0 2024-01-26 15:11:02.244178 gfx_perp_sdk-0.0.8/gfx_perp_sdk.egg-info/
+-rw-r--r--   0 shashank   (501) staff       (20)     7482 2024-01-26 15:11:02.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 shashank   (501) staff       (20)     3365 2024-01-26 15:11:02.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shashank   (501) staff       (20)        1 2024-01-26 15:11:02.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shashank   (501) staff       (20)        7 2024-01-26 15:11:02.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk.egg-info/requires.txt
+-rw-r--r--   0 shashank   (501) staff       (20)       13 2024-01-26 15:11:02.000000 gfx_perp_sdk-0.0.8/gfx_perp_sdk.egg-info/top_level.txt
+-rw-r--r--   0 shashank   (501) staff       (20)      384 2023-11-16 20:53:00.000000 gfx_perp_sdk-0.0.8/pyproject.toml
+-rw-r--r--   0 shashank   (501) staff       (20)       38 2024-01-26 15:11:02.245182 gfx_perp_sdk-0.0.8/setup.cfg
+-rw-r--r--   0 shashank   (501) staff       (20)      520 2024-01-26 15:09:21.000000 gfx_perp_sdk-0.0.8/setup.py
```

### Comparing `gfx_perp_sdk-0.0.6/LICENSE` & `gfx_perp_sdk-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/PKG-INFO` & `gfx_perp_sdk-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfx_perp_sdk
-Version: 0.0.6
+Version: 0.0.8
 Summary: Perp python sdk
 Home-page: https://github.com/GooseFX1/gfx-perps-python-sdk
 Author: Shashank Shekhar
 Author-email: shashank@goosefx.io
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytest
```

### Comparing `gfx_perp_sdk-0.0.6/README.md` & `gfx_perp_sdk-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/agnostic/EventQueue.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/agnostic/EventQueue.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/agnostic/Slabs.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/agnostic/Slabs.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/constant_instructions/instructions.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/constant_instructions/instructions.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/constants/perps_constants.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/constants/perps_constants.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/__init__.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/__init__.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/cancel_order.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/cancel_order.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/choose_successor.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/choose_successor.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/claim_authority.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/claim_authority.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/clear_expired_orderbook.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/clear_expired_orderbook.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/consume_orderbook_events.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/consume_orderbook_events.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/deposit_funds.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/deposit_funds.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/initialize_combo.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/initialize_combo.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/initialize_market_product.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/initialize_market_product.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/initialize_market_product_group.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/initialize_market_product_group.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/initialize_trader_risk_group.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/initialize_trader_risk_group.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/instruction_tag.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/instruction_tag.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/new_order.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/new_order.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/remove_market_product.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/remove_market_product.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/sweep_fees.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/sweep_fees.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/transfer_full_position.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/transfer_full_position.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/update_product_funding.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/update_product_funding.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/update_trader_funding.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/update_trader_funding.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/instructions/withdraw_funds.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/instructions/withdraw_funds.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/perp.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/perp.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/product.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/product.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/trader.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/trader.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/__init__.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/account_tag.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/account_tag.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/action_status.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/action_status.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/average_position.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/average_position.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/base.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/base.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/combo.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/combo.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/dex_error.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/dex_error.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/fractional.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/fractional.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/health_info.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/health_info.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/health_result.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/health_result.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/health_status.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/health_status.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/initialize_combo_params.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/initialize_combo_params.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/initialize_market_product_group_params.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/initialize_market_product_group_params.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/initialize_market_product_params.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/initialize_market_product_params.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/leg.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/leg.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/liquidation_info.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/liquidation_info.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/market_product_group.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/market_product_group.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/new_order_params.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/new_order_params.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/open_orders.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/open_orders.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/open_orders_metadata.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/open_orders_metadata.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/open_orders_node.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/open_orders_node.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/operation_type.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/operation_type.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/order_info.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/order_info.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/order_type.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/order_type.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/outright.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/outright.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/price_ewma.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/price_ewma.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/product.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/product.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/product_array.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/product_array.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/product_metadata.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/product_metadata.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/product_status.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/product_status.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/trade_history.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/trade_history.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/trader_fee_params.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/trader_fee_params.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/trader_fees.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/trader_fees.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/trader_position.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/trader_position.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/trader_risk_group.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/trader_risk_group.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/update_product_funding_params.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/update_product_funding_params.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/types/util_error.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/types/util_error.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk/utils.py` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk.egg-info/PKG-INFO` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gfx-perp-sdk
-Version: 0.0.6
+Name: gfx_perp_sdk
+Version: 0.0.8
 Summary: Perp python sdk
 Home-page: https://github.com/GooseFX1/gfx-perps-python-sdk
 Author: Shashank Shekhar
 Author-email: shashank@goosefx.io
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytest
```

### Comparing `gfx_perp_sdk-0.0.6/gfx_perp_sdk.egg-info/SOURCES.txt` & `gfx_perp_sdk-0.0.8/gfx_perp_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gfx_perp_sdk-0.0.6/setup.py` & `gfx_perp_sdk-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='gfx_perp_sdk',
-    version='0.0.6',
+    version='0.0.8',
     url='https://github.com/GooseFX1/gfx-perps-python-sdk',
     author='Shashank Shekhar',
     author_email='shashank@goosefx.io',
     description='Perp python sdk',
     packages=find_packages(),
     install_requires=[
         'pytest'
```

