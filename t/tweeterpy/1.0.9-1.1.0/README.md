# Comparing `tmp/tweeterpy-1.0.9.tar.gz` & `tmp/tweeterpy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweeterpy-1.0.9.tar", last modified: Wed Oct 11 13:51:43 2023, max compression
+gzip compressed data, was "tweeterpy-1.1.0.tar", last modified: Fri May 17 15:34:54 2024, max compression
```

## Comparing `tweeterpy-1.0.9.tar` & `tweeterpy-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-10-11 13:51:43.393494 tweeterpy-1.0.9/
--rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-1.0.9/LICENSE
--rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-1.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     3583 2023-10-11 13:51:43.393494 tweeterpy-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2530 2023-10-11 13:44:39.000000 tweeterpy-1.0.9/README.md
--rw-rw-rw-   0        0        0       42 2023-10-11 13:51:43.393494 tweeterpy-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1499 2023-10-11 13:45:33.000000 tweeterpy-1.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-11 13:51:43.346596 tweeterpy-1.0.9/tweeterpy/
--rw-rw-rw-   0        0        0       34 2023-09-16 06:13:29.000000 tweeterpy-1.0.9/tweeterpy/__init__.py
--rw-rw-rw-   0        0        0     6968 2023-10-11 13:29:25.000000 tweeterpy-1.0.9/tweeterpy/api_util.py
--rw-rw-rw-   0        0        0     2505 2023-10-11 13:49:03.000000 tweeterpy-1.0.9/tweeterpy/config.py
--rw-rw-rw-   0        0        0     3770 2023-09-17 11:41:01.000000 tweeterpy-1.0.9/tweeterpy/constants.py
--rw-rw-rw-   0        0        0     2058 2023-09-09 11:19:04.000000 tweeterpy-1.0.9/tweeterpy/logging_util.py
--rw-rw-rw-   0        0        0     9024 2023-10-10 14:44:59.000000 tweeterpy-1.0.9/tweeterpy/login_util.py
--rw-rw-rw-   0        0        0     1984 2023-09-09 10:43:43.000000 tweeterpy-1.0.9/tweeterpy/request_util.py
--rw-rw-rw-   0        0        0     2481 2023-09-07 09:39:56.000000 tweeterpy-1.0.9/tweeterpy/session_util.py
--rw-rw-rw-   0        0        0    27780 2023-10-11 13:34:59.000000 tweeterpy-1.0.9/tweeterpy/tweeterpy.py
--rw-rw-rw-   0        0        0    13673 2023-10-07 13:59:32.000000 tweeterpy-1.0.9/tweeterpy/util.py
-drwxrwxrwx   0        0        0        0 2023-10-11 13:51:43.377875 tweeterpy-1.0.9/tweeterpy.egg-info/
--rw-rw-rw-   0        0        0     3583 2023-10-11 13:51:43.000000 tweeterpy-1.0.9/tweeterpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2023-10-11 13:51:43.000000 tweeterpy-1.0.9/tweeterpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-11 13:51:43.000000 tweeterpy-1.0.9/tweeterpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      192 2023-10-11 13:51:43.000000 tweeterpy-1.0.9/tweeterpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-10-11 13:51:43.000000 tweeterpy-1.0.9/tweeterpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 15:34:54.036541 tweeterpy-1.1.0/
+-rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3967 2024-05-17 15:34:54.036541 tweeterpy-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2530 2023-10-11 13:44:39.000000 tweeterpy-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-17 15:34:54.036541 tweeterpy-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2024-05-17 15:30:12.000000 tweeterpy-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:34:53.989662 tweeterpy-1.1.0/tweeterpy/
+-rw-rw-rw-   0        0        0       34 2023-09-16 06:13:29.000000 tweeterpy-1.1.0/tweeterpy/__init__.py
+-rw-rw-rw-   0        0        0     8241 2024-01-02 14:26:34.000000 tweeterpy-1.1.0/tweeterpy/api_util.py
+-rw-rw-rw-   0        0        0     2505 2023-10-11 13:49:03.000000 tweeterpy-1.1.0/tweeterpy/config.py
+-rw-rw-rw-   0        0        0     3855 2024-05-17 15:23:46.000000 tweeterpy-1.1.0/tweeterpy/constants.py
+-rw-rw-rw-   0        0        0     2058 2023-09-09 11:19:04.000000 tweeterpy-1.1.0/tweeterpy/logging_util.py
+-rw-rw-rw-   0        0        0     9024 2023-10-10 14:44:59.000000 tweeterpy-1.1.0/tweeterpy/login_util.py
+-rw-rw-rw-   0        0        0     1984 2024-01-04 12:34:59.000000 tweeterpy-1.1.0/tweeterpy/request_util.py
+-rw-rw-rw-   0        0        0     2481 2023-09-07 09:39:56.000000 tweeterpy-1.1.0/tweeterpy/session_util.py
+-rw-rw-rw-   0        0        0    32367 2024-05-17 15:23:49.000000 tweeterpy-1.1.0/tweeterpy/tweeterpy.py
+-rw-rw-rw-   0        0        0    15955 2024-05-17 15:29:39.000000 tweeterpy-1.1.0/tweeterpy/util.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:34:54.036541 tweeterpy-1.1.0/tweeterpy.egg-info/
+-rw-rw-rw-   0        0        0     3967 2024-05-17 15:34:53.000000 tweeterpy-1.1.0/tweeterpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2024-05-17 15:34:53.000000 tweeterpy-1.1.0/tweeterpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 15:34:53.000000 tweeterpy-1.1.0/tweeterpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      192 2024-05-17 15:34:53.000000 tweeterpy-1.1.0/tweeterpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-17 15:34:53.000000 tweeterpy-1.1.0/tweeterpy.egg-info/top_level.txt
```

### Comparing `tweeterpy-1.0.9/LICENSE` & `tweeterpy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.0.9/PKG-INFO` & `tweeterpy-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 1.0.9
+Version: 1.1.0
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 Home-page: https://github.com/iSarabjitDhiman/TweeterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
@@ -15,14 +15,26 @@
 Classifier: Operating System :: Unix
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: beautifulsoup4==4.12.2
+Requires-Dist: Brotli==1.0.9
+Requires-Dist: bs4==0.0.1
+Requires-Dist: certifi==2023.7.22
+Requires-Dist: charset-normalizer==3.1.0
+Requires-Dist: demjson3==3.0.6
+Requires-Dist: idna==3.7
+Requires-Dist: lxml==4.9.2
+Requires-Dist: requests==2.31.0
+Requires-Dist: six==1.16.0
+Requires-Dist: soupsieve==2.4.1
+Requires-Dist: urllib3==2.0.7
 
 <h1 align="center">TweeterPy</h1>
 
 <p align="center">
 <a href="https://choosealicense.com/licenses/mit/"> <img src="https://img.shields.io/badge/License-MIT-green.svg"></a>
 <a href="https://www.python.org/"><img src="https://img.shields.io/pypi/pyversions/tweeterpy"></a>
 <a href="https://pypi.org/project/tweeterpy/"> <img src="https://img.shields.io/pypi/v/tweeterpy"></a>
