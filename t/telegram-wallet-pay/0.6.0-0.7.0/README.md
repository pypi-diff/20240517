# Comparing `tmp/telegram_wallet_pay-0.6.0.tar.gz` & `tmp/telegram_wallet_pay-0.7.0.tar.gz`

## Comparing `telegram_wallet_pay-0.6.0.tar` & `telegram_wallet_pay-0.7.0.tar`

### file list

```diff
@@ -1,48 +1,57 @@
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/.editorconfig
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/Makefile
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/codecov.yaml
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/examples/00_create_order.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/examples/01_get_order_preview.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/examples/02_bot_example.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/examples/03_webhook_handler_example.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/__init__.py
--rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/client.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/constants.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/errors.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/enums/__init__.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/enums/button_name.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/enums/currency.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/enums/order_status.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/enums/request_status.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/enums/webhook_message_type.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/_default.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/create_order_request.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/create_order_response.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/get_order_preview_response.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/get_order_reconciliation_list_response.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/money_amount.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/order_amount.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/order_amount_response.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/order_preview.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/order_reconciliation_item.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/order_reconciliation_list.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/payment_option.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/webhook_message.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/webhook_payload.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/tools/__init__.py
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/tools/fastapi.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/tools/signature.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/tools/text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/tests/samples.py
--rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/tests/test_client.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/tests/test_schemas.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/tests/test_tools/test_fastapi.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/tests/test_tools/test_signature.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/.gitignore
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/README.md
--rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/.editorconfig
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/Makefile
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/SECURITY.md
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/codecov.yaml
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/examples/00_create_order.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/examples/01_get_order_preview.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/examples/02_telegram_bot.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/examples/03_webhook_handler_fastapi.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/examples/04_webhook_handler_aiohttp.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/__init__.py
+-rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/client.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/constants.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/errors.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/enums/__init__.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/enums/button_name.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/enums/currency.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/enums/order_status.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/enums/request_status.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/enums/webhook_message_type.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/_default.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/create_order_request.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/create_order_response.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/get_order_preview_response.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/get_order_reconciliation_list_response.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/money_amount.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/order_amount.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/order_amount_response.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/order_preview.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/order_reconciliation_item.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/order_reconciliation_list.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/payment_option.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/webhook_message.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/webhook_payload.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/tools/__init__.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/tools/aiohttp.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/tools/fastapi.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/tools/ip_filter.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/tools/signature.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/telegram_wallet_pay/tools/text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/tests/samples.py
+-rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/tests/test_client.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/tests/test_schemas.py
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/tests/test_tools/test_aiohttp.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/tests/test_tools/test_fastapi.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/tests/test_tools/test_ip_filter.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/tests/test_tools/test_signature.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/LICENSE
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/README.md
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.7.0/PKG-INFO
```

### Comparing `telegram_wallet_pay-0.6.0/examples/00_create_order.py` & `telegram_wallet_pay-0.7.0/examples/00_create_order.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import asyncio
 import os
 from uuid import uuid4
 
 from telegram_wallet_pay import TelegramWalletPay
 
-# use your token from https://pay.wallet.tg/
+# store TELEGRAM_WALLET_PAY_TOKEN to your .env
+# wallet token can be issued via https://pay.wallet.tg/
 TOKEN = os.getenv("TELEGRAM_WALLET_PAY_TOKEN")
 
 
 async def main() -> None:
     """Create order."""
