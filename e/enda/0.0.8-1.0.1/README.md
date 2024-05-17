# Comparing `tmp/enda-0.0.8.tar.gz` & `tmp/enda-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enda-0.0.8.tar", last modified: Mon Jul 18 09:04:36 2022, max compression
+gzip compressed data, was "enda-1.0.1.tar", max compression
```

## Comparing `enda-0.0.8.tar` & `enda-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,29 @@
-drwxr-xr-x   0 clement.jeannesson   (502) staff       (20)        0 2022-07-18 09:04:36.426437 enda-0.0.8/
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)     1064 2022-03-16 16:03:15.000000 enda-0.0.8/LICENSE
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)     3709 2022-07-18 09:04:36.426300 enda-0.0.8/PKG-INFO
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)     3161 2022-06-22 11:47:44.000000 enda-0.0.8/README.md
-drwxr-xr-x   0 clement.jeannesson   (502) staff       (20)        0 2022-07-18 09:04:36.424965 enda-0.0.8/enda/
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)     1086 2022-05-17 12:32:13.000000 enda-0.0.8/enda/__init__.py
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)     5301 2022-06-28 08:59:27.000000 enda-0.0.8/enda/backtesting.py
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)    18584 2022-05-17 12:32:13.000000 enda-0.0.8/enda/contracts.py
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)     2726 2022-06-22 14:19:05.000000 enda-0.0.8/enda/decorators.py
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)    17737 2022-05-17 12:32:13.000000 enda-0.0.8/enda/estimators.py
-drwxr-xr-x   0 clement.jeannesson   (502) staff       (20)        0 2022-07-18 09:04:36.425736 enda-0.0.8/enda/feature_engineering/
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)        0 2022-03-16 16:03:15.000000 enda-0.0.8/enda/feature_engineering/__init__.py
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)     8480 2022-05-17 12:32:13.000000 enda-0.0.8/enda/feature_engineering/calendar.py
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)     8795 2022-05-17 12:32:13.000000 enda-0.0.8/enda/feature_engineering/datetime_features.py
-drwxr-xr-x   0 clement.jeannesson   (502) staff       (20)        0 2022-07-18 09:04:36.426141 enda-0.0.8/enda/ml_backends/
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)        0 2022-03-16 16:03:15.000000 enda-0.0.8/enda/ml_backends/__init__.py
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)     4900 2022-05-17 12:32:13.000000 enda-0.0.8/enda/ml_backends/h2o_estimator.py
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)     7451 2022-03-16 16:03:15.000000 enda-0.0.8/enda/ml_backends/h2o_model.py
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)      891 2022-04-28 16:11:25.000000 enda-0.0.8/enda/ml_backends/sklearn_estimator.py
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)     6323 2022-06-28 08:59:27.000000 enda-0.0.8/enda/power_predictor.py
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)    19765 2022-07-18 08:32:27.000000 enda-0.0.8/enda/power_stations.py
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)     2656 2022-06-28 08:59:27.000000 enda-0.0.8/enda/scoring.py
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)    16312 2022-06-22 11:47:08.000000 enda-0.0.8/enda/timeseries.py
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)     1774 2022-03-16 16:03:15.000000 enda-0.0.8/enda/timezone_utils.py
-drwxr-xr-x   0 clement.jeannesson   (502) staff       (20)        0 2022-07-18 09:04:36.425463 enda-0.0.8/enda.egg-info/
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)     3709 2022-07-18 09:04:36.000000 enda-0.0.8/enda.egg-info/PKG-INFO
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)      614 2022-07-18 09:04:36.000000 enda-0.0.8/enda.egg-info/SOURCES.txt
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)        1 2022-07-18 09:04:36.000000 enda-0.0.8/enda.egg-info/dependency_links.txt
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)       14 2022-07-18 09:04:36.000000 enda-0.0.8/enda.egg-info/requires.txt
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)        5 2022-07-18 09:04:36.000000 enda-0.0.8/enda.egg-info/top_level.txt
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)       38 2022-07-18 09:04:36.426477 enda-0.0.8/setup.cfg
--rw-r--r--   0 clement.jeannesson   (502) staff       (20)     1070 2022-07-18 08:32:27.000000 enda-0.0.8/setup.py
+-rw-r--r--   0        0        0     1064 2023-12-20 16:42:22.372923 enda-1.0.1/LICENSE
+drwxr-xr-x   0        0        0        0 2023-12-20 16:42:22.373324 enda-1.0.1/LICENSES/
+-rw-r--r--   0        0        0     2889 2023-12-20 16:42:22.373076 enda-1.0.1/LICENSES/LICENSE_DATEUTIL
+-rw-r--r--   0        0        0     1542 2023-12-20 16:42:22.373168 enda-1.0.1/LICENSES/LICENSE_NUMPY
+-rw-r--r--   0        0        0     1633 2023-12-20 16:42:22.373280 enda-1.0.1/LICENSES/LICENSE_PANDAS
+-rw-r--r--   0        0        0     1087 2023-12-20 16:42:22.373371 enda-1.0.1/LICENSES/LICENSE_PYTZ
+-rw-r--r--   0        0        0     4335 2024-05-17 15:47:50.819928 enda-1.0.1/README.md
+-rw-r--r--   0        0        0      874 2024-03-29 16:33:16.840268 enda-1.0.1/enda/__init__.py
+-rw-r--r--   0        0        0    13957 2024-05-16 10:14:01.481836 enda-1.0.1/enda/backtesting.py
+-rw-r--r--   0        0        0    18616 2024-05-16 08:53:18.664830 enda-1.0.1/enda/contracts.py
+-rw-r--r--   0        0        0    29845 2024-05-16 10:14:01.482743 enda-1.0.1/enda/estimators.py
+-rw-r--r--   0        0        0        0 2023-12-20 16:42:22.374308 enda-1.0.1/enda/feature_engineering/__init__.py
+-rw-r--r--   0        0        0    19557 2024-05-16 08:53:04.603685 enda-1.0.1/enda/feature_engineering/calendar.py
+-rw-r--r--   0        0        0    11249 2024-03-26 09:18:05.459044 enda-1.0.1/enda/feature_engineering/datetime_features.py
+-rw-r--r--   0        0        0        0 2023-12-20 16:42:22.374703 enda-1.0.1/enda/ml_backends/__init__.py
+-rw-r--r--   0        0        0     6977 2024-05-16 08:53:04.622732 enda-1.0.1/enda/ml_backends/h2o_estimator.py
+-rw-r--r--   0        0        0     4507 2024-05-06 09:42:02.369820 enda-1.0.1/enda/ml_backends/sklearn_estimator.py
+-rw-r--r--   0        0        0     6459 2024-03-26 09:18:05.460763 enda-1.0.1/enda/power_predictor.py
+-rw-r--r--   0        0        0    24117 2024-05-16 08:53:04.615302 enda-1.0.1/enda/power_stations.py
+-rw-r--r--   0        0        0     7125 2024-05-16 08:53:18.723738 enda-1.0.1/enda/scoring.py
+-rw-r--r--   0        0        0        0 2024-03-26 09:18:05.461734 enda-1.0.1/enda/tools/__init__.py
+-rw-r--r--   0        0        0     7877 2024-03-26 09:18:05.462472 enda-1.0.1/enda/tools/decorators.py
+-rw-r--r--   0        0        0     6704 2024-05-16 08:53:18.735529 enda-1.0.1/enda/tools/portfolio_tools.py
+-rw-r--r--   0        0        0    29462 2024-05-16 08:53:18.675778 enda-1.0.1/enda/tools/resample.py
+-rw-r--r--   0        0        0    36877 2024-05-16 08:53:18.753561 enda-1.0.1/enda/tools/timeseries.py
+-rw-r--r--   0        0        0    12207 2024-05-16 08:53:18.756601 enda-1.0.1/enda/tools/timezone_utils.py
+-rw-r--r--   0        0        0     2003 2024-05-17 14:34:06.826401 enda-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5443 1970-01-01 00:00:00.000000 enda-1.0.1/setup.py
+-rw-r--r--   0        0        0     5610 1970-01-01 00:00:00.000000 enda-1.0.1/PKG-INFO
```

### Comparing `enda-0.0.8/LICENSE` & `enda-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enda-0.0.8/enda/contracts.py` & `enda-1.0.1/enda/contracts.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,33 @@
+"""This module contains methods useful to handle contracts data"""
+
 import pandas as pd
 from pandas.api.types import is_string_dtype, is_datetime64_dtype
 from dateutil.relativedelta import relativedelta
+import numpy as np
 import pytz
 
-from enda.timezone_utils import TimezoneUtils
+from sklearn.linear_model import LinearRegression
+
+from enda.ml_backends.sklearn_estimator import EndaSklearnEstimator
+import enda.tools.decorators
+from enda.tools.portfolio_tools import PortfolioTools
+from enda.tools.resample import Resample
+from enda.tools.timeseries import TimeSeries
+from enda.tools.timezone_utils import TimezoneUtils
 
 
 class Contracts:
     """
     A class to help handle contracts data.
 
-    contracts : a dataframe with a contract or sub-contract on each row.
+    contracts : a dataframe with a contract or subcontract on each row.
         A contract row has fixed-values between two dates. In some systems, some values of a contract can change over
         time, for instance the "subscribed power" of an electricity consumption contract.
-        Different ERPs can handle it in different ways, for instance with "sub-contracts" inside a contract
+        Different ERPs can handle it in different ways, for instance with "subcontracts" inside a contract
         or with contract "amendments".
         Here each row is a period between two dates where all the values of the contract are fixed.
 
         Columns can be like in example_a.csv :
         [customer_id,
          contract_id,
          date_start,
@@ -34,361 +44,381 @@
     Columns [date_start, date_end_exclusive] are required (names can differ), and with dtype=datetime64 (tz-naive).
     Other columns describe contract characteristics.
 
 
     """
 
     @classmethod
-    def read_contracts_from_file(cls,
-                                 file_path,
-                                 date_start_col="date_start",
-                                 date_end_exclusive_col="date_end_exclusive",
-                                 date_format="%Y-%m-%d"):
+    def read_contracts_from_file(
+        cls,
+        file_path: str,
+        date_start_col: str = "date_start",
+        date_end_exclusive_col: str = "date_end_exclusive",
+        date_format: str = "%Y-%m-%d",
+    ) -> pd.DataFrame:
         """
         Reads contracts from a file. This will convert start and end date columns into dtype=datetime64 (tz-naive)
         :param file_path: where the source file is located.
         :param date_start_col: the name of your contract date start column.
         :param date_end_exclusive_col: the name of your contract date end column, end date is exclusive.
         :param date_format: the date format for pandas.to_datetime.
         :return: a pandas.DataFrame with a contract on each row.
         """
 
         df = pd.read_csv(file_path)
-        for c in [date_start_col, date_end_exclusive_col]:
-            if is_string_dtype(df[c]):
-                df[c] = pd.to_datetime(df[c], format=date_format)
+        for col in [date_start_col, date_end_exclusive_col]:
+            if col not in df.columns:
+                raise AttributeError(f"Column {col} is not present in the contracts file")
+            if is_string_dtype(df[col]):
+                df[col] = pd.to_datetime(df[col], format=date_format)
         cls.check_contracts_dates(df, date_start_col, date_end_exclusive_col)
         return df
 
     @staticmethod
-    def check_contracts_dates(df, date_start_col, date_end_exclusive_col, is_naive=True):
+    def check_contracts_dates(
+        df: pd.DataFrame,
+        date_start_col: str,
+        date_end_exclusive_col: str,
+        is_naive: bool = True,
+    ):
         """
-        Checks that the two columns are present, with dtype=datetime64 (tz-naive)
-        Checks that date_start is always present.
+        Checks that the two columns, date_start_col and date_end_exclusive_col, are present.
+        Checks that date_start does not have any null value.
         A date_end_exclusive==NaT means that the contract has no limited duration.
         Checks that date_start < date_end_exclusive when date_end_exclusive is set
+        If is_naive is set to True, check that timestamps in date_start_col and date_end_exclusive_col are naive
+        If any of these checks fail, raise a ValueError
 
         :param df: the pandas.DataFrame containing the contracts
         :param date_start_col: the name of your contract date start column.
         :param date_end_exclusive_col: the name of your contract date end column, end date is exclusive.
+        :param is_naive: whether the timestamps in the start and end dates columns are supposed to be naive
         """
 
         # check required columns and their types
-        for c in [date_start_col, date_end_exclusive_col]:
-            if c not in df.columns:
-                raise ValueError("Required column not found : {}".format(c))
+        for col in [date_start_col, date_end_exclusive_col]:
+            if col not in df.columns:
+                raise ValueError(f"Required column not found : {col}")
             # data at a 'daily' precision should not have TZ information
-            if not is_datetime64_dtype(df[c]) and is_naive:
-                raise ValueError("Expected tz-naive datetime dtype for column {}, but found dtype: {}"
-                                 .format(c, df[c].dtype))
+            if not is_datetime64_dtype(df[col]) and is_naive:
+                raise ValueError(
+                    f"Expected tz-naive datetime dtype for column {col}, but found dtype: {df[col].dtype}"
+                )
         # check NaN values for date_start
         if df[date_start_col].isnull().any():
             rows_with_nan_date_start = df[df[date_start_col].isnull()]
-            raise ValueError("There are NaN values in these rows:\n{}".format(rows_with_nan_date_start))
+            raise ValueError(
+                f"There are NaN values in these rows:\n{rows_with_nan_date_start}"
+            )
 
         contracts_with_end = df.dropna(subset=[date_end_exclusive_col])
-        not_ok = contracts_with_end[date_start_col] >= contracts_with_end[date_end_exclusive_col]
+        not_ok = (
+            contracts_with_end[date_start_col]
+            >= contracts_with_end[date_end_exclusive_col]
+        )
         if not_ok.sum() >= 1:
-            raise ValueError("Some ending date happens before starting date:\n{}".format(contracts_with_end[not_ok]))
-
-    @staticmethod
-    def __contract_to_events(contracts, date_start_col, date_end_exclusive_col):
-        # check that no column is named "event_type" or "event_date"
-        for c in ["event_type", "event_date"]:
-            if c in contracts.columns:
-                raise ValueError("contracts has a column named {}, but this name is reserved in this"
-                                 "function; rename your column.".format(c))
-
-        columns_to_keep = [c for c in contracts.columns if c not in [date_start_col, date_end_exclusive_col]]
-        events_columns = ["event_type", "event_date"] + columns_to_keep
-
-        # compute "contract start" and "contract end" events
-        start_contract_events = contracts.copy(deep=True)  # all contracts must have a start date
-        start_contract_events["event_type"] = "start"
-        start_contract_events["event_date"] = start_contract_events[date_start_col]
-        start_contract_events = start_contract_events[events_columns]
-
-        # for "contract end" events, only keep contracts with an end date (NaT = contract is not over)
-        end_contract_events = contracts[contracts[date_end_exclusive_col].notna()].copy(deep=True)
-        end_contract_events["event_type"] = "end"
-        end_contract_events["event_date"] = end_contract_events[date_end_exclusive_col]
-        end_contract_events = end_contract_events[events_columns]
-
-        # concat all events together and sort them chronologically
-        all_events = pd.concat([start_contract_events, end_contract_events])
-        all_events.sort_values(by=["event_date", "event_type"], inplace=True)
-
-        return all_events
+            raise ValueError(
+                f"Some ending date happens before starting date:\n{contracts_with_end[not_ok]}"
+            )
 
     @classmethod
     def compute_portfolio_by_day(
-            cls,
-            contracts,
-            columns_to_sum,
-            date_start_col="date_start",
-            date_end_exclusive_col="date_end_exclusive",
-            max_date_exclusive=None,
-    ):
+        cls,
+        contracts: pd.DataFrame,
+        columns_to_sum: list[str],
+        date_start_col: str = "date_start",
+        date_end_exclusive_col: str = "date_end_exclusive",
+        max_date_exclusive: pd.Timestamp = None,
+        ffill_until_max_date: bool = False,
+    ) -> pd.DataFrame:
         """
         Given a list of contracts_with_group ,
 
         Returns the "portfolio" by day, which is, for each day from the first start of a contract
         to the last end of a contract, the quantities in "columns_to_sum" over time.
         See unittests or enda's guides for examples.
 
         If you want to compute the quantities for a group of customers, filter contracts before using this function.
 
         :param contracts: the dataframe containing the list of contracts to consider.
             Each contract has at least these columns :
                 ["date_start", "date_end_exclusive", and all columns_to_sum]
                 each column in columns_to_sum must be of a summable dtype
         :param columns_to_sum: the columns on which to compute a running-sum over time
-        :param date_start_col:
-        :param date_end_exclusive_col:
+        :param date_start_col: the name of your contract date start column.
+        :param date_end_exclusive_col: the name of your contract date end column, end date is exclusive.
         :param max_date_exclusive: restricts the output to strictly before this date.
                                    Useful if you have end_dates far in the future.
-
+        :param ffill_until_max_date: Whether to forward fill the last available value until max_date_exclusive.
+            Default False
         :return: a 'portfolio' dataframe with one day per row,
                  and the following column hierarchy: (columns_to_sum, group_column)
                  Each day, we have the running sum of each columns_to_sum, for each group of contracts.
                  The first row is the earliest contract start date and the last row is the latest
                  contract start or contract end date.
         """
 
-        for c in ["date"]:
-            if c in contracts.columns:
-                raise ValueError("contracts has a column named {}, but this name is reserved in this"
-                                 "function; rename your column.".format(c))
+        for col in ["date"]:
+            if col in contracts.columns:
+                raise ValueError(
+                    f"contracts has a column named {col}, but this name is reserved in this"
+                    "function; rename your column."
+                )
 
         cls.check_contracts_dates(contracts, date_start_col, date_end_exclusive_col)
 
-        for c in columns_to_sum:
-            if c not in contracts.columns:
-                raise ValueError("missing column_to_sum: {}".format(c))
-            if contracts[c].isnull().any():
-                rows_with_nan_c = contracts[contracts[c].isnull()]
-                raise ValueError("There are NaN values for column {} in these rows:\n{}".format(c, rows_with_nan_c))
+        for col in columns_to_sum:
+            if col not in contracts.columns:
+                raise ValueError(f"missing column_to_sum: {col}")
+            if contracts[col].isnull().any():
+                rows_with_nan_c = contracts[contracts[col].isnull()]
+                raise ValueError(
+                    f"There are NaN values for column {col} in these rows:\n{rows_with_nan_c}"
+                )
 
         # keep only useful columns
         df = contracts[[date_start_col, date_end_exclusive_col] + columns_to_sum]
         # create start and end events for each contract, sorted chronologically
-        events = cls.__contract_to_events(df, date_start_col, date_end_exclusive_col)
+        events = PortfolioTools.portfolio_to_events(
+            df, date_start_col, date_end_exclusive_col
+        )
 
         # remove events after max_date if they are not wanted
         if max_date_exclusive is not None:
             events = events[events["event_date"] <= max_date_exclusive]
 
         # for each column to sum, replace the value by their "increment" (+X if contract starts; -X if contract ends)
-        for c in columns_to_sum:
-            events[c] = events.apply(lambda row: row[c] if row["event_type"] == "start" else -row[c], axis=1)
+        for col in columns_to_sum:
+            events[col] = events.apply(
+                lambda row: row[col] if row["event_type"] == "start" else -row[col], axis=1
+            )
 
         # group events by day and sum the individual contract increments of columns_to_sum to have daily increments
-        df_by_day = events.groupby(["event_date"]).sum()
+        df_by_day = (
+            events
+            .drop(columns={"event_type"})
+            .groupby(["event_date"])
+            .sum()
+        )
 
         # add days that have no increment (with NA values), else the result can have gaps
         # new "NA" increments = no contract start or end event that day = increment is 0
-        df_by_day = df_by_day.asfreq('D').fillna(0)
+        df_by_day = df_by_day.asfreq("D").fillna(0)
 
         # compute cumulative sums of daily increments to get daily totals
         portfolio = df_by_day.cumsum(axis=0)
         portfolio.index.name = "date"  # now values are not increments on an event_date but the total on this date
 
+        # Forward fill the last available value until max_date_exclusive if specified
+        if ffill_until_max_date:
+            if max_date_exclusive is None:
+                raise ValueError(
+                    "ffill_until_max_date has been set to True, but no max_date_exclusive given"
+                )
+            portfolio = Resample.forward_fill_final_record(
+                timeseries_df=portfolio, excl_end_time=max_date_exclusive
+            )
+
         return portfolio
 
     @staticmethod
-    def get_portfolio_between_dates(portfolio, start_datetime, end_datetime_exclusive):
+    @enda.tools.decorators.warning_deprecated_name(
+        namespace_name="Contracts", new_namespace_name="PortfolioTools"
+    )
+    def get_portfolio_between_dates(
+        portfolio: pd.DataFrame,
+        start_datetime: pd.Timestamp,
+        end_datetime_exclusive: pd.Timestamp,
+    ) -> pd.DataFrame:
         """
-        Adds or removes dates if needed.
-
-        If additional dates are needed at the beginning, add these dates with 0s
-        If additional dates needed at the end, copy the portfolio of the last date into the additional dates
-
-        :param portfolio: the dataframe with the portfolio, must have a pandas.DatetimeIndex with frequency
-        :param start_datetime:
-        :param end_datetime_exclusive:
-        :return:
+        Keeps portfolio data between the specified dates.
+        If the first date in portfolio is after start_datetime, we add missing dates with 0 as value.
+        If the last date in portfolio is before end_datetime_exclusive, we forward fill the last present values
+        until end_datetime_exclusive
+        :param portfolio: The portfolio DataFrame. It must have a pd.DatetimeIndex with a frequency
+        :param start_datetime: The start datetime from which to keep the portfolio
+        :param end_datetime_exclusive: The exclusive end datetime until which to keep the portfolio
+        :return: A portfolio DataFrame with values between specified dates
         """
 
-        df = portfolio.copy(deep=True)
-
-        if not isinstance(df.index, pd.DatetimeIndex):
-            raise TypeError("The index of daily_portfolio should be a pd.DatetimeIndex, but given {}"
-                            .format(df.index.dtype))
-
-        if df.index.freq is None:
-            raise ValueError("portfolio.index needs to have a freq. "
-                             "Maybe try to set one using df.index.inferred_freq")
-
-        freq = df.index.freq
-
-        # check that there is no missing value
-        if not df.isnull().sum().sum() == 0:
-            raise ValueError("daily_portfolio has NaN values.")
-
-        if start_datetime is not None and df.index.min() > start_datetime:
-            # add days with empty portfolio at the beginning
-            df = df.append(pd.Series(name=start_datetime, dtype='object'))
-            df.sort_index(inplace=True)  # put the new row first
-            df = df.asfreq(freq).fillna(0)
-
-        if end_datetime_exclusive is not None and df.index.max() < end_datetime_exclusive:
-            # add days at the end, with the same portfolio as the last available day
-            df = df.append(pd.Series(name=end_datetime_exclusive, dtype='object'))
-            df.sort_index(inplace=True)  # make sure this new row is last
-            df = df.asfreq(freq, method='ffill')
-
-        # remove dates outside of desired range
-        df = df[(df.index >= start_datetime) & (df.index < end_datetime_exclusive)]
-        assert df.isnull().sum().sum() == 0  # check that there is no missing value
-
-        return df
+        return PortfolioTools.get_portfolio_between_dates(
+            portfolio_df=portfolio,
+            start_datetime=start_datetime,
+            end_datetime_exclusive=end_datetime_exclusive,
+        )
 
     @classmethod
-    def forecast_portfolio_linear(cls,
-                                  portfolio_df: pd.DataFrame,
-                                  start_forecast_date,
-                                  end_forecast_date_exclusive,
-                                  freq: [pd.Timedelta, str],
-                                  max_allowed_gap: pd.Timedelta = pd.Timedelta(days=1),
-                                  tzinfo: [pytz.timezone, str, None] = None
-                                  ):
-
+    def forecast_portfolio_linear(
+        cls,
+        portfolio_df: pd.DataFrame,
+        start_forecast_date,
+        end_forecast_date_exclusive,
+        freq: [pd.Timedelta, str] = None,
+        max_allowed_gap: pd.Timedelta = pd.Timedelta(days=1),
+        tzinfo: [pytz.timezone, str, None] = None,
+    ) -> pd.DataFrame:
+        """
+        Forecast portfolio using a linear extrapolation for the next nb_days
+        The output has the frequency which is given as an input, and defaults to the one of input portfolio_df
+         if nothing is provided.
+        :param portfolio_df: The portfolio DataFrame to perform the forecast on
+        :param start_forecast_date: The start datetime from which to extend the portfolio
+        :param end_forecast_date_exclusive: The exclusive end datetime until which to extend the portfolio
+        :param freq: The frequency of the resulting linearly-extrapolated portfolio
+        :param max_allowed_gap: The max gap between the end of the portfolio and the start date of the extrapolation.
+                                Returns an error if exceeded.
+        :param tzinfo: The time-zone of the resulting dataframe, if we want to change it.
+        :return: pd.DataFrame (the linearly-extrapolated forecast portfolio data)
+        """
         if end_forecast_date_exclusive < start_forecast_date:
             raise ValueError("end_forecast_date must be after start_forecast_date")
 
         gap = portfolio_df.index.max() - start_forecast_date
         if gap > max_allowed_gap:
-            raise ValueError("The gap between the end of portfolio_df and start_forecast_date is too big:"
-                             "{} (max_allowed_gap={}). Provide more recent data or change max_allowed_gap."
-                             .format(gap, max_allowed_gap))
+            raise ValueError(
+                "The gap between the end of portfolio_df and start_forecast_date is too big:"
+                f"{gap} (max_allowed_gap={max_allowed_gap}). Provide more recent data or change "
+                "max_allowed_gap."
+            )
 
         if not isinstance(portfolio_df.index, pd.DatetimeIndex):
-            raise ValueError("portfolio_df should have a pandas.DatetimeIndex, but given {}"
-                             .format(portfolio_df.index.dtype))
+            raise ValueError(
+                f"portfolio_df should have a pandas.DatetimeIndex, but given {portfolio_df.index.dtype}"
+            )
 
-        try:
-            from enda.ml_backends.sklearn_estimator import EndaSklearnEstimator
-            from sklearn.linear_model import LinearRegression
-            import numpy as np
-        except ImportError:
-            raise ImportError("sklearn is required is you want to use this function. "
-                              "Try: pip install scikit-learn")
+        if not freq:
+            freq = TimeSeries.find_most_common_frequency(portfolio_df.index)
 
         result_index = pd.date_range(
             start=start_forecast_date,
             end=end_forecast_date_exclusive,
             freq=freq,
             name=portfolio_df.index.name,
-            closed='left'
+            inclusive="left",
         )
 
         if tzinfo is not None:
             result_index = result_index.tz_convert(tzinfo)
 
         predictions = []
 
-        for c in portfolio_df.columns:
-            epoch_column = "seconds_since_epoch_" if c != "seconds_since_epoch_" else "seconds_since_epoch__"
+        for col in portfolio_df.columns:
+            epoch_column = (
+                "seconds_since_epoch_"
+                if col != "seconds_since_epoch_"
+                else "seconds_since_epoch__"
+            )
 
