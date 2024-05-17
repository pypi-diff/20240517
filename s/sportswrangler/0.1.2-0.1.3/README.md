# Comparing `tmp/sportswrangler-0.1.2.tar.gz` & `tmp/sportswrangler-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sportswrangler-0.1.2.tar", max compression
+gzip compressed data, was "sportswrangler-0.1.3.tar", max compression
```

## Comparing `sportswrangler-0.1.2.tar` & `sportswrangler-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      454 2024-05-14 01:43:55.634893 sportswrangler-0.1.2/README.md
--rw-r--r--   0        0        0      422 2024-05-14 01:43:55.638893 sportswrangler-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      169 2024-05-14 01:43:55.638893 sportswrangler-0.1.2/sportswrangler/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 01:43:55.638893 sportswrangler-0.1.2/sportswrangler/generic/__init__.py
--rw-r--r--   0        0        0     2065 2024-05-14 01:43:55.638893 sportswrangler-0.1.2/sportswrangler/generic/wrangler.py
--rw-r--r--   0        0        0      154 2024-05-14 01:43:55.638893 sportswrangler-0.1.2/sportswrangler/global_configs.py
--rw-r--r--   0        0        0       28 2024-05-14 01:43:55.638893 sportswrangler-0.1.2/sportswrangler/odds/__init__.py
--rw-r--r--   0        0        0      206 2024-05-14 01:43:55.638893 sportswrangler-0.1.2/sportswrangler/odds/the_odds_api/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 01:43:55.638893 sportswrangler-0.1.2/sportswrangler/odds/the_odds_api/utils/__init__.py
--rw-r--r--   0        0        0     3747 2024-05-14 01:43:55.638893 sportswrangler-0.1.2/sportswrangler/odds/the_odds_api/utils/classes.py
--rw-r--r--   0        0        0      238 2024-05-14 01:43:55.638893 sportswrangler-0.1.2/sportswrangler/odds/the_odds_api/utils/constants.py
--rw-r--r--   0        0        0     4739 2024-05-14 01:43:55.638893 sportswrangler-0.1.2/sportswrangler/odds/the_odds_api/utils/enums.py
--rw-r--r--   0        0        0      252 2024-05-14 01:43:55.638893 sportswrangler-0.1.2/sportswrangler/odds/the_odds_api/wranglers/__init__.py
--rw-r--r--   0        0        0    20184 2024-05-14 01:43:55.638893 sportswrangler-0.1.2/sportswrangler/odds/the_odds_api/wranglers/base.py
--rw-r--r--   0        0        0     2059 2024-05-14 01:43:55.638893 sportswrangler-0.1.2/sportswrangler/odds/the_odds_api/wranglers/epl.py
--rw-r--r--   0        0        0     2109 2024-05-14 01:43:55.638893 sportswrangler-0.1.2/sportswrangler/odds/the_odds_api/wranglers/mlb.py
--rw-r--r--   0        0        0     1979 2024-05-14 01:43:55.638893 sportswrangler-0.1.2/sportswrangler/odds/the_odds_api/wranglers/nba.py
--rw-r--r--   0        0        0     2306 2024-05-14 01:43:55.638893 sportswrangler-0.1.2/sportswrangler/odds/the_odds_api/wranglers/nfl.py
--rw-r--r--   0        0        0     1382 2024-05-14 01:43:55.638893 sportswrangler-0.1.2/sportswrangler/odds/the_odds_api/wranglers/nhl.py
--rw-r--r--   0        0        0       51 2024-05-14 01:43:55.638893 sportswrangler-0.1.2/sportswrangler/sports/__init__.py
--rw-r--r--   0        0        0       40 2024-05-14 01:43:55.638893 sportswrangler-0.1.2/sportswrangler/sports/data_feeds/__init__.py
--rw-r--r--   0        0        0   531535 2024-05-14 01:43:55.642893 sportswrangler-0.1.2/sportswrangler/sports/data_feeds/assets/MLB/players.csv
--rw-r--r--   0        0        0     5204 2024-05-14 01:43:55.642893 sportswrangler-0.1.2/sportswrangler/sports/data_feeds/assets/MLB/teams.csv
--rw-r--r--   0        0        0   144790 2024-05-14 01:43:55.642893 sportswrangler-0.1.2/sportswrangler/sports/data_feeds/assets/NBA/players.csv
--rw-r--r--   0        0        0     3101 2024-05-14 01:43:55.642893 sportswrangler-0.1.2/sportswrangler/sports/data_feeds/assets/NBA/teams.csv
--rw-r--r--   0        0        0   774056 2024-05-14 01:43:55.646893 sportswrangler-0.1.2/sportswrangler/sports/data_feeds/assets/NFL/players.csv
--rw-r--r--   0        0        0     8878 2024-05-14 01:43:55.646893 sportswrangler-0.1.2/sportswrangler/sports/data_feeds/assets/NFL/teams.csv
--rw-r--r--   0        0        0   293594 2024-05-14 01:43:55.646893 sportswrangler-0.1.2/sportswrangler/sports/data_feeds/assets/NHL/players.csv
--rw-r--r--   0        0        0     3313 2024-05-14 01:43:55.646893 sportswrangler-0.1.2/sportswrangler/sports/data_feeds/assets/NHL/teams.csv
--rw-r--r--   0        0        0    12392 2024-05-14 01:43:55.646893 sportswrangler-0.1.2/sportswrangler/sports/data_feeds/wrangler.py
--rw-r--r--   0        0        0        0 2024-05-14 01:43:55.646893 sportswrangler-0.1.2/sportswrangler/utils/__init__.py
--rw-r--r--   0        0        0      250 2024-05-14 01:43:55.646893 sportswrangler-0.1.2/sportswrangler/utils/enums.py
--rw-r--r--   0        0        0      142 2024-05-14 01:43:55.646893 sportswrangler-0.1.2/sportswrangler/utils/helpers.py
--rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 sportswrangler-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      454 2024-05-17 05:12:12.889492 sportswrangler-0.1.3/README.md
+-rw-r--r--   0        0        0      422 2024-05-17 05:12:12.893493 sportswrangler-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      169 2024-05-17 05:12:12.893493 sportswrangler-0.1.3/sportswrangler/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-17 05:12:12.893493 sportswrangler-0.1.3/sportswrangler/generic/__init__.py
+-rw-r--r--   0        0        0     2070 2024-05-17 05:12:12.893493 sportswrangler-0.1.3/sportswrangler/generic/wrangler.py
+-rw-r--r--   0        0        0      149 2024-05-17 05:12:12.893493 sportswrangler-0.1.3/sportswrangler/global_configs.py
+-rw-r--r--   0        0        0       28 2024-05-17 05:12:12.893493 sportswrangler-0.1.3/sportswrangler/odds/__init__.py
+-rw-r--r--   0        0        0      206 2024-05-17 05:12:12.893493 sportswrangler-0.1.3/sportswrangler/odds/the_odds_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-17 05:12:12.893493 sportswrangler-0.1.3/sportswrangler/odds/the_odds_api/utils/__init__.py
+-rw-r--r--   0        0        0     3747 2024-05-17 05:12:12.893493 sportswrangler-0.1.3/sportswrangler/odds/the_odds_api/utils/classes.py
+-rw-r--r--   0        0        0      238 2024-05-17 05:12:12.893493 sportswrangler-0.1.3/sportswrangler/odds/the_odds_api/utils/constants.py
+-rw-r--r--   0        0        0     4739 2024-05-17 05:12:12.893493 sportswrangler-0.1.3/sportswrangler/odds/the_odds_api/utils/enums.py
+-rw-r--r--   0        0        0      252 2024-05-17 05:12:12.893493 sportswrangler-0.1.3/sportswrangler/odds/the_odds_api/wranglers/__init__.py
+-rw-r--r--   0        0        0    20184 2024-05-17 05:12:12.893493 sportswrangler-0.1.3/sportswrangler/odds/the_odds_api/wranglers/base.py
+-rw-r--r--   0        0        0     2059 2024-05-17 05:12:12.893493 sportswrangler-0.1.3/sportswrangler/odds/the_odds_api/wranglers/epl.py
+-rw-r--r--   0        0        0     2109 2024-05-17 05:12:12.893493 sportswrangler-0.1.3/sportswrangler/odds/the_odds_api/wranglers/mlb.py
+-rw-r--r--   0        0        0     1979 2024-05-17 05:12:12.893493 sportswrangler-0.1.3/sportswrangler/odds/the_odds_api/wranglers/nba.py
+-rw-r--r--   0        0        0     2306 2024-05-17 05:12:12.893493 sportswrangler-0.1.3/sportswrangler/odds/the_odds_api/wranglers/nfl.py
+-rw-r--r--   0        0        0     1382 2024-05-17 05:12:12.893493 sportswrangler-0.1.3/sportswrangler/odds/the_odds_api/wranglers/nhl.py
+-rw-r--r--   0        0        0       51 2024-05-17 05:12:12.893493 sportswrangler-0.1.3/sportswrangler/sports/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-17 05:12:12.893493 sportswrangler-0.1.3/sportswrangler/sports/data_feeds/__init__.py
+-rw-r--r--   0        0        0   531535 2024-05-17 05:12:12.897493 sportswrangler-0.1.3/sportswrangler/sports/data_feeds/assets/MLB/players.csv
+-rw-r--r--   0        0        0     5204 2024-05-17 05:12:12.897493 sportswrangler-0.1.3/sportswrangler/sports/data_feeds/assets/MLB/teams.csv
+-rw-r--r--   0        0        0   144790 2024-05-17 05:12:12.897493 sportswrangler-0.1.3/sportswrangler/sports/data_feeds/assets/NBA/players.csv
+-rw-r--r--   0        0        0     3101 2024-05-17 05:12:12.897493 sportswrangler-0.1.3/sportswrangler/sports/data_feeds/assets/NBA/teams.csv
+-rw-r--r--   0        0        0   774056 2024-05-17 05:12:12.901492 sportswrangler-0.1.3/sportswrangler/sports/data_feeds/assets/NFL/players.csv
+-rw-r--r--   0        0        0     8878 2024-05-17 05:12:12.901492 sportswrangler-0.1.3/sportswrangler/sports/data_feeds/assets/NFL/teams.csv
+-rw-r--r--   0        0        0   293594 2024-05-17 05:12:12.901492 sportswrangler-0.1.3/sportswrangler/sports/data_feeds/assets/NHL/players.csv
+-rw-r--r--   0        0        0     3313 2024-05-17 05:12:12.901492 sportswrangler-0.1.3/sportswrangler/sports/data_feeds/assets/NHL/teams.csv
+-rw-r--r--   0        0        0    12392 2024-05-17 05:12:12.901492 sportswrangler-0.1.3/sportswrangler/sports/data_feeds/wrangler.py
+-rw-r--r--   0        0        0        0 2024-05-17 05:12:12.901492 sportswrangler-0.1.3/sportswrangler/utils/__init__.py
+-rw-r--r--   0        0        0      250 2024-05-17 05:12:12.901492 sportswrangler-0.1.3/sportswrangler/utils/enums.py
+-rw-r--r--   0        0        0      142 2024-05-17 05:12:12.901492 sportswrangler-0.1.3/sportswrangler/utils/helpers.py
+-rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 sportswrangler-0.1.3/PKG-INFO
```

### Comparing `sportswrangler-0.1.2/sportswrangler/generic/wrangler.py` & `sportswrangler-0.1.3/sportswrangler/generic/wrangler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Literal
 
 from pydantic import BaseModel, model_validator, ConfigDict
 from requests import Session
 from requests.adapters import HTTPAdapter
 from typing_extensions import Self