+    # create wallet client instance
     wallet = TelegramWalletPay(TOKEN)
 
     # create your first order
     response = await wallet.create_order(
         amount=40,
         currency_code="EUR",
         description="TestPayment",
```

### Comparing `telegram_wallet_pay-0.6.0/examples/02_bot_example.py` & `telegram_wallet_pay-0.7.0/examples/02_telegram_bot.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.6.0/examples/03_webhook_handler_example.py` & `telegram_wallet_pay-0.7.0/examples/03_webhook_handler_fastapi.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from typing import Dict
 
 import uvicorn
 from fastapi import Depends, FastAPI
 from telegram_wallet_pay.schemas import WebhookMessages
 from telegram_wallet_pay.tools.fastapi import CheckSignature
 
+# store TELEGRAM_WALLET_PAY_TOKEN to your .env
+# wallet token can be issued via https://pay.wallet.tg/
 TELEGRAM_WALLET_PAY_TOKEN = os.getenv("TELEGRAM_WALLET_PAY_TOKEN")
 
 app = FastAPI()
 check_signature = CheckSignature(TELEGRAM_WALLET_PAY_TOKEN)
 
 
 @app.post("/wallet", dependencies=[Depends(check_signature)])
```

### Comparing `telegram_wallet_pay-0.6.0/telegram_wallet_pay/client.py` & `telegram_wallet_pay-0.7.0/telegram_wallet_pay/client.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/__init__.py` & `telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/create_order_request.py` & `telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/create_order_request.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/create_order_response.py` & `telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/create_order_response.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/order_preview.py` & `telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/order_preview.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/order_reconciliation_item.py` & `telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/order_reconciliation_item.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/webhook_message.py` & `telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/webhook_message.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/webhook_payload.py` & `telegram_wallet_pay-0.7.0/telegram_wallet_pay/schemas/webhook_payload.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.6.0/telegram_wallet_pay/tools/fastapi.py` & `telegram_wallet_pay-0.7.0/telegram_wallet_pay/tools/fastapi.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from secrets import compare_digest
 from typing import Optional
 
 from fastapi import Depends, HTTPException, Request
 
-from telegram_wallet_pay.tools import compute_signature
+from .signature import compute_signature
 
 
 def get_timestamp(request: Request) -> str:
     """Get timestamp from header."""
     try:
         timestamp = request.headers["WalletPay-Timestamp"]
     except KeyError:
@@ -16,15 +16,15 @@
             detail="Timestamp header is missing",
         ) from None
 
     if not timestamp:
         raise HTTPException(
             status_code=400,
             detail="Timestamp header is empty",
-        ) from None
+        )
 
     return timestamp
 
 
 def get_signature(request: Request) -> str:
     """Get signature from header."""
     try:
@@ -35,15 +35,15 @@
             detail="Signature header is missing",
         ) from None
 
     if not signature:
         raise HTTPException(
             status_code=400,
             detail="Signature header is empty",
-        ) from None
+        )
 
     return signature
 
 
 async def get_raw_body(request: Request) -> bytes:
     """Get request body."""
     return await request.body()
