# Comparing `tmp/privacera_shield-1.1.4-py3-none-any.whl.zip` & `tmp/privacera_shield-1.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 37205 bytes, number of entries: 20
+Zip file size: 37234 bytes, number of entries: 20
 -rw-r--r--  2.0 unx     1682 b- defN 20-Feb-02 00:00 privacera_shield/PluginAccessRequestEncryptor.py
 -rw-r--r--  2.0 unx       10 b- defN 20-Feb-02 00:00 privacera_shield/__init__.py
--rw-r--r--  2.0 unx    28024 b- defN 20-Feb-02 00:00 privacera_shield/backend.py
+-rw-r--r--  2.0 unx    28741 b- defN 20-Feb-02 00:00 privacera_shield/backend.py
 -rw-r--r--  2.0 unx     5605 b- defN 20-Feb-02 00:00 privacera_shield/client.py
--rw-r--r--  2.0 unx    40459 b- defN 20-Feb-02 00:00 privacera_shield/core.py
+-rw-r--r--  2.0 unx    39974 b- defN 20-Feb-02 00:00 privacera_shield/core.py
 -rw-r--r--  2.0 unx     6927 b- defN 20-Feb-02 00:00 privacera_shield/encryption.py
 -rw-r--r--  2.0 unx      642 b- defN 20-Feb-02 00:00 privacera_shield/exception.py
 -rw-r--r--  2.0 unx     4407 b- defN 20-Feb-02 00:00 privacera_shield/interceptor.py
 -rw-r--r--  2.0 unx      963 b- defN 20-Feb-02 00:00 privacera_shield/interceptor_setup.py
 -rw-r--r--  2.0 unx    14330 b- defN 20-Feb-02 00:00 privacera_shield/langchain_callback.py
--rw-r--r--  2.0 unx    16563 b- defN 20-Feb-02 00:00 privacera_shield/langchain_method_interceptor.py
+-rw-r--r--  2.0 unx    16229 b- defN 20-Feb-02 00:00 privacera_shield/langchain_method_interceptor.py
 -rw-r--r--  2.0 unx     7277 b- defN 20-Feb-02 00:00 privacera_shield/langchain_streaming_interceptor.py
 -rw-r--r--  2.0 unx     5734 b- defN 20-Feb-02 00:00 privacera_shield/message.py
 -rw-r--r--  2.0 unx     7575 b- defN 20-Feb-02 00:00 privacera_shield/milvus_method_interceptor.py
 -rw-r--r--  2.0 unx      600 b- defN 20-Feb-02 00:00 privacera_shield/model.py
 -rw-r--r--  2.0 unx     2616 b- defN 20-Feb-02 00:00 privacera_shield/util.py
-?rw-r--r--  2.0 unx      842 b- defN 20-Feb-02 00:00 privacera_shield-1.1.4.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 privacera_shield-1.1.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx       17 b- defN 20-Feb-02 00:00 privacera_shield-1.1.4.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1785 b- defN 20-Feb-02 00:00 privacera_shield-1.1.4.dist-info/RECORD
-20 files, 146145 bytes uncompressed, 34253 bytes compressed:  76.6%
+?rw-r--r--  2.0 unx      888 b- defN 20-Feb-02 00:00 privacera_shield-1.1.5.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 privacera_shield-1.1.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx       17 b- defN 20-Feb-02 00:00 privacera_shield-1.1.5.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1785 b- defN 20-Feb-02 00:00 privacera_shield-1.1.5.dist-info/RECORD
+20 files, 146089 bytes uncompressed, 34282 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: privacera_shield/model.py
 Comment: 
 
 Filename: privacera_shield/util.py
 Comment: 
 
-Filename: privacera_shield-1.1.4.dist-info/METADATA
+Filename: privacera_shield-1.1.5.dist-info/METADATA
 Comment: 
 
-Filename: privacera_shield-1.1.4.dist-info/WHEEL
+Filename: privacera_shield-1.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: privacera_shield-1.1.4.dist-info/licenses/LICENSE
+Filename: privacera_shield-1.1.5.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: privacera_shield-1.1.4.dist-info/RECORD
+Filename: privacera_shield-1.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## privacera_shield/backend.py

