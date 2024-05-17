# Comparing `tmp/jdTextEdit-9.0.tar.gz` & `tmp/jdTextEdit-9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdTextEdit-9.0.tar", last modified: Fri Jul 16 12:34:27 2021, max compression
+gzip compressed data, was "jdTextEdit-9.1.tar", last modified: Thu Jul 22 13:49:23 2021, max compression
```

## Comparing `jdTextEdit-9.0.tar` & `jdTextEdit-9.1.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 12:34:27.000000 jdTextEdit-9.0/
--rw-rw-rw-   0 root         (0) root         (0)    35077 2021-07-16 12:34:10.000000 jdTextEdit-9.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      281 2021-07-16 12:34:10.000000 jdTextEdit-9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2940 2021-07-16 12:34:27.000000 jdTextEdit-9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1144 2021-07-16 12:34:10.000000 jdTextEdit-9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit/
--rw-rw-rw-   0 root         (0) root         (0)      353 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/AutocompleteXML.py
--rw-rw-rw-   0 root         (0) root         (0)      920 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/EncodingList.py
--rw-rw-rw-   0 root         (0) root         (0)     8028 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/Enviroment.py
--rw-rw-rw-   0 root         (0) root         (0)     8121 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/Functions.py
--rw-rw-rw-   0 root         (0) root         (0)     4394 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/LexerList.py
--rw-rw-rw-   0 root         (0) root         (0)   151924 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/Logo.png
--rw-rw-rw-   0 root         (0) root         (0)     7174 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/Settings.py
--rw-rw-rw-   0 root         (0) root         (0)     3177 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/Updater.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit/api/
--rw-rw-rw-   0 root         (0) root         (0)     1442 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/api/LanguageBase.py
--rw-rw-rw-   0 root         (0) root         (0)      275 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/api/SettingsTabBase.py
--rw-rw-rw-   0 root         (0) root         (0)      327 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/api/SidebarWidgetBase.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/api/SignalBase.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/api/ThemeBase.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit/autocompletion/
--rw-rw-rw-   0 root         (0) root         (0)     3784 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/autocompletion/batch.xml
--rw-rw-rw-   0 root         (0) root         (0)     7891 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/autocompletion/cmake.xml
--rw-rw-rw-   0 root         (0) root         (0)     1510 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/autocompletion/coffee.xml
--rw-rw-rw-   0 root         (0) root         (0)    61530 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/autocompletion/cpp.xml
--rw-rw-rw-   0 root         (0) root         (0)    33726 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/autocompletion/cs.xml
--rw-rw-rw-   0 root         (0) root         (0)    11522 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/autocompletion/css.xml
--rw-rw-rw-   0 root         (0) root         (0)    19497 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/autocompletion/html.xml
--rw-rw-rw-   0 root         (0) root         (0)   205366 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/autocompletion/java.xml
--rw-rw-rw-   0 root         (0) root         (0)    23318 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/autocompletion/javascript.xml
--rw-rw-rw-   0 root         (0) root         (0)    90490 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/autocompletion/lua.xml
--rw-rw-rw-   0 root         (0) root         (0)    14269 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/autocompletion/perl.xml
--rw-rw-rw-   0 root         (0) root         (0)    61585 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/autocompletion/python.xml
--rw-rw-rw-   0 root         (0) root         (0)    67871 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/autocompletion/tex.xml
--rw-rw-rw-   0 root         (0) root         (0)     2632 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/autocompletion/vhdl.xml
--rw-rw-rw-   0 root         (0) root         (0)    12024 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/autocompletion/xml.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit/core/
--rw-rw-rw-   0 root         (0) root         (0)      931 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/core/BuiltinLanguage.py
--rw-rw-rw-   0 root         (0) root         (0)     1280 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/core/DefaultTheme.py
--rw-rw-rw-   0 root         (0) root         (0)     2522 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/core/FileTheme.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit/core/api/
--rw-rw-rw-   0 root         (0) root         (0)      146 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/core/api/ApplicationSignals.py
--rw-rw-rw-   0 root         (0) root         (0)      556 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/core/api/EditorSignals.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/core/api/MainWindowSignals.py
--rw-rw-rw-   0 root         (0) root         (0)     2001 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/core/api/PluginAPI.py
--rw-rw-rw-   0 root         (0) root         (0)      177 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/core/api/TabWidgetSignals.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/core/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit/gui/
--rw-rw-rw-   0 root         (0) root         (0)     2257 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/AboutWindow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit/gui/BannerWidgets/
--rw-rw-rw-   0 root         (0) root         (0)      540 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/BannerWidgets/BigFileBanner.py
--rw-rw-rw-   0 root         (0) root         (0)      526 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/BannerWidgets/EditorconfigBanner.py
--rw-rw-rw-   0 root         (0) root         (0)      930 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/BannerWidgets/FileChangedBanner.py
--rw-rw-rw-   0 root         (0) root         (0)      782 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/BannerWidgets/FileDeletedBanner.py
--rw-rw-rw-   0 root         (0) root         (0)      957 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/BannerWidgets/WrongEncodingBanner.py
--rw-rw-rw-   0 root         (0) root         (0)     1180 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/BannerWidgets/WrongEolBanner.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/BannerWidgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2457 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/CloseSaveWindow.py
--rw-rw-rw-   0 root         (0) root         (0)    20109 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/CodeEdit.py
--rw-rw-rw-   0 root         (0) root         (0)     4481 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/DateTimeWindow.py
--rw-rw-rw-   0 root         (0) root         (0)     1911 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/DayTipWindow.py
--rw-rw-rw-   0 root         (0) root         (0)     1386 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/DockWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     3638 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/DocumentStatistics.py
--rw-rw-rw-   0 root         (0) root         (0)     4559 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/EditCommandsWindow.py
--rw-rw-rw-   0 root         (0) root         (0)     3425 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/EditContainer.py
--rw-rw-rw-   0 root         (0) root         (0)     6446 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/EditTabWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     2061 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/ExecuteCommandWindow.py
--rw-rw-rw-   0 root         (0) root         (0)     1498 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/GotoLineWindow.py
--rw-rw-rw-   0 root         (0) root         (0)    76336 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/MainWindow.py
--rw-rw-rw-   0 root         (0) root         (0)     3741 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/ManageMacrosWindow.py
--rw-rw-rw-   0 root         (0) root         (0)     2082 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SearchAndReplaceWindow.py
--rw-rw-rw-   0 root         (0) root         (0)     1366 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SearchBar.py
--rw-rw-rw-   0 root         (0) root         (0)     4223 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SearchWindow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/
--rw-rw-rw-   0 root         (0) root         (0)     3245 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/AutocompletionTab.py
--rw-rw-rw-   0 root         (0) root         (0)     3385 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/BigFilesTab.py
--rw-rw-rw-   0 root         (0) root         (0)     4471 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/ContextMenuTab.py
--rw-rw-rw-   0 root         (0) root         (0)     4645 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/EditorTab.py
--rw-rw-rw-   0 root         (0) root         (0)     3189 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/EditorconfigTab.py
--rw-rw-rw-   0 root         (0) root         (0)     4827 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/GeneralTab.py
--rw-rw-rw-   0 root         (0) root         (0)     2727 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/InterfaceTab.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/OpenTab.py
--rw-rw-rw-   0 root         (0) root         (0)     3805 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/PathsTab.py
--rw-rw-rw-   0 root         (0) root         (0)     2496 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/PluginTab.py
--rw-rw-rw-   0 root         (0) root         (0)     3523 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/SaveTab.py
--rw-rw-rw-   0 root         (0) root         (0)     2645 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/ShortcutTab.py
--rw-rw-rw-   0 root         (0) root         (0)     5931 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/StyleTab.py
--rw-rw-rw-   0 root         (0) root         (0)     2863 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/TabBarTab.py
--rw-rw-rw-   0 root         (0) root         (0)     6397 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/ToolbarTab.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4792 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SettingsWindow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit/gui/SidebarWidgets/
--rw-rw-rw-   0 root         (0) root         (0)     1328 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SidebarWidgets/CharacterMapWidget.py
--rw-rw-rw-   0 root         (0) root         (0)      785 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SidebarWidgets/ClipboardWidget.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SidebarWidgets/FileTreeWidget.py
--rw-rw-rw-   0 root         (0) root         (0)      451 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SidebarWidgets/NotesWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SidebarWidgets/TabListWidget.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SidebarWidgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4488 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/SplitViewWidget.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/gui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit/icons/
--rw-rw-rw-   0 root         (0) root         (0)      764 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/application-exit.png
--rw-rw-rw-   0 root         (0) root         (0)      498 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/document-close-all.png
--rw-rw-rw-   0 root         (0) root         (0)      446 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/document-close.png
--rw-rw-rw-   0 root         (0) root         (0)      325 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/document-new.png
--rw-rw-rw-   0 root         (0) root         (0)      799 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/document-open-recent.png
--rw-rw-rw-   0 root         (0) root         (0)      751 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/document-open.png
--rw-rw-rw-   0 root         (0) root         (0)      662 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/document-print.png
--rw-rw-rw-   0 root         (0) root         (0)      815 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/document-save-all.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/document-save-as.png
--rw-rw-rw-   0 root         (0) root         (0)      589 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/document-save.png
--rw-rw-rw-   0 root         (0) root         (0)      344 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/document-saved.png
--rw-rw-rw-   0 root         (0) root         (0)      377 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/document-unsaved.png
--rw-rw-rw-   0 root         (0) root         (0)      623 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/edit-copy.png
--rw-rw-rw-   0 root         (0) root         (0)      777 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/edit-cut.png
--rw-rw-rw-   0 root         (0) root         (0)      830 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/edit-delete.png
--rw-rw-rw-   0 root         (0) root         (0)      985 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/edit-find-replace.png
--rw-rw-rw-   0 root         (0) root         (0)      875 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/edit-find.png
--rw-rw-rw-   0 root         (0) root         (0)      795 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/edit-paste.png
--rw-rw-rw-   0 root         (0) root         (0)      770 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/edit-redo.png
--rw-rw-rw-   0 root         (0) root         (0)      598 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/edit-select-all.png
--rw-rw-rw-   0 root         (0) root         (0)      798 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/edit-undo.png
--rw-rw-rw-   0 root         (0) root         (0)      633 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/folder-open.png
--rw-rw-rw-   0 root         (0) root         (0)      234 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/go-next.png
--rw-rw-rw-   0 root         (0) root         (0)      250 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/go-previous.png
--rw-rw-rw-   0 root         (0) root         (0)      919 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/preferences-other.png
--rw-rw-rw-   0 root         (0) root         (0)      430 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/window-close.png
--rw-rw-rw-   0 root         (0) root         (0)      367 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/word-wrap.png
--rw-rw-rw-   0 root         (0) root         (0)      701 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/zoom-in.png
--rw-rw-rw-   0 root         (0) root         (0)      763 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/zoom-original.png
--rw-rw-rw-   0 root         (0) root         (0)      722 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/icons/zoom-out.png
--rw-rw-rw-   0 root         (0) root         (0)     3781 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/jdTextEdit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit/plugins/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit/plugins/SpellChecker/
--rw-rw-rw-   0 root         (0) root         (0)     5580 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/plugins/SpellChecker/SpellChecker.py
--rw-rw-rw-   0 root         (0) root         (0)     3723 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/plugins/SpellChecker/SpellCheckingTab.py
--rw-rw-rw-   0 root         (0) root         (0)     1746 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/plugins/SpellChecker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit/plugins/SpellChecker/translation/
--rw-rw-rw-   0 root         (0) root         (0)      691 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/plugins/SpellChecker/translation/de_DE.lang
--rw-rw-rw-   0 root         (0) root         (0)      590 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/plugins/SpellChecker/translation/en_GB.lang
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/plugins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit/plugins/pluginmanager/
--rw-rw-rw-   0 root         (0) root         (0)     6134 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/plugins/pluginmanager/PluginManagerWindow.py
--rw-rw-rw-   0 root         (0) root         (0)      748 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/plugins/pluginmanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit/plugins/pluginmanager/translation/
--rw-rw-rw-   0 root         (0) root         (0)     1361 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/plugins/pluginmanager/translation/de_DE.lang
--rw-rw-rw-   0 root         (0) root         (0)     1191 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/plugins/pluginmanager/translation/en_GB.lang
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit/templates/
--rw-rw-rw-   0 root         (0) root         (0)      162 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/templates/BasicSite.html
--rw-rw-rw-   0 root         (0) root         (0)      128 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/templates/HelloWorld.cpp
--rw-rw-rw-   0 root         (0) root         (0)      124 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/templates/HelloWorld.java
--rw-rw-rw-   0 root         (0) root         (0)      256 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/templates/PyQt.py
--rw-rw-rw-   0 root         (0) root         (0)      191 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/templates/jdTextEditPlugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit/translation/
--rw-rw-rw-   0 root         (0) root         (0)    22990 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/translation/de_DE.lang
--rw-rw-rw-   0 root         (0) root         (0)    21000 2021-07-16 12:34:10.000000 jdTextEdit-9.0/jdTextEdit/translation/en_GB.lang
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2940 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5282 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      191 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2021-07-16 12:34:27.000000 jdTextEdit-9.0/jdTextEdit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-07-16 12:34:27.000000 jdTextEdit-9.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2363 2021-07-16 12:34:10.000000 jdTextEdit-9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:49:23.754870 jdTextEdit-9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35077 2021-07-22 13:49:06.000000 jdTextEdit-9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      281 2021-07-22 13:49:06.000000 jdTextEdit-9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2940 2021-07-22 13:49:23.754870 jdTextEdit-9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1144 2021-07-22 13:49:06.000000 jdTextEdit-9.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:49:23.707866 jdTextEdit-9.1/jdTextEdit/
+-rw-rw-rw-   0 root         (0) root         (0)      353 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/AutocompleteXML.py
+-rw-rw-rw-   0 root         (0) root         (0)      920 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/EncodingList.py
+-rw-rw-rw-   0 root         (0) root         (0)     8028 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/Enviroment.py
+-rw-rw-rw-   0 root         (0) root         (0)     8121 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/Functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4394 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/LexerList.py
+-rw-rw-rw-   0 root         (0) root         (0)   151924 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/Logo.png
+-rw-rw-rw-   0 root         (0) root         (0)     7174 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/Settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     3177 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/Updater.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:49:23.711867 jdTextEdit-9.1/jdTextEdit/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1442 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/api/LanguageBase.py
+-rw-rw-rw-   0 root         (0) root         (0)      275 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/api/SettingsTabBase.py
+-rw-rw-rw-   0 root         (0) root         (0)      327 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/api/SidebarWidgetBase.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/api/SignalBase.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/api/ThemeBase.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:49:23.717867 jdTextEdit-9.1/jdTextEdit/autocompletion/
+-rw-rw-rw-   0 root         (0) root         (0)     3784 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/autocompletion/batch.xml
+-rw-rw-rw-   0 root         (0) root         (0)     7891 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/autocompletion/cmake.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/autocompletion/coffee.xml
+-rw-rw-rw-   0 root         (0) root         (0)    61530 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/autocompletion/cpp.xml
+-rw-rw-rw-   0 root         (0) root         (0)    33726 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/autocompletion/cs.xml
+-rw-rw-rw-   0 root         (0) root         (0)    11522 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/autocompletion/css.xml
+-rw-rw-rw-   0 root         (0) root         (0)    19497 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/autocompletion/html.xml
+-rw-rw-rw-   0 root         (0) root         (0)   205366 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/autocompletion/java.xml
+-rw-rw-rw-   0 root         (0) root         (0)    23318 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/autocompletion/javascript.xml
+-rw-rw-rw-   0 root         (0) root         (0)    90490 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/autocompletion/lua.xml
+-rw-rw-rw-   0 root         (0) root         (0)    14269 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/autocompletion/perl.xml
+-rw-rw-rw-   0 root         (0) root         (0)    61585 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/autocompletion/python.xml
+-rw-rw-rw-   0 root         (0) root         (0)    67871 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/autocompletion/tex.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2632 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/autocompletion/vhdl.xml
+-rw-rw-rw-   0 root         (0) root         (0)    12024 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/autocompletion/xml.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:49:23.719867 jdTextEdit-9.1/jdTextEdit/core/
+-rw-rw-rw-   0 root         (0) root         (0)      931 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/core/BuiltinLanguage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1280 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/core/DefaultTheme.py
+-rw-rw-rw-   0 root         (0) root         (0)     2522 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/core/FileTheme.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:49:23.721867 jdTextEdit-9.1/jdTextEdit/core/api/
+-rw-rw-rw-   0 root         (0) root         (0)      146 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/core/api/ApplicationSignals.py
+-rw-rw-rw-   0 root         (0) root         (0)      556 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/core/api/EditorSignals.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/core/api/MainWindowSignals.py
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/core/api/PluginAPI.py
+-rw-rw-rw-   0 root         (0) root         (0)      177 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/core/api/TabWidgetSignals.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/core/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:49:23.728868 jdTextEdit-9.1/jdTextEdit/gui/
+-rw-rw-rw-   0 root         (0) root         (0)     2257 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/AboutWindow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:49:23.731868 jdTextEdit-9.1/jdTextEdit/gui/BannerWidgets/
+-rw-rw-rw-   0 root         (0) root         (0)      540 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/BannerWidgets/BigFileBanner.py
+-rw-rw-rw-   0 root         (0) root         (0)      526 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/BannerWidgets/EditorconfigBanner.py
+-rw-rw-rw-   0 root         (0) root         (0)      930 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/BannerWidgets/FileChangedBanner.py
+-rw-rw-rw-   0 root         (0) root         (0)      782 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/BannerWidgets/FileDeletedBanner.py
+-rw-rw-rw-   0 root         (0) root         (0)      957 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/BannerWidgets/WrongEncodingBanner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/BannerWidgets/WrongEolBanner.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/BannerWidgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2457 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/CloseSaveWindow.py
+-rw-rw-rw-   0 root         (0) root         (0)    20109 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/CodeEdit.py
+-rw-rw-rw-   0 root         (0) root         (0)     4481 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/DateTimeWindow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/DayTipWindow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/DockWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     3638 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/DocumentStatistics.py
+-rw-rw-rw-   0 root         (0) root         (0)     4559 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/EditCommandsWindow.py
+-rw-rw-rw-   0 root         (0) root         (0)     3425 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/EditContainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6446 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/EditTabWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/ExecuteCommandWindow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1498 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/GotoLineWindow.py
+-rw-rw-rw-   0 root         (0) root         (0)    76336 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/MainWindow.py
+-rw-rw-rw-   0 root         (0) root         (0)     3741 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/ManageMacrosWindow.py
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SearchAndReplaceWindow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SearchBar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4223 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SearchWindow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:49:23.736868 jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/
+-rw-rw-rw-   0 root         (0) root         (0)     3245 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/AutocompletionTab.py
+-rw-rw-rw-   0 root         (0) root         (0)     3385 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/BigFilesTab.py
+-rw-rw-rw-   0 root         (0) root         (0)     4471 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/ContextMenuTab.py
+-rw-rw-rw-   0 root         (0) root         (0)     4645 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/EditorTab.py
+-rw-rw-rw-   0 root         (0) root         (0)     3189 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/EditorconfigTab.py
+-rw-rw-rw-   0 root         (0) root         (0)     4827 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/GeneralTab.py
+-rw-rw-rw-   0 root         (0) root         (0)     2727 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/InterfaceTab.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/OpenTab.py
+-rw-rw-rw-   0 root         (0) root         (0)     3805 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/PathsTab.py
+-rw-rw-rw-   0 root         (0) root         (0)     2496 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/PluginTab.py
+-rw-rw-rw-   0 root         (0) root         (0)     3523 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/SaveTab.py
+-rw-rw-rw-   0 root         (0) root         (0)     2645 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/ShortcutTab.py
+-rw-rw-rw-   0 root         (0) root         (0)     5931 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/StyleTab.py
+-rw-rw-rw-   0 root         (0) root         (0)     2863 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/TabBarTab.py
+-rw-rw-rw-   0 root         (0) root         (0)     6397 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/ToolbarTab.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4792 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SettingsWindow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:49:23.738869 jdTextEdit-9.1/jdTextEdit/gui/SidebarWidgets/
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SidebarWidgets/CharacterMapWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)      785 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SidebarWidgets/ClipboardWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)      780 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SidebarWidgets/FileTreeWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)      451 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SidebarWidgets/NotesWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SidebarWidgets/TabListWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SidebarWidgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4541 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/SplitViewWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/gui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:49:23.748870 jdTextEdit-9.1/jdTextEdit/icons/
+-rw-rw-rw-   0 root         (0) root         (0)      764 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/application-exit.png
+-rw-rw-rw-   0 root         (0) root         (0)      498 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/document-close-all.png
+-rw-rw-rw-   0 root         (0) root         (0)      446 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/document-close.png
+-rw-rw-rw-   0 root         (0) root         (0)      325 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/document-new.png
+-rw-rw-rw-   0 root         (0) root         (0)      799 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/document-open-recent.png
+-rw-rw-rw-   0 root         (0) root         (0)      751 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/document-open.png
+-rw-rw-rw-   0 root         (0) root         (0)      662 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/document-print.png
+-rw-rw-rw-   0 root         (0) root         (0)      815 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/document-save-all.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/document-save-as.png
+-rw-rw-rw-   0 root         (0) root         (0)      589 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/document-save.png
+-rw-rw-rw-   0 root         (0) root         (0)      344 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/document-saved.png
+-rw-rw-rw-   0 root         (0) root         (0)      377 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/document-unsaved.png
+-rw-rw-rw-   0 root         (0) root         (0)      623 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/edit-copy.png
+-rw-rw-rw-   0 root         (0) root         (0)      777 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/edit-cut.png
+-rw-rw-rw-   0 root         (0) root         (0)      830 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/edit-delete.png
+-rw-rw-rw-   0 root         (0) root         (0)      985 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/edit-find-replace.png
+-rw-rw-rw-   0 root         (0) root         (0)      875 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/edit-find.png
+-rw-rw-rw-   0 root         (0) root         (0)      795 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/edit-paste.png
+-rw-rw-rw-   0 root         (0) root         (0)      770 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/edit-redo.png
+-rw-rw-rw-   0 root         (0) root         (0)      598 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/edit-select-all.png
+-rw-rw-rw-   0 root         (0) root         (0)      798 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/edit-undo.png
+-rw-rw-rw-   0 root         (0) root         (0)      633 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/folder-open.png
+-rw-rw-rw-   0 root         (0) root         (0)      234 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/go-next.png
+-rw-rw-rw-   0 root         (0) root         (0)      250 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/go-previous.png
+-rw-rw-rw-   0 root         (0) root         (0)      919 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/preferences-other.png
+-rw-rw-rw-   0 root         (0) root         (0)      430 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/window-close.png
+-rw-rw-rw-   0 root         (0) root         (0)      367 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/word-wrap.png
+-rw-rw-rw-   0 root         (0) root         (0)      701 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/zoom-in.png
+-rw-rw-rw-   0 root         (0) root         (0)      763 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/zoom-original.png
+-rw-rw-rw-   0 root         (0) root         (0)      722 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/icons/zoom-out.png
+-rw-rw-rw-   0 root         (0) root         (0)     3781 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/jdTextEdit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:49:23.749870 jdTextEdit-9.1/jdTextEdit/plugins/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:49:23.750870 jdTextEdit-9.1/jdTextEdit/plugins/SpellChecker/
+-rw-rw-rw-   0 root         (0) root         (0)     5580 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/plugins/SpellChecker/SpellChecker.py
+-rw-rw-rw-   0 root         (0) root         (0)     3723 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/plugins/SpellChecker/SpellCheckingTab.py
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/plugins/SpellChecker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:49:23.750870 jdTextEdit-9.1/jdTextEdit/plugins/SpellChecker/translation/
+-rw-rw-rw-   0 root         (0) root         (0)      691 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/plugins/SpellChecker/translation/de_DE.lang
+-rw-rw-rw-   0 root         (0) root         (0)      590 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/plugins/SpellChecker/translation/en_GB.lang
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/plugins/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:49:23.751870 jdTextEdit-9.1/jdTextEdit/plugins/pluginmanager/
+-rw-rw-rw-   0 root         (0) root         (0)     6134 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/plugins/pluginmanager/PluginManagerWindow.py
+-rw-rw-rw-   0 root         (0) root         (0)      748 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/plugins/pluginmanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:49:23.752870 jdTextEdit-9.1/jdTextEdit/plugins/pluginmanager/translation/
+-rw-rw-rw-   0 root         (0) root         (0)     1361 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/plugins/pluginmanager/translation/de_DE.lang
+-rw-rw-rw-   0 root         (0) root         (0)     1191 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/plugins/pluginmanager/translation/en_GB.lang
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:49:23.753870 jdTextEdit-9.1/jdTextEdit/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      162 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/templates/BasicSite.html
+-rw-rw-rw-   0 root         (0) root         (0)      128 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/templates/HelloWorld.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      124 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/templates/HelloWorld.java
+-rw-rw-rw-   0 root         (0) root         (0)      256 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/templates/PyQt.py
+-rw-rw-rw-   0 root         (0) root         (0)      191 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/templates/jdTextEditPlugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:49:23.754870 jdTextEdit-9.1/jdTextEdit/translation/
+-rw-rw-rw-   0 root         (0) root         (0)    22990 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/translation/de_DE.lang
+-rw-rw-rw-   0 root         (0) root         (0)    21000 2021-07-22 13:49:06.000000 jdTextEdit-9.1/jdTextEdit/translation/en_GB.lang
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-22 13:49:23.709867 jdTextEdit-9.1/jdTextEdit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2940 2021-07-22 13:49:23.000000 jdTextEdit-9.1/jdTextEdit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5282 2021-07-22 13:49:23.000000 jdTextEdit-9.1/jdTextEdit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-07-22 13:49:23.000000 jdTextEdit-9.1/jdTextEdit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2021-07-22 13:49:23.000000 jdTextEdit-9.1/jdTextEdit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      191 2021-07-22 13:49:23.000000 jdTextEdit-9.1/jdTextEdit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2021-07-22 13:49:23.000000 jdTextEdit-9.1/jdTextEdit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-07-22 13:49:23.755870 jdTextEdit-9.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2363 2021-07-22 13:49:06.000000 jdTextEdit-9.1/setup.py
```

### Comparing `jdTextEdit-9.0/LICENSE` & `jdTextEdit-9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/PKG-INFO` & `jdTextEdit-9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdTextEdit
-Version: 9.0
+Version: 9.1
 Summary:  A powerful texteditor with a lot of features
 Home-page: https://gitlab.com/JakobDev/jdTextEdit
 Author: JakobDev
 Author-email: jakobdev@gmx.de
 License: GPL v3
 Download-URL: https://gitlab.com/JakobDev/jdTextEdit/-/releases
 Project-URL: Issue tracker, https://gitlab.com/JakobDev/jdTextEdit/-/issues