```

#### html2text {}

```diff
@@ -1,21 +1,26 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 1.0.9 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 1.1.0 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
 TweeterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
 License: MIT Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix Classifier: License :: OSI Approved :: MIT
 License Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3 Description-Content-
-Type: text/markdown License-File: LICENSE
+Type: text/markdown License-File: LICENSE Requires-Dist: beautifulsoup4==4.12.2
+Requires-Dist: Brotli==1.0.9 Requires-Dist: bs4==0.0.1 Requires-Dist:
+certifi==2023.7.22 Requires-Dist: charset-normalizer==3.1.0 Requires-Dist:
+demjson3==3.0.6 Requires-Dist: idna==3.7 Requires-Dist: lxml==4.9.2 Requires-
+Dist: requests==2.31.0 Requires-Dist: six==1.16.0 Requires-Dist:
+soupsieve==2.4.1 Requires-Dist: urllib3==2.0.7
                             ************ TTwweeeetteerrPPyy ************
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_g_r_e_e_n_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
  _p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_t_w_e_e_t_e_r_p_y_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_t_w_e_e_t_e_r_p_y_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_a_s_t_-_c_o_m_m_i_t_/_i_S_a_r_a_b_j_i_t_D_h_i_m_a_n_/_T_w_e_e_t_e_r_P_y_]_[_D_i_s_c_o_r_d_]_[_h_t_t_p_s_:_/_/
     _i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/_f_o_l_l_o_w_/_i_S_a_r_a_b_j_i_t_D_h_i_m_a_n_?_s_t_y_l_e_=_s_o_c_i_a_l_]## Overview
 TweeterPy is a python library to extract data from Twitter. TweeterPy API lets
  you scrape data from a user's profile like username, userid, bio, followers/
```

### Comparing `tweeterpy-1.0.9/README.md` & `tweeterpy-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.0.9/setup.py` & `tweeterpy-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "1.0.9"
+VERSION = "1.1.0"
 SHORT_DESCRIPTION = "TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc."
 
 with open("requirements.txt") as file:
     dependencies = file.read().splitlines()
 with open("README.md", "r") as file:
     DESCRIPTION = file.read()
```

### Comparing `tweeterpy-1.0.9/tweeterpy/api_util.py` & `tweeterpy-1.1.0/tweeterpy/api_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from . import config
 
 logging.config.dictConfig(config.LOGGING_CONFIG)
 logger = logging.getLogger(__name__)
 
 dataset_regex = re.compile(r'''exports\s*=\s*{(.*?)},''', re.VERBOSE)
 api_file_regex = re.compile(r'''api:(.*?),''', re.VERBOSE)
