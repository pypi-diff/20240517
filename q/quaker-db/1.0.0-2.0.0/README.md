# Comparing `tmp/quaker_db-1.0.0.tar.gz` & `tmp/quaker_db-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quaker_db-1.0.0.tar", max compression
+gzip compressed data, was "quaker_db-2.0.0.tar", max compression
```

## Comparing `quaker_db-1.0.0.tar` & `quaker_db-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,11 @@
--rw-r--r--   0        0        0    35149 2022-10-02 20:53:18.880902 quaker_db-1.0.0/LICENSE
--rw-r--r--   0        0        0     8910 2023-05-25 22:55:47.124702 quaker_db-1.0.0/README.md
--rw-r--r--   0        0        0     4312 2023-09-10 05:27:07.564167 quaker_db-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      280 2023-01-30 09:38:59.163699 quaker_db-1.0.0/quaker/__init__.py
--rw-r--r--   0        0        0      107 2022-12-29 22:53:00.407656 quaker_db-1.0.0/quaker/__main__.py
--rw-r--r--   0        0        0     2416 2023-01-30 09:38:59.163699 quaker_db-1.0.0/quaker/cli.py
--rw-r--r--   0        0        0       52 2023-01-30 09:38:59.163699 quaker_db-1.0.0/quaker/core/__init__.py
--rw-r--r--   0        0        0     7294 2023-01-30 10:07:10.427734 quaker_db-1.0.0/quaker/core/client.py
--rw-r--r--   0        0        0     4412 2023-01-30 09:38:59.163699 quaker_db-1.0.0/quaker/core/parser.py
--rw-r--r--   0        0        0    16028 2023-01-30 09:38:59.163699 quaker_db-1.0.0/quaker/core/query.py
--rw-r--r--   0        0        0     1485 2023-01-30 09:38:59.163699 quaker_db-1.0.0/quaker/core/record_filter.py
--rw-r--r--   0        0        0     2867 2023-01-30 09:38:59.163699 quaker_db-1.0.0/quaker/core/writer.py
--rw-r--r--   0        0        0      307 2023-01-30 09:45:16.803823 quaker_db-1.0.0/quaker/globals.py
--rw-r--r--   0        0        0      316 2023-01-30 09:45:32.050589 quaker_db-1.0.0/quaker/log.py
--rw-r--r--   0        0        0     9498 1970-01-01 00:00:00.000000 quaker_db-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-02 20:53:18.880902 quaker_db-2.0.0/LICENSE
+-rw-r--r--   0        0        0     9382 2024-05-17 02:26:01.763533 quaker_db-2.0.0/README.md
+-rw-r--r--   0        0        0     4310 2024-05-17 01:58:20.633660 quaker_db-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       52 2024-05-17 02:25:12.623323 quaker_db-2.0.0/quaker_db/__init__.py
+-rw-r--r--   0        0        0     7426 2024-05-17 02:03:50.410612 quaker_db-2.0.0/quaker_db/__main__.py
+-rw-r--r--   0        0        0     1988 2024-05-17 01:48:12.016725 quaker_db-2.0.0/quaker_db/client.py
+-rw-r--r--   0        0        0     2194 2024-05-17 01:29:58.448030 quaker_db-2.0.0/quaker_db/file.py
+-rw-r--r--   0        0        0      193 2024-05-17 01:29:58.448030 quaker_db-2.0.0/quaker_db/globals.py
+-rw-r--r--   0        0        0     3046 2024-05-17 01:48:12.224726 quaker_db-2.0.0/quaker_db/query.py
+-rw-r--r--   0        0        0      246 2024-05-17 01:29:58.452030 quaker_db-2.0.0/quaker_db/utils.py
+-rw-r--r--   0        0        0     9982 1970-01-01 00:00:00.000000 quaker_db-2.0.0/PKG-INFO
```

### Comparing `quaker_db-1.0.0/LICENSE` & `quaker_db-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quaker_db-1.0.0/pyproject.toml` & `quaker_db-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -135,26 +135,27 @@
 
 # Minimum number of public methods for a class (see R0903).
 min-public-methods = 0
 
 
 [tool.poetry]
 name = "quaker-db"
