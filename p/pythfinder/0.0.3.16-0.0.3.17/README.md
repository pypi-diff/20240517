# Comparing `tmp/pythfinder-0.0.3.16.tar.gz` & `tmp/pythfinder-0.0.3.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythfinder-0.0.3.16.tar", last modified: Wed May 15 18:01:35 2024, max compression
+gzip compressed data, was "pythfinder-0.0.3.17.tar", last modified: Fri May 17 15:59:32 2024, max compression
```

## Comparing `pythfinder-0.0.3.16.tar` & `pythfinder-0.0.3.17.tar`

### file list

```diff
@@ -1,139 +1,141 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.266616 pythfinder-0.0.3.16/
--rw-rw-rw-   0        0        0     1873 2024-05-15 15:31:47.000000 pythfinder-0.0.3.16/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1295 2024-05-14 05:43:57.000000 pythfinder-0.0.3.16/LICENSE.txt
--rw-rw-rw-   0        0        0      253 2024-05-15 16:24:01.000000 pythfinder-0.0.3.16/MANIFEST.in
--rw-rw-rw-   0        0        0      311 2024-05-15 18:01:35.266616 pythfinder-0.0.3.16/PKG-INFO
--rw-rw-rw-   0        0        0      344 2024-05-14 18:26:37.000000 pythfinder-0.0.3.16/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.028325 pythfinder-0.0.3.16/pythfinder/
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.066082 pythfinder-0.0.3.16/pythfinder/Components/
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.081710 pythfinder-0.0.3.16/pythfinder/Components/BetterClasses/
--rw-rw-rw-   0        0        0        0 2024-05-15 15:03:55.000000 pythfinder-0.0.3.16/pythfinder/Components/BetterClasses/__init__.py
--rw-rw-rw-   0        0        0     1168 2024-05-13 14:52:24.000000 pythfinder-0.0.3.16/pythfinder/Components/BetterClasses/booleanEx.py
--rw-rw-rw-   0        0        0      627 2024-05-13 14:52:55.000000 pythfinder-0.0.3.16/pythfinder/Components/BetterClasses/edgeDetectorEx.py
--rw-rw-rw-   0        0        0     1140 2024-05-13 15:07:55.000000 pythfinder-0.0.3.16/pythfinder/Components/BetterClasses/errorEx.py
--rw-rw-rw-   0        0        0     4862 2024-05-13 14:45:33.000000 pythfinder-0.0.3.16/pythfinder/Components/BetterClasses/mathEx.py
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.081710 pythfinder-0.0.3.16/pythfinder/Components/Constants/
--rw-rw-rw-   0        0        0        0 2024-05-15 15:03:51.000000 pythfinder-0.0.3.16/pythfinder/Components/Constants/__init__.py
--rw-rw-rw-   0        0        0    23384 2024-05-15 17:24:02.000000 pythfinder-0.0.3.16/pythfinder/Components/Constants/constants.py
--rw-rw-rw-   0        0        0     2905 2024-05-13 15:08:14.000000 pythfinder-0.0.3.16/pythfinder/Components/Constants/constrains.py
--rw-rw-rw-   0        0        0     2705 2024-05-13 15:11:03.000000 pythfinder-0.0.3.16/pythfinder/Components/Constants/screenSize.py
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.097338 pythfinder-0.0.3.16/pythfinder/Components/Controllers/
--rw-rw-rw-   0        0        0      642 2024-05-13 15:12:44.000000 pythfinder-0.0.3.16/pythfinder/Components/Controllers/PIDCoefficients.py
--rw-rw-rw-   0        0        0     1163 2024-05-14 16:07:14.000000 pythfinder-0.0.3.16/pythfinder/Components/Controllers/PIDController.py
--rw-rw-rw-   0        0        0        0 2024-05-15 15:04:30.000000 pythfinder-0.0.3.16/pythfinder/Components/Controllers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.097338 pythfinder-0.0.3.16/pythfinder/Components/Menu/
--rw-rw-rw-   0        0        0        0 2024-05-15 15:03:47.000000 pythfinder-0.0.3.16/pythfinder/Components/Menu/__init__.py
--rw-rw-rw-   0        0        0    22763 2024-05-15 17:57:13.000000 pythfinder-0.0.3.16/pythfinder/Components/Menu/buttons.py
--rw-rw-rw-   0        0        0     1581 2024-05-15 17:22:04.000000 pythfinder-0.0.3.16/pythfinder/Components/Menu/enums.py
--rw-rw-rw-   0        0        0    22669 2024-05-15 17:52:23.000000 pythfinder-0.0.3.16/pythfinder/Components/Menu/main.py
--rw-rw-rw-   0        0        0     4103 2024-05-14 16:07:01.000000 pythfinder-0.0.3.16/pythfinder/Components/Menu/menus.py
--rw-rw-rw-   0        0        0        0 2024-05-15 15:04:12.000000 pythfinder-0.0.3.16/pythfinder/Components/__init__.py
--rw-rw-rw-   0        0        0     5720 2024-05-14 16:04:43.000000 pythfinder-0.0.3.16/pythfinder/Components/background.py
--rw-rw-rw-   0        0        0     9569 2024-05-14 16:05:08.000000 pythfinder-0.0.3.16/pythfinder/Components/controls.py
--rw-rw-rw-   0        0        0     1853 2024-05-14 16:05:12.000000 pythfinder-0.0.3.16/pythfinder/Components/fade.py
--rw-rw-rw-   0        0        0     9909 2024-05-15 16:43:21.000000 pythfinder-0.0.3.16/pythfinder/Components/robot.py
--rw-rw-rw-   0        0        0     2161 2024-05-15 17:34:53.000000 pythfinder-0.0.3.16/pythfinder/Components/table.py
--rw-rw-rw-   0        0        0     4633 2024-05-14 16:05:37.000000 pythfinder-0.0.3.16/pythfinder/Components/trail.py
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.097338 pythfinder-0.0.3.16/pythfinder/Font/
--rw-rw-rw-   0        0        0    40824 2024-05-15 15:06:17.000000 pythfinder-0.0.3.16/pythfinder/Font/GraffitiYouth-Regular.otf
--rw-rw-rw-   0        0        0       30 2024-05-15 16:46:45.000000 pythfinder-0.0.3.16/pythfinder/Font/__init__.py
--rw-rw-rw-   0        0        0      334 2024-05-15 15:06:17.000000 pythfinder-0.0.3.16/pythfinder/Font/credits.txt
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.112962 pythfinder-0.0.3.16/pythfinder/Images/
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.128589 pythfinder-0.0.3.16/pythfinder/Images/Controls/
--rw-rw-rw-   0        0        0        0 2024-05-14 18:17:56.000000 pythfinder-0.0.3.16/pythfinder/Images/Controls/__init__.py
--rw-rw-rw-   0        0        0   525562 2024-03-31 07:01:14.000000 pythfinder-0.0.3.16/pythfinder/Images/Controls/btn_backwards.png
--rw-rw-rw-   0        0        0   530916 2024-03-31 07:01:10.000000 pythfinder-0.0.3.16/pythfinder/Images/Controls/btn_forwards.png
--rw-rw-rw-   0        0        0   533042 2024-03-31 07:01:19.000000 pythfinder-0.0.3.16/pythfinder/Images/Controls/btn_hide_trail.png
--rw-rw-rw-   0        0        0   561920 2024-03-31 14:58:53.000000 pythfinder-0.0.3.16/pythfinder/Images/Controls/btn_selecting_off.png
--rw-rw-rw-   0        0        0   558616 2024-03-31 14:58:49.000000 pythfinder-0.0.3.16/pythfinder/Images/Controls/btn_selecting_on.png
--rw-rw-rw-   0        0        0   531856 2024-03-31 07:00:59.000000 pythfinder-0.0.3.16/pythfinder/Images/Controls/btn_show_trail.png
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.128589 pythfinder-0.0.3.16/pythfinder/Images/Menu/
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.128589 pythfinder-0.0.3.16/pythfinder/Images/Menu/General/
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.012699 pythfinder-0.0.3.16/pythfinder/Images/Menu/General/Arrows/
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.144215 pythfinder-0.0.3.16/pythfinder/Images/Menu/General/Arrows/Left/
--rw-rw-rw-   0        0        0     5149 2024-04-07 08:30:53.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/General/Arrows/Left/left_arrow.png
--rw-rw-rw-   0        0        0     5334 2024-04-07 08:30:48.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/General/Arrows/Left/selected_left_arrow.png
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.144215 pythfinder-0.0.3.16/pythfinder/Images/Menu/General/Arrows/Right/
--rw-rw-rw-   0        0        0     5181 2024-04-07 08:31:22.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/General/Arrows/Right/right_arrow.png
--rw-rw-rw-   0        0        0     5279 2024-04-07 08:31:21.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/General/Arrows/Right/selected_right_arrow.png
--rw-rw-rw-   0        0        0        0 2024-05-14 18:18:26.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/General/__init__.py
--rw-rw-rw-   0        0        0   467492 2024-04-07 08:30:13.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/General/general_menu.png
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.159842 pythfinder-0.0.3.16/pythfinder/Images/Menu/Main/
--rw-rw-rw-   0        0        0     8011 2024-04-05 16:14:53.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Main/menu_button.png
--rw-rw-rw-   0        0        0     6208 2024-04-05 16:14:57.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Main/menu_home_button.png
--rw-rw-rw-   0        0        0  1606752 2024-04-05 16:15:02.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Main/menu_main.png
--rw-rw-rw-   0        0        0     8399 2024-04-06 11:39:50.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Main/selected_menu_button.png
--rw-rw-rw-   0        0        0     6451 2024-04-06 11:39:46.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Main/selected_menu_home_button.png
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.166348 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.166348 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/DrawTable/
--rw-rw-rw-   0        0        0    33164 2024-05-15 17:13:46.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/DrawTable/draw_table_off.png
--rw-rw-rw-   0        0        0    33397 2024-05-15 17:13:39.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/DrawTable/draw_table_on.png
--rw-rw-rw-   0        0        0    34675 2024-05-15 17:13:44.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/DrawTable/selected_draw_table_off.png
--rw-rw-rw-   0        0        0    34863 2024-05-15 17:13:48.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/DrawTable/selected_draw_table_on.png
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.181979 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/FieldCentric/
--rw-rw-rw-   0        0        0    33821 2024-04-07 08:27:04.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/FieldCentric/field_centric_off.png
--rw-rw-rw-   0        0        0    34053 2024-04-07 08:27:04.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/FieldCentric/field_centric_on.png
--rw-rw-rw-   0        0        0    35325 2024-04-07 08:27:04.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_off.png
--rw-rw-rw-   0        0        0    35522 2024-04-07 08:27:04.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_on.png
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.181979 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/RobotBorder/
--rw-rw-rw-   0        0        0    32516 2024-04-07 08:27:48.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/RobotBorder/robot_border_off.png
--rw-rw-rw-   0        0        0    32757 2024-04-07 08:27:49.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/RobotBorder/robot_border_on.png
--rw-rw-rw-   0        0        0    33964 2024-04-07 08:27:48.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_off.png
--rw-rw-rw-   0        0        0    34153 2024-04-07 08:27:48.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_on.png
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.197606 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/ScreenBorder/
--rw-rw-rw-   0        0        0    34863 2024-04-07 08:28:53.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_off.png
--rw-rw-rw-   0        0        0    35031 2024-04-07 08:28:53.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_on.png
--rw-rw-rw-   0        0        0    36547 2024-04-07 08:28:53.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_off.png
--rw-rw-rw-   0        0        0    36670 2024-04-07 08:28:53.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_on.png
--rw-rw-rw-   0        0        0    20270 2024-04-09 17:13:50.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/other_indicator.png
--rw-rw-rw-   0        0        0    13339 2024-04-07 08:29:32.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/other_quadrant.png
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.213231 pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/
--rw-rw-rw-   0        0        0    28975 2024-04-08 04:32:03.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/height.png
--rw-rw-rw-   0        0        0    20193 2024-04-08 04:32:07.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/robot_indicator.png
--rw-rw-rw-   0        0        0    39077 2024-04-08 04:32:04.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/robot_path.png
--rw-rw-rw-   0        0        0   138988 2024-04-08 04:32:10.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/robot_path_quadrant.png
--rw-rw-rw-   0        0        0   115045 2024-04-08 04:32:12.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/robot_specs_quadrant.png
--rw-rw-rw-   0        0        0    20716 2024-04-08 04:32:17.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/scale.png
--rw-rw-rw-   0        0        0    30701 2024-04-08 04:32:20.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/selected_height.png
--rw-rw-rw-   0        0        0    40956 2024-04-08 04:32:22.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/selected_robot_path.png
--rw-rw-rw-   0        0        0    21855 2024-04-08 04:32:24.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/selected_scale.png
--rw-rw-rw-   0        0        0    21917 2024-04-08 04:32:27.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/selected_width.png
--rw-rw-rw-   0        0        0    20843 2024-04-08 04:32:30.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/width.png
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.244483 pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/
--rw-rw-rw-   0        0        0    19651 2024-04-06 15:09:11.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/interface_button.png
--rw-rw-rw-   0        0        0    14899 2024-04-06 15:09:15.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/other_button.png
--rw-rw-rw-   0        0        0    20750 2024-04-06 15:09:19.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/pathing_button.png
--rw-rw-rw-   0        0        0    13645 2024-04-06 15:09:23.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/robot_button.png
--rw-rw-rw-   0        0        0    16954 2024-04-06 15:09:26.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/selected_interface_button.png
--rw-rw-rw-   0        0        0    13205 2024-04-06 15:09:28.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/selected_other_button.png
--rw-rw-rw-   0        0        0    17797 2024-04-06 15:09:31.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/selected_pathing_button.png
--rw-rw-rw-   0        0        0    12126 2024-04-06 15:09:33.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/selected_robot_button.png
--rw-rw-rw-   0        0        0    11787 2024-04-06 15:09:36.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/selected_trail_button.png
--rw-rw-rw-   0        0        0    79511 2024-04-06 15:09:38.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/selection_menu.png
--rw-rw-rw-   0        0        0    13448 2024-04-06 15:09:41.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/trail_button.png
--rw-rw-rw-   0        0        0        0 2024-05-14 18:18:10.000000 pythfinder-0.0.3.16/pythfinder/Images/Menu/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.244483 pythfinder-0.0.3.16/pythfinder/Images/Robot/
--rw-rw-rw-   0        0        0        0 2024-05-14 18:18:58.000000 pythfinder-0.0.3.16/pythfinder/Images/Robot/__init__.py
--rw-rw-rw-   0        0        0   600926 2024-03-18 18:10:12.000000 pythfinder-0.0.3.16/pythfinder/Images/Robot/bot_from_above.png
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.244483 pythfinder-0.0.3.16/pythfinder/Images/Table/
--rw-rw-rw-   0        0        0  1025907 2024-04-29 12:07:29.000000 pythfinder-0.0.3.16/pythfinder/Images/Table/FLL_table_MP.jpg
--rw-rw-rw-   0        0        0        0 2024-05-14 18:19:06.000000 pythfinder-0.0.3.16/pythfinder/Images/Table/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-14 18:17:47.000000 pythfinder-0.0.3.16/pythfinder/Images/__init__.py
--rw-rw-rw-   0        0        0    16718 2024-04-07 11:58:49.000000 pythfinder-0.0.3.16/pythfinder/Images/none.png
--rw-rw-rw-   0        0        0    17665 2024-04-07 11:58:46.000000 pythfinder-0.0.3.16/pythfinder/Images/selected_none.png
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.266616 pythfinder-0.0.3.16/pythfinder/Trajectory/
--rw-rw-rw-   0        0        0       22 2024-05-15 16:36:13.000000 pythfinder-0.0.3.16/pythfinder/Trajectory/__init__.py
--rw-rw-rw-   0        0        0    58102 2024-05-15 16:21:04.000000 pythfinder-0.0.3.16/pythfinder/Trajectory/builder.py
--rw-rw-rw-   0        0        0     1709 2024-05-14 16:06:07.000000 pythfinder-0.0.3.16/pythfinder/Trajectory/feedback.py
--rw-rw-rw-   0        0        0     4366 2024-05-14 16:06:12.000000 pythfinder-0.0.3.16/pythfinder/Trajectory/feedforward.py
--rw-rw-rw-   0        0        0     1564 2024-05-14 16:06:17.000000 pythfinder-0.0.3.16/pythfinder/Trajectory/kinematics.py
--rw-rw-rw-   0        0        0     5914 2024-05-14 16:06:21.000000 pythfinder-0.0.3.16/pythfinder/Trajectory/splines.py
--rw-rw-rw-   0        0        0       98 2024-05-15 16:36:20.000000 pythfinder-0.0.3.16/pythfinder/__init__.py
--rw-rw-rw-   0        0        0    11107 2024-05-15 16:29:34.000000 pythfinder-0.0.3.16/pythfinder/core.py
-drwxrwxrwx   0        0        0        0 2024-05-15 18:01:35.059577 pythfinder-0.0.3.16/pythfinder.egg-info/
--rw-rw-rw-   0        0        0      311 2024-05-15 18:01:34.000000 pythfinder-0.0.3.16/pythfinder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4995 2024-05-15 18:01:34.000000 pythfinder-0.0.3.16/pythfinder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 18:01:34.000000 pythfinder-0.0.3.16/pythfinder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-15 18:01:34.000000 pythfinder-0.0.3.16/pythfinder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 18:01:35.266616 pythfinder-0.0.3.16/setup.cfg
--rw-rw-rw-   0        0        0      540 2024-05-15 17:58:52.000000 pythfinder-0.0.3.16/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:32.017423 pythfinder-0.0.3.17/
+-rw-rw-rw-   0        0        0     1873 2024-05-15 15:31:47.000000 pythfinder-0.0.3.17/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1295 2024-05-14 05:43:57.000000 pythfinder-0.0.3.17/LICENSE.txt
+-rw-rw-rw-   0        0        0      253 2024-05-15 16:24:01.000000 pythfinder-0.0.3.17/MANIFEST.in
+-rw-rw-rw-   0        0        0      311 2024-05-17 15:59:32.016423 pythfinder-0.0.3.17/PKG-INFO
+-rw-rw-rw-   0        0        0    16424 2024-05-17 15:53:24.000000 pythfinder-0.0.3.17/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.744458 pythfinder-0.0.3.17/pythfinder/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.789440 pythfinder-0.0.3.17/pythfinder/Components/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.790466 pythfinder-0.0.3.17/pythfinder/Components/BetterClasses/
+-rw-rw-rw-   0        0        0        0 2024-05-15 15:03:55.000000 pythfinder-0.0.3.17/pythfinder/Components/BetterClasses/__init__.py
+-rw-rw-rw-   0        0        0     1168 2024-05-13 14:52:24.000000 pythfinder-0.0.3.17/pythfinder/Components/BetterClasses/booleanEx.py
+-rw-rw-rw-   0        0        0      627 2024-05-13 14:52:55.000000 pythfinder-0.0.3.17/pythfinder/Components/BetterClasses/edgeDetectorEx.py
+-rw-rw-rw-   0        0        0     1140 2024-05-13 15:07:55.000000 pythfinder-0.0.3.17/pythfinder/Components/BetterClasses/errorEx.py
+-rw-rw-rw-   0        0        0     4862 2024-05-13 14:45:33.000000 pythfinder-0.0.3.17/pythfinder/Components/BetterClasses/mathEx.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.806092 pythfinder-0.0.3.17/pythfinder/Components/Constants/
+-rw-rw-rw-   0        0        0        0 2024-05-15 15:03:51.000000 pythfinder-0.0.3.17/pythfinder/Components/Constants/__init__.py
+-rw-rw-rw-   0        0        0    25636 2024-05-16 18:21:09.000000 pythfinder-0.0.3.17/pythfinder/Components/Constants/constants.py
+-rw-rw-rw-   0        0        0     2905 2024-05-13 15:08:14.000000 pythfinder-0.0.3.17/pythfinder/Components/Constants/constrains.py
+-rw-rw-rw-   0        0        0     2705 2024-05-13 15:11:03.000000 pythfinder-0.0.3.17/pythfinder/Components/Constants/screenSize.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.806092 pythfinder-0.0.3.17/pythfinder/Components/Controllers/
+-rw-rw-rw-   0        0        0      642 2024-05-13 15:12:44.000000 pythfinder-0.0.3.17/pythfinder/Components/Controllers/PIDCoefficients.py
+-rw-rw-rw-   0        0        0     1163 2024-05-14 16:07:14.000000 pythfinder-0.0.3.17/pythfinder/Components/Controllers/PIDController.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 15:04:30.000000 pythfinder-0.0.3.17/pythfinder/Components/Controllers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.821718 pythfinder-0.0.3.17/pythfinder/Components/Menu/
+-rw-rw-rw-   0        0        0        0 2024-05-15 15:03:47.000000 pythfinder-0.0.3.17/pythfinder/Components/Menu/__init__.py
+-rw-rw-rw-   0        0        0    23219 2024-05-16 15:21:08.000000 pythfinder-0.0.3.17/pythfinder/Components/Menu/buttons.py
+-rw-rw-rw-   0        0        0     1581 2024-05-15 17:22:04.000000 pythfinder-0.0.3.17/pythfinder/Components/Menu/enums.py
+-rw-rw-rw-   0        0        0    22764 2024-05-16 15:15:01.000000 pythfinder-0.0.3.17/pythfinder/Components/Menu/main.py
+-rw-rw-rw-   0        0        0     4196 2024-05-16 15:14:02.000000 pythfinder-0.0.3.17/pythfinder/Components/Menu/menus.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 15:04:12.000000 pythfinder-0.0.3.17/pythfinder/Components/__init__.py
+-rw-rw-rw-   0        0        0     5720 2024-05-14 16:04:43.000000 pythfinder-0.0.3.17/pythfinder/Components/background.py
+-rw-rw-rw-   0        0        0     9569 2024-05-14 16:05:08.000000 pythfinder-0.0.3.17/pythfinder/Components/controls.py
+-rw-rw-rw-   0        0        0     1853 2024-05-14 16:05:12.000000 pythfinder-0.0.3.17/pythfinder/Components/fade.py
+-rw-rw-rw-   0        0        0     9909 2024-05-15 16:43:21.000000 pythfinder-0.0.3.17/pythfinder/Components/robot.py
+-rw-rw-rw-   0        0        0     2161 2024-05-15 17:34:53.000000 pythfinder-0.0.3.17/pythfinder/Components/table.py
+-rw-rw-rw-   0        0        0     4633 2024-05-14 16:05:37.000000 pythfinder-0.0.3.17/pythfinder/Components/trail.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.837345 pythfinder-0.0.3.17/pythfinder/Font/
+-rw-rw-rw-   0        0        0    40824 2024-05-15 15:06:17.000000 pythfinder-0.0.3.17/pythfinder/Font/GraffitiYouth-Regular.otf
+-rw-rw-rw-   0        0        0       30 2024-05-15 16:46:45.000000 pythfinder-0.0.3.17/pythfinder/Font/__init__.py
+-rw-rw-rw-   0        0        0      334 2024-05-15 15:06:17.000000 pythfinder-0.0.3.17/pythfinder/Font/credits.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.860998 pythfinder-0.0.3.17/pythfinder/Images/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.876610 pythfinder-0.0.3.17/pythfinder/Images/Controls/
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:17:56.000000 pythfinder-0.0.3.17/pythfinder/Images/Controls/__init__.py
+-rw-rw-rw-   0        0        0   525562 2024-03-31 07:01:14.000000 pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_backwards.png
+-rw-rw-rw-   0        0        0   530916 2024-03-31 07:01:10.000000 pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_forwards.png
+-rw-rw-rw-   0        0        0   533042 2024-03-31 07:01:19.000000 pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_hide_trail.png
+-rw-rw-rw-   0        0        0   561920 2024-03-31 14:58:53.000000 pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_selecting_off.png
+-rw-rw-rw-   0        0        0   558616 2024-03-31 14:58:49.000000 pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_selecting_on.png
+-rw-rw-rw-   0        0        0   531856 2024-03-31 07:00:59.000000 pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_show_trail.png
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.876610 pythfinder-0.0.3.17/pythfinder/Images/Menu/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.876610 pythfinder-0.0.3.17/pythfinder/Images/Menu/General/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.707596 pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.892237 pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/Left/
+-rw-rw-rw-   0        0        0     5149 2024-04-07 08:30:53.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/Left/left_arrow.png
+-rw-rw-rw-   0        0        0     5334 2024-04-07 08:30:48.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/Left/selected_left_arrow.png
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.892237 pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/Right/
+-rw-rw-rw-   0        0        0     5181 2024-04-07 08:31:22.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/Right/right_arrow.png
+-rw-rw-rw-   0        0        0     5279 2024-04-07 08:31:21.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/Right/selected_right_arrow.png
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:18:26.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/General/__init__.py
+-rw-rw-rw-   0        0        0   467492 2024-04-07 08:30:13.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/General/general_menu.png
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.907862 pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/
+-rw-rw-rw-   0        0        0     8011 2024-04-05 16:14:53.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/menu_button.png
+-rw-rw-rw-   0        0        0     6208 2024-04-05 16:14:57.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/menu_home_button.png
+-rw-rw-rw-   0        0        0  1606752 2024-04-05 16:15:02.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/menu_main.png
+-rw-rw-rw-   0        0        0     8399 2024-04-06 11:39:50.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/selected_menu_button.png
+-rw-rw-rw-   0        0        0     6451 2024-04-06 11:39:46.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/selected_menu_home_button.png
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.907862 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.923823 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/DrawTable/
+-rw-rw-rw-   0        0        0    33164 2024-05-15 17:13:46.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/DrawTable/draw_table_off.png
+-rw-rw-rw-   0        0        0    33397 2024-05-15 17:13:39.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/DrawTable/draw_table_on.png
+-rw-rw-rw-   0        0        0    34675 2024-05-15 17:13:44.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/DrawTable/selected_draw_table_off.png
+-rw-rw-rw-   0        0        0    34863 2024-05-15 17:13:48.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/DrawTable/selected_draw_table_on.png
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.931692 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/FieldCentric/
+-rw-rw-rw-   0        0        0    33821 2024-04-07 08:27:04.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/FieldCentric/field_centric_off.png
+-rw-rw-rw-   0        0        0    34053 2024-04-07 08:27:04.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/FieldCentric/field_centric_on.png
+-rw-rw-rw-   0        0        0    35325 2024-04-07 08:27:04.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_off.png
+-rw-rw-rw-   0        0        0    35522 2024-04-07 08:27:04.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_on.png
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.940759 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/RobotBorder/
+-rw-rw-rw-   0        0        0    32516 2024-04-07 08:27:48.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/RobotBorder/robot_border_off.png
+-rw-rw-rw-   0        0        0    32757 2024-04-07 08:27:49.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/RobotBorder/robot_border_on.png
+-rw-rw-rw-   0        0        0    33964 2024-04-07 08:27:48.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_off.png
+-rw-rw-rw-   0        0        0    34153 2024-04-07 08:27:48.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_on.png
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.949406 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/ScreenBorder/
+-rw-rw-rw-   0        0        0    34863 2024-04-07 08:28:53.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_off.png
+-rw-rw-rw-   0        0        0    35031 2024-04-07 08:28:53.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_on.png
+-rw-rw-rw-   0        0        0    36547 2024-04-07 08:28:53.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_off.png
+-rw-rw-rw-   0        0        0    36670 2024-04-07 08:28:53.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_on.png
+-rw-rw-rw-   0        0        0    20270 2024-04-09 17:13:50.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/other_indicator.png
+-rw-rw-rw-   0        0        0    13339 2024-04-07 08:29:32.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/other_quadrant.png
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.971411 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/
+-rw-rw-rw-   0        0        0    28975 2024-04-08 04:32:03.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/height.png
+-rw-rw-rw-   0        0        0    20193 2024-04-08 04:32:07.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/robot_indicator.png
+-rw-rw-rw-   0        0        0    39077 2024-04-08 04:32:04.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/robot_path.png
+-rw-rw-rw-   0        0        0   138988 2024-04-08 04:32:10.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/robot_path_quadrant.png
+-rw-rw-rw-   0        0        0   115045 2024-04-08 04:32:12.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/robot_specs_quadrant.png
+-rw-rw-rw-   0        0        0    20716 2024-04-08 04:32:17.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/scale.png
+-rw-rw-rw-   0        0        0    30701 2024-04-08 04:32:20.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/selected_height.png
+-rw-rw-rw-   0        0        0    40956 2024-04-08 04:32:22.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/selected_robot_path.png
+-rw-rw-rw-   0        0        0    21855 2024-04-08 04:32:24.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/selected_scale.png
+-rw-rw-rw-   0        0        0    21917 2024-04-08 04:32:27.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/selected_width.png
+-rw-rw-rw-   0        0        0    20843 2024-04-08 04:32:30.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/width.png
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.993416 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/
+-rw-rw-rw-   0        0        0    19651 2024-04-06 15:09:11.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/interface_button.png
+-rw-rw-rw-   0        0        0    14899 2024-04-06 15:09:15.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/other_button.png
+-rw-rw-rw-   0        0        0    20750 2024-04-06 15:09:19.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/pathing_button.png
+-rw-rw-rw-   0        0        0    13645 2024-04-06 15:09:23.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/robot_button.png
+-rw-rw-rw-   0        0        0    16954 2024-04-06 15:09:26.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selected_interface_button.png
+-rw-rw-rw-   0        0        0    13205 2024-04-06 15:09:28.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selected_other_button.png
+-rw-rw-rw-   0        0        0    17797 2024-04-06 15:09:31.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selected_pathing_button.png
+-rw-rw-rw-   0        0        0    12126 2024-04-06 15:09:33.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selected_robot_button.png
+-rw-rw-rw-   0        0        0    11787 2024-04-06 15:09:36.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selected_trail_button.png
+-rw-rw-rw-   0        0        0    79511 2024-04-06 15:09:38.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selection_menu.png
+-rw-rw-rw-   0        0        0    13448 2024-04-06 15:09:41.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/trail_button.png
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:18:10.000000 pythfinder-0.0.3.17/pythfinder/Images/Menu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.996417 pythfinder-0.0.3.17/pythfinder/Images/Robot/
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:18:58.000000 pythfinder-0.0.3.17/pythfinder/Images/Robot/__init__.py
+-rw-rw-rw-   0        0        0   600926 2024-03-18 18:10:12.000000 pythfinder-0.0.3.17/pythfinder/Images/Robot/bot_from_above.png
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:32.003418 pythfinder-0.0.3.17/pythfinder/Images/Table/
+-rw-rw-rw-   0        0        0  1025907 2024-04-29 12:07:29.000000 pythfinder-0.0.3.17/pythfinder/Images/Table/FLL_table_MP.jpg
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:19:06.000000 pythfinder-0.0.3.17/pythfinder/Images/Table/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:17:47.000000 pythfinder-0.0.3.17/pythfinder/Images/__init__.py
+-rw-rw-rw-   0        0        0    16718 2024-04-07 11:58:49.000000 pythfinder-0.0.3.17/pythfinder/Images/none.png
+-rw-rw-rw-   0        0        0  1287680 2024-05-16 15:43:35.000000 pythfinder-0.0.3.17/pythfinder/Images/pythfinder_logo_mk3.png
+-rw-rw-rw-   0        0        0    17665 2024-04-07 11:58:46.000000 pythfinder-0.0.3.17/pythfinder/Images/selected_none.png
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:32.014422 pythfinder-0.0.3.17/pythfinder/Trajectory/
+-rw-rw-rw-   0        0        0       22 2024-05-15 16:36:13.000000 pythfinder-0.0.3.17/pythfinder/Trajectory/__init__.py
+-rw-rw-rw-   0        0        0    58104 2024-05-16 15:33:26.000000 pythfinder-0.0.3.17/pythfinder/Trajectory/builder.py
+-rw-rw-rw-   0        0        0     1709 2024-05-14 16:06:07.000000 pythfinder-0.0.3.17/pythfinder/Trajectory/feedback.py
+-rw-rw-rw-   0        0        0     4366 2024-05-14 16:06:12.000000 pythfinder-0.0.3.17/pythfinder/Trajectory/feedforward.py
+-rw-rw-rw-   0        0        0     1564 2024-05-14 16:06:17.000000 pythfinder-0.0.3.17/pythfinder/Trajectory/kinematics.py
+-rw-rw-rw-   0        0        0     5914 2024-05-14 16:06:21.000000 pythfinder-0.0.3.17/pythfinder/Trajectory/splines.py
+-rw-rw-rw-   0        0        0       98 2024-05-15 16:36:20.000000 pythfinder-0.0.3.17/pythfinder/__init__.py
+-rw-rw-rw-   0        0        0    11256 2024-05-17 15:58:18.000000 pythfinder-0.0.3.17/pythfinder/core.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:59:31.776371 pythfinder-0.0.3.17/pythfinder.egg-info/
+-rw-rw-rw-   0        0        0      311 2024-05-17 15:59:31.000000 pythfinder-0.0.3.17/pythfinder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5070 2024-05-17 15:59:31.000000 pythfinder-0.0.3.17/pythfinder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 15:59:31.000000 pythfinder-0.0.3.17/pythfinder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-17 15:59:31.000000 pythfinder-0.0.3.17/pythfinder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-17 15:59:31.000000 pythfinder-0.0.3.17/pythfinder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 15:59:32.017423 pythfinder-0.0.3.17/setup.cfg
+-rw-rw-rw-   0        0        0      568 2024-05-17 15:55:18.000000 pythfinder-0.0.3.17/setup.py
```

### Comparing `pythfinder-0.0.3.16/CHANGELOG.txt` & `pythfinder-0.0.3.17/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/LICENSE.txt` & `pythfinder-0.0.3.17/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Components/BetterClasses/booleanEx.py` & `pythfinder-0.0.3.17/pythfinder/Components/BetterClasses/booleanEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Components/BetterClasses/edgeDetectorEx.py` & `pythfinder-0.0.3.17/pythfinder/Components/BetterClasses/edgeDetectorEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Components/BetterClasses/errorEx.py` & `pythfinder-0.0.3.17/pythfinder/Components/BetterClasses/errorEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Components/BetterClasses/mathEx.py` & `pythfinder-0.0.3.17/pythfinder/Components/BetterClasses/mathEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Components/Constants/constants.py` & `pythfinder-0.0.3.17/pythfinder/Components/Constants/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -81,72 +81,96 @@
     print("\n\n")
     raise Exception("FONT NOT FOUND")
 
 
 
 class Constants():
     def __init__(self, 
-                 screen_size: ScreenSize = None):
+                 pixels_to_dec: int = default_pixels_to_decimeters,
+                 fps: int = default_frame_rate,
+                 robot_img_source: str = default_robot_image_source,
+                 robot_scale: int = default_robot_scaling_factor,
+                 robot_width: int = default_robot_width_cm,
+                 robot_height: int = default_robot_height_cm,
+                 text_color = default_text_color,
+                 text_font: str = default_system_font,
+                 max_trail_len: int = default_max_trail_length,
+                 max_trail_segment_len: int = default_max_segment_length,
+                 draw_trail_threshold: int = default_drawing_trail_threshold,
+                 trail_color = default_trail_color,
+                 trail_loops: int = default_trail_loops,
+                 trail_width: int = default_trail_width,
+                 background_color = default_background_color,
+                 axis_color = default_coordinate_system_color,
+                 grid_color = default_grid_color,
+                 width_percent: int = default_width_percent,
+                 backing_distance: int = default_backing_distance,
+                 arrow_offset: int = default_positive_direction_arrow_offset,
+                 half_unit_measure_line: int = default_half_unit_measure_line,
+                 time_until_fade: int = default_time_until_fade,
+                 fade_percent: int = default_fade_percent,
+                 screen_size: ScreenSize = ScreenSize()):
         
         self.recalculate = BooleanEx(False)
 
