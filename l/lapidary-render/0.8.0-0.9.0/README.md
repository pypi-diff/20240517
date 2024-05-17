# Comparing `tmp/lapidary_render-0.8.0.tar.gz` & `tmp/lapidary_render-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lapidary_render-0.8.0.tar", max compression
+gzip compressed data, was "lapidary_render-0.9.0.tar", max compression
```

## Comparing `lapidary_render-0.8.0.tar` & `lapidary_render-0.9.0.tar`

### file list

```diff
@@ -1,45 +1,62 @@
--rw-r--r--   0        0        0     2291 2022-12-17 21:20:37.031349 lapidary_render-0.8.0/Readme.md
--rw-r--r--   0        0        0      850 2023-01-02 15:07:41.559354 lapidary_render-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       21 2022-12-15 10:14:24.127524 lapidary_render-0.8.0/src/lapidary/render/__init__.py
--rw-r--r--   0        0        0       77 2022-12-15 10:14:24.127778 lapidary_render-0.8.0/src/lapidary/render/__main__.py
--rw-r--r--   0        0        0      427 2022-12-17 21:20:37.031968 lapidary_render-0.8.0/src/lapidary/render/black.py
--rw-r--r--   0        0        0     1797 2022-12-17 21:20:37.032855 lapidary_render-0.8.0/src/lapidary/render/cli.py
--rw-r--r--   0        0        0     2135 2022-12-29 15:20:56.034483 lapidary_render-0.8.0/src/lapidary/render/client.py
--rw-r--r--   0        0        0      858 2022-12-29 15:20:56.035358 lapidary_render-0.8.0/src/lapidary/render/config.py
--rw-r--r--   0        0        0     1975 2023-01-01 18:57:39.527755 lapidary_render-0.8.0/src/lapidary/render/main.py
--rw-r--r--   0        0        0     1865 2022-12-15 10:14:24.130351 lapidary_render-0.8.0/src/lapidary/render/model/__init__.py
--rw-r--r--   0        0        0     2382 2022-12-15 10:14:24.131260 lapidary_render-0.8.0/src/lapidary/render/model/attribute.py
--rw-r--r--   0        0        0     3471 2022-12-15 10:14:24.132437 lapidary_render-0.8.0/src/lapidary/render/model/attribute_annotation.py
--rw-r--r--   0        0        0     1330 2022-12-15 10:14:24.135495 lapidary_render-0.8.0/src/lapidary/render/model/auth_module.py
--rw-r--r--   0        0        0      974 2022-12-30 13:10:01.011069 lapidary_render-0.8.0/src/lapidary/render/model/client_class.py
--rw-r--r--   0        0        0     1076 2022-12-15 10:14:24.136719 lapidary_render-0.8.0/src/lapidary/render/model/client_init.py
--rw-r--r--   0        0        0     1869 2022-12-16 05:25:12.554763 lapidary_render-0.8.0/src/lapidary/render/model/client_module.py
--rw-r--r--   0        0        0      300 2022-12-15 10:14:24.138019 lapidary_render-0.8.0/src/lapidary/render/model/module.py
--rw-r--r--   0        0        0     5939 2023-01-02 08:30:58.185486 lapidary_render-0.8.0/src/lapidary/render/model/operation_function.py
--rw-r--r--   0        0        0     2576 2022-12-15 10:14:24.139909 lapidary_render-0.8.0/src/lapidary/render/model/param_model_class.py
--rw-r--r--   0        0        0     1695 2022-12-15 10:14:24.151546 lapidary_render-0.8.0/src/lapidary/render/model/request_body.py
--rw-r--r--   0        0        0     1342 2022-12-30 13:14:18.502050 lapidary_render-0.8.0/src/lapidary/render/model/response_body.py
--rw-r--r--   0        0        0     3231 2022-12-15 10:14:24.153642 lapidary_render-0.8.0/src/lapidary/render/model/schema_class.py
--rw-r--r--   0        0        0      556 2022-12-15 10:14:24.154349 lapidary_render-0.8.0/src/lapidary/render/model/schema_class_enum.py
--rw-r--r--   0        0        0      604 2022-12-15 10:14:24.154917 lapidary_render-0.8.0/src/lapidary/render/model/schema_class_model.py
--rw-r--r--   0        0        0     2626 2022-12-15 10:14:24.155396 lapidary_render-0.8.0/src/lapidary/render/model/schema_module.py
--rw-r--r--   0        0        0     2227 2022-12-30 18:52:12.117544 lapidary_render-0.8.0/src/lapidary/render/model/schema_modules.py
--rw-r--r--   0        0        0      726 2022-12-17 21:20:37.036603 lapidary_render-0.8.0/src/lapidary/render/pyproj.py
--rw-r--r--   0        0        0      997 2022-12-17 21:20:37.037433 lapidary_render-0.8.0/src/lapidary/render/render.py
--rw-r--r--   0        0        0     1457 2022-12-29 15:20:56.038440 lapidary_render-0.8.0/src/lapidary/render/spec.py
--rw-r--r--   0        0        0      347 2022-12-15 10:14:24.158683 lapidary_render-0.8.0/src/lapidary/render/templates/auth/auth.py.jinja2
--rw-r--r--   0        0        0      207 2022-12-29 15:20:56.039408 lapidary_render-0.8.0/src/lapidary/render/templates/client/client.py.jinja2
--rw-r--r--   0        0        0      607 2022-12-29 15:20:56.040189 lapidary_render-0.8.0/src/lapidary/render/templates/client/client.pyi.jinja2
--rw-r--r--   0        0        0      241 2022-12-15 10:14:24.159882 lapidary_render-0.8.0/src/lapidary/render/templates/client/method_init.py.jinja2
--rw-r--r--   0        0        0      728 2022-12-15 10:14:24.160209 lapidary_render-0.8.0/src/lapidary/render/templates/client/method_operation.py.jinja2
--rw-r--r--   0        0        0       60 2022-12-15 10:14:24.160942 lapidary_render-0.8.0/src/lapidary/render/templates/header.py.jinja2
--rw-r--r--   0        0        0       86 2022-12-15 10:14:24.161933 lapidary_render-0.8.0/src/lapidary/render/templates/init/init.py.jinja2
--rw-r--r--   0        0        0      762 2022-12-15 10:14:24.162638 lapidary_render-0.8.0/src/lapidary/render/templates/pyproject.toml.jinja2
--rw-r--r--   0        0        0      253 2022-11-27 22:40:35.867458 lapidary_render-0.8.0/src/lapidary/render/templates/schema_class_enum.py.jinja2
--rw-r--r--   0        0        0       50 2022-11-27 22:40:35.867743 lapidary_render-0.8.0/src/lapidary/render/templates/schema_class_exception.py.jinja2
--rw-r--r--   0        0        0      798 2022-11-27 22:40:35.868024 lapidary_render-0.8.0/src/lapidary/render/templates/schema_class_model.py.jinja2
--rw-r--r--   0        0        0      598 2022-11-27 22:40:35.868264 lapidary_render-0.8.0/src/lapidary/render/templates/schema_class_param_model.py.jinja2
--rw-r--r--   0        0        0      539 2022-12-15 10:14:24.163001 lapidary_render-0.8.0/src/lapidary/render/templates/schema_module.py.jinja2
--rw-r--r--   0        0        0      491 2022-11-27 22:40:35.868757 lapidary_render-0.8.0/src/lapidary/render/templates/type_hint.py.jinja2
--rw-r--r--   0        0        0     3674 1970-01-01 00:00:00.000000 lapidary_render-0.8.0/setup.py
--rw-r--r--   0        0        0     3374 1970-01-01 00:00:00.000000 lapidary_render-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2289 2024-02-01 23:24:36.268872 lapidary_render-0.9.0/Readme.md
+-rw-r--r--   0        0        0     1764 2024-05-17 15:46:32.164816 lapidary_render-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-01-31 09:21:16.972031 lapidary_render-0.9.0/src/lapidary/render/__init__.py
+-rw-r--r--   0        0        0       78 2024-02-20 17:47:56.993176 lapidary_render-0.9.0/src/lapidary/render/__main__.py
+-rw-r--r--   0        0        0      218 2024-05-16 15:58:10.736889 lapidary_render-0.9.0/src/lapidary/render/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     3539 2024-05-16 15:58:10.740889 lapidary_render-0.9.0/src/lapidary/render/__pycache__/cli.cpython-312.pyc
+-rw-r--r--   0        0        0     1157 2024-05-16 15:58:10.744889 lapidary_render-0.9.0/src/lapidary/render/__pycache__/config.cpython-312.pyc
+-rw-r--r--   0        0        0      721 2024-05-16 15:58:10.820889 lapidary_render-0.9.0/src/lapidary/render/__pycache__/json_pointer.cpython-312.pyc
+-rw-r--r--   0        0        0     9974 2024-05-17 15:44:59.397627 lapidary_render-0.9.0/src/lapidary/render/__pycache__/load.cpython-312.pyc
+-rw-r--r--   0        0        0     5445 2024-05-16 15:58:11.004889 lapidary_render-0.9.0/src/lapidary/render/__pycache__/main.cpython-312.pyc
+-rw-r--r--   0        0        0     3226 2024-05-16 15:58:10.836889 lapidary_render-0.9.0/src/lapidary/render/__pycache__/names.cpython-312.pyc
+-rw-r--r--   0        0        0      822 2024-05-16 15:58:10.844889 lapidary_render-0.9.0/src/lapidary/render/__pycache__/pydantic_utils.cpython-312.pyc
+-rw-r--r--   0        0        0     1849 2024-04-23 07:49:25.843382 lapidary_render-0.9.0/src/lapidary/render/cli.py
+-rw-r--r--   0        0        0      429 2024-04-06 13:13:07.932135 lapidary_render-0.9.0/src/lapidary/render/config.py
+-rw-r--r--   0        0        0      202 2024-02-06 21:55:44.910267 lapidary_render-0.9.0/src/lapidary/render/json_pointer.py
+-rw-r--r--   0        0        0     4393 2024-05-16 18:46:39.698320 lapidary_render-0.9.0/src/lapidary/render/load.py
+-rw-r--r--   0        0        0     3300 2024-02-29 11:28:01.434766 lapidary_render-0.9.0/src/lapidary/render/main.py
+-rw-r--r--   0        0        0       86 2024-02-16 22:25:43.276220 lapidary_render-0.9.0/src/lapidary/render/model/__init__.py
+-rw-r--r--   0        0        0      280 2024-05-16 15:58:10.820889 lapidary_render-0.9.0/src/lapidary/render/model/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0    19253 2024-05-17 15:44:59.109630 lapidary_render-0.9.0/src/lapidary/render/model/__pycache__/openapi_conv.cpython-312.pyc
+-rw-r--r--   0        0        0     1782 2024-05-16 15:58:10.980889 lapidary_render-0.9.0/src/lapidary/render/model/__pycache__/refs.cpython-312.pyc
+-rw-r--r--   0        0        0    13880 2024-05-17 15:44:59.293628 lapidary_render-0.9.0/src/lapidary/render/model/__pycache__/schema.cpython-312.pyc
+-rw-r--r--   0        0        0     2212 2024-05-17 15:44:59.289628 lapidary_render-0.9.0/src/lapidary/render/model/__pycache__/stack.cpython-312.pyc
+-rw-r--r--   0        0        0      890 2024-04-06 13:17:31.771459 lapidary_render-0.9.0/src/lapidary/render/model/openapi/__init__.py
+-rw-r--r--   0        0        0      977 2024-05-16 15:58:10.836889 lapidary_render-0.9.0/src/lapidary/render/model/openapi/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     3233 2024-05-16 15:58:10.844889 lapidary_render-0.9.0/src/lapidary/render/model/openapi/__pycache__/base.cpython-312.pyc
+-rw-r--r--   0        0        0      508 2024-05-16 15:58:10.840889 lapidary_render-0.9.0/src/lapidary/render/model/openapi/__pycache__/ext.cpython-312.pyc
+-rw-r--r--   0        0        0    27281 2024-05-16 15:58:10.840889 lapidary_render-0.9.0/src/lapidary/render/model/openapi/__pycache__/model.cpython-312.pyc
+-rw-r--r--   0        0        0     1735 2024-03-09 08:48:35.890403 lapidary_render-0.9.0/src/lapidary/render/model/openapi/base.py
+-rw-r--r--   0        0        0      286 2024-02-06 21:55:33.810682 lapidary_render-0.9.0/src/lapidary/render/model/openapi/ext.py
+-rw-r--r--   0        0        0    15031 2024-04-22 14:27:28.119250 lapidary_render-0.9.0/src/lapidary/render/model/openapi/model.py
+-rw-r--r--   0        0        0    11215 2024-05-16 18:48:47.830932 lapidary_render-0.9.0/src/lapidary/render/model/openapi_conv.py
+-rw-r--r--   0        0        0     1731 2024-04-22 14:35:02.801343 lapidary_render-0.9.0/src/lapidary/render/model/python/__init__.py
+-rw-r--r--   0        0        0     2360 2024-05-16 15:58:10.836889 lapidary_render-0.9.0/src/lapidary/render/model/python/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0    10238 2024-05-16 15:58:10.968889 lapidary_render-0.9.0/src/lapidary/render/model/python/__pycache__/model.cpython-312.pyc
+-rw-r--r--   0        0        0     4011 2024-05-16 15:58:10.976889 lapidary_render-0.9.0/src/lapidary/render/model/python/__pycache__/module.cpython-312.pyc
+-rw-r--r--   0        0        0     3166 2024-05-16 15:58:10.980889 lapidary_render-0.9.0/src/lapidary/render/model/python/__pycache__/module_path.cpython-312.pyc
+-rw-r--r--   0        0        0     9478 2024-05-16 15:58:10.968889 lapidary_render-0.9.0/src/lapidary/render/model/python/__pycache__/type_hint.cpython-312.pyc
+-rw-r--r--   0        0        0     4868 2024-04-22 14:47:46.164641 lapidary_render-0.9.0/src/lapidary/render/model/python/model.py
+-rw-r--r--   0        0        0     1915 2024-03-11 19:46:08.202978 lapidary_render-0.9.0/src/lapidary/render/model/python/module.py
+-rw-r--r--   0        0        0     1594 2024-04-22 14:27:28.559252 lapidary_render-0.9.0/src/lapidary/render/model/python/module_path.py
+-rw-r--r--   0        0        0     4075 2024-05-10 20:22:09.476541 lapidary_render-0.9.0/src/lapidary/render/model/python/type_hint.py
+-rw-r--r--   0        0        0      688 2024-02-20 15:44:43.621272 lapidary_render-0.9.0/src/lapidary/render/model/refs.py
+-rw-r--r--   0        0        0     8522 2024-05-16 18:48:53.522959 lapidary_render-0.9.0/src/lapidary/render/model/schema.py
+-rw-r--r--   0        0        0      750 2024-05-16 18:46:52.994383 lapidary_render-0.9.0/src/lapidary/render/model/stack.py
+-rw-r--r--   0        0        0     1644 2024-04-22 14:27:28.559252 lapidary_render-0.9.0/src/lapidary/render/names.py
+-rw-r--r--   0        0        0      342 2024-02-06 21:55:33.810682 lapidary_render-0.9.0/src/lapidary/render/pydantic_utils.py
+-rw-r--r--   0        0        0        0 2024-02-11 18:01:30.332150 lapidary_render-0.9.0/src/lapidary/render/templates/gen/{{loop_over(model.packages()).to_path(is_module=False)}}/__init__.py
+-rw-r--r--   0        0        0      375 2024-05-10 19:45:54.714317 lapidary_render-0.9.0/src/lapidary/render/templates/gen/{{loop_over(model.schemas).path.to_path()}}.jinja
+-rw-r--r--   0        0        0     1131 2024-05-10 19:22:38.013284 lapidary_render-0.9.0/src/lapidary/render/templates/gen/{{model.package}}/client.py.jinja
+-rw-r--r--   0        0        0      397 2024-04-06 13:17:31.771459 lapidary_render-0.9.0/src/lapidary/render/templates/gen/{{model.package}}/components/securitySchemes.py.jinja
+-rw-r--r--   0        0        0      241 2024-01-31 13:03:39.555446 lapidary_render-0.9.0/src/lapidary/render/templates/includes/client/method_init.py.jinja
+-rw-r--r--   0        0        0     1613 2024-04-22 14:46:20.000460 lapidary_render-0.9.0/src/lapidary/render/templates/includes/client/method_operation.py.jinja
+-rw-r--r--   0        0        0       87 2024-02-01 23:24:36.268872 lapidary_render-0.9.0/src/lapidary/render/templates/includes/header.py.jinja
+-rw-r--r--   0        0        0       85 2024-01-31 13:03:39.555446 lapidary_render-0.9.0/src/lapidary/render/templates/includes/header.txt
+-rw-r--r--   0        0        0       50 2024-01-31 13:03:39.559446 lapidary_render-0.9.0/src/lapidary/render/templates/includes/schema/schema_class_exception.py.jinja
+-rw-r--r--   0        0        0      772 2024-03-11 19:46:08.202978 lapidary_render-0.9.0/src/lapidary/render/templates/includes/schema/schema_class_model.py.jinja
+-rw-r--r--   0        0        0      367 2024-04-06 13:17:31.771459 lapidary_render-0.9.0/src/lapidary/render/templates/includes/security/api_key.py.jinja
+-rw-r--r--   0        0        0      454 2024-04-06 13:17:31.771459 lapidary_render-0.9.0/src/lapidary/render/templates/includes/security/oauth2_implicit.py.jinja
+-rw-r--r--   0        0        0      564 2024-04-06 13:11:34.442044 lapidary_render-0.9.0/src/lapidary/render/templates/includes/type_hint.py.jinja
+-rw-r--r--   0        0        0      856 2024-02-22 14:33:55.987124 lapidary_render-0.9.0/src/lapidary/render/templates/pyproject.toml.jinja
+-rw-r--r--   0        0        0     3702 1970-01-01 00:00:00.000000 lapidary_render-0.9.0/PKG-INFO
```

### Comparing `lapidary_render-0.8.0/Readme.md` & `lapidary_render-0.9.0/Readme.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 `lapidary` command offers inline help and shell command completion. See `lapidary --help` for details.
 
 ### lapidary init
 
 `lapidary init [--[no-]format-strict] [--[no-]render] SCHEMA_PATH PROJECT_ROOT PACKAGE_NAME`
 
