# Comparing `tmp/pythfinder-0.0.3.17.tar.gz` & `tmp/pythfinder-0.0.3.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythfinder-0.0.3.17.tar", last modified: Fri May 17 15:59:32 2024, max compression
+gzip compressed data, was "pythfinder-0.0.3.18.tar", last modified: Fri May 17 18:17:59 2024, max compression
```

## Comparing `pythfinder-0.0.3.17.tar` & `pythfinder-0.0.3.18.tar`

### file list

```diff
@@ -1,141 +1,143 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:32.017423 pythfinder-0.0.3.17/
--rw-rw-rw-   0        0        0     1873 2024-05-15 15:31:47.000000 pythfinder-0.0.3.17/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1295 2024-05-14 05:43:57.000000 pythfinder-0.0.3.17/LICENSE.txt
--rw-rw-rw-   0        0        0      253 2024-05-15 16:24:01.000000 pythfinder-0.0.3.17/MANIFEST.in
--rw-rw-rw-   0        0        0      311 2024-05-17 15:59:32.016423 pythfinder-0.0.3.17/PKG-INFO
--rw-rw-rw-   0        0        0    16424 2024-05-17 15:53:24.000000 pythfinder-0.0.3.17/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.744458 pythfinder-0.0.3.17/pythfinder/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.789440 pythfinder-0.0.3.17/pythfinder/Components/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.790466 pythfinder-0.0.3.17/pythfinder/Components/BetterClasses/
--rw-rw-rw-   0        0        0        0 2024-05-15 15:03:55.000000 pythfinder-0.0.3.17/pythfinder/Components/BetterClasses/__init__.py
--rw-rw-rw-   0        0        0     1168 2024-05-13 14:52:24.000000 pythfinder-0.0.3.17/pythfinder/Components/BetterClasses/booleanEx.py
--rw-rw-rw-   0        0        0      627 2024-05-13 14:52:55.000000 pythfinder-0.0.3.17/pythfinder/Components/BetterClasses/edgeDetectorEx.py
--rw-rw-rw-   0        0        0     1140 2024-05-13 15:07:55.000000 pythfinder-0.0.3.17/pythfinder/Components/BetterClasses/errorEx.py
--rw-rw-rw-   0        0        0     4862 2024-05-13 14:45:33.000000 pythfinder-0.0.3.17/pythfinder/Components/BetterClasses/mathEx.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.806092 pythfinder-0.0.3.17/pythfinder/Components/Constants/
--rw-rw-rw-   0        0        0        0 2024-05-15 15:03:51.000000 pythfinder-0.0.3.17/pythfinder/Components/Constants/__init__.py
--rw-rw-rw-   0        0        0    25636 2024-05-16 18:21:09.000000 pythfinder-0.0.3.17/pythfinder/Components/Constants/constants.py
--rw-rw-rw-   0        0        0     2905 2024-05-13 15:08:14.000000 pythfinder-0.0.3.17/pythfinder/Components/Constants/constrains.py
--rw-rw-rw-   0        0        0     2705 2024-05-13 15:11:03.000000 pythfinder-0.0.3.17/pythfinder/Components/Constants/screenSize.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.806092 pythfinder-0.0.3.17/pythfinder/Components/Controllers/
--rw-rw-rw-   0        0        0      642 2024-05-13 15:12:44.000000 pythfinder-0.0.3.17/pythfinder/Components/Controllers/PIDCoefficients.py
--rw-rw-rw-   0        0        0     1163 2024-05-14 16:07:14.000000 pythfinder-0.0.3.17/pythfinder/Components/Controllers/PIDController.py
--rw-rw-rw-   0        0        0        0 2024-05-15 15:04:30.000000 pythfinder-0.0.3.17/pythfinder/Components/Controllers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.821718 pythfinder-0.0.3.17/pythfinder/Components/Menu/
--rw-rw-rw-   0        0        0        0 2024-05-15 15:03:47.000000 pythfinder-0.0.3.17/pythfinder/Components/Menu/__init__.py
--rw-rw-rw-   0        0        0    23219 2024-05-16 15:21:08.000000 pythfinder-0.0.3.17/pythfinder/Components/Menu/buttons.py
--rw-rw-rw-   0        0        0     1581 2024-05-15 17:22:04.000000 pythfinder-0.0.3.17/pythfinder/Components/Menu/enums.py
--rw-rw-rw-   0        0        0    22764 2024-05-16 15:15:01.000000 pythfinder-0.0.3.17/pythfinder/Components/Menu/main.py
--rw-rw-rw-   0        0        0     4196 2024-05-16 15:14:02.000000 pythfinder-0.0.3.17/pythfinder/Components/Menu/menus.py
--rw-rw-rw-   0        0        0        0 2024-05-15 15:04:12.000000 pythfinder-0.0.3.17/pythfinder/Components/__init__.py
--rw-rw-rw-   0        0        0     5720 2024-05-14 16:04:43.000000 pythfinder-0.0.3.17/pythfinder/Components/background.py
--rw-rw-rw-   0        0        0     9569 2024-05-14 16:05:08.000000 pythfinder-0.0.3.17/pythfinder/Components/controls.py
--rw-rw-rw-   0        0        0     1853 2024-05-14 16:05:12.000000 pythfinder-0.0.3.17/pythfinder/Components/fade.py
--rw-rw-rw-   0        0        0     9909 2024-05-15 16:43:21.000000 pythfinder-0.0.3.17/pythfinder/Components/robot.py
--rw-rw-rw-   0        0        0     2161 2024-05-15 17:34:53.000000 pythfinder-0.0.3.17/pythfinder/Components/table.py
--rw-rw-rw-   0        0        0     4633 2024-05-14 16:05:37.000000 pythfinder-0.0.3.17/pythfinder/Components/trail.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.837345 pythfinder-0.0.3.17/pythfinder/Font/
--rw-rw-rw-   0        0        0    40824 2024-05-15 15:06:17.000000 pythfinder-0.0.3.17/pythfinder/Font/GraffitiYouth-Regular.otf
--rw-rw-rw-   0        0        0       30 2024-05-15 16:46:45.000000 pythfinder-0.0.3.17/pythfinder/Font/__init__.py
--rw-rw-rw-   0        0        0      334 2024-05-15 15:06:17.000000 pythfinder-0.0.3.17/pythfinder/Font/credits.txt
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.860998 pythfinder-0.0.3.17/pythfinder/Images/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.876610 pythfinder-0.0.3.17/pythfinder/Images/Controls/
--rw-rw-rw-   0        0        0        0 2024-05-14 18:17:56.000000 pythfinder-0.0.3.17/pythfinder/Images/Controls/__init__.py
--rw-rw-rw-   0        0        0   525562 2024-03-31 07:01:14.000000 pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_backwards.png
--rw-rw-rw-   0        0        0   530916 2024-03-31 07:01:10.000000 pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_forwards.png
--rw-rw-rw-   0        0        0   533042 2024-03-31 07:01:19.000000 pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_hide_trail.png
--rw-rw-rw-   0        0        0   561920 2024-03-31 14:58:53.000000 pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_selecting_off.png
--rw-rw-rw-   0        0        0   558616 2024-03-31 14:58:49.000000 pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_selecting_on.png
--rw-rw-rw-   0        0        0   531856 2024-03-31 07:00:59.000000 pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_show_trail.png
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.876610 pythfinder-0.0.3.17/pythfinder/Images/Menu/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.876610 pythfinder-0.0.3.17/pythfinder/Images/Menu/General/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.707596 pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.892237 pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/Left/
--rw-rw-rw-   0        0        0     5149 2024-04-07 08:30:53.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/Left/left_arrow.png
--rw-rw-rw-   0        0        0     5334 2024-04-07 08:30:48.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/Left/selected_left_arrow.png
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.892237 pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/Right/
--rw-rw-rw-   0        0        0     5181 2024-04-07 08:31:22.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/Right/right_arrow.png
--rw-rw-rw-   0        0        0     5279 2024-04-07 08:31:21.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/Right/selected_right_arrow.png
--rw-rw-rw-   0        0        0        0 2024-05-14 18:18:26.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/General/__init__.py
--rw-rw-rw-   0        0        0   467492 2024-04-07 08:30:13.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/General/general_menu.png
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.907862 pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/
--rw-rw-rw-   0        0        0     8011 2024-04-05 16:14:53.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/menu_button.png
--rw-rw-rw-   0        0        0     6208 2024-04-05 16:14:57.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/menu_home_button.png
--rw-rw-rw-   0        0        0  1606752 2024-04-05 16:15:02.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/menu_main.png
--rw-rw-rw-   0        0        0     8399 2024-04-06 11:39:50.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/selected_menu_button.png
--rw-rw-rw-   0        0        0     6451 2024-04-06 11:39:46.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/selected_menu_home_button.png
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.907862 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.923823 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/DrawTable/
--rw-rw-rw-   0        0        0    33164 2024-05-15 17:13:46.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/DrawTable/draw_table_off.png
--rw-rw-rw-   0        0        0    33397 2024-05-15 17:13:39.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/DrawTable/draw_table_on.png
--rw-rw-rw-   0        0        0    34675 2024-05-15 17:13:44.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/DrawTable/selected_draw_table_off.png
--rw-rw-rw-   0        0        0    34863 2024-05-15 17:13:48.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/DrawTable/selected_draw_table_on.png
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.931692 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/FieldCentric/
--rw-rw-rw-   0        0        0    33821 2024-04-07 08:27:04.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/FieldCentric/field_centric_off.png
--rw-rw-rw-   0        0        0    34053 2024-04-07 08:27:04.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/FieldCentric/field_centric_on.png
--rw-rw-rw-   0        0        0    35325 2024-04-07 08:27:04.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_off.png
--rw-rw-rw-   0        0        0    35522 2024-04-07 08:27:04.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_on.png
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.940759 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/RobotBorder/
--rw-rw-rw-   0        0        0    32516 2024-04-07 08:27:48.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/RobotBorder/robot_border_off.png
--rw-rw-rw-   0        0        0    32757 2024-04-07 08:27:49.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/RobotBorder/robot_border_on.png
--rw-rw-rw-   0        0        0    33964 2024-04-07 08:27:48.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_off.png
--rw-rw-rw-   0        0        0    34153 2024-04-07 08:27:48.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_on.png
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.949406 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/ScreenBorder/
--rw-rw-rw-   0        0        0    34863 2024-04-07 08:28:53.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_off.png
--rw-rw-rw-   0        0        0    35031 2024-04-07 08:28:53.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_on.png
--rw-rw-rw-   0        0        0    36547 2024-04-07 08:28:53.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_off.png
--rw-rw-rw-   0        0        0    36670 2024-04-07 08:28:53.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_on.png
--rw-rw-rw-   0        0        0    20270 2024-04-09 17:13:50.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/other_indicator.png
--rw-rw-rw-   0        0        0    13339 2024-04-07 08:29:32.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/other_quadrant.png
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.971411 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/
--rw-rw-rw-   0        0        0    28975 2024-04-08 04:32:03.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/height.png
--rw-rw-rw-   0        0        0    20193 2024-04-08 04:32:07.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/robot_indicator.png
--rw-rw-rw-   0        0        0    39077 2024-04-08 04:32:04.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/robot_path.png
--rw-rw-rw-   0        0        0   138988 2024-04-08 04:32:10.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/robot_path_quadrant.png
--rw-rw-rw-   0        0        0   115045 2024-04-08 04:32:12.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/robot_specs_quadrant.png
--rw-rw-rw-   0        0        0    20716 2024-04-08 04:32:17.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/scale.png
--rw-rw-rw-   0        0        0    30701 2024-04-08 04:32:20.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/selected_height.png
--rw-rw-rw-   0        0        0    40956 2024-04-08 04:32:22.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/selected_robot_path.png
--rw-rw-rw-   0        0        0    21855 2024-04-08 04:32:24.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/selected_scale.png
--rw-rw-rw-   0        0        0    21917 2024-04-08 04:32:27.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/selected_width.png
--rw-rw-rw-   0        0        0    20843 2024-04-08 04:32:30.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/width.png
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.993416 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/
--rw-rw-rw-   0        0        0    19651 2024-04-06 15:09:11.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/interface_button.png
--rw-rw-rw-   0        0        0    14899 2024-04-06 15:09:15.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/other_button.png
--rw-rw-rw-   0        0        0    20750 2024-04-06 15:09:19.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/pathing_button.png
--rw-rw-rw-   0        0        0    13645 2024-04-06 15:09:23.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/robot_button.png
--rw-rw-rw-   0        0        0    16954 2024-04-06 15:09:26.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selected_interface_button.png
--rw-rw-rw-   0        0        0    13205 2024-04-06 15:09:28.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selected_other_button.png
--rw-rw-rw-   0        0        0    17797 2024-04-06 15:09:31.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selected_pathing_button.png
--rw-rw-rw-   0        0        0    12126 2024-04-06 15:09:33.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selected_robot_button.png
--rw-rw-rw-   0        0        0    11787 2024-04-06 15:09:36.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selected_trail_button.png
--rw-rw-rw-   0        0        0    79511 2024-04-06 15:09:38.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selection_menu.png
--rw-rw-rw-   0        0        0    13448 2024-04-06 15:09:41.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/trail_button.png
--rw-rw-rw-   0        0        0        0 2024-05-14 18:18:10.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.996417 pythfinder-0.0.3.17/pythfinder/Images/Robot/
--rw-rw-rw-   0        0        0        0 2024-05-14 18:18:58.000000 pythfinder-0.0.3.17/pythfinder/Images/Robot/__init__.py
--rw-rw-rw-   0        0        0   600926 2024-03-18 18:10:12.000000 pythfinder-0.0.3.17/pythfinder/Images/Robot/bot_from_above.png
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:32.003418 pythfinder-0.0.3.17/pythfinder/Images/Table/
--rw-rw-rw-   0        0        0  1025907 2024-04-29 12:07:29.000000 pythfinder-0.0.3.17/pythfinder/Images/Table/FLL_table_MP.jpg
--rw-rw-rw-   0        0        0        0 2024-05-14 18:19:06.000000 pythfinder-0.0.3.17/pythfinder/Images/Table/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-14 18:17:47.000000 pythfinder-0.0.3.17/pythfinder/Images/__init__.py
--rw-rw-rw-   0        0        0    16718 2024-04-07 11:58:49.000000 pythfinder-0.0.3.17/pythfinder/Images/none.png
--rw-rw-rw-   0        0        0  1287680 2024-05-16 15:43:35.000000 pythfinder-0.0.3.17/pythfinder/Images/pythfinder_logo_mk3.png
--rw-rw-rw-   0        0        0    17665 2024-04-07 11:58:46.000000 pythfinder-0.0.3.17/pythfinder/Images/selected_none.png
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:32.014422 pythfinder-0.0.3.17/pythfinder/Trajectory/
--rw-rw-rw-   0        0        0       22 2024-05-15 16:36:13.000000 pythfinder-0.0.3.17/pythfinder/Trajectory/__init__.py
--rw-rw-rw-   0        0        0    58104 2024-05-16 15:33:26.000000 pythfinder-0.0.3.17/pythfinder/Trajectory/builder.py
--rw-rw-rw-   0        0        0     1709 2024-05-14 16:06:07.000000 pythfinder-0.0.3.17/pythfinder/Trajectory/feedback.py
--rw-rw-rw-   0        0        0     4366 2024-05-14 16:06:12.000000 pythfinder-0.0.3.17/pythfinder/Trajectory/feedforward.py
--rw-rw-rw-   0        0        0     1564 2024-05-14 16:06:17.000000 pythfinder-0.0.3.17/pythfinder/Trajectory/kinematics.py
--rw-rw-rw-   0        0        0     5914 2024-05-14 16:06:21.000000 pythfinder-0.0.3.17/pythfinder/Trajectory/splines.py
--rw-rw-rw-   0        0        0       98 2024-05-15 16:36:20.000000 pythfinder-0.0.3.17/pythfinder/__init__.py
--rw-rw-rw-   0        0        0    11256 2024-05-17 15:58:18.000000 pythfinder-0.0.3.17/pythfinder/core.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.776371 pythfinder-0.0.3.17/pythfinder.egg-info/
--rw-rw-rw-   0        0        0      311 2024-05-17 15:59:31.000000 pythfinder-0.0.3.17/pythfinder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5070 2024-05-17 15:59:31.000000 pythfinder-0.0.3.17/pythfinder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 15:59:31.000000 pythfinder-0.0.3.17/pythfinder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-17 15:59:31.000000 pythfinder-0.0.3.17/pythfinder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-17 15:59:31.000000 pythfinder-0.0.3.17/pythfinder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 15:59:32.017423 pythfinder-0.0.3.17/setup.cfg
--rw-rw-rw-   0        0        0      568 2024-05-17 15:55:18.000000 pythfinder-0.0.3.17/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.841752 pythfinder-0.0.3.18/
+-rw-rw-rw-   0        0        0     2117 2024-05-17 18:13:42.000000 pythfinder-0.0.3.18/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1295 2024-05-14 05:43:57.000000 pythfinder-0.0.3.18/LICENSE.txt
+-rw-rw-rw-   0        0        0      253 2024-05-15 16:24:01.000000 pythfinder-0.0.3.18/MANIFEST.in
+-rw-rw-rw-   0        0        0      311 2024-05-17 18:17:59.841752 pythfinder-0.0.3.18/PKG-INFO
+-rw-rw-rw-   0        0        0    16632 2024-05-17 18:16:25.000000 pythfinder-0.0.3.18/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.572205 pythfinder-0.0.3.18/pythfinder/
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.609967 pythfinder-0.0.3.18/pythfinder/Components/
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.625594 pythfinder-0.0.3.18/pythfinder/Components/BetterClasses/
+-rw-rw-rw-   0        0        0        0 2024-05-15 15:03:55.000000 pythfinder-0.0.3.18/pythfinder/Components/BetterClasses/__init__.py
+-rw-rw-rw-   0        0        0     1168 2024-05-13 14:52:24.000000 pythfinder-0.0.3.18/pythfinder/Components/BetterClasses/booleanEx.py
+-rw-rw-rw-   0        0        0      627 2024-05-13 14:52:55.000000 pythfinder-0.0.3.18/pythfinder/Components/BetterClasses/edgeDetectorEx.py
+-rw-rw-rw-   0        0        0     1140 2024-05-13 15:07:55.000000 pythfinder-0.0.3.18/pythfinder/Components/BetterClasses/errorEx.py
+-rw-rw-rw-   0        0        0     4862 2024-05-13 14:45:33.000000 pythfinder-0.0.3.18/pythfinder/Components/BetterClasses/mathEx.py
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.625594 pythfinder-0.0.3.18/pythfinder/Components/Constants/
+-rw-rw-rw-   0        0        0        0 2024-05-15 15:03:51.000000 pythfinder-0.0.3.18/pythfinder/Components/Constants/__init__.py
+-rw-rw-rw-   0        0        0    25787 2024-05-17 18:11:21.000000 pythfinder-0.0.3.18/pythfinder/Components/Constants/constants.py
+-rw-rw-rw-   0        0        0     2905 2024-05-13 15:08:14.000000 pythfinder-0.0.3.18/pythfinder/Components/Constants/constrains.py
+-rw-rw-rw-   0        0        0     2705 2024-05-13 15:11:03.000000 pythfinder-0.0.3.18/pythfinder/Components/Constants/screenSize.py
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.641221 pythfinder-0.0.3.18/pythfinder/Components/Controllers/
+-rw-rw-rw-   0        0        0      642 2024-05-13 15:12:44.000000 pythfinder-0.0.3.18/pythfinder/Components/Controllers/PIDCoefficients.py
+-rw-rw-rw-   0        0        0     1163 2024-05-14 16:07:14.000000 pythfinder-0.0.3.18/pythfinder/Components/Controllers/PIDController.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 15:04:30.000000 pythfinder-0.0.3.18/pythfinder/Components/Controllers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.641221 pythfinder-0.0.3.18/pythfinder/Components/Menu/
+-rw-rw-rw-   0        0        0        0 2024-05-15 15:03:47.000000 pythfinder-0.0.3.18/pythfinder/Components/Menu/__init__.py
+-rw-rw-rw-   0        0        0    23219 2024-05-16 15:21:08.000000 pythfinder-0.0.3.18/pythfinder/Components/Menu/buttons.py
+-rw-rw-rw-   0        0        0     1581 2024-05-15 17:22:04.000000 pythfinder-0.0.3.18/pythfinder/Components/Menu/enums.py
+-rw-rw-rw-   0        0        0    22764 2024-05-16 15:15:01.000000 pythfinder-0.0.3.18/pythfinder/Components/Menu/main.py
+-rw-rw-rw-   0        0        0     4196 2024-05-16 15:14:02.000000 pythfinder-0.0.3.18/pythfinder/Components/Menu/menus.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 15:04:12.000000 pythfinder-0.0.3.18/pythfinder/Components/__init__.py
+-rw-rw-rw-   0        0        0     5720 2024-05-14 16:04:43.000000 pythfinder-0.0.3.18/pythfinder/Components/background.py
+-rw-rw-rw-   0        0        0     9783 2024-05-17 17:01:46.000000 pythfinder-0.0.3.18/pythfinder/Components/controls.py
+-rw-rw-rw-   0        0        0     1853 2024-05-14 16:05:12.000000 pythfinder-0.0.3.18/pythfinder/Components/fade.py
+-rw-rw-rw-   0        0        0     9909 2024-05-15 16:43:21.000000 pythfinder-0.0.3.18/pythfinder/Components/robot.py
+-rw-rw-rw-   0        0        0     2161 2024-05-15 17:34:53.000000 pythfinder-0.0.3.18/pythfinder/Components/table.py
+-rw-rw-rw-   0        0        0     4633 2024-05-14 16:05:37.000000 pythfinder-0.0.3.18/pythfinder/Components/trail.py
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.672471 pythfinder-0.0.3.18/pythfinder/Font/
+-rw-rw-rw-   0        0        0    40824 2024-05-15 15:06:17.000000 pythfinder-0.0.3.18/pythfinder/Font/GraffitiYouth-Regular.otf
+-rw-rw-rw-   0        0        0       30 2024-05-15 16:46:45.000000 pythfinder-0.0.3.18/pythfinder/Font/__init__.py
+-rw-rw-rw-   0        0        0      334 2024-05-15 15:06:17.000000 pythfinder-0.0.3.18/pythfinder/Font/credits.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.688097 pythfinder-0.0.3.18/pythfinder/Images/
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.710234 pythfinder-0.0.3.18/pythfinder/Images/Controls/
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:17:56.000000 pythfinder-0.0.3.18/pythfinder/Images/Controls/__init__.py
+-rw-rw-rw-   0        0        0   525562 2024-03-31 07:01:14.000000 pythfinder-0.0.3.18/pythfinder/Images/Controls/btn_backwards.png
+-rw-rw-rw-   0        0        0   530916 2024-03-31 07:01:10.000000 pythfinder-0.0.3.18/pythfinder/Images/Controls/btn_forwards.png
+-rw-rw-rw-   0        0        0   533042 2024-03-31 07:01:19.000000 pythfinder-0.0.3.18/pythfinder/Images/Controls/btn_hide_trail.png
+-rw-rw-rw-   0        0        0   561920 2024-03-31 14:58:53.000000 pythfinder-0.0.3.18/pythfinder/Images/Controls/btn_selecting_off.png
+-rw-rw-rw-   0        0        0   558616 2024-03-31 14:58:49.000000 pythfinder-0.0.3.18/pythfinder/Images/Controls/btn_selecting_on.png
+-rw-rw-rw-   0        0        0   531856 2024-03-31 07:00:59.000000 pythfinder-0.0.3.18/pythfinder/Images/Controls/btn_show_trail.png
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.710234 pythfinder-0.0.3.18/pythfinder/Images/Menu/
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.710234 pythfinder-0.0.3.18/pythfinder/Images/Menu/General/
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.540953 pythfinder-0.0.3.18/pythfinder/Images/Menu/General/Arrows/
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.710234 pythfinder-0.0.3.18/pythfinder/Images/Menu/General/Arrows/Left/
+-rw-rw-rw-   0        0        0     5149 2024-04-07 08:30:53.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/General/Arrows/Left/left_arrow.png
+-rw-rw-rw-   0        0        0     5334 2024-04-07 08:30:48.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/General/Arrows/Left/selected_left_arrow.png
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.725859 pythfinder-0.0.3.18/pythfinder/Images/Menu/General/Arrows/Right/
+-rw-rw-rw-   0        0        0     5181 2024-04-07 08:31:22.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/General/Arrows/Right/right_arrow.png
+-rw-rw-rw-   0        0        0     5279 2024-04-07 08:31:21.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/General/Arrows/Right/selected_right_arrow.png
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:18:26.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/General/__init__.py
+-rw-rw-rw-   0        0        0   467492 2024-04-07 08:30:13.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/General/general_menu.png
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.725859 pythfinder-0.0.3.18/pythfinder/Images/Menu/Main/
+-rw-rw-rw-   0        0        0     8011 2024-04-05 16:14:53.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Main/menu_button.png
+-rw-rw-rw-   0        0        0     6208 2024-04-05 16:14:57.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Main/menu_home_button.png
+-rw-rw-rw-   0        0        0  1606752 2024-04-05 16:15:02.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Main/menu_main.png
+-rw-rw-rw-   0        0        0     8399 2024-04-06 11:39:50.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Main/selected_menu_button.png
+-rw-rw-rw-   0        0        0     6451 2024-04-06 11:39:46.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Main/selected_menu_home_button.png
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.741486 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.741486 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/DrawTable/
+-rw-rw-rw-   0        0        0    33164 2024-05-15 17:13:46.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/DrawTable/draw_table_off.png
+-rw-rw-rw-   0        0        0    33397 2024-05-15 17:13:39.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/DrawTable/draw_table_on.png
+-rw-rw-rw-   0        0        0    34675 2024-05-15 17:13:44.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/DrawTable/selected_draw_table_off.png
+-rw-rw-rw-   0        0        0    34863 2024-05-15 17:13:48.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/DrawTable/selected_draw_table_on.png
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.757112 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/FieldCentric/
+-rw-rw-rw-   0        0        0    33821 2024-04-07 08:27:04.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/FieldCentric/field_centric_off.png
+-rw-rw-rw-   0        0        0    34053 2024-04-07 08:27:04.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/FieldCentric/field_centric_on.png
+-rw-rw-rw-   0        0        0    35325 2024-04-07 08:27:04.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_off.png
+-rw-rw-rw-   0        0        0    35522 2024-04-07 08:27:04.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_on.png
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.757112 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/RobotBorder/
+-rw-rw-rw-   0        0        0    32516 2024-04-07 08:27:48.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/RobotBorder/robot_border_off.png
+-rw-rw-rw-   0        0        0    32757 2024-04-07 08:27:49.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/RobotBorder/robot_border_on.png
+-rw-rw-rw-   0        0        0    33964 2024-04-07 08:27:48.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_off.png
+-rw-rw-rw-   0        0        0    34153 2024-04-07 08:27:48.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_on.png
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.772739 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/ScreenBorder/
+-rw-rw-rw-   0        0        0    34863 2024-04-07 08:28:53.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_off.png
+-rw-rw-rw-   0        0        0    35031 2024-04-07 08:28:53.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_on.png
+-rw-rw-rw-   0        0        0    36547 2024-04-07 08:28:53.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_off.png
+-rw-rw-rw-   0        0        0    36670 2024-04-07 08:28:53.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_on.png
+-rw-rw-rw-   0        0        0    20270 2024-04-09 17:13:50.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/other_indicator.png
+-rw-rw-rw-   0        0        0    13339 2024-04-07 08:29:32.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/other_quadrant.png
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.794870 pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/
+-rw-rw-rw-   0        0        0    28975 2024-04-08 04:32:03.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/height.png
+-rw-rw-rw-   0        0        0    20193 2024-04-08 04:32:07.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/robot_indicator.png
+-rw-rw-rw-   0        0        0    39077 2024-04-08 04:32:04.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/robot_path.png
+-rw-rw-rw-   0        0        0   138988 2024-04-08 04:32:10.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/robot_path_quadrant.png
+-rw-rw-rw-   0        0        0   115045 2024-04-08 04:32:12.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/robot_specs_quadrant.png
+-rw-rw-rw-   0        0        0    20716 2024-04-08 04:32:17.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/scale.png
+-rw-rw-rw-   0        0        0    30701 2024-04-08 04:32:20.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/selected_height.png
+-rw-rw-rw-   0        0        0    40956 2024-04-08 04:32:22.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/selected_robot_path.png
+-rw-rw-rw-   0        0        0    21855 2024-04-08 04:32:24.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/selected_scale.png
+-rw-rw-rw-   0        0        0    21917 2024-04-08 04:32:27.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/selected_width.png
+-rw-rw-rw-   0        0        0    20843 2024-04-08 04:32:30.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/width.png
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.826126 pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/
+-rw-rw-rw-   0        0        0    19651 2024-04-06 15:09:11.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/interface_button.png
+-rw-rw-rw-   0        0        0    14899 2024-04-06 15:09:15.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/other_button.png
+-rw-rw-rw-   0        0        0    20750 2024-04-06 15:09:19.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/pathing_button.png
+-rw-rw-rw-   0        0        0    13645 2024-04-06 15:09:23.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/robot_button.png
+-rw-rw-rw-   0        0        0    16954 2024-04-06 15:09:26.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/selected_interface_button.png
+-rw-rw-rw-   0        0        0    13205 2024-04-06 15:09:28.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/selected_other_button.png
+-rw-rw-rw-   0        0        0    17797 2024-04-06 15:09:31.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/selected_pathing_button.png
+-rw-rw-rw-   0        0        0    12126 2024-04-06 15:09:33.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/selected_robot_button.png
+-rw-rw-rw-   0        0        0    11787 2024-04-06 15:09:36.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/selected_trail_button.png
+-rw-rw-rw-   0        0        0    79511 2024-04-06 15:09:38.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/selection_menu.png
+-rw-rw-rw-   0        0        0    13448 2024-04-06 15:09:41.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/trail_button.png
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:18:10.000000 pythfinder-0.0.3.18/pythfinder/Images/Menu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.826126 pythfinder-0.0.3.18/pythfinder/Images/Robot/
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:18:58.000000 pythfinder-0.0.3.18/pythfinder/Images/Robot/__init__.py
+-rw-rw-rw-   0        0        0   600926 2024-03-18 18:10:12.000000 pythfinder-0.0.3.18/pythfinder/Images/Robot/bot_from_above.png
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.826126 pythfinder-0.0.3.18/pythfinder/Images/Table/
+-rw-rw-rw-   0        0        0  1025907 2024-04-29 12:07:29.000000 pythfinder-0.0.3.18/pythfinder/Images/Table/FLL_table_MP.jpg
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:19:06.000000 pythfinder-0.0.3.18/pythfinder/Images/Table/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:17:47.000000 pythfinder-0.0.3.18/pythfinder/Images/__init__.py
+-rw-rw-rw-   0        0        0    16718 2024-04-07 11:58:49.000000 pythfinder-0.0.3.18/pythfinder/Images/none.png
+-rw-rw-rw-   0        0        0  1287680 2024-05-16 15:43:35.000000 pythfinder-0.0.3.18/pythfinder/Images/pythfinder_logo_mk3.png
+-rw-rw-rw-   0        0        0    17665 2024-04-07 11:58:46.000000 pythfinder-0.0.3.18/pythfinder/Images/selected_none.png
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.841752 pythfinder-0.0.3.18/pythfinder/Screenshots/
+-rw-rw-rw-   0        0        0        0 2024-05-17 17:05:52.000000 pythfinder-0.0.3.18/pythfinder/Screenshots/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.841752 pythfinder-0.0.3.18/pythfinder/Trajectory/
+-rw-rw-rw-   0        0        0       22 2024-05-15 16:36:13.000000 pythfinder-0.0.3.18/pythfinder/Trajectory/__init__.py
+-rw-rw-rw-   0        0        0    58104 2024-05-16 15:33:26.000000 pythfinder-0.0.3.18/pythfinder/Trajectory/builder.py
+-rw-rw-rw-   0        0        0     1709 2024-05-14 16:06:07.000000 pythfinder-0.0.3.18/pythfinder/Trajectory/feedback.py
+-rw-rw-rw-   0        0        0     4366 2024-05-14 16:06:12.000000 pythfinder-0.0.3.18/pythfinder/Trajectory/feedforward.py
+-rw-rw-rw-   0        0        0     1564 2024-05-14 16:06:17.000000 pythfinder-0.0.3.18/pythfinder/Trajectory/kinematics.py
+-rw-rw-rw-   0        0        0     5914 2024-05-14 16:06:21.000000 pythfinder-0.0.3.18/pythfinder/Trajectory/splines.py
+-rw-rw-rw-   0        0        0       98 2024-05-15 16:36:20.000000 pythfinder-0.0.3.18/pythfinder/__init__.py
+-rw-rw-rw-   0        0        0    12527 2024-05-17 18:09:40.000000 pythfinder-0.0.3.18/pythfinder/core.py
+drwxrwxrwx   0        0        0        0 2024-05-17 18:17:59.594338 pythfinder-0.0.3.18/pythfinder.egg-info/
+-rw-rw-rw-   0        0        0      311 2024-05-17 18:17:58.000000 pythfinder-0.0.3.18/pythfinder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5105 2024-05-17 18:17:59.000000 pythfinder-0.0.3.18/pythfinder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 18:17:58.000000 pythfinder-0.0.3.18/pythfinder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-17 18:17:58.000000 pythfinder-0.0.3.18/pythfinder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-17 18:17:58.000000 pythfinder-0.0.3.18/pythfinder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 18:17:59.857379 pythfinder-0.0.3.18/setup.cfg
+-rw-rw-rw-   0        0        0      568 2024-05-17 18:17:33.000000 pythfinder-0.0.3.18/setup.py
```

### Comparing `pythfinder-0.0.3.17/CHANGELOG.txt` & `pythfinder-0.0.3.18/CHANGELOG.txt`

 * *Files 13% similar despite different names*

```diff
@@ -25,24 +25,32 @@
     * limited use, can't directly influence robot's real life motion;
     * needs the the same code from the robot's project to be translated 
       (micropython to python and vice versa);
     * very limited user-friendly interface interraction;
     * hardcoded > abstraction;
 
 