-from urllib3 import Retry
+from urllib3.util import Retry
 
 from sportswrangler.global_configs import default_retry_config
 from sportswrangler.utils.enums import Sport
 
 
 class Wrangler(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
```

### Comparing `sportswrangler-0.1.2/sportswrangler/odds/the_odds_api/utils/classes.py` & `sportswrangler-0.1.3/sportswrangler/odds/the_odds_api/utils/classes.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.2/sportswrangler/odds/the_odds_api/utils/enums.py` & `sportswrangler-0.1.3/sportswrangler/odds/the_odds_api/utils/enums.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.2/sportswrangler/odds/the_odds_api/wranglers/base.py` & `sportswrangler-0.1.3/sportswrangler/odds/the_odds_api/wranglers/base.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.2/sportswrangler/odds/the_odds_api/wranglers/epl.py` & `sportswrangler-0.1.3/sportswrangler/odds/the_odds_api/wranglers/epl.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.2/sportswrangler/odds/the_odds_api/wranglers/mlb.py` & `sportswrangler-0.1.3/sportswrangler/odds/the_odds_api/wranglers/mlb.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.2/sportswrangler/odds/the_odds_api/wranglers/nba.py` & `sportswrangler-0.1.3/sportswrangler/odds/the_odds_api/wranglers/nba.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.2/sportswrangler/odds/the_odds_api/wranglers/nfl.py` & `sportswrangler-0.1.3/sportswrangler/odds/the_odds_api/wranglers/nfl.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.2/sportswrangler/odds/the_odds_api/wranglers/nhl.py` & `sportswrangler-0.1.3/sportswrangler/odds/the_odds_api/wranglers/nhl.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.2/sportswrangler/sports/data_feeds/assets/MLB/players.csv` & `sportswrangler-0.1.3/sportswrangler/sports/data_feeds/assets/MLB/players.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.2/sportswrangler/sports/data_feeds/assets/MLB/teams.csv` & `sportswrangler-0.1.3/sportswrangler/sports/data_feeds/assets/MLB/teams.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.2/sportswrangler/sports/data_feeds/assets/NBA/players.csv` & `sportswrangler-0.1.3/sportswrangler/sports/data_feeds/assets/NBA/players.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.2/sportswrangler/sports/data_feeds/assets/NBA/teams.csv` & `sportswrangler-0.1.3/sportswrangler/sports/data_feeds/assets/NBA/teams.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.2/sportswrangler/sports/data_feeds/assets/NFL/players.csv` & `sportswrangler-0.1.3/sportswrangler/sports/data_feeds/assets/NFL/players.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.2/sportswrangler/sports/data_feeds/assets/NFL/teams.csv` & `sportswrangler-0.1.3/sportswrangler/sports/data_feeds/assets/NFL/teams.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.2/sportswrangler/sports/data_feeds/assets/NHL/players.csv` & `sportswrangler-0.1.3/sportswrangler/sports/data_feeds/assets/NHL/players.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.2/sportswrangler/sports/data_feeds/assets/NHL/teams.csv` & `sportswrangler-0.1.3/sportswrangler/sports/data_feeds/assets/NHL/teams.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.2/sportswrangler/sports/data_feeds/wrangler.py` & `sportswrangler-0.1.3/sportswrangler/sports/data_feeds/wrangler.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.2/PKG-INFO` & `sportswrangler-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sportswrangler
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package for wranglin' sports and sports odds data
 Author: Dejon
 Author-email: dejon.wright@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