-            train_set = portfolio_df[[c]].copy(deep=True)
+            train_set = portfolio_df[[col]].copy(deep=True)
             train_set[epoch_column] = train_set.index.astype(np.int64) // 10**9
 
             test_set = pd.DataFrame(
-                data={"epoch_column": result_index.astype(np.int64) // 10**9},
-                index=result_index
+                data={epoch_column: result_index.astype(np.int64) // 10**9},
+                index=result_index,
             )
 
             lr = EndaSklearnEstimator(LinearRegression())
-            lr.train(train_set, target_col=c)
-            predictions.append(lr.predict(test_set, target_col=c))
+            lr.train(train_set, target_col=col)
+            predictions.append(lr.predict(test_set, target_col=col))
 
-        return pd.concat(predictions, axis=1, join='outer')
+        return pd.concat(predictions, axis=1, join="outer")
 
     @classmethod
-    def forecast_portfolio_holt(cls,
-                                portfolio_df: pd.DataFrame,
-                                start_forecast_date,
-                                nb_days: int = 14,
-                                past_days: int = 100,
-                                holt_init_params=None, holt_fit_params=None):
+    def forecast_portfolio_holt(
+        cls,
+        portfolio_df: pd.DataFrame,
+        start_forecast_date,
+        nb_days: int = 14,
+        past_days: int = 100,
+        holt_init_params=None,
+        holt_fit_params=None,
+    ) -> pd.DataFrame:
         """
         Forecast using exponential smoothing (Holt method) for the next nb_days
         The output has the same frequency as input portfolio_df.
 
-        :param portfolio_df:
+        :param portfolio_df: The portfolio DataFrame to perform the forecast on
         :param start_forecast_date: when we stop the portfolio data and start forecasting
         :param nb_days: number of days after 'end_date' to forecast
         :param past_days: max number of days to use in the past used to make the forecast
                           (it is better to use only recent data)
         :param holt_init_params: the dict of parameters to give to the Holt __init__ method. If none, defaults to :
                                 holt_fit_params={"initialization_method":"estimated"}
                                 For more details see the statsmodels documentation :
                                 https://www.statsmodels.org/stable/examples/notebooks/generated/exponential_smoothing.html
-        :param holt_fit_params: the dict of params to give to the Holt.fi() method. If none, defaults to : {}
+        :param holt_fit_params: the dict of params to give to the Holt.fit() method. If none, defaults to : {}
         :return: pd.DataFrame (the forecast data)
         """
 
         try:
             from statsmodels.tsa.api import Holt
-        except ImportError:
-            raise ImportError("statsmodels is required is you want to use this function. "
-                              "Try: pip install statsmodels>=0.12.0")
+        except ImportError as exc:
+            raise ImportError(
+                "statsmodels is required is you want to use this function. "
+                "Try: pip install statsmodels>=0.12.0"
+            ) from exc
 
         if holt_init_params is None:
             holt_init_params = {"initialization_method": "estimated"}
 
         if holt_fit_params is None:
             holt_fit_params = {}
 
         if nb_days < 1:
-            raise ValueError("nb_days should be at least 1, given {}".format(nb_days))
+            raise ValueError(f"nb_days should be at least 1, given {nb_days}")
 
         if start_forecast_date > portfolio_df.index.max() + relativedelta(days=1):
-            raise ValueError("Start forecast date ({}) more than 1 day after the latest portfolio information ({}). "
-                             "Portfolio information given is too old."
-                             .format(start_forecast_date, portfolio_df.index.max()))
+            raise ValueError(
+                f"Start forecast date ({start_forecast_date}) more than 1 day after the latest portfolio "
+                f"information ({portfolio_df.index.max()}). Portfolio information given is too old."
+            )
 
         if not isinstance(portfolio_df.index, pd.DatetimeIndex):
-            raise ValueError("portfolio_df should have a pandas.DatetimeIndex, but given {}"
-                             .format(portfolio_df.index.dtype))
+            raise ValueError(
+                f"portfolio_df should have a pandas.DatetimeIndex, but given {portfolio_df.index.dtype}"
+            )
 
         if portfolio_df.index.freq is None:
-            raise ValueError("Input portfolio_df must have a frequency. "
-                             "Maybe try to set it using pandas.index.inferred_freq")
+            raise ValueError(
+                "Input portfolio_df must have a frequency. "
+                "Maybe try to set it using pandas.index.inferred_freq"
+            )
 
         # only keep portfolio data before the start_forecast_date
         freq = portfolio_df.index.freq
         tzinfo = portfolio_df.index.tzinfo  # can be None
 
-        pf = portfolio_df
-        pf = pf[pf.index <= start_forecast_date]
+        p_df = portfolio_df
+        p_df = p_df[p_df.index <= start_forecast_date]
 
         end_forecast_date = TimezoneUtils.add_interval_to_day_dt(
-            day_dt=start_forecast_date,
-            interval=relativedelta(days=nb_days)
+            day_dt=start_forecast_date, interval=relativedelta(days=nb_days)
         )
         date_past_days_ago = TimezoneUtils.add_interval_to_day_dt(
-            day_dt=start_forecast_date,
-            interval=relativedelta(days=-past_days)
+            day_dt=start_forecast_date, interval=relativedelta(days=-past_days)
         )
 
         # only keep recent data to determine the trends
-        pf = pf[pf.index >= date_past_days_ago]
+        p_df = p_df[p_df.index >= date_past_days_ago]
 
         future_index = pd.date_range(
             start_forecast_date,
             end_forecast_date,
             freq=freq,
-            name=pf.index.name,
-            closed='left'
+            name=p_df.index.name,
+            inclusive="left"
         )
         if tzinfo is not None:
             future_index = future_index.tz_convert(tzinfo)
 
         # holt needs a basic integer index
-        pf = pf.reset_index(drop=True)
+        p_df = p_df.reset_index(drop=True)
         # forecast each column (all columns are measures)
-        result = pf.apply(lambda x: Holt(x, **holt_init_params).fit(**holt_fit_params).forecast(len(future_index)))
+        result = p_df.apply(
+            lambda x: Holt(x, **holt_init_params)
+            .fit(**holt_fit_params)
+            .forecast(len(future_index))
+        )
         result = result.round(1)
         result.index = future_index
 
         return result
```

### Comparing `enda-0.0.8/enda/estimators.py` & `enda-1.0.1/enda/estimators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,375 +1,682 @@
+"""This module contains several basic machine learning estimators"""
+
 import abc
-from collections import OrderedDict
-import pandas
+import collections
 import typing
+from collections import OrderedDict
+from typing import Iterable, Optional, Callable, Tuple
+
+import pandas as pd
+
+from enda.scoring import Scoring
 
 
 class EndaEstimator(metaclass=abc.ABCMeta):
     """
     This interface represents a simple machine learning estimator with some universal functions.
     We require these functions :
         train : train the estimator
         predict : predict using the estimator
+        get_model_params : return the hyperparameters of the model
 
     To save and load instances of a class, use tools like pickle or joblib
     (see information for instance here: https://scikit-learn.org/stable/modules/model_persistence.html).
 
     This interface is useful to create more advanced estimators based on these building blocks :
         EndaNormalizedEstimator : uses one of the inputs as a 'normalization variable' instead of a 'training feature'.
         EndaStackingEstimator : combines several estimators to create a more robust estimator
                                 (cross-algorithm 'ensemble' method).
         EndaEstimatorWithFallback : an estimator that can cope with missing input in a robust way.
 
     See tutorials about Python interfaces for instance here https://realpython.com/python-interface/ .
     """
-
-    @classmethod
-    def __subclasshook__(cls, subclass):
-        return (
-            hasattr(subclass, 'train') and callable(subclass.train) and
-            hasattr(subclass, 'predict') and callable(subclass.predict))
+    def __init__(self):
+        # if set, _training_df stores the training dataframe (features + target)
+        # if set, _target_name stores the target name
+        self._training_df = None
+        self._target = None
 
     @abc.abstractmethod
-    def train(self, df: pandas.DataFrame, target_col: str):
+    def train(self, df: pd.DataFrame, target_col: str):
         """Trains the estimator using the given data."""
         raise NotImplementedError
 
+    def fit(self, X: pd.DataFrame, y:pd.Series):
+        """Trains the estimator using the given data."""
+        return self.train(df=pd.concat([X, y], axis=1), target_col=y.name)
+
     @abc.abstractmethod
-    def predict(self, df: pandas.DataFrame, target_col: str) -> pandas.DataFrame:
-        """ Predicts and returns a dataframe with just 1 column: target_col_name """
+    def predict(self, df: pd.DataFrame, target_col: str) -> pd.DataFrame:
+        """Predicts and returns a dataframe with just 1 column: target_col_name"""
         raise NotImplementedError
 
+    def get_model_name(self) -> str:
+        """Return the estimator name"""
+        return self.__class__.__name__
 
-class EndaNormalizedEstimator(EndaEstimator):
+    @abc.abstractmethod
+    def get_model_params(self) -> dict:
+        """Return a dict with the model name and hyperparameters"""
+        raise NotImplementedError
+
+    def get_loss_training(self,
+                          score_list: list[str] = None,
+                          process_forecast_specs: Optional[Tuple[Callable, dict]] = None) -> pd.Series:
+        """
+         Compute the training loss, i.e. the error of the trained model on the training dataset.
+         If not overridden (eg. in H2OEstimator), this function computes the loss on the training
+         dataset, using scikit-learn built-in methods.
+        :param score_list: the statistics to consider. Either 'mae', 'rmse', 'r2', 'max_error', 'mape'.
+            Defaults to 'rmse'.
+        :param process_forecast_specs: Optional. If given, it defines a function to apply to the forecast before
+            calculating the loss.
+        :return: a series that contains for each statistics the score of the model on the training set
+        """
+
+        # if _training_df or _target is None, that means the model has not been trained
+        if self._training_df is None or self._target is None:
+            raise ValueError("The model must be trained before calling this method.")
+
+        # compute the prediction over the training dataset
+        predict_on_train_set_df = self.predict(df=self._training_df.drop(columns=self._target), target_col=self._target)
+
+        if process_forecast_specs is not None:
+            process_forecast_function, process_forecast_kwargs = process_forecast_specs
+            predict_on_train_set_df = process_forecast_function(predict_on_train_set_df, **process_forecast_kwargs)
+
+        score_series = Scoring.compute_loss(predicted_df=predict_on_train_set_df,
+                                            actual_df=self._training_df[self._target],
+                                            score_list=score_list)
 
-    def __init__(self,
-                 inner_estimator: EndaEstimator,
-                 target_col: str,
-                 normalization_col: str,
-                 columns_to_normalize: [typing.Iterable[str], None] = None):
-        """
-        An estimator that uses one of the inputs as a linear 'normalization variable' instead of a 'training feature'.
-        The prediction is:
-        predict(X) = X[normalization_col] * predict(X without normalization_col)
+        return score_series
+
+    def get_feature_importance(self) -> pd.Series:
+        """
+        Return the feature's importance once a model has been trained.
+        Such a feature is usually not implemented, except for some algorithm in
+        particular (let's say, sklearn and H2O, and not all of them)
+        :return: a series that contain the percentage of importance for each variable
+        """
+        raise NotImplementedError()
+
+
+class EndaNormalizedEstimator(EndaEstimator):
+    """
+    An estimator that uses one of the inputs as a linear 'normalization variable' instead of a 'training feature'.
+    The prediction is:
+    predict(X) = X[normalization_col] * predict(X without normalization_col)
 
-        The predict(X without normalization_col) is made by another underlying estimator: inner_estimator.
+    predict(X without normalization_col) is made by another underlying estimator: inner_estimator.
+    """
 
+    def __init__(
+            self,
+            inner_estimator: EndaEstimator,
+            target_col: str,
+            normalization_col: str,
+            columns_to_normalize: Optional[Iterable[str]] = None,
+    ):
+        """
+        Initialize the normalized estimator
         :param inner_estimator: the estimator that will perform predict(X without normalization_col)
         :param normalization_col: name of the column used as a multiplier and not as a feature.
         :param columns_to_normalize: (optional) columns in 'X without normalization_col' that must be divided
-        by normalization_col for the the underlying estimator to train/predict correctly.
+        by normalization_col for the underlying estimator to train/predict correctly.
         """
 
         if not issubclass(type(inner_estimator), EndaEstimator):
-            raise TypeError("inner_estimator's type is '{}' : it must implement EndaEstimator."
-                            .format(type(inner_estimator)))
+            raise TypeError(
+                f"inner_estimator's type is '{type(inner_estimator)}' : it must implement EndaEstimator."
+            )
 
         if columns_to_normalize and normalization_col in columns_to_normalize:
-            raise ValueError("normalisation_col '{}'should not be in columns_to_normalize {}"
-                             .format(normalization_col, columns_to_normalize))
+            raise ValueError(
+                f"normalisation_col '{normalization_col}'should not be in columns_to_normalize {columns_to_normalize}"
+            )
 
+        super().__init__()
         self.inner_estimator = inner_estimator
         self.target_col = target_col
         self.normalisation_col = normalization_col
         self.columns_to_normalize = columns_to_normalize
 
-    def check_normalization_col(self, df: pandas.DataFrame):
+    def get_model_params(self) -> dict:
+        """Return a dict with the model name and hyperparameters"""
+        return {self.get_model_name(): self.inner_estimator.get_model_params()}
+
+    def check_normalization_col(self, df: pd.DataFrame):
+        """
+        Checks that the values of the normalization col in the input DataFrame are strictly positive, otherwise
+        raise an error
+        :param df: The DataFrame to check
+        """
+
+        if self.normalisation_col not in df:
+            raise ValueError(
+                f"Normalisation_col '{self.normalisation_col}' not present in the Dataframe to normalize"
+            )
         zeros_df = df[df[self.normalisation_col] <= 0]
         if not zeros_df.empty:
-            raise ValueError("Normalisation_col '{}' : zeros found\n{}".format(self.normalisation_col, zeros_df))
+            raise ValueError(
+                f"Normalisation_col '{self.normalisation_col}' : zeros found\n{zeros_df}"
+            )
 
-    def normalize(self, df: pandas.DataFrame):
+    def normalize(self, df: pd.DataFrame) -> pd.DataFrame:
+        """
+        Checks that the normalization column has only strictly positive values, then normalizes the columns of the
+        DataFrame that are in the columns_to_normalize attribute by dividing them by the normalization column. Also
+        normalizes the target_col if it is in the DataFrame columns. Then, drops normalization_col
+        :param df: The DataFrame to normalize
+        :return: The DataFrame with columns part of columns_to_normalize or the target_col column normalized, and
+            without the normalization_col
+        """
         self.check_normalization_col(df)
         df_norm = df.copy(deep=True)
 
         if self.columns_to_normalize:
-            for c in df.columns:
-                if c in self.columns_to_normalize:
-                    df_norm[c] = df_norm[c]/df[self.normalisation_col]
+            for col in df.columns:
+                if col in self.columns_to_normalize:
+                    df_norm[col] = df_norm[col] / df[self.normalisation_col]
 
         # always normalize the target if it is in the df (present in train mode, not in predict mode)
         if self.target_col in df.columns:
-            df_norm[self.target_col] = df_norm[self.target_col]/df[self.normalisation_col]
+            df_norm[self.target_col] = (
+                    df_norm[self.target_col] / df[self.normalisation_col]
+            )
 
         df_norm.drop(columns=self.normalisation_col, inplace=True)
         return df_norm
 
-    def train(self, df: pandas.DataFrame, target_col: str = None, drop_where_normalization_under_zero: bool = False):
+    def train(
+            self,
+            df: pd.DataFrame,
+            target_col: str = None,
+            drop_where_normalization_under_zero: bool = False,
+    ):
+        """
+        Normalizes the DataFrame and trains the inner estimator
+        :param df: The training DataFrame
+        :param target_col: The variable to predict
+        :param drop_where_normalization_under_zero: Whether to drop rows where normalization_col is not strictly
+            positive. Note that the normalize function will raise an error if there is still negative values in
+            normalization_col
+        """
         if target_col and self.target_col != target_col:
-            raise ValueError("target should be None or {}, but given: {}".format(self.target_col, target_col))
+            raise ValueError(
+                f"target should be None or {self.target_col}, but given: {target_col}"
+            )
 
         if drop_where_normalization_under_zero:
             df = df.loc[df[self.normalisation_col] > 0, :]
         df_norm = self.normalize(df)
         self.inner_estimator.train(df_norm, self.target_col)
 
-    def predict(self, df: pandas.DataFrame, target_col: str = None):
-        if target_col and self.target_col != target_col:
-            raise ValueError("target should be None or '{}', but given: '{}'".format(self.target_col, target_col))
+        # store the training
+        self._training_df = df
+        self._target = target_col
 
-        df_norm = self.normalize(df)  # error out if any value of normalization_col is <= 0
+    def predict(self, df: pd.DataFrame, target_col: str = None) -> pd.DataFrame:
+        """
+        Normalizes the input DataFrame, then uses the inner estimator to make a prediction on target_col. Then,
+        multiplies the result by the normalization_col to get the final prediction
+        :param df: The forecast input DataFrame
+        :param target_col: The variable to predict
+        :return: The final prediction of the estimator
+        """
+        if target_col and self.target_col != target_col:
+            raise ValueError(
+                f"target should be None or '{self.target_col}', but given: '{target_col}'."
+            )
+
+        df_norm = self.normalize(
+            df
+        )  # error out if any value of normalization_col is <= 0
         predict_norm = self.inner_estimator.predict(df_norm, self.target_col)
 
         if (predict_norm.index != df.index).any():
-            raise ValueError("prediction must have the same index as given df. "
-                             "Check that for self.inner_estimator, the method 'predict' conserves index.")
+            raise ValueError(
+                "prediction must have the same index as given df. "
+                "Check that for self.inner_estimator, the method 'predict' conserves index."
+            )
 
-        predict = predict_norm.multiply(df[self.normalisation_col], axis='index')
+        predict = predict_norm.multiply(df[self.normalisation_col], axis="index")
         return predict
 
 
 class EndaStackingEstimator(EndaEstimator):
+    """
+    This class serves the same purpose as the Scikit-Learn "Stacking Regressor". However since we work on
+    time-series, we need fine control on which data is passed to train the base_estimators before training
+    the final_estimator (to keep it all chronologically consistent).
+
+    Training is made this way :
+        temporarily train base_estimators on train_set[:x]
+        use base_estimators to predict on train_set[x:] -> base_predictions
+        train final_estimator on the base_predictions
+        re-train base_estimators on the full train-set
+    We have to train base_estimators twice, because if we trained them on the full set and then predict on
+    train_set[x:] for training final_estimator, we would be making a prediction on part of the data that was used to
+    train them, which would be a huge risk of over-fitting
+    """
 
-    def __init__(self,
-                 base_estimators: typing.Mapping[str, EndaEstimator],
-                 final_estimator: EndaEstimator,
-                 base_stack_split_pct: float = 0.20
-                 ):
-        """
-        This class serves the same purpose as the Scikit-Learn "Stacking Regressor". However since we work on
-        time-series, we need fine control on which data is passed to train the base_estimators before training
-        the final_estimator (to keep it all chronologically consistent).
-
-        Training is made this way :
-            temporarily train base_estimators on train_set[:x]
-            use base_estimators to predict on train_set[x:] -> base_predictions
-            train final_estimator on the base_predictions
-            re-train base_estimators on the full train-set
-
-        :param base_estimators: a dict of {estimator_id -> estimator}, each estimator must be an EndaEstimator.
+    def __init__(
+            self,
+            base_estimators: typing.Mapping[str, EndaEstimator],
+            final_estimator: EndaEstimator,
+            base_stack_split_pct: float = 0.20,
+    ):
+        """
+        Initialize the stacking estimator
+        :param base_estimators: a dict of {estimator_id -> estimator}, each estimator (there must be at least 2) must
+            be an EndaEstimator.
         :param final_estimator: the estimator used for stacking, must also implement be an EndaEstimator.
-        :param base_stack_split_pct: the % of data used to train the base_estimators for
-                                     before training final_estimator
-                                     (this can be overwritten in the train function).
+        :param base_stack_split_pct: the % of data used to train the base_estimators before training final_estimator
+            (this can be overwritten in the train function).
         """
 
         if len(base_estimators) <= 1:
-            raise ValueError("At least 2 base_estimators are required, but given: {}".format(len(base_estimators)))
+            raise ValueError(
+                f"At least 2 base_estimators are required, but given: {len(base_estimators)}"
+            )
 
         # We store estimators in an ordered dict to make sure we always iterate over them in the same order
         self.base_estimators = OrderedDict()
         for estimator_id in sorted(base_estimators.keys()):
             self.base_estimators[estimator_id] = base_estimators[estimator_id]
 
+        super().__init__()
         self.final_estimator = final_estimator
         self.base_stack_split_pct = base_stack_split_pct
 
-    def train(self, df: pandas.DataFrame, target_col: str, base_stack_split_pct: [float, None] = None):
-
-        split_pct = base_stack_split_pct if base_stack_split_pct else self.base_stack_split_pct
+    def train(
+            self,
+            df: pd.DataFrame,
+            target_col: str,
+            base_stack_split_pct: [float, None] = None,
+    ):
+        """
+        Train base and final estimators.
+        :param df: The training dataset
+        :param target_col: The column to predict
+        :param base_stack_split_pct: If specified, will overwrite the EndaStackingEstimator attribute.
+        """
+        split_pct = (
+            base_stack_split_pct if base_stack_split_pct else self.base_stack_split_pct
+        )
 
         # training final_estimator will temporarily train single estimators on part of the data,
         # so it must be done before training the actual single estimators
         self.train_final_estimator(df, target_col, split_pct)
 
         # re-train base estimators with the full dataset
         self.train_base_estimators(df, target_col)
 
-    def train_final_estimator(self, df, target_col, split_pct):
+        # store the training
+        self._training_df = df
+        self._target = target_col
+
+    def train_final_estimator(
+            self, df: pd.DataFrame, target_col: str, split_pct: float
+    ):
         """
         Trains the final estimator used for stacking.
-
         (Temporarily) train the single estimators with a subset of the data,
         then apply them on the rest of the data. Use this to train the stacking estimator.
+        :param df: The DataFrame with training data
+        :param target_col: The column to predict
+        :param split_pct: The percentage of training data to use to train the base estimators. The rest of the data
+            will be used to train the final estimator based on the predictions of the base estimators
         """
 
         # split the training frame : ,
-        split_int = int(df.shape[0] * (1-split_pct))
+        split_int = int(df.shape[0] * (1 - split_pct))
         split_idx = df.index[split_int]
 
-        df_base_estimators = df[df.index < split_idx]  # one part to train the base estimators
-        df_stacking = df[df.index >= split_idx]  # the other to train the stacking estimator
+        df_base_estimators = df[
+            df.index < split_idx
+            ]  # one part to train the base estimators
+        df_stacking = df[
+            df.index >= split_idx
+            ]  # the other to train the stacking estimator
 
         if df_base_estimators.shape[0] == 0 or df_stacking.shape[0] == 0:
-            raise ValueError("The split gave an empty train set for the base estimators or the final estimator. "
-                             "Change parameter 'split_pct' (given {}) or provide a larger training set."
-                             .format(split_pct))
+            raise ValueError(
+                "The split gave an empty train set for the base estimators or the final estimator. "
+                f"Change parameter 'split_pct' (given {split_pct}) or provide a larger training set."
+            )
 
         self.train_base_estimators(df_base_estimators, target_col)
 
         # make predictions with these temporary base_estimators, without the target column
-        base_predictions = self.predict_base_estimators(df_stacking.drop(columns=[target_col]), target_col)
+        base_predictions = self.predict_base_estimators(
+            df_stacking.drop(columns=[target_col]), target_col
+        )
 
         # add the target back, to train the final estimator
         base_predictions[target_col] = df_stacking[target_col]
 
         self.final_estimator.train(base_predictions, target_col)
 
-    def predict_base_estimators(self, df, target_col):
+    def predict_base_estimators(
+            self, df: pd.DataFrame, target_col: str
+    ) -> pd.DataFrame:
         """
+        Make a prediction using base estimators
+        :param df: The input DataFrame for prediction
+        :param target_col: The name of the column to predict
         :return: a Dataframe with the prediction of each base estimator in each column (on several rows).
-        Each column's name is the estimator_id given on initialisation.
+            Each column's name is the estimator_id given on initialisation.
         """
 
         estimator_dfs = []
         for estimator_id, estimator in self.base_estimators.items():
             estimator_predict = estimator.predict(df, target_col)
 
             if (estimator_predict.index != df.index).any():
-                raise ValueError("prediction must have the same index as given df. "
-                                 "Check that for estimator with id '{}', the method 'predict' conserves index."
-                                 .format(estimator_id))
+                raise ValueError(
+                    "prediction must have the same index as given df. "
+                    f"Check that for estimator with id '{estimator_id}', the method 'predict' conserves index."
+                )
 
             estimator_predict.rename(columns={target_col: estimator_id}, inplace=True)
             estimator_dfs.append(estimator_predict)
 
-        predict_df = pandas.concat(estimator_dfs, axis=1, join='outer')
+        predict_df = pd.concat(estimator_dfs, axis=1, join="outer")
 
         if predict_df.shape[0] != df.shape[0]:
-            raise ValueError("Given {} values to predict, but predicted {}"
-                             .format(df.shape[0], predict_df.shape[0]))
+            raise ValueError(
+                f"Given {df.shape[0]} values to predict, but predicted {predict_df.shape[0]}"
+            )
 
         return predict_df
 
-    def train_base_estimators(self, df, target_col):
-        for estimator_id, estimator in self.base_estimators.items():
+    def train_base_estimators(self, df: pd.DataFrame, target_col: str):
+        """
+        Train the base estimators
+        :param df: The training data
+        :param target_col: The column to predict
+        """
+        for _, estimator in self.base_estimators.items():
             estimator.train(df, target_col)
 
-    def predict(self, df: pandas.DataFrame, target_col: str):
+    def predict(self, df: pd.DataFrame, target_col: str) -> pd.DataFrame:
+        """
+        Make predictions with base estimators, then uses them to make a prediction with the final estimator
+        :param df: The input data for prediction
+        :param target_col: The column to predict
+        :return: A DataFrame with the predicted column
+        """
         base_predictions = self.predict_base_estimators(df, target_col)
         prediction = self.final_estimator.predict(base_predictions, target_col)
 
         if (prediction.index != df.index).any():
-            raise ValueError("prediction must have the same index as given df. "
-                             "Check that self.final_estimator.predict conserves index.")
+            raise ValueError(
+                "prediction must have the same index as given df. "
+                "Check that self.final_estimator.predict conserves index."
+            )
 
         return prediction
 
+    def get_model_params(self) -> dict:
+        """
+        Get model parameters of estimators (each of base_estimator) and final_estimator
+        The principle is to return the model params as  a dict with two entries, base_estimators, and final_estimator
+        Each of these entries contains a dictionary as well, with the model name as a key, and model parameters
+        as values.
+        :return: A dictionary with one entry per model and associated parameters
+        """
+
+        model_params_dict = {"base_estimators": collections.defaultdict(dict)}
+
+        # define base estimator
+        for _, estimator in self.base_estimators.items():
+            model_params = estimator.get_model_params()
+            for estimator_name, estimator_params in model_params.items():
+
+                # we need to modify the estimator name in the dict keys, if the same estimator
+                # is defined several times. For instance, if several LinearRegression are defined,
+                # we call them LinearRegression, LinearRegression_1, LinearRegression_2...
+                original_estimator_name = estimator_name
+                count = 1
+                while estimator_name in model_params_dict["base_estimators"]:
+                    estimator_name = f"{original_estimator_name}_{count}"
+                    count += 1
+                model_params_dict["base_estimators"][estimator_name] = estimator_params
+        model_params_dict["base_estimators"] = dict(model_params_dict["base_estimators"])
+        model_params_dict["final_estimator"] = self.final_estimator.get_model_params()
+
+        return {self.get_model_name(): model_params_dict}
+
+    def get_all_model_names(self) -> dict[str, list[str]]:
+        """
+        Get name of all base models, plus name of final model
+        in a dictionary with two entries, "base_estimator" and "final_estimator"
+        """
+
+        sub_model_names_dict = {"base_estimators": []}
+        for _, estimator in self.base_estimators.items():
+            sub_model_names_dict["base_estimators"].append(estimator.get_model_name())
+
+        sub_model_names_dict["final_estimator"] = [self.final_estimator.get_model_name()]
+
+        return sub_model_names_dict
+
 
 class EndaEstimatorWithFallback(EndaEstimator):
     """
     This estimator allows to make a prediction even when some important input is missing.
 
     In order to deal with missing values, it is common practice to replace None/NA with some meaningful value like
     the mean or the median of the values found in the train set for this feature.
-    However this is problematic when the missing variable has a significant impact on the prediction.
+    However, this is problematic when the missing variable has a significant impact on the prediction.
 
     Instead, this estimator trains 2 underlying estimators:
     an 'estimator_with' and an 'estimator_without' the column that can be missing.
     When predicting, it will use the 'estimator_with' for inputs with the column present
     and the 'estimator_without' for the others.
     """
 
-    def __init__(self,
-                 resilient_column: str,
-                 estimator_with: EndaEstimator,
-                 estimator_without: EndaEstimator):
-        """ Provide 2 different raw estimators ready to be trained. """
+    def __init__(
+            self,
+            resilient_column: str,
+            estimator_with: EndaEstimator,
+            estimator_without: EndaEstimator,
+    ):
+        """
+        Initialize the estimator
+        :param resilient_column: The column that can be missing, which will be taken into account by estimator_with but
+            not by estimator_without
+        :param estimator_with: An EndaEstimator that will train/predict using resilient_column
+        :param estimator_without: An EndaEstimator that will train/predict without using resilient_column
+        """
 
         if estimator_with is estimator_without:  # check identity
-            raise AttributeError("estimator_with and estimator_without must be different objects. "
-                                 "If you want the same base estimator, you can use copying tools "
-                                 " (like copy.deepcopy()) to duplicate the raw estimator.")
+            raise AttributeError(
+                "estimator_with and estimator_without must be different objects. "
+                "If you want the same base estimator, you can use copying tools "
+                " (like copy.deepcopy()) to duplicate the raw estimator."
+            )
 
+        super().__init__()
         self.resilient_column = resilient_column
         self.estimator_with = estimator_with
         self.estimator_without = estimator_without
 
-    def train(self, df: pandas.DataFrame, target_col: str):
+    def train(self, df: pd.DataFrame, target_col: str):
         """
-        Trains the two estimators : estimator_with and estimator_without the 'column_name'
+        Trains the two estimators : estimator_with and estimator_without the resilient_column
+        :param df: The input data for training
+        :param target_col: The column to predict
         """
 
         # only train the "estimator_with" where resilient_column is present (not NA)
         self.estimator_with.train(df.dropna(subset=[self.resilient_column]), target_col)
         # train the "estimator_without" without resilient_column
-        self.estimator_without.train(df.drop(columns=[self.resilient_column]), target_col)
-
-    def predict_both(self, df: pandas.DataFrame, target_col: str):
-        df_with = df[df[self.resilient_column].notna()]  # only keeps rows where resilient_column is not NaN
+        self.estimator_without.train(
+            df.drop(columns=[self.resilient_column]), target_col
+        )
+
+        # store the training
+        self._training_df = df
+        self._target = target_col
+
+    def predict_both(
+            self, df: pd.DataFrame, target_col: str
+    ) -> (pd.DataFrame, pd.DataFrame):
+        """
+        Makes predictions with both estimators: estimator_with and estimator_without the resilient_column
+        :param df: The input data for prediction
+        :param target_col: The column to predict
+        :return: A tuple with two DataFrames, the first one being the prediction with the resilient_column and the
+            second one without
+        """
+        df_with = df[
+            df[self.resilient_column].notna()
+        ]  # only keeps rows where resilient_column is not NaN
         prediction_with = self.estimator_with.predict(df_with, target_col)
         if prediction_with.shape[0] != df.shape[0]:
             # make estimator_with predict NaN where resilient_column is Nan :
-            prediction_with = prediction_with.reindex(df.index)  # adds rows with NaN values
+            prediction_with = prediction_with.reindex(
+                df.index
+            )  # adds rows with NaN values
 
         if (prediction_with.index != df.index).any():
-            raise ValueError("prediction_with must have the same index as given df. "
-                             "Check that self.estimator_with.predict conserves index.")
+            raise ValueError(
+                "prediction_with must have the same index as given df. "
+                "Check that self.estimator_with.predict conserves index."
+            )
 
         df_without = df.drop(columns=[self.resilient_column])
         prediction_without = self.estimator_without.predict(df_without, target_col)
 
         if (prediction_without.index != df.index).any():
-            raise ValueError("prediction_without must have the same index as given df. "
-                             "Check that self.estimator_without.predict conserves index.")
+            raise ValueError(
+                "prediction_without must have the same index as given df. "
+                "Check that self.estimator_without.predict conserves index."
+            )
 
         return prediction_with, prediction_without
 
-    def predict(self, df: pandas.DataFrame, target_col: str) -> pandas.DataFrame:
+    def predict(self, df: pd.DataFrame, target_col: str) -> pd.DataFrame:
+        """
+        Makes a prediction with both estimators, takes prediction by estimator_with by default and fallbacks to
+        estimator_without when it is not available
+        :param df: The input data for prediction
+        :param target_col: The column to predict
+        :return: The final prediction combining both estimators
+        """
         predict_with, predict_without = self.predict_both(df, target_col)
 
         # keep prediction with column_name when available, else take the prediction of the estimator without it
-        result = predict_with[target_col].fillna(predict_without[target_col])  # pandas series
+        result = predict_with[target_col].fillna(
+            predict_without[target_col]
+        )  # pandas series
         result = result.to_frame(target_col)
         return result
 
+    def get_model_params(self) -> dict:
+        """
+        Get model parameters of estimator_with and estimator_without.
+        The principle is to store the model params as a dict with two entries, estimator_with, and estimator_without
+        Each of these entries contains a dictionary as well, with the model params as a key, and model parameters
+        as values.
+        :return: A dictionary with one entry per model and associated parameters
+        """
+        return {self.get_model_name(): {"estimator_with": self.estimator_with.get_model_params(),
+                                        "estimator_without": self.estimator_without.get_model_params()
+                                        }
+                }
+
+    def get_all_model_names(self) -> dict[str, list[str]]:
+        """
+        Get names of sub-model in a dictionary.
+        in a dictionary with two entries, "estimator_with" and "estimator_without"
+        """
+
+        return {"estimator_with": [self.estimator_with.get_model_name()],
+                "estimator_without": [self.estimator_without.get_model_name()]}
+
 
 class EndaEstimatorRecopy(EndaEstimator):
     """
     This estimator is used to recopy the information
-    It is notably used to predict the production of river power plants, for which no 
-    artificial intelligence is relevant. 
-    It simply recopies the most recent data on a daily basis. 
+    It is notably used to predict the production of river power plants, for which no
+    artificial intelligence is relevant.
+    It simply recopies the most recent data on a daily basis.
     """
 
-    def __init__(self, period: [str, pandas.Timedelta] = None, key_col: str = None):
-
-        '''
+    def __init__(self, period: [str, pd.Timedelta] = None):
+        """
         Set up the attribute data that will store the dataframe
         :param period: The period on which past data should be averaged to be used as future value.
-                       It must be convertible to a pandas.Timedelta object, eg '1D', '2H', etc...
-                       If nothing is provided, the last past value is used in the future    
-        '''
-        self.period = pandas.to_timedelta(period) if period is not None else None
+                       It must be convertible to a pd.Timedelta object, eg '1D', '2H', etc...
+                       If nothing is provided, the last past value is used in the future
+        """
+        super().__init__()
+        self.period = pd.to_timedelta(period) if period is not None else None
         self.training_data = None
-    
-    def train(self, df: pandas.DataFrame, target_col: str):
-        '''
+
+    def train(self, df: pd.DataFrame, target_col: str):
+        """
         This function keeps the more recent data of the input dataframe,
-        and stores it in the attribute training_data. If a period has been 
-        given to the estimator constructor, it is used to define a period on 
-        which to average the data. 
+        and stores it in the attribute training_data. If a period has been
+        given to the estimator constructor, it is used to define a period on
+        which to average the data.
 
         :param df: The input dataframe, with a single DatetimeIndex
-        :param target_col: the target column 
-        '''
+        :param target_col: the target column
+        """
 
-        if type(df.index) != pandas.DatetimeIndex:
+        if not isinstance(df.index, pd.DatetimeIndex):
             raise ValueError("Index should be of type DatetimeIndex")
 
-        if target_col not in df.columns: 
-            raise ValueError(f"Target column {target_col} not found in the training dataframe")
-            
+        if target_col not in df.columns:
+            raise ValueError(
+                f"Target column {target_col} not found in the training dataframe"
+            )
+
         if self.period is None:
-            self.training_data = (
-                df.sort_index()
-                  .iloc[-1, df.columns.get_indexer([target_col])]
-                )
-            
+            self.training_data = df.sort_index().iloc[
+                -1, df.columns.get_indexer([target_col])
+            ]
+
         else:
             # the training dataframe must have a well-defined frequency
-            self.training_data = (
-                df.iloc[df.index > df.index.max() - self.period, 
-                        df.columns.get_indexer([target_col])
-                        ]
-                .mean()
-                )     
+            self.training_data = df.iloc[
+                df.index > df.index.max() - self.period,
+                df.columns.get_indexer([target_col]),
+            ].mean()
+
+        # store the training
+        self._training_df = df
+        self._target = target_col
 
-    def predict(self, df: pandas.DataFrame, target_col: str):
-        '''
+    def predict(self, df: pd.DataFrame, target_col: str) -> pd.DataFrame:
+        """
         Make a prediction just copying the retained information.
-        :param df: The input forecast dataframe, with a single DatetimeIndex 
-        :param target_col: the target column 
-        '''
+        :param df: The input forecast dataframe, with a single DatetimeIndex
+        :param target_col: the target column
+        """
 
-        if self.training_data is None: 
-            raise ValueError("There is no training dataset defined. Must call 'train' before 'predict'")
+        if self.training_data is None:
+            raise ValueError(
+                "There is no training dataset defined. Must call 'train' before 'predict'"
+            )
 
         if not isinstance(df.index, type(self.training_data.index)):
-            raise ValueError("Forecast dataset index should be of same type of input dataset")
-           
+            raise ValueError(
+                "Forecast dataset index should be of same type of input dataset"
+            )
+
         df_predict = df.copy(deep=True)
-        
+
         df_predict[target_col] = self.training_data[target_col]
-        
+
         return df_predict.loc[:, [target_col]]
+
+    def get_model_params(self) -> dict:
+        """
+        Get model parameters of estimator_with and estimator_without
+        :return: A dictionary with one entry per model and associated parameters
+        """
+        return {self.__class__.__name__: {'period': self.period}}
```

### Comparing `enda-0.0.8/enda/ml_backends/h2o_estimator.py` & `enda-1.0.1/enda/ml_backends/h2o_estimator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,27 @@
-import pandas
-from enda.estimators import EndaEstimator
+"""This script contains a wrapper for H20 estimators"""
+
 import os
-import tempfile
 import shutil
+import tempfile
 import warnings
 
+import pandas
+import pandas as pd
+
+from enda.estimators import EndaEstimator
+
 try:
     import h2o
     import h2o.exceptions
-except ImportError:
-    raise ImportError("h2o is required is you want to use this enda's H2OEstimator. "
-                      "Try: pip install h2o>=3.32.0.3")
+except ImportError as exc:
+    raise ImportError(
+        "h2o is required is you want to use this enda's H2OEstimator. "
+        "Try: pip install h2o>=3.32.0.3"
+    ) from exc
 
 
 class EndaH2OEstimator(EndaEstimator):
     """
     This is a wrapper around any H2O estimator (or anything with the same train/predict methods).
     H2OEstimator implements enda's ModelInterface.
 
@@ -24,72 +31,137 @@
 
     H2O saves model data on the h2o server, so we cannot simply use pickle/joblib out of the box for these
     objects. So we have methods for that.
 
     """
 
     def __init__(self, h2o_estimator):
+        super().__init__()
         self.model = h2o_estimator
         self.__model_binary = None
 
-    def train(self, df: pandas.DataFrame, target_col: str):
-        x = [c for c in df.columns if c != target_col]  # for H20, x is the list of features
-        y = target_col  # for H20, y is the name of the target
-        training_frame = h2o.H2OFrame(df)  # H20 training frame containing both features and target
-        self.model.train(x, y, training_frame)
-
-    def predict(self, df: pandas.DataFrame, target_col: str):
+    def train(self, df: pandas.DataFrame, target_col: str, **kwargs):
+        """
+        Train a h2o-based model from an input dataframe with features and a target column
+        :param df: the input dataframe
+        :param target_col: the target column name
+        """
+        feature_list = [
+            c for c in df.columns if c != target_col
+        ]  # for H20, x is the list of features
+        training_frame = h2o.H2OFrame(
+            df
+        )  # H20 training frame containing both features and target
+        self.model.train(feature_list, target_col, training_frame, **kwargs)
+
+        # store the training
+        self._training_df = df
+        self._target = target_col
+
+    def predict(self, df: pandas.DataFrame, target_col: str, **kwargs):
+        """
+        Predict from a h2o-based trained model using an input dataframe with features
+        :param df: the input dataframe
+        :param target_col: the target column name
+        :return: a single-column dataframe with the predicted target
+        """
         test_data = h2o.H2OFrame(df)  # convert to H20 Frame
-        forecast = self.model.predict(test_data)  # returns an H20Frame named 'predict'
-        forecast = forecast.as_data_frame().rename(columns={'predict': target_col})  # convert to pandas and rename
-        forecast.index = df.index  # put back the correct index (typically a pandas.DatetimeIndex)
+        forecast = self.model.predict(test_data, **kwargs)  # returns an H20Frame named 'predict'
+        with h2o.utils.threading.local_context(polars_enabled=True, datatable_enabled=True):
+            forecast = forecast.as_data_frame().rename(
+                columns={"predict": target_col}  # convert to pandas and rename
+            )
+        forecast.index = (
+            df.index
+        )  # put back the correct index (typically a pandas.DatetimeIndex)
         return forecast
 
-    # All below is just for model persistence : to comply with pickle and deepcopy.
-
-    __tmp_file_path_1 = os.path.join(tempfile.gettempdir(), "__h2o_estimator_tmp_file_1_136987")
-    __tmp_file_path_2 = os.path.join(tempfile.gettempdir(), "__h2o_estimator_tmp_file_2_136987")
+    def get_model_name(self) -> str:
+        """
+        Return the H2O model name instead of EndaH2OEstimator
+        """
+        return self.model.__class__.__name__
+
+    def get_model_params(self) -> dict:
+        """
+        Return a dict with the model name and the model hyperparameters
+        """
+        return {self.get_model_name(): self.model.get_params()}
+
+    def get_feature_importance(self) -> pd.Series:
+        """
+        Return the feature's importance once a model has been trained.
+        This makes use of built-in method 'varimp' of an H2OEstimator,
+        and only returns the percentage column
+        :return: a series that contain the percentage of importance for each variable
+        """
+
+        feature_importance_series = (
+            self.model.varimp(use_pandas=True)
+            .loc[:, ['variable', 'percentage']]
+            .rename(columns={'percentage': 'variable_importance_pct'})
+            .set_index('variable')
+            .rename_axis(None, axis=0)
+            .astype(float)
+            .squeeze()
+        )
+
+        return feature_importance_series
+
+        # All below is just for model persistence : to comply with pickle and deepcopy.
+
+    __tmp_file_path_1 = os.path.join(
+        tempfile.gettempdir(), "__h2o_estimator_tmp_file_1_136987"
+    )
+    __tmp_file_path_2 = os.path.join(
+        tempfile.gettempdir(), "__h2o_estimator_tmp_file_2_136987"
+    )
 
     @staticmethod
     def __h2o_model_to_binary(h2o_model):
-
         # save h2o model to tmp file
         try:
-            model_path_from_h2o = h2o.save_model(h2o_model, path=EndaH2OEstimator.__tmp_file_path_1, force=True)
-        except (h2o.exceptions.H2OResponseError, TypeError) as e:
-            raise ValueError("Problem getting the model from h2o server. Train the model first. "
-                             "Cannot access model binary before training (for pickle or deepcopy or other uses).", e)
-        
+            model_path_from_h2o = h2o.save_model(
+                h2o_model, path=EndaH2OEstimator.__tmp_file_path_1, force=True
+            )
+        except (h2o.exceptions.H2OResponseError, TypeError) as exception:
+            raise ValueError(
+                "Problem getting the model from h2o server. Train the model first. "
+                "Cannot access model binary before training (for pickle or deepcopy or other uses)."
+            ) from exception
+
         # model can be saved in __tmp_file_path_1, or in private/__tmp_file_path_1
-        potential_startswith = [EndaH2OEstimator.__tmp_file_path_1, 
-                                "/private" + EndaH2OEstimator.__tmp_file_path_1]
+        potential_startswith = [
+            EndaH2OEstimator.__tmp_file_path_1,
+            "/private" + EndaH2OEstimator.__tmp_file_path_1,
+        ]
         if not model_path_from_h2o.startswith(tuple(potential_startswith)):
-            warnings.warn("Expected model_path_from_h2o={} to start with {}"
-                          .format(model_path_from_h2o, EndaH2OEstimator.__tmp_file_path_1))
+            warnings.warn(
+                f"Expected model_path_from_h2o={model_path_from_h2o} to start with {EndaH2OEstimator.__tmp_file_path_1}"
+            )
 
         # last step actually made a folder and a file inside (at path 'model_path_from_h2o')
         # but we must keep the file inside to read it later,
         # else reading the model later based on the folder does not work despite what H2O docs say
         shutil.move(model_path_from_h2o, EndaH2OEstimator.__tmp_file_path_2)
         shutil.rmtree(EndaH2OEstimator.__tmp_file_path_1)
 
         # read the tmp file as binary
-        with open(EndaH2OEstimator.__tmp_file_path_2, mode='rb') as file:
+        with open(EndaH2OEstimator.__tmp_file_path_2, mode="rb") as file:
             binary = file.read()
 
         # cleanup tmp file
         os.remove(EndaH2OEstimator.__tmp_file_path_2)
 
         return binary
 
     @staticmethod
     def __h2o_model_from_binary(binary):
-
         # save binary to tmp file
-        with open(EndaH2OEstimator.__tmp_file_path_2, mode='wb') as file:
+        with open(EndaH2OEstimator.__tmp_file_path_2, mode="wb") as file:
             file.write(binary)
 
         # load H2O model from the file
         h2o_model = h2o.upload_model(path=EndaH2OEstimator.__tmp_file_path_2)
 
         # cleanup tmp file
         os.remove(EndaH2OEstimator.__tmp_file_path_2)
@@ -98,15 +170,15 @@
 
     def __getstate__(self):
         # for pickle, see https://docs.python.org/3/library/pickle.html#pickle-state
 
         self.__model_binary = EndaH2OEstimator.__h2o_model_to_binary(self.model)
         state = self.__dict__.copy()
         # Remove the un-picklable entry : 'model', but keep the picklable entry: __model_binary
-        del state['model']
+        del state["model"]
         return state
 
     def __setstate__(self, state):
         # for pickle, see https://docs.python.org/3/library/pickle.html#pickle-state
 
         self.__dict__.update(state)  # loads only __model_binary
         self.model = EndaH2OEstimator.__h2o_model_from_binary(self.__model_binary)
```

### Comparing `enda-0.0.8/enda/power_predictor.py` & `enda-1.0.1/enda/power_predictor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,138 +1,153 @@
+"""A class that handles day-ahead power prediction"""
+
 import copy
+
 import pandas as pd
+
 from enda.estimators import EndaEstimator
 
 
-class PowerPredictor():
+class PowerPredictor:
     """
-    This class handles the day-ahead power prediction. 
-    It access the train() and predict() methods of an EndaEstimator object. 
-    We have the possibility to apply a standard power plant method 
-    considering all observations to be occurences of the same theoretical plant
-    under different conditions (eg. meteo, or installed kw). 
-    This is applied for solar and wind plants notably. 
-    We also have the possibility to treat each plant independently. Even if 
-    this is less interesting when applying an usual IA algorithm, this option 
+    This class handles the day-ahead power prediction.
+    It accesses the train() and predict() methods of an EndaEstimator object.
+    We have the possibility to apply a standard power plant method
+    considering all observations to be occurrences of the same theoretical plant
+    under different conditions (e.g. meteo, or installed kw).
+    This is applied for solar and wind plants notably.
+    We also have the possibility to treat each plant independently. Even if
+    this is less interesting when applying a usual AI algorithm, this option
     is typically used with a naive estimator for plants along the run of rivers.
     For these plants, we simply recopy the most recent information available.
     """
 
     def __init__(self, standard_plant: bool = False):
         """
-        :param standard_plant: boolean that indicates if we want to use a 
+        :param standard_plant: boolean that indicates if we want to use a
                standard plant approach, merging all observations over the plant
-               portfolio.  
+               portfolio.
         """
-        
+
         self.standard_plant = standard_plant
         self.prod_estimators = None
-    
+
     def train(self, df: pd.DataFrame, estimator: EndaEstimator, target_col: str):
-        '''
+        """
         We provide to this function an EndaEstimator, a training dataframe (two-levels
-        multiindexed), and the target column. 
+        multi-indexed), and the target column.
 
-        To train the estimator, we have two options. In the first case, we merge all the 
-        observations for all the plants, and consider them to be simple realizations 
-        of the same single power plant with different characteristics ; that's the standard 
-        power plant model, used notably for wind and solar stations. 
-        The second option is used for power plants along river, for which no IA is required. 
-        It is a naive recopy estimator which is used. 
-        
-        The training sets self.prod_estimators as a dictionnary of stations ID - estimator
-        In case of a standard plant approach, the returned dictionary has a single entry, 
-        called "standard_plant", which becomes a reserved ID. 
+        To train the estimator, we have two options. In the first case, we merge all the
+        observations for all the plants, and consider them to be simple realizations
+        of the same single power plant with different characteristics ; that's the standard
+        power plant model, used notably for wind and solar stations.
+        The second option is used for power plants along river, for which no IA is required.
+        It is a naive recopy estimator which is used.
+
+        The training sets self.prod_estimators as a dictionary of stations ID - estimator
+        In case of a standard plant approach, the returned dictionary has a single entry,
+        called "standard_plant", which becomes a reserved ID.
 
-        :param df: the training two-levels multiindexed dataframe
-        :param estimator: an EndaEstimator that will serve as a canvas to create other 
+        :param df: the training two-levels multi-indexed dataframe
+        :param estimator: an EndaEstimator that will serve as a canvas to create other
                estimators of the same type that will be trained over each plant or over
                all of them in case of non-standard plant.
         :param target_col: the target column
-        '''
+        """
 
         if not isinstance(estimator, EndaEstimator):
             raise ValueError("Couldn't generate an estimator")
 
         if not isinstance(df.index, pd.MultiIndex):
-            raise ValueError("Prediction for power stations must be performed using "
-                             "a two-levels multi-indexed dataframe")
-        
+            raise ValueError(
+                "Prediction for power stations must be performed using "
+                "a two-levels multi-indexed dataframe"
+            )
+
         key_col = df.index.levels[0].name
         date_col = df.index.levels[1].name
-    
+
         df_train = df.copy()
 
         if self.standard_plant:
-            # we don't consider the plants individually. 
+            # we don't consider the plants individually.
             # create a dictionary with a single entry called 'standard_plant'
             # if already present, throw an error
-            if "standard_plant" in df_train.index.get_level_values(0): 
-                raise ValueError("Found a station named 'standard_plant', which is "
-                                 "a reserved name in this situation.")
-            
-            df_train = df_train.reset_index().set_index(date_col).drop(columns=[key_col])
+            if "standard_plant" in df_train.index.get_level_values(0):
+                raise ValueError(
+                    "Found a station named 'standard_plant', which is "
+                    "a reserved name in this situation."
+                )
+
+            df_train = (
+                df_train.reset_index().set_index(date_col).drop(columns=[key_col])
+            )
             estimator.train(df_train, target_col)
-            prod_estimator = copy.deepcopy(estimator)            
-            self.prod_estimators = dict() 
-            self.prod_estimators["standard_plant"] = prod_estimator
+            prod_estimator = copy.deepcopy(estimator)
+            self.prod_estimators = {"standard_plant": prod_estimator}
 
-        else: 
+        else:
             # we consider the individual plants
             # create a dictionary with the id of the plant and a dedicated estimator
-            self.prod_estimators = dict() 
+            self.prod_estimators = {}
             for station_id, data in df.groupby(level=0):
                 data = data.reset_index().set_index(date_col).drop(columns=[key_col])
                 estimator.train(data, target_col)
                 prod_estimator = copy.deepcopy(estimator)
                 self.prod_estimators[station_id] = prod_estimator
-                
-    def predict(self, 
-                df: pd.DataFrame, 
-                target_col: str, 
-                is_positive: bool = False, 
-                is_normally_clamped: bool = False):
-        '''
-        Predict target_column values once train() has been called. 
-        :param df: the forecast two-levels multiindexed dataframe
+
+    def predict(
+        self,
+        df: pd.DataFrame,
+        target_col: str,
+        is_positive: bool = False,
+        is_normally_clamped: bool = False,
+    ):
+        """
+        Predict target_column values once train() has been called.
+        :param df: the forecast two-levels multi-indexed dataframe
         :param target_col: the target column
+        :param is_positive: If True, will set negative predicted values to 0
+        :param is_normally_clamped: If True, will set negative predicted values to 0, and values higher than 1 to 1
         :return: the two-levels dataframe with the predicted target only.
-        '''
+        """
 
         if not isinstance(df.index, pd.MultiIndex):
-            raise ValueError("Prediction for power generation must be performed using "
-                             "a two-levels multi-indexed dataframe")
+            raise ValueError(
+                "Prediction for power generation must be performed using "
+                "a two-levels multi-indexed dataframe"
+            )
 
-        if self.prod_estimators is None: 
+        if self.prod_estimators is None:
             raise ValueError("The estimators have to be trained before being used.")
 
         key_col = df.index.levels[0].name
         time_col = df.index.levels[1].name
 
         df_predict = df.copy(deep=True)
 
         df_new = pd.DataFrame()
         for station_id, data in df_predict.groupby(level=0):
             data = data.reset_index().set_index(time_col).drop(columns=[key_col])
-            
+
             if self.standard_plant:
                 data = self.prod_estimators["standard_plant"].predict(data, target_col)
             else:
-                if station_id in self.prod_estimators.keys():
+                if station_id in self.prod_estimators:
                     data = self.prod_estimators[station_id].predict(data, target_col)
                 else:
                     data[target_col] = 0
                     data = data.loc[:, [target_col]]
-            
+
             if is_positive or is_normally_clamped:
                 # reset to 0 negative values
                 data.loc[(data[target_col] < 0), target_col] = 0
 
-            if is_normally_clamped: 
+            if is_normally_clamped:
                 # reset to 1 values greater than 1
                 data.loc[(data[target_col] > 1), target_col] = 1
 
             data[key_col] = station_id
             data = data.reset_index().set_index([key_col, time_col])
             df_new = pd.concat([df_new, data], axis=0)
-            
+
         return df_new
```

### Comparing `enda-0.0.8/enda/power_stations.py` & `enda-1.0.1/enda/power_stations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,449 +1,568 @@
+"""This module contains functions to handle power stations data"""
+
 import numpy as np
 import pandas as pd
-from pandas.api.types import is_string_dtype
-from enda.timeseries import TimeSeries
+
 from enda.contracts import Contracts
+from enda.tools.portfolio_tools import PortfolioTools
+from enda.tools.timezone_utils import TimezoneUtils
+import enda.tools.decorators
 
 
 class PowerStations:
     """
     A class to help handle power_stations data.
 
     Columns [time, id] are required (names can differ), and with dtype=datetime64 (tz-naive).
     Other columns describe power_station characteristics (used as features).
 
-    All functions are meant to handle a set of station datapoints, that are considered as 
-    records (samples) for the power plant algorithms. 
+    All functions are meant to handle a set of station datapoints, that are considered as
+    records (samples) for the power plant algorithms.
     """
 
     # ------ Check
 
     @classmethod
-    def check_stations(cls, df, station_col, date_start_col, date_end_exclusive_col, is_naive=True):
-        '''
-        Check there is no NaN for date_start and power station id. 
-        Check the same timestamp is not used twice for the same power plant. 
-        Check the date starts and date end
-        '''
-        
+    def check_stations(
+        cls,
+        df: pd.DataFrame,
+        station_col: str,
+        date_start_col: str,
+        date_end_exclusive_col: str,
+        is_naive: bool = True,
+    ):
+        """
+        - Checks that station_col is in the DataFrame and has no NaN
+        - Checks that there are no duplicate timestamps for a power plant.
+        - Checks that date_start is not null and that it is before date_end when present
+        :param df: The DataFrame to check
+        :param station_col: The name of the plant identifier column
+        :param date_start_col: The name of the column containing contracts start dates
+        :param date_end_exclusive_col: The name of the column containing contracts exclusive end dates
+        :param is_naive: Whether date_start_col and date_end_exclusive_col are supposed to contain naïve Timestamps
+            (raises an error if it doesn't match)
+        """
+
         if station_col not in df.columns:
             raise ValueError(f"Required column not found : {station_col}")
         if df[station_col].isna().any():
             rows_with_nan_time = df[df[station_col].isna()]
-            raise ValueError(f"There are NaN values for {station_col} in these rows:\n"
-                             f"{rows_with_nan_time}")
-        
-        rows_with_duplicates = df.duplicated([station_col, date_start_col])   
+            raise ValueError(
+                f"There are NaN values for {station_col} in these rows:\n"
+                f"{rows_with_nan_time}"
+            )
+
+        rows_with_duplicates = df.duplicated([station_col, date_start_col])
         if rows_with_duplicates.any():
-            raise ValueError(f"Duplicated station_col date_col for these rows:\n"
-                             f"{df[rows_with_duplicates]}")
-        
+            raise ValueError(
+                f"Duplicated station_col date_col for these rows:\n"
+                f"{df[rows_with_duplicates]}"
+            )
+
         # Check date start and end using Contracts
-        Contracts.check_contracts_dates(df, date_start_col, date_end_exclusive_col, is_naive)
+        Contracts.check_contracts_dates(
+            df, date_start_col, date_end_exclusive_col, is_naive
+        )
 
     # ------ Build daily dataframes
 
-    @staticmethod
-    def __station_to_events(stations, date_start_col, date_end_exclusive_col):
-        '''
-        This function is basically the same as Contracts.__contract_to_event()
-        '''
-
-        # check that no column is named "event_type" or "event_date"
-        for c in ["event_type", "event_date"]:
-            if c in stations.columns:
-                raise ValueError("stations has a column named {}, but this name is reserved in this"
-                                 "function; rename your column.".format(c))
-
-        columns_to_keep = [c for c in stations.columns if c not in [date_start_col, date_end_exclusive_col]]
-        events_columns = ["event_type", "event_date"] + columns_to_keep
-
-        # compute "station start" and "station end" events
-        start_station_events = stations.copy(deep=True)  # all stations must have a start date
-        start_station_events["event_type"] = "start"
-        start_station_events["event_date"] = start_station_events[date_start_col]
-        start_station_events = start_station_events[events_columns]
-
-        # for "station end" events, only keep stations with an end date (NaT = station is not over)
-        end_station_events = stations[stations[date_end_exclusive_col].notna()].copy(deep=True)
-        end_station_events["event_type"] = "end"
-        end_station_events["event_date"] = end_station_events[date_end_exclusive_col]
-        end_station_events = end_station_events[events_columns]
-
-        # concat all events together and sort them chronologically
-        all_events = pd.concat([start_station_events, end_station_events])
-        all_events.sort_values(by=["event_date", "event_type"], inplace=True)
-
-        return all_events
-
     @classmethod
     def get_stations_daily(
-            cls, 
-            stations, 
-            station_col="station",
-            date_start_col="date_start",
-            date_end_exclusive_col="date_end_exclusive",
-            max_date_exclusive=None
-    ): 
-        '''
+        cls,
+        stations: pd.DataFrame,
+        station_col: str = "station",
+        date_start_col: str = "date_start",
+        date_end_exclusive_col: str = "date_end_exclusive",
+        max_date_exclusive: pd.Timestamp = None,
+        drop_gaps=False,
+    ) -> pd.DataFrame:
+        """
         This function creates a daily dataframe from a power station contracts dataframe.
         It checks the provided dataframe is consistent (dates)
-        '''
+        :param stations: The DataFrame containing station information
+        :param station_col: The column containing station name
+        :param date_start_col: The column containing start date information
+        :param date_end_exclusive_col: The column containing exclusive end date information
+        :param max_date_exclusive: A Timestamp indicating the maximum date until which to keep data. This is
+            mainly useful if you have contracts with no specified end date, as they will not be taken into account by
+            default.
+        :param drop_gaps: if True, will drop daily values that are gaps within the range of input contracts.
+            By default, these days are kept in the index with 0 as values
+            (For example, if we have a station with a first contract from 2023-01-01 to 2023-02-01 and a second
+            contract from 2023-03-01 to 2023-06-01, the period from 2023-02-01 to 2023-03-01 will be kept by default
+            with 0s for all values)
+        :return: A DataFrame with daily station information
+        """
 
         for c in ["date", "event_date"]:
             if c in stations.columns:
-                raise ValueError("stations has a column named {}, but this name is reserved in this"
-                                 "function; rename your column.".format(c))
+                raise ValueError(
+                    f"stations has a column named {c}, but this name is reserved in this"
+                    "function; rename your column."
+                )
+
+        cls.check_stations(
+            stations, station_col, date_start_col, date_end_exclusive_col
+        )
 
-        cls.check_stations(stations, station_col, date_start_col, date_end_exclusive_col)
-        
         # get an event-like dataframe
-        events = cls.__station_to_events(stations, date_start_col, date_end_exclusive_col)
+        events = PortfolioTools.portfolio_to_events(
+            stations, date_start_col, date_end_exclusive_col
+        )
 
         # remove events after max_date if they are not wanted
         if max_date_exclusive is not None:
             events = events[events["event_date"] <= max_date_exclusive]
 
-        other_columns = set(stations.columns) - set([station_col, date_start_col, date_end_exclusive_col])
+            # For stations where the last event before max_date_exclusive is a start, it means that a contract is still
+            # active at the time of max_date_exclusive. We add a 'fake' end for these contracts so that daily data is
+            # computed until max_date_exclusive (otherwise there would be no row to ffill to)
+            last_event_df = events.copy()
+            last_event_df = last_event_df.groupby(station_col).last().reset_index()
+            last_event_df = last_event_df.loc[last_event_df.event_type == "start"]
+            last_event_df["event_type"] = 'end'
+            last_event_df["event_date"] = max_date_exclusive
+
+            events = pd.concat([events, last_event_df])
+
+        other_columns = set(stations.columns) - {
+            station_col,
+            date_start_col,
+            date_end_exclusive_col,
+        }
         for c in other_columns:
-            events[c] = events.apply(lambda row: row[c] if row["event_type"] == "start" else 0, axis=1)
-        
+            events[c] = events.apply(
+                lambda row: row[c] if row["event_type"] == "start" else 0, axis=1
+            )
+
+        if drop_gaps:
+            if "control_column" in events.columns:
+                raise ValueError(
+                    "control_column should not be one of the columns in the events DataFrame, it is used"
+                    "in this function"
+                )
+
+            # We create a control column which is used to keep only days included in the events DataFrame period
+            events["control_column"] = "0"
+            events.loc[events.event_type == "start", "control_column"] = "control"
+
         events = events.groupby([station_col, "event_date"]).last().reset_index()
         events = events.drop(columns=["event_type"])
 
-        # iterate over a partition of the dataframe (each station) to resample 
-        # at a daily frequency, using a backfill of the dates. 
+        # iterate over a partition of the dataframe (each station) to resample
+        # at a daily frequency, using a backfill of the dates.
         df = pd.DataFrame()
-        for station, station_contracts in events.groupby(station_col):
-            station_contracts = station_contracts.set_index("event_date").asfreq('D', method='ffill')
+        for _, station_contracts in events.groupby(station_col):
+            station_contracts = station_contracts.set_index("event_date").asfreq(
+                "D", method="ffill"
+            )
             station_contracts = station_contracts.iloc[:-1]
             df = pd.concat([df, station_contracts], axis=0)
-        
+
         df.index.name = "date"
+
+        if drop_gaps:
+            # The way we compute a daily DataFrame, there is a problem if there is a gap between an end event and the
+            # next start event : for example, if a contract line ends on 2022 December 31st and next one begins on
+            # 2024 January 1st, the days in 2023 will still be present in df_daily_pf.
+            # However, the columns other than plant identification column will have '0' as a value,
+            # so using this control column we can keep only relevant dates.
+            df = df.loc[df.control_column == "control"]
+            df.drop("control_column", axis=1, inplace=True)
+
         return df.reset_index().set_index([station_col, "date"])
 
     @staticmethod
+    @enda.tools.decorators.warning_deprecated_name(
+        namespace_name="PowerStations",
+        new_namespace_name="PortfolioTools",
+        new_function_name="get_portfolio_between_dates",
+    )
     def get_stations_between_dates(
-            stations,
-            start_datetime, 
-            end_datetime_exclusive, 
-            freq=None
-            ):
+        stations: pd.DataFrame,
+        start_datetime: pd.Timestamp,
+        end_datetime_exclusive: pd.Timestamp,
+        freq: str = None,
+    ) -> pd.DataFrame:
         """
         Adds or removes dates if needed.
 
         If additional dates needed at the end, copy the data of the last date into the additional dates
 
-        :param stations: the dataframe with the stations. It must be a MultiIndex datframe,
+        :param stations: the dataframe with the stations. It must be a MultiIndex DataFrame,
                          whose second order index is a pandas.DatetimeIndex with frequency.
         :param start_datetime: the start date column, it is the same for all stations
         :param end_datetime_exclusive: the end date (exclusive)
-        :return: a station portfolio with characteristics between date_start and date_end. 
+        :param freq: The frequency of the DataFrame (ex: '30min'). If not specified, the function will try to infer it
+        :return: a station portfolio with characteristics between date_start and date_end.
         """
 
-        df = stations.copy()
+        return PortfolioTools.get_portfolio_between_dates(
+            portfolio_df=stations,
+            start_datetime=start_datetime,
+            end_datetime_exclusive=end_datetime_exclusive,
+            freq=freq,
+        )
 
-        if not isinstance(df.index, pd.MultiIndex):
-            raise TypeError("daily_stations must be a MultiIndex")
+    # ------ Outages
 
-        if len(df.index.levels) != 2:
-            raise TypeError("daily_stations must be a MultiIndex with two levels (stations and date)")
-
-        if not isinstance(df.index.levels[1], pd.DatetimeIndex):
-            raise TypeError("The second index of daily_stations should be a pd.DatetimeIndex, but given {}"
-                            .format(df.index.levels[1].dtype))
-      
-        if freq is None:
-            try:
-                freq = df.index.levels[1].inferred_freq
-            except Exception:
-                raise ValueError("No freq has been provided, and it could not be inferred"
-                                 "from the index itself. Please set it or check the data.")
-
-        # check that there is no missing value
-        if not df.isnull().sum().sum() == 0:
-            raise ValueError("daily_stations has NaN values.")
-
-        key_col = df.index.levels[0].name
-        date_col = df.index.levels[1].name 
-
-        df_new = pd.DataFrame()
-        for station, data in df.groupby(level=0):
-            if start_datetime is not None and data.index.levels[1].min() > start_datetime:
-                # add days with empty portfolio at the beginning
-                data.loc[(station, start_datetime), :] = tuple([0 for x in range(len(df.columns))])
-                data.sort_index(inplace=True)  # put the new row first
-                data = data.reset_index().set_index(date_col).asfreq(freq, method='ffill')
-                data = data.reset_index().set_index([key_col, date_col])
-        
-            if end_datetime_exclusive is not None and data.index.levels[1].max() < end_datetime_exclusive:
-                # add days at the end, with the same portfolio as the last available day
-                data.loc[(station, end_datetime_exclusive), :] = tuple([0 for x in range(len(df.columns))])
-                data.sort_index(inplace=True) 
-                data = data.reset_index().set_index(date_col).asfreq(freq, method='ffill')
-                data = data.reset_index().set_index([key_col, date_col])
-            
-            # remove dates outside of desired range
-            data = data[(data.index.get_level_values(date_col) >= start_datetime) & 
-                        (data.index.get_level_values(date_col) < end_datetime_exclusive)]
-            assert data.isnull().sum().sum() == 0  # check that there is no missing value
-            
-            df_new = pd.concat([df_new, data], axis=0)
+    @staticmethod
+    def get_outages_from_file(
+        file_path: str,
+        time_start_col: str = "time_start",
+        time_end_exclusive_col: str = "time_end_exclusive",
+        tzinfo: str = "Europe/Paris",
+        pct_outages_col: str = None,
+    ):
+        """
+        Reads outages from a file. This will convert start and end date columns into dtype=datetime64 (tz-naive) and
+        check that pct_outages_col is present in the DataFrame if specified, with values between 0 and 100 when not None
+        :param file_path: where the source file is located.
+        :param time_start_col: the name of the outage time start column.
+        :param time_end_exclusive_col: the name of the outage time end column, end date is exclusive.
+        :param tzinfo: The time zone of the data we read
+        :param pct_outages_col: The percentage of unavailability of the power plant (100 means complete shutdown).
+        :return: a pandas.DataFrame with an outage on each row.
+        """
 
-        return df_new
+        outages_df = TimezoneUtils.read_csv_and_set_tz_aware_columns(
+            file_path=file_path,
+            time_cols_list=[time_start_col, time_end_exclusive_col],
+            tz_info=tzinfo
+        )
 
-    # ------ Outages
+        # check pct_outage_col
+        if pct_outages_col is not None:
+            if pct_outages_col not in outages_df.columns:
+                raise ValueError(
+                    f"Provided column {pct_outages_col} is not present in dataframe"
+                )
+            if not (outages_df[pct_outages_col].dropna().between(0, 100)).all():
+                raise ValueError(
+                    f"Some values in {pct_outages_col} are not percentages between 0 and 100"
+                )
+
+        return outages_df
 
     @classmethod
     def read_outages_from_file(
-            cls,
-            file_path,
-            station_col="station",
-            time_start_col="time_start",
-            time_end_exclusive_col="time_end_exclusive",
-            tzinfo="Europe/Paris",          
-            pct_outages_col=None
-            ):
+        cls,
+        file_path: str,
+        station_col: str = "station",
+        time_start_col: str = "time_start",
+        time_end_exclusive_col: str = "time_end_exclusive",
+        tzinfo: str = "Europe/Paris",
+        pct_outages_col: str = None,
+    ) -> pd.DataFrame:
         """
-        Reads outages from a file. This will convert start and end date columns into dtype=datetime64 (tz-naive)
+        Reads outages from a file and checks that the resulting DataFrame is coherent. This will convert start and end
+        date columns into dtype=datetime64 (tz-naive)
         :param file_path: where the source file is located.
+        :param station_col: the name of the column containing stations names
         :param time_start_col: the name of the outage time start column.
         :param time_end_exclusive_col: the name of the outage time end column, end date is exclusive.
-        :param time_format: the time format for pandas.to_datetime
-        :param pct_outages_col: the percentage of availability of the powerplant. 
-               If none is given, it is assumled the power plant is simply shutdown. 
+        :param tzinfo: The time zone of the data we read
+        :param pct_outages_col: The percentage of unavailability of the power plant (100 means complete shutdown).
         :return: a pandas.DataFrame with an outage on each row.
         """
 
