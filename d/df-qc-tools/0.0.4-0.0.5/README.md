# Comparing `tmp/df_qc_tools-0.0.4.tar.gz` & `tmp/df_qc_tools-0.0.5.tar.gz`

## Comparing `df_qc_tools-0.0.4.tar` & `df_qc_tools-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 df_qc_tools-0.0.4/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 df_qc_tools-0.0.4/__init__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 df_qc_tools-0.0.4/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 df_qc_tools-0.0.4/src/df_qc_tools/__init__.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 df_qc_tools-0.0.4/src/df_qc_tools/config.py
--rw-r--r--   0        0        0    20161 2020-02-02 00:00:00.000000 df_qc_tools-0.0.4/src/df_qc_tools/qc.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 df_qc_tools-0.0.4/tests/test_config.py
--rw-r--r--   0        0        0    29781 2020-02-02 00:00:00.000000 df_qc_tools-0.0.4/tests/test_qc.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 df_qc_tools-0.0.4/tests/conf/conf_base.yaml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 df_qc_tools-0.0.4/tests/resources/data_velocity_acc.csv
--rw-r--r--   0        0        0  1417615 2020-02-02 00:00:00.000000 df_qc_tools-0.0.4/tests/resources/df_outliers.csv
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 df_qc_tools-0.0.4/.gitignore
--rw-r--r--   0        0        0    34475 2020-02-02 00:00:00.000000 df_qc_tools-0.0.4/LICENSE
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 df_qc_tools-0.0.4/README.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 df_qc_tools-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 df_qc_tools-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 df_qc_tools-0.0.5/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 df_qc_tools-0.0.5/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 df_qc_tools-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 df_qc_tools-0.0.5/requirements.txt_old
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 df_qc_tools-0.0.5/src/df_qc_tools/__init__.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 df_qc_tools-0.0.5/src/df_qc_tools/config.py
+-rw-r--r--   0        0        0    21054 2020-02-02 00:00:00.000000 df_qc_tools-0.0.5/src/df_qc_tools/qc.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 df_qc_tools-0.0.5/tests/test_config.py
+-rw-r--r--   0        0        0    31525 2020-02-02 00:00:00.000000 df_qc_tools-0.0.5/tests/test_qc.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 df_qc_tools-0.0.5/tests/conf/conf_base.yaml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 df_qc_tools-0.0.5/tests/resources/data_velocity_acc.csv
+-rw-r--r--   0        0        0  1417615 2020-02-02 00:00:00.000000 df_qc_tools-0.0.5/tests/resources/df_outliers.csv
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 df_qc_tools-0.0.5/.gitignore
+-rw-r--r--   0        0        0    34475 2020-02-02 00:00:00.000000 df_qc_tools-0.0.5/LICENSE
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 df_qc_tools-0.0.5/README.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 df_qc_tools-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 df_qc_tools-0.0.5/PKG-INFO
```

### Comparing `df_qc_tools-0.0.4/src/df_qc_tools/config.py` & `df_qc_tools-0.0.5/src/df_qc_tools/config.py`

 * *Files identical despite different names*

### Comparing `df_qc_tools-0.0.4/src/df_qc_tools/qc.py` & `df_qc_tools-0.0.5/src/df_qc_tools/qc.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,21 @@
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import xarray as xr
 from scipy import stats
 from tqdm import tqdm
 
-from pandassta.df import (Df, QualityFlags, get_acceleration_series, get_distance_geopy_series,
-                         get_velocity_series)
+from pandassta.df import (
+    Df,
+    QualityFlags,
+    get_acceleration_series,
+    get_distance_geopy_series,
+    get_velocity_series,
+)
 from pandassta.df import CAT_TYPE
 from pandassta.logging_constants import TQDM_DESC_FORMAT
 from pandassta.logging_constants import TQDM_BAR_FORMAT
 
 log = logging.getLogger(__name__)
 
 
@@ -38,15 +43,15 @@
     qc_type_max = f"qc_{qc_type}_max"
 
     columns0 = list(df.columns)
     nb_levels = df.columns.nlevels
     for ci in [qc_type_max, qc_type_min]:
         ci_i = ci
         if nb_levels > 1:
