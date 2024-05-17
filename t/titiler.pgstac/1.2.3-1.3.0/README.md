# Comparing `tmp/titiler.pgstac-1.2.3.tar.gz` & `tmp/titiler.pgstac-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titiler.pgstac-1.2.3.tar", last modified: Mon Mar 25 15:03:44 2024, max compression
+gzip compressed data, was "titiler.pgstac-1.3.0.tar", last modified: Fri May 17 06:55:47 2024, max compression
```

## Comparing `titiler.pgstac-1.2.3.tar` & `titiler.pgstac-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1097 2024-03-25 15:03:23.762537 titiler.pgstac-1.2.3/LICENSE
--rw-r--r--   0        0        0     4451 2024-03-25 15:03:23.762537 titiler.pgstac-1.2.3/README.md
--rw-r--r--   0        0        0     2742 2024-03-25 15:03:23.858537 titiler.pgstac-1.2.3/pyproject.toml
--rw-r--r--   0        0        0       44 2024-03-25 15:03:23.862537 titiler.pgstac-1.2.3/titiler/pgstac/__init__.py
--rw-r--r--   0        0        0     1202 2024-03-25 15:03:23.862537 titiler.pgstac-1.2.3/titiler/pgstac/db.py
--rw-r--r--   0        0        0     7158 2024-03-25 15:03:23.862537 titiler.pgstac-1.2.3/titiler/pgstac/dependencies.py
--rw-r--r--   0        0        0     5624 2024-03-25 15:03:23.862537 titiler.pgstac-1.2.3/titiler/pgstac/extensions.py
--rw-r--r--   0        0        0    48410 2024-03-25 15:03:23.862537 titiler.pgstac-1.2.3/titiler/pgstac/factory.py
--rw-r--r--   0        0        0       91 2024-03-25 15:03:23.862537 titiler.pgstac-1.2.3/titiler/pgstac/logger.py
--rw-r--r--   0        0        0     9595 2024-03-25 15:03:23.862537 titiler.pgstac-1.2.3/titiler/pgstac/main.py
--rw-r--r--   0        0        0     6060 2024-03-25 15:03:23.862537 titiler.pgstac-1.2.3/titiler/pgstac/model.py
--rw-r--r--   0        0        0    15511 2024-03-25 15:03:23.862537 titiler.pgstac-1.2.3/titiler/pgstac/mosaic.py
--rw-r--r--   0        0        0        0 2024-03-25 15:03:23.862537 titiler.pgstac-1.2.3/titiler/pgstac/py.typed
--rw-r--r--   0        0        0     3056 2024-03-25 15:03:23.862537 titiler.pgstac-1.2.3/titiler/pgstac/reader.py
--rw-r--r--   0        0        0     3661 2024-03-25 15:03:23.862537 titiler.pgstac-1.2.3/titiler/pgstac/settings.py
--rw-r--r--   0        0        0    10268 2024-03-25 15:03:23.862537 titiler.pgstac-1.2.3/titiler/pgstac/templates/index.html
--rw-r--r--   0        0        0     3058 2024-03-25 15:03:23.862537 titiler.pgstac-1.2.3/titiler/pgstac/templates/wmts.xml
--rw-r--r--   0        0        0      838 2024-03-25 15:03:23.862537 titiler.pgstac-1.2.3/titiler/pgstac/utils.py
--rw-r--r--   0        0        0     5722 1970-01-01 00:00:00.000000 titiler.pgstac-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1097 2024-05-17 06:55:20.256511 titiler.pgstac-1.3.0/LICENSE
+-rw-r--r--   0        0        0     4451 2024-05-17 06:55:20.256511 titiler.pgstac-1.3.0/README.md
+-rw-r--r--   0        0        0     2742 2024-05-17 06:55:20.352512 titiler.pgstac-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2024-05-17 06:55:20.356512 titiler.pgstac-1.3.0/titiler/pgstac/__init__.py
+-rw-r--r--   0        0        0     1202 2024-05-17 06:55:20.356512 titiler.pgstac-1.3.0/titiler/pgstac/db.py
+-rw-r--r--   0        0        0     8371 2024-05-17 06:55:20.356512 titiler.pgstac-1.3.0/titiler/pgstac/dependencies.py
+-rw-r--r--   0        0        0     5630 2024-05-17 06:55:20.356512 titiler.pgstac-1.3.0/titiler/pgstac/extensions.py
+-rw-r--r--   0        0        0    49591 2024-05-17 06:55:20.356512 titiler.pgstac-1.3.0/titiler/pgstac/factory.py
+-rw-r--r--   0        0        0       91 2024-05-17 06:55:20.356512 titiler.pgstac-1.3.0/titiler/pgstac/logger.py
+-rw-r--r--   0        0        0    11088 2024-05-17 06:55:20.356512 titiler.pgstac-1.3.0/titiler/pgstac/main.py
+-rw-r--r--   0        0        0     9958 2024-05-17 06:55:20.356512 titiler.pgstac-1.3.0/titiler/pgstac/model.py
+-rw-r--r--   0        0        0    15511 2024-05-17 06:55:20.356512 titiler.pgstac-1.3.0/titiler/pgstac/mosaic.py
+-rw-r--r--   0        0        0        0 2024-05-17 06:55:20.356512 titiler.pgstac-1.3.0/titiler/pgstac/py.typed
+-rw-r--r--   0        0        0     3056 2024-05-17 06:55:20.356512 titiler.pgstac-1.3.0/titiler/pgstac/reader.py
+-rw-r--r--   0        0        0     3661 2024-05-17 06:55:20.356512 titiler.pgstac-1.3.0/titiler/pgstac/settings.py
+-rw-r--r--   0        0        0    10268 2024-05-17 06:55:20.356512 titiler.pgstac-1.3.0/titiler/pgstac/templates/index.html
+-rw-r--r--   0        0        0     3093 2024-05-17 06:55:20.356512 titiler.pgstac-1.3.0/titiler/pgstac/templates/wmts.xml
+-rw-r--r--   0        0        0      838 2024-05-17 06:55:20.356512 titiler.pgstac-1.3.0/titiler/pgstac/utils.py
+-rw-r--r--   0        0        0     5722 1970-01-01 00:00:00.000000 titiler.pgstac-1.3.0/PKG-INFO
```

### Comparing `titiler.pgstac-1.2.3/LICENSE` & `titiler.pgstac-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-1.2.3/README.md` & `titiler.pgstac-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-1.2.3/pyproject.toml` & `titiler.pgstac-1.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -23,22 +23,22 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dependencies = [
-    "titiler.core>=0.17.0,<0.18",
-    "titiler.mosaic>=0.17.0,<0.18",
+    "titiler.core>=0.18.0,<0.19",
+    "titiler.mosaic>=0.18.0,<0.19",
     "geojson-pydantic~=1.0",
     "pydantic>=2.4,<3.0",
     "pydantic-settings~=2.0",
 ]
 dynamic = []