+main_file_regex = re.compile(r'''main(.?)(\w*).?js''', re.VERBOSE)
 feature_switch_regex = re.compile(r'''.featureSwitch.:(.*?)}},''', re.VERBOSE)
 # logging.basicConfig(level=logging.DEBUG,
 #                     format='%(asctime)s [%(levelname)s] %(module)s : %(funcName)s : %(lineno)d ::: %(message)s')
 
 
 class ApiUpdater:
     """
@@ -26,18 +27,26 @@
     def __init__(self, update_api=True):
         try:
             logger.debug('Updating API...')
             # fmt: off - Turns off formatting for this block of code.
             try:
                 if not update_api:
                     raise Exception("Skipping API Updates.")
+                api_files_data = []
                 page_source = self._get_home_page_source()
                 api_file_url = self._get_api_file_url(page_source)
+                main_file_url = self._get_main_file_url(page_source)
                 feature_switches = self._get_feature_switches(page_source)
-                api_endpoints_data = self._js_to_py_dict(self._get_api_file_content(api_file_url))
+                if api_file_url:
+                    api_files_data.append(self._get_api_file_content(api_file_url))
+                if main_file_url:
+                    api_files_data.append(self._get_main_file_content(main_file_url))
+                if not api_files_data:
+                    raise Exception("Couldn't get the API files content.")
+                api_endpoints_data = self._js_to_py_dict(api_files_data)
                 self._save_api_data(feature_switches,api_endpoints_data)
             except Exception as error:
                 logger.warn(f"{error} Couldn't get the latest API data.")
                 logger.debug("Trying to restore API data from the backup file.")
                 feature_switches, api_endpoints_data = self._load_api_data()
             current_api_endpoints = self._get_current_api_endpoints()
             new_api_endpoints = self._map_data(current_api_endpoints, api_endpoints_data)
@@ -56,34 +65,51 @@
         if page_source is None:
             page_source = self._get_home_page_source
         try:
             api_file_name = re.search(api_file_regex, page_source).group(1)
             api_file_url = f"{Path.TWITTER_CDN}/api.{eval(api_file_name)}a.js"
             logger.debug(f"API Url => {api_file_url}")
         except Exception as error:
-            logger.exception(f"Couldn't get the API Url.\n{error}")
-            raise
+            # logger.exception(f"Couldn't get the API file Url.\n{error}")
+            return None
         return api_file_url
 
+    def _get_main_file_url(self, page_source=None):
+        if page_source is None:
+            page_source = self._get_home_page_source
+        try:
+            main_file_name = re.search(main_file_regex, page_source).group(0)
+            main_file_url = f"{Path.TWITTER_CDN}/{main_file_name}"
+            logger.debug(f"Main File Url => {main_file_url}")
+        except Exception as error:
+            logger.exception(f"Couldn't get the main file Url.\n{error}")
+            return None
+        return main_file_url
+
     def _get_api_file_content(self, file_url=None):
         if file_url is None:
             file_url = self._get_api_file_url()
-        return make_request(file_url)
+        return str(make_request(file_url))
+
+    def _get_main_file_content(self, file_url=None):
+        if file_url is None:
+            file_url = self._get_main_file_url()
+        return str(make_request(file_url))
 
     def _js_to_py_dict(sel, page_source):
         if isinstance(page_source, list):
-            page_source = "\n".join([item for item in page_source])
+            page_source = "\n".join([str(item) for item in page_source])
         else:
             page_source = str(page_source)
         matches = []
         for match in dataset_regex.finditer(page_source):
             matches.append(match.group(1))
 
         dict_data = [demjson3.decode("{" + each_match)
-                     for each_match in matches]
+                     for each_match in matches if "function" not in each_match]
         return dict_data
 
     def _map_data(self, old_endpoints, new_endpoints):
         FeatureSwitch.api_endpoints = {
             f"{endpoint['queryId']}/{endpoint['operationName']}": endpoint for endpoint in new_endpoints}
         new_endpoints = {
             endpoint['operationName']: f"{endpoint['queryId']}/{endpoint['operationName']}" for endpoint in new_endpoints}
```

### Comparing `tweeterpy-1.0.9/tweeterpy/config.py` & `tweeterpy-1.1.0/tweeterpy/config.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.0.9/tweeterpy/constants.py` & `tweeterpy-1.1.0/tweeterpy/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,22 +34,23 @@
     CROSSED = "\033[9m"
     RESET = "\033[0m"
 
 
 class Path:
     # Data will be updated automatically upon API update (Manipulated by ApiUpdater in api_util.py).
     # URLS
-    DOMAIN = "twitter.com"
-    BASE_URL = "https://www.twitter.com/"
-    API_URL = "https://twitter.com/i/api/graphql/"
-    TASK_URL = "https://api.twitter.com/1.1/onboarding/task.json"
-    GUEST_TOKEN_URL = "https://api.twitter.com/1.1/guest/activate.json"
+    DOMAIN = "x.com"
+    BASE_URL = "https://x.com/"
+    API_URL = "https://x.com/i/api/graphql/"
+    TASK_URL = "https://api.x.com/1.1/onboarding/task.json"
+    GUEST_TOKEN_URL = "https://api.x.com/1.1/guest/activate.json"
     JAVSCRIPT_INSTRUMENTATION_URL = "https://twitter.com/i/js_inst"
     TWITTER_CDN = "https://abs.twimg.com/responsive-web/client-web"
-    HOME_TIMELINE_GUEST_URL = "https://twitter.com/i/api/2/guide.json"
+    HOME_TIMELINE_GUEST_URL = "https://x.com/i/api/2/guide.json"
+    X_MIGRATE_URL = "https://x.com/x/migrate"
     # ENDPOINTS
     HOME_TIMELINE_ENDPOINT = "ggIgQGz-fN1Z9YBhAoTCVA/HomeTimeline"
     HOME_LATEST_TIMELINE_ENDPOINT = "Js4oMnCV2D4gpEocblJ6Tg/HomeLatestTimeline"
     USER_ID_ENDPOINT = "9zwVLJ48lmVUk8u_Gh9DmA/ProfileSpotlightsQuery"
     USER_INFO_ENDPOINT = "8slyDObmnUzBOCu7kYZj_A/UserByRestId"
     USER_DATA_ENDPOINT = "qRednkZG-rn1P6b48NINmQ/UserByScreenName"
     MULTIPLE_USERS_DATA_ENDPOINT = "GD4q8bBE2i6cqWw2iT74Gg/UsersByRestIds"
@@ -65,14 +66,15 @@
     FOLLOWERS_ENDPOINT = "WWFQL1d4gxtqm2mjZCRa-Q/Followers"
     FOLLOWINGS_ENDPOINT = "OLcddmNLPVXGDgSdSVj0ow/Following"
     MUTUAL_FOLLOWERS_ENDPOINT = "wYAUyD58y1AFol2g2bLqzw/FollowersYouKnow"
     LIKED_TWEETS_ENDPOINT = "QPKcH_nml6UIOxHLjmNsuw/Likes"
     PROFILE_CATEGORY_ENDPOINT = "6OFpJ3TH3p8JpwOSgfgyhg/BizProfileFetchUser"
     TWEET_LIKES_ENDPOINT = "mpMee2WCjo7Nm4gRRHHnvA/Favoriters"
     RETWEETED_BY_ENDPOINT = "7Fwe5A6kE05QIybims116A/Retweeters"
+    USER_HIGHLIGHTS_ENDPOINT = "w9-i9VNm_92GYFaiyGT1NA/UserHighlightsTweets"
 
 
 class FeatureSwitch:
     # Data will be added automatically upon API update (Manipulated by ApiUpdater in api_util.py).
     all_feature_switches = {}
     api_endpoints = {}
```

### Comparing `tweeterpy-1.0.9/tweeterpy/logging_util.py` & `tweeterpy-1.1.0/tweeterpy/logging_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.0.9/tweeterpy/login_util.py` & `tweeterpy-1.1.0/tweeterpy/login_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.0.9/tweeterpy/request_util.py` & `tweeterpy-1.1.0/tweeterpy/request_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.0.9/tweeterpy/session_util.py` & `tweeterpy-1.1.0/tweeterpy/session_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.0.9/tweeterpy/tweeterpy.py` & `tweeterpy-1.1.0/tweeterpy/tweeterpy.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,15 +24,20 @@
         if config.DISABLE_LOGS or config.DISABLE_EXTERNAL_LOGS:
             logger.debug("Disabling logs...")
             config.LOG_LEVEL = "ERROR" if config.DISABLE_LOGS else config.LOG_LEVEL
             disable_external_only = config.DISABLE_EXTERNAL_LOGS if not config.DISABLE_LOGS else False
             set_log_level(logging.ERROR, external_only=disable_external_only)
         self.generate_session()
         # update api endpoints
-        ApiUpdater(update_api=config.UPDATE_API)
+        self.__token = self.session.headers.pop("Authorization")
+        try:
+            ApiUpdater(update_api=config.UPDATE_API)
+        except Exception as error:
+            logger.warn(error)
+        self.session.headers.update({"Authorization":self.__token})
 
     def _generate_request_data(self, endpoint, variables=None, **kwargs):
         # fmt: off - Turns off formatting for this block of code. Just for the readability purpose.
         url = util.generate_url(domain=Path.API_URL, url_path=endpoint)
         query_params = {}
         if variables:
             query_params["variables"] = json.dumps(variables)
@@ -40,26 +45,29 @@
             features = FeatureSwitch().get_query_features(endpoint) or util.generate_features(**kwargs)
             query_params["features"] = json.dumps(features)
         # fmt: on   
         request_payload = {"url": url, "params": query_params}
         logger.debug(f"Request Payload => {request_payload}")
         return request_payload
 
-    def _handle_pagination(self, url, params, end_cursor=None, data_path=None, total=None):
+    def _handle_pagination(self, url, params, end_cursor=None, data_path=None, total=None, pagination=True):
         # fmt: off  - Turns off formatting for this block of code. Just for the readability purpose.
         def filter_data(response):
             filtered_data = []
             for each_entry in response:
                 if each_entry['entryId'].startswith('cursor-top') or each_entry['entryId'].startswith('cursor-bottom'):
                     continue
                 filtered_data.append(each_entry)
                 if total is not None and (len(data_container['data']) + len(filtered_data)) >= total:
                     return filtered_data
             return filtered_data
 
+        if not pagination and total:
+            logger.warn("Either enable the pagination or disable total number of results.")
+            raise Exception("pagination cannot be disabled while the total number of results are specified.")
         data_container = {"data": [],"cursor_endpoint": None, "has_next_page": True, "api_rate_limit":config._RATE_LIMIT_STATS}
         while data_container["has_next_page"]:
             try:
                 if end_cursor:
                     varaibles = json.loads(params['variables'])
                     varaibles['cursor'] = end_cursor
                     params['variables'] = json.dumps(varaibles)
@@ -82,15 +90,15 @@
 
                 if end_cursor:
                     data_container['cursor_endpoint'] = end_cursor
 
                 if ((top_cursor and end_cursor) and len(data) == 2) or ((top_cursor or end_cursor) and len(data) == 1) or (not end_cursor):
                     data_container["has_next_page"] = False
 
-                if not data_container["has_next_page"] or (total is not None and len(data_container['data']) >= total):
+                if not data_container["has_next_page"] or (total is not None and len(data_container['data']) >= total) or not pagination:
                     return data_container
             # fmt: on 
             except ConnectionError as error:
                 logger.exception(error)
                 continue
 
             except Exception as error:
@@ -144,17 +152,18 @@
         try:
             logger.debug("Trying to generate a new session.")
             self.session = requests.Session()
             if config.PROXY is not None:
                 self.session.proxies = config.PROXY
                 self.session.verify = False
             self.session.headers.update(util.generate_headers())
-            make_request(Path.BASE_URL, session=self.session)
+            # home_page = make_request(Path.BASE_URL, session=self.session)
+            home_page = util.handle_x_migration(session=self.session)
             guest_token = make_request(
-                Path.GUEST_TOKEN_URL, method="POST", session=self.session)['guest_token']
+                Path.GUEST_TOKEN_URL, method="POST", session=self.session).get('guest_token', util.find_guest_token(home_page))
             self.session.headers.update({'X-Guest-Token': guest_token})
             self.session.cookies.update({'gt': guest_token})
             if auth_token:
                 self.session.cookies.update({'auth_token': auth_token})
                 util.generate_headers(self.session)
         except Exception as error:
             logger.exception(f"Couldn't generate a new session.\n{error}\n")
@@ -195,15 +204,15 @@
     def logged_in(self):
         """Check if the user is logged in.
 
         Returns:
             bool: Returns True if the user is logged in.
         """
         if "auth_token" in self.session.cookies.keys():
-            logger.info('User is authenticated.')
+            # logger.info('User is authenticated.')
             return True
         return False
 
     def login(self, username=None, password=None):
         """Log into an account.
 
         Args:
@@ -292,22 +301,23 @@
         """
         variables = {"userIds": user_ids}
         request_payload = self._generate_request_data(
             Path.MULTIPLE_USERS_DATA_ENDPOINT, variables, default_features=True)
         response = make_request(**request_payload)
         return response['data']['users']
 
-    def get_user_tweets(self, user_id, with_replies=False, end_cursor=None, total=None):
+    def get_user_tweets(self, user_id, with_replies=False, end_cursor=None, total=None, pagination=True):
         """Get Tweets from a user's profile.
 
         Args:
             user_id (int): User ID.
             with_replies (bool, optional): Set to True if want to get the tweets user replied to, from user's profile page. Defaults to False.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
             total (int, optional): Total(Max) number of results you want to get. If None, extracts all results. Defaults to None.
+            pagination (bool, optional): Set to False if want to handle each page request manually. Use end_cursor from the previous page/request to navigate to the next page. Defaults to True.
 
         Returns:
             dict: Returns data, cursor_endpoint, has_next_page
         """
         user_id = self.get_user_id(user_id)
         query_endpoint = Path.USER_TWEETS_ENDPOINT
         variables = {"userId": user_id, "count": 100, "includePromotedContent": True,
@@ -320,52 +330,54 @@
             query_endpoint = Path.USER_TWEETS_AND_REPLIES_ENDPOINT
             del variables['withQuickPromoteEligibilityTweetFields']
 
         request_payload = self._generate_request_data(
             query_endpoint, variables, additional_features=True)
         data_path = ('data', 'user', 'result', 'timeline_v2',
                      'timeline', 'instructions')
-        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total)
+        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total, pagination=pagination)
 
     @login_decorator
-    def get_user_media(self, user_id, end_cursor=None, total=None):
+    def get_user_media(self, user_id, end_cursor=None, total=None, pagination=True):
         """Get media from a user's profile.
 
         Args:
             user_id (int): User ID.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
             total (int, optional): Total(Max) number of results you want to get. If None, extracts all results. Defaults to None.
+            pagination (bool, optional): Set to False if want to handle each page request manually. Use end_cursor from the previous page/request to navigate to the next page. Defaults to True.
 
         Returns:
             dict: Returns data, cursor_endpoint, has_next_page
         """
         user_id = self.get_user_id(user_id)
         variables = {"userId": user_id, "count": 100, "includePromotedContent": False,
                      "withClientEventToken": False, "withBirdwatchNotes": False, "withVoice": True, "withV2Timeline": True}
         request_payload = self._generate_request_data(
             Path.USER_MEDIA_ENDPOINT, variables, additional_features=True)
         data_path = ('data', 'user', 'result', 'timeline_v2',
                      'timeline', 'instructions')
-        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total)
+        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total, pagination=pagination)
 
-    def get_tweet(self, tweet_id, with_tweet_replies=False, end_cursor=None, total=None):
+    def get_tweet(self, tweet_id, with_tweet_replies=False, end_cursor=None, total=None, pagination=True):
         """Get Tweets from a user's profile.
 
         Args:
             tweet_id (int): Tweet ID.
             with_tweet_replies (bool, optional): Set to True if want to get the tweets replies as well. Defaults to False.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Only applicable if with with_tweet_replies is True. Defaults to None.
             total (int, optional): Total(Max) number of results you want to get. If None, extracts all results. Defaults to None.
