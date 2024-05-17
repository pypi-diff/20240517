# Comparing `tmp/telegram_wallet_pay-0.7.0.tar.gz` & `tmp/telegram_wallet_pay-0.8.0.tar.gz`

## Comparing `telegram_wallet_pay-0.7.0.tar` & `telegram_wallet_pay-0.8.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/.editorconfig
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/Makefile
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/SECURITY.md
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/codecov.yaml
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/examples/00_create_order.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/examples/01_get_order_preview.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/examples/02_telegram_bot.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/examples/03_webhook_handler_fastapi.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/examples/04_webhook_handler_aiohttp.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/__init__.py
--rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/client.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/constants.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/errors.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/enums/__init__.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/enums/button_name.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/enums/currency.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/enums/order_status.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/enums/request_status.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/enums/webhook_message_type.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/_default.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/create_order_request.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/create_order_response.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/get_order_preview_response.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/get_order_reconciliation_list_response.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/money_amount.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/order_amount.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/order_amount_response.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/order_preview.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/order_reconciliation_item.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/order_reconciliation_list.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/payment_option.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/webhook_message.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/webhook_payload.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/tools/__init__.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/tools/aiohttp.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/tools/fastapi.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/tools/ip_filter.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/tools/signature.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/tools/text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/tests/samples.py
--rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/tests/test_client.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/tests/test_schemas.py
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/tests/test_tools/test_aiohttp.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/tests/test_tools/test_fastapi.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/tests/test_tools/test_ip_filter.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/tests/test_tools/test_signature.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/LICENSE
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/README.md
--rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/.editorconfig
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/Makefile
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/SECURITY.md
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/codecov.yaml
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/examples/00_create_order.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/examples/01_get_order_preview.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/examples/02_telegram_bot.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/examples/03_webhook_handler_fastapi.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/examples/04_webhook_handler_aiohttp.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/__init__.py
+-rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/client.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/constants.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/errors.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/enums/__init__.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/enums/button_name.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/enums/currency.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/enums/order_status.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/enums/request_status.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/enums/webhook_message_type.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/_default.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/create_order_request.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/create_order_response.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/get_order_preview_response.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/get_order_reconciliation_list_response.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/money_amount.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/order_amount.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/order_amount_response.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/order_preview.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/order_reconciliation_item.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/order_reconciliation_list.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/payment_option.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/webhook_message.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/webhook_payload.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/tools/__init__.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/tools/aiohttp.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/tools/fastapi.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/tools/ip_filter.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/tools/signature.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/telegram_wallet_pay/tools/text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/tests/samples.py
+-rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/tests/test_client.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/tests/test_schemas.py
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/tests/test_tools/test_aiohttp.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/tests/test_tools/test_fastapi.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/tests/test_tools/test_ip_filter.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/tests/test_tools/test_signature.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/LICENSE
+-rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/README.md
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.8.0/PKG-INFO
```

### Comparing `telegram_wallet_pay-0.7.0/CODE_OF_CONDUCT.md` & `telegram_wallet_pay-0.8.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/CONTRIBUTING.md` & `telegram_wallet_pay-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/examples/00_create_order.py` & `telegram_wallet_pay-0.8.0/examples/00_create_order.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/examples/01_get_order_preview.py` & `telegram_wallet_pay-0.8.0/examples/01_get_order_preview.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/examples/02_telegram_bot.py` & `telegram_wallet_pay-0.8.0/examples/02_telegram_bot.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/examples/03_webhook_handler_fastapi.py` & `telegram_wallet_pay-0.8.0/examples/03_webhook_handler_fastapi.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/examples/04_webhook_handler_aiohttp.py` & `telegram_wallet_pay-0.8.0/examples/04_webhook_handler_aiohttp.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/telegram_wallet_pay/client.py` & `telegram_wallet_pay-0.8.0/telegram_wallet_pay/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,26 +62,32 @@
 
     async def create_order(  # noqa: PLR0913
         self,
         *,
         amount: Union[str, Decimal, float],
         currency_code: Literal[
             Currency.TON,
+            Currency.NOT,
             Currency.BTC,
             Currency.USDT,
             Currency.EUR,
             Currency.USD,
             Currency.RUB,
         ],
         description: str,
         external_id: str,
         timeout_seconds: int,
         customer_telegram_user_id: int,
         auto_conversion_currency: Optional[
-            Literal[Currency.TON, Currency.BTC, Currency.USDT]
+            Literal[
+                Currency.TON,
+                Currency.NOT,
+                Currency.BTC,
+                Currency.USDT,
+            ]
         ] = None,
         return_url: Optional[str] = None,
         fail_return_url: Optional[str] = None,
         custom_data: Optional[str] = None,
     ) -> CreateOrderResponse:
         """Create an order.
```

### Comparing `telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/__init__.py` & `telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/create_order_request.py` & `telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/create_order_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 class CreateOrderRequest(DefaultModel):
     amount: MoneyAmount
     auto_conversion_currency: Optional[
         Literal[
             Currency.TON,
+            Currency.NOT,
             Currency.BTC,
             Currency.USDT,
         ]
     ] = None
     description: str = Field(min_length=5, max_length=100)
     return_url: Optional[str] = Field(None, max_length=255)
     fail_return_url: Optional[str] = Field(None, max_length=255)
```

### Comparing `telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/create_order_response.py` & `telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/create_order_response.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/order_preview.py` & `telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/order_preview.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         OrderStatus.CANCELLED,
     ]
     number: str
     amount: MoneyAmount
     auto_conversion_currency: Optional[
         Literal[
             Currency.TON,
+            Currency.NOT,
             Currency.BTC,
             Currency.USDT,
         ]
     ] = None
     created_datetime: datetime = Field(alias="createdDateTime")
     expiration_datetime: datetime = Field(alias="expirationDateTime")
     completed_datetime: Optional[datetime] = Field(None, alias="completedDateTime")
```

### Comparing `telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/order_reconciliation_item.py` & `telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/order_reconciliation_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         OrderStatus.PAID,
         OrderStatus.CANCELLED,
     ]
     amount: MoneyAmount
     auto_conversion_currency: Optional[
         Literal[
             Currency.TON,
+            Currency.NOT,
             Currency.BTC,
             Currency.USDT,
         ]
     ] = None
     external_id: str
     customer_telegram_user_id: Optional[int] = None
     created_datetime: datetime = Field(alias="createdDateTime")
```

### Comparing `telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/webhook_message.py` & `telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/webhook_message.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/webhook_payload.py` & `telegram_wallet_pay-0.8.0/telegram_wallet_pay/schemas/webhook_payload.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/telegram_wallet_pay/tools/aiohttp.py` & `telegram_wallet_pay-0.8.0/telegram_wallet_pay/tools/aiohttp.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/telegram_wallet_pay/tools/fastapi.py` & `telegram_wallet_pay-0.8.0/telegram_wallet_pay/tools/fastapi.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/telegram_wallet_pay/tools/ip_filter.py` & `telegram_wallet_pay-0.8.0/telegram_wallet_pay/tools/ip_filter.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/telegram_wallet_pay/tools/signature.py` & `telegram_wallet_pay-0.8.0/telegram_wallet_pay/tools/signature.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/tests/conftest.py` & `telegram_wallet_pay-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/tests/samples.py` & `telegram_wallet_pay-0.8.0/tests/samples.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/tests/test_client.py` & `telegram_wallet_pay-0.8.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/tests/test_schemas.py` & `telegram_wallet_pay-0.8.0/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/tests/test_tools/test_aiohttp.py` & `telegram_wallet_pay-0.8.0/tests/test_tools/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/tests/test_tools/test_fastapi.py` & `telegram_wallet_pay-0.8.0/tests/test_tools/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/tests/test_tools/test_ip_filter.py` & `telegram_wallet_pay-0.8.0/tests/test_tools/test_ip_filter.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/tests/test_tools/test_signature.py` & `telegram_wallet_pay-0.8.0/tests/test_tools/test_signature.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/.gitignore` & `telegram_wallet_pay-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/LICENSE` & `telegram_wallet_pay-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/README.md` & `telegram_wallet_pay-0.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -104,14 +104,14 @@
     asyncio.run(main())
 
 ```
 
 
 ## Other examples
 
-* [Telegram bot example (aiogram)](./examples/02_telegram_bot.py)
-* [Webhook handler example (FastAPI)](./examples/03_webhook_handler_fastapi.py)
-* [Webhook handler example (aiohttp)](./examples/04_webhook_handler_aiohttp.py)
+* [Telegram bot example (aiogram)](https://github.com/Olegt0rr/TelegramWalletPay/blob/main/examples/02_telegram_bot.py)
+* [Webhook handler example (FastAPI)](https://github.com/Olegt0rr/TelegramWalletPay/blob/main/examples/03_webhook_handler_fastapi.py)
+* [Webhook handler example (aiohttp)](https://github.com/Olegt0rr/TelegramWalletPay/blob/main/examples/04_webhook_handler_aiohttp.py)
 
 Also, feel free to open the
 [folder with examples](https://github.com/Olegt0rr/TelegramWalletPay/tree/main/examples),
 and if there is something missing there, describe your needs in [issue](https://github.com/Olegt0rr/TelegramWalletPay/issues/new/choose).
```

### Comparing `telegram_wallet_pay-0.7.0/pyproject.toml` & `telegram_wallet_pay-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.7.0/PKG-INFO` & `telegram_wallet_pay-0.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: telegram-wallet-pay
-Version: 0.7.0
+Version: 0.8.0
 Summary: Async client for Telegram Wallet Pay API
 Project-URL: Repository, https://github.com/Olegt0rr/TelegramWalletPay
 Project-URL: Documentation, https://docs.wallet.tg/pay/
 Author-email: Oleg Abramov <oleg@trueweb.app>
 Maintainer-email: Oleg Abramov <oleg@trueweb.app>
 License-Expression: MIT
 License-File: LICENSE
@@ -157,14 +157,14 @@
     asyncio.run(main())
 
 ```
 
 
 ## Other examples
 
-* [Telegram bot example (aiogram)](./examples/02_telegram_bot.py)
-* [Webhook handler example (FastAPI)](./examples/03_webhook_handler_fastapi.py)
-* [Webhook handler example (aiohttp)](./examples/04_webhook_handler_aiohttp.py)
+* [Telegram bot example (aiogram)](https://github.com/Olegt0rr/TelegramWalletPay/blob/main/examples/02_telegram_bot.py)
+* [Webhook handler example (FastAPI)](https://github.com/Olegt0rr/TelegramWalletPay/blob/main/examples/03_webhook_handler_fastapi.py)
+* [Webhook handler example (aiohttp)](https://github.com/Olegt0rr/TelegramWalletPay/blob/main/examples/04_webhook_handler_aiohttp.py)
 
 Also, feel free to open the
 [folder with examples](https://github.com/Olegt0rr/TelegramWalletPay/tree/main/examples),
 and if there is something missing there, describe your needs in [issue](https://github.com/Olegt0rr/TelegramWalletPay/issues/new/choose).
```

