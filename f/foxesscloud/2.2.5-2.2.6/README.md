# Comparing `tmp/foxesscloud-2.2.5.tar.gz` & `tmp/foxesscloud-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\python\FoxESS-Cloud\dist\.tmp-7nf_8d0n\foxesscloud-2.2.5.tar", last modified: Fri Apr 19 13:59:24 2024, max compression
+gzip compressed data, was "F:\python\FoxESS-Cloud\dist\.tmp-p061ai77\foxesscloud-2.2.6.tar", last modified: Fri May 17 11:13:17 2024, max compression
```

## Comparing `foxesscloud-2.2.5.tar` & `foxesscloud-2.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 13:59:24.000000 foxesscloud-2.2.5/
--rw-rw-rw-   0        0        0     1074 2023-08-27 11:13:04.000000 foxesscloud-2.2.5/LICENCE
--rw-rw-rw-   0        0        0    39749 2024-04-19 13:59:24.000000 foxesscloud-2.2.5/PKG-INFO
--rw-rw-rw-   0        0        0    39194 2024-04-19 13:43:40.000000 foxesscloud-2.2.5/README.md
--rw-rw-rw-   0        0        0      635 2024-04-17 17:44:34.000000 foxesscloud-2.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-19 13:59:24.000000 foxesscloud-2.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-19 13:59:24.000000 foxesscloud-2.2.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-19 13:59:24.000000 foxesscloud-2.2.5/src/foxesscloud/
--rw-rw-rw-   0        0        0   174707 2024-04-19 13:41:14.000000 foxesscloud-2.2.5/src/foxesscloud/foxesscloud.py
--rw-rw-rw-   0        0        0   168871 2024-04-19 13:41:14.000000 foxesscloud-2.2.5/src/foxesscloud/openapi.py
-drwxrwxrwx   0        0        0        0 2024-04-19 13:59:24.000000 foxesscloud-2.2.5/src/foxesscloud.egg-info/
--rw-rw-rw-   0        0        0    39749 2024-04-19 13:59:24.000000 foxesscloud-2.2.5/src/foxesscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-19 13:59:24.000000 foxesscloud-2.2.5/src/foxesscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 13:59:24.000000 foxesscloud-2.2.5/src/foxesscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-19 13:59:24.000000 foxesscloud-2.2.5/src/foxesscloud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 11:13:17.000000 foxesscloud-2.2.6/
+-rw-rw-rw-   0        0        0     1074 2023-08-27 11:13:04.000000 foxesscloud-2.2.6/LICENCE
+-rw-rw-rw-   0        0        0    41597 2024-05-17 11:13:17.000000 foxesscloud-2.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    41042 2024-05-17 11:01:10.000000 foxesscloud-2.2.6/README.md
+-rw-rw-rw-   0        0        0      635 2024-05-16 18:18:41.000000 foxesscloud-2.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 11:13:17.000000 foxesscloud-2.2.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 11:13:17.000000 foxesscloud-2.2.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 11:13:17.000000 foxesscloud-2.2.6/src/foxesscloud/
+-rw-rw-rw-   0        0        0   177033 2024-05-17 11:02:52.000000 foxesscloud-2.2.6/src/foxesscloud/foxesscloud.py
+-rw-rw-rw-   0        0        0   171254 2024-05-17 11:03:22.000000 foxesscloud-2.2.6/src/foxesscloud/openapi.py
+drwxrwxrwx   0        0        0        0 2024-05-17 11:13:17.000000 foxesscloud-2.2.6/src/foxesscloud.egg-info/
+-rw-rw-rw-   0        0        0    41597 2024-05-17 11:13:17.000000 foxesscloud-2.2.6/src/foxesscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-17 11:13:17.000000 foxesscloud-2.2.6/src/foxesscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 11:13:17.000000 foxesscloud-2.2.6/src/foxesscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-17 11:13:17.000000 foxesscloud-2.2.6/src/foxesscloud.egg-info/top_level.txt
```

### Comparing `foxesscloud-2.2.5/LICENCE` & `foxesscloud-2.2.6/LICENCE`

 * *Files identical despite different names*

### Comparing `foxesscloud-2.2.5/PKG-INFO` & `foxesscloud-2.2.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: foxesscloud
-Version: 2.2.5
-Summary: library for accessing Fox ESS cloud data using Open API
-Author-email: Tony Matthews <tony@quasair.co.uk>
-Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
-Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
 # FoxESS-Cloud
 
 <a href="https://www.buymeacoffee.com/tonym1958" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174" align="right"></a>
 This site contains sample python code for accessing the Fox cloud data via the REST API used by the Fox ESS Cloud web site and app.
 
 There is also a number of Jupyter Lab notebooks with examples of how to run the sample code.
 
@@ -95,63 +81,74 @@
 
 ```
 f.get_generation()
 f.get_battery()
 f.get_settings()
 f.get_charge()
 f.get_min()
+f.get_flag()
 f.get_schedule()
 
 ```
 Each of these calls will return a dictionary or list containing the relevant information.
 
 get_generation() will return the latest generation information for the device. The results are also stored in f.device as 'generationToday', 'generationMonth' and 'generationTotal'.
 
 get_battery() returns the current battery status, including 'soc', 'volt', 'current', 'power', 'temperature' and 'residual'. The result also updates f.battery.
 
 get_settings() will return the battery settings and is equivalent to get_charge() and get_min(). The results are stored in f.battery_settings. The settings include minSoc, minSocOnGrid, enable charge from grid and the charge times.
 
+get_flag() returns the current scheduler enable / support flags
+
 get_schedule() returns the current work mode / soc schedule settings. The result is stored in f.schedule.
 
 
 ## Inverter Settings
 You can change inverter settings using:
 
 ```
 f.set_min(minSocOnGrid, minSoc)
 f.set_charge(ch1, st1, en1, ch2, st2, en2)
 f.set_group(start, end, mode, min_soc, fdsoc, fdpwr)
-f.get_flag()
-f.set_schedule(enable, groups, template)
+f.set_strategy(strategy)
+f.charge_strategy(st1, en1, st2, en2, min_soc)
+f.set_schedule(groups, enable)
 ```
 
 set_min() applies new SoC settings to the inverter. The parameters update battery_settings:
 + minSocOnGrid: min Soc on Grid setting e.g. 15 = 15%
 + minSoc: min Soc setting e.g. 10 = 10%
 
 set_charge() takes the charge times from the battery_settings and applies these to the inverter. The parameters are optional and will update battery_settings. You should specify all 3 parameter for a time period:
 + ch1: enable charge from grid for period 1 (True or False)
 + st1: the start time for period 1
 + en1: the end time for period 1
 + ch2: enable charge from grid for period 2 (True or False)
 + st2: the start time for period 2
 + en2: the end time for period 2
 
-set_flag() returns the current settings for strategy periods: 'supported' and 'enable'
-
 set_group() returns a time segment structure that can be used to build a list of time segments for set_schedule()
-+ start, end, mode: required parameters
++ start, end, mode: required parameters. end time is exclusive e.g. end at '07:00' will set a period end time of '06:59'
 + min_soc: optional, default is 10
 + fdsoc: optional, default is 10. Used when setting a period with ForceDischarge mode
 + fdpwr: optional, default is 0. Used when setting a period with ForceDischarge mode
 + enable: sets whether this time segment is enable (1) or disabled (0). The default is enabled.
 
+set_strategy() creates a list of groups from the strategy. If strategy is not provided, it uses the strategy for the current tariff.
+
+charge_strategy(): returns a list of groups that describe the strategy for the current tariff and adds the groupd required for charging:
++ st1: the start time for the period when the battery charges from the grid
++ en1: the end time for period 1
++ st2: the start time for period when the battery is held at min_soc
++ en2: the end time for period 2
++ min_soc: the min_soc to use after the charge period, when you don't want the battery to discharge below this level
+
 set_schedule() configures a list of scheduled work mode / soc changes with enable=1. If called with enable=0, any existing schedules are disabled. To enable a schedule, you must provide a list of time segments
-+ enable: 1 to enable schedules, 0 to disable schedules. The default is 1.
 + groups: a time segment or list of time segments created using f.set_group().
++ enable: 1 to enable schedules, 0 to disable schedules. The default is 1.
 
 
 ## Real Time Data
 Real time data reports the latest values for inverter variables, collected every 5 minutes:
 
 ```
 f.invert_ct2 = 1
@@ -294,18 +291,18 @@
 
 ```
 f.charge_needed(forecast, force_charge, forecast_selection, forecast_times, update_setings, show_data, show_plot)
 ```
 
 All the parameters are optional:
 + forecast: the kWh expected tomorrow (optional, see below)
-+ force_charge: 1 any remaining time in a charge period has force charge set, 2 charging uses the entire charge period, 0 None (default)
++ force_charge: 1 any remaining time in a charge period has force charge / min_soc set, 2 charging uses the entire charge period, 0 None (default)
 + forecast_selection: if set to 1, settings are only updated if there is a forecast. Default is 0, generation is used when forecasts are not available
 + forecast_times: a list of hours when forecasts can be obtained. By default, the forecast times for the selected tariff are used (see below)
-+ update_settings: 0 no changes, 1 update charge time, 2 update work mode, 3 update charge time and work mode. The default is 0
++ update_settings: 0 no changes, 1 update charge settings. The default is 0
 + show_data: 1 show battery SoC data, 2 show battery Residual data, 3 show timed data, 4 show timed data before and after charging. The default is 1.
 + show_plot: 1 plot battery SoC data. 2 plot battery Residual, Generation and Consumption. 3 plot 2 + Charge and Discharge The default is 3
 
 ### Modelling
 
 charge_needed() uses a number of models to better estimate the state of the battery.
 
@@ -358,15 +355,15 @@
 use_today: 21.0               # hour when today's generation and consumption data will be used
 min_hours: 0.25               # minimum charge time to set (in decimal hours)
 min_kwh: 0.5                  # minimum charge to add in kwh
 solcast_adjust: 100           # % adjustment to make to Solcast forecast
 solar_adjust:  100            # % adjustment to make to Solar forecast
 forecast_selection: 1         # 1 = only update charge times if forecast is available, 0 = use best available data. Default is 1.
 annual_consumption: None      # optional annual consumption in kWh. If set, this replaces consumption history
-timed_mode: 0                 # 1 = apply timed work mode, 0 = None
+timed_mode: 0                 # 0 = None, 1 = use timed work mode, 2 = strategy mode
 special_contingency: 30       # contingency for special days when consumption might be higher
 special_days: ['12-25', '12-26', '01-01']
 full_charge: None             # day of month (1-28) to do full charge or 'daily' or day of week: 'Mon', 'Tue' etc
 derate_temp: 21               # battery temperature in C when derating charge current is applied
 derate_step: 5                # step size for derating e.g. 21, 16, 11
 derating: [24, 15, 10, 2]     # derated charge current for each temperature step e.g. 21C, 16C, 11C, 6C
 force: 1                      # 1 = disable strategy periods when setting charge. 0 = fail if strategy period has been set.
@@ -376,14 +373,16 @@
 These values are stored / available in f.charge_config.
 
 The default battery open circuit voltage curve versus SoC from 0% to 100% is:
 ```
 lifepo4_curve = [51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50]
 ```
 
+When operating in strategy mode (timed_mode=2), charge_needed will create a schedule that includes the strategy for the tariff with additional time segments added to charge from grid and (optionall) to stop the battery discharging. In other modes, charge_needed() will disable any schedules and set the battery charge times.
+
 This example shows the results reported by charge needed:
 
 ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-b165-20d806b1e7e8)
 
 
 ## Battery Info
 
@@ -467,26 +466,26 @@
 ```
 f.set_tariff('flux')
 ```
 
 When Agile Octopus is selected, a price based charging period is configured using the 30 minute price forecast. For example:
 
 ```
-f.set_tariff('agile', product, region, start_at, end_by, duration, times, forecast_times, work_times, update, weighting, time_shift)
+f.set_tariff('agile', product, region, start_at, end_by, duration, times, forecast_times, strategy, update, weighting, time_shift)
 ```
 
 This gets the latest 30 minute pricing and uses this to work out the best off peak charging period.
 + product: optional Agile Octopus product code (see below). The default is "AGILE-FLEX-22-11-25"
 + region: optional region to use for prices (se below). The default is 'H' (Southern England)
 + start_at: optional earliest start time for charge period in hours, the default is 23:00
 + end_by: optional latest end time for charge period in hours, the default is 08:00
 + duration: optional charge time period in hours, the default is 3 hours. Valid range is 1-6 hours
 + times: a list of charge periods that can be used instead of start_at, end_by and duration (see below)
 + forecast_times: a list of times when a forecast can be obtained from Solcast / forecast.solar
-+ work_times: a list of work modes and times when these are set. The format is [(mode, start, end),...]
++ strategy: an optional list of times and work modes (see below)
 + update: optional, 1 (the default) sets the current tariff to Agile Octopus. Setting to 0 does not change the current tariff
 + weighting: optional, default is None (see below)
 + time_shift: optional system time shift in hours. The default is for system time to be UTC and to apply the current day light saving time (e.g. GMT/BST)
 
 Product codes include: 
 + 'AGILE-18-02-21' = The original version capped at 35p per unit
 + 'AGILE-22-07-22' = The cap rose to 55p
@@ -520,14 +519,21 @@
 Specifying start_at, end_by and duration allows either the AM or PM charging slot for any tariif to be updated, depending on the time. Agile periods will be calculated; othe rtariffs will use the start and end times directly. By default, set_tariff() updates the AM charge period if start_at is after 9pm and end_by is before 8am; it updates the PM charge period if start_at is after 8am and the end_by is before 9pm. Only the relevant AM or PM charge time is updated e.g. if you configure a PM charging period, the AM charginig period is not changed.
 
 To disable a charging period, set duration=0.
 
 set_tariff() can configure multiple charging periods for any tariff using the times parameter instead of start_at, end_by and duration. Times is a list of tuples containing values for start_at, end_by and duration. For example, this parameter configures an AM charging period between 11pm and 8am with a 3 hour period and a PM charging period between 12 noon and 4pm with a 1 hour period:
 + times=[("23:00", "8:00", 3), ("12:00", "16:00", 1)]
 
+'strategy' allows you to configure times when work modes will be changed. The format is a list of dictionary items, containing:
++ 'start', 'end': times in decimal hours or time format. The end time is exclusive so setting an end time of '07:00' will set a schedule that ends at '06:59'
++ 'mode': the work mode to be used from 'SelfUse', 'Feedin', 'Backup', 'ForceCharge', 'ForceDischarge'
++ 'min_soc, 'fdsoc', 'fdpwr': optional values for each work mode. The defaults are 10, 10 and 0 respectively.
+
+The strategy should not include settings for the AM/PM charge times for the tariff. These will be added by charge_needed().
+
 
 # PV Output
 These functions produce CSV data for upload to [pvoutput.org](https://pvoutput.org) including PV generation, Export, Load and Grid consumption by day in Wh. The functions use the energy estimates created from the raw power data (see above). The estimates include PV energy generation that are not otherwise available from the Fox Cloud. Typically, the energy results are within 3% of the values reported by the meters built into the inverter.
 
 
 ## Get PV Output Data
 
@@ -666,15 +672,18 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.5<br>
+2.2.6<br>
+Implement 2 second delay between calls that change inverter settings.
+Added strategy mode (timed_mode=2) to charge_needed().
+Added set_strategy() and charge_strategy() to manage charging schedules and work mode changes.
 Refactor debug messaging.
 Simplify charge_needed() output.
 Added 'target_soc' to charge_needed() settings
 Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50 where there is no battery
 Fix key error when accessing cell volts and temps using an agent / installer account.
 Ensure output is generated if get_battery() fails using battery_info().
 Update f.avg() to include calculation of averages in lists containng None values.
```

#### html2text {}

```diff
@@ -1,16 +1,9 @@
-Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.5 Summary: library for
-accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
-quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
-Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
-for accessing the Fox cloud data via the REST API used by the Fox ESS Cloud web
+# FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code for
+accessing the Fox cloud data via the REST API used by the Fox ESS Cloud web
 site and app. There is also a number of Jupyter Lab notebooks with examples of
 how to run the sample code. This project is not endorsed by, directly
 affiliated with, maintained, authorized, or sponsored by Fox ESS. Please refer
 to the [LICENCE](https://github.com/TonyM1958/FoxESS-Cloud/blob/main/LICENCE)
 for information on copyright, permissions and warranty. # Open API This module
 builds on the Fox Open API to provide a sample code and utilities that can be
 used with your inverter and batteries. + Information on the API can be found
@@ -53,181 +46,189 @@
 there is more than 1 item, the call will show the list of items. To select a
 specific item to work with, call a qualifier: + Site: full or partial name of
 the site + Logger: full or partial serial number + Inverter: full or partial
 serial number When an item is selected, the functions returns a dictionary
 containing item details and saves these to a global variable (f.site, f.logger,
 f.device respectively) Once an inverter is selected, you can make other calls
 to get information: ``` f.get_generation() f.get_battery() f.get_settings()
-f.get_charge() f.get_min() f.get_schedule() ``` Each of these calls will return
-a dictionary or list containing the relevant information. get_generation() will
-return the latest generation information for the device. The results are also
-stored in f.device as 'generationToday', 'generationMonth' and
-'generationTotal'. get_battery() returns the current battery status, including
-'soc', 'volt', 'current', 'power', 'temperature' and 'residual'. The result
-also updates f.battery. get_settings() will return the battery settings and is
-equivalent to get_charge() and get_min(). The results are stored in
+f.get_charge() f.get_min() f.get_flag() f.get_schedule() ``` Each of these
+calls will return a dictionary or list containing the relevant information.
+get_generation() will return the latest generation information for the device.
+The results are also stored in f.device as 'generationToday', 'generationMonth'
+and 'generationTotal'. get_battery() returns the current battery status,
+including 'soc', 'volt', 'current', 'power', 'temperature' and 'residual'. The
+result also updates f.battery. get_settings() will return the battery settings
+and is equivalent to get_charge() and get_min(). The results are stored in
 f.battery_settings. The settings include minSoc, minSocOnGrid, enable charge
-from grid and the charge times. get_schedule() returns the current work mode /
-soc schedule settings. The result is stored in f.schedule. ## Inverter Settings
-You can change inverter settings using: ``` f.set_min(minSocOnGrid, minSoc)
+from grid and the charge times. get_flag() returns the current scheduler enable
+/ support flags get_schedule() returns the current work mode / soc schedule
+settings. The result is stored in f.schedule. ## Inverter Settings You can
+change inverter settings using: ``` f.set_min(minSocOnGrid, minSoc)
 f.set_charge(ch1, st1, en1, ch2, st2, en2) f.set_group(start, end, mode,
-min_soc, fdsoc, fdpwr) f.get_flag() f.set_schedule(enable, groups, template)
-``` set_min() applies new SoC settings to the inverter. The parameters update
-battery_settings: + minSocOnGrid: min Soc on Grid setting e.g. 15 = 15% +
-minSoc: min Soc setting e.g. 10 = 10% set_charge() takes the charge times from
-the battery_settings and applies these to the inverter. The parameters are
-optional and will update battery_settings. You should specify all 3 parameter
-for a time period: + ch1: enable charge from grid for period 1 (True or False)
-+ st1: the start time for period 1 + en1: the end time for period 1 + ch2:
-enable charge from grid for period 2 (True or False) + st2: the start time for
-period 2 + en2: the end time for period 2 set_flag() returns the current
-settings for strategy periods: 'supported' and 'enable' set_group() returns a
-time segment structure that can be used to build a list of time segments for
-set_schedule() + start, end, mode: required parameters + min_soc: optional,
-default is 10 + fdsoc: optional, default is 10. Used when setting a period with
-ForceDischarge mode + fdpwr: optional, default is 0. Used when setting a period
-with ForceDischarge mode + enable: sets whether this time segment is enable (1)
-or disabled (0). The default is enabled. set_schedule() configures a list of
-scheduled work mode / soc changes with enable=1. If called with enable=0, any
-existing schedules are disabled. To enable a schedule, you must provide a list
-of time segments + enable: 1 to enable schedules, 0 to disable schedules. The
-default is 1. + groups: a time segment or list of time segments created using
-f.set_group(). ## Real Time Data Real time data reports the latest values for
-inverter variables, collected every 5 minutes: ``` f.invert_ct2 = 1 f.get_vars
-() f.get_real(v) ``` f.invert_ct2 determines how the meterPower2 data is
-handled. When invert_ct2 = 0, meterPower2 produces +ve power values during
-secondary generation. If meterPower2 produces -ve power values during secondary
-generation, setting invert_ct2 = 1 will flip the values so they are +ve when
-generating. The default setting is 1 (invert). f.get_vars() returns the list of
-variables that can be queried. This also stores the information: + f.var_table:
-a table, indexed by variable that contains information such as the name and
-unit. ++ f.var_list: a list of all the variables that are available There are
-also pre-defined lists: + power_vars lists the main power variables provided by
-the inverter + battery_vars lists the main variables relevant to the battery /
-BMS f.get_real returns the latest values for a list of variables. + v is a
-variable, or list of variables. The default is to return the latest value for
-all available variables ## History Data History data reports inverter
-variables, collected every 5 minutes, on a given date / time and period: ```
-f.get_history(time_span, d, v, summary, save, load, plot) ``` + time_span
-determines the period covered by the data, for example, 'hour', 'day' or
-'week'. The default is 'hour' + d is a date and time in the format 'YYYY-MM-DD
-HH:MM:SS'. The default is today's date and time. d may also be a list of dates
-+ v is a variable, or list of variables (see above) + summary is optional - see
-below + save: set to the root part of a filename to save the results + load:
-set to the full filename to load previously saved results + plot is optional. 1
-plots the results with a chart per unit and per day. 2 plots multiple days on
-the same chart. Default is 0, no plots The setting for invert_ct2 is applied to
-history data for meterPower2, so +ve values are returned for secondary
-generation. f.sample_time is set to the sample time in minutes for the data
-processed, rounded to f.sample_rounding samples per minute. Data generation for
-the full list of raw_vars can be slow and return a lot of data, so it's best to
-select the vars you want from the list if you can. For example, this Jupyter
-Lab cell will load an inverter and return power data at 5 minute intervals for
-the 17th June 2023: ``` d = '2023-06-17 00:00:00' result=f.get_history('day',
-d=d, v=f.power_vars) ``` Setting the optional parameter 'summary' when calling
-get_raw() provides a summary of the raw data + summary = 0: basic history data,
-no summary + summary = 1: summary is calculated + summary = 2: summary is
-calculated and raw data is removed to save time / space + summary = 3: as (2)
-but for energy only, an hourly cumulative state is also generated, similar to
-the state used in Home Assistant long term statistics The summary includes the
-following attributes: + count: the number of data points + average: the average
-value of the data points + max: the maximum value of the data points +
-max_time: the time when the maximum value occured (HH:MM) + min: the minimum
-value of the data points + min_time: the time when the minimum value occured
-(HH:MM) For power values (unit = kW), the summary performs a Riemann sum of the
-data, integrating kW over the day to estimate energy in kWh. In this case, the
-following attributes are also added: + kwh: the total energy generated or
-consumed + kwh_off: the total energy consumed or generated during the off-peak
-time of use + kwh_peak: the total energy consumed or generated during the peak
-time of use + kwh_neg: the total energy from -ve power flow (all other totals
-are based on +ve power flow) This example shows power graphs for today and
-yesterday: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/
-d84c55c9-4f4c-431d-bc55-d7796b7e4fea) ## Report Data Report data provides
-information on the energy produced by the inverter, battery charge and
-discharge energy, grid consumption and feed-in energy and home energy
-consumption: ``` f.get_report(report_type, d, v, summary, save, load, plot,
-station) ``` + report_type sets the period covered by the report and is one of
-'day', 'week', 'month', 'year': + when 'day' is selected, energy is reported
-each hour through the day + when 'week' is selected, energy is reported for the
-7 days up to and including the date + when 'month' is selected, energy is
-reported each day through the month + when 'year' is selected, energy is
-reported each month through the year + d is a date and time in the format
-'YYYY-MM-DD HH:MM:SS'. The default is yesterday. d may also be a list of dates
-+ v is a variable, or list of variables. The default is to use report_vars +
-summary is optional - see below + save: set to the root part of a filename to
+min_soc, fdsoc, fdpwr) f.set_strategy(strategy) f.charge_strategy(st1, en1,
+st2, en2, min_soc) f.set_schedule(groups, enable) ``` set_min() applies new SoC
+settings to the inverter. The parameters update battery_settings: +
+minSocOnGrid: min Soc on Grid setting e.g. 15 = 15% + minSoc: min Soc setting
+e.g. 10 = 10% set_charge() takes the charge times from the battery_settings and
+applies these to the inverter. The parameters are optional and will update
+battery_settings. You should specify all 3 parameter for a time period: + ch1:
+enable charge from grid for period 1 (True or False) + st1: the start time for
+period 1 + en1: the end time for period 1 + ch2: enable charge from grid for
+period 2 (True or False) + st2: the start time for period 2 + en2: the end time
+for period 2 set_group() returns a time segment structure that can be used to
+build a list of time segments for set_schedule() + start, end, mode: required
+parameters. end time is exclusive e.g. end at '07:00' will set a period end
+time of '06:59' + min_soc: optional, default is 10 + fdsoc: optional, default
+is 10. Used when setting a period with ForceDischarge mode + fdpwr: optional,
+default is 0. Used when setting a period with ForceDischarge mode + enable:
+sets whether this time segment is enable (1) or disabled (0). The default is
+enabled. set_strategy() creates a list of groups from the strategy. If strategy
+is not provided, it uses the strategy for the current tariff. charge_strategy
+(): returns a list of groups that describe the strategy for the current tariff
+and adds the groupd required for charging: + st1: the start time for the period
+when the battery charges from the grid + en1: the end time for period 1 + st2:
+the start time for period when the battery is held at min_soc + en2: the end
+time for period 2 + min_soc: the min_soc to use after the charge period, when
+you don't want the battery to discharge below this level set_schedule()
+configures a list of scheduled work mode / soc changes with enable=1. If called
+with enable=0, any existing schedules are disabled. To enable a schedule, you
+must provide a list of time segments + groups: a time segment or list of time
+segments created using f.set_group(). + enable: 1 to enable schedules, 0 to
+disable schedules. The default is 1. ## Real Time Data Real time data reports
+the latest values for inverter variables, collected every 5 minutes: ```
+f.invert_ct2 = 1 f.get_vars() f.get_real(v) ``` f.invert_ct2 determines how the
+meterPower2 data is handled. When invert_ct2 = 0, meterPower2 produces +ve
+power values during secondary generation. If meterPower2 produces -ve power
+values during secondary generation, setting invert_ct2 = 1 will flip the values
+so they are +ve when generating. The default setting is 1 (invert). f.get_vars
+() returns the list of variables that can be queried. This also stores the
+information: + f.var_table: a table, indexed by variable that contains
+information such as the name and unit. ++ f.var_list: a list of all the
+variables that are available There are also pre-defined lists: + power_vars
+lists the main power variables provided by the inverter + battery_vars lists
+the main variables relevant to the battery / BMS f.get_real returns the latest
+values for a list of variables. + v is a variable, or list of variables. The
+default is to return the latest value for all available variables ## History
+Data History data reports inverter variables, collected every 5 minutes, on a
+given date / time and period: ``` f.get_history(time_span, d, v, summary, save,
+load, plot) ``` + time_span determines the period covered by the data, for
+example, 'hour', 'day' or 'week'. The default is 'hour' + d is a date and time
+in the format 'YYYY-MM-DD HH:MM:SS'. The default is today's date and time. d
+may also be a list of dates + v is a variable, or list of variables (see above)
++ summary is optional - see below + save: set to the root part of a filename to
 save the results + load: set to the full filename to load previously saved