-        self.PIXELS_2_DEC = 0
-        self.FPS = 0
+        self.PIXELS_2_DEC = pixels_to_dec
+        self.FPS = fps
 
-        self.ROBOT_IMG_NAME = 0
-        self.ROBOT_IMG_EX = 0
-        self.ROBOT_IMG_PATH = 0
-        self.ROBOT_IMG_SOURCE = 0
-
-        self.ROBOT_SCALE = 0
-        self.ROBOT_WIDTH = 0
-        self.ROBOT_HEIGHT = 0
-
-        self.TEXT_COLOR = 0
-        self.TEXT_FONT = 0
-
-        self.MAX_TRAIL_LEN = 0
-        self.MAX_TRAIL_SEGMENT_LEN = 0
-
-        self.DRAW_TRAIL_THRESHOLD = 0
-        self.TRAIL_COLOR = 0
-        self.TRAIL_LOOPS = 0
-        self.TRAIL_WIDTH = 0
-
-        self.BACKGROUND_COLOR = 0
-        self.AXIS_COLOR = 0
-        self.GRID_COLOR = 0
-
-        self.WIDTH_PERCENT = 0
-
-        self.BACKING_DISTANCE = 0
-
-        self.ARROW_OFFSET = 0
-        self.HALF_UNIT_MEASURE_LINE = 0
-
-        self.TIME_UNTIL_FADE = 0
-        self.FADE_PERCENT = 0
-
-        self.DRAW_ROBOT_BORDER = 0
-        self.FIELD_CENTRIC = 0
-        self.USE_SCREEN_BORDER = 0
-        self.MENU_ENTERED = 0
-        self.HEAD_SELECTION = 0
-        self.FORWARDS = 0
-        self.ERASE_TRAIL = 0
-        self.JOYSTICK_ENABLED = 0
-        self.FREEZE_TRAIL = 0
-        self.DRAW_TABLE = 0
-
-        self.COEFF_JOY_HEAD = 0
+        self.ROBOT_IMG_NAME = default_robot_image_name
+        self.ROBOT_IMG_EX = default_robot_image_extension
+        self.ROBOT_IMG_PATH = default_robot_image_path
+        self.ROBOT_IMG_SOURCE = robot_img_source
+
+        self.ROBOT_SCALE = robot_scale
+        self.ROBOT_WIDTH = robot_width
+        self.ROBOT_HEIGHT = robot_height
+
+        self.TEXT_COLOR = text_color
+        self.TEXT_FONT = text_font
+
+        self.MAX_TRAIL_LEN = max_trail_len
+        self.MAX_TRAIL_SEGMENT_LEN = max_trail_segment_len
+
+        self.DRAW_TRAIL_THRESHOLD = draw_trail_threshold
+        self.TRAIL_COLOR = trail_color
+        self.TRAIL_LOOPS = trail_loops
+        self.TRAIL_WIDTH = trail_width
+
+        self.BACKGROUND_COLOR = background_color
+        self.AXIS_COLOR = axis_color
+        self.GRID_COLOR = grid_color
+
+        self.WIDTH_PERCENT = width_percent
+
+        self.BACKING_DISTANCE = backing_distance
+
+        self.ARROW_OFFSET = arrow_offset
+        self.HALF_UNIT_MEASURE_LINE = half_unit_measure_line
+
+        self.TIME_UNTIL_FADE = time_until_fade
+        self.FADE_PERCENT = fade_percent
+
+        self.screen_size = screen_size
+
+        self.COEFF_JOY_HEAD = PIDCoefficients(kP = default_kP_joystick_head,
+                                              kI = default_kI_joystick_head,
+                                              kD = default_kD_joystick_head)
+
+        self.DRAW_ROBOT_BORDER = BooleanEx(default_draw_robot_border)
+        self.FIELD_CENTRIC = BooleanEx(default_field_centric)
+        self.USE_SCREEN_BORDER = BooleanEx(default_use_screen_border)
+        self.MENU_ENTERED = BooleanEx(default_menu_entered)
+        self.HEAD_SELECTION = BooleanEx(default_head_selection)
+        self.FORWARDS = BooleanEx(default_forwards)
+        self.ERASE_TRAIL = BooleanEx(default_erase_trail)
+        self.JOYSTICK_ENABLED = BooleanEx(default_joystick_enabled)
+        self.FREEZE_TRAIL = BooleanEx(default_freeze_trail)
+        self.DRAW_TABLE = BooleanEx(default_draw_table)
 
