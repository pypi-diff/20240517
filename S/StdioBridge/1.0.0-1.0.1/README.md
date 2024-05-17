# Comparing `tmp/StdioBridge-1.0.0.tar.gz` & `tmp/StdioBridge-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StdioBridge-1.0.0.tar", last modified: Fri May 17 10:29:08 2024, max compression
+gzip compressed data, was "StdioBridge-1.0.1.tar", last modified: Fri May 17 15:07:36 2024, max compression
```

## Comparing `StdioBridge-1.0.0.tar` & `StdioBridge-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:29:08.521624 StdioBridge-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-17 10:29:00.000000 StdioBridge-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-17 10:29:08.521624 StdioBridge-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:29:08.521624 StdioBridge-1.0.0/StdioBridge/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-17 10:29:00.000000 StdioBridge-1.0.0/StdioBridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-17 10:29:00.000000 StdioBridge-1.0.0/StdioBridge/_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:29:08.521624 StdioBridge-1.0.0/StdioBridge/api/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-17 10:29:00.000000 StdioBridge-1.0.0/StdioBridge/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-17 10:29:00.000000 StdioBridge-1.0.0/StdioBridge/api/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-17 10:29:00.000000 StdioBridge-1.0.0/StdioBridge/api/_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-17 10:29:00.000000 StdioBridge-1.0.0/StdioBridge/api/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:29:08.521624 StdioBridge-1.0.0/StdioBridge/client/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-17 10:29:00.000000 StdioBridge-1.0.0/StdioBridge/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-17 10:29:00.000000 StdioBridge-1.0.0/StdioBridge/client/_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:29:08.521624 StdioBridge-1.0.0/StdioBridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-17 10:29:08.000000 StdioBridge-1.0.0/StdioBridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-17 10:29:08.000000 StdioBridge-1.0.0/StdioBridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 10:29:08.000000 StdioBridge-1.0.0/StdioBridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 10:29:08.000000 StdioBridge-1.0.0/StdioBridge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 10:29:08.521624 StdioBridge-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-17 10:29:00.000000 StdioBridge-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:07:36.982055 StdioBridge-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-17 15:07:27.000000 StdioBridge-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-17 15:07:36.982055 StdioBridge-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:07:36.982055 StdioBridge-1.0.1/StdioBridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-17 15:07:27.000000 StdioBridge-1.0.1/StdioBridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-17 15:07:27.000000 StdioBridge-1.0.1/StdioBridge/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:07:36.982055 StdioBridge-1.0.1/StdioBridge/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-17 15:07:27.000000 StdioBridge-1.0.1/StdioBridge/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-17 15:07:27.000000 StdioBridge-1.0.1/StdioBridge/api/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-17 15:07:27.000000 StdioBridge-1.0.1/StdioBridge/api/_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-17 15:07:27.000000 StdioBridge-1.0.1/StdioBridge/api/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:07:36.982055 StdioBridge-1.0.1/StdioBridge/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-17 15:07:27.000000 StdioBridge-1.0.1/StdioBridge/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-17 15:07:27.000000 StdioBridge-1.0.1/StdioBridge/client/_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:07:36.982055 StdioBridge-1.0.1/StdioBridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-17 15:07:36.000000 StdioBridge-1.0.1/StdioBridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-17 15:07:36.000000 StdioBridge-1.0.1/StdioBridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:07:36.000000 StdioBridge-1.0.1/StdioBridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 15:07:36.000000 StdioBridge-1.0.1/StdioBridge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 15:07:36.982055 StdioBridge-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-17 15:07:27.000000 StdioBridge-1.0.1/setup.py
```

### Comparing `StdioBridge-1.0.0/LICENSE` & `StdioBridge-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.0.0/PKG-INFO` & `StdioBridge-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StdioBridge
-Version: 1.0.0
+Version: 1.0.1
 Summary: A StdioBridge package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) 2024 SergeiKrivko
         
@@ -26,36 +26,36 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Имя пакета: StdioBridge
+# StdioBridge
 
-Описание:
+## Описание:
 
 StdioBridge является универсальной протокол-библиотекой, предназначенной для связывания программ через стандартные вводы и выводы (stdin и stdout), предоставляя внешний интерфейс, схожий с HTTP. StdioBridge облегчает создание межпрограммного общения при минимальных накладных расходах и обеспечивает простоту интеграции с существующими приложениями.
 