-0.0.3 (15.05.2024)
------------------
+0.0.3.17 (17.05.2024)
+---------------------
 - First easy-use version out of all.
 - Small unusable versions were needed for packaging all the data right.
 - Improvements:
     * adding feedforward approach through complex trajectory building techniques,
       with velocity-constrained motion profiles, assuring continuity, for more 
       precise applications;
     * markers, interruptors and volatile constrains, which are more or less
       modifiers for the trajectory's behaviour. Markers enable you to perform
       multithreading-related tasks inside the trajectory;
     * in-game menu for easier manipulation of constants (NOT FULLY IMPLEMENTED)
     * migrating to more complex abstraction for elements such as the menu or the
       actual robot 
     * PS4 and PS5 controllers are now supported, but not any Nintendo device
     * visualisaltion of the velocity and acceleration profiles using matlib
+
+
+0.0.3.18 (17.05.2024)
+---------------------
+- you can take screenshots now! (press on the left joystick button and find them
+  in the 'Screenshots' folder where the library is installed)
+- easter egg?
+- fixed more visual bugs
```

### Comparing `pythfinder-0.0.3.17/LICENSE.txt` & `pythfinder-0.0.3.18/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/README.md` & `pythfinder-0.0.3.18/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -119,17 +119,18 @@
 <span style="font-size:0.8em;">*(the order of buttons is: **ps4 / xbox**)*</span>
 * <span style="color: lightgreen">△ / Y</span> **--** go forwards / backwards (when field centric is on) ;
 * <span style="color: lightgreen">□ / X</span> **--** enter / exit interface setting menu ;
 * <span style="color: lightgreen">○ / B</span> **--** reset robot pose to origin / selects buttons (when the menu is activated) ;
 * <span style="color: lightgreen">X / A</span> **--** show / hide trail ;
 * <span style="color: lightgreen">left bumper</span> **--** erase trail / sets values to default (when the menu is activated) ;
 * <span style="color: lightgreen">right bumper</span> **--** when held enters selection mode ;