```diff
@@ -45,15 +45,14 @@
         self.request_id = kwargs.get('request_id')
         self.user_name = kwargs.get('user_name')
         self.context = kwargs.get('context', {})
         self.request_text = kwargs.get('request_text')
         self.conversation_type = kwargs.get('conversation_type', ConversationType.PROMPT)
         self.shield_server_key_id = kwargs.get('shield_server_key_id', None)
         self.shield_plugin_key_id = kwargs.get('shield_plugin_key_id', None)
-        self.shield_run_mode = kwargs.get('shield_run_mode', "freemium")
         self.enable_audit = kwargs.get('enable_audit', True)
 
     def to_payload_dict(self):
         """
         Serialize the ShieldAccessRequest instance to a JSON string.
 
         Returns:
@@ -202,15 +201,14 @@
 
     def __init__(self, **kwargs):
         self.application_key = kwargs.get('application_key')
         self.client_application_key = kwargs.get('client_application_key')
         self.conversation_thread_id = kwargs.get('conversation_thread_id')
         self.request_id = kwargs.get('request_id')
         self.user_name = kwargs.get('user_name')
-        self.shield_run_mode = kwargs.get('shield_run_mode', "freemium")
 
     def to_payload_dict(self):
         """
                 Serialize the VectorDBAccessRequest instance to a JSON string.
 
                 Returns:
                     str: JSON representation of the instance.
@@ -299,15 +297,14 @@
             messages (list): List of messages associated with the request (default is an empty list).
             ranger_audit_ids (list): List of Ranger audit IDs (default is an empty list).
             ranger_policy_ids (list): List of Ranger policy IDs (default is an empty list).
             paig_policy_ids (list): List of PAIG policy IDs (default is an empty list).
             client_ip (str): The IP address of the client.
             client_hostname (str): The hostname of the client.
             number_of_tokens (int): The number of tokens (default is 0).
-            shield_run_mode (str): The shield run mode (default is "freemium").
             encryption_key_id (str): The ID of the encryption key (default is None).
         """
 
         self.event_time = kwargs.get("event_time")
         self.tenant_id = kwargs.get("tenant_id")
         self.conversation_id = kwargs.get("conversation_id")
         self.request_id = kwargs.get("request_id")
@@ -326,16 +323,14 @@
         self.ranger_audit_ids = kwargs.get("ranger_audit_ids", [])
         self.ranger_policy_ids = kwargs.get("ranger_policy_ids", [])
         self.paig_policy_ids = kwargs.get("paig_policy_ids", [])
         self.client_ip = kwargs.get("client_ip")
         self.client_hostname = kwargs.get("client_hostname")
         self.number_of_tokens = kwargs.get("number_of_tokens", 0)
 
-        self.shield_run_mode = kwargs.get('shield_run_mode', "freemium")
-
         # This is shield server key id
         self.encryption_key_id = kwargs.get('encryption_key_id', None)
 
     def to_payload_dict(self):
         """
         Returns a dictionary representation of the StreamAccessAuditRequest object.
 
@@ -368,14 +363,52 @@
             "numberOfTokens": self.number_of_tokens,
 
             "encryptionKeyId": self.encryption_key_id
         }
 
         return request_dict
 
+    @classmethod
+    def from_payload_dict(cls, payload_dict):
+        """
+        Creates a StreamAccessAuditRequest object from a dictionary payload.
+
+        Args:
+            payload_dict (dict): Dictionary containing attributes of the request.
+
+        Returns:
+            StreamAccessAuditRequest: An instance of StreamAccessAuditRequest.
+        """
+        kwargs = {
+            "event_time": payload_dict.get("eventTime"),
+            "tenant_id": payload_dict.get("tenantId"),
+            "conversation_id": payload_dict.get("conversationId"),
+            "request_id": payload_dict.get("requestId"),
+            "thread_id": payload_dict.get("threadId"),
+            "thread_sequence_number": payload_dict.get("threadSequenceNumber"),
+            "request_type": payload_dict.get("requestType"),
+            "user_id": payload_dict.get("userId"),
+            "client_application_key": payload_dict.get("clientApplicationKey"),
+            "application_key": payload_dict.get("applicationKey"),
+            "application_name": payload_dict.get("applicationName"),
+            "result": payload_dict.get("result"),
+            "traits": payload_dict.get("traits", []),
+            "masked_traits": payload_dict.get("maskedTraits", {}),
+            "context": payload_dict.get("context", {}),
+            "messages": payload_dict.get("messages", []),
+            "ranger_audit_ids": payload_dict.get("rangerAuditIds", []),
+            "ranger_policy_ids": payload_dict.get("rangerPolicyIds", []),
+            "paig_policy_ids": payload_dict.get("paigPolicyIds", []),
+            "client_ip": payload_dict.get("clientIp"),
+            "client_hostname": payload_dict.get("clientHostname"),
+            "number_of_tokens": payload_dict.get("numberOfTokens", 0),
+            "encryption_key_id": payload_dict.get("encryptionKeyId")
+        }
+        return cls(**kwargs)
+
 
 class HttpTransport:
     """
     HttpTransport class maintains a single instance of urllib3.PoolManager for all the ShieldRestHttpClient instances.
     """
     _http: urllib3.PoolManager = None
     _rw_lock = threading.RLock()
@@ -450,14 +483,17 @@
         self.request_kwargs = kwargs.get('request_kwargs', {})
         if 'timeout' not in self.request_kwargs:
             self.request_kwargs['timeout'] = Timeout(connect=2.0, read=7.0)
 
         self.plugin_access_request_encryptor = PluginAccessRequestEncryptor(self.tenant_id,
                                                                             kwargs["encryption_keys_info"])
 
+    def get_plugin_access_request_encryptor(self):
+        return self.plugin_access_request_encryptor
+
     def get_default_headers(self):
         headers = dict()
         if self.tenant_id:
             headers["x-tenant-id"] = self.tenant_id
         if self.api_key:
             headers["x-paig-api-key"] = self.api_key
         return headers
@@ -472,17 +508,16 @@
         Returns:
             ShieldAccessResult: The result of the access check.
         """
 
         if _logger.isEnabledFor(logging.DEBUG):
             _logger.debug(f"Access request parameters: {request.to_payload_dict()}")
 
-        if request.shield_run_mode == "freemium":
-            # Encrypt the request messages and set the encryption key id and plugin public key in request
-            self.plugin_access_request_encryptor.encrypt_request(request)
+        # Encrypt the request messages and set the encryption key id and plugin public key in request
+        self.plugin_access_request_encryptor.encrypt_request(request)
 
         request.shield_server_key_id = self.plugin_access_request_encryptor.shield_server_key_id
         request.shield_plugin_key_id = self.plugin_access_request_encryptor.shield_plugin_key_id
 
         if _logger.isEnabledFor(logging.DEBUG):
             _logger.debug(f"Access request parameters (encrypted): {request.to_payload_dict()}")
 
@@ -493,15 +528,15 @@
                                                     **self.request_kwargs)
 
         if _logger.isEnabledFor(logging.DEBUG):
             _logger.debug(f"Access response status (encrypted): {response.status}, body: {response.data}")
 
         if response.status == 200:
             access_result = ShieldAccessResult.from_json(**response.json())
-            if access_result.isAllowed and request.shield_run_mode == "freemium":
+            if access_result.isAllowed:
                 # Decrypt the response messages
                 self.plugin_access_request_encryptor.decrypt_response(access_result)
                 if _logger.isEnabledFor(logging.DEBUG):
                     _logger.debug(
                         f"Access response status: {response.status}, access_result: {json.dumps(access_result.__dict__)}")
             return access_result
         else:
@@ -599,30 +634,14 @@
         Returns:
             None
         """
 
         if _logger.isEnabledFor(logging.DEBUG):
             _logger.debug(f"Stream access audit request parameters: {request.to_payload_dict()}")
 
-        if request.shield_run_mode == "freemium":
-            # Encrypt the messages and set the encryption key id and plugin public key in request
-            messages = request.messages
-            encrypted_messages = []
-            for message in messages:
-                message["originalMessage"] = self.plugin_access_request_encryptor.encrypt_message(message["originalMessage"])
-                message["maskedMessage"] = self.plugin_access_request_encryptor.encrypt_message(message["maskedMessage"])
-                encrypted_messages.append(message)
-
-            request.messages = encrypted_messages
-
-        request.encryption_key_id = self.plugin_access_request_encryptor.shield_server_key_id
-
-        if _logger.isEnabledFor(logging.DEBUG):
-            _logger.debug(f"Stream access audit request parameters (encrypted): {request.to_payload_dict()}")
-
         response = HttpTransport.get_http().request(method="POST",
                                                     url=self.base_url + "/shield/audit",
                                                     headers=self.get_default_headers(),
                                                     json=request.to_payload_dict(),
                                                     **self.request_kwargs)
 
         if _logger.isEnabledFor(logging.DEBUG):
```