-        df = pd.read_csv(file_path)
-        for c in [time_start_col, time_end_exclusive_col]:
-            if is_string_dtype(df[c]):
-                df[c] = pd.to_datetime(df[c])
-                df[c] = TimeSeries.align_timezone(df[c], tzinfo=tzinfo)
-
-        # check stations
-        cls.check_stations(df, station_col, time_start_col, time_end_exclusive_col, is_naive=False)
-        
-        # check pct_outage_col
-        if pct_outages_col is not None:
-            if pct_outages_col not in df.columns:
-                raise ValueError(f"Provided column {pct_outages_col} is not present in dataframe")
-            if not (df[pct_outages_col].dropna().between(0, 100)).all(): 
-                raise ValueError(f"Some values in {pct_outages_col} are not percentage")    
-        
+        # Read the data and convert time columns to the correct type
+        df = cls.get_outages_from_file(
+            file_path, time_start_col, time_end_exclusive_col, tzinfo, pct_outages_col
+        )
+
+        # Check that the resulting DataFrame is coherent
+        cls.check_stations(
+            df, station_col, time_start_col, time_end_exclusive_col, is_naive=False
+        )
+
         return df
 
     @staticmethod
     def integrate_availability_from_outages(
-            df_stations, 
-            df_outages,
-            station_col, 
-            time_start_col, 
-            time_end_exclusive_col, 
-            pct_outages_col=None,
-            availability_col=None 
-            ):
-        '''
-        This function starts from a multi-indexed dataframe with stations-timeseries. 
-        It takes another unindexed dataframe containing the detail of the shutdowns 
-        and outages for the stations. 
-        It integrates to the station-timeseries data an extra column that describe the 
-        availability of the stations.  
+        df_stations: pd.DataFrame,
+        df_outages: pd.DataFrame,
+        station_col: str,
+        time_start_col: str,
+        time_end_exclusive_col: str,
+        pct_outages_col: str = None,
+        availability_col: str = None,
+    ) -> pd.DataFrame:
+        """
+        This function starts from a multi-indexed dataframe with stations-timeseries.
+        It takes another non-indexed dataframe containing the detail of the shutdowns
+        and outages for the stations.
+        It integrates to the station-timeseries data an extra column that describe the
+        availability of the stations.
 
         Conditions:
         - The stations ID column must be present in both dataframes.
         - df_stations must have a frequency. This condition is not strictly necessary
           to integrate outages a priori, but in our applications, it's almost always the case.
         - df_outages must have time_start/time_end fields (the length of the shutdown).
 
-        :param df_stations: the dataframe which contains the stations features as timeseries
-        :param df_outages: the outages unindexed dataframe
-        :station_col: the ID of the stations
-        :time_start_col: the start time of the outage
-        :time_end_exclusive_col: the end time of the outage
-        :pct_outage_col: name of the outage column.
-        :availability_col: name of the availability column in the new dataframe
-        '''
+        :param df_stations: The DataFrame which contains the stations features as timeseries
+        :param df_outages: The non-indexed outages DataFrame
+        :param station_col: The column containing the station identifier
+        :param time_start_col: The column containing the start time of the outage
+        :param time_end_exclusive_col: The column containing the exclusive end time of the outage
+        :param pct_outages_col: The column containing the information of outage impact on capacity.
+            If a null value is given, it is assumed the power plant is simply shutdown.
+        :param availability_col: The name of the availability column in the new DataFrame
+        """
 
         # check df_stations
         if not isinstance(df_stations.index, pd.MultiIndex):
-            raise TypeError("stations must be multiindexed dataframe")
-    
+            raise TypeError("stations must be multi-indexed dataframe")
+
         if len(df_stations.index.levels) != 2:
-            raise TypeError("The provided multi-indexed dataframe must be a two-levels one")
-    
+            raise TypeError(
+                "The provided multi-indexed dataframe must be a two-levels one"
+            )
+
         if not isinstance(df_stations.index.levels[1], pd.DatetimeIndex):
-            raise TypeError("The second index of the dataframe should be a pd.DatetimeIndex, "
-                            f"but {df_stations.index.levels[1].dtype} is found")
-        
+            raise TypeError(
+                "The second index of the dataframe should be a pd.DatetimeIndex, "
+                f"but {df_stations.index.levels[1].dtype} is found"
+            )
+
         # check df_outages
         if station_col not in df_outages.columns:
             raise ValueError(f"Station column {station_col} is not present in outages")
-            
+
         if time_start_col not in df_outages.columns:
-            raise ValueError(f"Time start column {time_start_col} is not present in outages")
-            
+            raise ValueError(
+                f"Time start column {time_start_col} is not present in outages"
+            )
+
         if time_end_exclusive_col not in df_outages.columns:
-            raise ValueError(f"Time end column {time_end_exclusive_col} is not present in outages")
+            raise ValueError(
+                f"Time end column {time_end_exclusive_col} is not present in outages"
+            )
 
-        # reset the availability column 
+        # reset the availability column
         if availability_col is None:
-            if 'availability' in df_stations.columns: 
-                raise ValueError("'availability' is a reserved keyword for this function")
-            availability_col = 'availability'
+            if "availability" in df_stations.columns:
+                raise ValueError(
+                    "'availability' is a reserved keyword for this function"
+                )
+            availability_col = "availability"
 
         df_stations = df_stations.copy()
         df_stations[availability_col] = 1
 
         # loop over outages to set the availability
-        for index, outage in df_outages.iterrows():
-            mask = (df_stations.index.get_level_values(0) == outage[station_col])\
-                   & (df_stations.index.get_level_values(1) >= outage[time_start_col])\
-                   & (df_stations.index.get_level_values(1) < outage[time_end_exclusive_col])
-            
-            availability = 0 if outage[pct_outages_col] is None else 1 - (outage[pct_outages_col] / 100.)
+        for _, outage in df_outages.iterrows():
+            mask = (
+                (df_stations.index.get_level_values(0) == outage[station_col])
+                & (df_stations.index.get_level_values(1) >= outage[time_start_col])
+                & (
+                    df_stations.index.get_level_values(1)
+                    < outage[time_end_exclusive_col]
+                )
+            )
+
+            availability = (
+                0
+                if pd.isna(outage[pct_outages_col])
+                else 1 - (outage[pct_outages_col] / 100.0)
+            )
             if abs(availability) < 1e-6:
                 availability = 0
             df_stations.loc[mask, availability_col] = availability
-           
+
         return df_stations
 
     @staticmethod
     def reset_installed_capacity(
-            df, 
-            installed_capacity_kw,
-            stations_availability,
-            drop_availability=True):
-        '''
-        This function is meant to reset the installed capacity of a station using 
-        a helper column. The helper column stores number between 0 and 1 which 
-        to detail the availability of the station. 
-        :param df: the dataframe to be changed. 
-        :param installed_capacity_kw: the column of df that contains the installed_capacity in kw
-        :param load_factor_col: name of the availaibility column
+        df: pd.DataFrame,
+        installed_capacity_kw: str,
+        stations_availability: str,
+        drop_availability: bool = True,
+    ) -> pd.DataFrame:
+        """
+        This function is meant to reset the installed capacity of a station using
+        a helper column. The helper column stores number between 0 and 1 detailing
+        the availability of the station.
+        :param df: The dataframe to be changed.
+        :param installed_capacity_kw: The column of df that contains the installed_capacity in kW
+        :param stations_availability: The name of the helper column used to compute installed capacity.
+            Values should be between 0 and 1, 0 meaning a shutdown and 1 meaning full installed capacity available
         :param drop_availability: boolean flag which indicates whether the availability