```

### Comparing `jdTextEdit-9.0/README.md` & `jdTextEdit-9.1/README.md`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/EncodingList.py` & `jdTextEdit-9.1/jdTextEdit/EncodingList.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/Enviroment.py` & `jdTextEdit-9.1/jdTextEdit/Enviroment.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import shutil
 import json
 import sys
 import os
 
 class Enviroment():
     def __init__(self):
-        self.version = "9.0"
+        self.version = "9.1"
         self.programDir = os.path.dirname(os.path.realpath(__file__))
 
         parser = argparse.ArgumentParser()
         parser.add_argument("filename",nargs="*")
         parser.add_argument("-p", "--portable",action="store_true", dest="portable",help="Portable")
         parser.add_argument("--data-dir", dest="dataDir",help="Sets the data directory")
         parser.add_argument("--disable-plugins",action="store_true", dest="disablePlugins",help="Disable Plugins")
```

### Comparing `jdTextEdit-9.0/jdTextEdit/Functions.py` & `jdTextEdit-9.1/jdTextEdit/Functions.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/LexerList.py` & `jdTextEdit-9.1/jdTextEdit/LexerList.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/Logo.png` & `jdTextEdit-9.1/jdTextEdit/Logo.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/Settings.py` & `jdTextEdit-9.1/jdTextEdit/Settings.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/Updater.py` & `jdTextEdit-9.1/jdTextEdit/Updater.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/api/LanguageBase.py` & `jdTextEdit-9.1/jdTextEdit/api/LanguageBase.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/autocompletion/batch.xml` & `jdTextEdit-9.1/jdTextEdit/autocompletion/batch.xml`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/autocompletion/cmake.xml` & `jdTextEdit-9.1/jdTextEdit/autocompletion/cmake.xml`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/autocompletion/coffee.xml` & `jdTextEdit-9.1/jdTextEdit/autocompletion/coffee.xml`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/autocompletion/cpp.xml` & `jdTextEdit-9.1/jdTextEdit/autocompletion/cpp.xml`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/autocompletion/cs.xml` & `jdTextEdit-9.1/jdTextEdit/autocompletion/cs.xml`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/autocompletion/css.xml` & `jdTextEdit-9.1/jdTextEdit/autocompletion/css.xml`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/autocompletion/html.xml` & `jdTextEdit-9.1/jdTextEdit/autocompletion/html.xml`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/autocompletion/java.xml` & `jdTextEdit-9.1/jdTextEdit/autocompletion/java.xml`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/autocompletion/javascript.xml` & `jdTextEdit-9.1/jdTextEdit/autocompletion/javascript.xml`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/autocompletion/lua.xml` & `jdTextEdit-9.1/jdTextEdit/autocompletion/lua.xml`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/autocompletion/perl.xml` & `jdTextEdit-9.1/jdTextEdit/autocompletion/perl.xml`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/autocompletion/python.xml` & `jdTextEdit-9.1/jdTextEdit/autocompletion/python.xml`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/autocompletion/tex.xml` & `jdTextEdit-9.1/jdTextEdit/autocompletion/tex.xml`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/autocompletion/vhdl.xml` & `jdTextEdit-9.1/jdTextEdit/autocompletion/vhdl.xml`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/autocompletion/xml.xml` & `jdTextEdit-9.1/jdTextEdit/autocompletion/xml.xml`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/core/BuiltinLanguage.py` & `jdTextEdit-9.1/jdTextEdit/core/BuiltinLanguage.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/core/DefaultTheme.py` & `jdTextEdit-9.1/jdTextEdit/core/DefaultTheme.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/core/FileTheme.py` & `jdTextEdit-9.1/jdTextEdit/core/FileTheme.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/core/api/EditorSignals.py` & `jdTextEdit-9.1/jdTextEdit/core/api/EditorSignals.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/core/api/PluginAPI.py` & `jdTextEdit-9.1/jdTextEdit/core/api/PluginAPI.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/AboutWindow.py` & `jdTextEdit-9.1/jdTextEdit/gui/AboutWindow.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/BannerWidgets/BigFileBanner.py` & `jdTextEdit-9.1/jdTextEdit/gui/BannerWidgets/BigFileBanner.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/BannerWidgets/EditorconfigBanner.py` & `jdTextEdit-9.1/jdTextEdit/gui/BannerWidgets/EditorconfigBanner.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/BannerWidgets/FileChangedBanner.py` & `jdTextEdit-9.1/jdTextEdit/gui/BannerWidgets/FileChangedBanner.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/BannerWidgets/FileDeletedBanner.py` & `jdTextEdit-9.1/jdTextEdit/gui/BannerWidgets/FileDeletedBanner.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/BannerWidgets/WrongEncodingBanner.py` & `jdTextEdit-9.1/jdTextEdit/gui/BannerWidgets/WrongEncodingBanner.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/BannerWidgets/WrongEolBanner.py` & `jdTextEdit-9.1/jdTextEdit/gui/BannerWidgets/WrongEolBanner.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/CloseSaveWindow.py` & `jdTextEdit-9.1/jdTextEdit/gui/CloseSaveWindow.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/CodeEdit.py` & `jdTextEdit-9.1/jdTextEdit/gui/CodeEdit.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/DateTimeWindow.py` & `jdTextEdit-9.1/jdTextEdit/gui/DateTimeWindow.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/DayTipWindow.py` & `jdTextEdit-9.1/jdTextEdit/gui/DayTipWindow.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/DockWidget.py` & `jdTextEdit-9.1/jdTextEdit/gui/DockWidget.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/DocumentStatistics.py` & `jdTextEdit-9.1/jdTextEdit/gui/DocumentStatistics.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/EditCommandsWindow.py` & `jdTextEdit-9.1/jdTextEdit/gui/EditCommandsWindow.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/EditContainer.py` & `jdTextEdit-9.1/jdTextEdit/gui/EditContainer.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/EditTabWidget.py` & `jdTextEdit-9.1/jdTextEdit/gui/EditTabWidget.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/ExecuteCommandWindow.py` & `jdTextEdit-9.1/jdTextEdit/gui/ExecuteCommandWindow.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/GotoLineWindow.py` & `jdTextEdit-9.1/jdTextEdit/gui/GotoLineWindow.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/MainWindow.py` & `jdTextEdit-9.1/jdTextEdit/gui/MainWindow.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/ManageMacrosWindow.py` & `jdTextEdit-9.1/jdTextEdit/gui/ManageMacrosWindow.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SearchAndReplaceWindow.py` & `jdTextEdit-9.1/jdTextEdit/gui/SearchAndReplaceWindow.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SearchBar.py` & `jdTextEdit-9.1/jdTextEdit/gui/SearchBar.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SearchWindow.py` & `jdTextEdit-9.1/jdTextEdit/gui/SearchWindow.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/AutocompletionTab.py` & `jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/AutocompletionTab.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/BigFilesTab.py` & `jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/BigFilesTab.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/ContextMenuTab.py` & `jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/ContextMenuTab.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/EditorTab.py` & `jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/EditorTab.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/EditorconfigTab.py` & `jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/EditorconfigTab.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/GeneralTab.py` & `jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/GeneralTab.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/InterfaceTab.py` & `jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/InterfaceTab.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/OpenTab.py` & `jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/OpenTab.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/PathsTab.py` & `jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/PathsTab.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/PluginTab.py` & `jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/PluginTab.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/SaveTab.py` & `jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/SaveTab.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/ShortcutTab.py` & `jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/ShortcutTab.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/StyleTab.py` & `jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/StyleTab.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/TabBarTab.py` & `jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/TabBarTab.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SettingsTabs/ToolbarTab.py` & `jdTextEdit-9.1/jdTextEdit/gui/SettingsTabs/ToolbarTab.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SettingsWindow.py` & `jdTextEdit-9.1/jdTextEdit/gui/SettingsWindow.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SidebarWidgets/CharacterMapWidget.py` & `jdTextEdit-9.1/jdTextEdit/gui/SidebarWidgets/CharacterMapWidget.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SidebarWidgets/ClipboardWidget.py` & `jdTextEdit-9.1/jdTextEdit/gui/SidebarWidgets/ClipboardWidget.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SidebarWidgets/FileTreeWidget.py` & `jdTextEdit-9.1/jdTextEdit/gui/SidebarWidgets/FileTreeWidget.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SidebarWidgets/TabListWidget.py` & `jdTextEdit-9.1/jdTextEdit/gui/SidebarWidgets/TabListWidget.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/gui/SplitViewWidget.py` & `jdTextEdit-9.1/jdTextEdit/gui/SplitViewWidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 
     def splitVertical(self):
         """
         Splits vertical
         """
         tabWidget = EditTabWidget(self.env,self,self.splitterWidget.count())
         tabWidget.createTab(self.env.translate("mainWindow.newTabTitle"))
