# Comparing `tmp/zetl-3.4.0.tar.gz` & `tmp/zetl-3.4.1.tar.gz`

## Comparing `zetl-3.4.0.tar` & `zetl-3.4.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 zetl-3.4.0/PyPI-Recovery-Codes-iamthedave-2024-04-29T14_24_52.946204.txt
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 zetl-3.4.0/testszetl_pythonscript_temp.log
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/.schemawiz_config3
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/1.CURRENT_DATE.sql
--rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/BMONAS-Finalresend.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/__init__.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/common.py
--rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/local_sqlite_db
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/menu.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/mysql_export.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/mysql_extract.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/mysql_import.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/postgres_export.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/postgres_extract.py
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/postgres_import.py
--rw-r--r--   0        0        0    29992 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/run.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/sample.csv
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/sample7.csv
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/sqlite_export.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/sqlite_extract.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/sqlite_import.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/view.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/z.sample8.ddl
--rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl.db
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_this_file.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_this_folder.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl1/0.init.sql
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl1/10.version_check.sql
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl1/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl1 - Copy/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl1 - Copy/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl2/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl2/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl2 - Copy/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl2 - Copy/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl3/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl3/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl3 - Copy/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl3 - Copy/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl4/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl4/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl4 - Copy/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl4 - Copy/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl4 - Copy - Copy/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl4 - Copy - Copy/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl4 - Copy - Copy (2)/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/etl4 - Copy - Copy (2)/z_etl.csv
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/test/1.another_mysqlcheck.sql
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/test/another_postgrescheck.sql
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/test/check.sql
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/test/postgrescheck.sql
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 zetl-3.4.0/src/zetl/zetl_scripts/test/z_etl.csv
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/.schemawiz_config3
--rwxr-xr-x   0        0        0      316 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/backup.bat
--rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/chk_zetl.bat
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/floats.csv
--rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/local_sqlite_db
--rwxr-xr-x   0        0        0      295 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/restore.bat
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/sample.csv
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/sample.tsv
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/sampletable.ddl
--rw-r--r--   0        0        0    50392 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/tesla.csv
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/z_etl.csv
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/z_log.csv
--rw-r--r--   0        0        0     8298 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/zetl_pythonscript_temp.log
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/zetl_scripts/audit/10.audit.sql
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/zetl_scripts/audit/z_etl.csv
--rwxr-xr-x   0        0        0      237 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/zetl_scripts/backup/15.extract_csv_files.bat
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/zetl_scripts/backup/z_etl.csv
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/zetl_scripts/demo2/1.somethings.sql
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/zetl_scripts/demo2/z_etl.csv
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/zetl_scripts/demo3/1.tms.sql
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/zetl_scripts/demo3/z_etl.csv
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/zetl_scripts/empty_log/1.truncate_zlog.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/zetl_scripts/empty_log/z_etl.csv
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/zetl_scripts/view_log/1.latest_log_view.sql
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 zetl-3.4.0/tests/zetl_scripts/view_log/z_etl.csv
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 zetl-3.4.0/.gitignore
--rw-r--r--   0        0        0    18431 2020-02-02 00:00:00.000000 zetl-3.4.0/LICENSE
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 zetl-3.4.0/README.md
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 zetl-3.4.0/pyproject.toml
--rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 zetl-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 zetl-3.4.1/PyPI-Recovery-Codes-iamthedave-2024-04-29T14_24_52.946204.txt
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 zetl-3.4.1/testszetl_pythonscript_temp.log
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/.schemawiz_config3
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/1.CURRENT_DATE.sql
+-rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/BMONAS-Finalresend.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/__init__.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/common.py
+-rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/local_sqlite_db
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/menu.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/mysql_export.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/mysql_extract.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/mysql_import.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/postgres_export.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/postgres_extract.py
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/postgres_import.py
+-rw-r--r--   0        0        0    29992 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/run.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/sample.csv
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/sample7.csv
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/sqlite_export.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/sqlite_extract.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/sqlite_import.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/view.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/z.sample8.ddl
+-rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl.db
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_this_file.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_this_folder.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl1/0.init.sql
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl1/10.version_check.sql
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl1/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl1 - Copy/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl1 - Copy/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl2/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl2/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl2 - Copy/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl2 - Copy/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl3/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl3/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl3 - Copy/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl3 - Copy/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl4/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl4/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl4 - Copy/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl4 - Copy/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl4 - Copy - Copy/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl4 - Copy - Copy/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl4 - Copy - Copy (2)/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/etl4 - Copy - Copy (2)/z_etl.csv
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/test/1.another_mysqlcheck.sql
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/test/another_postgrescheck.sql
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/test/check.sql
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/test/postgrescheck.sql
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 zetl-3.4.1/src/zetl/zetl_scripts/test/z_etl.csv
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/.schemawiz_config3
+-rwxr-xr-x   0        0        0      316 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/backup.bat
+-rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/chk_zetl.bat
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/floats.csv
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/local_sqlite_db
+-rwxr-xr-x   0        0        0      295 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/restore.bat
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/sample.csv
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/sample.tsv
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/sampletable.ddl
+-rw-r--r--   0        0        0    50392 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/tesla.csv
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/z_etl.csv
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/z_log.csv
+-rw-r--r--   0        0        0     8298 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/zetl_pythonscript_temp.log
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/zetl_scripts/audit/10.audit.sql
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/zetl_scripts/audit/z_etl.csv
+-rwxr-xr-x   0        0        0      237 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/zetl_scripts/backup/15.extract_csv_files.bat
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/zetl_scripts/backup/z_etl.csv
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/zetl_scripts/demo2/1.somethings.sql
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/zetl_scripts/demo2/z_etl.csv
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/zetl_scripts/demo3/1.tms.sql
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/zetl_scripts/demo3/z_etl.csv
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/zetl_scripts/empty_log/1.truncate_zlog.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/zetl_scripts/empty_log/z_etl.csv
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/zetl_scripts/view_log/1.latest_log_view.sql
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 zetl-3.4.1/tests/zetl_scripts/view_log/z_etl.csv
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 zetl-3.4.1/.gitignore
+-rw-r--r--   0        0        0    18431 2020-02-02 00:00:00.000000 zetl-3.4.1/LICENSE
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 zetl-3.4.1/README.md
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 zetl-3.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 zetl-3.4.1/PKG-INFO
```

### Comparing `zetl-3.4.0/src/zetl/BMONAS-Finalresend.csv` & `zetl-3.4.1/src/zetl/BMONAS-Finalresend.csv`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/src/zetl/common.py` & `zetl-3.4.1/src/zetl/common.py`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/src/zetl/local_sqlite_db` & `zetl-3.4.1/src/zetl/local_sqlite_db`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/src/zetl/menu.py` & `zetl-3.4.1/src/zetl/menu.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,23 +24,25 @@
 			if user_selection == 0:
 				sys.exit(0)
 			elif user_selection <= option_count and user_selection > -1:
 				print("Running ", user_selection, em.etl_list[user_selection])
 				em.run_zetl(em.etl_list[user_selection])
 			else:
 				print("You broke something ")
+		else:
+			sys.exit(0)
 
 class etl_menu:
 	def get_dir_separator(self):
 		somepath = os.getcwd()
 		if somepath.find('/') > -1:
 			self.dir_sep = '/'
 		else:
 			self.dir_sep = '\\'
-
+		self.dir_sep = 	os.sep
 		return self.dir_sep
 
 	def __init__(self):
 		self.dir_sep = self.get_dir_separator()
 		self.etl_path = os.getcwd() + self.dir_sep + 'zetl_scripts'
 		self.etl_list = []
 		self.etlcount = 0
@@ -53,15 +55,15 @@
 		my_zetl.zetldb.load_folders_to_zetl() 
 		my_zetl.proper_run(etl_name_to_run,run_parameter)
 
 	def findetls(self):
 		self.etl_list.append('0 - exit from zetl.menu')
 		subfolders = [ f.path for f in os.scandir(self.etl_path) if f.is_dir() ]
 		for etlwithpath in subfolders:
-			etl_with_char = etlwithpath.split(self.etl_path)[1]
+			etl_with_char = etlwithpath.split(self.etl_path)[1] 
 			etl = etl_with_char.split(self.get_dir_separator())[1]
 			self.etl_list.append(etl)
 			self.etl_list.sort()
 		self.etlcount = len(self.etl_list)
 
 	def show_menu(self):
```

