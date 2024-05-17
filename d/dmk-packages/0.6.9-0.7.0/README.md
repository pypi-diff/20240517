# Comparing `tmp/dmk_packages-0.6.9.tar.gz` & `tmp/dmk_packages-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmk_packages-0.6.9.tar", last modified: Sun May  5 04:27:50 2024, max compression
+gzip compressed data, was "dmk_packages-0.7.0.tar", last modified: Fri May 17 00:39:33 2024, max compression
```

## Comparing `dmk_packages-0.6.9.tar` & `dmk_packages-0.7.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-05 04:27:50.791354 dmk_packages-0.6.9/
--rw-r--r--   0 layla      (501) staff       (20)    11347 2024-03-25 06:00:17.000000 dmk_packages-0.6.9/LICENSE
--rw-r--r--   0 layla      (501) staff       (20)     1854 2024-05-05 04:27:50.790473 dmk_packages-0.6.9/PKG-INFO
--rw-r--r--   0 layla      (501) staff       (20)     1365 2024-03-25 06:00:17.000000 dmk_packages-0.6.9/README.md
--rw-r--r--   0 layla      (501) staff       (20)      584 2024-05-05 04:26:40.000000 dmk_packages-0.6.9/pyproject.toml
--rw-r--r--   0 layla      (501) staff       (20)       38 2024-05-05 04:27:50.791592 dmk_packages-0.6.9/setup.cfg
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-05 04:27:50.771828 dmk_packages-0.6.9/src/
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-05 04:27:50.774927 dmk_packages-0.6.9/src/dmk_packages/
--rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.6.9/src/dmk_packages/__init__.py
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-05 04:27:50.785877 dmk_packages-0.6.9/src/dmk_packages/crawler/
--rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.6.9/src/dmk_packages/crawler/__init__.py
--rw-r--r--   0 layla      (501) staff       (20)     3534 2024-05-04 15:01:16.000000 dmk_packages-0.6.9/src/dmk_packages/crawler/bigkinds.py
--rw-r--r--   0 layla      (501) staff       (20)     6580 2024-05-04 15:01:16.000000 dmk_packages-0.6.9/src/dmk_packages/crawler/clien.py
--rw-r--r--   0 layla      (501) staff       (20)     6685 2024-05-04 15:01:16.000000 dmk_packages-0.6.9/src/dmk_packages/crawler/fnguide.py
--rw-r--r--   0 layla      (501) staff       (20)     2321 2024-04-03 06:07:52.000000 dmk_packages-0.6.9/src/dmk_packages/crawler/naver_blog.py
--rw-r--r--   0 layla      (501) staff       (20)    15349 2024-04-15 02:00:30.000000 dmk_packages-0.6.9/src/dmk_packages/crawler/naver_search_volume.py
--rw-r--r--   0 layla      (501) staff       (20)     1382 2024-05-04 15:01:16.000000 dmk_packages-0.6.9/src/dmk_packages/crawler/pdf_to_text.py
--rw-r--r--   0 layla      (501) staff       (20)    14699 2024-05-05 04:01:44.000000 dmk_packages-0.6.9/src/dmk_packages/crawler/youtube.py
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-05 04:27:50.788163 dmk_packages-0.6.9/src/dmk_packages/database/
--rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.6.9/src/dmk_packages/database/__init__.py
--rw-r--r--   0 layla      (501) staff       (20)     3057 2024-04-15 03:09:28.000000 dmk_packages-0.6.9/src/dmk_packages/database/database.py
--rw-r--r--   0 layla      (501) staff       (20)     1895 2024-03-25 06:00:17.000000 dmk_packages-0.6.9/src/dmk_packages/naver_datalab.py
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-05 04:27:50.789484 dmk_packages-0.6.9/src/dmk_packages.egg-info/
--rw-r--r--   0 layla      (501) staff       (20)     1854 2024-05-05 04:27:50.000000 dmk_packages-0.6.9/src/dmk_packages.egg-info/PKG-INFO
--rw-r--r--   0 layla      (501) staff       (20)      677 2024-05-05 04:27:50.000000 dmk_packages-0.6.9/src/dmk_packages.egg-info/SOURCES.txt
--rw-r--r--   0 layla      (501) staff       (20)        1 2024-05-05 04:27:50.000000 dmk_packages-0.6.9/src/dmk_packages.egg-info/dependency_links.txt
--rw-r--r--   0 layla      (501) staff       (20)       41 2024-05-05 04:27:50.000000 dmk_packages-0.6.9/src/dmk_packages.egg-info/requires.txt
--rw-r--r--   0 layla      (501) staff       (20)       13 2024-05-05 04:27:50.000000 dmk_packages-0.6.9/src/dmk_packages.egg-info/top_level.txt
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-17 00:39:33.187007 dmk_packages-0.7.0/
+-rw-r--r--   0 layla      (501) staff       (20)    11347 2024-03-25 06:00:17.000000 dmk_packages-0.7.0/LICENSE
+-rw-r--r--   0 layla      (501) staff       (20)     1854 2024-05-17 00:39:33.186645 dmk_packages-0.7.0/PKG-INFO
+-rw-r--r--   0 layla      (501) staff       (20)     1365 2024-03-25 06:00:17.000000 dmk_packages-0.7.0/README.md
+-rw-r--r--   0 layla      (501) staff       (20)      584 2024-05-17 00:39:18.000000 dmk_packages-0.7.0/pyproject.toml
+-rw-r--r--   0 layla      (501) staff       (20)       38 2024-05-17 00:39:33.187101 dmk_packages-0.7.0/setup.cfg
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-17 00:39:33.171489 dmk_packages-0.7.0/src/
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-17 00:39:33.174862 dmk_packages-0.7.0/src/dmk_packages/
+-rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.7.0/src/dmk_packages/__init__.py
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-17 00:39:33.183630 dmk_packages-0.7.0/src/dmk_packages/crawler/
+-rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.7.0/src/dmk_packages/crawler/__init__.py
+-rw-r--r--   0 layla      (501) staff       (20)     3534 2024-05-04 15:01:16.000000 dmk_packages-0.7.0/src/dmk_packages/crawler/bigkinds.py
+-rw-r--r--   0 layla      (501) staff       (20)     6580 2024-05-04 15:01:16.000000 dmk_packages-0.7.0/src/dmk_packages/crawler/clien.py
+-rw-r--r--   0 layla      (501) staff       (20)     6685 2024-05-04 15:01:16.000000 dmk_packages-0.7.0/src/dmk_packages/crawler/fnguide.py
+-rw-r--r--   0 layla      (501) staff       (20)     2321 2024-04-03 06:07:52.000000 dmk_packages-0.7.0/src/dmk_packages/crawler/naver_blog.py
+-rw-r--r--   0 layla      (501) staff       (20)    17245 2024-05-17 00:38:35.000000 dmk_packages-0.7.0/src/dmk_packages/crawler/naver_search_volume.py
+-rw-r--r--   0 layla      (501) staff       (20)     1382 2024-05-04 15:01:16.000000 dmk_packages-0.7.0/src/dmk_packages/crawler/pdf_to_text.py
+-rw-r--r--   0 layla      (501) staff       (20)    14699 2024-05-05 04:51:03.000000 dmk_packages-0.7.0/src/dmk_packages/crawler/youtube.py
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-17 00:39:33.184891 dmk_packages-0.7.0/src/dmk_packages/database/
+-rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.7.0/src/dmk_packages/database/__init__.py
+-rw-r--r--   0 layla      (501) staff       (20)     3057 2024-04-15 03:09:28.000000 dmk_packages-0.7.0/src/dmk_packages/database/database.py
+-rw-r--r--   0 layla      (501) staff       (20)     1895 2024-03-25 06:00:17.000000 dmk_packages-0.7.0/src/dmk_packages/naver_datalab.py
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-17 00:39:33.185993 dmk_packages-0.7.0/src/dmk_packages.egg-info/
+-rw-r--r--   0 layla      (501) staff       (20)     1854 2024-05-17 00:39:33.000000 dmk_packages-0.7.0/src/dmk_packages.egg-info/PKG-INFO
+-rw-r--r--   0 layla      (501) staff       (20)      677 2024-05-17 00:39:33.000000 dmk_packages-0.7.0/src/dmk_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 layla      (501) staff       (20)        1 2024-05-17 00:39:33.000000 dmk_packages-0.7.0/src/dmk_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 layla      (501) staff       (20)       41 2024-05-17 00:39:33.000000 dmk_packages-0.7.0/src/dmk_packages.egg-info/requires.txt
+-rw-r--r--   0 layla      (501) staff       (20)       13 2024-05-17 00:39:33.000000 dmk_packages-0.7.0/src/dmk_packages.egg-info/top_level.txt
```

### Comparing `dmk_packages-0.6.9/LICENSE` & `dmk_packages-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.9/PKG-INFO` & `dmk_packages-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.6.9
+Version: 0.7.0
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dmk_packages-0.6.9/README.md` & `dmk_packages-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.9/pyproject.toml` & `dmk_packages-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmk_packages"
-version = "0.6.9"
+version = "0.7.0"
 authors = [{ name = "DataMarketingKorea", email = "infra@datamarketing.co.kr" }]
 description = "Common packages for DataMKTKorea"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = ["SQLAlchemy", "python-dotenv", "psycopg2-binary"]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `dmk_packages-0.6.9/src/dmk_packages/crawler/bigkinds.py` & `dmk_packages-0.7.0/src/dmk_packages/crawler/bigkinds.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.9/src/dmk_packages/crawler/clien.py` & `dmk_packages-0.7.0/src/dmk_packages/crawler/clien.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.9/src/dmk_packages/crawler/fnguide.py` & `dmk_packages-0.7.0/src/dmk_packages/crawler/fnguide.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.9/src/dmk_packages/crawler/naver_blog.py` & `dmk_packages-0.7.0/src/dmk_packages/crawler/naver_blog.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.9/src/dmk_packages/crawler/naver_search_volume.py` & `dmk_packages-0.7.0/src/dmk_packages/crawler/naver_search_volume.py`

 * *Files 14% similar despite different names*