```

### Comparing `telegram_wallet_pay-0.6.0/telegram_wallet_pay/tools/signature.py` & `telegram_wallet_pay-0.7.0/telegram_wallet_pay/tools/signature.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.6.0/tests/conftest.py` & `telegram_wallet_pay-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.6.0/tests/samples.py` & `telegram_wallet_pay-0.7.0/tests/samples.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.6.0/tests/test_client.py` & `telegram_wallet_pay-0.7.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.6.0/tests/test_schemas.py` & `telegram_wallet_pay-0.7.0/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.6.0/tests/test_tools/test_fastapi.py` & `telegram_wallet_pay-0.7.0/tests/test_tools/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.6.0/tests/test_tools/test_signature.py` & `telegram_wallet_pay-0.7.0/tests/test_tools/test_signature.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.6.0/.gitignore` & `telegram_wallet_pay-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.6.0/README.md` & `telegram_wallet_pay-0.7.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -6,16 +6,18 @@
  - `pydantic` models for every schema, even for incoming webhooks
  - signature validation tool, including ready-made `Depends` for `FastAPI`
 
 [![Python](https://img.shields.io/pypi/pyversions/telegram-wallet-pay.svg)](https://pypi.org/project/telegram-wallet-pay/)
 [![pypi](https://img.shields.io/pypi/v/telegram-wallet-pay?label=pypi%20package)](https://pypi.org/project/telegram-wallet-pay/)
 [![Tests](https://github.com/Olegt0rr/TelegramWalletPay/actions/workflows/tests.yml/badge.svg)](https://github.com/Olegt0rr/TelegramWalletPay/actions/workflows/tests.yml)
 [![Coverage](https://img.shields.io/codecov/c/github/Olegt0rr/TelegramWalletPay)](https://app.codecov.io/gh/Olegt0rr/TelegramWalletPay)
+
 [![Code linter: ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
-[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
+[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org)
+[![Gitmoji](https://img.shields.io/badge/gitmoji-%20😎-FFDD67.svg)](https://gitmoji.dev)
 ---
 
 ## Get started
 
 ### Read Telegram Wallet Pay API docs
 
 https://docs.wallet.tg/pay/#section/Get-started
@@ -31,20 +33,22 @@
 ```python
 import asyncio
 import os
 from uuid import uuid4
 
 from telegram_wallet_pay import TelegramWalletPay
 
-# use your token from https://pay.wallet.tg/
+# store TELEGRAM_WALLET_PAY_TOKEN to your .env
+# wallet token can be issued via https://pay.wallet.tg/
 TOKEN = os.getenv("TELEGRAM_WALLET_PAY_TOKEN")
 
 
 async def main() -> None:
     """Create order."""
+    # create wallet client instance
     wallet = TelegramWalletPay(TOKEN)
 
     # create your first order
     response = await wallet.create_order(
         amount=40,
         currency_code="EUR",
         description="TestPayment",
@@ -71,36 +75,43 @@
 
 ```python
 import asyncio
 import os
 
 from telegram_wallet_pay import TelegramWalletPay
 
+# store TELEGRAM_WALLET_PAY_TOKEN to your .env
+# wallet token can be issued via https://pay.wallet.tg/
 TOKEN = os.getenv("TELEGRAM_WALLET_PAY_TOKEN")
 
 
 async def main() -> None:
     """Get order preview."""
+    # create wallet client instance
     wallet = TelegramWalletPay(TOKEN)
 
+    # get order preview
     response = await wallet.get_order_preview("<your-order-id>")
 
+    # let's print received response
     print("Response:", response)
     print("Order Preview:", response.data)
 
+    # don't forget close API-client instance on your app shutdown
     await wallet.close()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 
 ```
 
 
 ## Other examples
 
-* [Telegram bot example (aiogram)](https://github.com/Olegt0rr/TelegramWalletPay/blob/main/examples/02_bot_example.py)
-* [Webhook handler example (FastAPI)](https://github.com/Olegt0rr/TelegramWalletPay/blob/main/examples/03_webhook_handler_example.py)
+* [Telegram bot example (aiogram)](./examples/02_telegram_bot.py)
+* [Webhook handler example (FastAPI)](./examples/03_webhook_handler_fastapi.py)
+* [Webhook handler example (aiohttp)](./examples/04_webhook_handler_aiohttp.py)
 
 Also, feel free to open the
 [folder with examples](https://github.com/Olegt0rr/TelegramWalletPay/tree/main/examples),
 and if there is something missing there, describe your needs in [issue](https://github.com/Olegt0rr/TelegramWalletPay/issues/new/choose).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `telegram_wallet_pay-0.6.0/pyproject.toml` & `telegram_wallet_pay-0.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     "httpx>=0.27,<1",
     "aiogram>=3.6,<4"
 ]
 test = [
     "coverage>=7,<8",
     "pytest>=8,<9",
     "pytest-asyncio>=0,<1",
+    "pytest-aiohttp>=1.0,<2",
     "pytest-cov>=5,<6",
     "aresponses>=3,<4",
     "fastapi-slim>=0.111,<1",
     "httpx>=0.27,<1",
 ]
 
 
@@ -191,9 +192,9 @@
 [tool.ruff.lint.mccabe]
 max-complexity = 10
 
 [tool.ruff.lint.flake8-type-checking]
 runtime-evaluated-base-classes = ["pydantic.BaseModel", "telegram_wallet_pay.schemas._default.DefaultModel"]
 
 [tool.ruff.lint.per-file-ignores]
-"tests/*" = ["S101", "INP001", "D"]
+"tests/*" = ["D", "FBT001", "INP001", "S101", "SLF001"]
 "examples/*" = ["INP001", "T201"]
```

### Comparing `telegram_wallet_pay-0.6.0/PKG-INFO` & `telegram_wallet_pay-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.3
 Name: telegram-wallet-pay
-Version: 0.6.0
+Version: 0.7.0
 Summary: Async client for Telegram Wallet Pay API
 Project-URL: Repository, https://github.com/Olegt0rr/TelegramWalletPay
 Project-URL: Documentation, https://docs.wallet.tg/pay/
 Author-email: Oleg Abramov <oleg@trueweb.app>
 Maintainer-email: Oleg Abramov <oleg@trueweb.app>
 License-Expression: MIT
+License-File: LICENSE
 Keywords: API,Pay,Telegram,Wallet,async
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: Pydantic
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
@@ -40,14 +41,15 @@
 Requires-Dist: ruff<1,>=0; extra == 'dev'
 Requires-Dist: uvicorn<1,>=0.29; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: aresponses<4,>=3; extra == 'test'
 Requires-Dist: coverage<8,>=7; extra == 'test'
 Requires-Dist: fastapi-slim<1,>=0.111; extra == 'test'
 Requires-Dist: httpx<1,>=0.27; extra == 'test'
+Requires-Dist: pytest-aiohttp<2,>=1.0; extra == 'test'
 Requires-Dist: pytest-asyncio<1,>=0; extra == 'test'
 Requires-Dist: pytest-cov<6,>=5; extra == 'test'
 Requires-Dist: pytest<9,>=8; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Telegram Wallet Pay
 
@@ -57,16 +59,18 @@
  - `pydantic` models for every schema, even for incoming webhooks
  - signature validation tool, including ready-made `Depends` for `FastAPI`
 
 [![Python](https://img.shields.io/pypi/pyversions/telegram-wallet-pay.svg)](https://pypi.org/project/telegram-wallet-pay/)
 [![pypi](https://img.shields.io/pypi/v/telegram-wallet-pay?label=pypi%20package)](https://pypi.org/project/telegram-wallet-pay/)
 [![Tests](https://github.com/Olegt0rr/TelegramWalletPay/actions/workflows/tests.yml/badge.svg)](https://github.com/Olegt0rr/TelegramWalletPay/actions/workflows/tests.yml)
 [![Coverage](https://img.shields.io/codecov/c/github/Olegt0rr/TelegramWalletPay)](https://app.codecov.io/gh/Olegt0rr/TelegramWalletPay)
+
 [![Code linter: ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
-[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
+[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org)
+[![Gitmoji](https://img.shields.io/badge/gitmoji-%20😎-FFDD67.svg)](https://gitmoji.dev)
 ---
 
 ## Get started
 
 ### Read Telegram Wallet Pay API docs
 
 https://docs.wallet.tg/pay/#section/Get-started
@@ -82,20 +86,22 @@
 ```python
 import asyncio
 import os
 from uuid import uuid4
 
 from telegram_wallet_pay import TelegramWalletPay
 
-# use your token from https://pay.wallet.tg/
+# store TELEGRAM_WALLET_PAY_TOKEN to your .env
+# wallet token can be issued via https://pay.wallet.tg/
 TOKEN = os.getenv("TELEGRAM_WALLET_PAY_TOKEN")
 
 
 async def main() -> None:
     """Create order."""
+    # create wallet client instance
     wallet = TelegramWalletPay(TOKEN)
 
     # create your first order
     response = await wallet.create_order(
         amount=40,
         currency_code="EUR",
         description="TestPayment",
@@ -122,36 +128,43 @@
 
 ```python
 import asyncio
 import os
 
 from telegram_wallet_pay import TelegramWalletPay
 
+# store TELEGRAM_WALLET_PAY_TOKEN to your .env
+# wallet token can be issued via https://pay.wallet.tg/
 TOKEN = os.getenv("TELEGRAM_WALLET_PAY_TOKEN")
 
 
 async def main() -> None:
     """Get order preview."""
+    # create wallet client instance
     wallet = TelegramWalletPay(TOKEN)
 
+    # get order preview
     response = await wallet.get_order_preview("<your-order-id>")
 
+    # let's print received response
     print("Response:", response)
     print("Order Preview:", response.data)
 
+    # don't forget close API-client instance on your app shutdown
     await wallet.close()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 
 ```
 
 
 ## Other examples
 
-* [Telegram bot example (aiogram)](https://github.com/Olegt0rr/TelegramWalletPay/blob/main/examples/02_bot_example.py)
-* [Webhook handler example (FastAPI)](https://github.com/Olegt0rr/TelegramWalletPay/blob/main/examples/03_webhook_handler_example.py)
+* [Telegram bot example (aiogram)](./examples/02_telegram_bot.py)
+* [Webhook handler example (FastAPI)](./examples/03_webhook_handler_fastapi.py)
+* [Webhook handler example (aiohttp)](./examples/04_webhook_handler_aiohttp.py)
 
 Also, feel free to open the
 [folder with examples](https://github.com/Olegt0rr/TelegramWalletPay/tree/main/examples),
 and if there is something missing there, describe your needs in [issue](https://github.com/Olegt0rr/TelegramWalletPay/issues/new/choose).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

