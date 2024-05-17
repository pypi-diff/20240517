# Comparing `tmp/goodpy-0.0.6-py2.py3-none-any.whl.zip` & `tmp/goodpy-0.0.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11081 bytes, number of entries: 25
+Zip file size: 12615 bytes, number of entries: 26
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 goodpy/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 goodpy/f/__init__.py
 -rw-r--r--  2.0 unx       54 b- defN 20-Feb-02 00:00 goodpy/f/date/__init__.py
 -rw-r--r--  2.0 unx      789 b- defN 20-Feb-02 00:00 goodpy/f/date/get_date_last_friday.py
 -rw-r--r--  2.0 unx       31 b- defN 20-Feb-02 00:00 goodpy/f/dict_key_and_value/__init__.py
 -rw-r--r--  2.0 unx      127 b- defN 20-Feb-02 00:00 goodpy/f/dict_key_and_value/update.py
 -rw-r--r--  2.0 unx       29 b- defN 20-Feb-02 00:00 goodpy/f/dirpath/__init__.py
@@ -12,16 +12,17 @@
 -rw-r--r--  2.0 unx       61 b- defN 20-Feb-02 00:00 goodpy/f/num1_and_num2/__init__.py
 -rw-r--r--  2.0 unx       75 b- defN 20-Feb-02 00:00 goodpy/f/num1_and_num2/check_if_greater_than.py
 -rw-r--r--  2.0 unx       43 b- defN 20-Feb-02 00:00 goodpy/f/row_and_keys/__init__.py
 -rw-r--r--  2.0 unx      205 b- defN 20-Feb-02 00:00 goodpy/f/row_and_keys/get_keys_row.py
 -rw-r--r--  2.0 unx       33 b- defN 20-Feb-02 00:00 goodpy/f/row_key_and_value/__init__.py
 -rw-r--r--  2.0 unx      355 b- defN 20-Feb-02 00:00 goodpy/f/row_key_and_value/add_key.py
 -rw-r--r--  2.0 unx        1 b- defN 20-Feb-02 00:00 goodpy/k/__init__.py
--rw-r--r--  2.0 unx     9447 b- defN 20-Feb-02 00:00 goodpy/k/dataframe.py
+-rw-r--r--  2.0 unx     9445 b- defN 20-Feb-02 00:00 goodpy/k/dataframe.py
 -rw-r--r--  2.0 unx     1539 b- defN 20-Feb-02 00:00 goodpy/k/spark_conf.py
 -rw-r--r--  2.0 unx      973 b- defN 20-Feb-02 00:00 goodpy/k/spark_context.py
 -rw-r--r--  2.0 unx      870 b- defN 20-Feb-02 00:00 goodpy/k/spark_session.py
--rw-r--r--  2.0 unx     6821 b- defN 20-Feb-02 00:00 goodpy/k/time_series_standard_scaler.py
-?rw-r--r--  2.0 unx       50 b- defN 20-Feb-02 00:00 goodpy-0.0.6.dist-info/METADATA
-?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 goodpy-0.0.6.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2114 b- defN 20-Feb-02 00:00 goodpy-0.0.6.dist-info/RECORD
-25 files, 24437 bytes uncompressed, 7601 bytes compressed:  68.9%
+-rw-r--r--  2.0 unx     6534 b- defN 20-Feb-02 00:00 goodpy/k/time_series_robust_scaler.py
+-rw-r--r--  2.0 unx     6733 b- defN 20-Feb-02 00:00 goodpy/k/time_series_standard_scaler.py
+?rw-r--r--  2.0 unx       50 b- defN 20-Feb-02 00:00 goodpy-0.0.7.dist-info/METADATA
+?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 goodpy-0.0.7.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2208 b- defN 20-Feb-02 00:00 goodpy-0.0.7.dist-info/RECORD
+26 files, 30975 bytes uncompressed, 8985 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -57,20 +57,23 @@
 
 Filename: goodpy/k/spark_context.py
 Comment: 
 
 Filename: goodpy/k/spark_session.py
 Comment: 
 
+Filename: goodpy/k/time_series_robust_scaler.py
+Comment: 
+
 Filename: goodpy/k/time_series_standard_scaler.py
 Comment: 
 
-Filename: goodpy-0.0.6.dist-info/METADATA
+Filename: goodpy-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: goodpy-0.0.6.dist-info/WHEEL
+Filename: goodpy-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: goodpy-0.0.6.dist-info/RECORD
+Filename: goodpy-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## goodpy/k/dataframe.py