-results + plot is optional. 1 to plot results + station is optional. 1 gets
-data for a site (using f.station_id), 0 gets data for a device (using
-f.device_id). The default is 0. The list of variables that can be reported on
-is stored in f.report_vars. Note that reporting by 'day' produces inaccurate
-hourly data, where the sum does not reconcile with the daily total given in the
-monthly report. To correct this, reporting by day also gets the monthly data
-and uses the daily total to correctly report the total. Setting the optional
-parameter 'summary' when calling get_report() provides a summary of the report
-data: + summary = 0: basic report data, no summary. report_type cannot be
-'week' + summary = 1: summary is calculated + summary = 2: corrected total only
-is reported to save time / space. report_type must be 'day' The result data for
-each variable includes the following attributes when summary=2 + 'variable':
-name of the data set + 'total': corrected total of the data items When
-summary=1, the following items are also added: + 'data': 'index' and 'value' of
-each data point + 'date': that was used to produce the report + 'count': the
-number of data items + 'sum': the sum of the data items + 'max': the biggest
-value in 'data' + 'max_index': the index of the biggest value in 'data' +
-'min': the smallest value in 'data' + 'min_index': the index of the smallest
-value in 'data' + 'average': corrected average of the data items For example,
-this Jupyter Lab cell will report energy data by day for the month of June
-2023: ``` d = '2023-06-17' result=f.get_report('month', d=d) ``` This example
-plots weekly data: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
-63789168/f408a010-9600-4b2f-979f-83e32d960586) # Built-in Utilities and
-Operations The previous section provides functions that can be used to access
-and control your inverter. This section covers utilities and operations that
-build upon these functions. ## Charge Needed Uses forecast PV yield for
-tomorrow to work out if charging from grid is needed tonight to deliver the
-expected consumption for tomorrow. If charging is needed, the charge times are
-configured. If charging is not needed, the charge times are cleared. The
-results are sent to the inverter. ``` f.charge_needed(forecast, force_charge,
-forecast_selection, forecast_times, update_setings, show_data, show_plot) ```
-All the parameters are optional: + forecast: the kWh expected tomorrow
-(optional, see below) + force_charge: 1 any remaining time in a charge period
-has force charge set, 2 charging uses the entire charge period, 0 None
-(default) + forecast_selection: if set to 1, settings are only updated if there
-is a forecast. Default is 0, generation is used when forecasts are not
-available + forecast_times: a list of hours when forecasts can be obtained. By
-default, the forecast times for the selected tariff are used (see below) +
-update_settings: 0 no changes, 1 update charge time, 2 update work mode, 3
-update charge time and work mode. The default is 0 + show_data: 1 show battery
-SoC data, 2 show battery Residual data, 3 show timed data, 4 show timed data
-before and after charging. The default is 1. + show_plot: 1 plot battery SoC
-data. 2 plot battery Residual, Generation and Consumption. 3 plot 2 + Charge
-and Discharge The default is 3 ### Modelling charge_needed() uses a number of
-models to better estimate the state of the battery. **Manual Consumption:** You
-can provide your 'annual_consumption' in kWh e.g. 5500. This figure is factored
-down to a daily consumption by dividing by 365 and applying **f.seasonality**.
-This normally decreases consumption in the summer and increases it in winter.
-Seasonality is a list of weightings by month for Jan, Feb, Mar, Apr etc. Preset
-lists are 'f.high_seasonality' (recommend where electric heating is ued),
-'f.medium_seasonality' (default) amd 'f.no_seasonality' (all months the same).
-The daily consumption is profiled by hour using **f.daily_consumption**. This
-maps your consumption for a day to the hours when more or less energy is
-consumed. It is a list of 24 values for the times 00, 01, 02, 03 .. 23. Preset
-lists are 'f.high_profile' (larger peaks at 8am and 6pm), 'f.medium_profile'
-(default, more balanced) and 'f.no_profile' (flat). **Historic Consumption:**
-If annual_consumption is not provided, your consumption history is used. By
-default, this looks at your average consumption for the last 3 days using the
-load power reported by your inverter. For systems with multiple inverters where
-CT2 is not connected, the load power may not be correct. For this and other
-cases where you want to set your consumption, provide your annual_consumption.
-**Manual Forecast:** You can provide a specific 'forecast' in kWh e.g. 20. This
-is profiled using **f.seasonal_sun** to map solar generation to the time of
-day. The mapping is broken down into 4 seasons: winter, spring, summer and
-autumn (winter is Dec, Jan, Feb, spring is Mar, Apr, May etc). There are 4
-preset lists: 'f.winter_sun', 'f.spring_sun', 'f.summer_sun' and
-'f.autumn_sun'. Seasonal_sun is used for manual and historic forecasts
-**Solcast:** If you provide an API key for Solcast, your forecast will be
-downloaded after 9pm each day and used as the basis for your next days
+results + plot is optional. 1 plots the results with a chart per unit and per
+day. 2 plots multiple days on the same chart. Default is 0, no plots The
+setting for invert_ct2 is applied to history data for meterPower2, so +ve
+values are returned for secondary generation. f.sample_time is set to the
+sample time in minutes for the data processed, rounded to f.sample_rounding
+samples per minute. Data generation for the full list of raw_vars can be slow
+and return a lot of data, so it's best to select the vars you want from the
+list if you can. For example, this Jupyter Lab cell will load an inverter and
+return power data at 5 minute intervals for the 17th June 2023: ``` d = '2023-
+06-17 00:00:00' result=f.get_history('day', d=d, v=f.power_vars) ``` Setting
+the optional parameter 'summary' when calling get_raw() provides a summary of
+the raw data + summary = 0: basic history data, no summary + summary = 1:
+summary is calculated + summary = 2: summary is calculated and raw data is
+removed to save time / space + summary = 3: as (2) but for energy only, an
+hourly cumulative state is also generated, similar to the state used in Home
+Assistant long term statistics The summary includes the following attributes: +
+count: the number of data points + average: the average value of the data
+points + max: the maximum value of the data points + max_time: the time when
+the maximum value occured (HH:MM) + min: the minimum value of the data points +
+min_time: the time when the minimum value occured (HH:MM) For power values
+(unit = kW), the summary performs a Riemann sum of the data, integrating kW
+over the day to estimate energy in kWh. In this case, the following attributes
+are also added: + kwh: the total energy generated or consumed + kwh_off: the
+total energy consumed or generated during the off-peak time of use + kwh_peak:
+the total energy consumed or generated during the peak time of use + kwh_neg:
+the total energy from -ve power flow (all other totals are based on +ve power
+flow) This example shows power graphs for today and yesterday: ![image](https:/
+/github.com/TonyM1958/FoxESS-Cloud/assets/63789168/d84c55c9-4f4c-431d-bc55-
+d7796b7e4fea) ## Report Data Report data provides information on the energy
+produced by the inverter, battery charge and discharge energy, grid consumption
+and feed-in energy and home energy consumption: ``` f.get_report(report_type,
+d, v, summary, save, load, plot, station) ``` + report_type sets the period
+covered by the report and is one of 'day', 'week', 'month', 'year': + when
+'day' is selected, energy is reported each hour through the day + when 'week'
+is selected, energy is reported for the 7 days up to and including the date +
+when 'month' is selected, energy is reported each day through the month + when
+'year' is selected, energy is reported each month through the year + d is a
+date and time in the format 'YYYY-MM-DD HH:MM:SS'. The default is yesterday. d
+may also be a list of dates + v is a variable, or list of variables. The
+default is to use report_vars + summary is optional - see below + save: set to
+the root part of a filename to save the results + load: set to the full
+filename to load previously saved results + plot is optional. 1 to plot results
++ station is optional. 1 gets data for a site (using f.station_id), 0 gets data
+for a device (using f.device_id). The default is 0. The list of variables that
+can be reported on is stored in f.report_vars. Note that reporting by 'day'
+produces inaccurate hourly data, where the sum does not reconcile with the
+daily total given in the monthly report. To correct this, reporting by day also
+gets the monthly data and uses the daily total to correctly report the total.
+Setting the optional parameter 'summary' when calling get_report() provides a
+summary of the report data: + summary = 0: basic report data, no summary.
+report_type cannot be 'week' + summary = 1: summary is calculated + summary =
+2: corrected total only is reported to save time / space. report_type must be
+'day' The result data for each variable includes the following attributes when
+summary=2 + 'variable': name of the data set + 'total': corrected total of the
+data items When summary=1, the following items are also added: + 'data':
+'index' and 'value' of each data point + 'date': that was used to produce the
+report + 'count': the number of data items + 'sum': the sum of the data items +
+'max': the biggest value in 'data' + 'max_index': the index of the biggest
+value in 'data' + 'min': the smallest value in 'data' + 'min_index': the index
+of the smallest value in 'data' + 'average': corrected average of the data
+items For example, this Jupyter Lab cell will report energy data by day for the
+month of June 2023: ``` d = '2023-06-17' result=f.get_report('month', d=d) ```
+This example plots weekly data: ![image](https://github.com/TonyM1958/FoxESS-
+Cloud/assets/63789168/f408a010-9600-4b2f-979f-83e32d960586) # Built-in
+Utilities and Operations The previous section provides functions that can be
+used to access and control your inverter. This section covers utilities and
+operations that build upon these functions. ## Charge Needed Uses forecast PV
+yield for tomorrow to work out if charging from grid is needed tonight to
+deliver the expected consumption for tomorrow. If charging is needed, the
+charge times are configured. If charging is not needed, the charge times are
+cleared. The results are sent to the inverter. ``` f.charge_needed(forecast,
+force_charge, forecast_selection, forecast_times, update_setings, show_data,
+show_plot) ``` All the parameters are optional: + forecast: the kWh expected
+tomorrow (optional, see below) + force_charge: 1 any remaining time in a charge
+period has force charge / min_soc set, 2 charging uses the entire charge
+period, 0 None (default) + forecast_selection: if set to 1, settings are only
+updated if there is a forecast. Default is 0, generation is used when forecasts
+are not available + forecast_times: a list of hours when forecasts can be
+obtained. By default, the forecast times for the selected tariff are used (see
+below) + update_settings: 0 no changes, 1 update charge settings. The default
+is 0 + show_data: 1 show battery SoC data, 2 show battery Residual data, 3 show
+timed data, 4 show timed data before and after charging. The default is 1. +
+show_plot: 1 plot battery SoC data. 2 plot battery Residual, Generation and
+Consumption. 3 plot 2 + Charge and Discharge The default is 3 ### Modelling
+charge_needed() uses a number of models to better estimate the state of the
+battery. **Manual Consumption:** You can provide your 'annual_consumption' in
+kWh e.g. 5500. This figure is factored down to a daily consumption by dividing
+by 365 and applying **f.seasonality**. This normally decreases consumption in
+the summer and increases it in winter. Seasonality is a list of weightings by
+month for Jan, Feb, Mar, Apr etc. Preset lists are 'f.high_seasonality'
+(recommend where electric heating is ued), 'f.medium_seasonality' (default) amd
+'f.no_seasonality' (all months the same). The daily consumption is profiled by
+hour using **f.daily_consumption**. This maps your consumption for a day to the
+hours when more or less energy is consumed. It is a list of 24 values for the
+times 00, 01, 02, 03 .. 23. Preset lists are 'f.high_profile' (larger peaks at
+8am and 6pm), 'f.medium_profile' (default, more balanced) and 'f.no_profile'
+(flat). **Historic Consumption:** If annual_consumption is not provided, your
+consumption history is used. By default, this looks at your average consumption
+for the last 3 days using the load power reported by your inverter. For systems
+with multiple inverters where CT2 is not connected, the load power may not be
+correct. For this and other cases where you want to set your consumption,
+provide your annual_consumption. **Manual Forecast:** You can provide a
+specific 'forecast' in kWh e.g. 20. This is profiled using **f.seasonal_sun**
+to map solar generation to the time of day. The mapping is broken down into 4
+seasons: winter, spring, summer and autumn (winter is Dec, Jan, Feb, spring is
+Mar, Apr, May etc). There are 4 preset lists: 'f.winter_sun', 'f.spring_sun',
+'f.summer_sun' and 'f.autumn_sun'. Seasonal_sun is used for manual and historic
+forecasts **Solcast:** If you provide an API key for Solcast, your forecast
+will be downloaded after 9pm each day and used as the basis for your next days
 generation (see below). **Solar:** if you configure one or more
 **f.solar_array**, forecast.solar will be called to provide a forrecast for
 your next days generation (see below). **Historic Generation:** If 'forecast'
 is not provided and Solcast and Solar forecasts are not available, your
 generation history is used. By default, this looks at your average solar
 generation for the last 3 days and applies the **f.seasonal_sun** profile.
 Note: if using Solcast or forecast.solar, calls to the API are very limited so
@@ -264,50 +265,54 @@
 e.g. Saturdays use_today: 21.0 # hour when today's generation and consumption
 data will be used min_hours: 0.25 # minimum charge time to set (in decimal
 hours) min_kwh: 0.5 # minimum charge to add in kwh solcast_adjust: 100 # %
 adjustment to make to Solcast forecast solar_adjust: 100 # % adjustment to make
 to Solar forecast forecast_selection: 1 # 1 = only update charge times if
 forecast is available, 0 = use best available data. Default is 1.
 annual_consumption: None # optional annual consumption in kWh. If set, this