-* <span style="color: lightgreen">D-pad</span> **--** select robot's orientation (when selection mode is on) ;
+* <span style="color: lightgreen">D-pad</span> **--** move through interface menu / select robot's orientation (when selection mode is on) ;
 * <span style="color: lightgreen">left joystick</span> **--** controls robot linear velocity + angular velocity (when field centric is on) ;
-* <span style="color: lightgreen">right joystick</span> -- controls angular velocity (**ONLY** when field centric is off) ;
+* <span style="color: lightgreen">right joystick</span> *--* controls angular velocity (**ONLY** when field centric is off) ;
+* <span style="color: lightgreen">left joystick button</span> **--** takes a screenshot (found in the 'Screenshots' folder inside the locally installed library location) ;
 
 ## Create a Trajectory
 
 Trajectory building is the main feature on our library. Although it's implementation is complicated (see the [documentation](#advanced-usage)), it's usage is trivialy simple.
 
 <span style="font-size:1.5em;">*What are trajectories?*</span> <br />
 Firstly, we define a particular set of robot information (like the pose, velocity, distance traveled etc.) as a '**MotionState**'. Multiple motion states sharing a specific similarity are called '**MotionSegments**'. With the same logic in mind, multiple motion segments compose e '**Trajectory**'.
@@ -302,15 +303,15 @@
 * *inspiration: [roadrunner FTC][13]*
 * *font: [graffitiyouthregular][5]*
 * *table image: [source][15]*
 
 <br />
 
 