## privacera_shield/core.py

```diff
@@ -3,14 +3,15 @@
 import os
 import threading
 import time
 import uuid
 from queue import Queue
 
 from . import interceptor_setup, util
+from privacera_shield_common.audit_spooler import AuditLogger
 from .backend import ShieldRestHttpClient, ShieldAccessRequest, HttpTransport, VectorDBAccessRequest, \
     ShieldAccessResult, StreamAccessAuditRequest
 from .exception import PAIGException, AccessControlException
 from .message import ErrorMessage, InfoMessage, WarningMessage
 from .model import ConversationType
 
 _logger = logging.getLogger(__name__)
@@ -116,17 +117,14 @@
 
     def get_application_key(self):
         return self.get_current_application().get_application_key()
 
     def get_client_application_key(self):
         return self.get_current_application().get_client_application_key()
 
-    def get_shield_run_mode(self):
-        return self.get_current_application().get_shield_run_mode()
-
     def setup(self):
         """
         Set up the PAIG plugin by intercepting methods for enhanced functionality.
         """
         if self.enable_privacera_shield:
             self.interceptor_installer_list = interceptor_setup.setup(self)
 
@@ -199,15 +197,15 @@
         Gets or creates an instance of StreamAuditLogger.
 
         Returns:
             StreamAuditLogger: An instance of StreamAuditLogger.
         """
         return self.get_current_application().get_or_create_llm_stream_audit_logger()
 
-    def log_stream_access_audit(self, audit_log_request : StreamAccessAuditRequest):
+    def log_stream_access_audit(self, audit_log_request: StreamAccessAuditRequest):
         """
         Logs a stream access audit.
 
         Args:
             audit_log_request (StreamAccessAuditRequest): The StreamAccessAuditRequest object containing the audit log details.
         """
         self.get_current_application().log_stream_access_audit(audit_log_request)
@@ -437,15 +435,14 @@
          tenant_id (str): The ID of the tenant using the plugin.
          shield_base_url (str): The base URL for the Shield service.
          api_key (str): The API key.
          shield_server_key_id (str): The key ID for the Shield server.
          shield_server_public_key (str): The public key for the Shield server.
          shield_plugin_key_id (str): The key ID for the Shield plugin.
          shield_plugin_private_key (str): The private key for the Shield plugin.
-         shield_run_mode (str): The run mode for the Shield plugin.
          shield_client: An instance of the ShieldRestHttpClient class for making requests to the Shield service.
          request_kwargs: The keyword arguments to be passed to the ShieldRestHttpClient class.
      """
 
     def __init__(self, **kwargs):
         """
         Initializes an instance of the PAIGPlugin class.
@@ -473,16 +470,15 @@
         else:
             self.shield_base_url = plugin_app_config_dict.get("apiServerUrl")
         self.api_key = plugin_app_config_dict.get("apiKey")
         self.shield_server_key_id = plugin_app_config_dict.get("shieldServerKeyId")
         self.shield_server_public_key = plugin_app_config_dict.get("shieldServerPublicKey")
         self.shield_plugin_key_id = plugin_app_config_dict.get("shieldPluginKeyId")
         self.shield_plugin_private_key = plugin_app_config_dict.get("shieldPluginPrivateKey")
-
-        self.shield_run_mode = plugin_app_config_dict.get("shieldRunMode", "freemium")
+        self.audit_spool_dir = plugin_app_config_dict.get("auditSpoolDir", "spool/audits/")
 
         # Allow override from kwargs
         for key, value in kwargs.items():
             if key in self.__dict__:
                 self.__dict__[key] = value
 
         encryption_keys_info = {
@@ -598,17 +594,14 @@
 
     def get_application_key(self):
         return self.application_key
 
     def get_client_application_key(self):
         return self.client_application_key
 
-    def get_shield_run_mode(self):
-        return self.shield_run_mode
-
     def authorize(self, **kwargs) -> ShieldAccessResult:
         access_request = kwargs.get("access_request")
         if access_request is None:
             if "text" not in kwargs:
                 raise PAIGException(ErrorMessage.PROMPT_NOT_PROVIDED)
             if "conversation_type" not in kwargs:
                 raise PAIGException(ErrorMessage.CONVERSATION_TYPE_NOT_PROVIDED)
@@ -623,15 +616,14 @@
                 conversation_thread_id=kwargs.get("thread_id", _paig_plugin.generate_conversation_thread_id()),
                 stream_id=kwargs.get("stream_id", None),
                 request_id=_paig_plugin.generate_request_id(),
                 user_name=_paig_plugin.get_current_user(),
                 context=ShieldAccessRequest.create_request_context(paig_plugin=_paig_plugin),
                 request_text=text if isinstance(text, list) else [text],
                 conversation_type=conversation_type,
-                shield_run_mode=self.shield_run_mode,
                 enable_audit=kwargs.get("enable_audit", True),
             )
         return self.get_shield_client().is_access_allowed(request=access_request)
 
     def check_access(self, **kwargs):
         access_result = self.authorize(**kwargs)
         if not access_result.get_is_allowed():
@@ -645,16 +637,15 @@
             global _paig_plugin
 
             access_request = VectorDBAccessRequest(
                 application_key=self.get_application_key(),
                 client_application_key=self.get_client_application_key(),
                 conversation_thread_id=kwargs.get("thread_id", _paig_plugin.generate_conversation_thread_id()),
                 request_id=_paig_plugin.generate_request_id(),
-                user_name=_paig_plugin.get_current_user(),
-                shield_run_mode=self.shield_run_mode
+                user_name=_paig_plugin.get_current_user()
             )
 
         access_result = self.get_shield_client().get_filter_expression(request=access_request)
         # In case if there is no policy to be evaluated for current user then we will get blank filter
         shield_filter_expr = access_result.get_filter_expression()
         # Setting the received shield_filter_expr inside context, so we can pass it for auditing when sending next
         # request for prompt authorization
@@ -671,29 +662,52 @@
 
         Returns:
             StreamAuditLogger: An instance of StreamAuditLogger.
 
         """
         if self.llm_stream_audit_logger is None:
             # Create an instance of StreamAuditLogger with shieldRestHttpClient as input
-            self.llm_stream_audit_logger = StreamAuditLogger(self.shield_client)
+            self.llm_stream_audit_logger = StreamAuditLogger(self.shield_client, self.audit_spool_dir)
 
             # Start the StreamAuditLogger thread
             self.llm_stream_audit_logger.start()
 
         return self.llm_stream_audit_logger
 
-    def log_stream_access_audit(self, audit_log_request : StreamAccessAuditRequest):
+    def log_stream_access_audit(self, audit_log_request: StreamAccessAuditRequest):
         """
         Logs a stream access audit.
 
         Args:
             audit_log_request (StreamAccessAuditRequest): The StreamAccessAuditRequest object containing the audit log details.
 
         """
+
+        plugin_access_request_encryptor = self.shield_client.get_plugin_access_request_encryptor()
+
+        if _logger.isEnabledFor(logging.DEBUG):
+            _logger.debug(f"Stream access audit request parameters: {audit_log_request.to_payload_dict()}")
+
+        # Encrypt the messages and set the encryption key id and plugin public key in request
+        messages = audit_log_request.messages
+        encrypted_messages = []
+        for message in messages:
+            message["originalMessage"] = plugin_access_request_encryptor.encrypt_message(
+                message["originalMessage"])
+            message["maskedMessage"] = plugin_access_request_encryptor.encrypt_message(
+                message["maskedMessage"])
+            encrypted_messages.append(message)
+
+        audit_log_request.messages = encrypted_messages
+
+        audit_log_request.encryption_key_id = plugin_access_request_encryptor.shield_server_key_id
+
+        if _logger.isEnabledFor(logging.DEBUG):
+            _logger.debug(f"Stream access audit request parameters (encrypted): {audit_log_request.to_payload_dict()}")
+
         llm_stream_audit_logger = self.get_or_create_llm_stream_audit_logger()
         llm_stream_audit_logger.log(audit_log_request)
 
 
 class LLMStreamAccessChecker:
     """
     Class for checking access on streaming data using the LLM model.
@@ -853,16 +867,14 @@
         ranger_policy_ids = []
         paig_policy_ids = []
 
         # Get client IP address and hostname
         client_ip = util.get_my_ip_address()
         client_hostname = util.get_my_hostname()
 
-        shield_run_mode = self.paig_plugin.get_current_application().get_shield_run_mode()
-
         # Initialize counters for allowed and denied responses
         allowed_count = 0
         denied_count = 0
 
         # Iterate over all responses from the shield server for the stream
         for record in self.shield_access_response_list:
             # Update counters based on whether the response is allowed or denied
@@ -916,16 +928,15 @@
             traits=traits,
             masked_traits=masked_traits,
             messages=messages,
             ranger_audit_ids=ranger_audit_ids,
             ranger_policy_ids=ranger_policy_ids,
             paig_policy_ids=paig_policy_ids,
             client_ip=client_ip,
-            client_hostname=client_hostname,
-            shield_run_mode=shield_run_mode,
+            client_hostname=client_hostname
         )
 
         return stream_access_audit_request
 
     def flush_audits(self):
         """
         Flushes the audit logs.
@@ -938,58 +949,30 @@
         if len(self.shield_access_response_list) > 0:
             stream_access_audit_request = self.create_stream_access_audit_request()
             self.paig_plugin.log_stream_access_audit(stream_access_audit_request)
         else:
             _logger.warning(f"No stream audits founds to be pushed")
 
 
-class StreamAuditLogger(threading.Thread):
+class StreamAuditLogger(AuditLogger):
     """
     A class to log audit data and push it to a server.
 
     Attributes:
         shield_rest_http_client (object): An object representing the REST HTTP client.
         audit_log_request_queue (Queue): A queue to store audit log data.
     """
 
-    def __init__(self, shield_rest_http_client: ShieldRestHttpClient):
+    def __init__(self, shield_rest_http_client: ShieldRestHttpClient, audit_spool_dir: str):
         """
         Initializes the StreamAuditLogger.
 
         Args:
             shield_rest_http_client (object): An object representing the REST HTTP client.
+            audit_spool_dir (str): Audit spool directory
         """
-        super().__init__()
-        self.shield_rest_http_client = shield_rest_http_client
-        self.audit_log_request_queue = Queue(maxsize=10000)
-
-    def log(self, audit_log_request: StreamAccessAuditRequest):
-        """
-        Logs the provided data.
-
-        Args:
-            audit_log_request (dict): The audit log request to be logged.
-        """
-        self.audit_log_request_queue.put(audit_log_request)
+        super().__init__(audit_spool_dir=audit_spool_dir, audit_event_cls=StreamAccessAuditRequest)
 
-    def run(self):
-        """
-        Runs the StreamAuditLogger thread.
+        self.shield_rest_http_client = shield_rest_http_client
 
-        Continuously checks for new logs in the audit_log_request_queue and pushes them to the server.
-        """
-        try:
-            while True:
-                # Check for new logs in the audit_log_request_queue
-                # This is a blocking queue, it will implicitly wait till record available in queue
-                audit_log_request = self.audit_log_request_queue.get()
-                try:
-                    # Push log to server using restHttpClient
-                    self.shield_rest_http_client.log_stream_access_audit(audit_log_request)
-                    if _logger.isEnabledFor(logging.DEBUG):
-                        _logger.debug("Audit log data pushed to server: %s", audit_log_request)
-                except Exception as e:
-                    _logger.error("Failed to push audit log data %s to server: %s", audit_log_request, e)
-                    # Adding it back to the queue for retry
-                    self.log(audit_log_request)
-        except Exception as e:
-            _logger.error("An error occurred in StreamAuditLogger: %s", e)
+    def push_audit_event_to_server(self, audit_event: StreamAccessAuditRequest):
+        self.shield_rest_http_client.log_stream_access_audit(audit_event)
```

