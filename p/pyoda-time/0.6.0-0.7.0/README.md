# Comparing `tmp/pyoda_time-0.6.0.tar.gz` & `tmp/pyoda_time-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoda_time-0.6.0.tar", max compression
+gzip compressed data, was "pyoda_time-0.7.0.tar", max compression
```

## Comparing `pyoda_time-0.6.0.tar` & `pyoda_time-0.7.0.tar`

### file list

```diff
@@ -1,12 +1,151 @@
--rw-r--r--   0        0        0    11357 2024-01-12 00:37:35.709362 pyoda_time-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0      595 2024-01-12 00:37:35.709362 pyoda_time-0.6.0/NOTICE.txt
--rw-r--r--   0        0        0     1296 2024-01-12 00:37:35.709362 pyoda_time-0.6.0/README.md
--rw-r--r--   0        0        0   184265 2024-01-12 00:37:35.709362 pyoda_time-0.6.0/pyoda_time/__init__.py
--rw-r--r--   0        0        0   114859 2024-01-12 00:37:35.709362 pyoda_time-0.6.0/pyoda_time/calendars.py
--rw-r--r--   0        0        0    11132 2024-01-12 00:37:35.709362 pyoda_time-0.6.0/pyoda_time/fields.py
--rw-r--r--   0        0        0        0 2024-01-12 00:37:35.709362 pyoda_time-0.6.0/pyoda_time/py.typed
--rw-r--r--   0        0        0     8358 2024-01-12 00:37:35.709362 pyoda_time-0.6.0/pyoda_time/time_zones.py
--rw-r--r--   0        0        0     7156 2024-01-12 00:37:35.709362 pyoda_time-0.6.0/pyoda_time/utility.py
--rw-r--r--   0        0        0      186 2024-01-12 00:37:35.709362 pyoda_time-0.6.0/pyoda_time/version.py
--rw-r--r--   0        0        0     1513 2024-01-12 00:37:35.709362 pyoda_time-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1862 1970-01-01 00:00:00.000000 pyoda_time-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-17 00:46:33.059584 pyoda_time-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0      595 2024-05-17 00:46:33.059584 pyoda_time-0.7.0/NOTICE.txt
+-rw-r--r--   0        0        0     1692 2024-05-17 00:46:33.059584 pyoda_time-0.7.0/README.md
+-rw-r--r--   0        0        0     1506 2024-05-17 00:46:33.075584 pyoda_time-0.7.0/pyoda_time/__init__.py
+-rw-r--r--   0        0        0     1093 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_calendar_ordinal.py
+-rw-r--r--   0        0        0    36810 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_calendar_system.py
+-rw-r--r--   0        0        0      164 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/__init__.py
+-rw-r--r--   0        0        0      770 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_argument_exception.py
+-rw-r--r--   0        0        0     2039 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_calendar.py
+-rw-r--r--   0        0        0    26120 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_calendar_data.py
+-rw-r--r--   0        0        0     4094 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_calendar_id.py
+-rw-r--r--   0        0        0    57748 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_culture_data.py
+-rw-r--r--   0        0        0    18099 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_culture_info.py
+-rw-r--r--   0        0        0     1757 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_culture_not_found_exception.py
+-rw-r--r--   0        0        0     1652 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_culture_types.py
+-rw-r--r--   0        0        0    23385 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_date_time_format_info.py
+-rw-r--r--   0        0        0      372 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_day_of_week.py
+-rw-r--r--   0        0        0     1148 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_globalization_mode.py
+-rw-r--r--   0        0        0      789 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_gregorian_calendar.py
+-rw-r--r--   0        0        0     1090 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_gregorian_calendar_helper.py
+-rw-r--r--   0        0        0      666 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_gregorian_calendar_types.py
+-rw-r--r--   0        0        0     2823 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_hebrew_calendar.py
+-rw-r--r--   0        0        0     2073 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_hijri_calendar.py
+-rw-r--r--   0        0        0      980 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_i_format_provider.py
+-rw-r--r--   0        0        0   172662 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_icu_locale_data.py
+-rw-r--r--   0        0        0    13348 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_interop.py
+-rw-r--r--   0        0        0     4767 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_japanese_calendar.py
+-rw-r--r--   0        0        0     1152 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_korean_calendar.py
+-rw-r--r--   0        0        0     2968 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_number_format_info.py
+-rw-r--r--   0        0        0     1226 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_persian_calendar.py
+-rw-r--r--   0        0        0     1150 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_string_builder.py
+-rw-r--r--   0        0        0     1111 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_taiwan_calendar.py
+-rw-r--r--   0        0        0      936 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_text_info.py
+-rw-r--r--   0        0        0      814 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_thai_buddhist_calendar.py
+-rw-r--r--   0        0        0      799 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_compatibility/_um_al_qura_calendar.py
+-rw-r--r--   0        0        0      797 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_date_adjusters.py
+-rw-r--r--   0        0        0     1934 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_date_interval.py
+-rw-r--r--   0        0        0     3481 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_date_time_zone.py
+-rw-r--r--   0        0        0    37920 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_duration.py
+-rw-r--r--   0        0        0    19497 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_instant.py
+-rw-r--r--   0        0        0      464 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_iso_day_of_week.py
+-rw-r--r--   0        0        0    17684 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_local_date.py
+-rw-r--r--   0        0        0    15920 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_local_date_time.py
+-rw-r--r--   0        0        0     4755 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_local_instant.py
+-rw-r--r--   0        0        0    25129 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_local_time.py
+-rw-r--r--   0        0        0    18405 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_offset.py
+-rw-r--r--   0        0        0     4229 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_offset_date_time.py
+-rw-r--r--   0        0        0     2697 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_offset_time.py
+-rw-r--r--   0        0        0    33887 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_period.py
+-rw-r--r--   0        0        0     4545 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_period_builder.py
+-rw-r--r--   0        0        0     1390 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_period_units.py
+-rw-r--r--   0        0        0     3545 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_pyoda_constants.py
+-rw-r--r--   0        0        0     8954 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_year_month.py
+-rw-r--r--   0        0        0     4146 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_year_month_day.py
+-rw-r--r--   0        0        0     4559 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_year_month_day_calendar.py
+-rw-r--r--   0        0        0     3668 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/_zoned_date_time.py
+-rw-r--r--   0        0        0      677 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/calendars/__init__.py
+-rw-r--r--   0        0        0    11193 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/calendars/_badi_year_month_day_calculator.py
+-rw-r--r--   0        0        0      411 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/calendars/_calendar_week_rule.py
+-rw-r--r--   0        0        0     1310 2024-05-17 00:46:33.079584 pyoda_time-0.7.0/pyoda_time/calendars/_coptic_year_month_day_calculator.py
+-rw-r--r--   0        0        0     4366 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_era.py
+-rw-r--r--   0        0        0     1208 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_era_calculator.py
+-rw-r--r--   0        0        0     2438 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_fixed_month_year_month_day_calculator.py
+-rw-r--r--   0        0        0     2048 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_g_j_era_calculator.py
+-rw-r--r--   0        0        0     3741 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_g_j_year_month_day_calculator.py
+-rw-r--r--   0        0        0     7126 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_gregorian_year_month_day_calculator.py
+-rw-r--r--   0        0        0     1781 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_hebrew_month_converter.py
+-rw-r--r--   0        0        0     1620 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_hebrew_month_numbering.py
+-rw-r--r--   0        0        0    12707 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_hebrew_scriptural_calculator.py
+-rw-r--r--   0        0        0    10894 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_hebrew_year_month_day_calculator.py
+-rw-r--r--   0        0        0      850 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_i_week_year_rule.py
+-rw-r--r--   0        0        0      866 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_islamic_epoch.py
+-rw-r--r--   0        0        0     1754 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_islamic_leap_year_pattern.py
+-rw-r--r--   0        0        0     7858 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_islamic_year_month_day_calculator.py
+-rw-r--r--   0        0        0     1559 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_julian_year_month_day_calculator.py
+-rw-r--r--   0        0        0     9097 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_persian_year_month_day_calculator.py
+-rw-r--r--   0        0        0     4737 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_regular_year_month_day_calculator.py
+-rw-r--r--   0        0        0    11988 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_simple_week_year_rule.py
+-rw-r--r--   0        0        0     2070 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_single_era_calculator.py
+-rw-r--r--   0        0        0     6168 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_um_al_qura_year_month_day_calculator.py
+-rw-r--r--   0        0        0     2998 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_week_year_rules.py
+-rw-r--r--   0        0        0    11714 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_year_month_day_calculator.py
+-rw-r--r--   0        0        0     2404 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/calendars/_year_start_cache_entry.py
+-rw-r--r--   0        0        0      188 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/fields/__init__.py
+-rw-r--r--   0        0        0      843 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/fields/_date_period_fields.py
+-rw-r--r--   0        0        0     3111 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/fields/_fixed_length_date_period_field.py
+-rw-r--r--   0        0        0     1552 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/fields/_i_date_period_field.py
+-rw-r--r--   0        0        0     1039 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/fields/_months_period_field.py
+-rw-r--r--   0        0        0     5401 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/fields/_time_period_field.py
+-rw-r--r--   0        0        0     2112 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/fields/_years_period_field.py
+-rw-r--r--   0        0        0      188 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/globalization/__init__.py
+-rw-r--r--   0        0        0     1287 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/globalization/_pattern_resources.py
+-rw-r--r--   0        0        0    24404 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/globalization/_pyoda_format_info.py
+-rw-r--r--   0        0        0        0 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/py.typed
+-rw-r--r--   0        0        0      803 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/__init__.py
+-rw-r--r--   0        0        0     4803 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_composite_pattern_builder.py
+-rw-r--r--   0        0        0     1289 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_fixed_format_info_pattern_parser.py
+-rw-r--r--   0        0        0     7164 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_format_helper.py
+-rw-r--r--   0        0        0      932 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_i_partial_pattern.py
+-rw-r--r--   0        0        0     1781 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_i_pattern.py
+-rw-r--r--   0        0        0    10384 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_instant_pattern.py
+-rw-r--r--   0        0        0     4142 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_instant_pattern_parser.py
+-rw-r--r--   0        0        0      834 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_invalid_pattern_exception.py
+-rw-r--r--   0        0        0    13443 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_local_date_pattern.py
+-rw-r--r--   0        0        0    18274 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_local_date_pattern_parser.py
+-rw-r--r--   0        0        0    21615 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_local_date_time_pattern.py
+-rw-r--r--   0        0        0    15907 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_local_date_time_pattern_parser.py
+-rw-r--r--   0        0        0    16845 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_local_time_pattern.py
+-rw-r--r--   0        0        0    12001 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_local_time_pattern_parser.py
+-rw-r--r--   0        0        0     7527 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_offset_pattern.py
+-rw-r--r--   0        0        0    12491 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_offset_pattern_parser.py
+-rw-r--r--   0        0        0     1044 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_parse_bucket.py
+-rw-r--r--   0        0        0    18467 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_parse_result.py
+-rw-r--r--   0        0        0     3604 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_text_cursor.py
+-rw-r--r--   0        0        0     7703 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_text_error_messages.py
+-rw-r--r--   0        0        0      403 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_unparsable_value_error.py
+-rw-r--r--   0        0        0     9795 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/_value_cursor.py
+-rw-r--r--   0        0        0      188 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/patterns/__init__.py
+-rw-r--r--   0        0        0    11760 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/patterns/_date_pattern_helper.py
+-rw-r--r--   0        0        0      594 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/patterns/_i_pattern_parser.py
+-rw-r--r--   0        0        0     1545 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/patterns/_pattern_bcl_support.py
+-rw-r--r--   0        0        0     4895 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/patterns/_pattern_cursor.py
+-rw-r--r--   0        0        0     2263 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/patterns/_pattern_fields.py
+-rw-r--r--   0        0        0    31977 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/patterns/_stepped_pattern_builder.py
+-rw-r--r--   0        0        0    13177 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/text/patterns/_time_pattern_helper.py
+-rw-r--r--   0        0        0      423 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/time_zones/__init__.py
+-rw-r--r--   0        0        0     2001 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/time_zones/_fixed_date_time_zone.py
+-rw-r--r--   0        0        0      777 2024-05-17 00:46:33.083584 pyoda_time-0.7.0/pyoda_time/time_zones/_i_zone_interval_map.py
+-rw-r--r--   0        0        0     9198 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/time_zones/_tzdb_zone_1970_location.py
+-rw-r--r--   0        0        0     5807 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/time_zones/_tzdb_zone_location.py
+-rw-r--r--   0        0        0     8399 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/time_zones/_zone_interval.py
+-rw-r--r--   0        0        0      297 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/time_zones/cldr/__init__.py
+-rw-r--r--   0        0        0     6446 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/time_zones/cldr/_map_zone.py
+-rw-r--r--   0        0        0     7056 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/time_zones/cldr/_windows_zones.py
+-rw-r--r--   0        0        0      188 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/time_zones/io/__init__.py
+-rw-r--r--   0        0        0     9693 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/time_zones/io/_date_time_zone_reader.py
+-rw-r--r--   0        0        0    11633 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/time_zones/io/_date_time_zone_writer.py
+-rw-r--r--   0        0        0     2906 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/time_zones/io/_i_date_time_zone_reader.py
+-rw-r--r--   0        0        0     2832 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/time_zones/io/_i_date_time_zone_writer.py
+-rw-r--r--   0        0        0     7959 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/time_zones/io/_tzdb_stream_data.py
+-rw-r--r--   0        0        0     2084 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/time_zones/io/_tzdb_stream_field.py
+-rw-r--r--   0        0        0     1801 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/time_zones/io/_tzdb_stream_field_id.py
+-rw-r--r--   0        0        0      277 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/utility/__init__.py
+-rw-r--r--   0        0        0     2620 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/utility/_cache.py
+-rw-r--r--   0        0        0     5089 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/utility/_csharp_compatibility.py
+-rw-r--r--   0        0        0      521 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/utility/_hash_code_helper.py
+-rw-r--r--   0        0        0      488 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/utility/_invalid_pyoda_data_exception.py
+-rw-r--r--   0        0        0     1904 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/utility/_preconditions.py
+-rw-r--r--   0        0        0     2115 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyoda_time/utility/_tick_arithmetic.py
+-rw-r--r--   0        0        0     1664 2024-05-17 00:46:33.087584 pyoda_time-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2447 1970-01-01 00:00:00.000000 pyoda_time-0.7.0/PKG-INFO
```

### Comparing `pyoda_time-0.6.0/LICENSE.txt` & `pyoda_time-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.6.0/NOTICE.txt` & `pyoda_time-0.7.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.6.0/pyoda_time/time_zones.py` & `pyoda_time-0.7.0/pyoda_time/time_zones/_zone_interval.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,192 +1,190 @@
 # Copyright 2024 The Pyoda Time Authors. All rights reserved.
 # Use of this source code is governed by the Apache License 2.0,
 # as found in the LICENSE.txt file.
 