-                                   column shall be dropped. 
-        '''
+                                   column shall be dropped.
+        :return: The DataFrame with corrected installed capacity
+        """
 
         for c in [installed_capacity_kw, stations_availability]:
             if c not in df.columns:
                 raise ValueError(f"Required column not found: {c}")
 
         if df[stations_availability].isna().any():
             raise ValueError(f"{stations_availability} column should not contain NaN")
 
         max_value = df[stations_availability].max()
         if df[stations_availability].max() > 1:
-            raise ValueError(f"{stations_availability} column should contain values"
-                             f" between 0 and 1, found: {max_value}")
+            raise ValueError(
+                f"{stations_availability} column should contain values"
+                f" between 0 and 1, found: {max_value}"
+            )
 
         min_value = df[stations_availability].min()
         if df[stations_availability].min() < 0:
-            raise ValueError(f"{stations_availability} column should contain values"
-                             f" between 0 and 1, found: {min_value}")
+            raise ValueError(
+                f"{stations_availability} column should contain values"
+                f" between 0 and 1, found: {min_value}"
+            )
 
         df = df.copy()
-        df[installed_capacity_kw] = df[installed_capacity_kw] * df[stations_availability]
+        df[installed_capacity_kw] = (
+            df[installed_capacity_kw] * df[stations_availability]
+        )
 
         if drop_availability:
             df = df.drop(columns=stations_availability)
 
         return df
 
     @staticmethod
     def integrate_outages(
-                df_stations, 
-                df_outages,
-                station_col, 
-                time_start_col, 
-                time_end_exclusive_col, 
-                installed_capacity_col,
-                pct_outages_col=None):
-        '''
-        This function makes successive calls to integrate_availability_from_outages() 
-        and to reset_installed_capacity(). 
-        '''
+        df_stations: pd.DataFrame,
+        df_outages: pd.DataFrame,
+        station_col: str,
+        time_start_col: str,
+        time_end_exclusive_col: str,
+        installed_capacity_col: str,
+        pct_outages_col: str = None,
+    ) -> pd.DataFrame:
+        """
+        This function makes successive calls to integrate_availability_from_outages()
+        and to reset_installed_capacity().
+
+        :param df_stations: The Dataframe which contains the stations features as timeseries
+        :param df_outages: The DataFrame containing outages information
+        :param station_col: The column containing the station identifier
+        :param time_start_col: The column containing the start time of the outage
+        :param time_end_exclusive_col: The column containing the exclusive end time of the outage
+        :param installed_capacity_col: The column containing the installed capacity in kW
+        :param pct_outages_col: The column containing the information of outage impact on capacity
+        :return: The DataFrame with corrected installed capacity
+        """
 
         # check station availability_col
-        if "availability" in df_stations.columns: 
-            raise ValueError("'availability' is a reserved keyword for this function")
+        if "availability_col" in df_stations.columns:
+            raise ValueError(
+                "'availability_col' is a reserved keyword for this function"
+            )
 
         df = PowerStations.integrate_availability_from_outages(
-                df_stations=df_stations, 
-                df_outages=df_outages,
-                station_col=station_col, 
-                time_start_col=time_start_col, 
-                time_end_exclusive_col=time_end_exclusive_col, 
-                pct_outages_col=pct_outages_col,
-                availability_col="availability_col"
-                )
-        
+            df_stations=df_stations,
+            df_outages=df_outages,
+            station_col=station_col,
+            time_start_col=time_start_col,
+            time_end_exclusive_col=time_end_exclusive_col,
+            pct_outages_col=pct_outages_col,
+            availability_col="availability_col",
+        )
+
         df = PowerStations.reset_installed_capacity(
-            df=df, 
+            df=df,
             installed_capacity_kw=installed_capacity_col,
-            stations_availability='availability_col',
-            drop_availability=True)
+            stations_availability="availability_col",
+            drop_availability=True,
+        )
 
         return df
 
     # ------ Load factor
 
     @staticmethod
     def compute_load_factor(
-            df,
-            installed_capacity_kw, 
-            power_kw, 
-            load_factor_col="load_factor",
-            drop_power_kw=True):
-        '''
-        This function computes the load_factor, which is the target column of most 
+        df: pd.DataFrame,
+        installed_capacity_kw: str,
+        power_kw: str,
+        load_factor_col: str = "load_factor",
+        drop_power_kw: bool = True,
+    ) -> pd.DataFrame:
+        """
+        This function computes the load_factor, which is the target column of most
         methods implemented for the power stations production prediction
-        :param installed_capacity_kw: the column of df that contains the installed_capacity in kw
-        :param power_kw: the column which contains the power (in kW)
-        :param load_factor_col: name of the computed load factor column
-        :param drop_power_kw: boolean flag which indicates whether the power  
-                              column shall be dropped. 
-        '''
+        :param df: The input DataFrame for computing load factor
+        :param installed_capacity_kw: The column that contains the installed_capacity in kW
+        :param power_kw: The column that contains the power (in kW)
+        :param load_factor_col: The name of the computed load factor column
+        :param drop_power_kw: A boolean flag which indicates whether the power
+                              column shall be dropped.
+        """
         df = df.copy()
 
         for c in [installed_capacity_kw, power_kw]:
             if c not in df.columns:
-                raise ValueError("Required column not found : {}".format(c))
-        
-        df[load_factor_col] = np.where(df[installed_capacity_kw] < 1e-5, 
-                                       0, 
-                                       df[power_kw] / df[installed_capacity_kw])
+                raise ValueError(f"Required column not found : {c}")
+
+        df[load_factor_col] = np.where(
+            df[installed_capacity_kw] < 1e-5,
+            0,
+            df[power_kw] / df[installed_capacity_kw],
+        )
 
         if drop_power_kw:
             df = df.drop(columns=power_kw)
 
-        return df 
+        return df
 
     @staticmethod
     def compute_power_kw_from_load_factor(
-            df,
-            installed_capacity_kw, 
-            load_factor, 
-            power_kw_col="power_kw",
-            drop_load_factor=True):
-        '''
-        This function computes the power (in kW) from the computed load_factor. 
+        df: pd.DataFrame,
+        installed_capacity_kw: str,
+        load_factor: str,
+        power_kw_col: str = "power_kw",
+        drop_load_factor: bool = True,
+    ) -> pd.DataFrame:
+        """
+        This function computes the power (in kW) from the computed load_factor.
         It is the inverse transform of compute_load_factor()
-        :param installed_capacity_kw: the column of df that contains the installed_capacity in kw
-        :param load_factor: the column which contains the load factor
-        :param power_kw_col: name of the computed power column 
-        :param drop_load_factor: boolean flag which indicates whether the load factor 
-                                 column shall be dropped. 
-        '''
+        :param df: The input DataFrame for computing power
+        :param installed_capacity_kw: The column that contains the installed_capacity in kW
+        :param load_factor: The column which contains the load factor
+        :param power_kw_col: The name of the computed power column
+        :param drop_load_factor: A boolean flag which indicates whether the load factor
+                                 column shall be dropped.
+        """
 
         df = df.copy()
         for c in [installed_capacity_kw, load_factor]:
             if c not in df.columns:
                 raise ValueError(f"Required column not found : {c}")
-        
+
         df[power_kw_col] = df[installed_capacity_kw] * df[load_factor]
 
         if drop_load_factor:
             df = df.drop(columns=load_factor)
 
-        return df 
+        return df
+
+    @staticmethod
+    def clip_column(
+            df: pd.DataFrame,
+            column_name: str,
+            lower_bound: float = None,
+            upper_bound: float = None
+    ) -> pd.DataFrame:
+        """Checks that values in the indicated colname are between the two specified bounds (bounds included).
+        If not, replaces the excessive values with the associated bounds
+        :param df: The DataFrame to use the function on
+        :param column_name: The column to check and clip
+        :param lower_bound: If not None, the lower bound that we can't go below of.
+        :param upper_bound: If not None, the upper bound that we can't go above of. Defaults to None.
+        :return: A dataframe where all the values in the specified columns are between the two bounds. If we find
+            excessive values, we set them equal to the closer bound"""
+
+        result_df = df.copy()
+
+        if lower_bound is not None:
+            result_df.loc[(result_df[column_name] < lower_bound), column_name] = lower_bound
+
+        if upper_bound is not None:
+            result_df.loc[(result_df[column_name] > upper_bound), column_name] = upper_bound
+
+        return result_df
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