```diff
@@ -108,15 +108,15 @@
     array_col_name = c(in_cols)
     s = s.add_array_col(in_cols, array_col_name)
     shifted_array_col_name = c([array_col_name] + ['shift', str(shift_size)])
     s = s.add_shifted_col(array_col_name, shift_size, shifted_array_col_name)
     shifted_col = col(shifted_array_col_name)
     cols += [shifted_col[i].alias(out_col_names[i]) for i in range(len(in_cols))]
     return DataFrame(s.select(cols), s.sparkSession)
-  
+
   # def add_ts_cols(
   #   s: Self,
   #   in_cols: list[Union[str, Column]],
   #   shift_size: int,
   #   out_col_names: list[str]
   # ) -> 'DataFrame':
   #   cols = s.columns
```

## goodpy/k/time_series_standard_scaler.py

```diff
@@ -1,21 +1,19 @@
 from goodpy.f.iterable_and_seperator.concat import f as concat
 from sklearn.preprocessing import StandardScaler as SS
 from pyspark.sql.functions import map_from_arrays
 from pyspark.testing import assertDataFrameEqual
 from goodpy.k.spark_session import SparkSession
-from pyspark.ml.linalg import DenseVector as DV
 from pyspark.ml.linalg import DenseMatrix as DM
 from pyspark.sql.types import BooleanType
 from pyspark.sql.types import IntegerType
 from pyspark.sql.types import StructField
 from goodpy.k.dataframe import DataFrame
 from pyspark.sql.types import StructType
 from pyspark.ml.linalg import MatrixUDT
-from pyspark.ml.linalg import VectorUDT
 from pyspark.sql.types import ArrayType
 from pyspark.sql.types import FloatType
 from pyspark.sql.functions import udf
 from pyspark.sql.functions import lit
 from typing_extensions import Self
 from dataclasses import dataclass
 from dataclasses import field
```

## Comparing `goodpy-0.0.6.dist-info/RECORD` & `goodpy-0.0.7.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 goodpy/f/num1_and_num2/__init__.py,sha256=6IQwo48SoTNvAQvveZho8aaFrbh2M9hQGLjXd6qNjj8,61
 goodpy/f/num1_and_num2/check_if_greater_than.py,sha256=RMnfD1UGEEVvtSG1rP3wgUr79tepprvGCkzHsHRvfks,75
 goodpy/f/row_and_keys/__init__.py,sha256=CGe-Uswik2tSH4Zph6SOLYW143AJlSo8AeO9k36aLvs,43
 goodpy/f/row_and_keys/get_keys_row.py,sha256=oXPz4Bxvuc5bt6abbd4QEL_IzydL8zq-YF8qFcKC8NU,205
 goodpy/f/row_key_and_value/__init__.py,sha256=Bg_ieuYVK61m1hZdEb5pkhpQK6ndhjTg_AL8Kd4IxiU,33
 goodpy/f/row_key_and_value/add_key.py,sha256=36dKFkdGvrpwvCUz00zYT4-f6uNxRGcukhk1cP-Ll8E,355
 goodpy/k/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-goodpy/k/dataframe.py,sha256=HtkDHQOzb-igPCsgo72ZJQhqHozTqfB-1ULmf7klbj8,9447
+goodpy/k/dataframe.py,sha256=yhyua2amTydjVtzJRkaKypciRRMqVQrE3fY5cpzNWa0,9445
 goodpy/k/spark_conf.py,sha256=h3a_qubJKHAC3-DkfvzjYgaHpf5pd3rkE-64FdkQyJM,1539
 goodpy/k/spark_context.py,sha256=V1-KtsXfzzuyXG4WMw6RGZPVygkClQvS_RXgmZnrxiM,973
 goodpy/k/spark_session.py,sha256=hmltKLoHKDae1VFBff0sF3RMq_gI3tZi1ECLIBpz66A,870
-goodpy/k/time_series_standard_scaler.py,sha256=jucJ1nbbozxNcByRlCxcEUpsmOcb0XDTRYGKhMTZDAs,6821
-goodpy-0.0.6.dist-info/METADATA,sha256=elj_qvyf7hZSf8u60VFhbCf44pCTbBvBwX_8TgnMKII,50
-goodpy-0.0.6.dist-info/WHEEL,sha256=cDcbFFSNXOE-241I5PFuLkIYfR_FM7WTlPEi33njInY,105
-goodpy-0.0.6.dist-info/RECORD,,
+goodpy/k/time_series_robust_scaler.py,sha256=-lerOR2zEFG-kuPktB4IKg47VM632q928r_jbhuMbao,6534
+goodpy/k/time_series_standard_scaler.py,sha256=hh3SLXzKrLd1VH47uDjf6l8NJqQtXXGuDhmQHDu2Guo,6733
+goodpy-0.0.7.dist-info/METADATA,sha256=odCvTldnDIuVYNZgmwwFGk-Jq3JSptVGN72rkfR1GsQ,50
+goodpy-0.0.7.dist-info/WHEEL,sha256=cDcbFFSNXOE-241I5PFuLkIYfR_FM7WTlPEi33njInY,105
+goodpy-0.0.7.dist-info/RECORD,,
```