-version = "1.0.0"
+version = "2.0.0"
 description = "Lightweight python API to USGS earthquake dataset"
 authors = ["BlakeJC94 <blakejamescook@gmail.com>"]
 license = "GNU GPLv3"
 readme = "README.md"
-packages = [{include = "quaker"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pandas = "^1.5.0"
 requests = "^2.29.0"
 
 [tool.poetry.group.dev.dependencies]
-requests-mock = "^1.10.0"
 pytest = "^7.3.1"
+pandas = "^2.2.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+quaker = "quaker_db.__main__:main"
```

### Comparing `quaker_db-1.0.0/PKG-INFO` & `quaker_db-2.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: quaker-db
-Version: 1.0.0
-Summary: Lightweight python API to USGS earthquake dataset
-License: GNU GPLv3
-Author: BlakeJC94
-Author-email: blakejamescook@gmail.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pandas (>=1.5.0,<2.0.0)
-Requires-Dist: requests (>=2.29.0,<3.0.0)
-Description-Content-Type: text/markdown
-
 # Quaker
 Lightweight python API to USGS earthquake dataset.
 [API Docs are located here](https://earthquake.usgs.gov/fdsnws/event/1/)
 
 ## Installation
 Clone the repo to your system and install
 
@@ -28,156 +11,154 @@
 $ pip install .
 ```
 
 ## Quickstart
 This package comes equipped with a batteries-included CLI interface for downloading the latest
 earthquake event data in CSV, GeoJSON, and plain text format from the USGS database.
 ```
-usage: quaker [-h] [--format VAL] [--endtime TIME] [--starttime TIME] [--updatedafter TIME] [--minlatitude LAT]
-              [--minlongitude LNG] [--maxlatitude LAT] [--maxlongitude LNG] [--latitude LAT] [--longitude LNG]
-              [--maxradius VAL] [--maxradiuskm DIST] [--catalog VAL] [--contributor VAL] [--eventid VAL]
-              [--includeallmagnitudes BOOL] [--includeallorigins BOOL] [--includedeleted VAL]
-              [--includesuperceded BOOL] [--limit VAL] [--maxdepth VAL] [--maxmagnitude VAL] [--mindepth VAL]
-              [--minmagnitude VAL] [--offset VAL] [--orderby VAL] [--alertlevel VAL] [--callback VAL]
-              [--eventtype VAL] [--jsonerror BOOL] [--kmlanimated BOOL] [--kmlcolorby VAL] [--maxcdi VAL]
-              [--maxgap VAL] [--maxmmi VAL] [--maxsig VAL] [--mincdi VAL] [--minfelt VAL] [--mingap VAL]
-              [--minsig VAL] [--producttype VAL] [--productcode VAL] [--reviewstatus VAL]
-              [mode]
-
-Access USGS Earthquake dataset API Docs: https://earthquake.usgs.gov/fdsnws/event/1/ NOTE: All times use
-ISO8601 Date/Time format (yyyy-mm-ddThh:mm:ss). UTC is assumed. NOTE: Minimum/maximum longitude values may
-cross the date line at 180 or -180
+usage: quaker [-h] [--format FORMAT] [--endtime ENDTIME] [--starttime STARTTIME] [--updatedafter UPDATEDAFTER]
+              [--minlatitude MINLATITUDE] [--minlongitude MINLONGITUDE] [--maxlatitude MAXLATITUDE]
+              [--maxlongitude MAXLONGITUDE] [--latitude LATITUDE] [--longitude LONGITUDE] [--maxradius MAXRADIUS]
+              [--maxradiuskm MAXRADIUSKM] [--catalog CATALOG] [--contributor CONTRIBUTOR] [--eventid EVENTID]
+              [--includeallmagnitudes] [--includeallorigins] [--includedeleted] [--includesuperseded]
+              [--maxmagnitude MAXMAGNITUDE] [--mindepth MINDEPTH] [--minmagnitude MINMAGNITUDE] [--orderby ORDERBY]
+              [argfile]
 
 positional arguments:
-  mode                  action to perform (default: download)
+  argfile               Optional comma separated file with API arguments
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
 
-Format:
-  --format VAL          specify the output format (one of "csv", "geojson", "kml", "quakeml", "text", or
-                        "xml").
-
-Time:
-  --endtime TIME        limit to events on or before the specified end time.
-  --starttime TIME      limit to events on or after the specified start time.
-  --updatedafter TIME   limit to events updated after the specified time.
-
-Location - rectangle:
-  --minlatitude LAT     limit to events with a latitude larger than the specified minimum [-90, 90].
-  --minlongitude LNG    limit to events with a longitude larger than the specified minimum [-360, 360].
-  --maxlatitude LAT     limit to events with a latitude smaller than the specified maximum [-90, 90].
-  --maxlongitude LNG    limit to events with a longitude smaller than the specified maximum [-360, 360].
-
-Location - circle:
-  --latitude LAT        specify the latitude to be used for a radius search [-90, 90].
-  --longitude LNG       specify the longitude to be used for a radius search [-180, 180].
-  --maxradius VAL       limit to events within the specified maximum number of degrees from the geographic
-                        point defined by the latitude and longitude parameters [0, 180].
-  --maxradiuskm DIST    limit to events within the specified maximum number of kilometers from the geographic
-                        point defined by the latitude and longitude parameters [0, 20001.6].
-
-Other:
-  --catalog VAL         limit to events from a specified catalog.
-  --contributor VAL     limit to events contributed by a specified contributor.
-  --eventid VAL         select a specific event by id; event identifiers are data center specific.
-  --includeallmagnitudes BOOL
-                        specify if all magnitudes for the event should be included.
-  --includeallorigins BOOL
-                        specify if all origins for the event should be included.
-  --includedeleted VAL  specify if deleted products and events should be included. the value "only" returns
-                        only deleted events. values "true" or "false" are typecast to bool.
-  --includesuperceded BOOL
-                        specify if superseded products should be included. this also includes all deleted
-                        products, and is mutually exclusive to the includedeleted parameter.
-  --limit VAL           limit the results to the specified number of events.
-  --maxdepth VAL        limit to events with depth less than the specified maximum.
-  --maxmagnitude VAL    limit to events with a magnitude smaller than the specified maximum.
-  --mindepth VAL        limit to events with depth more than the specified minimum.
-  --minmagnitude VAL    limit to events with a magnitude larger than the specified minimum.
-  --offset VAL          return results starting at the event count specified, starting at 1.
-  --orderby VAL         order the results (one of "time", "time-asc", "magnitude", or "magnitude-asc").
-
-Extensions:
-  --alertlevel VAL      limit to events with a specific pager alert level (one of "green", "yellow", "orange",
-                        or "red").
-  --callback VAL        convert geojson output to a jsonp response using this callback.
-  --eventtype VAL       limit to events of a specific type
-  --jsonerror BOOL      request json(p) formatted output even on api error results. (only for geojson format)
-  --kmlanimated BOOL    whether to include timestamp in generated kml, for google earth animation support.
-  --kmlcolorby VAL      how earthquakes are colored (one of "age", "depth").
-  --maxcdi VAL          maximum value for maximum community determined intensity reported by dyfi [0, 12].
-  --maxgap VAL          limit to events with no more than this azimuthal gap [0, 360].
-  --maxmmi VAL          maximum value for maximum modified mercalli intensity reported by shakemap [0, 12].
-  --maxsig VAL          limit to events with no more than this significance.
-  --mincdi VAL          minimum value for maximum community determined intensity reported by dyfi [0, 12].
-  --minfelt VAL         limit to events with this many dyfi responses.
-  --mingap VAL          limit to events with no less than this azimuthal gap [0, 360].
-  --minsig VAL          limit to events with no less than this significance.
-  --producttype VAL     limit to events that have this type of product associated.
-  --productcode VAL     return the event that is associated with the productcode.
-  --reviewstatus VAL    limit to events with a specific review status (one of "all", "automatic", or
-                        "reviewed").
+Formats arguments:
+  --format FORMAT       (default: quakeml) Specify the output format, one of csv, geojson, kml, quakeml, csv, text,
+                        xml
+
+Time arguments:
+  --endtime ENDTIME     (default: present time) Limit to events on or before the specified end time. NOTE: All times
+                        use ISO8601 Date/Time format. Unless a timezone is specified, UTC is assumed
+  --starttime STARTTIME
+                        (default: NOW - 30 days) Limit to events on or after the specified start time. NOTE: All
+                        times use ISO8601 Date/Time format. Unless a timezone is specified, UTC is assumed
+  --updatedafter UPDATEDAFTER
+                        (default: null) Limit to events updated after the specified time. NOTE: All times use
+                        ISO8601 Date/Time format. Unless a timezone is specified, UTC is assumed
+
+Location (rectangle) arguments:
+  --minlatitude MINLATITUDE
+                        (default: -90) [-90,90] degrees, Limit to events with a latitude larger than the specified
+                        minimum. NOTE: min values must be less than max values
+  --minlongitude MINLONGITUDE
+                        (default: -180) [-360,360] degrees, Limit to events with a longitude larger than the
+                        specified minimum. NOTE: rectangles may cross the date line by using a minlongitude < -180
+                        or maxlongitude > 180. NOTE: min values must be less than max values
+  --maxlatitude MAXLATITUDE
+                        (default: 90) [-90,90] degrees, Limit to events with a latitude smaller than the specified
+                        maximum. NOTE: min values must be less than max values
+  --maxlongitude MAXLONGITUDE
+                        (default: 180) [-360,360] degrees, Limit to events with a longitude smaller than the
+                        specified maximum. NOTE: rectangles may cross the date line by using a minlongitude < -180
+                        or maxlongitude > 180. NOTE: min values must be less than max values
+
+Location (circle) arguments:
+  --latitude LATITUDE   (default: null) [-90,90] degrees, Specify the latitude to be used for a radius search
+  --longitude LONGITUDE
+                        (default: null) [-180,180] degrees, Specify the longitude to be used for a radius search
+  --maxradius MAXRADIUS
+                        (default: 180) [0, 180] degrees, Limit to events within the specified maximum number of
+                        degrees from the geographic point defined by the latitude and longitude parameters. NOTE:
+                        This option is mutually exclusive with maxradiuskm and specifying both will result in an
+                        error
+  --maxradiuskm MAXRADIUSKM
+                        (default: 20001.6) [0, 20001.6] km, Limit to events within the specified maximum number of
+                        kilometers from the geographic point defined by the latitude and longitude parameters. NOTE:
+                        This option is mutually exclusive with maxradius and specifying both will result in an error
+
+Other arguments:
+  --catalog CATALOG     (default: null) Limit to events from a specified catalog. Use the Catalogs Method to find
+                        available catalogs. NOTE: when catalog and contributor are omitted, the most preferred
+                        information from any catalog or contributor for the event is returned
+  --contributor CONTRIBUTOR
+                        (default: null) Limit to events contributed by a specified contributor. Use the Contributors
+                        Method to find available contributors. NOTE: when catalog and contributor are omitted, the
+                        most preferred information from any catalog or contributor for the event is returned
+  --eventid EVENTID     (default: null) Select a specific event by ID; event identifiers are data center specific.
+                        NOTE: Selecting a specific event implies includeallorigins, includeallmagnitudes, and,
+                        additionally, associated moment tensor and focal-mechanisms are included
+  --includeallmagnitudes
+                        (default: false) Specify if all magnitudes for the event should be included, default is data
+                        center dependent but is suggested to be the preferred magnitude only. NOTE: because
+                        magnitudes and origins are strongly associated, this parameter is interchangeable with
+                        includeallmagnitude
+  --includeallorigins   (default: false) Specify if all origins for the event should be included, default is data
+                        center dependent but is suggested to be the preferred origin only. NOTE: because magnitudes
+                        and origins are strongly associated, this parameter is interchangable with
+                        includeallmagnitude
+  --includedeleted      (default: false) Specify if deleted products and events should be included. The value only
+                        returns only deleted events. Deleted events otherwise return the HTTP status 409 Conflict.
+                        NOTE: Only supported by the csv and geojson formats, which include status
+  --includesuperseded   (default: false) Specify if superseded products should be included. This also includes all
+                        deleted products, and is mutually exclusive to the includedeleted parameter. NOTE: Only
+                        works when specifying eventid parameter
+  --maxmagnitude MAXMAGNITUDE
+                        (default: null) Limit to events with a magnitude smaller than the specified maximum
+  --mindepth MINDEPTH   (default: -100) [-100, 1000] km Limit to events with depth more than the specified minimum
+  --minmagnitude MINMAGNITUDE
+                        (default: null) Limit to events with a magnitude larger than the specified minimum
+  --orderby ORDERBY     Order the results. The allowed values are: time, time-asc, magnitude, magnitude-asc
 ```
 
 Run `quaker download` and specify the parameters as keyword arguments and pipe the output to any
 location:
 ```bash
 $ quaker download --format csv --starttime 2022-08-01 --endtime 2022-09-01 > earthquake_data.csv
 ```
 
 For more details on the available query parameters, use `quaker --help` or view the
 [USGS documentation](https://earthquake.usgs.gov/fdsnws/event/1/).
 
 Using the python API is also fairly straight-forward:
 ```python
->>> from quaker import Query, Client
+>>> import io
+>>> import pandas as pd
+>>> from quaker_db import Client
 >>> client = Client()
 # An empty query defaults to all events in the last 30 days
->>> events_from_last_30_days = Query()
->>> client.execute(events_from_last_30_days, output_file="./path/to/example/output_1.csv")
+>>> recent_events = client.execute(format="csv")
+>>> df = pd.read_csv(io.StringIO(recent_events))
 # Large multi-page queries can also be handled
->>> events_from_last_5_months = Query(
+>>> events_from_last_5_months = client.execute(
 ...     format="csv",
 ...     starttime="2022-05-01",
 ...     endtime="2022-10-01",
 ... )
->>> client.execute(events_from_last_5_months, output_file="./path/to/example/output_2.csv")
-# Calling `client.execute` without an output file return results as a pandas DataFrame
->>> results = client.execute(events_from_last_5_months)
+>>> df = pd.read_csv(io.StringIO(events_from_last_5_months))
 # You can filter results by location using the API
->>> fields = {
-...     "format": "csv",
-...     "starttime": "2022-08-01",
-...     "endtime": "2022-09-01",
-...     "latitude": 35.652832,
-...     "longitude": 139.839478,
-...     "maxradiuskm": 120.0,
-...     "minmagnitude": 3.0,
+>>> events_in_august_in_120km_within_tokyo_above_mag_3 = client.execute(
+...     forma="csv",
+...     starttime="2022-08-01",
+...     endtime="2022-09-01",
+...     latitude=35.652832,
+...     longitude=139.839478,
+...     maxradiuskm=120.0,
+...     minmagnitude=3.0,
 ... }
->>> events_in_august_in_120km_within_tokyo_above_mag_3 = Query(**fields)
->>> client.execute(
-...     events_in_august_in_120km_within_tokyo_above_mag_3,
-...     output_file="./path/to/example/output_3.csv"
-... )
-# See `help(Query)` and https://earthquake.usgs.gov/fdsnws/event/1/ for more details
+# See `help(quaker_db.Query)` and https://earthquake.usgs.gov/fdsnws/event/1/ for more details
 ```
 
 ## Contributing
 This is a small personal project, but pull requests are most welcome!
 
 * Code is styled using `[black](https://github.com/psf/black)` (`pip install black`)
-* Code is linted with `pylint` (`pip install pylint`)
-* Requirements are managed using `pip-tools` (run `pip install pip-tools` if needed)
-    * Add dependencies by adding packages to `setup.py` and running `pip-compile`
+* Code is linted with `ruff` (`pip install ruff`)
+* Requirements are managed using `poetry`
 * [Semantic versioning](https://semver.org) is used in this repo
     * Major version: rare, substantial changes that break backward compatibility
     * Minor version: most changes - new features, models or improvements
     * Patch version: small bug fixes and documentation-only changes
 
 Virtual environment handling by `poetry` is preferred:
 ```bash
 # in the project directory
 $ poetry install
 $ poetry shell
 ```
-
```