-*v. alpha-0.0.3*
+*v. 0.0.3.17-alpha*
 
 
 [1]: https://www.python.org/downloads/             "python download page"
 [2]: https://pip.pypa.io/en/stable/installation/   "pip download page"
 [3]: https://www.pygame.org/docs/                  "pygame quick start"
 [4]: https://matplotlib.org/stable/                "matplot quick start"
 [5]: https://www.dafont.com/graffiti-youth.font    "our team's use-free font"
```

### Comparing `pythfinder-0.0.3.17/pythfinder/Components/BetterClasses/booleanEx.py` & `pythfinder-0.0.3.18/pythfinder/Components/BetterClasses/booleanEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Components/BetterClasses/edgeDetectorEx.py` & `pythfinder-0.0.3.18/pythfinder/Components/BetterClasses/edgeDetectorEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Components/BetterClasses/errorEx.py` & `pythfinder-0.0.3.18/pythfinder/Components/BetterClasses/errorEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Components/BetterClasses/mathEx.py` & `pythfinder-0.0.3.18/pythfinder/Components/BetterClasses/mathEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Components/Constants/constants.py` & `pythfinder-0.0.3.18/pythfinder/Components/Constants/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 #           - default constant values, image manipulation for the interface and Constants class
 #           - default keys for joystick control
 #           - helper methods for conversion
 
 
 device_relative_path = os.path.join(os.path.dirname(__file__), '..', '..', 'Images')
 