+            pagination (bool, optional): Set to False if want to handle each page request manually. Use end_cursor from the previous page/request to navigate to the next page. Defaults to True.
 
         Returns:
             dict: Tweet data.
         """
         if end_cursor is not None and not with_tweet_replies:
-            raise Exception(
-                "Either set with_tweet_replies to True or end_cursor to None.")
+            logger.exception("Either set with_tweet_replies to True or end_cursor to None.")
+            raise
         referer = 'tweet' if with_tweet_replies else random.choice(
             ['profile', 'home'])
         variables = {"focalTweetId": tweet_id, "referrer": referer, "with_rux_injections": False, "includePromotedContent": True,
                      "withCommunity": True, "withQuickPromoteEligibilityTweetFields": True, "withArticleRichContent": False, "withBirdwatchNotes": False,
                      "withVoice": True, "withV2Timeline": True}
         variables = variables if self.logged_in() else {
             "tweetId": tweet_id, "withCommunity": False, "includePromotedContent": False, "withVoice": False}
@@ -375,144 +387,151 @@
             request_payload['url'] = request_payload.get('url').replace(
                 Path.TWEET_DETAILS_ENDPOINT, Path.TWEET_DETAILS_BY_ID)
         if with_tweet_replies:
             if not self.logged_in():
                 self.login()
             data_path = (
                 'data', 'threaded_conversation_with_injections_v2', 'instructions')
-            return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total)
+            return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total, pagination=pagination)
         return make_request(**request_payload)
 
     @login_decorator
-    def get_liked_tweets(self, user_id, end_cursor=None, total=None):
+    def get_liked_tweets(self, user_id, end_cursor=None, total=None, pagination=True):
         """Get Tweets liked by a user.
 
         Args:
             user_id (int): User ID.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
             total (int, optional): Total(Max) number of results you want to get. If None, extracts all results. Defaults to None.
+            pagination (bool, optional): Set to False if want to handle each page request manually. Use end_cursor from the previous page/request to navigate to the next page. Defaults to True.
 
         Returns:
             dict: Returns data, cursor_endpoint, has_next_page
         """
         user_id = self.get_user_id(user_id)
         variables = {"userId": user_id, "count": 100, "includePromotedContent": False,
                      "withClientEventToken": False, "withBirdwatchNotes": False, "withVoice": True, "withV2Timeline": True}
         request_payload = self._generate_request_data(
             Path.LIKED_TWEETS_ENDPOINT, variables, additional_features=True)
         data_path = ('data', 'user', 'result', 'timeline_v2',
                      'timeline', 'instructions')
-        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total)
+        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total, pagination=pagination)
 
     @login_decorator
-    def get_user_timeline(self, end_cursor=None, total=None):
+    def get_user_timeline(self, end_cursor=None, total=None, pagination=True):
         """Get tweets from home timeline (Home Page).
 
         Args:
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
             total (int, optional): Total(Max) number of results you want to get. If None, extracts all results. Defaults to None.
+            pagination (bool, optional): Set to False if want to handle each page request manually. Use end_cursor from the previous page/request to navigate to the next page. Defaults to True.
 
         Returns:
             dict: Returns data, cursor_endpoint, has_next_page
         """
         variables = {"count": 40, "includePromotedContent": True,
                      "latestControlAvailable": True, "withCommunity": True}
         request_payload = self._generate_request_data(
             Path.HOME_TIMELINE_ENDPOINT, variables, additional_features=True)
         data_path = ('data', 'home', 'home_timeline_urt', 'instructions')
-        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total)
+        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total, pagination=pagination)
 
     @login_decorator
-    def get_list_tweets(self, list_id, end_cursor=None, total=None):
+    def get_list_tweets(self, list_id, end_cursor=None, total=None, pagination=True):
         """Get tweets from a Tweets List.
 
         Args:
             list_id (str/int): Tweets List ID. (Can be extracted from twitter mobile app.)
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
             total (int, optional): Total(Max) number of results you want to get. If None, extracts all results. Defaults to None.
+            pagination (bool, optional): Set to False if want to handle each page request manually. Use end_cursor from the previous page/request to navigate to the next page. Defaults to True.
 
         Returns:
             dict: Returns data, cursor_endpoint, has_next_page
         """
         variables = {"listId": str(list_id), "count": 100}
         request_payload = self._generate_request_data(
             Path.TWEETS_LIST_ENDPOINT, variables, additional_features=True)
         data_path = ('data', 'list', 'tweets_timeline',
                      'timeline', 'instructions')
-        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total)
+        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total, pagination=pagination)
 
     @login_decorator
-    def get_topic_tweets(self, topic_id, end_cursor=None, total=None):
+    def get_topic_tweets(self, topic_id, end_cursor=None, total=None, pagination=True):
         """Get tweets from a Topic.
 
         Args:
             topic_id (str/int): Topic ID.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
             total (int, optional): Total(Max) number of results you want to get. If None, extracts all results. Defaults to None.
+            pagination (bool, optional): Set to False if want to handle each page request manually. Use end_cursor from the previous page/request to navigate to the next page. Defaults to True.
 
         Returns:
             dict: Returns data, cursor_endpoint, has_next_page
         """
         variables = {"rest_id": topic_id, "count": 100}
         request_payload = self._generate_request_data(
             Path.TOPIC_TWEETS_ENDPOINT, variables, additional_features=True)
         data_path = ('data', 'topic_by_rest_id', 'topic_page',
                      'body', 'timeline', 'instructions')
-        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total)
+        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total, pagination=pagination)
 
     @login_decorator
-    def search(self, search_query, end_cursor=None, total=None, search_filter=None):
+    def search(self, search_query, end_cursor=None, total=None, search_filter=None, pagination=True):
         """Get search results.
 
         Args:
             search_query (str): Search term.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
             total (int, optional): Total(Max) Number of results you want to get. If None, extracts all results. Defaults to None.
             search_filter (str, optional): Type of search you want to perform. Available filters - Latest , Top , People , Photos , Videos. Defaults to 'Top'.