-            ci_i =(ci,) + ("",)*(nb_levels-1)
+            ci_i = (ci,) + ("",) * (nb_levels - 1)
         if ci_i not in columns0:
             columns0 += [ci_i]
     df = df.reindex(columns=columns0)
     mask_max_not_null = ~df[qc_type_max].isnull()
     mask_min_not_null = ~df[qc_type_min].isnull()
     s_bool_out = (df.loc[mask_max_not_null, qc_on] > df.loc[mask_max_not_null, qc_type_max]) | (df.loc[mask_min_not_null, qc_on] < df.loc[mask_min_not_null, qc_type_min])  # type: ignore
 
@@ -85,60 +90,89 @@
     log.info(f"Flags set: {df_out.loc[bool_mainland | bool_nan, [Df.QC_FLAG, Df.REGION]].value_counts(dropna=False)}")  # type: ignore
     return df_out
 
 
 # TODO: refactor, complete df is not needed
 def calc_gradient_results(df: pd.DataFrame, groupby: Df) -> pd.DataFrame:
     log.info(f"Start gradient calculations per {groupby}.")
+    df_copy = deepcopy(df)
 
     def grad_function(group):
         nb_row, nb_columns = group.shape
         if nb_row < 2:
             group[Df.GRADIENT] = None
             return group
         g = np.gradient(
             # group.result, group.phenomenonTime.astype("datetime64[s]").astype("int64")
-            group.result, group.phenomenonTime.astype("datetime64[ns]").astype("int64")
+            group.result,
+            group.phenomenonTime.astype("datetime64[ns]").astype("int64"),
         )
-        group[Df.GRADIENT] = g*1e9
+        group[Df.GRADIENT] = g * 1e9
         return group
 
-    df_tmp = df.sort_values(Df.TIME)
-    df_grouped = df.groupby(by=[groupby], group_keys=False)
+    df_tmp = df_copy.sort_values(Df.TIME)
+    df_grouped = df_copy.groupby(by=[groupby], group_keys=False)
     df_tmp = df_grouped[[str(Df.RESULT), str(Df.TIME)]].apply(
         grad_function
     )  # casted to string to avoid type error
-    df_out = df.join(df_tmp[Df.GRADIENT])
+    df_out = df_copy.join(df_tmp[Df.GRADIENT])
     return df_out
 
-    
-def calc_zscore_results(df: pd.DataFrame, groupby: Df, rolling_time_window: str="60min") -> pd.DataFrame:
+
+def calc_zscore_results(
+    df: pd.DataFrame, groupby: Df, rolling_time_window: str = "60min"
+) -> pd.DataFrame:
+    df_copy = deepcopy(df)
     def mod_z(df_: pd.DataFrame) -> pd.Series:
         # transformed, _ = stats.yeojohnson(col.values)
         # col[col.columns[0]] = transformed.ravel()
-        roll = df_.sort_values(Df.TIME).rolling(rolling_time_window, on=Df.TIME, center=True)
+        # df_ = df_.loc[df_.get(Df.QC_FLAG, pd.Series(0, index=df_.index)) <= 2]
+        # try:
+        # df_ = df_.loc[df_[Df.QC_FLAG] <= 2]
+        # except KeyError as e:
+        # pass
+        roll = df_.sort_values(Df.TIME).rolling(
+            rolling_time_window, on=Df.TIME, center=True
+        )
         col = df_[Df.RESULT]
         df_["median"] = roll[Df.RESULT].median()
         df_["abs_dev"] = (df_[Df.RESULT] - df_["median"]).abs()
-        # med_abs_dev = np.median(np.abs(col - med_col)) 
+        # med_abs_dev = np.median(np.abs(col - med_col))
         # med_abs_dev = np.abs(roll[Df.RESULT] - med_col).median() # type: ignore
-        roll = df_.sort_values(Df.TIME).rolling(rolling_time_window, on=Df.TIME, center=True)
+        roll = df_.sort_values(Df.TIME).rolling(
+            rolling_time_window, on=Df.TIME, center=True
+        )
         df_["med_abs_dev"] = roll["abs_dev"].median()