+screenshot_path = os.path.join(device_relative_path, 'Screenshots\\')
+
 default_robot_image_name = 'bot_from_above'
 default_robot_image_path = 'Robot/'
 default_robot_image_extension = 'png'
 default_robot_image_source = os.path.join(device_relative_path, 'Robot/bot_from_above.png')
 
 default_robot_scaling_factor = 1
 default_robot_height_cm = 20
@@ -301,14 +303,15 @@
 
 xbox_disable_button = 2
 xbox_direction_button = 3
 xbox_zero_button = 1
 xbox_head_selection_button = 5
 xbox_trail_button = 0
 xbox_erase_trail_button = 4
+xbox_screenshot_button = 8
 
 xbox_turn_0 = (0, 1)
 xbox_turn_45 = (1, 1)
 xbox_turn_90 = (1, 0)
 xbox_turn_135 = (1, -1)
 xbox_turn_180 = (0, -1)
 xbox_turn_225 = (-1, -1)
@@ -323,14 +326,15 @@
 
 ps4_disable_button = 2
 ps4_direction_button = 3
 ps4_zero_button = 1
 ps4_head_selection_button = 10
 ps4_trail_button = 0
 ps4_erase_trail_button = 9
+ps4_screenshot_button = 8
 
 ps4_turn_0 = 11
 ps4_turn_45 = None
 ps4_turn_90 = 14
 ps4_turn_135 = None
 ps4_turn_180 = 12
 ps4_turn_225 = None