-from __future__ import annotations as _annotations
+from __future__ import annotations
 
-import typing as _typing
+from typing import TYPE_CHECKING, Final, final
 
-if _typing.TYPE_CHECKING:
-    from . import (
-        Duration as _Duration,
+if TYPE_CHECKING:
+    from .. import (
+        Duration,
+        Instant,
+        LocalDateTime,
+        Offset,
     )
-    from . import (
-        Instant as _Instant,
-    )
-    from . import (
-        LocalDateTime as _LocalDateTime,
-    )
-    from . import (
-        Offset as _Offset,
-    )
-    from . import (
+    from .._local_instant import (
         _LocalInstant,
     )
 
-from pyoda_time.utility import _hash_code_helper, _Preconditions, _sealed
+from pyoda_time.utility._csharp_compatibility import _sealed
+from pyoda_time.utility._hash_code_helper import _hash_code_helper
+from pyoda_time.utility._preconditions import _Preconditions
+
+__all__ = ["ZoneInterval"]
 
 
 @_sealed
-@_typing.final
+@final
 class ZoneInterval:
     """Represents a range of time for which a particular Offset applies.
 
     Equality is defined component-wise in terms of all properties: the name, the start and end, and the offsets.
     There is no ordering defined between zone intervals.
     """
 
     @property
-    def _raw_start(self) -> _Instant:
+    def _raw_start(self) -> Instant:
         """Returns the underlying start instant of this zone interval.
 
         If the zone interval extends to the beginning of time, the return
         value will be ``Instant._before_min_value``; this value
         should *not* be exposed publicly.
         """
         return self.__raw_start
 
     @property
-    def _raw_end(self) -> _Instant:
+    def _raw_end(self) -> Instant:
         """Returns the underlying end instant of this zone interval.
 
         If the zone interval extends to the end of time, the return
         value will be ``Instant._after_max_value``; this value
         should *not* be exposed publicly.
         """
         return self.__raw_end
 
     @property
-    def standard_offset(self) -> _Offset:
+    def standard_offset(self) -> Offset:
         """Gets the standard offset for this period.
 
         This is the offset without any daylight savings contributions.
         """
         return self.wall_offset - self.savings
 
     @property
-    def duration(self) -> _Duration:
+    def duration(self) -> Duration:
         """The Duration of this zone interval."""
         return self.end - self.start
 
     @property
     def has_start(self) -> bool:
         """Returns ``True`` if this zone interval has a fixed start point, or ``False`` if it extends to the beginning
         of time."""
         return self._raw_start._is_valid
 
     @property
-    def end(self) -> _Instant:
+    def end(self) -> Instant:
         """The last Instant (exclusive) that the Offset applies."""
         _Preconditions._check_state(self._raw_end._is_valid, "Zone interval extends to the end of time")
         return self._raw_end
 
     @property
     def has_end(self) -> bool:
         """Returns ``True`` if this zone interval has a fixed end point, or ``False`` if it extends to the beginning of
         time."""
         return self._raw_end._is_valid
 
     @property
-    def iso_local_start(self) -> _LocalDateTime:
+    def iso_local_start(self) -> LocalDateTime:
         """Gets the local start time of the interval, as a ``LocalDateTime`` in the ISO calendar."""
         # Use the Start property to trigger the appropriate end-of-time exception.
         # Call Plus to trigger an appropriate out-of-range exception.
-        from . import LocalDateTime
+        from .. import LocalDateTime
 
         return LocalDateTime._ctor(local_instant=self.start._plus(self.wall_offset))
 
     @property
-    def iso_local_end(self) -> _LocalDateTime:
+    def iso_local_end(self) -> LocalDateTime:
         """Gets the local end time of the interval, as a ``LocalDateTime`` in the ISO calendar."""
         # Use the End property to trigger the appropriate end-of-time exception.
         # Call Plus to trigger an appropriate out-of-range exception.
-        from . import LocalDateTime
+        from .. import LocalDateTime
 
         return LocalDateTime._ctor(local_instant=self.end._plus(self.wall_offset))
 
     @property
     def name(self) -> str:
         """The name of this offset period (e.g. PST or PDT)."""
         return self.__name
 
     @property
-    def wall_offset(self) -> _Offset:
+    def wall_offset(self) -> Offset:
         """The offset from UTC for this period.
 
         This includes any daylight savings value.
         """
         return self.__wall_offset
 
     @property
-    def savings(self) -> _Offset:
+    def savings(self) -> Offset:
         """The daylight savings value for this period."""
         return self.__savings
 
     @property
-    def start(self) -> _Instant:
+    def start(self) -> Instant:
         """The first Instant that the Offset applies."""
         _Preconditions._check_state(self._raw_start._is_valid, "Zone interval extends to the beginning of time")
         return self._raw_start
 
     # Note: This initialiser is intended to replicate the functionality of both
     # of the private constructors for the equivalent Noda Time class.
     def __init__(
         self,
         *,
         name: str,
-        start: _Instant | None = None,
-        end: _Instant | None = None,
-        wall_offset: _Offset,
-        savings: _Offset,
+        start: Instant | None = None,
+        end: Instant | None = None,
+        wall_offset: Offset,
+        savings: Offset,
     ) -> None:
-        from . import Instant
+        from .. import Instant
 
         # Do not expose these defaults in the __init__ signature.
         if start is None:
             start = Instant._before_min_value()
         if end is None:
             end = Instant._after_max_value()
 
         _Preconditions._check_not_null(name, "name")
         _Preconditions._check_argument(
             start < end, "start", f"The start Instant must be less than the end Instant. start: {start}; end: {end}"
         )
-        self.__name: _typing.Final[str] = name
-        self.__raw_start: _typing.Final[_Instant] = start
-        self.__raw_end: _typing.Final[_Instant] = end
-        self.__wall_offset: _typing.Final[_Offset] = wall_offset
-        self.__savings: _typing.Final[_Offset] = savings
+        self.__name: Final[str] = name
+        self.__raw_start: Final[Instant] = start
+        self.__raw_end: Final[Instant] = end
+        self.__wall_offset: Final[Offset] = wall_offset
+        self.__savings: Final[Offset] = savings
         # Work out the corresponding local instants, taking care to "go infinite" appropriately.
-        self.__local_start: _typing.Final[_LocalInstant] = start._safe_plus(wall_offset)
-        self.__local_end: _typing.Final[_LocalInstant] = end._safe_plus(wall_offset)
+        self.__local_start: Final[_LocalInstant] = start._safe_plus(wall_offset)
+        self.__local_end: Final[_LocalInstant] = end._safe_plus(wall_offset)
 
-    def _with_start(self, new_start: _Instant) -> ZoneInterval:
+    def _with_start(self, new_start: Instant) -> ZoneInterval:
         """Returns a copy of this zone interval, but with the given start instant."""
         return ZoneInterval(
             name=self.name,
             start=new_start,
             end=self._raw_end,
             wall_offset=self.wall_offset,
             savings=self.savings,
         )
 
-    def _with_end(self, new_end: _Instant) -> ZoneInterval:
+    def _with_end(self, new_end: Instant) -> ZoneInterval:
         """Returns a copy of this zone interval, but with the given end instant."""
         return ZoneInterval(
             name=self.name,
             start=self._raw_start,
             end=new_end,
             wall_offset=self.wall_offset,
             savings=self.savings,
         )
 
     # region Contains
 
-    def __contains__(self, instant: _Instant) -> bool:
+    def __contains__(self, instant: Instant) -> bool:
         """Determines whether this period contains the given Instant in its range."""
         # Implementation of ``public bool Contains(Instant instant)``
         return self._raw_start <= instant < self._raw_end
 
     def _contains(self, local_instant: _LocalInstant) -> bool:
         """Determines whether this period contains the given LocalInstant in its range."""
         # Implementation of ``internal bool Contains(LocalInstant localInstant)``
@@ -201,24 +199,27 @@
 
     # region IEquatable<ZoneInterval> Members
 
     def equals(self, other: ZoneInterval) -> bool:
         return self == other
 
     def __eq__(self, other: object) -> bool:
+        if not isinstance(other, ZoneInterval):
+            return NotImplemented
         return (
-            isinstance(other, ZoneInterval)
-            and self.name == other.name
+            self.name == other.name
             and self._raw_start == other._raw_start
             and self._raw_end == other._raw_end
             and self.wall_offset == other.wall_offset
             and self.savings == other.savings
-        ) or NotImplemented
+        )
 
     def __ne__(self, other: object) -> bool:
+        if not isinstance(other, ZoneInterval):
+            return NotImplemented
         return not self == other
 
     # endregion
 
     # region Object overrides
 
     def __hash__(self) -> int:
```

### Comparing `pyoda_time-0.6.0/pyoda_time/utility.py` & `pyoda_time-0.7.0/pyoda_time/utility/_csharp_compatibility.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,181 +1,147 @@
 # Copyright 2024 The Pyoda Time Authors. All rights reserved.
 # Use of this source code is governed by the Apache License 2.0,
 # as found in the LICENSE.txt file.
 
-from __future__ import annotations as _annotations
+from __future__ import annotations
 
-__all__: list[str] = []
-
-import datetime as _datetime
-import typing as _typing
-
-_T = _typing.TypeVar("_T")
-_Ttype = _typing.TypeVar("_Ttype", bound=type)
-
-
-class _Preconditions:
-    """Helper static methods for argument/state validation."""
-
-    @classmethod
-    def _check_not_null(cls, argument: _T, param_name: str) -> _T:
-        """Returns the given argument after checking whether it's null.
-
-        This is useful for putting nullity checks in parameters which are passed to base class constructors.
-        """
-        if argument is None:
-            raise TypeError(f"{param_name} cannot be None.")
-        return argument
-
-    @classmethod
-    def _check_argument_range(cls, param_name: str, value: int, min_inclusive: int, max_inclusive: int) -> None:
-        if (value < min_inclusive) or (value > max_inclusive):
-            cls._throw_argument_out_of_range_exception(param_name, value, min_inclusive, max_inclusive)
-
-    @staticmethod
-    def _throw_argument_out_of_range_exception(
-        param_name: str, value: _T, min_inclusive: _T, max_inclusive: _T
-    ) -> None:
-        raise ValueError(
-            f"Value should be in range [{min_inclusive}-{max_inclusive}]\n"
-            f"Parameter name: {param_name}\n"
-            f"Actual value was {value}"
-        )
-
-    @classmethod
-    def _check_argument(cls, expession: bool, parameter: str, message: str, *message_args: _typing.Any) -> None:
-        if not expession:
-            if message_args:
-                message = message.format(*message_args)
-            raise ValueError(f"{message}\nParameter name: {parameter}")
-
-    @classmethod
-    def _check_state(cls, expression: bool, message: str) -> None:
-        if not expression:
-            raise RuntimeError(message)
+import datetime
+import decimal
+from typing import Any, Final, Literal, TypeVar
 
+__all__: list[str] = []
 
-class _TickArithmetic:
-    """Common operations on ticks."""
-
-    @staticmethod
-    def ticks_to_days_and_tick_of_day(ticks: int) -> tuple[int, int]:
-        """Cautiously converts a number of ticks (which can have any value) into a number of days and a tick within that
-        day."""
-
-        from pyoda_time import PyodaConstants
-
-        if ticks >= 0:
-            days = int((ticks >> 14) / 52734375)
-            tick_of_day = ticks - days * PyodaConstants.TICKS_PER_DAY
-        else:
-            days = _towards_zero_division(ticks + 1, PyodaConstants.TICKS_PER_DAY) - 1
-            tick_of_day = ticks - (days + 1) * PyodaConstants.TICKS_PER_DAY + PyodaConstants.TICKS_PER_DAY
-
-        return days, tick_of_day
-
-    @staticmethod
-    def days_and_tick_of_day_to_ticks(days: int, tick_of_day: int) -> int:
-        """Cautiously computes a number of ticks from day/tick-of-day value.
-
-        This may overflow, but will only do so if it has to.
-        """
-        from . import PyodaConstants
-
-        # TODO: Get a better handle on what this is doing with regard to long overflow
-        if days >= _towards_zero_division(_CsharpConstants.LONG_MIN_VALUE, PyodaConstants.TICKS_PER_DAY):
-            return days * PyodaConstants.TICKS_PER_DAY + tick_of_day
-        return (days + 1) * PyodaConstants.TICKS_PER_DAY + tick_of_day - PyodaConstants.TICKS_PER_DAY
-
-    @staticmethod
-    def bounded_days_and_tick_of_day_to_ticks(days: int, tick_of_day: int) -> int:
-        """Computes a number of ticks from a day/tick-of-day value which is trusted not to overflow, even when computed
-        in the simplest way.
-
-        Only call this method from places where there are suitable constraints on the input.
-        """
+SEALED_CLASSES: Final[list[type]] = []
+_T = TypeVar("_T")
+_Ttype = TypeVar("_Ttype", bound=type)
 
-        from pyoda_time import PyodaConstants
 
-        return days * PyodaConstants.TICKS_PER_DAY + tick_of_day
+def _as_span(text: str | None, start: int) -> str:
+    """Roughly equivalent to:
+    public static ReadOnlySpan<char> AsSpan(this string? text, int start)
+    """
+    if text is None:
+        if start != 0:
+            raise IndexError("start index out of range")
+        return ""
+    if not (0 <= start <= len(text)):
+        raise IndexError("start index out of range")
+    return text[start:]
 
 
-def _towards_zero_division(x: int | float, y: int | float) -> int:
+def _towards_zero_division(x: int | float | decimal.Decimal, y: int | float | decimal.Decimal) -> int:
     """Divide two numbers using "towards zero" rounding.
 
     This ensures that integer division produces the same result as it would do in C#.
     """
     from decimal import ROUND_DOWN, Decimal
 
     return int((Decimal(x) / Decimal(y)).quantize(0, ROUND_DOWN))
 
 
-def _to_ticks(dt: _datetime.datetime) -> int:
+def _to_ticks(dt: datetime.datetime) -> int:
     """Get a value akin to C#'s DateTime.Ticks property from a python datetime."""
     # Gratefully stolen from https://stackoverflow.com/a/29368771
-    return int((dt - _datetime.datetime(1, 1, 1, tzinfo=_datetime.timezone.utc)).total_seconds() * 10000000)
+    return int((dt - datetime.datetime(1, 1, 1, tzinfo=datetime.timezone.utc)).total_seconds() * 10000000)
 
 
 def _sealed(cls: _Ttype) -> _Ttype:
     """Prevents the decorated class from being subclassed.
 
-    This is intended to loosely emulate the behaviour of the `sealed` keyword in C#.
-    Its use should be accompanied by the `typing.final` decorator to aid static analysis.
+    This is intended to loosely emulate the behaviour of the ``sealed`` keyword in C#.
+    Its use should be accompanied by the ``typing.final`` decorator to aid static analysis.
     """
 
     def __init_subclass__() -> None:
         raise TypeError(f"{cls.__name__} is not intended to be subclassed.")
 
     # Use setattr to stop mypy shouting
     setattr(cls, "__init_subclass__", __init_subclass__)
 
+    SEALED_CLASSES.append(cls)
+
     return cls
 
 
 def _private(klass: _Ttype) -> _Ttype:
     """Prevents the decorated class from being instantiated.
 
     This is used to decorate Python classes which have been ported from C#, where the C# class has no public
     constructor.
     """
 
     msg = f"{klass.__name__} is not intended to be initialised directly."
 
-    def __init__(*_args: _typing.Any, **_kwargs: _typing.Any) -> None:
+    def __init__(self: Any) -> None:
+        """
+
+        :raises TypeError: This class is not intended to be instantiated directly.
+        """
         raise TypeError(msg)
 
-    def __new__(*_args: _typing.Any, **_kwargs: _typing.Any) -> _Ttype:
+    def __new__(cls: _Ttype) -> _Ttype:
+        """
+
+        :raises TypeError: This class is not intended to be instantiated directly.
+        """
         raise TypeError(msg)
 
-    def __call__(*_args: _typing.Any, **_kwargs: _typing.Any) -> _Ttype:
+    def __call__(*_args: Any, **_kwargs: Any) -> _Ttype:
+        """
+
+        :raises TypeError: This class is not intended to be instantiated directly.
+        """
         raise TypeError(msg)
 
     # Use setattr to stop mypy shouting
     setattr(klass, "__init__", __init__)
     setattr(klass, "__new__", __new__)
     setattr(klass, "__call__", __call__)
 
+    # This is used in sphinx docs to ignore the special methods assigned above.
+    setattr(klass, "__no_public_constructor__", True)
+
     return klass
 
 
 class _CsharpConstants:
-    LONG_MAX_VALUE: _typing.Final[int] = 9223372036854775807
-    LONG_MIN_VALUE: _typing.Final[int] = -9223372036854775808
+    INT_MIN_VALUE: Final[int] = -2147483648
+    INT_MAX_VALUE: Final[int] = 2147483647
+    LONG_MIN_VALUE: Final[int] = -9223372036854775808
+    LONG_MAX_VALUE: Final[int] = 9223372036854775807
+
+
+def __int_overflow(value: int, bits: Literal[32, 64]) -> int:
+    """Simulates C# signed integer overflow behavior for a specified bit width.
+
+    :param value: The integer value to apply overflow to.
+    :param bits: The bit width of the integer.
+    :return: The result after simulating overflow for the specified bit width.
+    """
+    max_value: int = 2 ** (bits - 1)
+    result: int = (value + max_value) % (2**bits) - max_value
+    return result
 
 
 def _int32_overflow(value: int) -> int:
-    """Simulates 32-bit signed integer overflow behavior.
+    """Simulates C# 32-bit signed integer overflow behavior.
 
-    Args:
-        value (int): The integer value to apply 32-bit overflow to.
+    :param value: The integer value to apply 32-bit overflow to.
+    :return: The result after simulating 32-bit overflow.
+    """
+    return __int_overflow(value, 32)
 
-    Returns:
-        int: The result after simulating 32-bit overflow.
+
+def _int64_overflow(value: int) -> int:
+    """Simulates C# 64-bit signed integer overflow behavior.
+
+    :param value: The integer value to apply 64-bit overflow to.
+    :return: The result after simulating 64-bit overflow.
     """
-    return (value + 2**31) % 2**32 - 2**31
+    return __int_overflow(value, 64)
 
 
 def _csharp_modulo(dividend: int, divisor: int) -> int:
     """Perform a modulo operation with C# behavior, where the result has the same sign as the divisor.
 
     In C#, the result of a modulo operation takes the sign of the divisor, unlike Python where it
     takes the sign of the dividend. This function adjusts the Python modulo result to mimic C#'s behavior.
@@ -187,17 +153,7 @@
     Returns:
     int: The result of the modulo operation, adjusted for C# behavior.
     """
     result = dividend % divisor
     if dividend < 0 < result:
         result -= abs(divisor)
     return result
-
-
-def _hash_code_helper(*values: _typing.Hashable) -> int:
-    """Provides help with generating hash codes."""
-    # In Noda Time, this is a builder pattern struct.
-    multiplier = 37
-    ret = 17
-    for v in values:
-        ret += ret * multiplier + hash(v)
-    return ret
```

### Comparing `pyoda_time-0.6.0/pyproject.toml` & `pyoda_time-0.7.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,69 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.commitizen]
-name = "cz_conventional_commits"
-tag_format = "$version"
-version_scheme = "pep440"
-version_provider = "poetry"
-update_changelog_on_bump = true
-major_version_zero = true
-
 [tool.docformatter]
 black = true
 recursive = true
 in-place = true
 wrap-summaries = 120
 wrap-descriptions = 120
 
 [tool.mypy]
 disallow_untyped_defs = true
-# strict mode sounds good, but at time of writing it just warns about pytest.mark.parametrize
-# strict = true
+implicit_reexport = false
+pretty = true
+strict = true
+warn_no_return = true
+warn_redundant_casts = true
 warn_return_any = true
+warn_unreachable = true
 warn_unused_configs = true
+warn_unused_ignores = true
 
 [tool.poetry]
 name = "pyoda-time"
-version = "0.6.0"
+version = "0.7.0"
 description = "An alternative datetime library for Python."
 authors = ["Christopher McEvoy <12284065+chrisimcevoy@users.noreply.github.com>"]
 license = "Apache-2.0"
 readme = "README.md"
+homepage = "https://pyodatime.org/"
 repository = "https://github.com/chrisimcevoy/pyoda-time"
 classifiers = [
-    "Development Status :: 1 - Planning"
+    "Development Status :: 1 - Planning",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: Apache Software License",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
+    "Typing :: Typed",
 ]
 include = [
     "LICENSE.txt",
     "NOTICE.txt",
     "py.typed",
-    "version.py",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.12"
+pyicu = "^2.12"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4.3"
-pytz = "^2023.3.post1"
+pytest = ">=7.4.3,<9.0.0"
+pytz = ">=2023.3,<2025.0"
 pre-commit = "^3.5.0"
 coverage = "^7.3.2"
-commitizen = "^3.12.0"
+sphinx = "^7.2.6"
+pytest-xdist = "^3.6.1"
 
 [tool.ruff]
 line-length = 120
 
+[tool.ruff.lint]
 # Allow fix for all enabled rules (when `--fix`) is provided.
 fixable = ["ALL"]
 unfixable = []
 
 select = [
     "E",    # pycodestyle (error)
     "F",    # pyflakes
```