+            pagination (bool, optional): Set to False if want to handle each page request manually. Use end_cursor from the previous page/request to navigate to the next page. Defaults to True.
 
         Returns:
             dict: Returns data, cursor_endpoint, has_next_page
         """
+        # typed_query, hashtag_click, trend_click, recent_search_click, typeahead_click
         search_filter = "Top" if search_filter is None else search_filter
         # Latest , Top , People , Photos , Videos (Product) - Filter
         variables = {"rawQuery": search_query, "count": 20,
-                     "querySource": "hashtag_click", "product": search_filter}
+                     "querySource": "typed_query", "product": search_filter}
         request_payload = self._generate_request_data(
             Path.SEARCH_ENDPOINT, variables, additional_features=True)
         data_path = ('data', 'search_by_raw_query',
                      'search_timeline', 'timeline', 'instructions')
-        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total)
+        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total, pagination=pagination)
 
     @login_decorator
-    def get_friends(self, user_id, follower=False, following=False, mutual_follower=False, end_cursor=None, total=None):
+    def get_friends(self, user_id, follower=False, following=False, mutual_follower=False, end_cursor=None, total=None, pagination=True):
         """Get User's follower, followings or mutual followers.
 
         Args:
             user_id (int): User ID.
             follower (bool, optional): Set to True if want to extract User's follower. Defaults to False.
             following (bool, optional): Set to True if want to extract User's following. Defaults to False.
             mutual_followers (bool, optional): Set to True if want to extract mutual follower. Defaults to False.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
             total (int, optional): Total(Max) number of results you want to get. If None, extracts all results. Defaults to None.
+            pagination (bool, optional): Set to False if want to handle each page request manually. Use end_cursor from the previous page/request to navigate to the next page. Defaults to True.
 
         Returns:
             dict: Returns data, cursor_endpoint, has_next_page
         """
         if (not follower and not following and not mutual_follower) or (follower and following and mutual_follower):
-            raise Exception(
-                "Set one of the (follower,following,mutual_follower) to True.")
+            logger.exception("Set one of the (follower,following,mutual_follower) to True.")
+            raise
         user_id = self.get_user_id(user_id)
         query_path = Path.FOLLOWERS_ENDPOINT if follower else Path.FOLLOWINGS_ENDPOINT if following else Path.MUTUAL_FOLLOWERS_ENDPOINT if mutual_follower else None
         variables = {"userId": user_id, "count": 100,
                      "includePromotedContent": False}
         request_payload = self._generate_request_data(
             query_path, variables, additional_features=True)
         data_path = ('data', 'user', 'result', 'timeline',
                      'timeline', 'instructions')
-        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total)
+        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total, pagination=pagination)
 
     @login_decorator
     def get_profile_business_category(self, user_id):
         """Extracts profile category of a Professional/Business twitter profile. Can also be extracted from get_user_info and get_user_data methods.
 
         Args:
             user_id (int): User ID.
@@ -524,47 +543,69 @@
         variables = {"rest_id": user_id}
         request_payload = self._generate_request_data(
             Path.PROFILE_CATEGORY_ENDPOINT, variables)
         response = make_request(**request_payload)
         return response
 
     @login_decorator
-    def get_tweet_likes(self, tweet_id, end_cursor=None, total=None):
+    def get_tweet_likes(self, tweet_id, end_cursor=None, total=None, pagination=True):
         """Returns data about the users who liked the given tweet post.
 
         Args:
             tweet_id (int): Tweet ID.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
             total (int, optional): Total(Max) number of results you want to get. If None, extracts all results. Defaults to None.
+            pagination (bool, optional): Set to False if want to handle each page request manually. Use end_cursor from the previous page/request to navigate to the next page. Defaults to True.
 
         Returns:
             dict: Returns data, cursor_endpoint, has_next_page
         """
         variables = {"tweetId": str(tweet_id), "count": 100,
                      "includePromotedContent": True}
         request_payload = self._generate_request_data(
             Path.TWEET_LIKES_ENDPOINT, variables, additional_features=True)
         data_path = ('data', 'favoriters_timeline', 'timeline', 'instructions')
-        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total)
+        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total, pagination=pagination)
 
     @login_decorator
-    def get_retweeters(self, tweet_id, end_cursor=None, total=None):
+    def get_retweeters(self, tweet_id, end_cursor=None, total=None, pagination=True):
         """Returs data about the users who retweeted the given tweet post.
 
         Args:
             tweet_id (int): Tweet ID.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
             total (int, optional): Total(Max) number of results you want to get. If None, extracts all results. Defaults to None.
+            pagination (bool, optional): Set to False if want to handle each page request manually. Use end_cursor from the previous page/request to navigate to the next page. Defaults to True.
 
         Returns:
             dict: Returns data, cursor_endpoint, has_next_page
         """
         variables = {"tweetId": str(tweet_id), "count": 100,
                      "includePromotedContent": True}
         request_payload = self._generate_request_data(
             Path.RETWEETED_BY_ENDPOINT, variables, additional_features=True)
         data_path = ('data', 'retweeters_timeline', 'timeline', 'instructions')
