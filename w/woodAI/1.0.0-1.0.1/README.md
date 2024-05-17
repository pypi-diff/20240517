# Comparing `tmp/woodAI-1.0.0-py3-none-any.whl.zip` & `tmp/woodAI-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3996 bytes, number of entries: 7
+Zip file size: 4030 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       47 b- defN 24-May-15 06:19 woodAI/__init__.py
--rw-r--r--  2.0 unx     5373 b- defN 24-May-15 08:26 woodAI/ai_chat.py
--rw-rw-r--  2.0 unx     1081 b- defN 24-May-15 08:31 woodAI-1.0.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      231 b- defN 24-May-15 08:31 woodAI-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-15 08:31 woodAI-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-May-15 08:31 woodAI-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      530 b- defN 24-May-15 08:31 woodAI-1.0.0.dist-info/RECORD
-7 files, 7361 bytes uncompressed, 3056 bytes compressed:  58.5%
+-rw-r--r--  2.0 unx     5558 b- defN 24-May-16 11:02 woodAI/ai_chat.py
+-rw-rw-r--  2.0 unx     1081 b- defN 24-May-16 11:03 woodAI-1.0.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      231 b- defN 24-May-16 11:03 woodAI-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 11:03 woodAI-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-May-16 11:03 woodAI-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      530 b- defN 24-May-16 11:03 woodAI-1.0.1.dist-info/RECORD
+7 files, 7546 bytes uncompressed, 3090 bytes compressed:  59.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: woodAI/__init__.py
 Comment: 
 
 Filename: woodAI/ai_chat.py
 Comment: 
 
-Filename: woodAI-1.0.0.dist-info/LICENSE.txt
+Filename: woodAI-1.0.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: woodAI-1.0.0.dist-info/METADATA
+Filename: woodAI-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: woodAI-1.0.0.dist-info/WHEEL
+Filename: woodAI-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: woodAI-1.0.0.dist-info/top_level.txt
+Filename: woodAI-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: woodAI-1.0.0.dist-info/RECORD
+Filename: woodAI-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## woodAI/ai_chat.py

```diff
@@ -1,31 +1,33 @@
 import websocket
 import json
 import os
+import ssl
 
 ws = None
 default_error_tips = "未知错误："
 no_login_tips = "用户未登录，无法使用 AI chat 功能，请登录后重试"
 error_record = {
     10000000: "操作失败，请稍后重试",
     10000011: "该账户暂未开启 AI chat 体验权限",
     20000001: "失败请重试",
     80000001: "登录态校验失败",
     80000003: "请求参数异常",
     80000004: "AI chat 对话内容涉嫌违规，已结束当前对话，请重新开启对话",
     80000006: "每日使用次数已达上限",
 }
 
+
 def generate_default_error(code: int):
-    global default_error_tips,error_record
+    global default_error_tips, error_record
     return RuntimeError(
-                default_error_tips + code
-                if code not in error_record.keys()
-                else error_record[code]
-            )
+        default_error_tips + code
+        if code not in error_record.keys()
+        else error_record[code]
+    )
 
 
 def parse_message(str: str):
     # print(str)
     if str.startswith("42"):
         data = json.loads(str[2:])
         return {"type": data[0], "payload": data[1]}
@@ -50,15 +52,15 @@
 def wait_until_can_join(ws: websocket.WebSocket):
     while True:
         rec = ws.recv()
         data = parse_message(rec)
         name = data["type"]
         payload = data["payload"]
         if name == "server_push_waiting_count":
-            print(f'正在接入AIchat，您前面还有 {payload['waiting_count']} 位用户')
+            print("正在接入AIchat，您前面还有 " + payload["waiting_count"] + " 位用户")
         if name == "server_push_to_join":
             print("您已成功接入AIchat，现在可以开始对话了")
             break
 
 
 def wait_until_connect(ws: websocket.WebSocket):
     while True:
@@ -66,42 +68,52 @@
         data = parse_message(rec)
         name = data["type"]
         payload = data["payload"]
         if name != "on_connect_ack":
             continue
         if payload["code"] == 10000012:
             print(
-                f'正在接入AIchat，您前面还有 {payload['data']['waiting_count']} 位用户'
+                "正在接入AIchat，您前面还有 "
+                + payload["data"]["waiting_count"]
+                + " 位用户"
             )
             wait_until_can_join(ws)
         elif payload["code"] != 1:
             ws.close()
-            raise generate_default_error(payload['code'])
+            raise generate_default_error(payload["code"])
         join(ws)
         break
 
 
 def connect():
     global ws
-    token = os.environ.get('WOODAI_USER_AUTH')
-    env = os.environ.get('WOODAI_RUNTIME_ENV')
-    url_prefix = ''
-    if (env == 'dev'):
-        url_prefix = 'dev-'
-    elif (env == 'test'):
-        url_prefix = 'test-'
-    elif (env == 'staging'):
-        url_prefix = 'staging-'
+    token = os.environ.get("WOODAI_USER_AUTH")
+    env = os.environ.get("WOODAI_RUNTIME_ENV")
+    url_prefix = ""
+    if env == "dev":
+        url_prefix = "dev-"
+    elif env == "test":
+        url_prefix = "test-"
+    elif env == "staging":
+        url_prefix = "staging-"
     if token is None:
-        raise RuntimeError('用户未登录，无法使用 AI chat 功能，请登录后重试')
+        raise RuntimeError("用户未登录，无法使用 AI chat 功能，请登录后重试")
     if ws is None or ws.connected is False:
-        stag = 3
+        stag = "3"
         model = "ALIYUN-QWENPTURBO"
+        websocket.sock_opt.sslopt = {"cert_reqs": ssl.CERT_NONE}
         ws = websocket.create_connection(
-            f"wss://{url_prefix}cr-aichat.codemao.cn/aichat/?EIO=3&transport=websocket&stag={stag}&model={model}&token={token}"
+            "ws://"
+            + url_prefix
+            + "cr-aichat.codemao.cn/aichat/?EIO=3&transport=websocket&stag="
+            + stag
+            + "&model="
+            + model
+            + "&token="
+            + token
         )
         wait_until_connect(ws)
     return ws
 
 
 def chat_set(system_role: str = "你是一个友好的AI助手", turn_count: int = 3):
     if len(system_role) > 30:
@@ -138,15 +150,15 @@
         data = parse_message(rec)
         name = data["type"]
         payload = data["payload"]
         if name != "chat_ack":
             continue
         if payload["code"] != 1:
             ws.close()
-            raise generate_default_error(payload['code'])
+            raise generate_default_error(payload["code"])
         if payload["data"]["content_type"] == "stream_output_begin":
             answer = ""
         if payload["data"]["content_type"] == "stream_output_content":
             answer += payload["data"]["content"]
             if output:
                 print(payload["data"]["content"], end="", flush=True)
         if payload["data"]["content_type"] == "stream_output_end":
@@ -162,9 +174,9 @@
         rec = ws.recv()
         data = parse_message(rec)
         name = data["type"]
         payload = data["payload"]
         if name == "clear_chatting_msg_ack":
             if payload["code"] != 1:
                 ws.close()
-                raise generate_default_error(payload['code'])
+                raise generate_default_error(payload["code"])
             break
```

## Comparing `woodAI-1.0.0.dist-info/LICENSE.txt` & `woodAI-1.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