-        self.default()
 
-        if exists(screen_size):
-            self.screen_size = screen_size
 
     #resets all the values to default
     def default(self):
         self.PIXELS_2_DEC = default_pixels_to_decimeters
         self.FPS = default_frame_rate
 
         self.ROBOT_IMG_NAME = default_robot_image_name
```

### Comparing `pythfinder-0.0.3.16/pythfinder/Components/Constants/constrains.py` & `pythfinder-0.0.3.17/pythfinder/Components/Constants/constrains.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Components/Constants/screenSize.py` & `pythfinder-0.0.3.17/pythfinder/Components/Constants/screenSize.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Components/Controllers/PIDCoefficients.py` & `pythfinder-0.0.3.17/pythfinder/Components/Controllers/PIDCoefficients.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Components/Controllers/PIDController.py` & `pythfinder-0.0.3.17/pythfinder/Components/Controllers/PIDController.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Components/Menu/buttons.py` & `pythfinder-0.0.3.17/pythfinder/Components/Menu/buttons.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,18 +108,24 @@
             Dpad.RIGHT: [False, None],
             Dpad.DOWN: [False, None],
             Dpad.LEFT: [False, None]
         }
 
 
 
+    #resets button to the default value
     @abstractmethod
     def default(self, default: bool):
         ...
 