## privacera_shield/langchain_method_interceptor.py

```diff
@@ -139,16 +139,15 @@
             application_key=self.paig_plugin.get_application_key(),
             client_application_key=self.paig_plugin.get_client_application_key(),
             conversation_thread_id=self.paig_plugin.generate_conversation_thread_id(),
             request_id=self.paig_plugin.generate_request_id(),
             user_name=self.paig_plugin.get_current_user(),
             context=ShieldAccessRequest.create_request_context(paig_plugin=self.paig_plugin),
             request_text=args[0],
-            conversation_type=ConversationType.PROMPT,
-            shield_run_mode=self.paig_plugin.get_shield_run_mode()
+            conversation_type=ConversationType.PROMPT
         )
 
         access_result = self.paig_plugin.get_shield_client().is_access_allowed(access_request)
 
         # Throw exception if access is denied
         self.check_access(access_result)
 
@@ -187,16 +186,15 @@
                     application_key=self.paig_plugin.get_application_key(),
                     client_application_key=self.paig_plugin.get_client_application_key(),
                     conversation_thread_id=self.paig_plugin.generate_conversation_thread_id(),
                     request_id=self.paig_plugin.generate_request_id(),
                     user_name=self.paig_plugin.get_current_user(),
                     context=ShieldAccessRequest.create_request_context(paig_plugin=self.paig_plugin),
                     request_text=request_text,
-                    conversation_type=ConversationType.REPLY,
-                    shield_run_mode=self.paig_plugin.get_shield_run_mode()
+                    conversation_type=ConversationType.REPLY
                 )
 
                 access_result = self.paig_plugin.get_shield_client().is_access_allowed(access_request)
 
                 # Throw exception if access is denied
                 self.check_access(access_result)
 
@@ -260,16 +258,15 @@
                 application_key=self.paig_plugin.get_application_key(),
                 client_application_key=self.paig_plugin.get_client_application_key(),
                 conversation_thread_id=self.paig_plugin.thread_local.conversation_thread_id,
                 request_id=self.paig_plugin.generate_request_id(),
                 user_name=self.paig_plugin.get_current_user(),
                 context=ShieldAccessRequest.create_request_context(paig_plugin=self.paig_plugin),
                 request_text=args[0]["question"],
-                conversation_type=ConversationType.PROMPT,
-                shield_run_mode=self.paig_plugin.shield_run_mode
+                conversation_type=ConversationType.PROMPT
             )
 
             access_result = self.paig_plugin.get_shield_client().is_access_allowed(access_request)
 
             # Throw exception if access is denied
             self.check_access(access_result)
 
@@ -342,16 +339,15 @@
             application_key=self.paig_plugin.get_application_key(),
             client_application_key=self.paig_plugin.get_client_application_key(),
             conversation_thread_id=self.paig_plugin.generate_conversation_thread_id(),
             request_id=self.paig_plugin.generate_request_id(),
             user_name=self.paig_plugin.get_current_user(),
             context=ShieldAccessRequest.create_request_context(paig_plugin=self.paig_plugin),
             request_text=[args[0]],
-            conversation_type=ConversationType.PROMPT,
-            shield_run_mode=self.paig_plugin.shield_run_mode
+            conversation_type=ConversationType.PROMPT
         )
 
         access_result = self.paig_plugin.get_shield_client().is_access_allowed(access_request)
 
         # Throw exception if access is denied
         self.check_access(access_result)
 
@@ -376,16 +372,15 @@
             application_key=self.paig_plugin.get_application_key(),
             client_application_key=self.paig_plugin.get_client_application_key(),
             conversation_thread_id=self.paig_plugin.generate_conversation_thread_id(),
             request_id=self.paig_plugin.generate_request_id(),
             user_name=self.paig_plugin.get_current_user(),
             context=ShieldAccessRequest.create_request_context(paig_plugin=self.paig_plugin),
             request_text=[output],
-            conversation_type=ConversationType.REPLY,
-            shield_run_mode=self.paig_plugin.shield_run_mode
+            conversation_type=ConversationType.REPLY
         )
 
         access_result = self.paig_plugin.get_shield_client().is_access_allowed(access_request)
 
         # Throw exception if access is denied
         self.check_access(access_result)
```