-        mod_z = 0.6745 * ((col - df_["median"]) / df_["med_abs_dev"])
-        mod_z.loc[df_["med_abs_dev"] == 0] = ((col - df_["median"]) / (1.253314*roll["abs_dev"].mean()))
+        # (X-MED)/(1.486*MAD)
+        mod_z = (col-df_["median"])/(1.486*df_["med_abs_dev"])
+        # mod_z = 0.6745 * ((col - df_["median"]) / df_["med_abs_dev"])
+        mod_z.loc[df_["med_abs_dev"] == 0] = (col - df_["median"]) / (
+            1.253314 * roll["abs_dev"].mean()
+        )
         # return np.abs(mod_z)
         return mod_z
+
     def _calc_zscore_results(df, groupby):
-        group = df.groupby(by=groupby, group_keys=False)
+        # group = df.groupby(by=groupby, group_keys=False)
+        # group = df.loc[df.get(Df.QC_FLAG, pd.Series(0, index=df.index).map(QualityFlags)) <= QualityFlags(2)].groupby(
+        df_ = df.loc[:]
+        df_.loc[df_.get(Df.QC_FLAG, pd.Series(0, index=df_.index).map(QualityFlags)) >= QualityFlags.PROBABLY_BAD, Df.RESULT] = pd.NA
+        group = df_.groupby(
+            by=groupby, group_keys=False
+        )
         # group = df[[Df.TIME, Df.RESULT, groupby]].groupby(by=groupby, group_keys=False)
         # z = group[[Df.TIME, Df.RESULT]].rolling(rolling_time_window=Df.TIME, center=True).apply(stats.zscore)
         z = group[[Df.TIME, Df.RESULT]].apply(mod_z)
         # z = group[[Df.RESULT]].apply(stats.zscore)
+        if group.ngroups == 1:
+            return z.T
         return z
-    df[Df.ZSCORE] = _calc_zscore_results(df, groupby=[Df.DATASTREAM_ID])
+
+    df_copy[Df.ZSCORE] = _calc_zscore_results(df_copy, groupby=[Df.DATASTREAM_ID])
+    df[Df.ZSCORE] = df_copy[Df.ZSCORE]
     # roll_median = df.loc[:, [Df.RESULT, Df.DATASTREAM_ID, Df.TIME]].sort_values(Df.TIME).rolling(rolling_time_window, on=Df.TIME, center=True).median()
     # df.loc[:, [Df.RESULT, Df.TIME]].sort_values(Df.TIME)
     # df[Df.ZSCORE]
     # roll_median = roll.median()
     return df
 
 
@@ -362,21 +396,20 @@
     # rolling_time = (
     #     df_time_sorted.loc[:, [Df.TIME, "dt"]]
     #     .sort_values(Df.TIME)
     #     .rolling(time_window, on=Df.TIME, center=True)
     #     .apply(delta)
     # )
     # rolling_time = (rolling_t.max() - rolling_t.min()).dt
-    rolling_t = (
-        df_time_sorted.loc[:, [Df.TIME, "dt"]]
-        .rolling(time_window, on=Df.TIME, center=True)
+    rolling_t = df_time_sorted.loc[:, [Df.TIME, "dt"]].rolling(
+        time_window, on=Df.TIME, center=True
     )
-    rolling_time = (rolling_t.max() - rolling_t.min())
+    rolling_time = rolling_t.max() - rolling_t.min()
 
-    rolling_time[Df.TIME] =  df_time_sorted[Df.TIME]
+    rolling_time[Df.TIME] = df_time_sorted[Df.TIME]
 
     rolling_median = rolling_median.reindex(index=rolling_time.index, fill_value=None)
     rolling_median.loc[entries_excluded_from_calculations, Df.TIME] = rolling_time.loc[
         entries_excluded_from_calculations, Df.TIME
     ]
     rolling_median = rolling_median.ffill().bfill()
 
@@ -519,15 +552,15 @@
                     flag_on_false=self.flag_on_false,
                 ),  # type: ignore
                 self.bool_merge_function,
                 fill_value=self.flag_on_nan,  # type: ignore
             )
         ).astype(CAT_TYPE)
         log.info(f"Execution {self.label} qc result: {self.bool_series.sum()} True")