+    #checks if the current button display is matching the value it stores
+    @abstractmethod
+    def check(self):
+        ...
+
     # gets the value stored by the button
     def getType(self) -> ButtonType:
         if isinstance(self.raw_value, (int, float)):
             return ButtonType.INT
         if isinstance(self.raw_value, (bool, BooleanEx)):
             return ButtonType.BOOL
         if isinstance(self.raw_value, str):
@@ -240,14 +246,17 @@
     def default(self, default: bool):
         if not default:
             return 0
 
     def change(self):
         ...
     
+    def check(self):
+        return None
+    
     def update(self, selected, clicked: bool, value = None):
         super().update(selected, clicked, value)
 
         if selected is self.name:
             self.SELECTED.set(True)
         else: self.SELECTED.set(False)
 
@@ -280,15 +289,18 @@
         if self.go_next:
             self.go_next = False
             return self.next
         return None
     
     def change(self):
         self.go_next = True
-        
+    
+    def check(self):
+        return None
+
     def update(self, selected: Selected, clicked: bool, value = None):
         super().update(selected, clicked, value)
 
         if selected is self.name:
             if clicked:
                 self.change()
             self.SELECTED.set(True)
@@ -341,14 +353,17 @@
     
     def on(self):
         return (self.toggle, self.ON.get())
     
     def reset(self):
         self.ON.set(False)
     
