# Comparing `tmp/iudex-0.4.9.tar.gz` & `tmp/iudex-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iudex-0.4.9.tar", max compression
+gzip compressed data, was "iudex-0.5.0.tar", max compression
```

## Comparing `iudex-0.4.9.tar` & `iudex-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,11 @@
--rw-r--r--   0        0        0    11357 2024-03-05 02:32:42.683184 iudex-0.4.9/LICENSE
--rw-r--r--   0        0        0     8426 2024-05-07 17:48:23.958486 iudex-0.4.9/README.md
--rw-r--r--   0        0        0       54 2024-03-05 02:32:42.685374 iudex-0.4.9/iudex/__init__.py
--rw-r--r--   0        0        0     7348 2024-03-22 23:11:09.655241 iudex-0.4.9/iudex/chat.py
--rw-r--r--   0        0        0     7295 2024-03-22 23:11:09.655456 iudex-0.4.9/iudex/client.py
--rw-r--r--   0        0        0     1653 2024-03-22 23:11:09.655988 iudex-0.4.9/iudex/functions.py
--rw-r--r--   0        0        0     1402 2024-05-10 22:37:34.746644 iudex-0.4.9/iudex/instrumentation/README.md
--rw-r--r--   0        0        0      136 2024-05-11 00:45:08.006406 iudex-0.4.9/iudex/instrumentation/__init__.py
--rw-r--r--   0        0        0     2821 2024-05-10 22:37:34.746966 iudex-0.4.9/iudex/instrumentation/attributes.py
--rw-r--r--   0        0        0     1923 2024-05-12 20:44:31.688333 iudex-0.4.9/iudex/instrumentation/fastapi.py
--rw-r--r--   0        0        0     5747 2024-05-12 20:42:37.749677 iudex-0.4.9/iudex/instrumentation/instrumentation.py
--rw-r--r--   0        0        0     1470 2024-05-12 07:34:47.015381 iudex-0.4.9/iudex/instrumentation/lambda.py
--rw-r--r--   0        0        0      236 2024-03-05 02:32:42.686766 iudex-0.4.9/iudex/resource.py
--rw-r--r--   0        0        0     4349 2024-03-22 23:11:09.656442 iudex-0.4.9/iudex/types/function.py
--rw-r--r--   0        0        0      137 2024-03-06 19:49:41.321305 iudex-0.4.9/iudex/utils.py
--rw-r--r--   0        0        0      667 2024-05-12 20:44:07.476957 iudex-0.4.9/pyproject.toml
--rw-r--r--   0        0        0     9170 1970-01-01 00:00:00.000000 iudex-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-26 21:03:01.210390 iudex-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1502 2024-05-17 01:14:03.519309 iudex-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 01:39:19.649489 iudex-0.5.0/iudex/__init__.py
+-rw-r--r--   0        0        0     1502 2024-05-14 23:55:03.479188 iudex-0.5.0/iudex/instrumentation/README.md
+-rw-r--r--   0        0        0      106 2024-05-17 01:17:53.127532 iudex-0.5.0/iudex/instrumentation/__init__.py
+-rw-r--r--   0        0        0     2821 2024-05-10 20:15:13.224407 iudex-0.5.0/iudex/instrumentation/attributes.py
+-rw-r--r--   0        0        0     1974 2024-05-14 23:55:03.479780 iudex-0.5.0/iudex/instrumentation/fastapi.py
+-rw-r--r--   0        0        0     6043 2024-05-17 01:33:17.021670 iudex-0.5.0/iudex/instrumentation/instrumentation.py
+-rw-r--r--   0        0        0     1517 2024-05-17 01:41:47.528945 iudex-0.5.0/iudex/instrumentation/lambda.py
+-rw-r--r--   0        0        0      610 2024-05-17 01:42:21.010860 iudex-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2125 1970-01-01 00:00:00.000000 iudex-0.5.0/PKG-INFO
```

### Comparing `iudex-0.4.9/LICENSE` & `iudex-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iudex-0.4.9/iudex/instrumentation/README.md` & `iudex-0.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # Find this in your code base
 app = FastAPI()
 
 # Add this
 instrument(
   app=app,
   service_name=__name__, # or any string describing your service
+  env="development", # or any string for your env
 )
 ```
 3. Make sure the app has access to the environment variable `IUDEX_API_KEY`
 4. You should be all set! Go to [https://app.iudex.ai/](https://app.iudex.ai/) and enter your API key
 5. Go to [https://app.iudex.ai/logs](https://app.iudex.ai/logs) and press `Search` to view your logs
 
 
@@ -33,12 +34,13 @@
 ```
 2. Import `instrument` from `iudex` and invoke it in your entrypoint (usually `main.py`)
 ```python
 # Add this in your lambda function file (likely lambda_function.py)
 from iudex.instrumentation.lambda import instrument
 instrument(
   service_name=__name__, # or any string describing your service
+  env="development", # or any string for your env
 )
 ```
 3. Make sure the app has access to the environment variable `IUDEX_API_KEY`
 4. You should be all set! Go to [https://app.iudex.ai/](https://app.iudex.ai/) and enter your API key
 5. Go to [https://app.iudex.ai/logs](https://app.iudex.ai/logs) and press `Search` to view your logs
```

### Comparing `iudex-0.4.9/iudex/instrumentation/attributes.py` & `iudex-0.5.0/iudex/instrumentation/attributes.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.9/iudex/instrumentation/fastapi.py` & `iudex-0.5.0/iudex/instrumentation/fastapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     app: FastAPI,
     service_name: Optional[str] = None,
     instance_id: Optional[str] = None,
     iudex_api_key: Optional[str] = None,
     log_level: Optional[Union[int, str]] = None,
     git_commit: Optional[str] = None,
     github_url: Optional[str] = None,
+    env: Optional[str] = None,
     config: Optional[IudexConfig] = None,
 ):
     """Auto-instruments FastAPI app to send OTel signals to Iudex.
 
     Invoke this function in your FastAPI entrypoint.
 
     If you use Gunicorn, invoke it within a post_fork hook:
@@ -43,14 +44,15 @@
         "service_name": service_name,
         "instance_id": instance_id,
         "logs_endpoint": None,
         "traces_endpoint": None,
         "log_level": log_level,
         "git_commit": git_commit,
         "github_url": github_url,
+        "env": env,
     }
     iudex_config = _IudexConfig(**config)
 
     iudex_config.configure()
     FastAPIInstrumentor().instrument_app(app)
 
     return iudex_config
```

### Comparing `iudex-0.4.9/iudex/instrumentation/instrumentation.py` & `iudex-0.5.0/iudex/instrumentation/instrumentation.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from opentelemetry.sdk.environment_variables import (
     OTEL_EXPORTER_OTLP_HEADERS,
     OTEL_EXPORTER_OTLP_LOGS_ENDPOINT,
     OTEL_EXPORTER_OTLP_TRACES_ENDPOINT,
     OTEL_LOG_LEVEL,
     OTEL_SERVICE_NAME,
 )
-from opentelemetry.sdk.resources import Resource
+from opentelemetry.sdk.resources import Resource, Attributes
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from opentelemetry.trace import set_tracer_provider
 
 from .attributes import get_attributes
 
 _logger = logging.getLogger(__name__)
@@ -35,28 +35,30 @@
     "CRITICAL": logging.CRITICAL,
     "NOTSET": logging.NOTSET,
 }
 DEFAULT_LOG_LEVEL = logging.INFO
 
 IUDEX_CONFIGURED = False
 
-class IudexConfig(TypedDict):
-    iudex_api_key: Optional[str] = None,
-    service_name: Optional[str] = None,
-    instance_id: Optional[str] = None,
-    logs_endpoint: Optional[str] = None,
-    traces_endpoint: Optional[str] = None,
-    log_level: Optional[Union[str, int]] = None,
-    git_commit: Optional[str] = None,
-    github_url: Optional[str] = None,
+class IudexConfig(TypedDict, total=False):
+    iudex_api_key: Optional[str]
+    service_name: Optional[str]
+    instance_id: Optional[str]
+    logs_endpoint: Optional[str]
+    traces_endpoint: Optional[str]
+    log_level: Optional[Union[str, int]]
+    git_commit: Optional[str]
+    github_url: Optional[str]
+    env: Optional[str]
+    attributes: Optional[Attributes]
 
-class _IudexConfig:
+class _IudexConfig():
     def __init__(
         self,
-        **kwargs: IudexConfig,
+        **kwargs,
     ):
         self.iudex_api_key = kwargs["iudex_api_key"] or os.getenv("IUDEX_API_KEY")
         if not self.iudex_api_key:
             _logger.warning(
                 "Missing API key, no telemetry will be sent to Iudex. "
                 + "Provide the iudex_api_key parameter or set the IUDEX_API_KEY environment variable."
             )
@@ -88,14 +90,18 @@
         if not self.git_commit:
             try:
                 self.git_commit = subprocess.check_output(['git', 'rev-parse', 'HEAD']).strip()
             except:
                 pass
 
         self.github_url = kwargs["github_url"] or os.getenv("GITHUB_URL")
+        
+        self.env = kwargs["env"] or os.getenv("ENV") or os.getenv("ENVIRONMENT")
+
+        self.attributes = kwargs.get("attributes", {})
 
     def configure(self):
         if not self.iudex_api_key:
             _logger.warning(
                 "Missing API key, no telemetry will be sent to Iudex. "
                 + "Provide the iudex_api_key parameter or set the IUDEX_API_KEY environment variable."
             )
@@ -107,16 +113,22 @@
 
         # configure common
         attributes = {}
         attributes["service.name"] = self.service_name
         attributes["service.instance.id"] = self.instance_id
         attributes["git.commit"] = self.git_commit
         attributes["github.url"] = self.github_url
+        attributes["env"] = self.env
         # clean attributes
         attributes = {key: value for key, value in attributes.items() if value is not None}
+
+        # add manual attributes
+        attributes.update(self.attributes)
+
+        # create resource
         resource = Resource.create(attributes)
 
         # set default headers to send iudex api key
         headers = {"x-api-key": self.iudex_api_key}
         os.environ[OTEL_EXPORTER_OTLP_HEADERS] = f"x-api-key:{self.iudex_api_key}"
 
         # configure logger
```

### Comparing `iudex-0.4.9/iudex/instrumentation/lambda.py` & `iudex-0.5.0/iudex/instrumentation/lambda.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 def instrument(
     service_name: Optional[str] = None,
     instance_id: Optional[str] = None,
     iudex_api_key: Optional[str] = None,
     log_level: Optional[Union[int, str]] = None,
     git_commit: Optional[str] = None,
     github_url: Optional[str] = None,
+    env: Optional[str] = None,
     config: Optional[IudexConfig] = None,
 ):
     """Auto-instruments app to send OTel signals to Iudex.
 
     Invoke this function in your Lambda entrypoint.
 
     Args:
@@ -22,22 +23,23 @@
         instance_id: ID of the service instance, e.g. container id, pod name.
         iudex_api_key: Your Iudex API key.
             If not supplied, env var IUDEX_API_KEY will be used.
         log_level: Logging level for the root logger.
         config: IudexConfig object with more granular options.
             Will override all other args, so provide them to the object instead.
     """
-    iudex_config = config or {
+    config = config or {
         "iudex_api_key": iudex_api_key,
         "service_name": service_name,
         "instance_id": instance_id,
         "logs_endpoint": None,
         "traces_endpoint": None,
         "log_level": log_level,
         "git_commit": git_commit,
         "github_url": github_url,
+        "env": env,
     }
-    config = config or _IudexConfig(**iudex_config)
+    iudex_config = _IudexConfig(**config)
 
-    config.configure()
+    iudex_config.configure()
 
-    return config
+    return iudex_config
```

### Comparing `iudex-0.4.9/pyproject.toml` & `iudex-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 [tool.poetry]
 name = "iudex"
-version = "0.4.9"
+version = "0.5.0"
 description = ""
 authors = ["Drake Wong <drake@iudex.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-openai = "^1.12.0"
-httpx = "^0.26.0"
-pydantic = "^2.7.1"
 opentelemetry-distro = "^0.45b0"
 opentelemetry-instrumentation-fastapi = "^0.45b0"
 opentelemetry-exporter-otlp-proto-http = "^1.24.0"
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.1"
```