@@ -345,14 +349,15 @@
 
 ps5_disable_button = 2
 ps5_direction_button = 3
 ps5_zero_button = 1
 ps5_head_selection_button = 10
 ps5_trail_button = 0
 ps5_erase_trail_button = 9
+ps5_screenshot_button = 11
 
 ps5_turn_0 = (0, 1)
 ps5_turn_45 = (1, 1)
 ps5_turn_90 = (1, 0)
 ps5_turn_135 = (1, -1)
 ps5_turn_180 = (0, -1)
 ps5_turn_225 = (-1, -1)
```

### Comparing `pythfinder-0.0.3.17/pythfinder/Components/Constants/constrains.py` & `pythfinder-0.0.3.18/pythfinder/Components/Constants/constrains.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Components/Constants/screenSize.py` & `pythfinder-0.0.3.18/pythfinder/Components/Constants/screenSize.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Components/Controllers/PIDCoefficients.py` & `pythfinder-0.0.3.18/pythfinder/Components/Controllers/PIDCoefficients.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Components/Controllers/PIDController.py` & `pythfinder-0.0.3.18/pythfinder/Components/Controllers/PIDController.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Components/Menu/buttons.py` & `pythfinder-0.0.3.18/pythfinder/Components/Menu/buttons.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Components/Menu/enums.py` & `pythfinder-0.0.3.18/pythfinder/Components/Menu/enums.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Components/Menu/main.py` & `pythfinder-0.0.3.18/pythfinder/Components/Menu/main.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Components/Menu/menus.py` & `pythfinder-0.0.3.18/pythfinder/Components/Menu/menus.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Components/background.py` & `pythfinder-0.0.3.18/pythfinder/Components/background.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Components/controls.py` & `pythfinder-0.0.3.18/pythfinder/Components/controls.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 
             self.disable_button = 0
             self.direction_button = 0
             self.zero_button = 0
             self.head_selection_button = 0
             self.trail_button = 0
             self.erase_trail_button = 0