-        self.series_out = series_out # type: ignore
+        self.series_out = series_out  # type: ignore
         return self.series_out
 
 
 def combine_dicts(a, b, op=operator.add):
     return a | b | dict([(k, op(a[k], b[k])) for k in set(b) & set(a)])
```

### Comparing `df_qc_tools-0.0.4/tests/test_config.py` & `df_qc_tools-0.0.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `df_qc_tools-0.0.4/tests/test_qc.py` & `df_qc_tools-0.0.5/tests/test_qc.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,27 @@
 import pandas as pd
 import pandas.testing as pdt
 import pytest
 from geopy import Point as gp_point
 from pandassta.df import CAT_TYPE, Df, QualityFlags, df_type_conversions
 
 from src.df_qc_tools.qc import (
-    calc_gradient_results, calc_zscore_results, combine_dicts,
-    get_bool_exceed_max_acceleration, get_bool_exceed_max_velocity,
-    get_bool_land_region, get_bool_null_region, get_bool_out_of_range,
-    get_bool_spacial_outlier_compared_to_median, get_qc_flag_from_bool,
-    qc_dependent_quantity_base, qc_dependent_quantity_secondary)
+    calc_gradient_results,
+    calc_zscore_results,
+    combine_dicts,
+    get_bool_exceed_max_acceleration,
+    get_bool_exceed_max_velocity,
+    get_bool_land_region,
+    get_bool_null_region,
+    get_bool_out_of_range,
+    get_bool_spacial_outlier_compared_to_median,
+    get_qc_flag_from_bool,
+    qc_dependent_quantity_base,
+    qc_dependent_quantity_secondary,
+)
 from searegion_detection.queryregion import build_points_query
 
 
 @pytest.fixture
 def df_velocity_acceleration() -> gpd.GeoDataFrame:
     df_t = pd.read_csv("./tests/resources/data_velocity_acc.csv", header=0)
     df_t[Df.TIME] = pd.to_timedelta(df_t["Time (s)"], "s") + pd.Timestamp("now")
@@ -120,15 +128,17 @@
                 map(
                     add,
                     base_results * MULTIPL_FACTOR,
                     [i * 10 for i in datastream_id_series.to_list()],
                 ),  # type: ignore
                 dtype=float,
             ),  # type: ignore
-            Df.OBSERVATION_TYPE: datastream_id_series.apply(lambda x: ds_id_type_dict[x]),
+            Df.OBSERVATION_TYPE: datastream_id_series.apply(
+                lambda x: ds_id_type_dict[x]
+            ),
         }
     )
     return df_out
 
 
 @pytest.fixture
 def df_outliers() -> pd.DataFrame:
@@ -587,21 +597,59 @@
     )
     pdt.assert_series_equal(bool_ref, bool_range, check_names=False)
 
 
 @pytest.mark.parametrize("zscore", [25])
 @pytest.mark.parametrize("rolling_time_window", ["60min"])
 def test_qc_outlier(df_outliers, zscore, rolling_time_window):
-    df = calc_zscore_results(df_outliers, groupby=Df.DATASTREAM_ID, rolling_time_window=rolling_time_window)
-    df[["qc_zscore_min", "qc_zscore_max"]] = [-1*zscore, zscore]
+    df_outliers[Df.QC_FLAG] = QualityFlags(0)
+    df = calc_zscore_results(
+        df_outliers, groupby=Df.DATASTREAM_ID, rolling_time_window=rolling_time_window
+    )
+    df[["qc_zscore_min", "qc_zscore_max"]] = [-1 * zscore, zscore]
     # df[["qc_zscore_min", "qc_zscore_max"]] = [-3.5, 3.5]
     bool_zscore = get_bool_out_of_range(df=df, qc_on=Df.ZSCORE, qc_type="zscore")
     assert bool_zscore.sum() == 9
 
 
+@pytest.mark.parametrize("zscore", [25])
+@pytest.mark.parametrize("rolling_time_window", ["60min"])
+def test_qc_outlier_qcflags(df_outliers, zscore, rolling_time_window):
+    df = calc_zscore_results(
+        df_outliers, groupby=Df.DATASTREAM_ID, rolling_time_window=rolling_time_window
+    )
+    df[["qc_zscore_min", "qc_zscore_max"]] = [-1 * zscore, zscore]
+    # df[["qc_zscore_min", "qc_zscore_max"]] = [-3.5, 3.5]
+    bool_zscore = get_bool_out_of_range(df=df, qc_on=Df.ZSCORE, qc_type="zscore")
+    assert bool_zscore.sum() == 4
+
+
+def test_zscore_flag_exclusion(df_testing):
+    df_testing[Df.DATASTREAM_ID] = 0
+    df_testing[Df.RESULT] = pd.Series(range(df_testing.shape[0]))
+    df_all0 = calc_zscore_results(df_testing, groupby=Df.DATASTREAM_ID)
+    assert not df_all0[Df.ZSCORE].isnull().any()
+    df_testing.loc[5, Df.QC_FLAG] = QualityFlags(4)
+    df_one4 = calc_zscore_results(df_testing, groupby=Df.DATASTREAM_ID)
+    assert df_one4[Df.ZSCORE].isnull().sum() == 1
+    assert not df_one4[Df.RESULT].isnull().any()
+    assert not df_testing[Df.RESULT].isnull().any()
+
+
+def test_zscore_flag_exclusion2(df_testing):
+    df_testing[Df.DATASTREAM_ID] = 0
+    df_testing.loc[5, Df.QC_FLAG] = QualityFlags(4)
+    df_testing = calc_zscore_results(df_testing, groupby=Df.DATASTREAM_ID)
+    assert df_testing[Df.ZSCORE].isnull().sum() == 1
+    assert not df_testing[Df.RESULT].isnull().any()
+    df_testing[Df.ZSCORE] = calc_zscore_results(df_testing, Df.DATASTREAM_ID, rolling_time_window="60min")[Df.ZSCORE]
+    assert not df_testing[Df.RESULT].isnull().any()
+    assert df_testing[Df.ZSCORE].isnull().sum() == 1
+
+
 @pytest.mark.parametrize("n", tuple(range(len(base_list_region))))
 def test_qc_dependent_quantities_mismatch(df_testing, n):
     # setup ref count
     qc_flag_count_ref = {
         QualityFlags.GOOD: df_testing.shape[0] - 1,
         QualityFlags.BAD: 1,
     }
```