## Comparing `privacera_shield-1.1.4.dist-info/METADATA` & `privacera_shield-1.1.5.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.3
 Name: privacera_shield
-Version: 1.1.4
+Version: 1.1.5
 Summary: Privacera AI Governance (PAIG) Shield Plugin Library
 Project-URL: Homepage, https://github.com/pypa/privacera_shield
 Project-URL: Bug Tracker, https://github.com/pypa/privacera_shield/issues
 Author-email: PAIG Shield <paig@privacera.com>
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8.1
 Requires-Dist: cryptography>=41.0.4
+Requires-Dist: privacera-shield-common==1.0.0
 Requires-Dist: urllib3>=2.0.6
 Description-Content-Type: text/markdown
 
 # Privacera AI Goverance Shield Library
 
 The `privacera_shield` library allows you to seamlessly integrate Privacera AI Governance into your Langchain projects.
```

## Comparing `privacera_shield-1.1.4.dist-info/RECORD` & `privacera_shield-1.1.5.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 privacera_shield/PluginAccessRequestEncryptor.py,sha256=vPuctK9G-eulvFLqEK5_-2wE16Y9OXd0iedOiUQyz-w,1682
 privacera_shield/__init__.py,sha256=UnxmjVrk-eNORsitiM48W0pB6yfsaErOak8RYh_ELt8,10