+            self.screenshot_button = 0
 
             self.turn_0 = 0
             self.turn_45 = 0
             self.turn_90 = 0
             self.turn_135 = 0
             self.turn_180 = 0
             self.turn_225 = 0
@@ -80,14 +81,15 @@
 
             self.disable_button = xbox_disable_button
             self.direction_button = xbox_direction_button
             self.zero_button = xbox_zero_button
             self.head_selection_button = xbox_head_selection_button
             self.trail_button = xbox_trail_button
             self.erase_trail_button = xbox_erase_trail_button
+            self.screenshot_button = xbox_screenshot_button
 
             self.turn_0 = xbox_turn_0
             self.turn_45 = xbox_turn_45
             self.turn_90 = xbox_turn_90
             self.turn_135 = xbox_turn_135
             self.turn_180 = xbox_turn_180
             self.turn_225 = xbox_turn_225
@@ -110,14 +112,15 @@
 
             self.disable_button = ps4_disable_button
             self.direction_button = ps4_direction_button
             self.zero_button = ps4_zero_button
             self.head_selection_button = ps4_head_selection_button
             self.trail_button = ps4_trail_button
             self.erase_trail_button = ps4_erase_trail_button
+            self.screenshot_button = ps4_screenshot_button
 
             self.turn_0 = ps4_turn_0
             self.turn_45 = ps4_turn_45
             self.turn_90 = ps4_turn_90
             self.turn_135 = ps4_turn_135
             self.turn_180 = ps4_turn_180
             self.turn_225 = ps4_turn_225
@@ -135,14 +138,15 @@
 
             self.disable_button = ps5_disable_button
             self.direction_button = ps5_direction_button
             self.zero_button = ps5_zero_button
             self.head_selection_button = ps5_head_selection_button
             self.trail_button = ps5_trail_button
             self.erase_trail_button = ps5_erase_trail_button
+            self.screenshot_button = ps5_screenshot_button
 
             self.turn_0 = ps5_turn_0
             self.turn_45 = ps5_turn_45
             self.turn_90 = ps5_turn_90
             self.turn_135 = ps5_turn_135
             self.turn_180 = ps5_turn_180
             self.turn_225 = ps5_turn_225
@@ -227,26 +231,26 @@
                     return Dpad.RIGHT
 
     
     def __initKeyboardDetector(self):
         keyboard_detector = []
         key_states = pygame.key.get_pressed()
 
-        for key in key_states:
+        for _ in key_states:
             keyboard_detector.append(EdgeDetectorEx())
         
         self.keyboard_len = len(key_states)
         return keyboard_detector
     
     def __initJoystickDetector(self):
         joystick_detector = []
         if exists(self.joystick):
             self.joystick_len = self.joystick.get_numbuttons()                                                                    
 
-            for button in range(self.joystick_len):
+            for _ in range(self.joystick_len):
                 joystick_detector.append(EdgeDetectorEx())
         
         return joystick_detector
     
     def update(self):
         if self.using_joystick.compare():
             self.__updateJoystick()