```diff
@@ -256,42 +256,25 @@
                     if target_keyword_hits == len(keywords_bundle):
                         break
             return searchad_data
         except Exception as error:
             raise Exception(error)
 
     def get_datalab_data(
-        self, keywords_bundle: List[str], start_dt, end_dt
+        self, keywords_bundle: List[str], start_dt, end_dt, age_gender=False
     ) -> List[DatalabResult]:
         """
         네이버 데이터랩 API 데이터 가져오기
 
         API 문서: https://developers.naver.com/docs/serviceapi/datalab/search/search.md#python
         """
-        try:
-            if len(keywords_bundle) > 5:
-                raise ValueError("keywords_bundle 리스트는 최대 5개까지만 허용됩니다.")
 
-            datalab_data = []
-
-            headers = {
-                "X-Naver-Client-Id": self._datalab_key.get("client_id"),
-                "X-Naver-Client-Secret": self._datalab_key.get("client_secret"),
-                "Content-Type": "application/json",
-            }
-            body = {
-                "startDate": start_dt,
-                "endDate": end_dt,
-                "timeUnit": "date",
-                "keywordGroups": [
-                    {"groupName": k, "keywords": [k]} for k in keywords_bundle
-                ],
-            }
+        def __add_results_to_datalab_data(p_headers, p_body, p_datalab_data, p_age_gender=False):
             response = requests.post(
-                url=self.DATALAB_URL, headers=headers, data=json.dumps(body)
+                url=self.DATALAB_URL, headers=p_headers, data=json.dumps(p_body)
             )
 
             if not response.ok:
                 self._datalab_key = self._get_datalab_key()
 
                 if response.status_code == 401:
                     # ============================================================
@@ -303,77 +286,134 @@
                     #  NOTE: 데이터랩 호출 한도 초과시 업데이트
                     self._update_datalab_key(self._datalab_key["key_id"], "active")
                     # ============================================================
 
                 return self.get_datalab_data(keywords_bundle, start_dt, end_dt)
 
             results = response.json().get("results")
-
             for result in results:
                 keyword = result.get("title", "")
                 data = result.get("data", [])
+                if p_age_gender:
+                    data = [d.update({"gender": gender, "age": age}) or d for d in data]
 
                 temp_data = data.copy()
                 existing_dates = {d["period"] for d in data}
 
                 start_date = pendulum.from_format(start_dt, "YYYY-MM-DD")
                 end_date = pendulum.from_format(end_dt, "YYYY-MM-DD")
 
                 current_date = start_date
                 while current_date <= end_date:
                     current_date_str = current_date.strftime("%Y-%m-%d")
                     if current_date_str not in existing_dates:
-                        temp_data.append({"period": current_date_str, "ratio": 0.0})
+                        if p_age_gender:
+                            temp_data.append({
+                                "period": current_date_str, "ratio": 0.0, "gender": gender, "age": age
+                            })
+                        else:
+                            temp_data.append({"period": current_date_str, "ratio": 0.0})
                     current_date = current_date.add(days=1)
 
                 temp_data.sort(key=lambda x: x["period"])
-                datalab_data.append({"keyword": keyword, "data": temp_data})
+                p_datalab_data.append({"keyword": keyword, "data": temp_data})
+
+        try:
+            if len(keywords_bundle) > 5:
+                raise ValueError("keywords_bundle 리스트는 최대 5개까지만 허용됩니다.")
+
+            datalab_data = []
+            headers = {
+                "X-Naver-Client-Id": self._datalab_key.get("client_id"),
+                "X-Naver-Client-Secret": self._datalab_key.get("client_secret"),
+                "Content-Type": "application/json",
+            }
+            body = {
+                "startDate": start_dt,
+                "endDate": end_dt,
+                "timeUnit": "date",
+                "keywordGroups": [
+                    {"groupName": k, "keywords": [k]} for k in keywords_bundle
+                ],
+            }
+
+            if age_gender:
+                ages_category: dict = dict({str(x): [str(x)] for x in range(1, 12)})
+                genders_category: dict = {"남": "m", "여": "f"}
+
+                for age, age_value in ages_category.items():
+                    for gender, gender_value in genders_category.items():
+                        body.update({"gender": gender_value, "ages": age_value})
+                        __add_results_to_datalab_data(headers, body, datalab_data, age_gender)
+            else:
+                __add_results_to_datalab_data(headers, body, datalab_data, age_gender)
             return datalab_data
+
         except Exception as error:
             raise Exception(error)
 
     def calc_search_volume(
         self,
         keywords_bundle,
         searchad_data: List[SearchadResult],
         datalab_data: List[DatalabResult],
+        age_gender=False
     ):
+        def __add_results_to_search_volume(p_data, p_total_volume, p_search_volume, p_age_gender):
+            total_ratio = sum(
+                [d["ratio"] for d in p_data.get("data")]
+            )
+
+            volume_per_ratio = (
+                p_total_volume / total_ratio if total_ratio > 0 else 0
+            )
+
+            for d in p_data.get("data"):
+                if p_age_gender:
+                    new_data = {
+                        "keyword_text": kwd,
+                        "keyword_date": pendulum.parse(d["period"], tz=tz),
+                        "keyword_volume": int(d["ratio"] * volume_per_ratio),
+                        "gender": d["gender"],
+                        "age": d["age"],
+                        "collected_at": pendulum.today(),
+                    }
+                else:
+                    new_data = {
+                        "keyword_text": kwd,
+                        "keyword_date": pendulum.parse(d["period"], tz=tz),
+                        "keyword_volume": int(d["ratio"] * volume_per_ratio),
+                        "collected_at": pendulum.today(),
+                    }
+                p_search_volume.append(new_data)
+
         try:
             search_volume = []
 
             for kwd in keywords_bundle:
                 tgt_searchad_datum = [d for d in searchad_data if d["keyword"] == kwd]
                 tgt_datalab_datum = [d for d in datalab_data if d["keyword"] == kwd]
 
                 if tgt_searchad_datum and tgt_datalab_datum:
                     monthly_pc_volume = tgt_searchad_datum[0].get(self.MPQC)
                     monthly_mo_volume = tgt_searchad_datum[0].get(self.MMQC)
-
                     total_volume = monthly_pc_volume + monthly_mo_volume
-                    total_ratio = sum(
-                        [d["ratio"] for d in tgt_datalab_datum[0].get("data")]
-                    )
 
-                    volume_per_ratio = (
-                        total_volume / total_ratio if total_ratio > 0 else 0
-                    )
+                    if age_gender:
+                        for datum in tgt_datalab_datum:
+                            __add_results_to_search_volume(datum, total_volume, search_volume, age_gender)
+                    else:
+                        __add_results_to_search_volume(tgt_datalab_datum[0], total_volume, search_volume, age_gender)
 
-                    for d in tgt_datalab_datum[0].get("data"):
-                        new_data = {
-                            "keyword_text": kwd,
-                            "keyword_date": pendulum.parse(d["period"], tz=tz),
-                            "keyword_volume": int(d["ratio"] * volume_per_ratio),
-                            "collected_at": pendulum.today(),
-                        }
-                        search_volume.append(new_data)
             return search_volume
+
         except Exception as error:
             logger.error(error)
 
-    def get_search_volume(self):
+    def get_search_volume(self, age_gender=False):
         try:
             results = []
 
             if not self._searchad_key or not self._datalab_key:
                 return results
 
             self._set_date_range(target_date=self._date_until)
@@ -383,33 +423,30 @@
 
             for kwds_bundle in self._keywords_bundle:
                 searchad_data = self.get_searchad_data(kwds_bundle)
 
                 for date_range in self._date_range:
                     start_dt, end_dt = [d.strftime("%Y-%m-%d") for d in date_range]
                     logger.info(f"{start_dt} ~ {end_dt} {kwds_bundle}")
-                    datalab_data = self.get_datalab_data(
-                        kwds_bundle,
-                        start_dt,
-                        end_dt,
-                    )
 
+                    datalab_data = self.get_datalab_data(kwds_bundle, start_dt, end_dt, age_gender)
                     search_volume = self.calc_search_volume(
                         kwds_bundle,
                         searchad_data,
                         datalab_data,
+                        age_gender
                     )
                     results.extend(search_volume)
             return results
         except Exception as error:
             logger.error(error)
 
 
-if __name__ == "__main__":
-    try:
-        naver_search_volume_crawler = NaverSearchVolumeCrawler()
-        search_volume = naver_search_volume_crawler.get_search_volume()
-
-        for vol in search_volume:
-            logger.debug(vol)
-    except Exception as error:
-        logger.error(error)
+# if __name__ == "__main__":
+#     try:
+#         naver_search_volume_crawler = NaverSearchVolumeCrawler()
+#         search_volume = naver_search_volume_crawler.get_searchad_data()
+#
+#         for vol in search_volume:
+#             logger.debug(vol)
+#     except Exception as error:
+#         logger.error(error)
```

### Comparing `dmk_packages-0.6.9/src/dmk_packages/crawler/pdf_to_text.py` & `dmk_packages-0.7.0/src/dmk_packages/crawler/pdf_to_text.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.9/src/dmk_packages/crawler/youtube.py` & `dmk_packages-0.7.0/src/dmk_packages/crawler/youtube.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.9/src/dmk_packages/database/database.py` & `dmk_packages-0.7.0/src/dmk_packages/database/database.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.9/src/dmk_packages/naver_datalab.py` & `dmk_packages-0.7.0/src/dmk_packages/naver_datalab.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.9/src/dmk_packages.egg-info/PKG-INFO` & `dmk_packages-0.7.0/src/dmk_packages.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.6.9
+Version: 0.7.0
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dmk_packages-0.6.9/src/dmk_packages.egg-info/SOURCES.txt` & `dmk_packages-0.7.0/src/dmk_packages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