-        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total)
+        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total, pagination=pagination)
+    
+    def get_user_highlights(self, user_id, end_cursor=None, total=None, pagination=True):
+        """Get highlights from a user's profile.
+
+        Args:
+            user_id (int): User ID.
+            end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
+            total (int, optional): Total(Max) number of results you want to get. If None, extracts all results. Defaults to None.
+            pagination (bool, optional): Set to False if want to handle each page request manually. Use end_cursor from the previous page/request to navigate to the next page. Defaults to True.
+
+        Returns:
+            dict: Returns data, cursor_endpoint, has_next_page
+        """
+        user_id = self.get_user_id(user_id)
+        variables = {"userId": user_id, "count": 100,
+                     "includePromotedContent": True, "withVoice": True}
+        request_payload = self._generate_request_data(
+            Path.USER_HIGHLIGHTS_ENDPOINT, variables, additional_features=True)
+        data_path = ('data', 'user', 'result', 'timeline', 'timeline', 'instructions')
+        return self._handle_pagination(**request_payload, end_cursor=end_cursor, data_path=data_path, total=total, pagination=pagination)
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `tweeterpy-1.0.9/tweeterpy/util.py` & `tweeterpy-1.1.0/tweeterpy/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import re
 import datetime
 import time
+import bs4
 import logging.config
 from functools import reduce
 from urllib.parse import urljoin
 from typing import Dict, List
 from .constants import Path, PUBLIC_TOKEN
 from . import config
 from dataclasses import dataclass, field, fields, asdict, _MISSING_TYPE
@@ -22,78 +24,109 @@
 class RateLimitError(Exception):
     def __init__(self, message=None):
         if message is None:
             message = "API rate limit exhausted."
         super().__init__(message)
 
 
-def generate_headers(session=None):
+def generate_headers(session=None, custom_headers=None):
     headers = {"Authority": Path.DOMAIN,
                "Accept-Encoding": "gzip, deflate, br",
                "Accept-Language": "en-US,en;q=0.9",
-               "Authorization": PUBLIC_TOKEN,
                "Cache-Control": "no-cache",
                "Referer": Path.BASE_URL,
                "User-Agent": config._USER_AGENT,
                "X-Twitter-Active-User": "yes",
                "X-Twitter-Client-Language": "en"
                }
+    if custom_headers and isinstance(custom_headers, dict):
+        headers.update(custom_headers)
     if session:
+        headers.update({"Authorization": PUBLIC_TOKEN})
+        headers.update(dict(session.headers))
         if "auth_token" in session.cookies.keys():
             session.get(Path.BASE_URL)
             csrf_token = session.cookies.get("ct0", None)
-            auth_headers = {"X-Csrf-Token": csrf_token,
-                            "X-Twitter-Auth-Type": "OAuth2Session"}
-            session.headers.update(auth_headers)
-            headers.update(auth_headers)
+            headers.update({"X-Csrf-Token": csrf_token,
+                            "X-Twitter-Auth-Type": "OAuth2Session"})
+        session.headers.update(headers)
     return headers
 
 
 def generate_features(default_features=True, user_data_features=False, user_info_feautres=False, additional_features=False):
     features = {}
     if default_features:
         default_features = {"responsive_web_graphql_exclude_directive_enabled": True, "verified_phone_label_enabled": True,
                             "responsive_web_graphql_skip_user_profile_image_extensions_enabled": False,
                             "responsive_web_graphql_timeline_navigation_enabled": True}
         features.update(default_features)
 
     if user_data_features or user_info_feautres:
-        features.update({"hidden_profile_likes_enabled": False, "highlights_tweets_tab_ui_enabled": True,
-                         "creator_subscriptions_tweet_preview_api_enabled": True})
+        features.update({"hidden_profile_likes_enabled": False, "hidden_profile_subscriptions_enabled":True, "highlights_tweets_tab_ui_enabled": True,
+                         "responsive_web_twitter_article_notes_tab_enabled":False, "creator_subscriptions_tweet_preview_api_enabled": True})
         if user_info_feautres:
             features.update(
-                {"subscriptions_verification_info_verified_since_enabled": True})
+                {"subscriptions_verification_info_is_identity_verified_enabled":True, "subscriptions_verification_info_verified_since_enabled": True})
 
     if additional_features:
-        features.update({"rweb_lists_timeline_redesign_enabled": True, "creator_subscriptions_tweet_preview_api_enabled": True, "tweetypie_unmention_optimization_enabled": True,
+        features.update({"rweb_lists_timeline_redesign_enabled": True, "creator_subscriptions_tweet_preview_api_enabled": True, "c9s_tweet_anatomy_moderator_badge_enabled":True,"tweetypie_unmention_optimization_enabled": True,
                          "responsive_web_edit_tweet_api_enabled": True, "graphql_is_translatable_rweb_tweet_is_translatable_enabled": True, "view_counts_everywhere_api_enabled": True,
                          "longform_notetweets_consumption_enabled": True, "responsive_web_twitter_article_tweet_consumption_enabled": False, "tweet_awards_web_tipping_enabled": False,
-                         "freedom_of_speech_not_reach_fetch_enabled": True, "standardized_nudges_misinfo": True, "tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled": False,
-                         "longform_notetweets_rich_text_read_enabled": True, "longform_notetweets_inline_media_enabled": False, "responsive_web_enhance_cards_enabled": False})
+                         "freedom_of_speech_not_reach_fetch_enabled": True, "standardized_nudges_misinfo": True, "tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled": False, "rweb_video_timestamps_enabled":True,
+                         "longform_notetweets_rich_text_read_enabled": True, "longform_notetweets_inline_media_enabled": False, "responsive_web_media_download_video_enabled": False, "responsive_web_enhance_cards_enabled": False})
 
     return features
 
 
 def generate_url(domain=None, url_path=None):
     if not domain and not url_path:
         raise TypeError("URL Path cannot be of NoneType.")
     if not domain:
         domain = Path.API_URL
     return urljoin(domain, url_path)
 
+def find_guest_token(page_source):
+    guest_token_regex = re.compile(r"""gt=(\d+);""",re.VERBOSE)
+    try:
+        guest_token_match = re.search(guest_token_regex,str(page_source))
+        if not guest_token_match:
+            raise Exception("Couldn't find guest token")
+        guest_token = guest_token_match.group(1)
+        return guest_token
+    except Exception as error:
+        logger.error(error)
+        raise
+
+def handle_x_migration(session):
+    home_page = None
+    try:
+        response = session.request(method="GET", url=Path.BASE_URL)
+        home_page = bs4.BeautifulSoup(response.content, 'lxml')
+        migration_form = home_page.select_one("form[name='f']") or home_page.select_one(f"form[action='{Path.X_MIGRATE_URL}']")
+        if migration_form:
+            url = migration_form.attrs.get("action", Path.X_MIGRATE_URL)
+            method = migration_form.attrs.get("method", "POST")
+            request_payload = {input_field.get("name"):input_field.get("value") for input_field in migration_form.select("input")}
+            response = session.request(method=method, url=url, data=request_payload)
+            home_page = bs4.BeautifulSoup(response.content, 'lxml')
+    except Exception as error:
+        logger.error(error)
+    finally:
+        generate_headers(session=session)
+        return home_page
 
 def check_for_errors(response):
     if isinstance(response, dict) and "errors" in response.keys():
-        if "data" not in response.keys():
+        if not response.get("data"):
             error_message = "\n".join([error['message']
                                        for error in response['errors']])
             raise Exception(error_message)
-    if "data" in response.keys():
-        if not response.get("data"):
-            raise Exception("Couldn't fetch data.")
+    # if "data" in response.keys():
+    #     if not response.get("data"):
+    #         raise Exception("Couldn't fetch data.")
     # return response['flow_token'] # For manual Way - login_util
     return response
 
 
 def check_api_rate_limits(response):
     # fmt:off - Code fomatting turned off
     try:
@@ -167,15 +200,15 @@
             complex_keys (dict, optional): Multi-level nested keys. Its better to specify the exact path as there can be duplicates as well. Defaults to None.
         """
         # fmt:off
         if self._dataset and isinstance(self._dataset, dict):
             legacy_dataset = find_nested_key(self._dataset,legacy_path) if legacy_path else None
             original_dataset = find_nested_key(self._dataset,dataset_path) if dataset_path else self._dataset
             for dataset in [legacy_dataset,original_dataset]:
-                if dataset is None:
+                if dataset is None or not isinstance(dataset,dict):
                     continue
                 if complex_keys and isinstance(complex_keys,dict):
                     for item_key, path in complex_keys.items():
                         setattr(self, item_key, find_nested_key(dataset, path)) if not getattr(self, item_key) else ''
                 for field in fields(self):
                     if field.name in complex_keys.keys():
                         continue
@@ -233,19 +266,22 @@
     verification_info: dict = None
     verified: bool = None
     verified_phone_status: bool = None
     verified_type: str = None
     withheld_in_countries: List[str] = field(default_factory=list)
 
     def __post_init__(self):
+        user_result = find_nested_key(self._dataset, ("user_results", "result"))
+        self._dataset = user_result or self._dataset
         custom_keys = {"urls": ("entities", "url", "urls"),
                        "description_urls": ("entities", "description", "urls")}
         self.load_data(direct_keys=['id', 'rest_id', 'description', 'url'],
                        legacy_path="legacy", complex_keys=custom_keys)
-        setattr(self, "profile_url", f"{Path.BASE_URL}{self.screen_name}")
+        profile_url = f"{Path.BASE_URL}{self.screen_name}" if self.screen_name else None
+        setattr(self, "profile_url", profile_url)
 
 
 @dataclass
 class Tweet(_Item):
     bookmark_count: int = None
     bookmarked: bool = None
     conversation_id_str: str = None
@@ -274,19 +310,21 @@
     source: str = None
     tweet_url: str = None
     user_id_str: str = None
     user_mentions: List[Dict] = field(default_factory=list)
     views: dict = field(default_factory=dict)
 
     def __post_init__(self):
-        custom_keys = {"screen_name": ("user_results", "result", "legacy", "screen_name"), "name": (
-            "user_results", "result", "legacy", "name")}
-        self.load_data(direct_keys=['id_str', 'rest_id', 'source', 'is_translatable', 'possibly_sensitive', 'views'],
-                       legacy_path=("tweet_results", "result", "legacy"), dataset_path=("tweet_results", "result"),
-                       complex_keys=custom_keys)
+        is_status = find_nested_key(self._dataset, ("tweetResult", "result"))
+        legacy_path = ("tweetResult" if is_status else "tweet_results", "result", "legacy")
+        dataset_path = ("tweetResult" if is_status else "tweet_results", "result")
+        custom_keys = {"screen_name": ("core", "user_results", "result", "legacy", "screen_name"), "name": (
+            "core", "user_results", "result", "legacy", "name")}
+        self.load_data(direct_keys=['id_str', 'rest_id', 'source', 'is_translatable', 'possibly_sensitive', 'views', 'created_at'],
+                       legacy_path=legacy_path, dataset_path=dataset_path, complex_keys=custom_keys)
         setattr(self, "tweet_url",
                 f"{Path.BASE_URL}{self.screen_name}/status/{self.rest_id}")
         setattr(self, "original_tweet",
                 f"{Path.BASE_URL}{self.in_reply_to_screen_name}/status/{self.in_reply_to_status_id_str}") if self.in_reply_to_screen_name else ''
 
 
 if __name__ == "__main__":
```

