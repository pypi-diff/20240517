# Comparing `tmp/arbmaster-0.1.1.tar.gz` & `tmp/arbmaster-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\239294\OneDrive - V\344ster\345s Stad\Skrivbordet\project\dist\.tmp-uefw6v4q\arbmaster-0.1.1.tar", last modified: Tue Apr 30 19:47:47 2024, max compression
+gzip compressed data, was "C:\Users\239294\OneDrive - V\344ster\345s Stad\Skrivbordet\upload\dist\.tmp-z7lx0k58\arbmaster-0.1.2.tar", last modified: Fri May 17 17:15:16 2024, max compression
```

## Comparing `arbmaster-0.1.1.tar` & `arbmaster-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 19:47:47.032640 arbmaster-0.1.1/
--rw-rw-rw-   0        0        0     1086 2024-04-30 17:51:08.000000 arbmaster-0.1.1/LICENCE
--rw-rw-rw-   0        0        0     1912 2024-04-30 19:47:47.016938 arbmaster-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1342 2024-04-30 17:51:08.000000 arbmaster-0.1.1/README.md
--rw-rw-rw-   0        0        0      660 2024-04-30 19:47:22.000000 arbmaster-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-30 19:47:47.035632 arbmaster-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-30 19:47:46.756690 arbmaster-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-30 19:47:46.886711 arbmaster-0.1.1/src/arbmaster/
--rw-rw-rw-   0        0        0      168 2024-04-30 19:41:10.000000 arbmaster-0.1.1/src/arbmaster/__init__.py
--rw-rw-rw-   0        0        0     1553 2024-04-30 19:29:20.000000 arbmaster-0.1.1/src/arbmaster/calc.py
--rw-rw-rw-   0        0        0     5346 2024-04-30 17:51:08.000000 arbmaster-0.1.1/src/arbmaster/client.py
--rw-rw-rw-   0        0        0     6671 2024-04-30 17:51:08.000000 arbmaster-0.1.1/src/arbmaster/constants.py
--rw-rw-rw-   0        0        0     4363 2024-04-30 18:33:36.000000 arbmaster-0.1.1/src/arbmaster/ext.py
--rw-rw-rw-   0        0        0      527 2024-04-30 17:51:08.000000 arbmaster-0.1.1/src/arbmaster/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-30 19:47:47.016938 arbmaster-0.1.1/src/arbmaster.egg-info/
--rw-rw-rw-   0        0        0     1912 2024-04-30 19:47:46.000000 arbmaster-0.1.1/src/arbmaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      418 2024-04-30 19:47:46.000000 arbmaster-0.1.1/src/arbmaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 19:47:46.000000 arbmaster-0.1.1/src/arbmaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-30 19:47:46.000000 arbmaster-0.1.1/src/arbmaster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-30 19:47:46.000000 arbmaster-0.1.1/src/arbmaster.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-30 19:47:47.000472 arbmaster-0.1.1/tests/
--rw-rw-rw-   0        0        0     1581 2024-04-30 17:51:09.000000 arbmaster-0.1.1/tests/test_calc.py
--rw-rw-rw-   0        0        0     3440 2024-04-30 17:51:09.000000 arbmaster-0.1.1/tests/test_client.py
--rw-rw-rw-   0        0        0     4542 2024-04-30 17:51:09.000000 arbmaster-0.1.1/tests/test_ext.py
+drwxrwxrwx   0        0        0        0 2024-05-17 17:15:16.078611 arbmaster-0.1.2/
+-rw-rw-rw-   0        0        0     1086 2024-04-30 17:51:08.000000 arbmaster-0.1.2/LICENCE
+-rw-rw-rw-   0        0        0     1912 2024-05-17 17:15:16.075346 arbmaster-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1342 2024-05-17 17:14:56.000000 arbmaster-0.1.2/README.md
+-rw-rw-rw-   0        0        0      660 2024-05-17 17:13:59.000000 arbmaster-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 17:15:16.080313 arbmaster-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 17:15:16.021742 arbmaster-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 17:15:16.050867 arbmaster-0.1.2/src/arbmaster/
+-rw-rw-rw-   0        0        0      168 2024-05-17 17:06:48.000000 arbmaster-0.1.2/src/arbmaster/__init__.py
+-rw-rw-rw-   0        0        0     1553 2024-04-30 19:29:20.000000 arbmaster-0.1.2/src/arbmaster/calc.py
+-rw-rw-rw-   0        0        0     5772 2024-05-17 17:10:13.000000 arbmaster-0.1.2/src/arbmaster/client.py
+-rw-rw-rw-   0        0        0     6712 2024-05-17 16:51:26.000000 arbmaster-0.1.2/src/arbmaster/constants.py
+-rw-rw-rw-   0        0        0     4383 2024-05-17 16:56:38.000000 arbmaster-0.1.2/src/arbmaster/ext.py
+-rw-rw-rw-   0        0        0      527 2024-04-30 17:51:08.000000 arbmaster-0.1.2/src/arbmaster/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-17 17:15:16.074385 arbmaster-0.1.2/src/arbmaster.egg-info/
+-rw-rw-rw-   0        0        0     1912 2024-05-17 17:15:15.000000 arbmaster-0.1.2/src/arbmaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      418 2024-05-17 17:15:16.000000 arbmaster-0.1.2/src/arbmaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 17:15:15.000000 arbmaster-0.1.2/src/arbmaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-17 17:15:15.000000 arbmaster-0.1.2/src/arbmaster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-17 17:15:15.000000 arbmaster-0.1.2/src/arbmaster.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 17:15:16.071148 arbmaster-0.1.2/tests/
+-rw-rw-rw-   0        0        0     1581 2024-04-30 17:51:09.000000 arbmaster-0.1.2/tests/test_calc.py
+-rw-rw-rw-   0        0        0     3440 2024-04-30 17:51:09.000000 arbmaster-0.1.2/tests/test_client.py
+-rw-rw-rw-   0        0        0     4542 2024-04-30 17:51:09.000000 arbmaster-0.1.2/tests/test_ext.py
```

### Comparing `arbmaster-0.1.1/LICENCE` & `arbmaster-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.1/PKG-INFO` & `arbmaster-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arbmaster
-Version: 0.1.1
+Version: 0.1.2
 Summary: Odds api automated arbitrage calculator
 Author: Rashoo18
 License: MIT License
 Project-URL: Homepage, https://github.com/Rashoo18/arbmaster
 Project-URL: Issues, https://github.com/Rashoo18/arbmaster/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `arbmaster-0.1.1/README.md` & `arbmaster-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.1/pyproject.toml` & `arbmaster-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arbmaster"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
   "requests-cache",
   "colorlog",
 ]
 requires-python = ">=3.8"
 authors = [
   { name = "Rashoo18" },
```

### Comparing `arbmaster-0.1.1/src/arbmaster/calc.py` & `arbmaster-0.1.2/src/arbmaster/calc.py`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.1/src/arbmaster/client.py` & `arbmaster-0.1.2/src/arbmaster/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,48 +7,52 @@
     SerializerType,
     DEFAULT_CACHE_NAME,
     StrOrPath,
 )
 
 from arbmaster.ext import Match
 from arbmaster.logger import logger
-from arbmaster.constants import DEFAULT_HEADERS, DEFAULT_BOOKMAKERS, LEAGUES
+from arbmaster.constants import (
+    DEFAULT_HEADERS, 
+    DEFAULT_BOOKMAKERS,
+    DEFAULT_REQUESTS_REMAINING,
+    LEAGUES
+)
 
 
 class Client:
     
     #: Odds api url
     url: str = "https://api.the-odds-api.com/v4/sports/{}/odds"
-    
-    #: Requests remaining for the api key
-    requests_remaining: int = 500
 
     #: Available leagues to fetch
     _leagues = LEAGUES
     
     def __init__(self,
                  api_key: str,
                  *,
                  params: Optional[Dict[str, str]] = None,
                  headers: Dict[str, str] = DEFAULT_HEADERS,
                  bookmakers: List[str] = DEFAULT_BOOKMAKERS,
+                 requests_remaining: int = DEFAULT_REQUESTS_REMAINING,
                  use_cache: Optional[bool] = None,
                  cache_name: Optional[StrOrPath] = DEFAULT_CACHE_NAME,
                  expire_after: Optional[Any] = -1,
                  cache_backend: Optional[BackendSpecifier] = None,
                  serializer: Optional[SerializerType] = None
                 ) -> None:
         
         self.api_key = api_key
         self.params = params or self._make_params(api_key, bookmakers)
         if "apiKey" not in self.params.keys():
             self.update_params(apiKey=api_key)
         
         self.headers = headers
         self.bookmakers = bookmakers
+        self.requests_remaining: int = requests_remaining
         
         if use_cache:
             self.session: CachedSession = CachedSession(cache_name=cache_name,
                                                         backend=cache_backend,
                                                         serializer=serializer,
                                                         expire_after=expire_after)
         else:
@@ -79,61 +83,68 @@
         for k, v in kwargs.items():
             self.params.update({k: v})
     
     def update_headers(self, **kwargs) -> None:
         for k, v in kwargs.items():
             self.headers.update({k: v})
     
-    def parse_response(self, response: Response) -> Optional[List[Match]]:
+    def parse_response(self, response: Response, stake: float) -> Optional[List[Match]]:
         self.requests_remaining = int(response.headers.get("x-requests-remaining", 0))
         body: List[dict] = response.json()
         matches: List[Match] = []
         
         for match_data in body:
-            match: Match = Match(match_data)
+            match: Match = Match(match_data, stake=stake)
              
             if match.is_arbitrage:
                 matches.append(match)
         
         return matches if matches else None
     
-    def fetch_league(self, key: str, 
+    def fetch_league(self, 
+                     key: str,
+                     stake: float = 100,
                      timeout: Optional[float] = None) -> Optional[List[Match]]:
         if self.requests_remaining >= 2:
             url = self.url.format(key)
             resp: Response = self.session.get(url=url,
                                               params=self.params,
                                               headers=self.headers,
                                               timeout=timeout)
             
             if resp.status_code == 200:
                 logger.info(f"Successfully fetched odds for league '{key}'.")
-                return self.parse_response(response=resp)
+                return self.parse_response(response=resp, stake=stake)
             elif resp.status_code == 429:
                 logger.error("Rate Limit exceeded. We recommend spacing out requests over several seconds.")
             elif resp.status_code == 401:
                 logger.error("Unauthorized, Check that the api key is valid")
             else:
                 logger.error(f"Error: {resp.status_code}")
         else:
             logger.error("There are no requests remaining. Change/update the API key")
 
-    def fetch_all(self, timeout: Optional[float] = None) -> List[Optional[List[Match]]]:
+    def fetch_all(self,
+                stake: float = 100,
+                leagues: Optional[List[Dict[str, str]]] = None,
+                timeout: Optional[float] = None) -> List[Optional[List[Match]]]:
         result = []
-        for league in LEAGUES:
-            resp = self.fetch_league(league['key'], timeout=timeout)
+        leagues_list = leagues or LEAGUES
+        for league in leagues_list:
+            resp = self.fetch_league(league['key'], stake, timeout=timeout)
             if resp is not None:
                 result.append(resp)
         return result
     
-    def fetch_sport(self, 
+    def fetch_sport(self,
                     sport: Literal["soccer", "basketball", "icehockey"],
+                    stake: float = 100,
                     timeout: Optional[float] = None
                     ) -> List[Optional[List[Match]]]:
         result = []
         for league in LEAGUES:
             league_sport = league['key'].split('_')[0]
             if league_sport == sport.lower():
-                resp = self.fetch_league(league["key"], timeout=timeout)
+                resp = self.fetch_league(league["key"], stake, timeout=timeout)
                 if resp is not None:
                     result.append(resp)
         return result
```

### Comparing `arbmaster-0.1.1/src/arbmaster/constants.py` & `arbmaster-0.1.2/src/arbmaster/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 }
 
 DEFAULT_BOOKMAKERS: "list[str]" = [
     "sport888", "leovegas", "betsson", "betway",
     "nordicbet", "pinnacle", "mrgreen", "casumo", "coolbet"
 ]
 
+DEFAULT_REQUESTS_REMAINING: int = 500
+
 LEAGUES: "list[dict[str, str]]" = [
   {
     "key": "basketball_euroleague",
     "group": "Basketball",
     "title": "Euroleague",
     "country": "International"
   },
```

### Comparing `arbmaster-0.1.1/src/arbmaster/ext.py` & `arbmaster-0.1.2/src/arbmaster/ext.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,58 +7,59 @@
 StrPath = NewType("StrPath", str)
 
 @dataclass
 class Bookmaker:
     key: str
     title: str
     home_odds: float
-    away_odds: float
     draw_odds: Optional[float] = None
+    away_odds: float
 
     @classmethod
     def new(cls, bm_data: Dict[str, Any]) -> "Bookmaker":
         key: str = bm_data['key']
         title: str = bm_data['title']
         outcomes = bm_data['markets'][0]['outcomes']
         home_odds: float = outcomes[0]['price']
         away_odds: float = outcomes[1]['price']
         draw_odds: Optional[float] = None
         if len(outcomes) == 3:
             draw_odds = outcomes[2]['price']
-        return cls(key, title, home_odds, away_odds, draw_odds)
+        return cls(key, title, home_odds, draw_odds, away_odds)
 
     def json(self, price) -> Dict[str, Any]:
         return {
             "key": self.key,
             "title": self.title,
             "price": price
         }
 
 class Odds:
     def __init__(self, bookmakers: List[Bookmaker]) -> None:
         home = max([b.home_odds for b in bookmakers if b.home_odds is not None], default=None)
-        away = max([b.away_odds for b in bookmakers if b.away_odds is not None], default=None)
         draw = max([b.draw_odds for b in bookmakers if b.draw_odds is not None], default=None)
+        away = max([b.away_odds for b in bookmakers if b.away_odds is not None], default=None)
+        
         self.home = [bm.json(home) for bm in bookmakers if bm.home_odds == home] if home is not None else []
-        self.away = [bm.json(away) for bm in bookmakers if bm.away_odds == away] if away is not None else []
         self.draw = [bm.json(draw) for bm in bookmakers if bm.draw_odds == draw] if draw is not None else []
+        self.away = [bm.json(away) for bm in bookmakers if bm.away_odds == away] if away is not None else []
 
     @classmethod
     def new(cls, odds_data: Dict[str, Any]) -> "Odds":
-        home = [Bookmaker(bm['key'], bm['title'], bm['price'], 0) for bm in odds_data['home_team']]
-        away = [Bookmaker(bm['key'], bm['title'], 0, bm['price']) for bm in odds_data['away_team']]
-        draw = [Bookmaker(bm['key'], bm['title'], 0, 0, bm['price']) for bm in odds_data['draw'] if len(odds_data['draw']) >= 1]
+        home = [Bookmaker(bm['key'], bm['title'], bm['price'], 0, 0) for bm in odds_data['home_team']]
+        draw = [Bookmaker(bm['key'], bm['title'], 0, bm['price'], 0) for bm in odds_data['draw'] if len(odds_data['draw']) >= 1]
+        away = [Bookmaker(bm['key'], bm['title'], 0, 0, bm['price']) for bm in odds_data['away_team']]
         bookmakers = home + away + draw
         return cls(bookmakers)
         
     def json(self) -> Dict[str, Any]:
         return {
             "home_team": self.home,
-            "away_team": self.away,
-            "draw": self.draw
+            "draw": self.draw,
+            "away_team": self.away
         }
 
 class Match:
     def __init__(self, match_data: Dict[str, Any], stake: float = 100) -> None:
         self.id: str = match_data['id']
         self.sport_key: str = match_data['sport_key']
         self.sport_title: str = match_data['sport_title']
@@ -88,15 +89,15 @@
             "sport_key": self.sport_key,
             "sport_title": self.sport_title,
             "home_team": self.home_team,
             "away_team": self.away_team,
             "commence_time": self.commence_time,
             "odds": self.odds.json() if isinstance(self.odds, Odds) else self.odds
         }
-
+    
 def make_europe_time(utc_str: str) -> str:
     utc_time = datetime.strptime(utc_str, "%Y-%m-%dT%H:%M:%SZ")
     start = datetime(utc_time.year, 3, 31, 2, 0)
     end = datetime(utc_time.year, 10, 31, 3, 0)
     
     if start <= utc_time < end:
         offset = timedelta(hours=2)
```

### Comparing `arbmaster-0.1.1/src/arbmaster/logger.py` & `arbmaster-0.1.2/src/arbmaster/logger.py`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.1/src/arbmaster.egg-info/PKG-INFO` & `arbmaster-0.1.2/src/arbmaster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arbmaster
-Version: 0.1.1
+Version: 0.1.2
 Summary: Odds api automated arbitrage calculator
 Author: Rashoo18
 License: MIT License
 Project-URL: Homepage, https://github.com/Rashoo18/arbmaster
 Project-URL: Issues, https://github.com/Rashoo18/arbmaster/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `arbmaster-0.1.1/tests/test_calc.py` & `arbmaster-0.1.2/tests/test_calc.py`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.1/tests/test_client.py` & `arbmaster-0.1.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `arbmaster-0.1.1/tests/test_ext.py` & `arbmaster-0.1.2/tests/test_ext.py`

 * *Files identical despite different names*