-replaces consumption history timed_mode: 0 # 1 = apply timed work mode, 0 =
-None special_contingency: 30 # contingency for special days when consumption
-might be higher special_days: ['12-25', '12-26', '01-01'] full_charge: None #
-day of month (1-28) to do full charge or 'daily' or day of week: 'Mon', 'Tue'
-etc derate_temp: 21 # battery temperature in C when derating charge current is
-applied derate_step: 5 # step size for derating e.g. 21, 16, 11 derating: [24,
-15, 10, 2] # derated charge current for each temperature step e.g. 21C, 16C,
-11C, 6C force: 1 # 1 = disable strategy periods when setting charge. 0 = fail
-if strategy period has been set. data_wrap: 6 # data items to show per line
-target_soc: None # target soc for charging ``` These values are stored /
-available in f.charge_config. The default battery open circuit voltage curve
-versus SoC from 0% to 100% is: ``` lifepo4_curve = [51.30, 52.00, 52.30, 52.40,
-52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ``` This example shows the
-results reported by charge needed: ![image](https://github.com/TonyM1958/
-FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-b165-20d806b1e7e8) ## Battery
-Info Provides detailed information on the current state of the batteries: ```
-f.battery_info(count, plot, log) f.battery_monitor(interval, run, log, save,
-count) ``` battery_info() prints information on the battery and cells: + count:
-optional over-ride. The default is based on factorising the number of cells
-reported by 16 or 18 to work out the number of batteries. + plot: 1 plot the
-cell voltages for each battery, 2 plot the cell temperatueres, 0 don't plot.
-The default is 1 + log: see below. Default is 0 battery_monitor() runs
-battery_info() in log mode on a schedule to provide information on the battery
-status over a period of time: + interval: the time in minutes between log
-entries. The default is 30 minutes + run: the number of log entries to create.
-The default is 48 i.e. every 30 minues for 24 hours in total + log: 0 =
-display, 1 = log battery info, 2 = add cell volts, 3 = add cell temps. The
-default is 1 + save: name of a CSV file to write log data to + count: optional
-over-ride for the number of batteries This is an example of the output from
-battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
-63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ``` f.date_list
-(s, e, limit, span, today) ``` Returns a list of dates in the format 'YYYY-MM-
-DD'. This function will not return dates in the future. The last date will be
-yesterday or today (if today is True). All parameters are optional: + s: start
-date + e: end date + limit: maximum number of days. The default is 200 + span:
-the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
+replaces consumption history timed_mode: 0 # 0 = None, 1 = use timed work mode,
+2 = strategy mode special_contingency: 30 # contingency for special days when
+consumption might be higher special_days: ['12-25', '12-26', '01-01']
+full_charge: None # day of month (1-28) to do full charge or 'daily' or day of
+week: 'Mon', 'Tue' etc derate_temp: 21 # battery temperature in C when derating
+charge current is applied derate_step: 5 # step size for derating e.g. 21, 16,
+11 derating: [24, 15, 10, 2] # derated charge current for each temperature step
+e.g. 21C, 16C, 11C, 6C force: 1 # 1 = disable strategy periods when setting
+charge. 0 = fail if strategy period has been set. data_wrap: 6 # data items to
+show per line target_soc: None # target soc for charging ``` These values are
+stored / available in f.charge_config. The default battery open circuit voltage
+curve versus SoC from 0% to 100% is: ``` lifepo4_curve = [51.30, 52.00, 52.30,
+52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ``` When operating in
+strategy mode (timed_mode=2), charge_needed will create a schedule that
+includes the strategy for the tariff with additional time segments added to
+charge from grid and (optionall) to stop the battery discharging. In other
+modes, charge_needed() will disable any schedules and set the battery charge
+times. This example shows the results reported by charge needed: ![image]
+(https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-
+b165-20d806b1e7e8) ## Battery Info Provides detailed information on the current
+state of the batteries: ``` f.battery_info(count, plot, log) f.battery_monitor
+(interval, run, log, save, count) ``` battery_info() prints information on the
+battery and cells: + count: optional over-ride. The default is based on
+factorising the number of cells reported by 16 or 18 to work out the number of
+batteries. + plot: 1 plot the cell voltages for each battery, 2 plot the cell
+temperatueres, 0 don't plot. The default is 1 + log: see below. Default is 0
+battery_monitor() runs battery_info() in log mode on a schedule to provide
+information on the battery status over a period of time: + interval: the time
+in minutes between log entries. The default is 30 minutes + run: the number of
+log entries to create. The default is 48 i.e. every 30 minues for 24 hours in
+total + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add
+cell temps. The default is 1 + save: name of a CSV file to write log data to +
+count: optional over-ride for the number of batteries This is an example of the
+output from battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/
+assets/63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ```
+f.date_list(s, e, limit, span, today) ``` Returns a list of dates in the format
+'YYYY-MM-DD'. This function will not return dates in the future. The last date
+will be yesterday or today (if today is True). All parameters are optional: +
+s: start date + e: end date + limit: maximum number of days. The default is 200
++ span: the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
 'weekday' + today: 1 allows today to be included, 2 allows future dates to be
 included. Default is 0, date list will stop at yesterday You can use 'span' as
 follows: + 'day' provides a single day + 'week' will provide the dates of 7
 consequetive days + 'month' will provide the dates of the days up to the same
 date in the preceeding (or follwing) month + '2days' will provide the dates of
 yesterday and today + 'weekday' will provide the dates of the same day of the
 week, going backwards (or forwards) up to 7 weeks ``` f.british_summer_time(d)
@@ -334,145 +339,156 @@
 to 23:59 + Eco 7: Economy 7: off-peak from 00:30 to 07:30 GMT (01:30 to 08:30
 during BST) Custom periods can be configured for specific times if required: +
 Custom: charging from 02:00 to 05:00, no off-peak or peak times, forecasts from
 22:00 to 23:59 The active tariff is configured by calling 'f.set_tariff() with
 the name of the tariff to use: ``` f.set_tariff('flux') ``` When Agile Octopus
 is selected, a price based charging period is configured using the 30 minute
 price forecast. For example: ``` f.set_tariff('agile', product, region,
-start_at, end_by, duration, times, forecast_times, work_times, update,
-weighting, time_shift) ``` This gets the latest 30 minute pricing and uses this
-to work out the best off peak charging period. + product: optional Agile
-Octopus product code (see below). The default is "AGILE-FLEX-22-11-25" +
-region: optional region to use for prices (se below). The default is 'H'
-(Southern England) + start_at: optional earliest start time for charge period
-in hours, the default is 23:00 + end_by: optional latest end time for charge
-period in hours, the default is 08:00 + duration: optional charge time period
-in hours, the default is 3 hours. Valid range is 1-6 hours + times: a list of
-charge periods that can be used instead of start_at, end_by and duration (see
-below) + forecast_times: a list of times when a forecast can be obtained from
-Solcast / forecast.solar + work_times: a list of work modes and times when
-these are set. The format is [(mode, start, end),...] + update: optional, 1
-(the default) sets the current tariff to Agile Octopus. Setting to 0 does not
-change the current tariff + weighting: optional, default is None (see below) +
-time_shift: optional system time shift in hours. The default is for system time
-to be UTC and to apply the current day light saving time (e.g. GMT/BST) Product
-codes include: + 'AGILE-18-02-21' = The original version capped at 35p per unit
-+ 'AGILE-22-07-22' = The cap rose to 55p + 'AGILE-22-08-31' = The cap was
-increased to 78p + 'AGILE-VAR-22-10-19' = This version raised the cap to Â£1
-per unit and also introduced a new formula. + 'AGILE-FLEX-22-11-25' = Cap stays
-at Â£1 per unit but new formula only deducts 17.9p from higher unit prices
-(default) Region codes include: + 'A' = Eastern England + 'B' = East Midlands +
-'C' = London + 'D' = Merseyside and Northern Wales + 'E' = West Midlands + 'F'
-= North Eastern England + 'G' = North Western England + 'H' = Southern England
-(default) + 'J' = South Eastern England + 'K' = Southern Wales + 'L' = South
-Western England + 'M' = Yorkshire + 'N' = Southern Scotland + 'P' = Northern
-Scotland Pricing for tomorrow is updated around 4pm each day. If run before
-this time, prices from yesterday are used. By default, prices for tomorrow are
-fetched after 5pm. The setting for this is: + f.agile_update_time = 17 The best
-charging period is determined based on the weighted average of the 30 minute
-prices over the duration. The default is flat (all prices are weighted
-equally). You can change the weighting by providing 'weighting'. The following
-preset weightings are provided: + f.front_loaded: [1.0, 0.9, 0.8, 0.7, 0.6,
-0.5] + f.first_hour: [1.0, 1.0] Specifying start_at, end_by and duration allows
-either the AM or PM charging slot for any tariif to be updated, depending on
-the time. Agile periods will be calculated; othe rtariffs will use the start
-and end times directly. By default, set_tariff() updates the AM charge period
-if start_at is after 9pm and end_by is before 8am; it updates the PM charge
-period if start_at is after 8am and the end_by is before 9pm. Only the relevant
-AM or PM charge time is updated e.g. if you configure a PM charging period, the
-AM charginig period is not changed. To disable a charging period, set
-duration=0. set_tariff() can configure multiple charging periods for any tariff
-using the times parameter instead of start_at, end_by and duration. Times is a
-list of tuples containing values for start_at, end_by and duration. For
-example, this parameter configures an AM charging period between 11pm and 8am
-with a 3 hour period and a PM charging period between 12 noon and 4pm with a 1
-hour period: + times=[("23:00", "8:00", 3), ("12:00", "16:00", 1)] # PV Output
-These functions produce CSV data for upload to [pvoutput.org](https://
-pvoutput.org) including PV generation, Export, Load and Grid consumption by day
-in Wh. The functions use the energy estimates created from the raw power data
-(see above). The estimates include PV energy generation that are not otherwise
-available from the Fox Cloud. Typically, the energy results are within 3% of
-the values reported by the meters built into the inverter. ## Get PV Output
-Data Returns CSV upload data using the [API format](https://pvoutput.org/help/
-api_specification.html#csv-data-parameter): ``` f.get_pvoutput(d, tou) ``` + d
-is the date or a list of dates, to get data for. The default is yesterday +
-tou: optional, setting tou=1 uploads data with time of use. The default, tou=0
-does not split data and is more accurate. You can copy and paste the output
-data to the pvoutput data CSV Loader, using the following settings: ![image]
-(https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/21459cdc-a943-4e9d-
-a204-7efd45a422d8) For example, this Jupyer Lab cell will provide a CSV data
-upload for June 2023: ``` f.get_pvoutput(f.date_list('2023-06-01', '2023-06-
-30')) ``` ## Set PV Output Data Loads CSV data directly using the PV Ouput API:
-``` f.set_pvoutput(d, system_id, tou, push) ``` + d is optional and is the
-date, or a list of dates, to upload + system_id is optional and allow you to
-select where data is uploaded to (where you have more than 1 registered system)
-+ tou: optional, setting tou=1 uploads data with time of use. The default,
-tou=0 does not split data and is more accurate + push: optional. 0 = do not
-sent to pushover, 1 = send summary to pushover, 2 = send first day summary only
-# Solar Forecasting # Solcast Get and display solar data from your solcast.com
-account using your API key: ``` f.solcast_api_key = "my.solcast_api_key" fcast
-= f.Solcast() print(fcast) ``` Returns a 7 day forecast. Optional parameters
-are: + days: number of days to get. The default is 7 + estimated: whether to
-get history / estimated data. 1 = yes, 0 = no. Default is 0. + reload: cached
-data handling. 0 = use saved data, 1 = fetch new data, 2 = use saved data for
-today (default) + quiet: True to stop Solcast producing progress messages
-Forecast data is saved to f.solcast_save. The default is 'solcast.txt'. ```
-fcast.plot_daily() fcast.plot_hourly(day) ``` Plots the estimate / forecast
-data. plot_daily() plots the daily yield. plot_hourly() plots each day
-separately. + day: optional. 'today', 'tomorrow', 'all' or a specific list of
-dates. The default is to plot today and tomorrow # Forecast.solar Get and
-display solar data from forecast.solar for today and tomorrow: ```
-f.solar_array('South', lat=51.1789, lon=-1.8262, kwp=6.4) ``` You need to
-configure your solar arrays by calling f.solar_array(). This takes the
-following parameters: + name: the name of each of your arrays + lat: the
-latitude where the array is located. The default is Stonehenge. + lon: the
-longitude where the array is located. The default is Stonehenge. + dec: the
-declination of the array - 0 is lying flat and 90 is vertical. Default is 30 +
-az: azimuth of the array. 0 is pointing due South, -90 is pointing East, 90 is
-pointing West. The default is 0 + kwp: the size of the array in kWp. The
-default is 5kWp + dam: damping factor. Default is None + inv: inverter power
-limit (when the array will clip). The default is None + hor: a list of values
-describing obstructions on the horizon Add one array for each string attached
-to your inverter. If your solar production is limited by clipping, set the
-inverter power so the forecast better matches your generation. See the [API
-documentation](https://doc.forecast.solar/api) for more information on
-parameter values. ``` fcast = f.Solar() print(fcast) ``` Returns a forecast for
-today and tomorrow. Optional parameters are: + reload: cached data handling. 0
-= use saved data, 1 = fetch new data, 2 = use saved data for today (default) +
-quiet: set to True to stop Solar producing progress messages Forecast data is
-saved to f.solar_save. The default is 'solar.txt'. ``` fcast.plot_daily()
+start_at, end_by, duration, times, forecast_times, strategy, update, weighting,
+time_shift) ``` This gets the latest 30 minute pricing and uses this to work
+out the best off peak charging period. + product: optional Agile Octopus
+product code (see below). The default is "AGILE-FLEX-22-11-25" + region:
+optional region to use for prices (se below). The default is 'H' (Southern
+England) + start_at: optional earliest start time for charge period in hours,
+the default is 23:00 + end_by: optional latest end time for charge period in
+hours, the default is 08:00 + duration: optional charge time period in hours,
+the default is 3 hours. Valid range is 1-6 hours + times: a list of charge
+periods that can be used instead of start_at, end_by and duration (see below) +
+forecast_times: a list of times when a forecast can be obtained from Solcast /
+forecast.solar + strategy: an optional list of times and work modes (see below)
++ update: optional, 1 (the default) sets the current tariff to Agile Octopus.
+Setting to 0 does not change the current tariff + weighting: optional, default
+is None (see below) + time_shift: optional system time shift in hours. The
+default is for system time to be UTC and to apply the current day light saving
+time (e.g. GMT/BST) Product codes include: + 'AGILE-18-02-21' = The original
+version capped at 35p per unit + 'AGILE-22-07-22' = The cap rose to 55p +
+'AGILE-22-08-31' = The cap was increased to 78p + 'AGILE-VAR-22-10-19' = This
+version raised the cap to Â£1 per unit and also introduced a new formula. +
+'AGILE-FLEX-22-11-25' = Cap stays at Â£1 per unit but new formula only deducts
+17.9p from higher unit prices (default) Region codes include: + 'A' = Eastern
+England + 'B' = East Midlands + 'C' = London + 'D' = Merseyside and Northern
+Wales + 'E' = West Midlands + 'F' = North Eastern England + 'G' = North Western
+England + 'H' = Southern England (default) + 'J' = South Eastern England + 'K'
+= Southern Wales + 'L' = South Western England + 'M' = Yorkshire + 'N' =
+Southern Scotland + 'P' = Northern Scotland Pricing for tomorrow is updated
+around 4pm each day. If run before this time, prices from yesterday are used.
+By default, prices for tomorrow are fetched after 5pm. The setting for this is:
++ f.agile_update_time = 17 The best charging period is determined based on the
+weighted average of the 30 minute prices over the duration. The default is flat
+(all prices are weighted equally). You can change the weighting by providing
+'weighting'. The following preset weightings are provided: + f.front_loaded:
+[1.0, 0.9, 0.8, 0.7, 0.6, 0.5] + f.first_hour: [1.0, 1.0] Specifying start_at,
+end_by and duration allows either the AM or PM charging slot for any tariif to
+be updated, depending on the time. Agile periods will be calculated; othe
+rtariffs will use the start and end times directly. By default, set_tariff()
+updates the AM charge period if start_at is after 9pm and end_by is before 8am;
+it updates the PM charge period if start_at is after 8am and the end_by is
+before 9pm. Only the relevant AM or PM charge time is updated e.g. if you
+configure a PM charging period, the AM charginig period is not changed. To
+disable a charging period, set duration=0. set_tariff() can configure multiple
+charging periods for any tariff using the times parameter instead of start_at,
+end_by and duration. Times is a list of tuples containing values for start_at,
+end_by and duration. For example, this parameter configures an AM charging
+period between 11pm and 8am with a 3 hour period and a PM charging period
+between 12 noon and 4pm with a 1 hour period: + times=[("23:00", "8:00", 3),
+("12:00", "16:00", 1)] 'strategy' allows you to configure times when work modes
+will be changed. The format is a list of dictionary items, containing: +
+'start', 'end': times in decimal hours or time format. The end time is
+exclusive so setting an end time of '07:00' will set a schedule that ends at
+'06:59' + 'mode': the work mode to be used from 'SelfUse', 'Feedin', 'Backup',
+'ForceCharge', 'ForceDischarge' + 'min_soc, 'fdsoc', 'fdpwr': optional values
+for each work mode. The defaults are 10, 10 and 0 respectively. The strategy
+should not include settings for the AM/PM charge times for the tariff. These
+will be added by charge_needed(). # PV Output These functions produce CSV data
+for upload to [pvoutput.org](https://pvoutput.org) including PV generation,
+Export, Load and Grid consumption by day in Wh. The functions use the energy
+estimates created from the raw power data (see above). The estimates include PV
+energy generation that are not otherwise available from the Fox Cloud.
+Typically, the energy results are within 3% of the values reported by the
+meters built into the inverter. ## Get PV Output Data Returns CSV upload data
+using the [API format](https://pvoutput.org/help/api_specification.html#csv-
+data-parameter): ``` f.get_pvoutput(d, tou) ``` + d is the date or a list of
+dates, to get data for. The default is yesterday + tou: optional, setting tou=1
+uploads data with time of use. The default, tou=0 does not split data and is
+more accurate. You can copy and paste the output data to the pvoutput data CSV
+Loader, using the following settings: ![image](https://github.com/TonyM1958/
+FoxESS-Cloud/assets/63789168/21459cdc-a943-4e9d-a204-7efd45a422d8) For example,
+this Jupyer Lab cell will provide a CSV data upload for June 2023: ```
+f.get_pvoutput(f.date_list('2023-06-01', '2023-06-30')) ``` ## Set PV Output
+Data Loads CSV data directly using the PV Ouput API: ``` f.set_pvoutput(d,
+system_id, tou, push) ``` + d is optional and is the date, or a list of dates,
+to upload + system_id is optional and allow you to select where data is
+uploaded to (where you have more than 1 registered system) + tou: optional,
+setting tou=1 uploads data with time of use. The default, tou=0 does not split
+data and is more accurate + push: optional. 0 = do not sent to pushover, 1 =
+send summary to pushover, 2 = send first day summary only # Solar Forecasting #
+Solcast Get and display solar data from your solcast.com account using your API
+key: ``` f.solcast_api_key = "my.solcast_api_key" fcast = f.Solcast() print
+(fcast) ``` Returns a 7 day forecast. Optional parameters are: + days: number
+of days to get. The default is 7 + estimated: whether to get history /
+estimated data. 1 = yes, 0 = no. Default is 0. + reload: cached data handling.
+0 = use saved data, 1 = fetch new data, 2 = use saved data for today (default)
++ quiet: True to stop Solcast producing progress messages Forecast data is
+saved to f.solcast_save. The default is 'solcast.txt'. ``` fcast.plot_daily()
 fcast.plot_hourly(day) ``` Plots the estimate / forecast data. plot_daily()
 plots the daily yield. plot_hourly() plots each day separately. + day:
 optional. 'today', 'tomorrow', 'all' or a specific list of dates. The default
-is to plot today and tomorrow # Pushover Send messages to a pushover user
-account: ``` f.output_spool(app_key, h) f.output(s) f.output_close(plot, file)
-f.output_message(app_key, message, plot) ``` Calling f.output_spool() with an
-app key will start the system spooling output to send to pushover. h is an
-optional header to add as the first line of the message. H may include \
+is to plot today and tomorrow # Forecast.solar Get and display solar data from
+forecast.solar for today and tomorrow: ``` f.solar_array('South', lat=51.1789,
+lon=-1.8262, kwp=6.4) ``` You need to configure your solar arrays by calling
+f.solar_array(). This takes the following parameters: + name: the name of each
+of your arrays + lat: the latitude where the array is located. The default is
+Stonehenge. + lon: the longitude where the array is located. The default is
+Stonehenge. + dec: the declination of the array - 0 is lying flat and 90 is
+vertical. Default is 30 + az: azimuth of the array. 0 is pointing due South, -
+90 is pointing East, 90 is pointing West. The default is 0 + kwp: the size of
+the array in kWp. The default is 5kWp + dam: damping factor. Default is None +
+inv: inverter power limit (when the array will clip). The default is None +
+hor: a list of values describing obstructions on the horizon Add one array for
+each string attached to your inverter. If your solar production is limited by
+clipping, set the inverter power so the forecast better matches your
+generation. See the [API documentation](https://doc.forecast.solar/api) for
+more information on parameter values. ``` fcast = f.Solar() print(fcast) ```
+Returns a forecast for today and tomorrow. Optional parameters are: + reload:
+cached data handling. 0 = use saved data, 1 = fetch new data, 2 = use saved
+data for today (default) + quiet: set to True to stop Solar producing progress
+messages Forecast data is saved to f.solar_save. The default is 'solar.txt'.
+``` fcast.plot_daily() fcast.plot_hourly(day) ``` Plots the estimate / forecast
+data. plot_daily() plots the daily yield. plot_hourly() plots each day
+separately. + day: optional. 'today', 'tomorrow', 'all' or a specific list of
+dates. The default is to plot today and tomorrow # Pushover Send messages to a
+pushover user account: ``` f.output_spool(app_key, h) f.output(s)
+f.output_close(plot, file) f.output_message(app_key, message, plot) ``` Calling
+f.output_spool() with an app key will start the system spooling output to send
+to pushover. h is an optional header to add as the first line of the message. H
+may include \
 >, \
 > or \
 > and these will be set to current system time and date respectively. When
 spooling is active, any calls to f.output() add lines to the spooled message.
 If appending to the message would exceed 1024 characters, the existing spooled
 message is sent and a new message spool is started. Calling f.output_close()
 will send the spooled message and optionally attach a binary image file. You
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.5
-Refactor debug messaging. Simplify charge_needed() output. Added 'target_soc'
-to charge_needed() settings Fix bat_info() giving incorrect temperatures when
-API returns 0 instead of -50 where there is no battery Fix key error when
-accessing cell volts and temps using an agent / installer account. Ensure
-output is generated if get_battery() fails using battery_info(). Update f.avg()
-to include calculation of averages in lists containng None values. Added
+(verbose) # Version Info 2.2.6
+Implement 2 second delay between calls that change inverter settings. Added
+strategy mode (timed_mode=2) to charge_needed(). Added set_strategy() and
+charge_strategy() to manage charging schedules and work mode changes. Refactor
+debug messaging. Simplify charge_needed() output. Added 'target_soc' to
+charge_needed() settings Fix bat_info() giving incorrect temperatures when API
+returns 0 instead of -50 where there is no battery Fix key error when accessing
+cell volts and temps using an agent / installer account. Ensure output is
+generated if get_battery() fails using battery_info(). Update f.avg() to
+include calculation of averages in lists containng None values. Added
 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
```

### Comparing `foxesscloud-2.2.5/README.md` & `foxesscloud-2.2.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: foxesscloud
+Version: 2.2.6
+Summary: library for accessing Fox ESS cloud data using Open API
+Author-email: Tony Matthews <tony@quasair.co.uk>
+Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
+Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
 # FoxESS-Cloud
 
 <a href="https://www.buymeacoffee.com/tonym1958" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174" align="right"></a>
 This site contains sample python code for accessing the Fox cloud data via the REST API used by the Fox ESS Cloud web site and app.
 
 There is also a number of Jupyter Lab notebooks with examples of how to run the sample code.
 
@@ -81,63 +95,74 @@
 
 ```
 f.get_generation()
 f.get_battery()
 f.get_settings()
 f.get_charge()
 f.get_min()
+f.get_flag()
 f.get_schedule()
 
 ```
 Each of these calls will return a dictionary or list containing the relevant information.
 
 get_generation() will return the latest generation information for the device. The results are also stored in f.device as 'generationToday', 'generationMonth' and 'generationTotal'.
 
 get_battery() returns the current battery status, including 'soc', 'volt', 'current', 'power', 'temperature' and 'residual'. The result also updates f.battery.
 
 get_settings() will return the battery settings and is equivalent to get_charge() and get_min(). The results are stored in f.battery_settings. The settings include minSoc, minSocOnGrid, enable charge from grid and the charge times.
 
+get_flag() returns the current scheduler enable / support flags
+
 get_schedule() returns the current work mode / soc schedule settings. The result is stored in f.schedule.
 
 
 ## Inverter Settings
 You can change inverter settings using:
 
 ```
 f.set_min(minSocOnGrid, minSoc)
 f.set_charge(ch1, st1, en1, ch2, st2, en2)
 f.set_group(start, end, mode, min_soc, fdsoc, fdpwr)
-f.get_flag()
-f.set_schedule(enable, groups, template)
+f.set_strategy(strategy)
+f.charge_strategy(st1, en1, st2, en2, min_soc)
+f.set_schedule(groups, enable)
 ```
 
 set_min() applies new SoC settings to the inverter. The parameters update battery_settings:
 + minSocOnGrid: min Soc on Grid setting e.g. 15 = 15%
 + minSoc: min Soc setting e.g. 10 = 10%
 
 set_charge() takes the charge times from the battery_settings and applies these to the inverter. The parameters are optional and will update battery_settings. You should specify all 3 parameter for a time period:
 + ch1: enable charge from grid for period 1 (True or False)
 + st1: the start time for period 1
 + en1: the end time for period 1
 + ch2: enable charge from grid for period 2 (True or False)
 + st2: the start time for period 2
 + en2: the end time for period 2
 
-set_flag() returns the current settings for strategy periods: 'supported' and 'enable'
-
 set_group() returns a time segment structure that can be used to build a list of time segments for set_schedule()
-+ start, end, mode: required parameters
++ start, end, mode: required parameters. end time is exclusive e.g. end at '07:00' will set a period end time of '06:59'
 + min_soc: optional, default is 10
 + fdsoc: optional, default is 10. Used when setting a period with ForceDischarge mode
 + fdpwr: optional, default is 0. Used when setting a period with ForceDischarge mode
 + enable: sets whether this time segment is enable (1) or disabled (0). The default is enabled.
 
+set_strategy() creates a list of groups from the strategy. If strategy is not provided, it uses the strategy for the current tariff.
+
+charge_strategy(): returns a list of groups that describe the strategy for the current tariff and adds the groupd required for charging:
++ st1: the start time for the period when the battery charges from the grid
++ en1: the end time for period 1
++ st2: the start time for period when the battery is held at min_soc
++ en2: the end time for period 2
++ min_soc: the min_soc to use after the charge period, when you don't want the battery to discharge below this level
+
 set_schedule() configures a list of scheduled work mode / soc changes with enable=1. If called with enable=0, any existing schedules are disabled. To enable a schedule, you must provide a list of time segments
-+ enable: 1 to enable schedules, 0 to disable schedules. The default is 1.
 + groups: a time segment or list of time segments created using f.set_group().
++ enable: 1 to enable schedules, 0 to disable schedules. The default is 1.
 
 
 ## Real Time Data
 Real time data reports the latest values for inverter variables, collected every 5 minutes:
 
 ```
 f.invert_ct2 = 1
@@ -280,18 +305,18 @@
 
 ```
 f.charge_needed(forecast, force_charge, forecast_selection, forecast_times, update_setings, show_data, show_plot)
 ```
 
 All the parameters are optional:
 + forecast: the kWh expected tomorrow (optional, see below)
-+ force_charge: 1 any remaining time in a charge period has force charge set, 2 charging uses the entire charge period, 0 None (default)
++ force_charge: 1 any remaining time in a charge period has force charge / min_soc set, 2 charging uses the entire charge period, 0 None (default)
 + forecast_selection: if set to 1, settings are only updated if there is a forecast. Default is 0, generation is used when forecasts are not available
 + forecast_times: a list of hours when forecasts can be obtained. By default, the forecast times for the selected tariff are used (see below)
-+ update_settings: 0 no changes, 1 update charge time, 2 update work mode, 3 update charge time and work mode. The default is 0
++ update_settings: 0 no changes, 1 update charge settings. The default is 0
 + show_data: 1 show battery SoC data, 2 show battery Residual data, 3 show timed data, 4 show timed data before and after charging. The default is 1.
 + show_plot: 1 plot battery SoC data. 2 plot battery Residual, Generation and Consumption. 3 plot 2 + Charge and Discharge The default is 3
 
 ### Modelling
 
 charge_needed() uses a number of models to better estimate the state of the battery.
 
@@ -344,15 +369,15 @@
 use_today: 21.0               # hour when today's generation and consumption data will be used
 min_hours: 0.25               # minimum charge time to set (in decimal hours)
 min_kwh: 0.5                  # minimum charge to add in kwh
 solcast_adjust: 100           # % adjustment to make to Solcast forecast
 solar_adjust:  100            # % adjustment to make to Solar forecast
 forecast_selection: 1         # 1 = only update charge times if forecast is available, 0 = use best available data. Default is 1.
 annual_consumption: None      # optional annual consumption in kWh. If set, this replaces consumption history
-timed_mode: 0                 # 1 = apply timed work mode, 0 = None
+timed_mode: 0                 # 0 = None, 1 = use timed work mode, 2 = strategy mode
 special_contingency: 30       # contingency for special days when consumption might be higher
 special_days: ['12-25', '12-26', '01-01']
 full_charge: None             # day of month (1-28) to do full charge or 'daily' or day of week: 'Mon', 'Tue' etc
 derate_temp: 21               # battery temperature in C when derating charge current is applied
 derate_step: 5                # step size for derating e.g. 21, 16, 11
 derating: [24, 15, 10, 2]     # derated charge current for each temperature step e.g. 21C, 16C, 11C, 6C
 force: 1                      # 1 = disable strategy periods when setting charge. 0 = fail if strategy period has been set.
@@ -362,14 +387,16 @@
 These values are stored / available in f.charge_config.
 
 The default battery open circuit voltage curve versus SoC from 0% to 100% is:
 ```
 lifepo4_curve = [51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50]
 ```
 
+When operating in strategy mode (timed_mode=2), charge_needed will create a schedule that includes the strategy for the tariff with additional time segments added to charge from grid and (optionall) to stop the battery discharging. In other modes, charge_needed() will disable any schedules and set the battery charge times.
+
 This example shows the results reported by charge needed:
 
 ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-b165-20d806b1e7e8)
 
 
 ## Battery Info
 
@@ -453,26 +480,26 @@
 ```
 f.set_tariff('flux')
 ```
 
 When Agile Octopus is selected, a price based charging period is configured using the 30 minute price forecast. For example:
 
 ```
-f.set_tariff('agile', product, region, start_at, end_by, duration, times, forecast_times, work_times, update, weighting, time_shift)
+f.set_tariff('agile', product, region, start_at, end_by, duration, times, forecast_times, strategy, update, weighting, time_shift)
 ```
 
 This gets the latest 30 minute pricing and uses this to work out the best off peak charging period.
 + product: optional Agile Octopus product code (see below). The default is "AGILE-FLEX-22-11-25"
 + region: optional region to use for prices (se below). The default is 'H' (Southern England)
 + start_at: optional earliest start time for charge period in hours, the default is 23:00
 + end_by: optional latest end time for charge period in hours, the default is 08:00
 + duration: optional charge time period in hours, the default is 3 hours. Valid range is 1-6 hours
 + times: a list of charge periods that can be used instead of start_at, end_by and duration (see below)
 + forecast_times: a list of times when a forecast can be obtained from Solcast / forecast.solar
-+ work_times: a list of work modes and times when these are set. The format is [(mode, start, end),...]
++ strategy: an optional list of times and work modes (see below)
 + update: optional, 1 (the default) sets the current tariff to Agile Octopus. Setting to 0 does not change the current tariff
 + weighting: optional, default is None (see below)
 + time_shift: optional system time shift in hours. The default is for system time to be UTC and to apply the current day light saving time (e.g. GMT/BST)
 
 Product codes include: 
 + 'AGILE-18-02-21' = The original version capped at 35p per unit
 + 'AGILE-22-07-22' = The cap rose to 55p
@@ -506,14 +533,21 @@
 Specifying start_at, end_by and duration allows either the AM or PM charging slot for any tariif to be updated, depending on the time. Agile periods will be calculated; othe rtariffs will use the start and end times directly. By default, set_tariff() updates the AM charge period if start_at is after 9pm and end_by is before 8am; it updates the PM charge period if start_at is after 8am and the end_by is before 9pm. Only the relevant AM or PM charge time is updated e.g. if you configure a PM charging period, the AM charginig period is not changed.
 
 To disable a charging period, set duration=0.
 
 set_tariff() can configure multiple charging periods for any tariff using the times parameter instead of start_at, end_by and duration. Times is a list of tuples containing values for start_at, end_by and duration. For example, this parameter configures an AM charging period between 11pm and 8am with a 3 hour period and a PM charging period between 12 noon and 4pm with a 1 hour period:
 + times=[("23:00", "8:00", 3), ("12:00", "16:00", 1)]
 
+'strategy' allows you to configure times when work modes will be changed. The format is a list of dictionary items, containing:
++ 'start', 'end': times in decimal hours or time format. The end time is exclusive so setting an end time of '07:00' will set a schedule that ends at '06:59'
++ 'mode': the work mode to be used from 'SelfUse', 'Feedin', 'Backup', 'ForceCharge', 'ForceDischarge'
++ 'min_soc, 'fdsoc', 'fdpwr': optional values for each work mode. The defaults are 10, 10 and 0 respectively.
+
+The strategy should not include settings for the AM/PM charge times for the tariff. These will be added by charge_needed().
+
 
 # PV Output
 These functions produce CSV data for upload to [pvoutput.org](https://pvoutput.org) including PV generation, Export, Load and Grid consumption by day in Wh. The functions use the energy estimates created from the raw power data (see above). The estimates include PV energy generation that are not otherwise available from the Fox Cloud. Typically, the energy results are within 3% of the values reported by the meters built into the inverter.
 
 
 ## Get PV Output Data
 
@@ -652,15 +686,18 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.5<br>
+2.2.6<br>
+Implement 2 second delay between calls that change inverter settings.
+Added strategy mode (timed_mode=2) to charge_needed().
+Added set_strategy() and charge_strategy() to manage charging schedules and work mode changes.
 Refactor debug messaging.
 Simplify charge_needed() output.
 Added 'target_soc' to charge_needed() settings
 Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50 where there is no battery
 Fix key error when accessing cell volts and temps using an agent / installer account.
 Ensure output is generated if get_battery() fails using battery_info().
 Update f.avg() to include calculation of averages in lists containng None values.
```

#### html2text {}

```diff
@@ -1,9 +1,16 @@
-# FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code for
-accessing the Fox cloud data via the REST API used by the Fox ESS Cloud web
+Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.6 Summary: library for
+accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
+quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
+Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
+LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
+for accessing the Fox cloud data via the REST API used by the Fox ESS Cloud web
 site and app. There is also a number of Jupyter Lab notebooks with examples of
 how to run the sample code. This project is not endorsed by, directly
 affiliated with, maintained, authorized, or sponsored by Fox ESS. Please refer
 to the [LICENCE](https://github.com/TonyM1958/FoxESS-Cloud/blob/main/LICENCE)
 for information on copyright, permissions and warranty. # Open API This module
 builds on the Fox Open API to provide a sample code and utilities that can be
 used with your inverter and batteries. + Information on the API can be found
@@ -46,181 +53,189 @@
 there is more than 1 item, the call will show the list of items. To select a
 specific item to work with, call a qualifier: + Site: full or partial name of
 the site + Logger: full or partial serial number + Inverter: full or partial
 serial number When an item is selected, the functions returns a dictionary
 containing item details and saves these to a global variable (f.site, f.logger,
 f.device respectively) Once an inverter is selected, you can make other calls
 to get information: ``` f.get_generation() f.get_battery() f.get_settings()
-f.get_charge() f.get_min() f.get_schedule() ``` Each of these calls will return
-a dictionary or list containing the relevant information. get_generation() will
-return the latest generation information for the device. The results are also
-stored in f.device as 'generationToday', 'generationMonth' and
-'generationTotal'. get_battery() returns the current battery status, including
-'soc', 'volt', 'current', 'power', 'temperature' and 'residual'. The result
-also updates f.battery. get_settings() will return the battery settings and is
-equivalent to get_charge() and get_min(). The results are stored in
+f.get_charge() f.get_min() f.get_flag() f.get_schedule() ``` Each of these
+calls will return a dictionary or list containing the relevant information.
+get_generation() will return the latest generation information for the device.
+The results are also stored in f.device as 'generationToday', 'generationMonth'
+and 'generationTotal'. get_battery() returns the current battery status,
+including 'soc', 'volt', 'current', 'power', 'temperature' and 'residual'. The
+result also updates f.battery. get_settings() will return the battery settings
+and is equivalent to get_charge() and get_min(). The results are stored in
 f.battery_settings. The settings include minSoc, minSocOnGrid, enable charge
-from grid and the charge times. get_schedule() returns the current work mode /
-soc schedule settings. The result is stored in f.schedule. ## Inverter Settings
-You can change inverter settings using: ``` f.set_min(minSocOnGrid, minSoc)
+from grid and the charge times. get_flag() returns the current scheduler enable
+/ support flags get_schedule() returns the current work mode / soc schedule
+settings. The result is stored in f.schedule. ## Inverter Settings You can
+change inverter settings using: ``` f.set_min(minSocOnGrid, minSoc)
 f.set_charge(ch1, st1, en1, ch2, st2, en2) f.set_group(start, end, mode,
-min_soc, fdsoc, fdpwr) f.get_flag() f.set_schedule(enable, groups, template)
-``` set_min() applies new SoC settings to the inverter. The parameters update
-battery_settings: + minSocOnGrid: min Soc on Grid setting e.g. 15 = 15% +
-minSoc: min Soc setting e.g. 10 = 10% set_charge() takes the charge times from
-the battery_settings and applies these to the inverter. The parameters are
-optional and will update battery_settings. You should specify all 3 parameter
-for a time period: + ch1: enable charge from grid for period 1 (True or False)
-+ st1: the start time for period 1 + en1: the end time for period 1 + ch2:
-enable charge from grid for period 2 (True or False) + st2: the start time for
-period 2 + en2: the end time for period 2 set_flag() returns the current
-settings for strategy periods: 'supported' and 'enable' set_group() returns a
-time segment structure that can be used to build a list of time segments for
-set_schedule() + start, end, mode: required parameters + min_soc: optional,
-default is 10 + fdsoc: optional, default is 10. Used when setting a period with
-ForceDischarge mode + fdpwr: optional, default is 0. Used when setting a period
-with ForceDischarge mode + enable: sets whether this time segment is enable (1)
-or disabled (0). The default is enabled. set_schedule() configures a list of
-scheduled work mode / soc changes with enable=1. If called with enable=0, any
-existing schedules are disabled. To enable a schedule, you must provide a list
-of time segments + enable: 1 to enable schedules, 0 to disable schedules. The
-default is 1. + groups: a time segment or list of time segments created using
-f.set_group(). ## Real Time Data Real time data reports the latest values for
-inverter variables, collected every 5 minutes: ``` f.invert_ct2 = 1 f.get_vars
-() f.get_real(v) ``` f.invert_ct2 determines how the meterPower2 data is
-handled. When invert_ct2 = 0, meterPower2 produces +ve power values during
-secondary generation. If meterPower2 produces -ve power values during secondary
-generation, setting invert_ct2 = 1 will flip the values so they are +ve when
-generating. The default setting is 1 (invert). f.get_vars() returns the list of
-variables that can be queried. This also stores the information: + f.var_table:
-a table, indexed by variable that contains information such as the name and
-unit. ++ f.var_list: a list of all the variables that are available There are
-also pre-defined lists: + power_vars lists the main power variables provided by
-the inverter + battery_vars lists the main variables relevant to the battery /
-BMS f.get_real returns the latest values for a list of variables. + v is a
-variable, or list of variables. The default is to return the latest value for
-all available variables ## History Data History data reports inverter
-variables, collected every 5 minutes, on a given date / time and period: ```
-f.get_history(time_span, d, v, summary, save, load, plot) ``` + time_span
-determines the period covered by the data, for example, 'hour', 'day' or
-'week'. The default is 'hour' + d is a date and time in the format 'YYYY-MM-DD
-HH:MM:SS'. The default is today's date and time. d may also be a list of dates
-+ v is a variable, or list of variables (see above) + summary is optional - see
-below + save: set to the root part of a filename to save the results + load:
-set to the full filename to load previously saved results + plot is optional. 1
-plots the results with a chart per unit and per day. 2 plots multiple days on
-the same chart. Default is 0, no plots The setting for invert_ct2 is applied to
-history data for meterPower2, so +ve values are returned for secondary
-generation. f.sample_time is set to the sample time in minutes for the data
-processed, rounded to f.sample_rounding samples per minute. Data generation for
-the full list of raw_vars can be slow and return a lot of data, so it's best to
-select the vars you want from the list if you can. For example, this Jupyter
-Lab cell will load an inverter and return power data at 5 minute intervals for
-the 17th June 2023: ``` d = '2023-06-17 00:00:00' result=f.get_history('day',
-d=d, v=f.power_vars) ``` Setting the optional parameter 'summary' when calling
-get_raw() provides a summary of the raw data + summary = 0: basic history data,
-no summary + summary = 1: summary is calculated + summary = 2: summary is
-calculated and raw data is removed to save time / space + summary = 3: as (2)
-but for energy only, an hourly cumulative state is also generated, similar to
-the state used in Home Assistant long term statistics The summary includes the
-following attributes: + count: the number of data points + average: the average
-value of the data points + max: the maximum value of the data points +
-max_time: the time when the maximum value occured (HH:MM) + min: the minimum
-value of the data points + min_time: the time when the minimum value occured
-(HH:MM) For power values (unit = kW), the summary performs a Riemann sum of the
-data, integrating kW over the day to estimate energy in kWh. In this case, the
-following attributes are also added: + kwh: the total energy generated or
-consumed + kwh_off: the total energy consumed or generated during the off-peak
-time of use + kwh_peak: the total energy consumed or generated during the peak
-time of use + kwh_neg: the total energy from -ve power flow (all other totals
-are based on +ve power flow) This example shows power graphs for today and
-yesterday: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/
-d84c55c9-4f4c-431d-bc55-d7796b7e4fea) ## Report Data Report data provides
-information on the energy produced by the inverter, battery charge and
-discharge energy, grid consumption and feed-in energy and home energy
-consumption: ``` f.get_report(report_type, d, v, summary, save, load, plot,
-station) ``` + report_type sets the period covered by the report and is one of
-'day', 'week', 'month', 'year': + when 'day' is selected, energy is reported
-each hour through the day + when 'week' is selected, energy is reported for the
-7 days up to and including the date + when 'month' is selected, energy is
-reported each day through the month + when 'year' is selected, energy is
-reported each month through the year + d is a date and time in the format
-'YYYY-MM-DD HH:MM:SS'. The default is yesterday. d may also be a list of dates
-+ v is a variable, or list of variables. The default is to use report_vars +
-summary is optional - see below + save: set to the root part of a filename to
+min_soc, fdsoc, fdpwr) f.set_strategy(strategy) f.charge_strategy(st1, en1,
+st2, en2, min_soc) f.set_schedule(groups, enable) ``` set_min() applies new SoC
+settings to the inverter. The parameters update battery_settings: +
+minSocOnGrid: min Soc on Grid setting e.g. 15 = 15% + minSoc: min Soc setting
+e.g. 10 = 10% set_charge() takes the charge times from the battery_settings and
+applies these to the inverter. The parameters are optional and will update
+battery_settings. You should specify all 3 parameter for a time period: + ch1:
+enable charge from grid for period 1 (True or False) + st1: the start time for
+period 1 + en1: the end time for period 1 + ch2: enable charge from grid for
+period 2 (True or False) + st2: the start time for period 2 + en2: the end time
+for period 2 set_group() returns a time segment structure that can be used to
+build a list of time segments for set_schedule() + start, end, mode: required
+parameters. end time is exclusive e.g. end at '07:00' will set a period end
+time of '06:59' + min_soc: optional, default is 10 + fdsoc: optional, default
+is 10. Used when setting a period with ForceDischarge mode + fdpwr: optional,
+default is 0. Used when setting a period with ForceDischarge mode + enable:
+sets whether this time segment is enable (1) or disabled (0). The default is
+enabled. set_strategy() creates a list of groups from the strategy. If strategy
+is not provided, it uses the strategy for the current tariff. charge_strategy
+(): returns a list of groups that describe the strategy for the current tariff
+and adds the groupd required for charging: + st1: the start time for the period
+when the battery charges from the grid + en1: the end time for period 1 + st2:
+the start time for period when the battery is held at min_soc + en2: the end
+time for period 2 + min_soc: the min_soc to use after the charge period, when
+you don't want the battery to discharge below this level set_schedule()
+configures a list of scheduled work mode / soc changes with enable=1. If called
+with enable=0, any existing schedules are disabled. To enable a schedule, you
+must provide a list of time segments + groups: a time segment or list of time
+segments created using f.set_group(). + enable: 1 to enable schedules, 0 to
+disable schedules. The default is 1. ## Real Time Data Real time data reports
+the latest values for inverter variables, collected every 5 minutes: ```
+f.invert_ct2 = 1 f.get_vars() f.get_real(v) ``` f.invert_ct2 determines how the
+meterPower2 data is handled. When invert_ct2 = 0, meterPower2 produces +ve
+power values during secondary generation. If meterPower2 produces -ve power
+values during secondary generation, setting invert_ct2 = 1 will flip the values
+so they are +ve when generating. The default setting is 1 (invert). f.get_vars
+() returns the list of variables that can be queried. This also stores the
+information: + f.var_table: a table, indexed by variable that contains
+information such as the name and unit. ++ f.var_list: a list of all the
+variables that are available There are also pre-defined lists: + power_vars
+lists the main power variables provided by the inverter + battery_vars lists
+the main variables relevant to the battery / BMS f.get_real returns the latest
+values for a list of variables. + v is a variable, or list of variables. The
+default is to return the latest value for all available variables ## History
+Data History data reports inverter variables, collected every 5 minutes, on a
+given date / time and period: ``` f.get_history(time_span, d, v, summary, save,
+load, plot) ``` + time_span determines the period covered by the data, for
+example, 'hour', 'day' or 'week'. The default is 'hour' + d is a date and time
+in the format 'YYYY-MM-DD HH:MM:SS'. The default is today's date and time. d
+may also be a list of dates + v is a variable, or list of variables (see above)
++ summary is optional - see below + save: set to the root part of a filename to
 save the results + load: set to the full filename to load previously saved
-results + plot is optional. 1 to plot results + station is optional. 1 gets
-data for a site (using f.station_id), 0 gets data for a device (using
-f.device_id). The default is 0. The list of variables that can be reported on
-is stored in f.report_vars. Note that reporting by 'day' produces inaccurate
-hourly data, where the sum does not reconcile with the daily total given in the
-monthly report. To correct this, reporting by day also gets the monthly data
-and uses the daily total to correctly report the total. Setting the optional
-parameter 'summary' when calling get_report() provides a summary of the report
-data: + summary = 0: basic report data, no summary. report_type cannot be
-'week' + summary = 1: summary is calculated + summary = 2: corrected total only
-is reported to save time / space. report_type must be 'day' The result data for
-each variable includes the following attributes when summary=2 + 'variable':
-name of the data set + 'total': corrected total of the data items When
-summary=1, the following items are also added: + 'data': 'index' and 'value' of
-each data point + 'date': that was used to produce the report + 'count': the
-number of data items + 'sum': the sum of the data items + 'max': the biggest
-value in 'data' + 'max_index': the index of the biggest value in 'data' +
-'min': the smallest value in 'data' + 'min_index': the index of the smallest
-value in 'data' + 'average': corrected average of the data items For example,
-this Jupyter Lab cell will report energy data by day for the month of June
-2023: ``` d = '2023-06-17' result=f.get_report('month', d=d) ``` This example
-plots weekly data: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
-63789168/f408a010-9600-4b2f-979f-83e32d960586) # Built-in Utilities and
-Operations The previous section provides functions that can be used to access
-and control your inverter. This section covers utilities and operations that
-build upon these functions. ## Charge Needed Uses forecast PV yield for
-tomorrow to work out if charging from grid is needed tonight to deliver the
-expected consumption for tomorrow. If charging is needed, the charge times are
-configured. If charging is not needed, the charge times are cleared. The
-results are sent to the inverter. ``` f.charge_needed(forecast, force_charge,
-forecast_selection, forecast_times, update_setings, show_data, show_plot) ```
-All the parameters are optional: + forecast: the kWh expected tomorrow
-(optional, see below) + force_charge: 1 any remaining time in a charge period
-has force charge set, 2 charging uses the entire charge period, 0 None
-(default) + forecast_selection: if set to 1, settings are only updated if there
-is a forecast. Default is 0, generation is used when forecasts are not
-available + forecast_times: a list of hours when forecasts can be obtained. By
-default, the forecast times for the selected tariff are used (see below) +
-update_settings: 0 no changes, 1 update charge time, 2 update work mode, 3
-update charge time and work mode. The default is 0 + show_data: 1 show battery
-SoC data, 2 show battery Residual data, 3 show timed data, 4 show timed data
-before and after charging. The default is 1. + show_plot: 1 plot battery SoC
-data. 2 plot battery Residual, Generation and Consumption. 3 plot 2 + Charge
-and Discharge The default is 3 ### Modelling charge_needed() uses a number of
-models to better estimate the state of the battery. **Manual Consumption:** You
-can provide your 'annual_consumption' in kWh e.g. 5500. This figure is factored
-down to a daily consumption by dividing by 365 and applying **f.seasonality**.
-This normally decreases consumption in the summer and increases it in winter.
-Seasonality is a list of weightings by month for Jan, Feb, Mar, Apr etc. Preset
-lists are 'f.high_seasonality' (recommend where electric heating is ued),
-'f.medium_seasonality' (default) amd 'f.no_seasonality' (all months the same).
-The daily consumption is profiled by hour using **f.daily_consumption**. This
-maps your consumption for a day to the hours when more or less energy is
-consumed. It is a list of 24 values for the times 00, 01, 02, 03 .. 23. Preset
-lists are 'f.high_profile' (larger peaks at 8am and 6pm), 'f.medium_profile'
-(default, more balanced) and 'f.no_profile' (flat). **Historic Consumption:**
-If annual_consumption is not provided, your consumption history is used. By
-default, this looks at your average consumption for the last 3 days using the
-load power reported by your inverter. For systems with multiple inverters where
-CT2 is not connected, the load power may not be correct. For this and other
-cases where you want to set your consumption, provide your annual_consumption.
-**Manual Forecast:** You can provide a specific 'forecast' in kWh e.g. 20. This
-is profiled using **f.seasonal_sun** to map solar generation to the time of
-day. The mapping is broken down into 4 seasons: winter, spring, summer and
-autumn (winter is Dec, Jan, Feb, spring is Mar, Apr, May etc). There are 4
-preset lists: 'f.winter_sun', 'f.spring_sun', 'f.summer_sun' and
-'f.autumn_sun'. Seasonal_sun is used for manual and historic forecasts
-**Solcast:** If you provide an API key for Solcast, your forecast will be
-downloaded after 9pm each day and used as the basis for your next days
+results + plot is optional. 1 plots the results with a chart per unit and per
+day. 2 plots multiple days on the same chart. Default is 0, no plots The
+setting for invert_ct2 is applied to history data for meterPower2, so +ve
+values are returned for secondary generation. f.sample_time is set to the
+sample time in minutes for the data processed, rounded to f.sample_rounding
+samples per minute. Data generation for the full list of raw_vars can be slow
+and return a lot of data, so it's best to select the vars you want from the
+list if you can. For example, this Jupyter Lab cell will load an inverter and
+return power data at 5 minute intervals for the 17th June 2023: ``` d = '2023-
+06-17 00:00:00' result=f.get_history('day', d=d, v=f.power_vars) ``` Setting
+the optional parameter 'summary' when calling get_raw() provides a summary of
+the raw data + summary = 0: basic history data, no summary + summary = 1:
+summary is calculated + summary = 2: summary is calculated and raw data is
+removed to save time / space + summary = 3: as (2) but for energy only, an
+hourly cumulative state is also generated, similar to the state used in Home
+Assistant long term statistics The summary includes the following attributes: +
+count: the number of data points + average: the average value of the data
+points + max: the maximum value of the data points + max_time: the time when
+the maximum value occured (HH:MM) + min: the minimum value of the data points +
+min_time: the time when the minimum value occured (HH:MM) For power values
+(unit = kW), the summary performs a Riemann sum of the data, integrating kW
+over the day to estimate energy in kWh. In this case, the following attributes
+are also added: + kwh: the total energy generated or consumed + kwh_off: the
+total energy consumed or generated during the off-peak time of use + kwh_peak:
+the total energy consumed or generated during the peak time of use + kwh_neg:
+the total energy from -ve power flow (all other totals are based on +ve power
+flow) This example shows power graphs for today and yesterday: ![image](https:/
+/github.com/TonyM1958/FoxESS-Cloud/assets/63789168/d84c55c9-4f4c-431d-bc55-
+d7796b7e4fea) ## Report Data Report data provides information on the energy
+produced by the inverter, battery charge and discharge energy, grid consumption
+and feed-in energy and home energy consumption: ``` f.get_report(report_type,
+d, v, summary, save, load, plot, station) ``` + report_type sets the period
+covered by the report and is one of 'day', 'week', 'month', 'year': + when
+'day' is selected, energy is reported each hour through the day + when 'week'
+is selected, energy is reported for the 7 days up to and including the date +
+when 'month' is selected, energy is reported each day through the month + when
+'year' is selected, energy is reported each month through the year + d is a
+date and time in the format 'YYYY-MM-DD HH:MM:SS'. The default is yesterday. d
+may also be a list of dates + v is a variable, or list of variables. The
+default is to use report_vars + summary is optional - see below + save: set to
+the root part of a filename to save the results + load: set to the full
+filename to load previously saved results + plot is optional. 1 to plot results
++ station is optional. 1 gets data for a site (using f.station_id), 0 gets data
+for a device (using f.device_id). The default is 0. The list of variables that
+can be reported on is stored in f.report_vars. Note that reporting by 'day'
+produces inaccurate hourly data, where the sum does not reconcile with the
+daily total given in the monthly report. To correct this, reporting by day also
+gets the monthly data and uses the daily total to correctly report the total.
+Setting the optional parameter 'summary' when calling get_report() provides a
+summary of the report data: + summary = 0: basic report data, no summary.
+report_type cannot be 'week' + summary = 1: summary is calculated + summary =
+2: corrected total only is reported to save time / space. report_type must be
+'day' The result data for each variable includes the following attributes when
+summary=2 + 'variable': name of the data set + 'total': corrected total of the
+data items When summary=1, the following items are also added: + 'data':
+'index' and 'value' of each data point + 'date': that was used to produce the
+report + 'count': the number of data items + 'sum': the sum of the data items +
+'max': the biggest value in 'data' + 'max_index': the index of the biggest
+value in 'data' + 'min': the smallest value in 'data' + 'min_index': the index
+of the smallest value in 'data' + 'average': corrected average of the data
+items For example, this Jupyter Lab cell will report energy data by day for the
+month of June 2023: ``` d = '2023-06-17' result=f.get_report('month', d=d) ```
+This example plots weekly data: ![image](https://github.com/TonyM1958/FoxESS-
+Cloud/assets/63789168/f408a010-9600-4b2f-979f-83e32d960586) # Built-in
+Utilities and Operations The previous section provides functions that can be
+used to access and control your inverter. This section covers utilities and
+operations that build upon these functions. ## Charge Needed Uses forecast PV
+yield for tomorrow to work out if charging from grid is needed tonight to
+deliver the expected consumption for tomorrow. If charging is needed, the
+charge times are configured. If charging is not needed, the charge times are
+cleared. The results are sent to the inverter. ``` f.charge_needed(forecast,
+force_charge, forecast_selection, forecast_times, update_setings, show_data,
+show_plot) ``` All the parameters are optional: + forecast: the kWh expected
+tomorrow (optional, see below) + force_charge: 1 any remaining time in a charge
+period has force charge / min_soc set, 2 charging uses the entire charge
+period, 0 None (default) + forecast_selection: if set to 1, settings are only
+updated if there is a forecast. Default is 0, generation is used when forecasts
+are not available + forecast_times: a list of hours when forecasts can be
+obtained. By default, the forecast times for the selected tariff are used (see
+below) + update_settings: 0 no changes, 1 update charge settings. The default
+is 0 + show_data: 1 show battery SoC data, 2 show battery Residual data, 3 show
+timed data, 4 show timed data before and after charging. The default is 1. +
+show_plot: 1 plot battery SoC data. 2 plot battery Residual, Generation and
+Consumption. 3 plot 2 + Charge and Discharge The default is 3 ### Modelling
+charge_needed() uses a number of models to better estimate the state of the
+battery. **Manual Consumption:** You can provide your 'annual_consumption' in
+kWh e.g. 5500. This figure is factored down to a daily consumption by dividing
+by 365 and applying **f.seasonality**. This normally decreases consumption in
+the summer and increases it in winter. Seasonality is a list of weightings by
+month for Jan, Feb, Mar, Apr etc. Preset lists are 'f.high_seasonality'
+(recommend where electric heating is ued), 'f.medium_seasonality' (default) amd
+'f.no_seasonality' (all months the same). The daily consumption is profiled by
+hour using **f.daily_consumption**. This maps your consumption for a day to the
+hours when more or less energy is consumed. It is a list of 24 values for the
+times 00, 01, 02, 03 .. 23. Preset lists are 'f.high_profile' (larger peaks at
+8am and 6pm), 'f.medium_profile' (default, more balanced) and 'f.no_profile'
+(flat). **Historic Consumption:** If annual_consumption is not provided, your
+consumption history is used. By default, this looks at your average consumption
+for the last 3 days using the load power reported by your inverter. For systems
+with multiple inverters where CT2 is not connected, the load power may not be
+correct. For this and other cases where you want to set your consumption,
+provide your annual_consumption. **Manual Forecast:** You can provide a
+specific 'forecast' in kWh e.g. 20. This is profiled using **f.seasonal_sun**
+to map solar generation to the time of day. The mapping is broken down into 4
+seasons: winter, spring, summer and autumn (winter is Dec, Jan, Feb, spring is
+Mar, Apr, May etc). There are 4 preset lists: 'f.winter_sun', 'f.spring_sun',
+'f.summer_sun' and 'f.autumn_sun'. Seasonal_sun is used for manual and historic
+forecasts **Solcast:** If you provide an API key for Solcast, your forecast
+will be downloaded after 9pm each day and used as the basis for your next days
 generation (see below). **Solar:** if you configure one or more
 **f.solar_array**, forecast.solar will be called to provide a forrecast for
 your next days generation (see below). **Historic Generation:** If 'forecast'
 is not provided and Solcast and Solar forecasts are not available, your
 generation history is used. By default, this looks at your average solar
 generation for the last 3 days and applies the **f.seasonal_sun** profile.
 Note: if using Solcast or forecast.solar, calls to the API are very limited so
@@ -257,50 +272,54 @@
 e.g. Saturdays use_today: 21.0 # hour when today's generation and consumption
 data will be used min_hours: 0.25 # minimum charge time to set (in decimal
 hours) min_kwh: 0.5 # minimum charge to add in kwh solcast_adjust: 100 # %
 adjustment to make to Solcast forecast solar_adjust: 100 # % adjustment to make
 to Solar forecast forecast_selection: 1 # 1 = only update charge times if
 forecast is available, 0 = use best available data. Default is 1.
 annual_consumption: None # optional annual consumption in kWh. If set, this
-replaces consumption history timed_mode: 0 # 1 = apply timed work mode, 0 =
-None special_contingency: 30 # contingency for special days when consumption
-might be higher special_days: ['12-25', '12-26', '01-01'] full_charge: None #
-day of month (1-28) to do full charge or 'daily' or day of week: 'Mon', 'Tue'
-etc derate_temp: 21 # battery temperature in C when derating charge current is
-applied derate_step: 5 # step size for derating e.g. 21, 16, 11 derating: [24,
-15, 10, 2] # derated charge current for each temperature step e.g. 21C, 16C,
-11C, 6C force: 1 # 1 = disable strategy periods when setting charge. 0 = fail
-if strategy period has been set. data_wrap: 6 # data items to show per line
-target_soc: None # target soc for charging ``` These values are stored /
-available in f.charge_config. The default battery open circuit voltage curve
-versus SoC from 0% to 100% is: ``` lifepo4_curve = [51.30, 52.00, 52.30, 52.40,
-52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ``` This example shows the
-results reported by charge needed: ![image](https://github.com/TonyM1958/
-FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-b165-20d806b1e7e8) ## Battery
-Info Provides detailed information on the current state of the batteries: ```
-f.battery_info(count, plot, log) f.battery_monitor(interval, run, log, save,
-count) ``` battery_info() prints information on the battery and cells: + count:
-optional over-ride. The default is based on factorising the number of cells
-reported by 16 or 18 to work out the number of batteries. + plot: 1 plot the
-cell voltages for each battery, 2 plot the cell temperatueres, 0 don't plot.
-The default is 1 + log: see below. Default is 0 battery_monitor() runs
-battery_info() in log mode on a schedule to provide information on the battery
-status over a period of time: + interval: the time in minutes between log
-entries. The default is 30 minutes + run: the number of log entries to create.
-The default is 48 i.e. every 30 minues for 24 hours in total + log: 0 =
-display, 1 = log battery info, 2 = add cell volts, 3 = add cell temps. The
-default is 1 + save: name of a CSV file to write log data to + count: optional
-over-ride for the number of batteries This is an example of the output from
-battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
-63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ``` f.date_list
-(s, e, limit, span, today) ``` Returns a list of dates in the format 'YYYY-MM-
-DD'. This function will not return dates in the future. The last date will be
-yesterday or today (if today is True). All parameters are optional: + s: start
-date + e: end date + limit: maximum number of days. The default is 200 + span:
-the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
+replaces consumption history timed_mode: 0 # 0 = None, 1 = use timed work mode,
+2 = strategy mode special_contingency: 30 # contingency for special days when
+consumption might be higher special_days: ['12-25', '12-26', '01-01']
+full_charge: None # day of month (1-28) to do full charge or 'daily' or day of
+week: 'Mon', 'Tue' etc derate_temp: 21 # battery temperature in C when derating
+charge current is applied derate_step: 5 # step size for derating e.g. 21, 16,
+11 derating: [24, 15, 10, 2] # derated charge current for each temperature step
+e.g. 21C, 16C, 11C, 6C force: 1 # 1 = disable strategy periods when setting
+charge. 0 = fail if strategy period has been set. data_wrap: 6 # data items to
+show per line target_soc: None # target soc for charging ``` These values are
+stored / available in f.charge_config. The default battery open circuit voltage
+curve versus SoC from 0% to 100% is: ``` lifepo4_curve = [51.30, 52.00, 52.30,
+52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ``` When operating in
+strategy mode (timed_mode=2), charge_needed will create a schedule that
+includes the strategy for the tariff with additional time segments added to
+charge from grid and (optionall) to stop the battery discharging. In other
+modes, charge_needed() will disable any schedules and set the battery charge
+times. This example shows the results reported by charge needed: ![image]
+(https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-
+b165-20d806b1e7e8) ## Battery Info Provides detailed information on the current
+state of the batteries: ``` f.battery_info(count, plot, log) f.battery_monitor
+(interval, run, log, save, count) ``` battery_info() prints information on the
+battery and cells: + count: optional over-ride. The default is based on
+factorising the number of cells reported by 16 or 18 to work out the number of
+batteries. + plot: 1 plot the cell voltages for each battery, 2 plot the cell
+temperatueres, 0 don't plot. The default is 1 + log: see below. Default is 0
+battery_monitor() runs battery_info() in log mode on a schedule to provide
+information on the battery status over a period of time: + interval: the time
+in minutes between log entries. The default is 30 minutes + run: the number of
+log entries to create. The default is 48 i.e. every 30 minues for 24 hours in
+total + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add
+cell temps. The default is 1 + save: name of a CSV file to write log data to +
+count: optional over-ride for the number of batteries This is an example of the
+output from battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/
+assets/63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ```
+f.date_list(s, e, limit, span, today) ``` Returns a list of dates in the format
+'YYYY-MM-DD'. This function will not return dates in the future. The last date
+will be yesterday or today (if today is True). All parameters are optional: +
+s: start date + e: end date + limit: maximum number of days. The default is 200
++ span: the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
 'weekday' + today: 1 allows today to be included, 2 allows future dates to be
 included. Default is 0, date list will stop at yesterday You can use 'span' as
 follows: + 'day' provides a single day + 'week' will provide the dates of 7
 consequetive days + 'month' will provide the dates of the days up to the same
 date in the preceeding (or follwing) month + '2days' will provide the dates of
 yesterday and today + 'weekday' will provide the dates of the same day of the
 week, going backwards (or forwards) up to 7 weeks ``` f.british_summer_time(d)
@@ -327,145 +346,156 @@
 to 23:59 + Eco 7: Economy 7: off-peak from 00:30 to 07:30 GMT (01:30 to 08:30
 during BST) Custom periods can be configured for specific times if required: +
 Custom: charging from 02:00 to 05:00, no off-peak or peak times, forecasts from
 22:00 to 23:59 The active tariff is configured by calling 'f.set_tariff() with
 the name of the tariff to use: ``` f.set_tariff('flux') ``` When Agile Octopus
 is selected, a price based charging period is configured using the 30 minute
 price forecast. For example: ``` f.set_tariff('agile', product, region,
-start_at, end_by, duration, times, forecast_times, work_times, update,
-weighting, time_shift) ``` This gets the latest 30 minute pricing and uses this
-to work out the best off peak charging period. + product: optional Agile
-Octopus product code (see below). The default is "AGILE-FLEX-22-11-25" +
-region: optional region to use for prices (se below). The default is 'H'
-(Southern England) + start_at: optional earliest start time for charge period
-in hours, the default is 23:00 + end_by: optional latest end time for charge
-period in hours, the default is 08:00 + duration: optional charge time period
-in hours, the default is 3 hours. Valid range is 1-6 hours + times: a list of
-charge periods that can be used instead of start_at, end_by and duration (see
-below) + forecast_times: a list of times when a forecast can be obtained from
-Solcast / forecast.solar + work_times: a list of work modes and times when
-these are set. The format is [(mode, start, end),...] + update: optional, 1
-(the default) sets the current tariff to Agile Octopus. Setting to 0 does not
-change the current tariff + weighting: optional, default is None (see below) +
-time_shift: optional system time shift in hours. The default is for system time
-to be UTC and to apply the current day light saving time (e.g. GMT/BST) Product
-codes include: + 'AGILE-18-02-21' = The original version capped at 35p per unit
-+ 'AGILE-22-07-22' = The cap rose to 55p + 'AGILE-22-08-31' = The cap was
-increased to 78p + 'AGILE-VAR-22-10-19' = This version raised the cap to Â£1
-per unit and also introduced a new formula. + 'AGILE-FLEX-22-11-25' = Cap stays
-at Â£1 per unit but new formula only deducts 17.9p from higher unit prices
-(default) Region codes include: + 'A' = Eastern England + 'B' = East Midlands +
-'C' = London + 'D' = Merseyside and Northern Wales + 'E' = West Midlands + 'F'
-= North Eastern England + 'G' = North Western England + 'H' = Southern England
-(default) + 'J' = South Eastern England + 'K' = Southern Wales + 'L' = South
-Western England + 'M' = Yorkshire + 'N' = Southern Scotland + 'P' = Northern
-Scotland Pricing for tomorrow is updated around 4pm each day. If run before
-this time, prices from yesterday are used. By default, prices for tomorrow are
-fetched after 5pm. The setting for this is: + f.agile_update_time = 17 The best
-charging period is determined based on the weighted average of the 30 minute
-prices over the duration. The default is flat (all prices are weighted
-equally). You can change the weighting by providing 'weighting'. The following
-preset weightings are provided: + f.front_loaded: [1.0, 0.9, 0.8, 0.7, 0.6,
-0.5] + f.first_hour: [1.0, 1.0] Specifying start_at, end_by and duration allows
-either the AM or PM charging slot for any tariif to be updated, depending on
-the time. Agile periods will be calculated; othe rtariffs will use the start
-and end times directly. By default, set_tariff() updates the AM charge period
-if start_at is after 9pm and end_by is before 8am; it updates the PM charge
-period if start_at is after 8am and the end_by is before 9pm. Only the relevant
-AM or PM charge time is updated e.g. if you configure a PM charging period, the
-AM charginig period is not changed. To disable a charging period, set
-duration=0. set_tariff() can configure multiple charging periods for any tariff
-using the times parameter instead of start_at, end_by and duration. Times is a
-list of tuples containing values for start_at, end_by and duration. For
-example, this parameter configures an AM charging period between 11pm and 8am
-with a 3 hour period and a PM charging period between 12 noon and 4pm with a 1
-hour period: + times=[("23:00", "8:00", 3), ("12:00", "16:00", 1)] # PV Output
-These functions produce CSV data for upload to [pvoutput.org](https://
-pvoutput.org) including PV generation, Export, Load and Grid consumption by day
-in Wh. The functions use the energy estimates created from the raw power data
-(see above). The estimates include PV energy generation that are not otherwise
-available from the Fox Cloud. Typically, the energy results are within 3% of
-the values reported by the meters built into the inverter. ## Get PV Output
-Data Returns CSV upload data using the [API format](https://pvoutput.org/help/
-api_specification.html#csv-data-parameter): ``` f.get_pvoutput(d, tou) ``` + d
-is the date or a list of dates, to get data for. The default is yesterday +
-tou: optional, setting tou=1 uploads data with time of use. The default, tou=0
-does not split data and is more accurate. You can copy and paste the output
-data to the pvoutput data CSV Loader, using the following settings: ![image]
-(https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/21459cdc-a943-4e9d-
-a204-7efd45a422d8) For example, this Jupyer Lab cell will provide a CSV data
-upload for June 2023: ``` f.get_pvoutput(f.date_list('2023-06-01', '2023-06-
-30')) ``` ## Set PV Output Data Loads CSV data directly using the PV Ouput API:
-``` f.set_pvoutput(d, system_id, tou, push) ``` + d is optional and is the
-date, or a list of dates, to upload + system_id is optional and allow you to
-select where data is uploaded to (where you have more than 1 registered system)
-+ tou: optional, setting tou=1 uploads data with time of use. The default,
-tou=0 does not split data and is more accurate + push: optional. 0 = do not
-sent to pushover, 1 = send summary to pushover, 2 = send first day summary only
-# Solar Forecasting # Solcast Get and display solar data from your solcast.com
-account using your API key: ``` f.solcast_api_key = "my.solcast_api_key" fcast
-= f.Solcast() print(fcast) ``` Returns a 7 day forecast. Optional parameters
-are: + days: number of days to get. The default is 7 + estimated: whether to
-get history / estimated data. 1 = yes, 0 = no. Default is 0. + reload: cached
-data handling. 0 = use saved data, 1 = fetch new data, 2 = use saved data for
-today (default) + quiet: True to stop Solcast producing progress messages
-Forecast data is saved to f.solcast_save. The default is 'solcast.txt'. ```
-fcast.plot_daily() fcast.plot_hourly(day) ``` Plots the estimate / forecast
-data. plot_daily() plots the daily yield. plot_hourly() plots each day
-separately. + day: optional. 'today', 'tomorrow', 'all' or a specific list of
-dates. The default is to plot today and tomorrow # Forecast.solar Get and
-display solar data from forecast.solar for today and tomorrow: ```
-f.solar_array('South', lat=51.1789, lon=-1.8262, kwp=6.4) ``` You need to
-configure your solar arrays by calling f.solar_array(). This takes the
-following parameters: + name: the name of each of your arrays + lat: the
-latitude where the array is located. The default is Stonehenge. + lon: the
-longitude where the array is located. The default is Stonehenge. + dec: the
-declination of the array - 0 is lying flat and 90 is vertical. Default is 30 +
-az: azimuth of the array. 0 is pointing due South, -90 is pointing East, 90 is
-pointing West. The default is 0 + kwp: the size of the array in kWp. The
-default is 5kWp + dam: damping factor. Default is None + inv: inverter power
-limit (when the array will clip). The default is None + hor: a list of values
-describing obstructions on the horizon Add one array for each string attached
-to your inverter. If your solar production is limited by clipping, set the
-inverter power so the forecast better matches your generation. See the [API
-documentation](https://doc.forecast.solar/api) for more information on
-parameter values. ``` fcast = f.Solar() print(fcast) ``` Returns a forecast for
-today and tomorrow. Optional parameters are: + reload: cached data handling. 0
-= use saved data, 1 = fetch new data, 2 = use saved data for today (default) +
-quiet: set to True to stop Solar producing progress messages Forecast data is
-saved to f.solar_save. The default is 'solar.txt'. ``` fcast.plot_daily()
+start_at, end_by, duration, times, forecast_times, strategy, update, weighting,
+time_shift) ``` This gets the latest 30 minute pricing and uses this to work
+out the best off peak charging period. + product: optional Agile Octopus
+product code (see below). The default is "AGILE-FLEX-22-11-25" + region:
+optional region to use for prices (se below). The default is 'H' (Southern
+England) + start_at: optional earliest start time for charge period in hours,
+the default is 23:00 + end_by: optional latest end time for charge period in
+hours, the default is 08:00 + duration: optional charge time period in hours,
+the default is 3 hours. Valid range is 1-6 hours + times: a list of charge
+periods that can be used instead of start_at, end_by and duration (see below) +
+forecast_times: a list of times when a forecast can be obtained from Solcast /
+forecast.solar + strategy: an optional list of times and work modes (see below)
++ update: optional, 1 (the default) sets the current tariff to Agile Octopus.
+Setting to 0 does not change the current tariff + weighting: optional, default
+is None (see below) + time_shift: optional system time shift in hours. The
+default is for system time to be UTC and to apply the current day light saving
+time (e.g. GMT/BST) Product codes include: + 'AGILE-18-02-21' = The original
+version capped at 35p per unit + 'AGILE-22-07-22' = The cap rose to 55p +
+'AGILE-22-08-31' = The cap was increased to 78p + 'AGILE-VAR-22-10-19' = This
+version raised the cap to Â£1 per unit and also introduced a new formula. +
+'AGILE-FLEX-22-11-25' = Cap stays at Â£1 per unit but new formula only deducts
+17.9p from higher unit prices (default) Region codes include: + 'A' = Eastern
+England + 'B' = East Midlands + 'C' = London + 'D' = Merseyside and Northern
+Wales + 'E' = West Midlands + 'F' = North Eastern England + 'G' = North Western
+England + 'H' = Southern England (default) + 'J' = South Eastern England + 'K'
+= Southern Wales + 'L' = South Western England + 'M' = Yorkshire + 'N' =
+Southern Scotland + 'P' = Northern Scotland Pricing for tomorrow is updated
+around 4pm each day. If run before this time, prices from yesterday are used.
+By default, prices for tomorrow are fetched after 5pm. The setting for this is:
++ f.agile_update_time = 17 The best charging period is determined based on the
+weighted average of the 30 minute prices over the duration. The default is flat
+(all prices are weighted equally). You can change the weighting by providing
+'weighting'. The following preset weightings are provided: + f.front_loaded:
+[1.0, 0.9, 0.8, 0.7, 0.6, 0.5] + f.first_hour: [1.0, 1.0] Specifying start_at,
+end_by and duration allows either the AM or PM charging slot for any tariif to
+be updated, depending on the time. Agile periods will be calculated; othe
+rtariffs will use the start and end times directly. By default, set_tariff()
+updates the AM charge period if start_at is after 9pm and end_by is before 8am;
+it updates the PM charge period if start_at is after 8am and the end_by is
+before 9pm. Only the relevant AM or PM charge time is updated e.g. if you
+configure a PM charging period, the AM charginig period is not changed. To
+disable a charging period, set duration=0. set_tariff() can configure multiple
+charging periods for any tariff using the times parameter instead of start_at,
+end_by and duration. Times is a list of tuples containing values for start_at,
+end_by and duration. For example, this parameter configures an AM charging
+period between 11pm and 8am with a 3 hour period and a PM charging period
+between 12 noon and 4pm with a 1 hour period: + times=[("23:00", "8:00", 3),
+("12:00", "16:00", 1)] 'strategy' allows you to configure times when work modes
+will be changed. The format is a list of dictionary items, containing: +
+'start', 'end': times in decimal hours or time format. The end time is
+exclusive so setting an end time of '07:00' will set a schedule that ends at
+'06:59' + 'mode': the work mode to be used from 'SelfUse', 'Feedin', 'Backup',
+'ForceCharge', 'ForceDischarge' + 'min_soc, 'fdsoc', 'fdpwr': optional values
+for each work mode. The defaults are 10, 10 and 0 respectively. The strategy
+should not include settings for the AM/PM charge times for the tariff. These
+will be added by charge_needed(). # PV Output These functions produce CSV data
+for upload to [pvoutput.org](https://pvoutput.org) including PV generation,
+Export, Load and Grid consumption by day in Wh. The functions use the energy
+estimates created from the raw power data (see above). The estimates include PV
+energy generation that are not otherwise available from the Fox Cloud.
+Typically, the energy results are within 3% of the values reported by the
+meters built into the inverter. ## Get PV Output Data Returns CSV upload data
+using the [API format](https://pvoutput.org/help/api_specification.html#csv-
+data-parameter): ``` f.get_pvoutput(d, tou) ``` + d is the date or a list of
+dates, to get data for. The default is yesterday + tou: optional, setting tou=1
+uploads data with time of use. The default, tou=0 does not split data and is
+more accurate. You can copy and paste the output data to the pvoutput data CSV
+Loader, using the following settings: ![image](https://github.com/TonyM1958/
+FoxESS-Cloud/assets/63789168/21459cdc-a943-4e9d-a204-7efd45a422d8) For example,
+this Jupyer Lab cell will provide a CSV data upload for June 2023: ```
+f.get_pvoutput(f.date_list('2023-06-01', '2023-06-30')) ``` ## Set PV Output
+Data Loads CSV data directly using the PV Ouput API: ``` f.set_pvoutput(d,
+system_id, tou, push) ``` + d is optional and is the date, or a list of dates,
+to upload + system_id is optional and allow you to select where data is
+uploaded to (where you have more than 1 registered system) + tou: optional,
+setting tou=1 uploads data with time of use. The default, tou=0 does not split
+data and is more accurate + push: optional. 0 = do not sent to pushover, 1 =
+send summary to pushover, 2 = send first day summary only # Solar Forecasting #
+Solcast Get and display solar data from your solcast.com account using your API
+key: ``` f.solcast_api_key = "my.solcast_api_key" fcast = f.Solcast() print
+(fcast) ``` Returns a 7 day forecast. Optional parameters are: + days: number
+of days to get. The default is 7 + estimated: whether to get history /
+estimated data. 1 = yes, 0 = no. Default is 0. + reload: cached data handling.
+0 = use saved data, 1 = fetch new data, 2 = use saved data for today (default)
++ quiet: True to stop Solcast producing progress messages Forecast data is
+saved to f.solcast_save. The default is 'solcast.txt'. ``` fcast.plot_daily()
 fcast.plot_hourly(day) ``` Plots the estimate / forecast data. plot_daily()
 plots the daily yield. plot_hourly() plots each day separately. + day:
 optional. 'today', 'tomorrow', 'all' or a specific list of dates. The default
-is to plot today and tomorrow # Pushover Send messages to a pushover user
-account: ``` f.output_spool(app_key, h) f.output(s) f.output_close(plot, file)
-f.output_message(app_key, message, plot) ``` Calling f.output_spool() with an
-app key will start the system spooling output to send to pushover. h is an
-optional header to add as the first line of the message. H may include \
+is to plot today and tomorrow # Forecast.solar Get and display solar data from
+forecast.solar for today and tomorrow: ``` f.solar_array('South', lat=51.1789,
+lon=-1.8262, kwp=6.4) ``` You need to configure your solar arrays by calling
+f.solar_array(). This takes the following parameters: + name: the name of each
+of your arrays + lat: the latitude where the array is located. The default is
+Stonehenge. + lon: the longitude where the array is located. The default is
+Stonehenge. + dec: the declination of the array - 0 is lying flat and 90 is
+vertical. Default is 30 + az: azimuth of the array. 0 is pointing due South, -
+90 is pointing East, 90 is pointing West. The default is 0 + kwp: the size of
+the array in kWp. The default is 5kWp + dam: damping factor. Default is None +
+inv: inverter power limit (when the array will clip). The default is None +
+hor: a list of values describing obstructions on the horizon Add one array for
+each string attached to your inverter. If your solar production is limited by
+clipping, set the inverter power so the forecast better matches your
+generation. See the [API documentation](https://doc.forecast.solar/api) for
+more information on parameter values. ``` fcast = f.Solar() print(fcast) ```
+Returns a forecast for today and tomorrow. Optional parameters are: + reload:
+cached data handling. 0 = use saved data, 1 = fetch new data, 2 = use saved
+data for today (default) + quiet: set to True to stop Solar producing progress
+messages Forecast data is saved to f.solar_save. The default is 'solar.txt'.
+``` fcast.plot_daily() fcast.plot_hourly(day) ``` Plots the estimate / forecast
+data. plot_daily() plots the daily yield. plot_hourly() plots each day
+separately. + day: optional. 'today', 'tomorrow', 'all' or a specific list of
+dates. The default is to plot today and tomorrow # Pushover Send messages to a
+pushover user account: ``` f.output_spool(app_key, h) f.output(s)
+f.output_close(plot, file) f.output_message(app_key, message, plot) ``` Calling
+f.output_spool() with an app key will start the system spooling output to send
+to pushover. h is an optional header to add as the first line of the message. H
+may include \
 >, \
 > or \
 > and these will be set to current system time and date respectively. When
 spooling is active, any calls to f.output() add lines to the spooled message.
 If appending to the message would exceed 1024 characters, the existing spooled
 message is sent and a new message spool is started. Calling f.output_close()
 will send the spooled message and optionally attach a binary image file. You
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.5
-Refactor debug messaging. Simplify charge_needed() output. Added 'target_soc'
-to charge_needed() settings Fix bat_info() giving incorrect temperatures when
-API returns 0 instead of -50 where there is no battery Fix key error when
-accessing cell volts and temps using an agent / installer account. Ensure
-output is generated if get_battery() fails using battery_info(). Update f.avg()
-to include calculation of averages in lists containng None values. Added
+(verbose) # Version Info 2.2.6
+Implement 2 second delay between calls that change inverter settings. Added
+strategy mode (timed_mode=2) to charge_needed(). Added set_strategy() and
+charge_strategy() to manage charging schedules and work mode changes. Refactor
+debug messaging. Simplify charge_needed() output. Added 'target_soc' to
+charge_needed() settings Fix bat_info() giving incorrect temperatures when API
+returns 0 instead of -50 where there is no battery Fix key error when accessing
+cell volts and temps using an agent / installer account. Ensure output is
+generated if get_battery() fails using battery_info(). Update f.avg() to
+include calculation of averages in lists containng None values. Added
 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
```

### Comparing `foxesscloud-2.2.5/pyproject.toml` & `foxesscloud-2.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "foxesscloud"
-version = "2.2.5"
+version = "2.2.6"
 authors = [
   {name="Tony Matthews", email="tony@quasair.co.uk"},
 ]
 description = "library for accessing Fox ESS cloud data using Open API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `foxesscloud-2.2.5/src/foxesscloud/foxesscloud.py` & `foxesscloud-2.2.6/src/foxesscloud/foxesscloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################################
 """
 Module:   Fox ESS Cloud
-Updated:  19 April 2024
+Updated:  12 May 2024
 By:       Tony Matthews
 """
 ##################################################################################################
 # Code for getting and setting inverter data via the Fox ESS cloud web site, including
 # getting forecast data from solcast.com.au and sending inverter data to pvoutput.org
 # ALL RIGHTS ARE RESERVED © Tony Matthews 2023
 ##################################################################################################
 
-version = "1.3.7"
+version = "1.3.8"
 print(f"FoxESS-Cloud version {version}")
 
 debug_setting = 1
 
 # constants
 month_names = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
 day_names = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
@@ -93,15 +93,15 @@
     elif f >= len(v) - 1:
         return v[-1]
     i = int(f)
     x = f - i
     return v[i] * (1-x) + v[i+1] * x
 
 # build request header with signing
-http_timeout = 60        # http request timeout in seconds
+http_timeout = 60       # http request timeout in seconds
 http_tries = 2
 response_time = {}
 
 class MockResponse:
     def __init__(self, status_code, reason):
         self.status_code = status_code
         self.reason = reason
@@ -152,14 +152,32 @@
             return response
         except Exception as e:
             message = str(e)
             output(f"** signed_post(): {message}\n  path = {path}\n  headers = {headers}")
             continue
     return MockResponse(999, message)
 
+# implement minimum time between updates for inverter remote settings
+
+update_delay = 2       # delay between inverter setting updates in seconds
+update_time = {}       # last inverter setting update time
+
+def setting_delay():
+    global update_delay, update_time, device_sn
+    sn = device_sn if device_sn is not None else ''
+    t_now = time.time()
+    t_last = update_time.get(sn)
+    delta = t_now - t_last if t_last is not None else update_delay
+    if delta < update_delay:
+        time.sleep(update_delay - delta)
+        t_now = time.time()
+        output(f"-- setting_delay() --", 2)
+    update_time[sn] = t_now
+    return
+
 
 ##################################################################################################
 # get error messages
 ##################################################################################################
 
 messages = None
 user_agent = None
@@ -668,14 +686,15 @@
         battery_settings['times'][1]['endTime']['hour'] = int(en2)
         battery_settings['times'][1]['endTime']['minute'] = int(60 * (en2 - int(en2)) + 0.5)
     output(f"\nSetting time periods:", 1)
     output(f"   Time Period 1 = {time_period(battery_settings['times'][0])}", 1)
     output(f"   Time Period 2 = {time_period(battery_settings['times'][1])}", 1)
     # set charge times
     data = {'sn': device_sn, 'times': battery_settings.get('times')}
+    setting_delay()
     response = signed_post(path="/c/v0/device/battery/time/set", data=data)
     if response.status_code != 200:
         output(f"** set_charge() got response code {response.status_code}: {response.reason}")
         return None
     errno = response.json().get('errno')
     if errno != 0:
         if errno == 44096:
@@ -683,14 +702,30 @@
         else:
             output(f"** set_charge(), {errno_message(errno)}")
         return None
     else:
         output(f"success", 2) 
     return battery_settings
 
+def charge_strategy(st1 = None, en1 = None, st2 = None, en2 = None, adjust=0, min_soc=None):
+    output(f"\nConfiguring schedule",1)
+    periods = set_strategy()
+    if st1 is not None and en1 is not None and st1 != en1:
+        st1 = round_time(time_hours(st1) + adjust)
+        en1 = round_time(time_hours(en1) + adjust)
+        output(f"   Force Charge from {hours_time(st1)} to {hours_time(en1)}", 1)
+        periods.append(set_period(start = st1, end = en1, mode = 'ForceCharge'))
+    if st2 is not None and en2 is not None and st2 != en2:
+        st2 = round_time(time_hours(st2) + adjust)
+        en2 = round_time(time_hours(en2) + adjust)
+        mode = 'SelfUse'
+        output(f"   {mode} from {hours_time(st2)} to {hours_time(en2)} with min_soc = {min_soc}%", 1)
+        periods.append(set_period(start = st2, end = en2, mode = mode, fdsoc = min_soc))
+    return periods
+
 ##################################################################################################
 # get min soc settings and save in battery_settings
 ##################################################################################################
 
 def get_min():
     global token, device_sn, battery_settings, debug_setting, messages
     if get_device() is None:
@@ -713,15 +748,15 @@
     return battery_settings
 
 ##################################################################################################
 # set min soc from battery_settings or parameters
 ##################################################################################################
 
 def set_min(minGridSoc = None, minSoc = None, force = 0):
-    global token, device_sn, bat_settings, debug_setting, messages, default_min_soc
+    global token, device_sn, battery_settings, debug_setting, messages, default_min_soc
     if get_device() is None:
         return None
     if get_schedule().get('enable'):
         if force == 0:
             output(f"** set_min(): cannot set min SoC mode when a schedule is enabled")
             return None
         set_schedule(enable=0)
@@ -730,17 +765,16 @@
         battery_settings = {}
     if minGridSoc is not None:
         data['minGridSoc'] = minGridSoc
         battery_settings['minGridSoc'] = minGridSoc
     if minSoc is not None:
         data['minSoc'] = minSoc
         battery_settings['minSoc'] = minSoc
-        output(f"set_min(): {battery_settings}", 2)
-        return None
     output(f"\nSetting minSoc = {battery_settings.get('minSoc')}, minGridSoc = {battery_settings.get('minGridSoc')}", 1)
+    setting_delay()
     response = signed_post(path="/c/v0/device/battery/soc/set", data=data)
     if response.status_code != 200:
         output(f"** set_min() got response code {response.status_code}: {response.reason}")
         return None
     errno = response.json().get('errno')
     if errno != 0:
         if errno == 44096:
@@ -972,20 +1006,17 @@
     if get_flag() is None:
         return None
     if schedule.get('enable') == True:
         if force == 0:
             output(f"** set_work_mode(): cannot set work mode when a schedule is enabled")
             return None
         set_schedule(enable=0)
-    if debug_setting > 1:
-        output(f"set_work_mode(): {mode}")
-        return None
-    if debug_setting > 0:
-        output(f"\nSetting work mode: {mode}")
+    output(f"\nSetting work mode: {mode}", 1)
     data = {'id': device_id, 'key': 'operation_mode__work_mode', 'values': {'operation_mode__work_mode': mode}, 'raw': ''}
+    setting_delay()
     response = signed_post(path="/c/v0/device/setting/set", data=data)
     if response.status_code != 200:
         output(f"** set_work_mode() got response code {response.status_code}: {response.reason}")
         return None
     errno = response.json().get('errno')
     if errno != 0:
         if errno == 44096:
@@ -1130,56 +1161,76 @@
     return None
 
 
 ##################################################################################################
 # set schedule
 ##################################################################################################
 
-# create a period structure
-def set_period(start, end, mode, min_soc=10, fdsoc=10, fdpwr=0):
+# create a period structure. Note: end time is exclusive.
+def set_period(start, end, mode=None, min_soc=None, fdsoc=None, fdpwr=None):
     if type(start) is str:
         start = time_hours(start)
     if type(end) is str:
         end = time_hours(end)
     if start is None or end is None:
         return None
+    mode = 'SelfUse' if mode is None else mode
     if mode not in work_modes:
         output(f"** mode must be one of {work_modes}")
         return None
-    device_power = device.get('power')
+    min_soc = 10 if min_soc is None else min_soc
+    fdsoc = 10 if fdsoc is None else fdsoc
+    fdpwr = 0 if fdpwr is None else fdpwr
+    device_power = device.get('power') if device is not None else None
     if device_power is None:
         device_power = 12000
     if fdpwr < 0 or fdpwr > 12000:
         output(f"** fdpwr must be between 0 and {device_power}")
         return None
     if fdsoc < 10 or fdsoc > 100:
         output(f"** fdsoc must between 10 and 100")
         return None
     start_h, start_m = split_hours(start)
-    end_h, end_m = split_hours(end)
+    end_h, end_m = split_hours(end - 1/60)
     period = {'startH': start_h, 'startM': start_m, 'endH': end_h, 'endM': end_m, 'workMode': mode, 'minSocOnGrid': min_soc, 'fdSoc': fdsoc, 'fdPwr': fdpwr}
     return period
 
+# create periods from a list of strategy times:
+def set_strategy(strategy=None):
+    global tariff
+    if strategy is None and tariff is not None:
+        strategy = tariff.get('strategy')
+    if strategy is None:
+        return []
+    if type(strategy) is not list:
+        strategy = [strategy]
+    periods = []
+    for s in strategy:
+        p = set_period(s['start'], s['end'], s['mode'], s.get('min_soc'), s.get('fdsoc'), s.get('fdpwr'))
+        if p is not None:
+            periods.append(p)
+    return periods
+
 # set a schedule from a period or list of periods
-def set_schedule(enable=1, periods=None, template=None):
+def set_schedule(periods=None, template=None, enable=1):
     global token, device_sn, debug_setting, messages, schedule, templates
     if get_flag() is None:
         return None
     if schedule.get('support') == False:
         output(f"** set_schedule(), not supported on this device")
         return None
     if schedule is None:
         schedule = get_schedule()
     output(f"set_schedule(): enable = {enable}, periods = {periods}, template={template}", 2)
     if debug_setting > 1:
         return None
     params = {'deviceSN': device_sn}
     if enable == 0:
-        if debug_setting > 0:
-            output(f"\nDisabling schedule")
+        output(f"\nDisabling schedule", 1)
+        setting_delay()
         response = signed_get(path="/generic/v0/device/scheduler/disable", params=params)
         if response.status_code != 200:
             output(f"** set_schedule() got disable response code {response.status_code}: {response.reason}")
             return None
         errno = response.json().get('errno')
         if errno != 0:
             output(f"** set_schedule(), disable, {errno_message(errno)}")
@@ -1197,16 +1248,16 @@
             template_id = template if template in templates.keys() else find_template(template)
             if template_id is None:
                 return None
             data = {'templateID': template_id, 'deviceSN': device_sn}
         else:
             output(f"** set_schedule() requires periods or template parameter")
             return None
-        if debug_setting > 0:
-            output(f"\nEnabling schedule")
+        output(f"\nEnabling schedule", 1)
+        setting_delay()
         response = signed_post(path="/generic/v0/device/scheduler/enable", data=data)
         if response.status_code != 200:
             output(f"** set_schedule() got enable response code {response.status_code}: {response.reason}")
             return None
         errno = response.json().get('errno')
         if errno != 0:
             output(f"** set_schedule(), enable, {errno_message(errno)}")
@@ -1873,16 +1924,17 @@
 octopus_flux = {
     'name': 'Octopus Flux',
     'off_peak1': {'start': 2.0, 'end': 5.0, 'force': 1},        # off-peak period 1 / am charging period
     'off_peak2': {'start': 0.0, 'end': 0.0, 'force': 0},        # off-peak period 2 / pm charging period
     'peak': {'start': 16.0, 'end': 19.0 },                      # peak period 1
     'peak2': {'start': 0.0, 'end': 0.0 },                       # peak period 2
     'forecast_times': [22, 23],                                 # hours in a day to get a forecast
-    'work_hours': [                                             # timed work mode settings
-        {'mode': 'SelfUse', 'start': 7, 'end': 16}, {'mode': 'Feedin', 'start': 16, 'end': 7}]
+    'strategy': [                                               # timed work mode settings
+        {'start': 5, 'end': 12, 'mode': 'SelfUse'},
+        {'start': 16, 'end': 23, 'mode': 'Feedin'}]
     }
 
 # time periods for Intelligent Octopus
 intelligent_octopus = {
     'name': 'Intelligent Octopus',
     'off_peak1': {'start': 23.5, 'end': 5.5, 'force': 1},
     'off_peak2': {'start': 0.0, 'end': 0.0, 'force': 0},
@@ -2135,15 +2187,15 @@
         tariff['off_peak1']['start'] = start
         tariff['off_peak1']['end'] = end
         gmt = ' GMT' if tariff['off_peak1'].get('gmt') is not None else ''
     print(f"\n{tariff['name']} {am_pm} charging period: {hours_time(start)} to {hours_time(end)}{gmt}")
     return 1
 
 # set tariff and AM/PM charge time period
-def set_tariff(find, update=1, start_at=None, end_by=None, duration=None, times=None, forecast_times=None, work_times=None, d=None, **settings):
+def set_tariff(find, update=1, start_at=None, end_by=None, duration=None, times=None, forecast_times=None, strategy=None, d=None, **settings):
     global debug_setting, agile_octopus, tariff, tariff_list
     print(f"\n---------------- set_tariff -----------------")
     # validate parameters
     args = locals()
     s = ""
     for k in [k for k in args.keys() if args[k] is not None and k != 'settings']:
         s += f"\n  {k} = {args[k]}"
@@ -2186,35 +2238,31 @@
             forecast_times = [forecast_times]
         forecast_hours = []
         for i, t in enumerate(forecast_times):
             forecast_times[i] = hours_time(t)
             forecast_hours.append(time_hours(t))
         use['forecast_times'] = forecast_hours
         output(f"\nForecast times set to {forecast_times}")
-    if work_times is not None:
-        if type(work_times) is not None:
-            work_times = [work_times]
-        work_hours = []
-        for d in work_times:
-            (mode, start, end) = d
-            work_hours.append({'mode': mode, 'start': time_hours(start), 'end': time_hours(end)})
-        use['work_hours'] = work_hours
-        output(f"\nWork mode times set to {work_hours}")
+    if strategy is not None:
+        if type(strategy) is not list:
+            strategy = [strategy]
+        use['strategy'] = strategy
+        output(f"\nStrategy set to {strategy}")
     if update == 1:
         tariff = use
         output(f"\nTariff set to {tariff['name']}")
     else:
         output(f"\nNo changes made to current tariff", 1)
     return None
 
 # get work mode for a time of day based on the tariff:
 def timed_work_mode(h, default = 'SelfUse'):
-    if tariff is None or tariff.get('work_hours') is None:
+    if tariff is None or tariff.get('strategy') is None:
         return default
-    for d in tariff['work_hours']:
+    for d in tariff['strategy']:
         if hour_in(h, d):
             return d['mode']
     return default
 
 ##################################################################################################
 # CHARGE_NEEDED - calculate charge from current battery charge, forecast yield and expected load
 ##################################################################################################
@@ -2324,15 +2372,15 @@
     'use_today': 21.0,                # hour when todays consumption and generation can be used
     'min_hours': 0.25,                # minimum charge time in decimal hours
     'min_kwh': 0.5,                   # minimum to add in kwh
     'solcast_adjust': 100,            # % adjustment to make to Solcast forecast
     'solar_adjust':  100,             # % adjustment to make to Solar forecast
     'forecast_selection': 1,          # 0 = use available forecast / generation, 1 only update settings with forecast
     'annual_consumption': None,       # optional annual consumption in kWh
-    'timed_mode': 0,                  # 1 = apply timed work mode, 0 = None
+    'timed_mode': 0,                  # = = None, 1 = timed mode, 2 = strategy mode
     'special_contingency': 33,        # contingency for special days when consumption might be higher
     'special_days': ['12-25', '12-26', '01-01'],
     'full_charge': None,              # day of month (1-28) to do full charge, or 'daily' or 'Mon', 'Tue' etc
     'derate_temp': 22,                # battery temperature where cold derating starts to be applied
     'derate_step': 5,                 # scale for derating factors in C
     'derating': [24, 15, 10, 2],      # max charge current e.g. 5C step = 22C, 17C, 12C, 7C
     'force': 1,                       # 0 = don't over-ride schedule, 1 = disable schedule
@@ -2341,15 +2389,15 @@
 }
 
 # app key for charge_needed (used to send output via pushover)
 charge_needed_app_key = "awcr5gro2v13oher3v1qu6hwnovp28"
 
 # work out the charge times to set using the parameters:
 #  forecast: the kWh expected tomorrow. If none, forecast data is loaded from solcast etc
-#  update_settings: 0 no updates, 1 update charge settings, 2 update work mode, 3 update both. The default is 0
+#  update_settings: 0 no updates, 1 update charge settings. The default is 0
 #  show_data: 1 shows battery SoC, 2 shows battery residual. Default = 0
 #  show_plot: 1 plots battery SoC, 2 plots battery residual. Default = 1
 #  run_after: 0 over-rides 'forecast_times'. The default is 1.
 #  forecast_times: list of hours when forecast can be fetched
 #  force_charge: 1 = set force charge, 2 = charge for whole period
 
 def charge_needed(forecast=None, update_settings=0, timed_mode=None, show_data=None, show_plot=None, run_after=None,
@@ -2372,15 +2420,15 @@
         output(f"Parameters: {s}", 2)
     if tariff is not None:
         output(f"  tariff = {tariff['name']}", 2)
     # set default parameters
     show_data = 1 if show_data is None or show_data == True else 0 if show_data == False else show_data
     show_plot = 3 if show_plot is None or show_plot == True else 0 if show_plot == False else show_plot
     run_after = 1 if run_after is None else run_after 
-    timed_mode = 1 if timed_mode is None and tariff is not None and tariff.get('work_hours') is not None else 0 if timed_mode is None else timed_mode
+    timed_mode = 1 if timed_mode is None and tariff is not None and tariff.get('strategy') is not None else 0 if timed_mode is None else timed_mode
     if forecast_times is None:
         forecast_times = tariff['forecast_times'] if tariff is not None and tariff.get('forecast_times') is not None else [22,23]
     if type(forecast_times) is not list:
         forecast_times = [forecast_times]
     # get dates and times
     system_time = (datetime.now(tz=timezone.utc) + timedelta(hours=time_shift)) if test_time is None else datetime.strptime(test_time, '%Y-%m-%d %H:%M')
     time_offset = daylight_saving(system_time) if daylight_saving is not None else 0
@@ -2667,24 +2715,24 @@
         output_close()
         return None
     else:
         expected = generation
         generation_timed = [expected * x / sun_sum for x in sun_timed]
         if charge_config['forecast_selection'] == 1 and update_settings > 0:
             output(f"\nSettings will not be updated when forecast is not available")
-            update_settings = 2 if update_settings == 3 else 0
+            update_settings = 0
     # produce time lines for main charge and discharge (after losses)
     charge_timed = [x * charge_config['pv_loss'] for x in generation_timed]
     discharge_timed = [x / charge_config['discharge_loss'] for x in consumption_timed]
     # adjust charge and discharge time lines for work mode, force charge and power limits
     work_mode = current_mode
     for i in range(0, run_time):
         h = base_hour + i
         # get work mode and check for changes
-        new_work_mode = timed_work_mode(h, current_mode) if timed_mode == 1 else current_mode
+        new_work_mode = timed_work_mode(h, current_mode) if timed_mode > 0 else current_mode
         if new_work_mode is not None and new_work_mode != work_mode:
             output(f"  {hours_time(h)}: {new_work_mode} work mode", 2)
             work_mode = new_work_mode
         # cap charge / discharge power
         charge_timed[i] = charge_limit if charge_timed[i] > charge_limit else charge_timed[i]
         discharge_timed[i] = discharge_limit if discharge_timed[i] > discharge_limit else discharge_timed[i]
         if force_charge_am == 1 and hour_in(h, {'start': start_am, 'end': end_am}):
@@ -2738,14 +2786,16 @@
     day_when = 'today' if min_hour < 24 else 'tomorrow' if min_hour <= 48 else 'day after tomorrow'
     if kwh_min > reserve and kwh_needed < charge_config['min_kwh'] and full_charge is None and test_charge is None:
         output(f"\nNo charging is needed (forecast = {expected:.1f}kWh, consumption = {consumption:.1f}kWh)")
         charge_message = "no charge needed"
         kwh_needed = 0.0
         hours = 0.0
         end1 = start_at
+        end_soc = int(start_residual / capacity * 100 + 0.5)
+        output(f"   Expected SoC at {hours_time(start_at)} is {end_soc}%")
     else:
         charge_message = "with charge added"
         if test_charge is None:
             min_hour_adjust = min_hour - hour_adjustment if min_hour >= change_hour else 0
             output(f"\nCharge of {kwh_needed:.2f}kWh is needed (forecast = {expected:.1f}kWh, consumption = {consumption:.1f}kWh)")
         else:
             output(f"\nTest charge of {test_charge}kWh")
@@ -2813,17 +2863,18 @@
             h += 1
         time_to_end = int(start_timed + hours) + 1
         kwh_added = bat_timed[time_to_end] - bat_timed_old[time_to_end]
         end_part_hour = end_timed - int(end_timed)
         old_residual = interpolate(end_timed, bat_timed_old)
         new_residual = capacity if old_residual + kwh_added > capacity else old_residual + kwh_added
         net_added = new_residual - start_residual
+        end_soc = int(new_residual / capacity * 100 + 0.5)
 #        output(f"  Charging for {int(hours * 60)} minutes adds {net_added:.2f}kWh")
         output(f"  Start SoC: {start_residual / capacity * 100:3.0f}% at {hours_time(start_at)} ({start_residual:.2f}kWh)")
-        output(f"  End SoC:   {new_residual / capacity * 100:3.0f}% at {hours_time(end1)} ({new_residual:.2f}kWh)")
+        output(f"  End SoC:   {end_soc:3.0f}% at {hours_time(end1)} ({new_residual:.2f}kWh)")
     if show_data > 2:
         output(f"\nTime, Generation, Charge, Consumption, Discharge, Residual, kWh")
         for i in range(0, run_time):
             h = base_hour + i
             output(f"  {hours_time(h)}, {generation_timed[i]:6.3f}, {charge_timed[i]:6.3f}, {consumption_timed[i]:6.3f}, {discharge_timed[i]:6.3f}, {bat_timed[i]:6.3f}")
         if kwh_needed > 0 and show_data > 3:
             output(f"\nTime, Generation, Charge, Consumption, Discharge, Residual, kWh (before charging)")
@@ -2869,19 +2920,23 @@
     # work out charge periods settings
     start2 = round_time(start_at if hours == 0 else end1 + 1 / 60)       # add 1 minute to end time
     if force_charge == 1 and hour_in(start2, {'start':start_at, 'end': end_by}):
         end2 = end_by
     else:
             end2 = start2
     # setup charging
-    if update_settings in [1,3]:
+    if update_settings == 1:
         # adjust times for clock changes
         adjust = hour_adjustment if hour_adjustment != 0 and start_hour > change_hour else 0
-
-        set_charge(ch1 = True, st1 = start_at, en1 = end1, ch2 = False, st2 = start2, en2 = end2, adjust = adjust, force = charge_config['force'])
+        if timed_mode > 1:
+            schedule = charge_strategy(st1 = start_at, en1 = end1, st2 = start2, en2 = end2, adjust = adjust, min_soc = end_soc)
+            output(f"Schedule = {schedule}", 2)
+            set_schedule(periods = schedule)
+        else:
+            set_charge(ch1 = True, st1 = start_at, en1 = end1, ch2 = False, st2 = start2, en2 = end2, adjust = adjust, force = charge_config['force'])
     else:
         print(f"\nNo changes made to charge settings")
     output_close(plot=show_plot)
     return None
 
 
 ##################################################################################################
```

### Comparing `foxesscloud-2.2.5/src/foxesscloud/openapi.py` & `foxesscloud-2.2.6/src/foxesscloud/openapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################################
 """
 Module:   Fox ESS Cloud using Open API
-Updated:  19 April 2024
+Updated:  12 May 2024
 By:       Tony Matthews
 """
 ##################################################################################################
 # Code for getting and setting inverter data via the Fox ESS cloud api site, including
 # getting forecast data from solcast.com.au and sending inverter data to pvoutput.org
 # ALL RIGHTS ARE RESERVED © Tony Matthews 2024
 ##################################################################################################
 
-version = "2.2.5"
+version = "2.2.6"
 print(f"FoxESS-Cloud Open API version {version}")
 
 debug_setting = 1
 
 # constants
 month_names = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
 day_names = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
@@ -116,14 +116,15 @@
     return v[i] * (1-x) + v[i+1] * x
 
 # return the average of a list
 def avg(x):
     if len(x) == 0:
         return None
     return sum(x) / len(x)
+
 # build request header with signing and throttling for queries
 
 last_call = {}          # timestamp of the last call for a given path
 response_time = {}      # response time in seconds of the last call for a given path
 query_delay = 1         # minimum time between calls in seconds
 http_timeout = 60       # http request timeout in seconds
 http_tries = 2          # number of times to re-try requst
@@ -190,14 +191,31 @@
             return response
         except Exception as e:
             message = str(e)
             output(f"** signed_post(): {message}\n  path = {path}\n  headers = {headers}")
             continue
     return MockResponse(999, message)
 
+# implement minimum time between updates for inverter remote settings
+
+update_delay = 2       # delay between inverter setting updates in seconds
+update_time = {}       # last inverter setting update time
+
+def setting_delay():
+    global update_delay, update_time, device_sn
+    sn = device_sn if device_sn is not None else ''
+    t_now = time.time()
+    t_last = update_time.get(sn)
+    delta = t_now - t_last if t_last is not None else update_delay
+    if delta < update_delay:
+        time.sleep(update_delay - delta)
+        t_now = time.time()
+        output(f"-- setting_delay() --", 2)
+    update_time[sn] = t_now
+    return
 
 ##################################################################################################
 # get error messages / error handling
 ##################################################################################################
 
 messages = None
 
@@ -619,14 +637,15 @@
     output(f"\nSetting time periods:", 1)
     output(f"   Time Period 1 = {time_period(battery_settings['times'], 1)}", 1)
     output(f"   Time Period 2 = {time_period(battery_settings['times'], 2)}", 1)
     # set charge times
     body = {'sn': device_sn}
     for k in ['enable1', 'startTime1', 'endTime1', 'enable2', 'startTime2', 'endTime2']:
         body[k] = battery_settings['times'][k]          # try forcing order of items?
+    setting_delay
     response = signed_post(path="/op/v0/device/battery/forceChargeTime/set", body=body)
     if response.status_code != 200:
         output(f"** set_charge() got response code {response.status_code}: {response.reason}")
         return None
     errno = response.json().get('errno')
     if errno != 0:
         if errno == 44096:
@@ -634,14 +653,30 @@
         else:
             output(f"** set_charge(), {errno_message(response)}")
         return None
     else:
         output(f"success", 2) 
     return battery_settings
 
+def charge_strategy(st1 = None, en1 = None, st2 = None, en2 = None, adjust=0, min_soc=None):
+    output(f"\nConfiguring schedule", 1)
+    periods = set_strategy()
+    if st1 is not None and en1 is not None and st1 != en1:
+        st1 = round_time(time_hours(st1) + adjust)
+        en1 = round_time(time_hours(en1) + adjust)
+        output(f"   Force Charge from {hours_time(st1)} to {hours_time(en1)}", 1)
+        periods.append(set_group(start = st1, end = en1, mode = 'ForceCharge'))
+    if st2 is not None and en2 is not None and st2 != en2:
+        st2 = round_time(time_hours(st2) + adjust)
+        en2 = round_time(time_hours(en2) + adjust)
+        mode = 'SelfUse'
+        output(f"   {mode} from {hours_time(st2)} to {hours_time(en2)} with min_soc = {min_soc}%", 1)
+        periods.append(set_group(start = st2, end = en2, mode = mode, fdsoc = min_soc))
+    return periods
+
 ##################################################################################################
 # get min soc settings and save in battery_settings
 ##################################################################################################
 
 def get_min():
     global token, device_sn, battery_settings, debug_setting
     if get_device() is None:
@@ -683,23 +718,21 @@
             return None
         battery_settings['minSocOnGrid'] = minSocOnGrid
     if minSoc is not None:
         if minSoc < 10 or minSoc > 100:
             output(f"** set_min(): invalid minSoc = {minSoc}. Must be between 10 and 100")
             return None
         battery_settings['minSoc'] = minSoc
-    if debug_setting > 1:
-        output(f"set_min(): {battery_settings}")
-        return None
     body = {'sn': device_sn}
     if battery_settings.get('minSocOnGrid') is not None:
         body['minSocOnGrid'] = battery_settings['minSocOnGrid']
     if battery_settings.get('minSoc') is not None:
         body['minSoc'] = battery_settings['minSoc']
     output(f"\nSetting minSoc = {battery_settings.get('minSoc')}, minSocOnGrid = {battery_settings.get('minSocOnGrid')}", 1)
+    setting_delay()
     response = signed_post(path="/op/v0/device/battery/soc/set", body=body)
     if response.status_code != 200:
         output(f"** set_min() got response code {response.status_code}: {response.reason}")
         return None
     errno = response.json().get('errno')
     if errno != 0:
         if errno == 44096:
@@ -933,19 +966,17 @@
         output(f"** work mode: must be one of {settable_modes}")
         return None
     if get_schedule().get('enable'):
         if force == 0:
             output(f"** set_work_mode(): cannot set work mode when a schedule is enabled")
             return None
         set_schedule(enable=0)
-    if debug_setting > 1:
-        output(f"set_work_mode(): {mode}")
-        return None
     output(f"\nSetting work mode: {mode}", 1)
     body = {'sn': device_sn, 'key': 'operation_mode__work_mode', 'values': {'operation_mode__work_mode': mode}, 'raw': ''}
+    setting_delay()
     response = signed_post(path="/op/v0/device/setting/set", body=body)
     if response.status_code != 200:
         output(f"** set_work_mode() got response code {response.status_code}: {response.reason}")
         return None
     errno = response.json().get('errno')
     if errno != 0:
         if errno == 44096:
@@ -1014,61 +1045,85 @@
             schedule['groups'].append(g)
     return schedule
 
 ##################################################################################################
 # set schedule
 ##################################################################################################
 
-# create time segment structure
-def set_group(start, end, mode, min_soc=10, fdsoc=10, fdpwr=0, enable=1):
+# create time segment structure. Note: end time is exclusive.
+def set_group(start, end, mode=None, min_soc=None, fdsoc=None, fdpwr=None, enable=1):
     if start is None or end is None:
         return None
     start = time_hours(start)
     end = time_hours(end)
+    mode = 'SelfUse' if mode is None else mode
+    min_soc = 10 if min_soc is None else min_soc
+    fdsoc = 10 if fdsoc is None else fdsoc
+    fdpwr = 0 if fdpwr is None else fdpwr
     if mode not in work_modes:
         output(f"** mode must be one of {work_modes}")
         return None
-    device_power = device.get('power')
+    device_power = device.get('power') if device is not None else None
     if device_power is None:
         device_power = 12000
     if fdpwr < 0 or fdpwr > 12000:
         output(f"** fdpwr must be between 0 and {device_power}")
         return None
     if fdsoc < 10 or fdsoc > 100:
         output(f"** fdsoc must between 10 and 100")
         return None
     start_hour, start_minute = split_hours(start)
-    end_hour, end_minute = split_hours(end)
+    end_hour, end_minute = split_hours(end - 1/60)
     group = {'enable': enable, 'startHour': start_hour, 'startMinute': start_minute, 'endHour': end_hour, 'endMinute': end_minute, 'workMode': mode, 'minSocOnGrid': min_soc, 'fdSoc': fdsoc, 'fdPwr': fdpwr}
     return group
 
+# create groups from a list of strategy periods
+def set_strategy(strategy=None):
+    global tariff
+    if strategy is None and tariff is not None:
+        strategy = tariff.get('strategy')
+    if strategy is None:
+        return []
+    if type(strategy) is not list:
+        strategy = [strategy]
+    groups = []
+    for s in strategy:
+        p = set_group(s['start'], s['end'], s.get('mode'), s.get('min_soc'), s.get('fdsoc'), s.get('fdpwr'))
+        if p is not None:
+            groups.append(p)
+    return groups
+
 # set a schedule from a period or list of time segment groups
-def set_schedule(enable=1, groups=None):
+def set_schedule(groups=None, enable=1):
     global token, device_sn, debug_setting, schedule
     if get_flag() is None:
         return None
     output(f"set_schedule(): enable = {enable}, groups = {groups}", 2)
     if debug_setting > 1:
         return None
+    if enable == 0:
+        output(f"\nDisabling schedule", 1)
+    else:
+        output(f"\nEnabling schedule", 1)
     if groups is not None:
         if type(groups) is not list:
             groups = [groups]
         body = {'deviceSN': device_sn, 'groups': groups}
-        output(f"\nSaving schedule", 1)
+        setting_delay()
         response = signed_post(path="/op/v0/device/scheduler/enable", body=body)
         if response.status_code != 200:
             output(f"** set_schedule() groups response code {response.status_code}: {response.reason}")
             return None
         errno = response.json().get('errno')
         if errno != 0:
             output(f"** set_schedule(), enable, {errno_message(response)}")
             return None
         schedule['groups'] = groups
-    output(f"\nSetting schedule enable flag to {enable}", 1)
     body = {'deviceSN': device_sn, 'enable': enable}
+    setting_delay()
     response = signed_post(path="/op/v0/device/scheduler/set/flag", body=body)
     if response.status_code != 200:
         output(f"** set_schedule() flag response code {response.status_code}: {response.reason}")
         return None
     errno = response.json().get('errno')
     if errno != 0:
         output(f"** set_schedule(), flag, {errno_message(response)}")
@@ -1742,16 +1797,17 @@
 octopus_flux = {
     'name': 'Octopus Flux',
     'off_peak1': {'start': 2.0, 'end': 5.0, 'force': 1},        # off-peak period 1 / am charging period
     'off_peak2': {'start': 0.0, 'end': 0.0, 'force': 0},        # off-peak period 2 / pm charging period
     'peak': {'start': 16.0, 'end': 19.0 },                      # peak period 1
     'peak2': {'start': 0.0, 'end': 0.0 },                       # peak period 2
     'forecast_times': [22, 23],                                 # hours in a day to get a forecast
-    'work_hours': [                                             # timed work mode settings
-        {'mode': 'SelfUse', 'start': 7, 'end': 16}, {'mode': 'Feedin', 'start': 16, 'end': 7}]
+    'strategy': [                                               # timed work mode settings
+        {'start': 5, 'end': 12, 'mode': 'SelfUse'},
+        {'start': 16, 'end': 23, 'mode': 'Feedin'}]
     }
 
 # time periods for Intelligent Octopus
 intelligent_octopus = {
     'name': 'Intelligent Octopus',
     'off_peak1': {'start': 23.5, 'end': 5.5, 'force': 1},
     'off_peak2': {'start': 0.0, 'end': 0.0, 'force': 0},
@@ -2004,15 +2060,15 @@
         tariff['off_peak1']['start'] = start
         tariff['off_peak1']['end'] = end
         gmt = " GMT" if tariff['off_peak1'].get('gmt') is not None else ""
     print(f"\n{tariff['name']} {am_pm} charging period: {hours_time(start)} to {hours_time(end)}{gmt}")
     return 1
 
 # set tariff and AM/PM charge time period
-def set_tariff(find, update=1, start_at=None, end_by=None, duration=None, times=None, forecast_times=None, work_times=None, d=None, **settings):
+def set_tariff(find, update=1, start_at=None, end_by=None, duration=None, times=None, forecast_times=None, strategy=None, d=None, **settings):
     global debug_setting, agile_octopus, tariff, tariff_list
     print(f"\n---------------- set_tariff -----------------")
     # validate parameters
     args = locals()
     s = ""
     for k in [k for k in args.keys() if args[k] is not None and k != 'settings']:
         s += f"\n  {k} = {args[k]}"
@@ -2055,35 +2111,31 @@
             forecast_times = [forecast_times]
         forecast_hours = []
         for i, t in enumerate(forecast_times):
             forecast_times[i] = hours_time(t)
             forecast_hours.append(time_hours(t))
         use['forecast_times'] = forecast_hours
         print(f"\nForecast times set to {forecast_times}")
-    if work_times is not None:
-        if type(work_times) is not None:
-            work_times = [work_times]
-        work_hours = []
-        for d in work_times:
-            (mode, start, end) = d
-            work_hours.append({'mode': mode, 'start': time_hours(start), 'end': time_hours(end)})
-        use['work_hours'] = work_hours
-        print(f"\nWork mode times set to {work_hours}")
+    if strategy is not None:
+        if type(strategy) is not list:
+            strategy = [strategy]
+        use['strategy'] = strategy
+        print(f"\nStrategy set to {strategy}")
     if update == 1:
         tariff = use
         print(f"\nTariff set to {tariff['name']}")
     elif debug_setting > 0:
         print(f"\nNo changes made to current tariff")
     return None
 
 # get work mode for a time of day based on the tariff:
 def timed_work_mode(h, default = 'SelfUse'):
-    if tariff is None or tariff.get('work_hours') is None:
+    if tariff is None or tariff.get('strategy') is None:
         return default
-    for d in tariff['work_hours']:
+    for d in tariff['strategy']:
         if hour_in(h, d):
             return d['mode']
     return default
 
 ##################################################################################################
 # CHARGE_NEEDED - calculate charge from current battery charge, forecast yield and expected load
 ##################################################################################################
@@ -2193,15 +2245,15 @@
     'use_today': 21.0,                # hour when todays consumption and generation can be used
     'min_hours': 0.25,                # minimum charge time in decimal hours
     'min_kwh': 0.5,                   # minimum to add in kwh
     'solcast_adjust': 100,            # % adjustment to make to Solcast forecast
     'solar_adjust':  100,             # % adjustment to make to Solar forecast
     'forecast_selection': 1,          # 0 = use available forecast / generation, 1 only update settings with forecast
     'annual_consumption': None,       # optional annual consumption in kWh
-    'timed_mode': 0,                  # 1 = apply timed work mode, 0 = None
+    'timed_mode': 0,                  # 0 = None, 1 = timed mode, 2 = strategy mode
     'special_contingency': 33,        # contingency for special days when consumption might be higher
     'special_days': ['12-25', '12-26', '01-01'],
     'full_charge': None,              # day of month (1-28) to do full charge, or 'daily' or 'Mon', 'Tue' etc
     'derate_temp': 22,                # battery temperature where cold derating starts to be applied
     'derate_step': 5,                 # scale for derating factors in C
     'derating': [24, 15, 10, 2],      # max charge current e.g. 5C step = 22C, 17C, 12C, 7C
     'force': 1,                       # 0 = don't over-ride schedule, 1 = disable schedule
@@ -2210,15 +2262,15 @@
 }
 
 # app key for charge_needed (used to send output via pushover)
 charge_needed_app_key = "awcr5gro2v13oher3v1qu6hwnovp28"
 
 # work out the charge times to set using the parameters:
 #  forecast: the kWh expected tomorrow. If none, forecast data is loaded from solcast etc
-#  update_settings: 0 no updates, 1 update charge settings, 2 update work mode, 3 update both. The default is 0
+#  update_settings: 0 no updates, 1 update charge settings. The default is 0
 #  show_data: 1 shows battery SoC, 2 shows battery residual. Default = 0
 #  show_plot: 1 plots battery SoC, 2 plots battery residual. Default = 1
 #  run_after: 0 over-rides 'forecast_times'. The default is 1.
 #  forecast_times: list of hours when forecast can be fetched
 #  force_charge: 1 = set force charge, 2 = charge for whole period
 
 def charge_needed(forecast=None, update_settings=0, timed_mode=None, show_data=None, show_plot=None, run_after=None,
@@ -2241,15 +2293,15 @@
         output(f"Parameters: {s}", 2)
     if tariff is not None:
         output(f"  tariff = {tariff['name']}", 2)
     # set default parameters
     show_data = 1 if show_data is None or show_data == True else 0 if show_data == False else show_data
     show_plot = 3 if show_plot is None or show_plot == True else 0 if show_plot == False else show_plot
     run_after = 1 if run_after is None else run_after 
-    timed_mode = 1 if timed_mode is None and tariff is not None and tariff.get('work_hours') is not None else 0 if timed_mode is None else timed_mode
+    timed_mode = 1 if timed_mode is None and tariff is not None and tariff.get('strategy') is not None else 0 if timed_mode is None else timed_mode
     if forecast_times is None:
         forecast_times = tariff['forecast_times'] if tariff is not None and tariff.get('forecast_times') is not None else [22,23]
     if type(forecast_times) is not list:
         forecast_times = [forecast_times]
     # get dates and times
     system_time = (datetime.now(tz=timezone.utc) + timedelta(hours=time_shift)) if test_time is None else datetime.strptime(test_time, '%Y-%m-%d %H:%M')
     time_offset = daylight_saving(system_time) if daylight_saving is not None else 0
@@ -2533,24 +2585,24 @@
         output_close()
         return None
     else:
         expected = generation
         generation_timed = [expected * x / sun_sum for x in sun_timed]
         if charge_config['forecast_selection'] == 1 and update_settings > 0:
             output(f"\nSettings will not be updated when forecast is not available")
-            update_settings = 2 if update_settings == 3 else 0
+            update_settings = 0
     # produce time lines for main charge and discharge (after losses)
     charge_timed = [x * charge_config['pv_loss'] for x in generation_timed]
     discharge_timed = [x / charge_config['discharge_loss'] for x in consumption_timed]
     # adjust charge and discharge time lines for work mode, force charge and power limits
     work_mode = current_mode
     for i in range(0, run_time):
         h = base_hour + i
         # get work mode and check for changes
-        new_work_mode = timed_work_mode(h, current_mode) if timed_mode == 1 else current_mode
+        new_work_mode = timed_work_mode(h, current_mode) if timed_mode > 0 else current_mode
         if new_work_mode is not None and new_work_mode != work_mode:
             output(f"  {hours_time(h)}: {new_work_mode} work mode", 2)
             work_mode = new_work_mode
         # cap charge / discharge power
         charge_timed[i] = charge_limit if charge_timed[i] > charge_limit else charge_timed[i]
         discharge_timed[i] = discharge_limit if discharge_timed[i] > discharge_limit else discharge_timed[i]
         if force_charge_am == 1 and hour_in(h, {'start': start_am, 'end': end_am}):
@@ -2604,14 +2656,16 @@
     day_when = 'today' if min_hour < 24 else 'tomorrow' if min_hour <= 48 else 'day after tomorrow'
     if kwh_min > reserve and kwh_needed < charge_config['min_kwh'] and full_charge is None and test_charge is None:
         output(f"\nNo charging is needed (forecast = {expected:.1f}kWh, consumption = {consumption:.1f}kWh)")
         charge_message = "no charge needed"
         kwh_needed = 0.0
         hours = 0.0
         end1 = start_at
+        end_soc = int(start_residual / capacity * 100 + 0.5)
+        output(f"   Expected SoC at {hours_time(start_at)} is {end_soc}%")
     else:
         charge_message = "with charge added"
         if test_charge is None:
             min_hour_adjust = min_hour - hour_adjustment if min_hour >= change_hour else 0
             output(f"\nCharge of {kwh_needed:.2f}kWh is needed (forecast = {expected:.1f}kWh, consumption = {consumption:.1f}kWh)")
         else:
             output(f"\nTest charge of {test_charge}kWh")
@@ -2678,17 +2732,18 @@
             h += 1
         time_to_end = int(start_timed + hours) + 1
         kwh_added = bat_timed[time_to_end] - bat_timed_old[time_to_end]
         end_part_hour = end_timed - int(end_timed)
         old_residual = interpolate(end_timed, bat_timed_old)
         new_residual = capacity if old_residual + kwh_added > capacity else old_residual + kwh_added
         net_added = new_residual - start_residual
+        end_soc = int(new_residual / capacity * 100 + 0.5)
 #        output(f"  Charging for {int(hours * 60)} minutes adds {net_added:.2f}kWh")
         output(f"  Start SoC: {start_residual / capacity * 100:3.0f}% at {hours_time(start_at)} ({start_residual:.2f}kWh)")
-        output(f"  End SoC:   {new_residual / capacity * 100:3.0f}% at {hours_time(end1)} ({new_residual:.2f}kWh)")
+        output(f"  End SoC:   {end_soc:3.0f}% at {hours_time(end1)} ({new_residual:.2f}kWh)")
     if show_data > 2:
         output(f"\nTime, Generation, Charge, Consumption, Discharge, Residual, kWh")
         for i in range(0, run_time):
             h = base_hour + i
             output(f"  {hours_time(h)}, {generation_timed[i]:6.3f}, {charge_timed[i]:6.3f}, {consumption_timed[i]:6.3f}, {discharge_timed[i]:6.3f}, {bat_timed[i]:6.3f}")
         if kwh_needed > 0 and show_data > 3:
             output(f"\nTime, Generation, Charge, Consumption, Discharge, Residual, kWh (before charging)")
@@ -2732,20 +2787,25 @@
     if test_charge is not None:
         return None
     # work out charge periods settings
     start2 = round_time(start_at if hours == 0 else end1 + 1 / 60)       # add 1 minute to end time
     if force_charge == 1 and hour_in(start2, {'start':start_at, 'end': end_by}):
         end2 = end_by
     else:
-            end2 = start2
+        end2 = start2
     # setup charging
-    if update_settings in [1,3]:
+    if update_settings == 1:
         # adjust times for clock changes
         adjust = hour_adjustment if hour_adjustment != 0 and start_hour > change_hour else 0
-        set_charge(ch1 = True, st1 = start_at, en1 = end1, ch2 = False, st2 = start2, en2 = end2, adjust = adjust, force = charge_config['force'])
+        if timed_mode > 1:
+            schedule = charge_strategy(st1 = start_at, en1 = end1, st2 = start2, en2 = end2, adjust = adjust, min_soc = end_soc)
+            output(f"Schedule = {schedule}", 2)
+            set_schedule(schedule)
+        else:
+            set_charge(ch1 = True, st1 = start_at, en1 = end1, ch2 = False, st2 = start2, en2 = end2, adjust = adjust, force = charge_config['force'])
     else:
         output(f"\nNo changes made to charge settings")
     output_close(plot=show_plot)
     return None
 
 
 ##################################################################################################
```

### Comparing `foxesscloud-2.2.5/src/foxesscloud.egg-info/PKG-INFO` & `foxesscloud-2.2.6/src/foxesscloud.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxesscloud
-Version: 2.2.5
+Version: 2.2.6
 Summary: library for accessing Fox ESS cloud data using Open API
 Author-email: Tony Matthews <tony@quasair.co.uk>
 Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -95,63 +95,74 @@
 
 ```
 f.get_generation()
 f.get_battery()
 f.get_settings()
 f.get_charge()
 f.get_min()
+f.get_flag()
 f.get_schedule()
 
 ```
 Each of these calls will return a dictionary or list containing the relevant information.
 
 get_generation() will return the latest generation information for the device. The results are also stored in f.device as 'generationToday', 'generationMonth' and 'generationTotal'.
 
 get_battery() returns the current battery status, including 'soc', 'volt', 'current', 'power', 'temperature' and 'residual'. The result also updates f.battery.
 
 get_settings() will return the battery settings and is equivalent to get_charge() and get_min(). The results are stored in f.battery_settings. The settings include minSoc, minSocOnGrid, enable charge from grid and the charge times.
 
+get_flag() returns the current scheduler enable / support flags
+
 get_schedule() returns the current work mode / soc schedule settings. The result is stored in f.schedule.
 
 
 ## Inverter Settings
 You can change inverter settings using:
 
 ```
 f.set_min(minSocOnGrid, minSoc)
 f.set_charge(ch1, st1, en1, ch2, st2, en2)
 f.set_group(start, end, mode, min_soc, fdsoc, fdpwr)
-f.get_flag()
-f.set_schedule(enable, groups, template)
+f.set_strategy(strategy)
+f.charge_strategy(st1, en1, st2, en2, min_soc)
+f.set_schedule(groups, enable)
 ```
 
 set_min() applies new SoC settings to the inverter. The parameters update battery_settings:
 + minSocOnGrid: min Soc on Grid setting e.g. 15 = 15%
 + minSoc: min Soc setting e.g. 10 = 10%
 
 set_charge() takes the charge times from the battery_settings and applies these to the inverter. The parameters are optional and will update battery_settings. You should specify all 3 parameter for a time period:
 + ch1: enable charge from grid for period 1 (True or False)
 + st1: the start time for period 1
 + en1: the end time for period 1
 + ch2: enable charge from grid for period 2 (True or False)
 + st2: the start time for period 2
 + en2: the end time for period 2
 
-set_flag() returns the current settings for strategy periods: 'supported' and 'enable'
-
 set_group() returns a time segment structure that can be used to build a list of time segments for set_schedule()
-+ start, end, mode: required parameters
++ start, end, mode: required parameters. end time is exclusive e.g. end at '07:00' will set a period end time of '06:59'
 + min_soc: optional, default is 10
 + fdsoc: optional, default is 10. Used when setting a period with ForceDischarge mode
 + fdpwr: optional, default is 0. Used when setting a period with ForceDischarge mode
 + enable: sets whether this time segment is enable (1) or disabled (0). The default is enabled.
 
+set_strategy() creates a list of groups from the strategy. If strategy is not provided, it uses the strategy for the current tariff.
+
+charge_strategy(): returns a list of groups that describe the strategy for the current tariff and adds the groupd required for charging:
++ st1: the start time for the period when the battery charges from the grid
++ en1: the end time for period 1
++ st2: the start time for period when the battery is held at min_soc
++ en2: the end time for period 2
++ min_soc: the min_soc to use after the charge period, when you don't want the battery to discharge below this level
+
 set_schedule() configures a list of scheduled work mode / soc changes with enable=1. If called with enable=0, any existing schedules are disabled. To enable a schedule, you must provide a list of time segments
-+ enable: 1 to enable schedules, 0 to disable schedules. The default is 1.
 + groups: a time segment or list of time segments created using f.set_group().
++ enable: 1 to enable schedules, 0 to disable schedules. The default is 1.
 
 
 ## Real Time Data
 Real time data reports the latest values for inverter variables, collected every 5 minutes:
 
 ```
 f.invert_ct2 = 1
@@ -294,18 +305,18 @@
 
 ```
 f.charge_needed(forecast, force_charge, forecast_selection, forecast_times, update_setings, show_data, show_plot)
 ```
 
 All the parameters are optional:
 + forecast: the kWh expected tomorrow (optional, see below)
-+ force_charge: 1 any remaining time in a charge period has force charge set, 2 charging uses the entire charge period, 0 None (default)
++ force_charge: 1 any remaining time in a charge period has force charge / min_soc set, 2 charging uses the entire charge period, 0 None (default)
 + forecast_selection: if set to 1, settings are only updated if there is a forecast. Default is 0, generation is used when forecasts are not available
 + forecast_times: a list of hours when forecasts can be obtained. By default, the forecast times for the selected tariff are used (see below)
-+ update_settings: 0 no changes, 1 update charge time, 2 update work mode, 3 update charge time and work mode. The default is 0
++ update_settings: 0 no changes, 1 update charge settings. The default is 0
 + show_data: 1 show battery SoC data, 2 show battery Residual data, 3 show timed data, 4 show timed data before and after charging. The default is 1.
 + show_plot: 1 plot battery SoC data. 2 plot battery Residual, Generation and Consumption. 3 plot 2 + Charge and Discharge The default is 3
 
 ### Modelling
 
 charge_needed() uses a number of models to better estimate the state of the battery.
 
@@ -358,15 +369,15 @@
 use_today: 21.0               # hour when today's generation and consumption data will be used
 min_hours: 0.25               # minimum charge time to set (in decimal hours)
 min_kwh: 0.5                  # minimum charge to add in kwh
 solcast_adjust: 100           # % adjustment to make to Solcast forecast
 solar_adjust:  100            # % adjustment to make to Solar forecast
 forecast_selection: 1         # 1 = only update charge times if forecast is available, 0 = use best available data. Default is 1.
 annual_consumption: None      # optional annual consumption in kWh. If set, this replaces consumption history
-timed_mode: 0                 # 1 = apply timed work mode, 0 = None
+timed_mode: 0                 # 0 = None, 1 = use timed work mode, 2 = strategy mode
 special_contingency: 30       # contingency for special days when consumption might be higher
 special_days: ['12-25', '12-26', '01-01']
 full_charge: None             # day of month (1-28) to do full charge or 'daily' or day of week: 'Mon', 'Tue' etc
 derate_temp: 21               # battery temperature in C when derating charge current is applied
 derate_step: 5                # step size for derating e.g. 21, 16, 11
 derating: [24, 15, 10, 2]     # derated charge current for each temperature step e.g. 21C, 16C, 11C, 6C
 force: 1                      # 1 = disable strategy periods when setting charge. 0 = fail if strategy period has been set.
@@ -376,14 +387,16 @@
 These values are stored / available in f.charge_config.
 
 The default battery open circuit voltage curve versus SoC from 0% to 100% is:
 ```
 lifepo4_curve = [51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50]
 ```
 
+When operating in strategy mode (timed_mode=2), charge_needed will create a schedule that includes the strategy for the tariff with additional time segments added to charge from grid and (optionall) to stop the battery discharging. In other modes, charge_needed() will disable any schedules and set the battery charge times.
+
 This example shows the results reported by charge needed:
 
 ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-b165-20d806b1e7e8)
 
 
 ## Battery Info
 
@@ -467,26 +480,26 @@
 ```
 f.set_tariff('flux')
 ```
 
 When Agile Octopus is selected, a price based charging period is configured using the 30 minute price forecast. For example:
 
 ```
-f.set_tariff('agile', product, region, start_at, end_by, duration, times, forecast_times, work_times, update, weighting, time_shift)
+f.set_tariff('agile', product, region, start_at, end_by, duration, times, forecast_times, strategy, update, weighting, time_shift)
 ```
 
 This gets the latest 30 minute pricing and uses this to work out the best off peak charging period.
 + product: optional Agile Octopus product code (see below). The default is "AGILE-FLEX-22-11-25"
 + region: optional region to use for prices (se below). The default is 'H' (Southern England)
 + start_at: optional earliest start time for charge period in hours, the default is 23:00
 + end_by: optional latest end time for charge period in hours, the default is 08:00
 + duration: optional charge time period in hours, the default is 3 hours. Valid range is 1-6 hours
 + times: a list of charge periods that can be used instead of start_at, end_by and duration (see below)
 + forecast_times: a list of times when a forecast can be obtained from Solcast / forecast.solar
-+ work_times: a list of work modes and times when these are set. The format is [(mode, start, end),...]
++ strategy: an optional list of times and work modes (see below)
 + update: optional, 1 (the default) sets the current tariff to Agile Octopus. Setting to 0 does not change the current tariff
 + weighting: optional, default is None (see below)
 + time_shift: optional system time shift in hours. The default is for system time to be UTC and to apply the current day light saving time (e.g. GMT/BST)
 
 Product codes include: 
 + 'AGILE-18-02-21' = The original version capped at 35p per unit
 + 'AGILE-22-07-22' = The cap rose to 55p
@@ -520,14 +533,21 @@
 Specifying start_at, end_by and duration allows either the AM or PM charging slot for any tariif to be updated, depending on the time. Agile periods will be calculated; othe rtariffs will use the start and end times directly. By default, set_tariff() updates the AM charge period if start_at is after 9pm and end_by is before 8am; it updates the PM charge period if start_at is after 8am and the end_by is before 9pm. Only the relevant AM or PM charge time is updated e.g. if you configure a PM charging period, the AM charginig period is not changed.
 
 To disable a charging period, set duration=0.
 
 set_tariff() can configure multiple charging periods for any tariff using the times parameter instead of start_at, end_by and duration. Times is a list of tuples containing values for start_at, end_by and duration. For example, this parameter configures an AM charging period between 11pm and 8am with a 3 hour period and a PM charging period between 12 noon and 4pm with a 1 hour period:
 + times=[("23:00", "8:00", 3), ("12:00", "16:00", 1)]
 
+'strategy' allows you to configure times when work modes will be changed. The format is a list of dictionary items, containing:
++ 'start', 'end': times in decimal hours or time format. The end time is exclusive so setting an end time of '07:00' will set a schedule that ends at '06:59'
++ 'mode': the work mode to be used from 'SelfUse', 'Feedin', 'Backup', 'ForceCharge', 'ForceDischarge'
++ 'min_soc, 'fdsoc', 'fdpwr': optional values for each work mode. The defaults are 10, 10 and 0 respectively.
+
+The strategy should not include settings for the AM/PM charge times for the tariff. These will be added by charge_needed().
+
 
 # PV Output
 These functions produce CSV data for upload to [pvoutput.org](https://pvoutput.org) including PV generation, Export, Load and Grid consumption by day in Wh. The functions use the energy estimates created from the raw power data (see above). The estimates include PV energy generation that are not otherwise available from the Fox Cloud. Typically, the energy results are within 3% of the values reported by the meters built into the inverter.
 
 
 ## Get PV Output Data
 
@@ -666,15 +686,18 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.5<br>
+2.2.6<br>
+Implement 2 second delay between calls that change inverter settings.
+Added strategy mode (timed_mode=2) to charge_needed().
+Added set_strategy() and charge_strategy() to manage charging schedules and work mode changes.
 Refactor debug messaging.
 Simplify charge_needed() output.
 Added 'target_soc' to charge_needed() settings
 Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50 where there is no battery
 Fix key error when accessing cell volts and temps using an agent / installer account.
 Ensure output is generated if get_battery() fails using battery_info().
 Update f.avg() to include calculation of averages in lists containng None values.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.5 Summary: library for
+Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.6 Summary: library for
 accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
 quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
@@ -53,181 +53,189 @@
 there is more than 1 item, the call will show the list of items. To select a
 specific item to work with, call a qualifier: + Site: full or partial name of
 the site + Logger: full or partial serial number + Inverter: full or partial
 serial number When an item is selected, the functions returns a dictionary
 containing item details and saves these to a global variable (f.site, f.logger,
 f.device respectively) Once an inverter is selected, you can make other calls
 to get information: ``` f.get_generation() f.get_battery() f.get_settings()
-f.get_charge() f.get_min() f.get_schedule() ``` Each of these calls will return
-a dictionary or list containing the relevant information. get_generation() will
-return the latest generation information for the device. The results are also
-stored in f.device as 'generationToday', 'generationMonth' and
-'generationTotal'. get_battery() returns the current battery status, including
-'soc', 'volt', 'current', 'power', 'temperature' and 'residual'. The result
-also updates f.battery. get_settings() will return the battery settings and is
-equivalent to get_charge() and get_min(). The results are stored in
+f.get_charge() f.get_min() f.get_flag() f.get_schedule() ``` Each of these
+calls will return a dictionary or list containing the relevant information.
+get_generation() will return the latest generation information for the device.
+The results are also stored in f.device as 'generationToday', 'generationMonth'
+and 'generationTotal'. get_battery() returns the current battery status,
+including 'soc', 'volt', 'current', 'power', 'temperature' and 'residual'. The
+result also updates f.battery. get_settings() will return the battery settings
+and is equivalent to get_charge() and get_min(). The results are stored in
 f.battery_settings. The settings include minSoc, minSocOnGrid, enable charge
-from grid and the charge times. get_schedule() returns the current work mode /
-soc schedule settings. The result is stored in f.schedule. ## Inverter Settings
-You can change inverter settings using: ``` f.set_min(minSocOnGrid, minSoc)
+from grid and the charge times. get_flag() returns the current scheduler enable
+/ support flags get_schedule() returns the current work mode / soc schedule
+settings. The result is stored in f.schedule. ## Inverter Settings You can
+change inverter settings using: ``` f.set_min(minSocOnGrid, minSoc)
 f.set_charge(ch1, st1, en1, ch2, st2, en2) f.set_group(start, end, mode,
-min_soc, fdsoc, fdpwr) f.get_flag() f.set_schedule(enable, groups, template)
-``` set_min() applies new SoC settings to the inverter. The parameters update
-battery_settings: + minSocOnGrid: min Soc on Grid setting e.g. 15 = 15% +
-minSoc: min Soc setting e.g. 10 = 10% set_charge() takes the charge times from
-the battery_settings and applies these to the inverter. The parameters are
-optional and will update battery_settings. You should specify all 3 parameter
-for a time period: + ch1: enable charge from grid for period 1 (True or False)
-+ st1: the start time for period 1 + en1: the end time for period 1 + ch2:
-enable charge from grid for period 2 (True or False) + st2: the start time for
-period 2 + en2: the end time for period 2 set_flag() returns the current
-settings for strategy periods: 'supported' and 'enable' set_group() returns a
-time segment structure that can be used to build a list of time segments for
-set_schedule() + start, end, mode: required parameters + min_soc: optional,
-default is 10 + fdsoc: optional, default is 10. Used when setting a period with
-ForceDischarge mode + fdpwr: optional, default is 0. Used when setting a period
-with ForceDischarge mode + enable: sets whether this time segment is enable (1)
-or disabled (0). The default is enabled. set_schedule() configures a list of
-scheduled work mode / soc changes with enable=1. If called with enable=0, any
-existing schedules are disabled. To enable a schedule, you must provide a list
-of time segments + enable: 1 to enable schedules, 0 to disable schedules. The
-default is 1. + groups: a time segment or list of time segments created using
-f.set_group(). ## Real Time Data Real time data reports the latest values for
-inverter variables, collected every 5 minutes: ``` f.invert_ct2 = 1 f.get_vars
-() f.get_real(v) ``` f.invert_ct2 determines how the meterPower2 data is
-handled. When invert_ct2 = 0, meterPower2 produces +ve power values during
-secondary generation. If meterPower2 produces -ve power values during secondary
-generation, setting invert_ct2 = 1 will flip the values so they are +ve when
-generating. The default setting is 1 (invert). f.get_vars() returns the list of
-variables that can be queried. This also stores the information: + f.var_table:
-a table, indexed by variable that contains information such as the name and
-unit. ++ f.var_list: a list of all the variables that are available There are
-also pre-defined lists: + power_vars lists the main power variables provided by
-the inverter + battery_vars lists the main variables relevant to the battery /
-BMS f.get_real returns the latest values for a list of variables. + v is a
-variable, or list of variables. The default is to return the latest value for
-all available variables ## History Data History data reports inverter
-variables, collected every 5 minutes, on a given date / time and period: ```
-f.get_history(time_span, d, v, summary, save, load, plot) ``` + time_span
-determines the period covered by the data, for example, 'hour', 'day' or
-'week'. The default is 'hour' + d is a date and time in the format 'YYYY-MM-DD
-HH:MM:SS'. The default is today's date and time. d may also be a list of dates
-+ v is a variable, or list of variables (see above) + summary is optional - see
-below + save: set to the root part of a filename to save the results + load:
-set to the full filename to load previously saved results + plot is optional. 1
-plots the results with a chart per unit and per day. 2 plots multiple days on
-the same chart. Default is 0, no plots The setting for invert_ct2 is applied to
-history data for meterPower2, so +ve values are returned for secondary
-generation. f.sample_time is set to the sample time in minutes for the data
-processed, rounded to f.sample_rounding samples per minute. Data generation for
-the full list of raw_vars can be slow and return a lot of data, so it's best to
-select the vars you want from the list if you can. For example, this Jupyter
-Lab cell will load an inverter and return power data at 5 minute intervals for
-the 17th June 2023: ``` d = '2023-06-17 00:00:00' result=f.get_history('day',
-d=d, v=f.power_vars) ``` Setting the optional parameter 'summary' when calling
-get_raw() provides a summary of the raw data + summary = 0: basic history data,
-no summary + summary = 1: summary is calculated + summary = 2: summary is
-calculated and raw data is removed to save time / space + summary = 3: as (2)
-but for energy only, an hourly cumulative state is also generated, similar to
-the state used in Home Assistant long term statistics The summary includes the
-following attributes: + count: the number of data points + average: the average
-value of the data points + max: the maximum value of the data points +
-max_time: the time when the maximum value occured (HH:MM) + min: the minimum
-value of the data points + min_time: the time when the minimum value occured
-(HH:MM) For power values (unit = kW), the summary performs a Riemann sum of the
-data, integrating kW over the day to estimate energy in kWh. In this case, the
-following attributes are also added: + kwh: the total energy generated or
-consumed + kwh_off: the total energy consumed or generated during the off-peak
-time of use + kwh_peak: the total energy consumed or generated during the peak
-time of use + kwh_neg: the total energy from -ve power flow (all other totals
-are based on +ve power flow) This example shows power graphs for today and
-yesterday: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/
-d84c55c9-4f4c-431d-bc55-d7796b7e4fea) ## Report Data Report data provides
-information on the energy produced by the inverter, battery charge and
-discharge energy, grid consumption and feed-in energy and home energy
-consumption: ``` f.get_report(report_type, d, v, summary, save, load, plot,
-station) ``` + report_type sets the period covered by the report and is one of
-'day', 'week', 'month', 'year': + when 'day' is selected, energy is reported
-each hour through the day + when 'week' is selected, energy is reported for the
-7 days up to and including the date + when 'month' is selected, energy is
-reported each day through the month + when 'year' is selected, energy is
-reported each month through the year + d is a date and time in the format
-'YYYY-MM-DD HH:MM:SS'. The default is yesterday. d may also be a list of dates
-+ v is a variable, or list of variables. The default is to use report_vars +
-summary is optional - see below + save: set to the root part of a filename to
+min_soc, fdsoc, fdpwr) f.set_strategy(strategy) f.charge_strategy(st1, en1,
+st2, en2, min_soc) f.set_schedule(groups, enable) ``` set_min() applies new SoC
+settings to the inverter. The parameters update battery_settings: +
+minSocOnGrid: min Soc on Grid setting e.g. 15 = 15% + minSoc: min Soc setting
+e.g. 10 = 10% set_charge() takes the charge times from the battery_settings and
+applies these to the inverter. The parameters are optional and will update
+battery_settings. You should specify all 3 parameter for a time period: + ch1:
+enable charge from grid for period 1 (True or False) + st1: the start time for
+period 1 + en1: the end time for period 1 + ch2: enable charge from grid for
+period 2 (True or False) + st2: the start time for period 2 + en2: the end time
+for period 2 set_group() returns a time segment structure that can be used to
+build a list of time segments for set_schedule() + start, end, mode: required
+parameters. end time is exclusive e.g. end at '07:00' will set a period end
+time of '06:59' + min_soc: optional, default is 10 + fdsoc: optional, default
+is 10. Used when setting a period with ForceDischarge mode + fdpwr: optional,
+default is 0. Used when setting a period with ForceDischarge mode + enable:
+sets whether this time segment is enable (1) or disabled (0). The default is
+enabled. set_strategy() creates a list of groups from the strategy. If strategy
+is not provided, it uses the strategy for the current tariff. charge_strategy
+(): returns a list of groups that describe the strategy for the current tariff
+and adds the groupd required for charging: + st1: the start time for the period
+when the battery charges from the grid + en1: the end time for period 1 + st2:
+the start time for period when the battery is held at min_soc + en2: the end
+time for period 2 + min_soc: the min_soc to use after the charge period, when
+you don't want the battery to discharge below this level set_schedule()
+configures a list of scheduled work mode / soc changes with enable=1. If called
+with enable=0, any existing schedules are disabled. To enable a schedule, you
+must provide a list of time segments + groups: a time segment or list of time
+segments created using f.set_group(). + enable: 1 to enable schedules, 0 to
+disable schedules. The default is 1. ## Real Time Data Real time data reports
+the latest values for inverter variables, collected every 5 minutes: ```
+f.invert_ct2 = 1 f.get_vars() f.get_real(v) ``` f.invert_ct2 determines how the
+meterPower2 data is handled. When invert_ct2 = 0, meterPower2 produces +ve
+power values during secondary generation. If meterPower2 produces -ve power
+values during secondary generation, setting invert_ct2 = 1 will flip the values
+so they are +ve when generating. The default setting is 1 (invert). f.get_vars
+() returns the list of variables that can be queried. This also stores the
+information: + f.var_table: a table, indexed by variable that contains
+information such as the name and unit. ++ f.var_list: a list of all the
+variables that are available There are also pre-defined lists: + power_vars
+lists the main power variables provided by the inverter + battery_vars lists
+the main variables relevant to the battery / BMS f.get_real returns the latest
+values for a list of variables. + v is a variable, or list of variables. The
+default is to return the latest value for all available variables ## History
+Data History data reports inverter variables, collected every 5 minutes, on a
+given date / time and period: ``` f.get_history(time_span, d, v, summary, save,
+load, plot) ``` + time_span determines the period covered by the data, for
+example, 'hour', 'day' or 'week'. The default is 'hour' + d is a date and time
+in the format 'YYYY-MM-DD HH:MM:SS'. The default is today's date and time. d
+may also be a list of dates + v is a variable, or list of variables (see above)
++ summary is optional - see below + save: set to the root part of a filename to
 save the results + load: set to the full filename to load previously saved
-results + plot is optional. 1 to plot results + station is optional. 1 gets
-data for a site (using f.station_id), 0 gets data for a device (using
-f.device_id). The default is 0. The list of variables that can be reported on
-is stored in f.report_vars. Note that reporting by 'day' produces inaccurate
-hourly data, where the sum does not reconcile with the daily total given in the
-monthly report. To correct this, reporting by day also gets the monthly data
-and uses the daily total to correctly report the total. Setting the optional
-parameter 'summary' when calling get_report() provides a summary of the report
-data: + summary = 0: basic report data, no summary. report_type cannot be
-'week' + summary = 1: summary is calculated + summary = 2: corrected total only
-is reported to save time / space. report_type must be 'day' The result data for
-each variable includes the following attributes when summary=2 + 'variable':
-name of the data set + 'total': corrected total of the data items When
-summary=1, the following items are also added: + 'data': 'index' and 'value' of
-each data point + 'date': that was used to produce the report + 'count': the
-number of data items + 'sum': the sum of the data items + 'max': the biggest
-value in 'data' + 'max_index': the index of the biggest value in 'data' +
-'min': the smallest value in 'data' + 'min_index': the index of the smallest
-value in 'data' + 'average': corrected average of the data items For example,
-this Jupyter Lab cell will report energy data by day for the month of June
-2023: ``` d = '2023-06-17' result=f.get_report('month', d=d) ``` This example
-plots weekly data: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
-63789168/f408a010-9600-4b2f-979f-83e32d960586) # Built-in Utilities and
-Operations The previous section provides functions that can be used to access
-and control your inverter. This section covers utilities and operations that
-build upon these functions. ## Charge Needed Uses forecast PV yield for
-tomorrow to work out if charging from grid is needed tonight to deliver the
-expected consumption for tomorrow. If charging is needed, the charge times are
-configured. If charging is not needed, the charge times are cleared. The
-results are sent to the inverter. ``` f.charge_needed(forecast, force_charge,
-forecast_selection, forecast_times, update_setings, show_data, show_plot) ```
-All the parameters are optional: + forecast: the kWh expected tomorrow
-(optional, see below) + force_charge: 1 any remaining time in a charge period
-has force charge set, 2 charging uses the entire charge period, 0 None
-(default) + forecast_selection: if set to 1, settings are only updated if there
-is a forecast. Default is 0, generation is used when forecasts are not
-available + forecast_times: a list of hours when forecasts can be obtained. By
-default, the forecast times for the selected tariff are used (see below) +
-update_settings: 0 no changes, 1 update charge time, 2 update work mode, 3
-update charge time and work mode. The default is 0 + show_data: 1 show battery
-SoC data, 2 show battery Residual data, 3 show timed data, 4 show timed data
-before and after charging. The default is 1. + show_plot: 1 plot battery SoC
-data. 2 plot battery Residual, Generation and Consumption. 3 plot 2 + Charge
-and Discharge The default is 3 ### Modelling charge_needed() uses a number of
-models to better estimate the state of the battery. **Manual Consumption:** You
-can provide your 'annual_consumption' in kWh e.g. 5500. This figure is factored
-down to a daily consumption by dividing by 365 and applying **f.seasonality**.
-This normally decreases consumption in the summer and increases it in winter.
-Seasonality is a list of weightings by month for Jan, Feb, Mar, Apr etc. Preset
-lists are 'f.high_seasonality' (recommend where electric heating is ued),
-'f.medium_seasonality' (default) amd 'f.no_seasonality' (all months the same).
-The daily consumption is profiled by hour using **f.daily_consumption**. This
-maps your consumption for a day to the hours when more or less energy is
-consumed. It is a list of 24 values for the times 00, 01, 02, 03 .. 23. Preset
-lists are 'f.high_profile' (larger peaks at 8am and 6pm), 'f.medium_profile'
-(default, more balanced) and 'f.no_profile' (flat). **Historic Consumption:**
-If annual_consumption is not provided, your consumption history is used. By
-default, this looks at your average consumption for the last 3 days using the
-load power reported by your inverter. For systems with multiple inverters where
-CT2 is not connected, the load power may not be correct. For this and other
-cases where you want to set your consumption, provide your annual_consumption.
-**Manual Forecast:** You can provide a specific 'forecast' in kWh e.g. 20. This
-is profiled using **f.seasonal_sun** to map solar generation to the time of
-day. The mapping is broken down into 4 seasons: winter, spring, summer and
-autumn (winter is Dec, Jan, Feb, spring is Mar, Apr, May etc). There are 4
-preset lists: 'f.winter_sun', 'f.spring_sun', 'f.summer_sun' and
-'f.autumn_sun'. Seasonal_sun is used for manual and historic forecasts
-**Solcast:** If you provide an API key for Solcast, your forecast will be
-downloaded after 9pm each day and used as the basis for your next days
+results + plot is optional. 1 plots the results with a chart per unit and per
+day. 2 plots multiple days on the same chart. Default is 0, no plots The
+setting for invert_ct2 is applied to history data for meterPower2, so +ve
+values are returned for secondary generation. f.sample_time is set to the
+sample time in minutes for the data processed, rounded to f.sample_rounding
+samples per minute. Data generation for the full list of raw_vars can be slow
+and return a lot of data, so it's best to select the vars you want from the
+list if you can. For example, this Jupyter Lab cell will load an inverter and
+return power data at 5 minute intervals for the 17th June 2023: ``` d = '2023-
+06-17 00:00:00' result=f.get_history('day', d=d, v=f.power_vars) ``` Setting
+the optional parameter 'summary' when calling get_raw() provides a summary of
+the raw data + summary = 0: basic history data, no summary + summary = 1:
+summary is calculated + summary = 2: summary is calculated and raw data is
+removed to save time / space + summary = 3: as (2) but for energy only, an
+hourly cumulative state is also generated, similar to the state used in Home
+Assistant long term statistics The summary includes the following attributes: +
+count: the number of data points + average: the average value of the data
+points + max: the maximum value of the data points + max_time: the time when
+the maximum value occured (HH:MM) + min: the minimum value of the data points +
+min_time: the time when the minimum value occured (HH:MM) For power values
+(unit = kW), the summary performs a Riemann sum of the data, integrating kW
+over the day to estimate energy in kWh. In this case, the following attributes
+are also added: + kwh: the total energy generated or consumed + kwh_off: the
+total energy consumed or generated during the off-peak time of use + kwh_peak:
+the total energy consumed or generated during the peak time of use + kwh_neg:
+the total energy from -ve power flow (all other totals are based on +ve power
+flow) This example shows power graphs for today and yesterday: ![image](https:/
+/github.com/TonyM1958/FoxESS-Cloud/assets/63789168/d84c55c9-4f4c-431d-bc55-
+d7796b7e4fea) ## Report Data Report data provides information on the energy
+produced by the inverter, battery charge and discharge energy, grid consumption
+and feed-in energy and home energy consumption: ``` f.get_report(report_type,
+d, v, summary, save, load, plot, station) ``` + report_type sets the period
+covered by the report and is one of 'day', 'week', 'month', 'year': + when
+'day' is selected, energy is reported each hour through the day + when 'week'
+is selected, energy is reported for the 7 days up to and including the date +
+when 'month' is selected, energy is reported each day through the month + when
+'year' is selected, energy is reported each month through the year + d is a
+date and time in the format 'YYYY-MM-DD HH:MM:SS'. The default is yesterday. d
+may also be a list of dates + v is a variable, or list of variables. The
+default is to use report_vars + summary is optional - see below + save: set to
+the root part of a filename to save the results + load: set to the full
+filename to load previously saved results + plot is optional. 1 to plot results
++ station is optional. 1 gets data for a site (using f.station_id), 0 gets data
+for a device (using f.device_id). The default is 0. The list of variables that
+can be reported on is stored in f.report_vars. Note that reporting by 'day'
+produces inaccurate hourly data, where the sum does not reconcile with the
+daily total given in the monthly report. To correct this, reporting by day also
+gets the monthly data and uses the daily total to correctly report the total.
+Setting the optional parameter 'summary' when calling get_report() provides a
+summary of the report data: + summary = 0: basic report data, no summary.
+report_type cannot be 'week' + summary = 1: summary is calculated + summary =
+2: corrected total only is reported to save time / space. report_type must be
+'day' The result data for each variable includes the following attributes when
+summary=2 + 'variable': name of the data set + 'total': corrected total of the
+data items When summary=1, the following items are also added: + 'data':
+'index' and 'value' of each data point + 'date': that was used to produce the
+report + 'count': the number of data items + 'sum': the sum of the data items +
+'max': the biggest value in 'data' + 'max_index': the index of the biggest
+value in 'data' + 'min': the smallest value in 'data' + 'min_index': the index
+of the smallest value in 'data' + 'average': corrected average of the data
+items For example, this Jupyter Lab cell will report energy data by day for the
+month of June 2023: ``` d = '2023-06-17' result=f.get_report('month', d=d) ```
+This example plots weekly data: ![image](https://github.com/TonyM1958/FoxESS-
+Cloud/assets/63789168/f408a010-9600-4b2f-979f-83e32d960586) # Built-in
+Utilities and Operations The previous section provides functions that can be
+used to access and control your inverter. This section covers utilities and
+operations that build upon these functions. ## Charge Needed Uses forecast PV
+yield for tomorrow to work out if charging from grid is needed tonight to
+deliver the expected consumption for tomorrow. If charging is needed, the
+charge times are configured. If charging is not needed, the charge times are
+cleared. The results are sent to the inverter. ``` f.charge_needed(forecast,
+force_charge, forecast_selection, forecast_times, update_setings, show_data,
+show_plot) ``` All the parameters are optional: + forecast: the kWh expected
+tomorrow (optional, see below) + force_charge: 1 any remaining time in a charge
+period has force charge / min_soc set, 2 charging uses the entire charge
+period, 0 None (default) + forecast_selection: if set to 1, settings are only
+updated if there is a forecast. Default is 0, generation is used when forecasts
+are not available + forecast_times: a list of hours when forecasts can be
+obtained. By default, the forecast times for the selected tariff are used (see
+below) + update_settings: 0 no changes, 1 update charge settings. The default
+is 0 + show_data: 1 show battery SoC data, 2 show battery Residual data, 3 show
+timed data, 4 show timed data before and after charging. The default is 1. +
+show_plot: 1 plot battery SoC data. 2 plot battery Residual, Generation and
+Consumption. 3 plot 2 + Charge and Discharge The default is 3 ### Modelling
+charge_needed() uses a number of models to better estimate the state of the
+battery. **Manual Consumption:** You can provide your 'annual_consumption' in
+kWh e.g. 5500. This figure is factored down to a daily consumption by dividing
+by 365 and applying **f.seasonality**. This normally decreases consumption in
+the summer and increases it in winter. Seasonality is a list of weightings by
+month for Jan, Feb, Mar, Apr etc. Preset lists are 'f.high_seasonality'
+(recommend where electric heating is ued), 'f.medium_seasonality' (default) amd
+'f.no_seasonality' (all months the same). The daily consumption is profiled by
+hour using **f.daily_consumption**. This maps your consumption for a day to the
+hours when more or less energy is consumed. It is a list of 24 values for the
+times 00, 01, 02, 03 .. 23. Preset lists are 'f.high_profile' (larger peaks at
+8am and 6pm), 'f.medium_profile' (default, more balanced) and 'f.no_profile'
+(flat). **Historic Consumption:** If annual_consumption is not provided, your
+consumption history is used. By default, this looks at your average consumption
+for the last 3 days using the load power reported by your inverter. For systems
+with multiple inverters where CT2 is not connected, the load power may not be
+correct. For this and other cases where you want to set your consumption,
+provide your annual_consumption. **Manual Forecast:** You can provide a
+specific 'forecast' in kWh e.g. 20. This is profiled using **f.seasonal_sun**
+to map solar generation to the time of day. The mapping is broken down into 4
+seasons: winter, spring, summer and autumn (winter is Dec, Jan, Feb, spring is
+Mar, Apr, May etc). There are 4 preset lists: 'f.winter_sun', 'f.spring_sun',
+'f.summer_sun' and 'f.autumn_sun'. Seasonal_sun is used for manual and historic
+forecasts **Solcast:** If you provide an API key for Solcast, your forecast
+will be downloaded after 9pm each day and used as the basis for your next days
 generation (see below). **Solar:** if you configure one or more
 **f.solar_array**, forecast.solar will be called to provide a forrecast for
 your next days generation (see below). **Historic Generation:** If 'forecast'
 is not provided and Solcast and Solar forecasts are not available, your
 generation history is used. By default, this looks at your average solar
 generation for the last 3 days and applies the **f.seasonal_sun** profile.
 Note: if using Solcast or forecast.solar, calls to the API are very limited so
@@ -264,50 +272,54 @@
 e.g. Saturdays use_today: 21.0 # hour when today's generation and consumption
 data will be used min_hours: 0.25 # minimum charge time to set (in decimal
 hours) min_kwh: 0.5 # minimum charge to add in kwh solcast_adjust: 100 # %
 adjustment to make to Solcast forecast solar_adjust: 100 # % adjustment to make
 to Solar forecast forecast_selection: 1 # 1 = only update charge times if
 forecast is available, 0 = use best available data. Default is 1.
 annual_consumption: None # optional annual consumption in kWh. If set, this
-replaces consumption history timed_mode: 0 # 1 = apply timed work mode, 0 =
-None special_contingency: 30 # contingency for special days when consumption
-might be higher special_days: ['12-25', '12-26', '01-01'] full_charge: None #
-day of month (1-28) to do full charge or 'daily' or day of week: 'Mon', 'Tue'
-etc derate_temp: 21 # battery temperature in C when derating charge current is
-applied derate_step: 5 # step size for derating e.g. 21, 16, 11 derating: [24,
-15, 10, 2] # derated charge current for each temperature step e.g. 21C, 16C,
-11C, 6C force: 1 # 1 = disable strategy periods when setting charge. 0 = fail
-if strategy period has been set. data_wrap: 6 # data items to show per line
-target_soc: None # target soc for charging ``` These values are stored /
-available in f.charge_config. The default battery open circuit voltage curve
-versus SoC from 0% to 100% is: ``` lifepo4_curve = [51.30, 52.00, 52.30, 52.40,
-52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ``` This example shows the
-results reported by charge needed: ![image](https://github.com/TonyM1958/
-FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-b165-20d806b1e7e8) ## Battery
-Info Provides detailed information on the current state of the batteries: ```
-f.battery_info(count, plot, log) f.battery_monitor(interval, run, log, save,
-count) ``` battery_info() prints information on the battery and cells: + count:
-optional over-ride. The default is based on factorising the number of cells
-reported by 16 or 18 to work out the number of batteries. + plot: 1 plot the
-cell voltages for each battery, 2 plot the cell temperatueres, 0 don't plot.
-The default is 1 + log: see below. Default is 0 battery_monitor() runs
-battery_info() in log mode on a schedule to provide information on the battery
-status over a period of time: + interval: the time in minutes between log
-entries. The default is 30 minutes + run: the number of log entries to create.
-The default is 48 i.e. every 30 minues for 24 hours in total + log: 0 =
-display, 1 = log battery info, 2 = add cell volts, 3 = add cell temps. The
-default is 1 + save: name of a CSV file to write log data to + count: optional
-over-ride for the number of batteries This is an example of the output from
-battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
-63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ``` f.date_list
-(s, e, limit, span, today) ``` Returns a list of dates in the format 'YYYY-MM-
-DD'. This function will not return dates in the future. The last date will be
-yesterday or today (if today is True). All parameters are optional: + s: start
-date + e: end date + limit: maximum number of days. The default is 200 + span:
-the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
+replaces consumption history timed_mode: 0 # 0 = None, 1 = use timed work mode,
+2 = strategy mode special_contingency: 30 # contingency for special days when
+consumption might be higher special_days: ['12-25', '12-26', '01-01']
+full_charge: None # day of month (1-28) to do full charge or 'daily' or day of
+week: 'Mon', 'Tue' etc derate_temp: 21 # battery temperature in C when derating
+charge current is applied derate_step: 5 # step size for derating e.g. 21, 16,
+11 derating: [24, 15, 10, 2] # derated charge current for each temperature step
+e.g. 21C, 16C, 11C, 6C force: 1 # 1 = disable strategy periods when setting
+charge. 0 = fail if strategy period has been set. data_wrap: 6 # data items to
+show per line target_soc: None # target soc for charging ``` These values are
+stored / available in f.charge_config. The default battery open circuit voltage
+curve versus SoC from 0% to 100% is: ``` lifepo4_curve = [51.30, 52.00, 52.30,
+52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ``` When operating in
+strategy mode (timed_mode=2), charge_needed will create a schedule that
+includes the strategy for the tariff with additional time segments added to
+charge from grid and (optionall) to stop the battery discharging. In other
+modes, charge_needed() will disable any schedules and set the battery charge
+times. This example shows the results reported by charge needed: ![image]
+(https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-
+b165-20d806b1e7e8) ## Battery Info Provides detailed information on the current
+state of the batteries: ``` f.battery_info(count, plot, log) f.battery_monitor
+(interval, run, log, save, count) ``` battery_info() prints information on the
+battery and cells: + count: optional over-ride. The default is based on
+factorising the number of cells reported by 16 or 18 to work out the number of
+batteries. + plot: 1 plot the cell voltages for each battery, 2 plot the cell
+temperatueres, 0 don't plot. The default is 1 + log: see below. Default is 0
+battery_monitor() runs battery_info() in log mode on a schedule to provide
+information on the battery status over a period of time: + interval: the time
+in minutes between log entries. The default is 30 minutes + run: the number of
+log entries to create. The default is 48 i.e. every 30 minues for 24 hours in
+total + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add
+cell temps. The default is 1 + save: name of a CSV file to write log data to +
+count: optional over-ride for the number of batteries This is an example of the
+output from battery_info(): ![image](https://github.com/TonyM1958/FoxESS-Cloud/
+assets/63789168/a8eb52b6-ce3f-4b58-bb76-5483d5e40fa7) ## Date Ranges ```
+f.date_list(s, e, limit, span, today) ``` Returns a list of dates in the format
+'YYYY-MM-DD'. This function will not return dates in the future. The last date
+will be yesterday or today (if today is True). All parameters are optional: +
+s: start date + e: end date + limit: maximum number of days. The default is 200
++ span: the range of dates. One of 'day', 'week', 'month' or 'year', '2days' or
 'weekday' + today: 1 allows today to be included, 2 allows future dates to be
 included. Default is 0, date list will stop at yesterday You can use 'span' as
 follows: + 'day' provides a single day + 'week' will provide the dates of 7
 consequetive days + 'month' will provide the dates of the days up to the same
 date in the preceeding (or follwing) month + '2days' will provide the dates of
 yesterday and today + 'weekday' will provide the dates of the same day of the
 week, going backwards (or forwards) up to 7 weeks ``` f.british_summer_time(d)
@@ -334,145 +346,156 @@
 to 23:59 + Eco 7: Economy 7: off-peak from 00:30 to 07:30 GMT (01:30 to 08:30
 during BST) Custom periods can be configured for specific times if required: +
 Custom: charging from 02:00 to 05:00, no off-peak or peak times, forecasts from
 22:00 to 23:59 The active tariff is configured by calling 'f.set_tariff() with
 the name of the tariff to use: ``` f.set_tariff('flux') ``` When Agile Octopus
 is selected, a price based charging period is configured using the 30 minute
 price forecast. For example: ``` f.set_tariff('agile', product, region,
-start_at, end_by, duration, times, forecast_times, work_times, update,
-weighting, time_shift) ``` This gets the latest 30 minute pricing and uses this
-to work out the best off peak charging period. + product: optional Agile
-Octopus product code (see below). The default is "AGILE-FLEX-22-11-25" +
-region: optional region to use for prices (se below). The default is 'H'
-(Southern England) + start_at: optional earliest start time for charge period
-in hours, the default is 23:00 + end_by: optional latest end time for charge
-period in hours, the default is 08:00 + duration: optional charge time period
-in hours, the default is 3 hours. Valid range is 1-6 hours + times: a list of
-charge periods that can be used instead of start_at, end_by and duration (see
-below) + forecast_times: a list of times when a forecast can be obtained from
-Solcast / forecast.solar + work_times: a list of work modes and times when
-these are set. The format is [(mode, start, end),...] + update: optional, 1
-(the default) sets the current tariff to Agile Octopus. Setting to 0 does not
-change the current tariff + weighting: optional, default is None (see below) +
-time_shift: optional system time shift in hours. The default is for system time
-to be UTC and to apply the current day light saving time (e.g. GMT/BST) Product
-codes include: + 'AGILE-18-02-21' = The original version capped at 35p per unit
-+ 'AGILE-22-07-22' = The cap rose to 55p + 'AGILE-22-08-31' = The cap was
-increased to 78p + 'AGILE-VAR-22-10-19' = This version raised the cap to Â£1
-per unit and also introduced a new formula. + 'AGILE-FLEX-22-11-25' = Cap stays
-at Â£1 per unit but new formula only deducts 17.9p from higher unit prices
-(default) Region codes include: + 'A' = Eastern England + 'B' = East Midlands +
-'C' = London + 'D' = Merseyside and Northern Wales + 'E' = West Midlands + 'F'
-= North Eastern England + 'G' = North Western England + 'H' = Southern England
-(default) + 'J' = South Eastern England + 'K' = Southern Wales + 'L' = South
-Western England + 'M' = Yorkshire + 'N' = Southern Scotland + 'P' = Northern
-Scotland Pricing for tomorrow is updated around 4pm each day. If run before
-this time, prices from yesterday are used. By default, prices for tomorrow are
-fetched after 5pm. The setting for this is: + f.agile_update_time = 17 The best
-charging period is determined based on the weighted average of the 30 minute
-prices over the duration. The default is flat (all prices are weighted
-equally). You can change the weighting by providing 'weighting'. The following
-preset weightings are provided: + f.front_loaded: [1.0, 0.9, 0.8, 0.7, 0.6,
-0.5] + f.first_hour: [1.0, 1.0] Specifying start_at, end_by and duration allows
-either the AM or PM charging slot for any tariif to be updated, depending on
-the time. Agile periods will be calculated; othe rtariffs will use the start
-and end times directly. By default, set_tariff() updates the AM charge period
-if start_at is after 9pm and end_by is before 8am; it updates the PM charge
-period if start_at is after 8am and the end_by is before 9pm. Only the relevant
-AM or PM charge time is updated e.g. if you configure a PM charging period, the
-AM charginig period is not changed. To disable a charging period, set
-duration=0. set_tariff() can configure multiple charging periods for any tariff
-using the times parameter instead of start_at, end_by and duration. Times is a
-list of tuples containing values for start_at, end_by and duration. For
-example, this parameter configures an AM charging period between 11pm and 8am
-with a 3 hour period and a PM charging period between 12 noon and 4pm with a 1
-hour period: + times=[("23:00", "8:00", 3), ("12:00", "16:00", 1)] # PV Output
-These functions produce CSV data for upload to [pvoutput.org](https://
-pvoutput.org) including PV generation, Export, Load and Grid consumption by day
-in Wh. The functions use the energy estimates created from the raw power data
-(see above). The estimates include PV energy generation that are not otherwise
-available from the Fox Cloud. Typically, the energy results are within 3% of
-the values reported by the meters built into the inverter. ## Get PV Output
-Data Returns CSV upload data using the [API format](https://pvoutput.org/help/
-api_specification.html#csv-data-parameter): ``` f.get_pvoutput(d, tou) ``` + d
-is the date or a list of dates, to get data for. The default is yesterday +
-tou: optional, setting tou=1 uploads data with time of use. The default, tou=0
-does not split data and is more accurate. You can copy and paste the output
-data to the pvoutput data CSV Loader, using the following settings: ![image]
-(https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/21459cdc-a943-4e9d-
-a204-7efd45a422d8) For example, this Jupyer Lab cell will provide a CSV data
-upload for June 2023: ``` f.get_pvoutput(f.date_list('2023-06-01', '2023-06-
-30')) ``` ## Set PV Output Data Loads CSV data directly using the PV Ouput API:
-``` f.set_pvoutput(d, system_id, tou, push) ``` + d is optional and is the
-date, or a list of dates, to upload + system_id is optional and allow you to
-select where data is uploaded to (where you have more than 1 registered system)
-+ tou: optional, setting tou=1 uploads data with time of use. The default,
-tou=0 does not split data and is more accurate + push: optional. 0 = do not
-sent to pushover, 1 = send summary to pushover, 2 = send first day summary only
-# Solar Forecasting # Solcast Get and display solar data from your solcast.com
-account using your API key: ``` f.solcast_api_key = "my.solcast_api_key" fcast
-= f.Solcast() print(fcast) ``` Returns a 7 day forecast. Optional parameters
-are: + days: number of days to get. The default is 7 + estimated: whether to
-get history / estimated data. 1 = yes, 0 = no. Default is 0. + reload: cached
-data handling. 0 = use saved data, 1 = fetch new data, 2 = use saved data for
-today (default) + quiet: True to stop Solcast producing progress messages
-Forecast data is saved to f.solcast_save. The default is 'solcast.txt'. ```
-fcast.plot_daily() fcast.plot_hourly(day) ``` Plots the estimate / forecast
-data. plot_daily() plots the daily yield. plot_hourly() plots each day
-separately. + day: optional. 'today', 'tomorrow', 'all' or a specific list of
-dates. The default is to plot today and tomorrow # Forecast.solar Get and
-display solar data from forecast.solar for today and tomorrow: ```
-f.solar_array('South', lat=51.1789, lon=-1.8262, kwp=6.4) ``` You need to
-configure your solar arrays by calling f.solar_array(). This takes the
-following parameters: + name: the name of each of your arrays + lat: the
-latitude where the array is located. The default is Stonehenge. + lon: the
-longitude where the array is located. The default is Stonehenge. + dec: the
-declination of the array - 0 is lying flat and 90 is vertical. Default is 30 +
-az: azimuth of the array. 0 is pointing due South, -90 is pointing East, 90 is
-pointing West. The default is 0 + kwp: the size of the array in kWp. The
-default is 5kWp + dam: damping factor. Default is None + inv: inverter power
-limit (when the array will clip). The default is None + hor: a list of values
-describing obstructions on the horizon Add one array for each string attached
-to your inverter. If your solar production is limited by clipping, set the
-inverter power so the forecast better matches your generation. See the [API
-documentation](https://doc.forecast.solar/api) for more information on
-parameter values. ``` fcast = f.Solar() print(fcast) ``` Returns a forecast for
-today and tomorrow. Optional parameters are: + reload: cached data handling. 0
-= use saved data, 1 = fetch new data, 2 = use saved data for today (default) +
-quiet: set to True to stop Solar producing progress messages Forecast data is
-saved to f.solar_save. The default is 'solar.txt'. ``` fcast.plot_daily()
+start_at, end_by, duration, times, forecast_times, strategy, update, weighting,
+time_shift) ``` This gets the latest 30 minute pricing and uses this to work
+out the best off peak charging period. + product: optional Agile Octopus
+product code (see below). The default is "AGILE-FLEX-22-11-25" + region:
+optional region to use for prices (se below). The default is 'H' (Southern
+England) + start_at: optional earliest start time for charge period in hours,
+the default is 23:00 + end_by: optional latest end time for charge period in
+hours, the default is 08:00 + duration: optional charge time period in hours,
+the default is 3 hours. Valid range is 1-6 hours + times: a list of charge
+periods that can be used instead of start_at, end_by and duration (see below) +
+forecast_times: a list of times when a forecast can be obtained from Solcast /
+forecast.solar + strategy: an optional list of times and work modes (see below)
++ update: optional, 1 (the default) sets the current tariff to Agile Octopus.
+Setting to 0 does not change the current tariff + weighting: optional, default
+is None (see below) + time_shift: optional system time shift in hours. The
+default is for system time to be UTC and to apply the current day light saving
+time (e.g. GMT/BST) Product codes include: + 'AGILE-18-02-21' = The original
+version capped at 35p per unit + 'AGILE-22-07-22' = The cap rose to 55p +
+'AGILE-22-08-31' = The cap was increased to 78p + 'AGILE-VAR-22-10-19' = This
+version raised the cap to Â£1 per unit and also introduced a new formula. +
+'AGILE-FLEX-22-11-25' = Cap stays at Â£1 per unit but new formula only deducts
+17.9p from higher unit prices (default) Region codes include: + 'A' = Eastern
+England + 'B' = East Midlands + 'C' = London + 'D' = Merseyside and Northern
+Wales + 'E' = West Midlands + 'F' = North Eastern England + 'G' = North Western
+England + 'H' = Southern England (default) + 'J' = South Eastern England + 'K'
+= Southern Wales + 'L' = South Western England + 'M' = Yorkshire + 'N' =
+Southern Scotland + 'P' = Northern Scotland Pricing for tomorrow is updated
+around 4pm each day. If run before this time, prices from yesterday are used.
+By default, prices for tomorrow are fetched after 5pm. The setting for this is:
++ f.agile_update_time = 17 The best charging period is determined based on the
+weighted average of the 30 minute prices over the duration. The default is flat
+(all prices are weighted equally). You can change the weighting by providing
+'weighting'. The following preset weightings are provided: + f.front_loaded:
+[1.0, 0.9, 0.8, 0.7, 0.6, 0.5] + f.first_hour: [1.0, 1.0] Specifying start_at,
+end_by and duration allows either the AM or PM charging slot for any tariif to
+be updated, depending on the time. Agile periods will be calculated; othe
+rtariffs will use the start and end times directly. By default, set_tariff()
+updates the AM charge period if start_at is after 9pm and end_by is before 8am;
+it updates the PM charge period if start_at is after 8am and the end_by is
+before 9pm. Only the relevant AM or PM charge time is updated e.g. if you
+configure a PM charging period, the AM charginig period is not changed. To
+disable a charging period, set duration=0. set_tariff() can configure multiple
+charging periods for any tariff using the times parameter instead of start_at,
+end_by and duration. Times is a list of tuples containing values for start_at,
+end_by and duration. For example, this parameter configures an AM charging
+period between 11pm and 8am with a 3 hour period and a PM charging period
+between 12 noon and 4pm with a 1 hour period: + times=[("23:00", "8:00", 3),
+("12:00", "16:00", 1)] 'strategy' allows you to configure times when work modes
+will be changed. The format is a list of dictionary items, containing: +
+'start', 'end': times in decimal hours or time format. The end time is
+exclusive so setting an end time of '07:00' will set a schedule that ends at
+'06:59' + 'mode': the work mode to be used from 'SelfUse', 'Feedin', 'Backup',
+'ForceCharge', 'ForceDischarge' + 'min_soc, 'fdsoc', 'fdpwr': optional values
+for each work mode. The defaults are 10, 10 and 0 respectively. The strategy
+should not include settings for the AM/PM charge times for the tariff. These
+will be added by charge_needed(). # PV Output These functions produce CSV data
+for upload to [pvoutput.org](https://pvoutput.org) including PV generation,
+Export, Load and Grid consumption by day in Wh. The functions use the energy
+estimates created from the raw power data (see above). The estimates include PV
+energy generation that are not otherwise available from the Fox Cloud.
+Typically, the energy results are within 3% of the values reported by the
+meters built into the inverter. ## Get PV Output Data Returns CSV upload data
+using the [API format](https://pvoutput.org/help/api_specification.html#csv-
+data-parameter): ``` f.get_pvoutput(d, tou) ``` + d is the date or a list of
+dates, to get data for. The default is yesterday + tou: optional, setting tou=1
+uploads data with time of use. The default, tou=0 does not split data and is
+more accurate. You can copy and paste the output data to the pvoutput data CSV
+Loader, using the following settings: ![image](https://github.com/TonyM1958/
+FoxESS-Cloud/assets/63789168/21459cdc-a943-4e9d-a204-7efd45a422d8) For example,
+this Jupyer Lab cell will provide a CSV data upload for June 2023: ```
+f.get_pvoutput(f.date_list('2023-06-01', '2023-06-30')) ``` ## Set PV Output
+Data Loads CSV data directly using the PV Ouput API: ``` f.set_pvoutput(d,
+system_id, tou, push) ``` + d is optional and is the date, or a list of dates,
+to upload + system_id is optional and allow you to select where data is
+uploaded to (where you have more than 1 registered system) + tou: optional,
+setting tou=1 uploads data with time of use. The default, tou=0 does not split
+data and is more accurate + push: optional. 0 = do not sent to pushover, 1 =
+send summary to pushover, 2 = send first day summary only # Solar Forecasting #
+Solcast Get and display solar data from your solcast.com account using your API
+key: ``` f.solcast_api_key = "my.solcast_api_key" fcast = f.Solcast() print
+(fcast) ``` Returns a 7 day forecast. Optional parameters are: + days: number
+of days to get. The default is 7 + estimated: whether to get history /
+estimated data. 1 = yes, 0 = no. Default is 0. + reload: cached data handling.
+0 = use saved data, 1 = fetch new data, 2 = use saved data for today (default)
++ quiet: True to stop Solcast producing progress messages Forecast data is
+saved to f.solcast_save. The default is 'solcast.txt'. ``` fcast.plot_daily()
 fcast.plot_hourly(day) ``` Plots the estimate / forecast data. plot_daily()
 plots the daily yield. plot_hourly() plots each day separately. + day:
 optional. 'today', 'tomorrow', 'all' or a specific list of dates. The default
-is to plot today and tomorrow # Pushover Send messages to a pushover user
-account: ``` f.output_spool(app_key, h) f.output(s) f.output_close(plot, file)
-f.output_message(app_key, message, plot) ``` Calling f.output_spool() with an
-app key will start the system spooling output to send to pushover. h is an
-optional header to add as the first line of the message. H may include \
+is to plot today and tomorrow # Forecast.solar Get and display solar data from
+forecast.solar for today and tomorrow: ``` f.solar_array('South', lat=51.1789,
+lon=-1.8262, kwp=6.4) ``` You need to configure your solar arrays by calling
+f.solar_array(). This takes the following parameters: + name: the name of each
+of your arrays + lat: the latitude where the array is located. The default is
+Stonehenge. + lon: the longitude where the array is located. The default is
+Stonehenge. + dec: the declination of the array - 0 is lying flat and 90 is
+vertical. Default is 30 + az: azimuth of the array. 0 is pointing due South, -
+90 is pointing East, 90 is pointing West. The default is 0 + kwp: the size of
+the array in kWp. The default is 5kWp + dam: damping factor. Default is None +
+inv: inverter power limit (when the array will clip). The default is None +
+hor: a list of values describing obstructions on the horizon Add one array for
+each string attached to your inverter. If your solar production is limited by
+clipping, set the inverter power so the forecast better matches your
+generation. See the [API documentation](https://doc.forecast.solar/api) for
+more information on parameter values. ``` fcast = f.Solar() print(fcast) ```
+Returns a forecast for today and tomorrow. Optional parameters are: + reload:
+cached data handling. 0 = use saved data, 1 = fetch new data, 2 = use saved
+data for today (default) + quiet: set to True to stop Solar producing progress
+messages Forecast data is saved to f.solar_save. The default is 'solar.txt'.
+``` fcast.plot_daily() fcast.plot_hourly(day) ``` Plots the estimate / forecast
+data. plot_daily() plots the daily yield. plot_hourly() plots each day
+separately. + day: optional. 'today', 'tomorrow', 'all' or a specific list of
+dates. The default is to plot today and tomorrow # Pushover Send messages to a
+pushover user account: ``` f.output_spool(app_key, h) f.output(s)
+f.output_close(plot, file) f.output_message(app_key, message, plot) ``` Calling
+f.output_spool() with an app key will start the system spooling output to send
+to pushover. h is an optional header to add as the first line of the message. H
+may include \
 >, \
 > or \
 > and these will be set to current system time and date respectively. When
 spooling is active, any calls to f.output() add lines to the spooled message.
 If appending to the message would exceed 1024 characters, the existing spooled
 message is sent and a new message spool is started. Calling f.output_close()
 will send the spooled message and optionally attach a binary image file. You
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.5
-Refactor debug messaging. Simplify charge_needed() output. Added 'target_soc'
-to charge_needed() settings Fix bat_info() giving incorrect temperatures when
-API returns 0 instead of -50 where there is no battery Fix key error when
-accessing cell volts and temps using an agent / installer account. Ensure
-output is generated if get_battery() fails using battery_info(). Update f.avg()
-to include calculation of averages in lists containng None values. Added
+(verbose) # Version Info 2.2.6
+Implement 2 second delay between calls that change inverter settings. Added
+strategy mode (timed_mode=2) to charge_needed(). Added set_strategy() and
+charge_strategy() to manage charging schedules and work mode changes. Refactor
+debug messaging. Simplify charge_needed() output. Added 'target_soc' to
+charge_needed() settings Fix bat_info() giving incorrect temperatures when API
+returns 0 instead of -50 where there is no battery Fix key error when accessing
+cell volts and temps using an agent / installer account. Ensure output is
+generated if get_battery() fails using battery_info(). Update f.avg() to
+include calculation of averages in lists containng None values. Added
 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
```