### Comparing `tweeterpy-1.0.9/tweeterpy.egg-info/PKG-INFO` & `tweeterpy-1.1.0/tweeterpy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 1.0.9
+Version: 1.1.0
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 Home-page: https://github.com/iSarabjitDhiman/TweeterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
@@ -15,14 +15,26 @@
 Classifier: Operating System :: Unix
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: beautifulsoup4==4.12.2
+Requires-Dist: Brotli==1.0.9
+Requires-Dist: bs4==0.0.1
+Requires-Dist: certifi==2023.7.22
+Requires-Dist: charset-normalizer==3.1.0
+Requires-Dist: demjson3==3.0.6
+Requires-Dist: idna==3.7
+Requires-Dist: lxml==4.9.2
+Requires-Dist: requests==2.31.0
+Requires-Dist: six==1.16.0
+Requires-Dist: soupsieve==2.4.1
+Requires-Dist: urllib3==2.0.7
 
 <h1 align="center">TweeterPy</h1>
 
 <p align="center">
 <a href="https://choosealicense.com/licenses/mit/"> <img src="https://img.shields.io/badge/License-MIT-green.svg"></a>
 <a href="https://www.python.org/"><img src="https://img.shields.io/pypi/pyversions/tweeterpy"></a>
 <a href="https://pypi.org/project/tweeterpy/"> <img src="https://img.shields.io/pypi/v/tweeterpy"></a>
```

#### html2text {}

```diff
@@ -1,21 +1,26 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 1.0.9 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 1.1.0 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
 TweeterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
 License: MIT Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix Classifier: License :: OSI Approved :: MIT
 License Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3 Description-Content-
-Type: text/markdown License-File: LICENSE
+Type: text/markdown License-File: LICENSE Requires-Dist: beautifulsoup4==4.12.2
+Requires-Dist: Brotli==1.0.9 Requires-Dist: bs4==0.0.1 Requires-Dist:
+certifi==2023.7.22 Requires-Dist: charset-normalizer==3.1.0 Requires-Dist:
+demjson3==3.0.6 Requires-Dist: idna==3.7 Requires-Dist: lxml==4.9.2 Requires-
+Dist: requests==2.31.0 Requires-Dist: six==1.16.0 Requires-Dist:
+soupsieve==2.4.1 Requires-Dist: urllib3==2.0.7
                             ************ TTwweeeetteerrPPyy ************
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_g_r_e_e_n_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
  _p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_t_w_e_e_t_e_r_p_y_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_t_w_e_e_t_e_r_p_y_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_a_s_t_-_c_o_m_m_i_t_/_i_S_a_r_a_b_j_i_t_D_h_i_m_a_n_/_T_w_e_e_t_e_r_P_y_]_[_D_i_s_c_o_r_d_]_[_h_t_t_p_s_:_/_/
     _i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/_f_o_l_l_o_w_/_i_S_a_r_a_b_j_i_t_D_h_i_m_a_n_?_s_t_y_l_e_=_s_o_c_i_a_l_]## Overview
 TweeterPy is a python library to extract data from Twitter. TweeterPy API lets
  you scrape data from a user's profile like username, userid, bio, followers/
```