-Основные возможности:
+## Основные возможности:
 
 - Простота подключения и настройки без необходимости использования сложных веб-серверов или API;
 - Поддержка различных языков программирования, обеспечивая максимальную гибкость при интеграции;
 - Функциональность по преобразованию данных между стандартными вводом/выводом (stdin/stdout) и HTTP-подобным интерфейсом для бесшовного соединения между программами;
 - Возможность расширения и дополнения функциональности в соответствии с требованиями вашего проекта;
 - Надежность и гарантированная производительность благодаря оптимальной архитектуре и использованию системных ресурсов.
 
-Требования:
+## Требования:
 
 - Python версии 3.10 и выше
 
-Установка:
+## Установка:
 
 Установка StdioBridge осуществляется через pip:
 
 ```bash
 pip install stdiobridge
 ```
 
-Лицензия:
+## Лицензия:
 
 StdioBridge доступна под лицензией MIT.
```

### Comparing `StdioBridge-1.0.0/StdioBridge/api/_api.py` & `StdioBridge-1.0.1/StdioBridge/api/_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,16 @@
                             else:
                                 params[param_name] = param_type(query_params[param_name])
                 except ValueError:
                     raise ErrorUnprocessableEntity()
 
                 try:
                     return Response(200, func(**params))
+                except ApiError as e:
+                    raise e
                 except Exception as e:
                     raise InternalServerError(f"{e.__class__.__name__}: {e}")
 
             self.add(method, url, wrapper)
 
             return wrapper
```

### Comparing `StdioBridge-1.0.0/StdioBridge/api/errors.py` & `StdioBridge-1.0.1/StdioBridge/api/errors.py`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.0.0/StdioBridge/client/_client.py` & `StdioBridge-1.0.1/StdioBridge/client/_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -86,23 +86,7 @@
     async def delete(self, url: str, data: dict = None) -> Response:
         resp = await self._request('delete', url, data)
         return resp
 
     async def patch(self, url: str, data: dict) -> Response:
         resp = await self._request('patch', url, data)
         return resp
-
-
-async def main():
-    client = Client('python -m TestPluginSrc.api')
-
-    resp = await client.get('url?key=6')
-    print(resp, resp.data)
-    resp = await client.post('url/4d5515be-bf03-4c66-874e-31063045a9f6', {'1': 1, '2': 2, '5': 5})
-    print(resp, resp.data)
-    resp = await client.post('url/last', {'1': 1, '2': 2, '5': 5})
-    print(resp, resp.data)
-    client.terminate()
-
-
-if __name__ == '__main__':
-    asyncio.run(main())
```

### Comparing `StdioBridge-1.0.0/StdioBridge.egg-info/PKG-INFO` & `StdioBridge-1.0.1/StdioBridge.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StdioBridge
-Version: 1.0.0
+Version: 1.0.1
 Summary: A StdioBridge package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) 2024 SergeiKrivko
         
@@ -26,36 +26,36 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Имя пакета: StdioBridge
+# StdioBridge
 
-Описание:
+## Описание:
 
 StdioBridge является универсальной протокол-библиотекой, предназначенной для связывания программ через стандартные вводы и выводы (stdin и stdout), предоставляя внешний интерфейс, схожий с HTTP. StdioBridge облегчает создание межпрограммного общения при минимальных накладных расходах и обеспечивает простоту интеграции с существующими приложениями.
 
-Основные возможности:
+## Основные возможности:
 
 - Простота подключения и настройки без необходимости использования сложных веб-серверов или API;
 - Поддержка различных языков программирования, обеспечивая максимальную гибкость при интеграции;
 - Функциональность по преобразованию данных между стандартными вводом/выводом (stdin/stdout) и HTTP-подобным интерфейсом для бесшовного соединения между программами;
 - Возможность расширения и дополнения функциональности в соответствии с требованиями вашего проекта;
 - Надежность и гарантированная производительность благодаря оптимальной архитектуре и использованию системных ресурсов.
 
-Требования:
+## Требования:
 
 - Python версии 3.10 и выше
 
-Установка:
+## Установка:
 
 Установка StdioBridge осуществляется через pip:
 
 ```bash
 pip install stdiobridge
 ```
 
-Лицензия:
+## Лицензия:
 
 StdioBridge доступна под лицензией MIT.
```

### Comparing `StdioBridge-1.0.0/setup.py` & `StdioBridge-1.0.1/setup.py`

 * *Files identical despite different names*