+        tabWidget.updateSettings(self.env.settings)
         self.splitterWidget.insertWidget(self.activeID+1,tabWidget)
         self.env.mainWindow.deleteCurrentViewAction.setEnabled(True)
 
     def deleteCurrentView(self):
         """
         Deletes the current view
         """
@@ -114,8 +115,8 @@
             self.env.mainWindow.deleteCurrentViewAction.setEnabled(True)
 
     def updateTabWidgetID(self):
         """
         Update the IDs of the TabWidgets. This is needed is a TabWidget is removed.
         """
         for count,i in enumerate(self.getAllTabWidgets()):
-            i.splitID = count
+            i.splitID = count
```

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/application-exit.png` & `jdTextEdit-9.1/jdTextEdit/icons/application-exit.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/document-open-recent.png` & `jdTextEdit-9.1/jdTextEdit/icons/document-open-recent.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/document-open.png` & `jdTextEdit-9.1/jdTextEdit/icons/document-open.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/document-print.png` & `jdTextEdit-9.1/jdTextEdit/icons/document-print.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/document-save-all.png` & `jdTextEdit-9.1/jdTextEdit/icons/document-save-all.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/document-save-as.png` & `jdTextEdit-9.1/jdTextEdit/icons/document-save-as.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/document-save.png` & `jdTextEdit-9.1/jdTextEdit/icons/document-save.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/edit-copy.png` & `jdTextEdit-9.1/jdTextEdit/icons/edit-copy.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/edit-cut.png` & `jdTextEdit-9.1/jdTextEdit/icons/edit-cut.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/edit-delete.png` & `jdTextEdit-9.1/jdTextEdit/icons/edit-delete.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/edit-find-replace.png` & `jdTextEdit-9.1/jdTextEdit/icons/edit-find-replace.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/edit-find.png` & `jdTextEdit-9.1/jdTextEdit/icons/edit-find.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/edit-paste.png` & `jdTextEdit-9.1/jdTextEdit/icons/edit-paste.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/edit-redo.png` & `jdTextEdit-9.1/jdTextEdit/icons/edit-redo.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/edit-select-all.png` & `jdTextEdit-9.1/jdTextEdit/icons/edit-select-all.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/edit-undo.png` & `jdTextEdit-9.1/jdTextEdit/icons/edit-undo.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/folder-open.png` & `jdTextEdit-9.1/jdTextEdit/icons/folder-open.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/preferences-other.png` & `jdTextEdit-9.1/jdTextEdit/icons/preferences-other.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/zoom-in.png` & `jdTextEdit-9.1/jdTextEdit/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/zoom-original.png` & `jdTextEdit-9.1/jdTextEdit/icons/zoom-original.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/icons/zoom-out.png` & `jdTextEdit-9.1/jdTextEdit/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/jdTextEdit.py` & `jdTextEdit-9.1/jdTextEdit/jdTextEdit.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/plugins/SpellChecker/SpellChecker.py` & `jdTextEdit-9.1/jdTextEdit/plugins/SpellChecker/SpellChecker.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/plugins/SpellChecker/SpellCheckingTab.py` & `jdTextEdit-9.1/jdTextEdit/plugins/SpellChecker/SpellCheckingTab.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/plugins/SpellChecker/__init__.py` & `jdTextEdit-9.1/jdTextEdit/plugins/SpellChecker/__init__.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/plugins/SpellChecker/translation/de_DE.lang` & `jdTextEdit-9.1/jdTextEdit/plugins/SpellChecker/translation/de_DE.lang`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/plugins/SpellChecker/translation/en_GB.lang` & `jdTextEdit-9.1/jdTextEdit/plugins/SpellChecker/translation/en_GB.lang`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/plugins/pluginmanager/PluginManagerWindow.py` & `jdTextEdit-9.1/jdTextEdit/plugins/pluginmanager/PluginManagerWindow.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/plugins/pluginmanager/__init__.py` & `jdTextEdit-9.1/jdTextEdit/plugins/pluginmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/plugins/pluginmanager/translation/de_DE.lang` & `jdTextEdit-9.1/jdTextEdit/plugins/pluginmanager/translation/de_DE.lang`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/plugins/pluginmanager/translation/en_GB.lang` & `jdTextEdit-9.1/jdTextEdit/plugins/pluginmanager/translation/en_GB.lang`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/translation/de_DE.lang` & `jdTextEdit-9.1/jdTextEdit/translation/de_DE.lang`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit/translation/en_GB.lang` & `jdTextEdit-9.1/jdTextEdit/translation/en_GB.lang`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/jdTextEdit.egg-info/PKG-INFO` & `jdTextEdit-9.1/jdTextEdit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdTextEdit
-Version: 9.0
+Version: 9.1
 Summary:  A powerful texteditor with a lot of features
 Home-page: https://gitlab.com/JakobDev/jdTextEdit
 Author: JakobDev
 Author-email: jakobdev@gmx.de
 License: GPL v3
 Download-URL: https://gitlab.com/JakobDev/jdTextEdit/-/releases
 Project-URL: Issue tracker, https://gitlab.com/JakobDev/jdTextEdit/-/issues
```

### Comparing `jdTextEdit-9.0/jdTextEdit.egg-info/SOURCES.txt` & `jdTextEdit-9.1/jdTextEdit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jdTextEdit-9.0/setup.py` & `jdTextEdit-9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 from setuptools import find_packages, setup
 
 setup(name='jdTextEdit',
-    version='9.0',
+    version='9.1',
     description=' A powerful texteditor with a lot of features',
     long_description=open("README.md").read(),
     long_description_content_type='text/markdown',
     author='JakobDev',
     author_email='jakobdev@gmx.de',
     url='https://gitlab.com/JakobDev/jdTextEdit',
     download_url='https://gitlab.com/JakobDev/jdTextEdit/-/releases',
```