### Comparing `zetl-3.4.0/src/zetl/mysql_export.py` & `zetl-3.4.1/src/zetl/mysql_export.py`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/src/zetl/mysql_extract.py` & `zetl-3.4.1/src/zetl/mysql_extract.py`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/src/zetl/mysql_import.py` & `zetl-3.4.1/src/zetl/mysql_import.py`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/src/zetl/postgres_export.py` & `zetl-3.4.1/src/zetl/postgres_export.py`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/src/zetl/postgres_extract.py` & `zetl-3.4.1/src/zetl/postgres_extract.py`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/src/zetl/postgres_import.py` & `zetl-3.4.1/src/zetl/postgres_import.py`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/src/zetl/run.py` & `zetl-3.4.1/src/zetl/run.py`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/src/zetl/sqlite_export.py` & `zetl-3.4.1/src/zetl/sqlite_export.py`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/src/zetl/sqlite_extract.py` & `zetl-3.4.1/src/zetl/sqlite_extract.py`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/src/zetl/sqlite_import.py` & `zetl-3.4.1/src/zetl/sqlite_import.py`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/src/zetl/view.py` & `zetl-3.4.1/src/zetl/view.py`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/src/zetl/zetl.db` & `zetl-3.4.1/src/zetl/zetl.db`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/src/zetl/zetl_this_file.py` & `zetl-3.4.1/src/zetl/zetl_this_file.py`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/src/zetl/zetl_this_folder.py` & `zetl-3.4.1/src/zetl/zetl_this_folder.py`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/src/zetl/zetl_scripts/test/1.another_mysqlcheck.sql` & `zetl-3.4.1/src/zetl/zetl_scripts/test/1.another_mysqlcheck.sql`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/tests/local_sqlite_db` & `zetl-3.4.1/tests/local_sqlite_db`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/tests/tesla.csv` & `zetl-3.4.1/tests/tesla.csv`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/tests/zetl_pythonscript_temp.log` & `zetl-3.4.1/tests/zetl_pythonscript_temp.log`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/LICENSE` & `zetl-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/README.md` & `zetl-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `zetl-3.4.0/pyproject.toml` & `zetl-3.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling","schemawizard_package","postgresdave_package","mysqldave_package","garbledave_package"]
 
 build-backend = "hatchling.build"
 
 [project]
 name = "zetl"
-version = "3.4.0"
+version = "3.4.1"
 dependencies = [
   'schemawizard_package >= 2.5.1',
   'postgresdave_package >= 1.8.0',
   'mysqldave_package >= 1.5.0',
   'sqlitedave_package >= 1.3.0',
   'garbledave_package >= 1.0.0 '
 ]
```

### Comparing `zetl-3.4.0/PKG-INFO` & `zetl-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: zetl
-Version: 3.4.0
+Version: 3.4.1
 Summary: A simple ETL framework for Python, SQL and BAT files which uses a Postgres database for activity logging.
 Project-URL: Homepage, https://github.com/daveskura/zetl
 Project-URL: Author Linkedin, https://www.linkedin.com/in/2166883
 Author-email: Dave Skura <dskura@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