### Comparing `df_qc_tools-0.0.4/tests/resources/data_velocity_acc.csv` & `df_qc_tools-0.0.5/tests/resources/data_velocity_acc.csv`

 * *Files identical despite different names*

### Comparing `df_qc_tools-0.0.4/tests/resources/df_outliers.csv` & `df_qc_tools-0.0.5/tests/resources/df_outliers.csv`

 * *Files identical despite different names*

### Comparing `df_qc_tools-0.0.4/LICENSE` & `df_qc_tools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `df_qc_tools-0.0.4/pyproject.toml` & `df_qc_tools-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "df-qc-tools"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="nvds" },
 ]
 description = "Package for easy datarequests from sensortings"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `df_qc_tools-0.0.4/PKG-INFO` & `df_qc_tools-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: df-qc-tools
-Version: 0.0.4
+Version: 0.0.5
 Summary: Package for easy datarequests from sensortings
 Project-URL: Homepage, https://github.com/nvdsteen/pandassta
 Project-URL: Issues, https://github.com/nvdsteen/pandassta/issues
 Author: nvds
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Requires-Python: >=3.11
 Requires-Dist: geopandas==0.14.3
 Requires-Dist: geopy==2.4.1
 Requires-Dist: hydra-core==1.3.2
 Requires-Dist: numpy==1.26.4
 Requires-Dist: omegaconf==2.3.0
 Requires-Dist: pandas==2.2.1
-Requires-Dist: pandassta>=0.0.2
+Requires-Dist: pandassta>=0.0.3
 Requires-Dist: pytest==8.1.1
 Requires-Dist: scipy==1.12.0
 Requires-Dist: searegion-detection>=0.0.3
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: xarray==2024.2.0
 Description-Content-Type: text/markdown
```