-privacera_shield/backend.py,sha256=It6QURd7BNNZ7MYhwuVynMuJ2IG1z1vdJ6ZYYXIM4xQ,28024
+privacera_shield/backend.py,sha256=FSln0S47zeenigv75-O8xp5uHFVdoGFF1MRnvMpTPo0,28741
 privacera_shield/client.py,sha256=7MNwv7xullB9fXV4KV13Vc_hJmJk2EAVpTS94emWzzw,5605
-privacera_shield/core.py,sha256=bes54DhSGzue6L_fdfhq_Vm08NlOkH0im6Dxo2vJhs4,40459
+privacera_shield/core.py,sha256=Aur3FuRlhB7bsUX647rj9sRZlbMBagJHtUETAMRnQyc,39974
 privacera_shield/encryption.py,sha256=pOW5gLrho9oAqK2Z9Pm6tw59fUDL61e4v_TcSjr2dKE,6927
 privacera_shield/exception.py,sha256=__5EU2XWjig09R3wg8eAde6mFFLex0Zthk_CpKIeq6s,642
 privacera_shield/interceptor.py,sha256=MKYECHkYiyuf8eRbtdJi8NBmR09i-UPFQuVwOoOQVZQ,4407
 privacera_shield/interceptor_setup.py,sha256=hcx7jiNk4wT0c3LngkhVOJtJRRkyXVtdLkeSWDeJMzE,963
 privacera_shield/langchain_callback.py,sha256=7uXyZmyBpS9ifG0pYbRVFW3pMRpD3ZOiWbE9lMtXNTg,14330