-version = "1.2.3"
+version = "1.3.0"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 psycopg = [
     "psycopg[pool]",
```

### Comparing `titiler.pgstac-1.2.3/titiler/pgstac/db.py` & `titiler.pgstac-1.3.0/titiler/pgstac/db.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-1.2.3/titiler/pgstac/dependencies.py` & `titiler.pgstac-1.3.0/titiler/pgstac/dependencies.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """titiler-pgstac dependencies."""
 
+import warnings
 from dataclasses import dataclass, field
 from typing import Optional, Tuple
 
 import morecantile
 import pystac
 from cachetools import TTLCache, cached
 from cachetools.keys import hashkey
@@ -42,15 +43,15 @@
     tries=retry_config.retry,
     delay=retry_config.delay,
     exceptions=(
         pgErrors.OperationalError,
         pgErrors.InterfaceError,
     ),
 )
-def get_collection_id(pool: ConnectionPool, collection_id: str) -> str:
+def get_collection_id(pool: ConnectionPool, collection_id: str) -> str:  # noqa: C901
     """Get Search Id for a Collection."""
     search = model.PgSTACSearch(collections=[collection_id])
 
     with pool.connection() as conn:
         with conn.cursor(row_factory=dict_row) as cursor:
             cursor.execute(
                 "SELECT * FROM pgstac.get_collection(%s);",
@@ -60,19 +61,49 @@
             if not collection:
                 raise MosaicNotFoundError(f"CollectionId `{collection_id}` not found")
 
             bbox = collection["extent"]["spatial"].get("bbox", [[-180, -90, 180, 90]])
             metadata = model.Metadata(
                 name=f"Mosaic for '{collection_id}' Collection",
                 bounds=bbox[0],
-                # TODO:
-                # - use the `asset`` extension to populate the `assets` attribute
-                # - use the `render` extension to populate the `defaults` attribute
             )
 
+            # item-assets https://github.com/stac-extensions/item-assets
+            if "item_assets" in collection:
+                metadata.assets = list(collection["item_assets"])
+
+            # render https://github.com/stac-extensions/render
+            if "renders" in collection:
+                renders = {}
+                for name, render in collection["renders"].items():
+                    try:
+                        # `title` is not a parameter expected by titiler-pgstac
+                        _ = render.pop("title", None)
+
+                        # TODO: add support for tilematrixset
+                        _ = render.pop("tilematrixsets", None)
+
+                        # `minmax_zoom` is not a parameter expected by titiler-pgstac
+                        zooms = render.pop("minmax_zoom", None)
+                        if zooms and len(zooms) == 2:
+                            render["minzoom"] = zooms[0]
+                            render["maxzoom"] = zooms[1]
+
+                        renders[name] = render
+
+                    except Exception as e:
+                        warnings.warn(
+                            f"Invalid render `{name}`: {repr(e)}",
+                            UserWarning,
+                            stacklevel=2,
+                        )
+                        continue
+
+                metadata.defaults = renders
+
             cursor.row_factory = class_row(model.Search)
             cursor.execute(
                 "SELECT * FROM search_query(%s, _metadata => %s);",
                 (
                     search.model_dump_json(by_alias=True, exclude_none=True),
                     metadata.model_dump_json(exclude_none=True),
                 ),
```

### Comparing `titiler.pgstac-1.2.3/titiler/pgstac/extensions.py` & `titiler.pgstac-1.3.0/titiler/pgstac/extensions.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from dataclasses import dataclass
 from typing import List, Tuple
 from urllib.parse import urlencode
 
 from cogeo_mosaic.errors import MosaicNotFoundError
 from fastapi import Depends
 from psycopg.rows import class_row
-from starlette.datastructures import QueryParams
 from starlette.requests import Request
 from starlette.routing import NoMatchFound
 
 from titiler.core.factory import FactoryExtension
 from titiler.pgstac import model
 from titiler.pgstac.factory import MosaicTilerFactory, check_query_params
 
@@ -26,15 +25,15 @@
 
         @factory.router.get(
             "/info",
             responses={200: {"description": "Get Search query metadata."}},
             response_model=model.Info,
             response_model_exclude_none=True,
         )
-        def info_search(  # noqa: C901
+        def info(  # noqa: C901
             request: Request, search_id=Depends(factory.path_dependency)
         ):
             """Get Search query metadata."""
             with request.app.state.dbpool.connection() as conn:
                 with conn.cursor(row_factory=class_row(model.Search)) as cursor:
                     cursor.execute(
                         "SELECT * FROM searches WHERE hash=%s;",
@@ -45,20 +44,20 @@
             if not search_info:
                 raise MosaicNotFoundError(f"SearchId `{search_id}` not found")
 
             links: List[model.Link] = [
                 model.Link(
                     rel="self",
                     title="Mosaic metadata",
-                    href=factory.url_for(request, "info_search"),
+                    href=factory.url_for(request, "info"),
                 ),
             ]
 
             layers: List[Tuple[str, str]] = []
-            if search_info.metadata.defaults:
+            if renders := search_info.metadata.defaults_params:
                 # List of dependencies a `/tile` URL should validate
                 # Note: Those dependencies should only require Query() inputs
                 tile_dependencies = [
                     factory.layer_dependency,
                     factory.dataset_dependency,
                     factory.pixel_selection_dependency,
                     factory.process_dependency,
@@ -66,87 +65,90 @@
                     factory.colormap_dependency,
                     factory.render_dependency,
                     factory.pgstac_dependency,
                     factory.reader_dependency,
                     factory.backend_dependency,
                 ]
 
-                for name, values in search_info.metadata.defaults.items():
-                    query_string = urlencode(values, doseq=True)
+                for name, values in renders.items():
                     try:
                         check_query_params(
                             dependencies=tile_dependencies,
-                            query_params=QueryParams(query_string),
+                            query_params=values,
                         )
                     except Exception as e:
                         warnings.warn(
                             f"Cannot construct URL for layer `{name}`: {repr(e)}",
                             UserWarning,
                             stacklevel=2,
                         )
                         continue
-                    layers.append((name, query_string))
+
+                    layers.append((name, urlencode(values, doseq=True)))
 
             try:
-                tilejson_endpoint = factory.url_for(request, "tilejson")
+                tilejson_endpoint = factory.url_for(
+                    request, "tilejson", tileMatrixSetId="{tileMatrixSetId}"
+                )
                 links.append(
                     model.Link(
-                        title="TileJSON link (Template URL)",
+                        title="TileJSON link (Template URL).",
                         rel="tilejson",
                         href=tilejson_endpoint,
+                        templated=True,
                     ),
                 )
                 for layer, qs in layers:
                     links.append(
                         model.Link(
-                            title=f"TileJSON link for `{layer}` layer",
+                            title=f"TileJSON link for `{layer}` layer (Template URL).",
                             rel="tilejson",
                             href=tilejson_endpoint + f"?{qs}",
+                            templated=True,
                         ),
                     )
 
             except NoMatchFound:
                 pass
 
             try:
-                map_viewer_endpoint = factory.url_for(request, "map_viewer")
+                map_viewer_endpoint = factory.url_for(
+                    request, "map_viewer", tileMatrixSetId="{tileMatrixSetId}"
+                )
                 links.append(
                     model.Link(
                         rel="map",
-                        title="Map viewer link (Template URL)",
+                        title="Map viewer link (Template URL).",
                         href=map_viewer_endpoint,
+                        templated=True,
                     )
                 )
                 for layer, qs in layers:
                     links.append(
                         model.Link(
-                            title=f"Map viewer link for `{layer}` layer",
+                            title=f"Map viewer link for `{layer}` layer (Template URL).",
                             rel="map",
                             href=map_viewer_endpoint + f"?{qs}",
+                            templated=True,
                         ),
                     )
 
             except NoMatchFound:
                 pass
 
             try:
-                wmts_endpoint = factory.url_for(request, "wmts")
+                wmts_endpoint = factory.url_for(
+                    request, "wmts", tileMatrixSetId="{tileMatrixSetId}"
+                )
                 links.append(
                     model.Link(
                         rel="wmts",
                         title="WMTS link (Template URL)",
                         href=wmts_endpoint,
+                        templated=True,
                     )
                 )
-                for _layer, qs in layers:
-                    links.append(
-                        model.Link(
-                            title=f"WMTS link for `{layer}` layer",
-                            rel="wmts",
-                            href=wmts_endpoint + f"?{qs}",
-                        ),
-                    )
 
             except NoMatchFound:
                 pass
 
             return model.Info(search=search_info, links=links)
```

### Comparing `titiler.pgstac-1.2.3/titiler/pgstac/factory.py` & `titiler.pgstac-1.3.0/titiler/pgstac/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         ]
     ),
 )
 DEFAULT_TEMPLATES = Jinja2Templates(env=jinja2_env)
 
 
 def check_query_params(
-    *, dependencies: List[Callable], query_params: QueryParams
+    *, dependencies: List[Callable], query_params: Union[QueryParams, Dict]
 ) -> None:
     """Check QueryParams for Query dependency.
 
     1. `get_dependant` is used to get the query-parameters required by the `callable`
     2. we use `request_params_to_args` to construct arguments needed to call the `callable`
     3. we call the `callable` and catch any errors
 
@@ -161,18 +161,26 @@
 
         if self.add_viewer:
             self._map_routes()
 
     def _tiles_routes(self) -> None:
         """register tiles routes."""
 
-        @self.router.get("/tiles/{z}/{x}/{y}", **img_endpoint_params)
-        @self.router.get("/tiles/{z}/{x}/{y}.{format}", **img_endpoint_params)
-        @self.router.get("/tiles/{z}/{x}/{y}@{scale}x", **img_endpoint_params)
-        @self.router.get("/tiles/{z}/{x}/{y}@{scale}x.{format}", **img_endpoint_params)
+        @self.router.get("/tiles/{z}/{x}/{y}", **img_endpoint_params, deprecated=True)
+        @self.router.get(
+            "/tiles/{z}/{x}/{y}.{format}", **img_endpoint_params, deprecated=True
+        )
+        @self.router.get(
+            "/tiles/{z}/{x}/{y}@{scale}x", **img_endpoint_params, deprecated=True
+        )
+        @self.router.get(
+            "/tiles/{z}/{x}/{y}@{scale}x.{format}",
+            **img_endpoint_params,
+            deprecated=True,
+        )
         @self.router.get("/tiles/{tileMatrixSetId}/{z}/{x}/{y}", **img_endpoint_params)
         @self.router.get(
             "/tiles/{tileMatrixSetId}/{z}/{x}/{y}.{format}",
             **img_endpoint_params,
         )
         @self.router.get(
             "/tiles/{tileMatrixSetId}/{z}/{x}/{y}@{scale}x",
@@ -270,14 +278,15 @@
         """register tiles routes."""
 
         @self.router.get(
             "/tilejson.json",
             response_model=TileJSON,
             responses={200: {"description": "Return a tilejson"}},
             response_model_exclude_none=True,
+            deprecated=True,
         )
         @self.router.get(
             "/{tileMatrixSetId}/tilejson.json",
             response_model=TileJSON,
             responses={200: {"description": "Return a tilejson"}},
             response_model_exclude_none=True,
         )
@@ -354,15 +363,15 @@
             ]
             qs = [
                 (key, value)
                 for (key, value) in request.query_params._list
                 if key.lower() not in qs_key_to_remove
             ]
             if qs:
-                tiles_url += f"?{urlencode(qs)}"
+                tiles_url += f"?{urlencode(qs, doseq=True)}"
 
             tms = self.supported_tms.get(tileMatrixSetId)
             minzoom = _first_value([minzoom, search_info.metadata.minzoom], tms.minzoom)
             maxzoom = _first_value([maxzoom, search_info.metadata.maxzoom], tms.maxzoom)
             bounds = _first_value(
                 [search_info.input_search.get("bbox"), search_info.metadata.bounds],
                 tms.bbox,
@@ -374,15 +383,15 @@
                 "name": search_info.metadata.name or search_info.id,
                 "tiles": [tiles_url],
             }
 
     def _map_routes(self):  # noqa: C901
         """Register /map endpoint."""
 
-        @self.router.get("/map", response_class=HTMLResponse)
+        @self.router.get("/map", response_class=HTMLResponse, deprecated=True)
         @self.router.get("/{tileMatrixSetId}/map", response_class=HTMLResponse)
         def map_viewer(
             request: Request,
             search_id=Depends(self.path_dependency),
             tileMatrixSetId: Annotated[
                 Literal[tuple(self.supported_tms.list())],
                 f"Identifier selecting one of the TileMatrixSetId supported (default: '{self.default_tms}')",
@@ -424,32 +433,34 @@
             """Return a simple map viewer."""
             tilejson_url = self.url_for(
                 request,
                 "tilejson",
                 tileMatrixSetId=tileMatrixSetId,
             )
             if request.query_params._list:
-                tilejson_url += f"?{urlencode(request.query_params._list)}"
+                tilejson_url += f"?{urlencode(request.query_params._list, doseq=True)}"
 
             tms = self.supported_tms.get(tileMatrixSetId)
             return self.templates.TemplateResponse(
+                request,
                 name="map.html",
                 context={
-                    "request": request,
                     "tilejson_endpoint": tilejson_url,
                     "tms": tms,
                     "resolutions": [matrix.cellSize for matrix in tms],
                 },
                 media_type="text/html",
             )
 
     def _wmts_routes(self):  # noqa: C901
         """Add wmts endpoint."""
 
-        @self.router.get("/WMTSCapabilities.xml", response_class=XMLResponse)
+        @self.router.get(
+            "/WMTSCapabilities.xml", response_class=XMLResponse, deprecated=True
+        )
         @self.router.get(
             "/{tileMatrixSetId}/WMTSCapabilities.xml",
             response_class=XMLResponse,
         )
         def wmts(
             request: Request,
             search_id=Depends(self.path_dependency),
@@ -511,68 +522,77 @@
                 self.render_dependency,
                 self.pgstac_dependency,
                 self.reader_dependency,
                 self.backend_dependency,
             ]
 
             layers: List[Dict[str, Any]] = []
-            if search_info.metadata.defaults:
-                for name, values in search_info.metadata.defaults.items():
-                    query_string = urlencode(values, doseq=True)
+
+            # LAYERS from mosaic metadata
+            if renders := search_info.metadata.defaults_params:
+                for name, values in renders.items():
                     try:
                         check_query_params(
                             dependencies=tile_dependencies,
-                            query_params=QueryParams(query_string),
+                            query_params=values,
                         )
                     except Exception as e:
                         warnings.warn(
                             f"Cannot construct URL for layer `{name}`: {repr(e)}",
                             UserWarning,
                             stacklevel=2,
                         )
                         continue
 
                     layers.append(
                         {
                             "name": name,
-                            "endpoint": tiles_url + f"?{query_string}",
+                            "tiles_url": tiles_url,
+                            "query_string": urlencode(values, doseq=True)
+                            if values
+                            else None,
                         }
                     )
 
+            # LAYER from query-parameters
             qs_key_to_remove = [
                 "tilematrixsetid",
                 "tile_format",
                 "tile_scale",
                 "minzoom",
                 "maxzoom",
                 "service",
                 "request",
             ]
             qs = [
                 (key, value)
                 for (key, value) in request.query_params._list
                 if key.lower() not in qs_key_to_remove
             ]
-            if qs:
-                tiles_url += f"?{urlencode(qs)}"
 
             # Checking if we can construct a valid tile URL
             # 1. we use `check_query_params` to validate the query-parameter
             # 2. if there is no layers (from mosaic metadata) we raise the caught error
             # 3. if there no errors we then add a default `layer` to the layers stack
             try:
                 check_query_params(
                     dependencies=tile_dependencies,
                     query_params=QueryParams(qs),
                 )
             except Exception as e:
                 if not layers:
                     raise e
             else:
-                layers.append({"name": "default", "endpoint": tiles_url})
+                layers.append(
+                    {
+                        "name": "default",
+                        "tiles_url": tiles_url,
+                        "query_string": urlencode(qs, doseq=True) if qs else None,
+                    }
+                )
 
             tms = self.supported_tms.get(tileMatrixSetId)
             minzoom = _first_value([minzoom, search_info.metadata.minzoom], tms.minzoom)
             maxzoom = _first_value([maxzoom, search_info.metadata.maxzoom], tms.maxzoom)
             bounds = _first_value(
                 [search_info.input_search.get("bbox"), search_info.metadata.bounds],
                 tms.bbox,
@@ -590,18 +610,21 @@
                             <TileHeight>{matrix.tileHeight}</TileHeight>
                             <MatrixWidth>{matrix.matrixWidth}</MatrixWidth>
                             <MatrixHeight>{matrix.matrixHeight}</MatrixHeight>
                         </TileMatrix>"""
                 tileMatrix.append(tm)
 
             return self.templates.TemplateResponse(
-                "wmts.xml",
-                {
-                    "request": request,
+                request,
+                name="wmts.xml",
+                context={
                     "title": search_info.metadata.name or search_id,
+                    "service_url": self.url_for(
+                        request, "wmts", tileMatrixSetId=tileMatrixSetId
+                    ),
                     "bounds": bounds,
                     "tileMatrix": tileMatrix,
                     "tms": tms,
                     "layers": layers,
                     "media_type": tile_format.mediatype,
                 },
                 media_type=MediaType.xml.value,
@@ -609,14 +632,15 @@
 
     def _assets_routes(self):
         """Register assets routes."""
 
         @self.router.get(
             "/tiles/{z}/{x}/{y}/assets",
             responses={200: {"description": "Return list of assets"}},
+            deprecated=True,
         )
         @self.router.get(
             "/tiles/{tileMatrixSetId}/{z}/{x}/{y}/assets",
             responses={200: {"description": "Return list of assets"}},
             response_model=List[Dict],
         )
         def assets_for_tile(
@@ -987,101 +1011,108 @@
                 )
                 search_info = cursor.fetchone()
 
         links: List[model.Link] = []
 
         base_url = str(request.base_url)
 
-        mosaic_info_endpoint = None
         try:
-            mosaic_info_endpoint = str(
-                app.url_path_for(
-                    "info_search", search_id=search_info.id
-                ).make_absolute_url(base_url=base_url)
-            )
             links.append(
                 model.Link(
-                    rel="metadata", title="Mosaic metadata", href=mosaic_info_endpoint
+                    rel="metadata",
+                    title="Mosaic metadata",
+                    href=str(
+                        app.url_path_for(
+                            "info",
+                            search_id=search_info.id,
+                        ).make_absolute_url(base_url=base_url)
+                    ),
                 ),
             )
         except NoMatchFound:
             pass
 
         tilejson_endpoint = None
         try:
             tilejson_endpoint = str(
                 app.url_path_for(
-                    "tilejson", search_id=search_info.id
+                    "tilejson",
+                    search_id=search_info.id,
+                    tileMatrixSetId="{tileMatrixSetId}",
                 ).make_absolute_url(base_url=base_url)
             )
 
             links.append(
                 model.Link(
-                    rel="tilejson", title="Link for TileJSON", href=tilejson_endpoint
+                    rel="tilejson",
+                    title="Link for TileJSON (Template URL)",
+                    href=tilejson_endpoint,
+                    templated=True,
                 )
             )
         except NoMatchFound:
             pass
 
-        map_endpoint = None
         try:
-            map_endpoint = str(
-                app.url_path_for(
-                    "map_viewer",
-                    search_id=search_info.id,
-                ).make_absolute_url(base_url=base_url)
-            )
-
             links.append(
                 model.Link(
                     rel="map",
-                    title="Link for Map viewer",
-                    href=map_endpoint,
+                    title="Link for Map viewer (Template URL)",
+                    href=str(
+                        app.url_path_for(
+                            "map_viewer",
+                            search_id=search_info.id,
+                            tileMatrixSetId="{tileMatrixSetId}",
+                        ).make_absolute_url(base_url=base_url)
+                    ),
+                    templated=True,
                 )
             )
         except NoMatchFound:
             pass
 
         try:
             links.append(
                 model.Link(
                     rel="wmts",
-                    title="Link for WMTS",
+                    title="Link for WMTS (Template URL)",
                     href=str(
                         app.url_path_for(
                             "wmts",
                             search_id=search_info.id,
+                            tileMatrixSetId="{tileMatrixSetId}",
                         ).make_absolute_url(base_url=base_url)
                     ),
+                    templated=True,
                 )
             )
         except NoMatchFound:
             pass
 
-        if search_info.metadata.defaults:
-            for name, values in search_info.metadata.defaults.items():
-                query_string = urlencode(values, doseq=True)
+        if renders := search_info.metadata.defaults_params:
+            for name, values in renders.items():
                 try:
                     check_query_params(
                         dependencies=tile_dependencies,
-                        query_params=QueryParams(query_string),
+                        query_params=values,
                     )
                 except Exception as e:
                     warnings.warn(
                         f"Cannot construct URL for layer `{name}`: {repr(e)}",
                         UserWarning,
                         stacklevel=2,
                     )
                     continue
 
                 links.append(
                     model.Link(
-                        title=f"TileJSON link for `{name}` layer.",
+                        title=f"TileJSON link for `{name}` layer (Template URL).",
                         rel="tilejson",
-                        href=f"{tilejson_endpoint}?{query_string}",
+                        href=f"{tilejson_endpoint}?{urlencode(values, doseq=True)}",
+                        templated=True,
                     )
                 )
 
         return model.RegisterResponse(id=search_info.id, links=links)
 
 
 def add_search_list_route(  # noqa: C901
@@ -1222,27 +1253,29 @@
             links.append(
                 model.Link(rel="prev", href=f"{list_endpoint}?{qs}"),
             )
 
         tilejson_endpoint = None
         try:
             tilejson_endpoint = str(
-                app.url_path_for("tilejson", search_id="{search_id}").make_absolute_url(
-                    base_url=base_url
-                )
+                app.url_path_for(
+                    "tilejson",
+                    search_id="{search_id}",
+                    tileMatrixSetId="{tileMatrixSetId}",
+                ).make_absolute_url(base_url=base_url)
             )
         except NoMatchFound:
             pass
 
         mosaic_info_endpoint = None
         try:
             mosaic_info_endpoint = str(
-                app.url_path_for(
-                    "info_search", search_id="{search_id}"
-                ).make_absolute_url(base_url=base_url)
+                app.url_path_for("info", search_id="{search_id}").make_absolute_url(
+                    base_url=base_url
+                )
             )
         except NoMatchFound:
             pass
 
         searches = []
         for search in searches_info:
             search_links: List[model.Link] = []
@@ -1255,16 +1288,17 @@
                     ),
                 )
 
             if tilejson_endpoint:
                 search_links.append(
                     model.Link(
                         rel="tilejson",
-                        title="Link for TileJSON",
+                        title="Link for TileJSON (Template URL)",
                         href=tilejson_endpoint.replace("{search_id}", search.id),
+                        templated=True,
                     ),
                 )
 
             searches.append(model.Info(search=search, links=search_links))
 
         return model.Infos(
             searches=searches,
```

### Comparing `titiler.pgstac-1.2.3/titiler/pgstac/main.py` & `titiler.pgstac-1.3.0/titiler/pgstac/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,24 +2,30 @@
 
 import logging
 import re
 from contextlib import asynccontextmanager
 from typing import Dict
 
 import jinja2
-from fastapi import FastAPI, Query
+from fastapi import FastAPI, Path, Query
 from psycopg import OperationalError
+from psycopg.rows import dict_row
 from psycopg_pool import PoolTimeout
 from starlette.middleware.cors import CORSMiddleware
 from starlette.requests import Request
 from starlette.responses import HTMLResponse
 from starlette.templating import Jinja2Templates
 
 from titiler.core.errors import DEFAULT_STATUS_CODES, add_exception_handlers
-from titiler.core.factory import AlgorithmFactory, MultiBaseTilerFactory, TMSFactory
+from titiler.core.factory import (
+    AlgorithmFactory,
+    ColorMapFactory,
+    MultiBaseTilerFactory,
+    TMSFactory,
+)
 from titiler.core.middleware import (
     CacheControlMiddleware,
     LoggerMiddleware,
     TotalTimeMiddleware,
 )
 from titiler.core.resources.enums import OptionalHeader
 from titiler.mosaic.errors import MOSAIC_STATUS_CODES
@@ -92,22 +98,44 @@
         allow_origins=settings.cors_origins,
         allow_credentials=True,
         allow_methods=["GET", "POST", "OPTIONS"],
         allow_headers=["*"],
     )
 
 app.add_middleware(CacheControlMiddleware, cachecontrol=settings.cachecontrol)
+
+optional_headers = []
 if settings.debug:
     app.add_middleware(TotalTimeMiddleware)
     app.add_middleware(LoggerMiddleware)
 
-if settings.debug:
     optional_headers = [OptionalHeader.server_timing, OptionalHeader.x_assets]
-else:
-    optional_headers = []
+
+    @app.get("/collections", include_in_schema=False, tags=["DEBUG"])
+    async def list_collections(request: Request):
+        """list collections."""
+        with request.app.state.dbpool.connection() as conn:
+            with conn.cursor(row_factory=dict_row) as cursor:
+                cursor.execute("SELECT * FROM pgstac.all_collections();")
+                r = cursor.fetchone()
+                cols = r.get("all_collections", [])
+                return [col["id"] for col in cols]
+
+    @app.get("/collections/{collection_id}", include_in_schema=False, tags=["DEBUG"])
+    async def get_collection(request: Request, collection_id: str = Path()):
+        """get collection."""
+        with request.app.state.dbpool.connection() as conn:
+            with conn.cursor(row_factory=dict_row) as cursor:
+                cursor.execute(
+                    "SELECT * FROM get_collection(%s);",
+                    (collection_id,),
+                )
+                r = cursor.fetchone()
+                return r.get("get_collection") or {}
+
 
 ###############################################################################
 # STAC Search Endpoints
 searches = MosaicTilerFactory(
     path_dependency=SearchIdParams,
     optional_headers=optional_headers,
     router_prefix="/searches/{search_id}",
@@ -146,14 +174,17 @@
 collection = MosaicTilerFactory(
     path_dependency=CollectionIdParams,
     optional_headers=optional_headers,
     router_prefix="/collections/{collection_id}",
     add_statistics=True,
     add_viewer=True,
     add_part=True,
+    extensions=[
+        searchInfoExtension(),
+    ],
 )
 app.include_router(
     collection.router, tags=["STAC Collection"], prefix="/collections/{collection_id}"
 )
 
 ###############################################################################
 # STAC Item Endpoints
@@ -176,14 +207,21 @@
 app.include_router(tms.router, tags=["Tiling Schemes"])
 
 ###############################################################################
 # Algorithms Endpoints
 algorithms = AlgorithmFactory()
 app.include_router(algorithms.router, tags=["Algorithms"])
 
+###############################################################################
+# Colormaps endpoints
+cmaps = ColorMapFactory()
+app.include_router(
+    cmaps.router,
+    tags=["ColorMaps"],
+)
 
 ###############################################################################
 # Health Check Endpoint
 @app.get("/healthz", description="Health Check", tags=["Health Check"])
 def ping(
     timeout: int = Query(1, description="Timeout getting SQL connection from the pool.")
 ) -> Dict:
@@ -196,15 +234,15 @@
         db_online = False
 
     return {"database_online": db_online}
 
 
 ###############################################################################
 # Landing Page
-@app.get("/", response_class=HTMLResponse)
+@app.get("/", response_class=HTMLResponse, tags=["Landing"])
 def landing(request: Request):
     """Get landing page."""
     data = {
         "title": "TiTiler-PgSTACr",
         "links": [
             {
                 "title": "Landing page",
@@ -231,28 +269,31 @@
                 "rel": "data",
             },
             {
                 "title": "PgSTAC Virtual Mosaic viewer (template URL)",
                 "href": app.url_path_for("map_viewer", search_id="{search_id}"),
                 "type": "text/html",
                 "rel": "data",
+                "templated": True,
             },
             {
                 "title": "PgSTAC Collection viewer (template URL)",
                 "href": app.url_path_for("map_viewer", collection_id="{collection_id}"),
                 "type": "text/html",
                 "rel": "data",
+                "templated": True,
             },
             {
                 "title": "PgSTAC Item viewer (template URL)",
                 "href": app.url_path_for(
                     "map_viewer", collection_id="{collection_id}", item_id="{item_id}"
                 ),
                 "type": "text/html",
                 "rel": "data",
+                "templated": True,
             },
             {
                 "title": "TiTiler-PgSTAC Documentation (external link)",
                 "href": "https://stac-utils.github.io/titiler-pgstac/",
                 "type": "text/html",
                 "rel": "doc",
             },
@@ -277,16 +318,17 @@
         part = crumb
         if part is None or part == "":
             part = "Home"
         crumbpath += f"/{crumb}"
         crumbs.append({"url": crumbpath.rstrip("/"), "part": part.capitalize()})
 
     return templates.TemplateResponse(
-        "index.html",
-        {
+        request,
+        name="index.html",
+        context={
             "request": request,
             "response": data,
             "template": {
                 "api_root": baseurl,
                 "params": request.query_params,
                 "title": "TiTiler-PgSTAC",
             },
```

### Comparing `titiler.pgstac-1.2.3/titiler/pgstac/mosaic.py` & `titiler.pgstac-1.3.0/titiler/pgstac/mosaic.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-1.2.3/titiler/pgstac/reader.py` & `titiler.pgstac-1.3.0/titiler/pgstac/reader.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-1.2.3/titiler/pgstac/settings.py` & `titiler.pgstac-1.3.0/titiler/pgstac/settings.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-1.2.3/titiler/pgstac/templates/index.html` & `titiler.pgstac-1.3.0/titiler/pgstac/templates/index.html`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-1.2.3/titiler/pgstac/templates/wmts.xml` & `titiler.pgstac-1.3.0/titiler/pgstac/templates/wmts.xml`

 * *Files 6% similar despite different names*

#### Comparing `titiler.pgstac-1.2.3/titiler/pgstac/templates/wmts.xml` & `titiler.pgstac-1.3.0/titiler/pgstac/templates/wmts.xml`

```diff
@@ -5,28 +5,28 @@
     <ows:ServiceType>OGC WMTS</ows:ServiceType>
     <ows:ServiceTypeVersion>1.0.0</ows:ServiceTypeVersion>
   </ows:ServiceIdentification>
   <ows:OperationsMetadata>
     <ows:Operation name="GetCapabilities">
       <ows:DCP>
         <ows:HTTP>
-          <ows:Get xlink:href="{{ request.url }}">
+          <ows:Get xlink:href="{{ service_url }}">
             <ows:Constraint name="GetEncoding">
               <ows:AllowedValues>
                 <ows:Value>RESTful</ows:Value>
               </ows:AllowedValues>
             </ows:Constraint>
           </ows:Get>
         </ows:HTTP>
       </ows:DCP>
     </ows:Operation>
     <ows:Operation name="GetTile">
       <ows:DCP>
         <ows:HTTP>
-          <ows:Get xlink:href="{{ request.url }}">
+          <ows:Get xlink:href="{{ service_url }}">
             <ows:Constraint name="GetEncoding">
               <ows:AllowedValues>
                 <ows:Value>RESTful</ows:Value>
               </ows:AllowedValues>
             </ows:Constraint>
           </ows:Get>
         </ows:HTTP>
@@ -46,20 +46,20 @@
       <Style isDefault="true">
         <ows:Identifier>default</ows:Identifier>
       </Style>
       <Format>{{ media_type }}</Format>
       <TileMatrixSetLink>
         <TileMatrixSet>{{ tms.id }}</TileMatrixSet>
       </TileMatrixSetLink>
-      <ResourceURL format="{{ media_type }}" resourceType="tile" template="{{ layer.endpoint }}"/>
+      <ResourceURL format="{{ media_type }}" resourceType="tile" template="{{ layer.tiles_url }}?{{ layer.query_string | escape }}"/>
     </Layer>
     {% endfor %}
     <TileMatrixSet>
       <ows:Identifier>{{ tms.id }}</ows:Identifier>
       <ows:SupportedCRS>{{ tms.crs.srs }}</ows:SupportedCRS>
       {% for item in tileMatrix %}
             {{ item | safe }}
             {% endfor %}
     </TileMatrixSet>
   </Contents>
-  <ServiceMetadataURL xlink:href="{{ request.url }}"/>
+  <ServiceMetadataURL xlink:href="{{ service_url }}"/>
 </Capabilities>
```

### Comparing `titiler.pgstac-1.2.3/titiler/pgstac/utils.py` & `titiler.pgstac-1.3.0/titiler/pgstac/utils.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-1.2.3/PKG-INFO` & `titiler.pgstac-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titiler.pgstac
-Version: 1.2.3
+Version: 1.3.0
 Summary: Connect PgSTAC and TiTiler.
 Keywords: COG,STAC,MosaicJSON,Fastapi,Dynamic tile server,pgSTAC
 Author-email: Vincent Sarago <vincent@developmentseed.com>,David Bitner <david@developmentseed.com>
 Requires-Python: >=3.8
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: titiler.pgstac Version: 1.2.3 Summary: Connect
+Metadata-Version: 2.1 Name: titiler.pgstac Version: 1.3.0 Summary: Connect
 PgSTAC and TiTiler. Keywords: COG,STAC,MosaicJSON,Fastapi,Dynamic tile
 server,pgSTAC Author-email: Vincent Sarago
 developmentseed.com>,David Bitner
 developmentseed.com> Requires-Python: >=3.8 Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