+    def check(self):
+        ...
+
     def update(self, selected: Selected, clicked: bool, value=None):
         super().update(selected, clicked, value)
 
         if selected is self.name:
             if clicked:
                 self.change()
             self.SELECTED.set(True)
@@ -357,14 +372,15 @@
         self.SELECTED.update()
 
         if self.SELECTED.rising:
             self.display_title = self.selected_title
         if self.SELECTED.falling:
             self.display_title = self.title
 
+
 class InputButton(AbsButton):
     def __init__(self, 
                  name: Selected, 
                  quadrant_surface: pygame.Surface | None, 
                  title_surface: List[pygame.Surface] | pygame.Surface | None, 
                  selected_title_surface: List[pygame.Surface] | pygame.Surface | None, 
                  constants: Constants,
@@ -437,16 +453,14 @@
             self.input = '_'
             self.displayValue(self.input)
             return 0
 
         if self.input == '_':
             self.displayValue(self.raw_value)
             return 0
-        
-        before = self.raw_value
     
         match self.type:
             case InputType.DIMENSION:
                 try:
                     self.raw_value = int(self.input)
                     setattr(self.constants, self.name.name, self.raw_value)
                 except: pass
@@ -462,19 +476,21 @@
             case InputType.IMAGE_PATH:
                 try: 
                     pygame.image.load(self.input)
                     self.raw_value = self.input
                     setattr(self.constants, self.name.name, self.raw_value)
                 except: pass
         
+        self.check()
+    
+    def check(self):
         if not self.original_value == getattr(self.constants, self.name.name):
-            print(self.original_value, getattr(self.constants, self.name.name))
-
             self.original_value = getattr(self.constants, self.name.name)
             self.constants.recalculate.set(True)
+            
         self.displayValue(self.raw_value)
 
     
     def update(self, selected: Selected, clicked: bool, value = None):
         if not isinstance(self.type, InputType):
             raise Exception("please initialize {0}'s input type".format(self.name))
         super().update(selected, clicked, value)
@@ -583,25 +599,31 @@
             self.raw_value.set(self.original)
         except: self.raw_value = self.original
         finally: self.getIndex()
 
     def change(self): 
         try:
             self.raw_value.negate()
-
+        except: self.raw_value = not self.raw_value
+        finally:
+            self.check()
+    
+    def check(self):
+        try:
             if self.raw_value.compare():
                 self.index = 1
             else: self.index = 0
         except:
-            self.raw_value = not self.raw_value
             if self.raw_value:
                 self.index = 1
             else: self.index = 0
         finally:
-            self.display_title = self.selected_title[self.index]
+            if self.SELECTED.rising or self.SELECTED.high:
+                self.display_title = self.selected_title[self.index]
+            else: self.display_title = self.title[self.index]
 
     def update(self, selected, clicked: bool, value = None):
         super().update(selected, clicked, value)
         self.selected = selected
 
         if selected is self.name:
             if clicked:
```

### Comparing `pythfinder-0.0.3.16/pythfinder/Components/Menu/enums.py` & `pythfinder-0.0.3.17/pythfinder/Components/Menu/enums.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Components/Menu/main.py` & `pythfinder-0.0.3.17/pythfinder/Components/Menu/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,16 +319,20 @@
     def recalculate(self):
         self.recalculateMainMenu()
         self.recalculateRobotMenu()
         self.recalculateOtherMenu()
         self.recalculateUpperBar()
         self.recalculateSelectionMenu()
 
+    def check(self):
+        for menu in self.menus:
+            menu.check()
+    
     def update(self):
-        ...
+        return None
 
 
 
     def enable(self):
         
         for menu in self.menus: # first check in overlapping is allowed
             if self.selected in menu.name.value and (menu.always_display or menu.overlap):
```

### Comparing `pythfinder-0.0.3.16/pythfinder/Components/Menu/menus.py` & `pythfinder-0.0.3.17/pythfinder/Components/Menu/menus.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,18 @@
 
 
 
     def update(self, selected: Selected, clicked: bool, default: bool = False, value = None):
         for button in self.buttons:
             button.update(selected, clicked, value)
             button.default(default)
+    
+    def check(self):
+        for button in self.buttons:
+            button.check()
 
     def updateSelections(self, direction: Dpad | None) -> Selected:
         FINAL = None
 
         for button in self.buttons:
             move_to = button.move(direction)
```

### Comparing `pythfinder-0.0.3.16/pythfinder/Components/background.py` & `pythfinder-0.0.3.17/pythfinder/Components/background.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Components/controls.py` & `pythfinder-0.0.3.17/pythfinder/Components/controls.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Components/fade.py` & `pythfinder-0.0.3.17/pythfinder/Components/fade.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Components/robot.py` & `pythfinder-0.0.3.17/pythfinder/Components/robot.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Components/table.py` & `pythfinder-0.0.3.17/pythfinder/Components/table.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Components/trail.py` & `pythfinder-0.0.3.17/pythfinder/Components/trail.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Font/GraffitiYouth-Regular.otf` & `pythfinder-0.0.3.17/pythfinder/Font/GraffitiYouth-Regular.otf`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Controls/btn_backwards.png` & `pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_backwards.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Controls/btn_forwards.png` & `pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_forwards.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Controls/btn_hide_trail.png` & `pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_hide_trail.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Controls/btn_selecting_off.png` & `pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_selecting_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Controls/btn_selecting_on.png` & `pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_selecting_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Controls/btn_show_trail.png` & `pythfinder-0.0.3.17/pythfinder/Images/Controls/btn_show_trail.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/General/Arrows/Left/left_arrow.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/Left/left_arrow.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/General/Arrows/Left/selected_left_arrow.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/Left/selected_left_arrow.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/General/Arrows/Right/right_arrow.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/Right/right_arrow.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/General/Arrows/Right/selected_right_arrow.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/General/Arrows/Right/selected_right_arrow.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/General/general_menu.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/General/general_menu.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Main/menu_button.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/menu_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Main/menu_home_button.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/menu_home_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Main/menu_main.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/menu_main.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Main/selected_menu_button.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/selected_menu_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Main/selected_menu_home_button.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Main/selected_menu_home_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/DrawTable/draw_table_off.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/DrawTable/draw_table_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/DrawTable/draw_table_on.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/DrawTable/draw_table_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/DrawTable/selected_draw_table_off.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/DrawTable/selected_draw_table_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/DrawTable/selected_draw_table_on.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/DrawTable/selected_draw_table_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/FieldCentric/field_centric_off.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/FieldCentric/field_centric_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/FieldCentric/field_centric_on.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/FieldCentric/field_centric_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_off.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_on.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/FieldCentric/selected_field_centric_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/RobotBorder/robot_border_off.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/RobotBorder/robot_border_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/RobotBorder/robot_border_on.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/RobotBorder/robot_border_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_off.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_on.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/RobotBorder/selected_robot_border_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_off.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_on.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/ScreenBorder/screen_border_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_off.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_off.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_on.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/ScreenBorder/selected_screen_border_on.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/other_indicator.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/other_indicator.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Other/other_quadrant.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Other/other_quadrant.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/height.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/height.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/robot_indicator.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/robot_indicator.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/robot_path.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/robot_path.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/robot_path_quadrant.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/robot_path_quadrant.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/robot_specs_quadrant.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/robot_specs_quadrant.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/scale.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/scale.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/selected_height.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/selected_height.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/selected_robot_path.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/selected_robot_path.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/selected_scale.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/selected_scale.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/selected_width.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/selected_width.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Robot/width.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Robot/width.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/interface_button.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/interface_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/other_button.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/other_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/pathing_button.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/pathing_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/robot_button.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/robot_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/selected_interface_button.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selected_interface_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/selected_other_button.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selected_other_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/selected_pathing_button.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selected_pathing_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/selected_robot_button.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selected_robot_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/selected_trail_button.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selected_trail_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/selection_menu.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/selection_menu.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Menu/Selection/trail_button.png` & `pythfinder-0.0.3.17/pythfinder/Images/Menu/Selection/trail_button.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Robot/bot_from_above.png` & `pythfinder-0.0.3.17/pythfinder/Images/Robot/bot_from_above.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/Table/FLL_table_MP.jpg` & `pythfinder-0.0.3.17/pythfinder/Images/Table/FLL_table_MP.jpg`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/none.png` & `pythfinder-0.0.3.17/pythfinder/Images/none.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Images/selected_none.png` & `pythfinder-0.0.3.17/pythfinder/Images/selected_none.png`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Trajectory/builder.py` & `pythfinder-0.0.3.17/pythfinder/Trajectory/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -411,14 +411,15 @@
 
             mplt.axhline(0, color = 'white', linewidth = 0.5)
             q_index += 1
 
 
         mplt.subplots_adjust(wspace = 0.15, hspace = 0.4) 
         mplt.tight_layout()
+
         mplt.show()
 
 
     def __getDerivative(self, t: List[int], vel: List[float]):
         if len(vel) > 1:
             dt = (t[-1] - t[-2]) / 1000 #ms to s
             dv = vel[-1] - vel[-2]
```

### Comparing `pythfinder-0.0.3.16/pythfinder/Trajectory/feedback.py` & `pythfinder-0.0.3.17/pythfinder/Trajectory/feedback.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Trajectory/feedforward.py` & `pythfinder-0.0.3.17/pythfinder/Trajectory/feedforward.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Trajectory/kinematics.py` & `pythfinder-0.0.3.17/pythfinder/Trajectory/kinematics.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/Trajectory/splines.py` & `pythfinder-0.0.3.17/pythfinder/Trajectory/splines.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.16/pythfinder/core.py` & `pythfinder-0.0.3.17/pythfinder/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 
 class Auto(Enum):
     ENTER = auto()
     EXIT = auto()
 
 
 class Simulator():
-    def __init__(self):
+    def __init__(self, constants: Constants = Constants()):
         pygame.init()
         pygame.display.set_caption("FLL PythFinder simulator")
         self.running = BooleanEx(True)
         self.manual_control = BooleanEx(True)
 
-        self.constants = Constants()
+        self.constants = constants
         self.clock = pygame.time.Clock()
         self.screen = pygame.display.set_mode(self.constants.screen_size.get())
 
         self.dt = 0
 
         self.background = Background(self.constants)
         self.table = Table(self.constants)
@@ -72,27 +72,30 @@
     def chooseJoystickEnabled(self, fun: Fun, bool = None):
         self.constants.JOYSTICK_ENABLED.choose(fun, bool)
 
 
     def autonomus(self, do: Auto):
         match do:
             case Auto.ENTER:
+                print("\n\nentering autonomus... ready?")
+
                 self.robot.trail.draw_trail.set(True)
                 self.constants.ERASE_TRAIL.set(False)
                 self.manual_control.set(False)
                 self.constants.USE_SCREEN_BORDER.set(False)
                 self.constants.DRAW_TABLE.set(True)
 
                 self.robot.zeroDistance()
             case Auto.EXIT:
                 self.manual_control.set(True)
                 self.robot.trail.draw_trail.set(False)
                 self.constants.ERASE_TRAIL.set(True)
                 self.constants.USE_SCREEN_BORDER.set(True)
-                #self.constants.DRAW_TABLE.set(False)
+
+                print("\n\ntele-op just started! ---- ding ding 🔔")            
             case _:
                 pass
 
 
     def recalculate(self):
         if self.constants.recalculate.compare(False):
             return 0
@@ -100,14 +103,15 @@
         self.screen = pygame.display.set_mode(self.constants.screen_size.get())
         self.menu.recalculate()
         self.fade.recalculate()
         self.robot.recalculate()
         self.table.recalculate()
         self.background.recalculate()
 
+        self.menu.check()
         self.constants.recalculate.set(False)
 
 
     def matchScreenSize(self, image: pygame.Surface, width):
         size_multiplier = self.constants.WIDTH_PERCENT / 100 * width / self.constants.screen_size.MAX_WIDTH
 
         return pygame.transform.scale(image,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pythfinder-0.0.3.16/pythfinder.egg-info/SOURCES.txt` & `pythfinder-0.0.3.17/pythfinder.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 README.md
 setup.py
 pythfinder/__init__.py
 pythfinder/core.py
 pythfinder.egg-info/PKG-INFO
 pythfinder.egg-info/SOURCES.txt
 pythfinder.egg-info/dependency_links.txt
+pythfinder.egg-info/requires.txt
 pythfinder.egg-info/top_level.txt
 pythfinder/Components/__init__.py
 pythfinder/Components/background.py
 pythfinder/Components/controls.py
 pythfinder/Components/fade.py
 pythfinder/Components/robot.py
 pythfinder/Components/table.py
@@ -34,14 +35,15 @@
 pythfinder/Components/Menu/main.py
 pythfinder/Components/Menu/menus.py
 pythfinder/Font/GraffitiYouth-Regular.otf
 pythfinder/Font/__init__.py
 pythfinder/Font/credits.txt
 pythfinder/Images/__init__.py
 pythfinder/Images/none.png
+pythfinder/Images/pythfinder_logo_mk3.png
 pythfinder/Images/selected_none.png
 pythfinder/Images/Controls/__init__.py
 pythfinder/Images/Controls/btn_backwards.png
 pythfinder/Images/Controls/btn_forwards.png
 pythfinder/Images/Controls/btn_hide_trail.png
 pythfinder/Images/Controls/btn_selecting_off.png
 pythfinder/Images/Controls/btn_selecting_on.png
```