-privacera_shield/langchain_method_interceptor.py,sha256=H4CFRhak7hJan7Nlkfe5ycWUTFBP5wKTFmoL-cViHfQ,16563
+privacera_shield/langchain_method_interceptor.py,sha256=Crohb-qjmKglU4xClWaj3o-mTM5By4THQ2JJRFvbJWU,16229
 privacera_shield/langchain_streaming_interceptor.py,sha256=-YVe8J11X6gopGsnEjN9P-vBBG0AEU5N98fBO2QLvws,7277
 privacera_shield/message.py,sha256=ymFaVHs28MZuHs50AkunbU43PVhV5R2UxwPMiJb4U_s,5734
 privacera_shield/milvus_method_interceptor.py,sha256=E-HoAd_1OwYtfhibqpjet1ZIIakX8kJssPbUaqgXpao,7575
 privacera_shield/model.py,sha256=DYivnpTvFCrTyotnUThN-_VyJwiKleoN6D3_Cddt5ZE,600
 privacera_shield/util.py,sha256=WLsdCnAAQLasvVvXebWoyHDbfgk6fNlTE8ho-NJhTpY,2616
-privacera_shield-1.1.4.dist-info/METADATA,sha256=V_98PEDgDiECUjJiqVY91KSeTtgTgIcw59__5_b1SB8,842
-privacera_shield-1.1.4.dist-info/WHEEL,sha256=uNdcs2TADwSd5pVaP0Z_kcjcvvTUklh2S7bxZMF8Uj0,87
-privacera_shield-1.1.4.dist-info/licenses/LICENSE,sha256=141Y00luDiocNKqpg-owxKfwapO9XSfng11NjgHWAmQ,17
-privacera_shield-1.1.4.dist-info/RECORD,,
+privacera_shield-1.1.5.dist-info/METADATA,sha256=iTzLKYXgp8cJNtp0QeW8kmV1GrHz9YWRz6XkfQ9e06Q,888
+privacera_shield-1.1.5.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+privacera_shield-1.1.5.dist-info/licenses/LICENSE,sha256=141Y00luDiocNKqpg-owxKfwapO9XSfng11NjgHWAmQ,17
+privacera_shield-1.1.5.dist-info/RECORD,,
```