-Lapidary will create 
+Lapidary will create
 - PROJECT_ROOT and all necessary directories,
 - \_\_init\_\_.py files,
 - pyproject.toml with [poetry](https://python-poetry.org/) configured,
 - py.typed
 - client.pyi with function stubs for all operations and a client.py with an empty client class.
 - [Pydantic](https://docs.pydantic.dev/) model classes for each schema.
 
@@ -51,13 +51,13 @@
 
 ## Configuration
 
 Lapidary can be configured with a pyproject.yaml file, under [tool.lapidary] path.
 
 Only `package` value is required, and it's set by `lapidary init`.
 
-- package [str] - root package name 
+- package [str] - root package name
 - format [bool] - whether to format the generated code with black [default = True].
 - cache [bool] - whether to cache openapi and patches as pickle files. Only files larger than 50kB are cached [default = True].
 - src_root [str] - sources root, in PROJECT_ROOT [default = 'src'].
 - gen_root [str] = generated sources root, in PROJECT_ROOT [default = 'gen'].
 - patches [str] = patches directory, under sources root [default = 'patches'].
```

### Comparing `lapidary_render-0.8.0/src/lapidary/render/templates/pyproject.toml.jinja2` & `lapidary_render-0.9.0/src/lapidary/render/templates/pyproject.toml.jinja`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.3.2"]
 
 [tool.poetry]
-name = "{{ project_name }}"
-description = "Client library for {{ openapi_title }}"
+name = "{{ config.package }}"
+description = "Client library for {{ document.info.title }}"
 version = "0.1.0"
 authors = []
 license = ""
 packages = [
-    { include = '{{ package }}', from = "gen" },
+    { include = '{{ config.package }}', from = "gen" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pydantic = { extras = ["email"], version = "^{{ versions.pydantic }}" }
-lapidary = "{{ versions.lapidary }}"
+pydantic = { extras = ["email"], version = "^{{ get_version('pydantic') }}" }
+lapidary = "{{ get_version('lapidary') }}"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "0.990"
-lapidary-render = "{{ versions.lapidary_render }}"
+lapidary-render = "{{ get_version('lapidary_render') }}"
 taskipy = "^1.10.3"
 
 [tool.taskipy.tasks]
 update = 'lapidary update'
 mypy = 'mypy'
 check = 'task mypy'
 
 [tool.lapidary]
-package = '{{ package }}'
+{%- for key, value in config.items() %}
+{{ key }} = "{{ value }}"
+{%- endfor %}
 
 [tool.mypy]
 mypy_path = ['gen']
-packages = ['{{ package }}']
+packages = ['{{ config.package }}']
```

### Comparing `lapidary_render-0.8.0/PKG-INFO` & `lapidary_render-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 Metadata-Version: 2.1
 Name: lapidary-render
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python async OpenAPI client library generator
 Home-page: https://github.com/python-lapidary/lapidary
 License: AGPL-3.0
 Author: Raphael Krupinski
 Author-email: rafalkrupinski@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Typing :: Typed
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: black (>=22.8.0,<23.0.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: jsonpatch (>=1.32,<2.0)
-Requires-Dist: lapidary (==0.8.0)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: lapidary (>=0.9.0,<0.10.0)
+Requires-Dist: platformdirs (>=4.2.0,<5.0.0)
+Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Requires-Dist: python-mimeparse (>=1.6.0,<2.0.0)
-Requires-Dist: tomlkit (>=0.11.4,<0.12.0)
-Requires-Dist: typer (>=0.6.1,<0.7.0)
+Requires-Dist: ruamel-yaml (>=0.18.6,<0.19.0)
+Requires-Dist: rybak (>=0.3.0,<0.4.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/python-lapidary/lapidary
 Description-Content-Type: text/markdown
 
 # Code generator
 ## Installation
 
 lapidary-render requires python 3.9 or higher to run.
@@ -40,15 +47,15 @@
 
 `lapidary` command offers inline help and shell command completion. See `lapidary --help` for details.
 
 ### lapidary init
 
 `lapidary init [--[no-]format-strict] [--[no-]render] SCHEMA_PATH PROJECT_ROOT PACKAGE_NAME`
 
-Lapidary will create 
+Lapidary will create
 - PROJECT_ROOT and all necessary directories,
 - \_\_init\_\_.py files,
 - pyproject.toml with [poetry](https://python-poetry.org/) configured,
 - py.typed
 - client.pyi with function stubs for all operations and a client.py with an empty client class.
 - [Pydantic](https://docs.pydantic.dev/) model classes for each schema.
 
@@ -78,14 +85,14 @@
 
 ## Configuration
 
 Lapidary can be configured with a pyproject.yaml file, under [tool.lapidary] path.
 
 Only `package` value is required, and it's set by `lapidary init`.
 
-- package [str] - root package name 
+- package [str] - root package name
 - format [bool] - whether to format the generated code with black [default = True].
 - cache [bool] - whether to cache openapi and patches as pickle files. Only files larger than 50kB are cached [default = True].
 - src_root [str] - sources root, in PROJECT_ROOT [default = 'src'].
 - gen_root [str] = generated sources root, in PROJECT_ROOT [default = 'gen'].
 - patches [str] = patches directory, under sources root [default = 'patches'].
```