```

### Comparing `pythfinder-0.0.3.17/pythfinder/Components/fade.py` & `pythfinder-0.0.3.18/pythfinder/Components/fade.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Components/robot.py` & `pythfinder-0.0.3.18/pythfinder/Components/robot.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Components/table.py` & `pythfinder-0.0.3.18/pythfinder/Components/table.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Components/trail.py` & `pythfinder-0.0.3.18/pythfinder/Components/trail.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Font/GraffitiYouth-Regular.otf` & `pythfinder-0.0.3.18/pythfinder/Font/GraffitiYouth-Regular.otf`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_backwards.png` & `pythfinder-0.0.3.18/pythfinder/Images/Controls/btn_backwards.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_forwards.png` & `pythfinder-0.0.3.18/pythfinder/Images/Controls/btn_forwards.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_hide_trail.png` & `pythfinder-0.0.3.18/pythfinder/Images/Controls/btn_hide_trail.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_selecting_off.png` & `pythfinder-0.0.3.18/pythfinder/Images/Controls/btn_selecting_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_selecting_on.png` & `pythfinder-0.0.3.18/pythfinder/Images/Controls/btn_selecting_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_show_trail.png` & `pythfinder-0.0.3.18/pythfinder/Images/Controls/btn_show_trail.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/Left/left_arrow.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/General/Arrows/Left/left_arrow.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/Left/selected_left_arrow.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/General/Arrows/Left/selected_left_arrow.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/Right/right_arrow.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/General/Arrows/Right/right_arrow.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/Right/selected_right_arrow.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/General/Arrows/Right/selected_right_arrow.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/General/general_menu.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/General/general_menu.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/menu_button.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Main/menu_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/menu_home_button.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Main/menu_home_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/menu_main.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Main/menu_main.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/selected_menu_button.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Main/selected_menu_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/selected_menu_home_button.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Main/selected_menu_home_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/DrawTable/draw_table_off.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/DrawTable/draw_table_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/DrawTable/draw_table_on.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/DrawTable/draw_table_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/DrawTable/selected_draw_table_off.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/DrawTable/selected_draw_table_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/DrawTable/selected_draw_table_on.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/DrawTable/selected_draw_table_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/FieldCentric/field_centric_off.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/FieldCentric/field_centric_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/FieldCentric/field_centric_on.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/FieldCentric/field_centric_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_off.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_on.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/RobotBorder/robot_border_off.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/RobotBorder/robot_border_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/RobotBorder/robot_border_on.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/RobotBorder/robot_border_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_off.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_on.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_off.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_on.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_off.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_on.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/other_indicator.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/other_indicator.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/other_quadrant.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Other/other_quadrant.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/height.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/height.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/robot_indicator.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/robot_indicator.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/robot_path.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/robot_path.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/robot_path_quadrant.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/robot_path_quadrant.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/robot_specs_quadrant.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/robot_specs_quadrant.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/scale.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/scale.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/selected_height.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/selected_height.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/selected_robot_path.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/selected_robot_path.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/selected_scale.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/selected_scale.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/selected_width.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/selected_width.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/width.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Robot/width.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/interface_button.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/interface_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/other_button.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/other_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/pathing_button.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/pathing_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/robot_button.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/robot_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selected_interface_button.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/selected_interface_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selected_other_button.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/selected_other_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selected_pathing_button.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/selected_pathing_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selected_robot_button.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/selected_robot_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selected_trail_button.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/selected_trail_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selection_menu.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/selection_menu.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/trail_button.png` & `pythfinder-0.0.3.18/pythfinder/Images/Menu/Selection/trail_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Robot/bot_from_above.png` & `pythfinder-0.0.3.18/pythfinder/Images/Robot/bot_from_above.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/Table/FLL_table_MP.jpg` & `pythfinder-0.0.3.18/pythfinder/Images/Table/FLL_table_MP.jpg`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/none.png` & `pythfinder-0.0.3.18/pythfinder/Images/none.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/pythfinder_logo_mk3.png` & `pythfinder-0.0.3.18/pythfinder/Images/pythfinder_logo_mk3.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Images/selected_none.png` & `pythfinder-0.0.3.18/pythfinder/Images/selected_none.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Trajectory/builder.py` & `pythfinder-0.0.3.18/pythfinder/Trajectory/builder.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Trajectory/feedback.py` & `pythfinder-0.0.3.18/pythfinder/Trajectory/feedback.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Trajectory/feedforward.py` & `pythfinder-0.0.3.18/pythfinder/Trajectory/feedforward.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Trajectory/kinematics.py` & `pythfinder-0.0.3.18/pythfinder/Trajectory/kinematics.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/Trajectory/splines.py` & `pythfinder-0.0.3.18/pythfinder/Trajectory/splines.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.17/pythfinder/core.py` & `pythfinder-0.0.3.18/pythfinder/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pythfinder.Components.background import *
 from pythfinder.Components.Menu.main import *
 from pythfinder.Components.controls import *
 from pythfinder.Components.robot import *
 from pythfinder.Components.table import *
 from pythfinder.Components.fade import *
 
-
+from datetime import datetime
 import pygame
 
 
 # file connecting all features into one big ecosystem of classes
 #
 # from the Simulator object, all different aspects of the simulator can be accessed and be modified
 #
@@ -90,14 +90,16 @@
                 self.robot.trail.draw_trail.set(False)
                 self.constants.ERASE_TRAIL.set(True)
                 self.constants.USE_SCREEN_BORDER.set(True)
 
                 print("\n\ntele-op just started! ---- ding ding 🔔")            
             case _:
                 pass
+        
+        self.menu.check()
 
 
     def recalculate(self):
         if self.constants.recalculate.compare(False):
             return 0
         
         self.screen = pygame.display.set_mode(self.constants.screen_size.get())
@@ -138,14 +140,15 @@
         self.background.onScreen(self.screen)
         self.robot.onScreen(self.screen)
         self.fade.onScreen(self.screen)
         if self.constants.MENU_ENTERED.compare():
             self.menu.addControls(self.controls)
             self.menu.onScreen(self.screen)
 
+        self.__updateScreenshoot()
         pygame.display.update()
         self.dt = self.clock.tick(self.constants.FPS) / 1000
     
 
 
     def __updateEventManager(self):
         self.menu.addKey(None)
@@ -297,11 +300,38 @@
                 elif self.controls.joystick_detector[self.controls.keybinds.turn_270].rising:
                     target = 270
             elif self.controls.keybinds.calculate(self.controls.joystick.get_hat(0)) != None:
                 target = self.controls.keybinds.calculate(self.controls.joystick.get_hat(0))
             
             self.robot.pose.head = self.robot.target_head = target
 
+    def __updateScreenshoot(self):
+        if exists(self.controls.joystick):
+            self.controls.update()
+            
+            if self.controls.joystick_detector[self.controls.keybinds.screenshot_button].rising:
+                #take a screenshot
+
+                screenshot = pygame.Surface(self.constants.screen_size.get())
+                screenshot.blit(self.screen, (0, 0))
+
+                date_and_time_info = datetime.now().strftime("%d-%m-%Y-%H-%M-%S")
+                image_name_with_time_format = "{0}.png".format(date_and_time_info)
+                individual_data = date_and_time_info.split("-")
+
+                device_screenshot_path = os.path.join(os.path.join(os.path.dirname(__file__), "Screenshots"), image_name_with_time_format)
+                pygame.image.save(screenshot, device_screenshot_path)
+
+                print("\n\nyou took a screenshot :o -- check it out:")
+
+                for each in individual_data: # easter egg? :0
+                    if each == '42' or each == '69':
+                        print("\n\nnice 😎")
+                        break
+
+                print(device_screenshot_path)
+                
+
```

### Comparing `pythfinder-0.0.3.17/pythfinder.egg-info/SOURCES.txt` & `pythfinder-0.0.3.18/pythfinder.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -100,13 +100,14 @@
 pythfinder/Images/Menu/Selection/selected_trail_button.png
 pythfinder/Images/Menu/Selection/selection_menu.png
 pythfinder/Images/Menu/Selection/trail_button.png
 pythfinder/Images/Robot/__init__.py
 pythfinder/Images/Robot/bot_from_above.png
 pythfinder/Images/Table/FLL_table_MP.jpg
 pythfinder/Images/Table/__init__.py
+pythfinder/Screenshots/__init__.py
 pythfinder/Trajectory/__init__.py
 pythfinder/Trajectory/builder.py
 pythfinder/Trajectory/feedback.py
 pythfinder/Trajectory/feedforward.py
 pythfinder/Trajectory/kinematics.py
 pythfinder/Trajectory/splines.py
```

### Comparing `pythfinder-0.0.3.17/setup.py` & `pythfinder-0.0.3.18/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pythfinder',
-    version='0.0.3.17',
+    version='0.0.3.18',
     license='MIT',
     author='Contraș Adrian',
     author_email='omegacoresincai@gmail.com',
     description='Motion Planning library designed for FLL teams',
     packages=find_packages(),
     keywords=[
         'motion-planning',
```

