# Comparing `tmp/core_commands-0.4.4.tar.gz` & `tmp/core_commands-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_commands-0.4.4.tar", max compression
+gzip compressed data, was "core_commands-0.5.0.tar", max compression
```

## Comparing `core_commands-0.4.4.tar` & `core_commands-0.5.0.tar`

### file list

```diff
@@ -1,39 +1,194 @@
--rw-r--r--   0        0        0       20 2023-11-24 10:50:39.212993 core_commands-0.4.4/core_commands/__init__.py
--rw-r--r--   0        0        0       18 2024-04-27 16:09:33.472746 core_commands-0.4.4/core_commands/cmd/__init__.py
--rw-r--r--   0        0        0      423 2024-04-14 12:32:15.243453 core_commands-0.4.4/core_commands/cmd/__pycache__/command_cmd.cpython-311.pyc
--rw-r--r--   0        0        0      339 2024-04-26 09:35:36.626791 core_commands-0.4.4/core_commands/cmd/attrib.py
--rw-r--r--   0        0        0      620 2023-11-26 14:53:35.801583 core_commands-0.4.4/core_commands/cmd/call.py
--rw-r--r--   0        0        0      192 2024-04-27 12:30:59.113021 core_commands-0.4.4/core_commands/cmd/cd.py
--rw-r--r--   0        0        0      162 2023-11-26 13:34:37.662604 core_commands-0.4.4/core_commands/cmd/chdir.py
--rw-r--r--   0        0        0       74 2023-11-26 13:40:27.657852 core_commands-0.4.4/core_commands/cmd/cls.py
--rw-r--r--   0        0        0      844 2024-05-03 12:48:03.466092 core_commands-0.4.4/core_commands/cmd/cmd.py
--rw-r--r--   0        0        0      682 2024-04-27 07:51:44.074159 core_commands-0.4.4/core_commands/cmd/color.py
--rw-r--r--   0        0        0      170 2024-04-26 23:21:15.988546 core_commands-0.4.4/core_commands/cmd/command_cmd.py
--rw-r--r--   0        0        0      236 2023-11-26 14:35:07.010104 core_commands-0.4.4/core_commands/cmd/copy.py
--rw-r--r--   0        0        0      305 2023-11-26 15:00:26.545414 core_commands-0.4.4/core_commands/cmd/curl.py
--rw-r--r--   0        0        0      298 2024-04-26 23:42:17.496887 core_commands-0.4.4/core_commands/cmd/date.py
--rw-r--r--   0        0        0      515 2024-04-26 23:50:17.588678 core_commands-0.4.4/core_commands/cmd/DEL.py
--rw-r--r--   0        0        0      172 2023-11-26 13:19:57.348400 core_commands-0.4.4/core_commands/cmd/dir.py
--rw-r--r--   0        0        0      270 2024-05-03 12:38:26.310842 core_commands-0.4.4/core_commands/cmd/echo.py
--rw-r--r--   0        0        0      183 2024-04-27 00:01:46.298923 core_commands-0.4.4/core_commands/cmd/hostname.py
--rw-r--r--   0        0        0      434 2023-11-26 13:45:26.083270 core_commands-0.4.4/core_commands/cmd/mkdir.py
--rw-r--r--   0        0        0       81 2024-04-26 23:34:26.835037 core_commands-0.4.4/core_commands/cmd/ver.py
--rw-r--r--   0        0        0      158 2024-04-26 23:57:32.523142 core_commands-0.4.4/core_commands/cmd/verify.py
--rw-r--r--   0        0        0      107 2024-04-26 10:41:32.743320 core_commands-0.4.4/core_commands/cmd/w32tm.py
--rw-r--r--   0        0        0       98 2024-04-26 11:00:05.864162 core_commands-0.4.4/core_commands/cmd/waitfor.py
--rw-r--r--   0        0        0      111 2024-04-26 23:26:24.217463 core_commands-0.4.4/core_commands/cmd/wbadmin.py
--rw-r--r--   0        0        0      149 2024-04-26 23:25:22.564346 core_commands-0.4.4/core_commands/cmd/wecutil.py
--rw-r--r--   0        0        0      113 2024-04-26 23:22:14.346255 core_commands-0.4.4/core_commands/cmd/wevtutil.py
--rw-r--r--   0        0        0      241 2024-04-26 10:02:55.946106 core_commands-0.4.4/core_commands/cmd/where.py
--rw-r--r--   0        0        0      217 2024-04-26 09:54:04.254430 core_commands-0.4.4/core_commands/cmd/whoami.py
--rw-r--r--   0        0        0      117 2024-04-26 23:27:44.659390 core_commands-0.4.4/core_commands/cmd/windiff.py
--rw-r--r--   0        0        0      198 2024-04-26 09:43:50.036526 core_commands-0.4.4/core_commands/cmd/winget.py
--rw-r--r--   0        0        0      103 2024-04-26 10:43:30.309215 core_commands-0.4.4/core_commands/cmd/wpr.py
--rw-r--r--   0        0        0      338 2024-04-26 10:40:42.176790 core_commands-0.4.4/core_commands/cmd/wt.py
--rw-r--r--   0        0        0      277 2024-04-26 23:32:19.197506 core_commands-0.4.4/core_commands/cmd/xcopy.py
--rw-r--r--   0        0        0        0 2023-08-15 15:36:53.392178 core_commands-0.4.4/core_commands/commands/winrar,py
--rw-r--r--   0        0        0      185 2024-04-26 09:24:52.311676 core_commands-0.4.4/core_commands/powershell/command_powershell.py
--rw-r--r--   0        0        0        0 2024-04-26 09:16:20.617692 core_commands-0.4.4/core_commands/powershell/powershell.py
--rw-r--r--   0        0        0      383 2024-05-03 12:50:32.417261 core_commands-0.4.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-21 14:03:17.437817 core_commands-0.4.4/README.md
--rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 core_commands-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0       20 2023-11-24 10:50:39.212993 core_commands-0.5.0/core_commands/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-27 16:09:33.472746 core_commands-0.5.0/core_commands/cmd/__init__.py
+-rw-r--r--   0        0        0      423 2024-04-14 12:32:15.243453 core_commands-0.5.0/core_commands/cmd/__pycache__/command_cmd.cpython-311.pyc
+-rw-r--r--   0        0        0      200 2024-05-03 12:59:49.003701 core_commands-0.5.0/core_commands/cmd/arp.py
+-rw-r--r--   0        0        0      238 2024-05-03 13:05:55.081910 core_commands-0.5.0/core_commands/cmd/assoc.py
+-rw-r--r--   0        0        0      339 2024-04-26 09:35:36.626791 core_commands-0.5.0/core_commands/cmd/attrib.py
+-rw-r--r--   0        0        0      111 2024-05-03 13:11:40.338949 core_commands-0.5.0/core_commands/cmd/auditpol.py
+-rw-r--r--   0        0        0      151 2024-05-03 13:13:52.246599 core_commands-0.5.0/core_commands/cmd/bcdboot.py
+-rw-r--r--   0        0        0      178 2024-05-03 13:18:20.912908 core_commands-0.5.0/core_commands/cmd/bcdedit.py
+-rw-r--r--   0        0        0      133 2024-05-03 13:20:29.796757 core_commands-0.5.0/core_commands/cmd/bitsadmin.py
+-rw-r--r--   0        0        0      156 2024-05-17 14:38:35.176544 core_commands-0.5.0/core_commands/cmd/BREAK.py
+-rw-r--r--   0        0        0      203 2024-05-03 13:34:44.291982 core_commands-0.5.0/core_commands/cmd/cacls.py
+-rw-r--r--   0        0        0      620 2023-11-26 14:53:35.801583 core_commands-0.5.0/core_commands/cmd/call.py
+-rw-r--r--   0        0        0      192 2024-04-27 12:30:59.113021 core_commands-0.5.0/core_commands/cmd/cd.py
+-rw-r--r--   0        0        0      117 2024-05-17 14:32:04.659787 core_commands-0.5.0/core_commands/cmd/certreq.py
+-rw-r--r--   0        0        0      119 2024-05-17 14:31:33.689366 core_commands-0.5.0/core_commands/cmd/certutil.py
+-rw-r--r--   0        0        0      115 2024-05-17 14:31:00.399296 core_commands-0.5.0/core_commands/cmd/change.py
+-rw-r--r--   0        0        0      119 2024-05-17 14:30:37.666052 core_commands-0.5.0/core_commands/cmd/changepk.py
+-rw-r--r--   0        0        0      111 2024-05-17 14:30:11.861587 core_commands-0.5.0/core_commands/cmd/chcp.py
+-rw-r--r--   0        0        0      162 2023-11-26 13:34:37.662604 core_commands-0.5.0/core_commands/cmd/chdir.py
+-rw-r--r--   0        0        0      115 2024-05-17 14:29:28.959003 core_commands-0.5.0/core_commands/cmd/chkdsk.py
+-rw-r--r--   0        0        0      117 2024-05-17 14:29:02.118448 core_commands-0.5.0/core_commands/cmd/chkntfs.py
+-rw-r--r--   0        0        0      115 2024-05-17 14:28:28.432879 core_commands-0.5.0/core_commands/cmd/choice.py
+-rw-r--r--   0        0        0      115 2024-05-17 14:28:07.600459 core_commands-0.5.0/core_commands/cmd/cipher.py
+-rw-r--r--   0        0        0      119 2024-05-17 14:27:44.022006 core_commands-0.5.0/core_commands/cmd/cleanmgr.py
+-rw-r--r--   0        0        0      111 2024-05-17 14:27:21.659359 core_commands-0.5.0/core_commands/cmd/clip.py
+-rw-r--r--   0        0        0       74 2023-11-26 13:40:27.657852 core_commands-0.5.0/core_commands/cmd/cls.py
+-rw-r--r--   0        0        0     5119 2024-05-17 15:23:31.581506 core_commands-0.5.0/core_commands/cmd/cmd.py
+-rw-r--r--   0        0        0      115 2024-05-17 14:26:54.721650 core_commands-0.5.0/core_commands/cmd/cmdkey.py
+-rw-r--r--   0        0        0      682 2024-04-27 07:51:44.074159 core_commands-0.5.0/core_commands/cmd/color.py
+-rw-r--r--   0        0        0      499 2024-05-16 14:03:26.004219 core_commands-0.5.0/core_commands/cmd/command_cmd.py
+-rw-r--r--   0        0        0      111 2024-05-17 14:26:13.383964 core_commands-0.5.0/core_commands/cmd/comp.py
+-rw-r--r--   0        0        0      117 2024-05-17 14:25:55.433273 core_commands-0.5.0/core_commands/cmd/compact.py
+-rw-r--r--   0        0        0      117 2024-05-17 14:25:17.563253 core_commands-0.5.0/core_commands/cmd/convert.py
+-rw-r--r--   0        0        0      236 2023-11-26 14:35:07.010104 core_commands-0.5.0/core_commands/cmd/copy.py
+-rw-r--r--   0        0        0      305 2023-11-26 15:00:26.545414 core_commands-0.5.0/core_commands/cmd/curl.py
+-rw-r--r--   0        0        0      298 2024-04-26 23:42:17.496887 core_commands-0.5.0/core_commands/cmd/date.py
+-rw-r--r--   0        0        0      115 2024-05-17 14:23:55.325345 core_commands-0.5.0/core_commands/cmd/defrag.py
+-rw-r--r--   0        0        0      515 2024-04-26 23:50:17.588678 core_commands-0.5.0/core_commands/cmd/DEL.py
+-rw-r--r--   0        0        0      172 2023-11-26 13:19:57.348400 core_commands-0.5.0/core_commands/cmd/dir.py
+-rw-r--r--   0        0        0      119 2024-05-17 14:21:42.370107 core_commands-0.5.0/core_commands/cmd/diskpart.py
+-rw-r--r--   0        0        0      111 2024-05-17 14:20:55.667804 core_commands-0.5.0/core_commands/cmd/dism.py
+-rw-r--r--   0        0        0      129 2024-05-17 14:20:32.385254 core_commands-0.5.0/core_commands/cmd/displayswitch.py
+-rw-r--r--   0        0        0      115 2024-05-17 14:18:41.740911 core_commands-0.5.0/core_commands/cmd/doskey.py
+-rw-r--r--   0        0        0      125 2024-05-17 14:18:22.086661 core_commands-0.5.0/core_commands/cmd/driverquery.py
+-rw-r--r--   0        0        0      119 2024-05-17 14:16:31.084912 core_commands-0.5.0/core_commands/cmd/dsregcmd.py
+-rw-r--r--   0        0        0      270 2024-05-03 12:38:26.310842 core_commands-0.5.0/core_commands/cmd/echo.py
+-rw-r--r--   0        0        0      119 2024-05-16 22:33:37.798501 core_commands-0.5.0/core_commands/cmd/endlocal.py
+-rw-r--r--   0        0        0      113 2024-05-16 22:29:49.819615 core_commands-0.5.0/core_commands/cmd/erase.py
+-rw-r--r--   0        0        0      119 2024-05-16 22:29:31.788385 core_commands-0.5.0/core_commands/cmd/esentutl.py
+-rw-r--r--   0        0        0      125 2024-05-16 22:29:04.397551 core_commands-0.5.0/core_commands/cmd/eventcreate.py
+-rw-r--r--   0        0        0      111 2024-05-16 22:28:37.624879 core_commands-0.5.0/core_commands/cmd/exit.py
+-rw-r--r--   0        0        0      115 2024-05-16 22:28:22.621890 core_commands-0.5.0/core_commands/cmd/expand.py
+-rw-r--r--   0        0        0      119 2024-05-16 22:28:03.888035 core_commands-0.5.0/core_commands/cmd/explorer.py
+-rw-r--r--   0        0        0      107 2024-05-16 22:27:00.519708 core_commands-0.5.0/core_commands/cmd/fc.py
+-rw-r--r--   0        0        0      111 2024-05-16 22:26:42.070029 core_commands-0.5.0/core_commands/cmd/find.py
+-rw-r--r--   0        0        0      117 2024-05-16 22:26:16.092730 core_commands-0.5.0/core_commands/cmd/findstr.py
+-rw-r--r--   0        0        0      113 2024-05-16 22:25:48.430436 core_commands-0.5.0/core_commands/cmd/fltmc.py
+-rw-r--r--   0        0        0      109 2024-05-16 22:24:50.543403 core_commands-0.5.0/core_commands/cmd/FOR.py
+-rw-r--r--   0        0        0      119 2024-05-16 22:24:12.451699 core_commands-0.5.0/core_commands/cmd/forfiles.py
+-rw-r--r--   0        0        0      115 2024-05-16 22:23:46.799587 core_commands-0.5.0/core_commands/cmd/format.py
+-rw-r--r--   0        0        0      115 2024-05-16 22:23:12.790796 core_commands-0.5.0/core_commands/cmd/fsutil.py
+-rw-r--r--   0        0        0      109 2024-05-16 22:22:50.239676 core_commands-0.5.0/core_commands/cmd/ftp.py
+-rw-r--r--   0        0        0      113 2024-05-16 22:22:29.824728 core_commands-0.5.0/core_commands/cmd/ftype.py
+-rw-r--r--   0        0        0      115 2024-05-16 22:21:58.800700 core_commands-0.5.0/core_commands/cmd/getmac.py
+-rw-r--r--   0        0        0      111 2024-05-16 22:20:22.743855 core_commands-0.5.0/core_commands/cmd/goto.py
+-rw-r--r--   0        0        0      119 2024-05-16 22:20:06.574886 core_commands-0.5.0/core_commands/cmd/gpresult.py
+-rw-r--r--   0        0        0      119 2024-05-16 22:19:31.913270 core_commands-0.5.0/core_commands/cmd/gpupdate.py
+-rw-r--r--   0        0        0      111 2024-05-16 22:12:22.262348 core_commands-0.5.0/core_commands/cmd/help.py
+-rw-r--r--   0        0        0      183 2024-04-27 00:01:46.298923 core_commands-0.5.0/core_commands/cmd/hostname.py
+-rw-r--r--   0        0        0      115 2024-05-16 22:11:54.061002 core_commands-0.5.0/core_commands/cmd/icacls.py
+-rw-r--r--   0        0        0      119 2024-05-16 22:11:19.825638 core_commands-0.5.0/core_commands/cmd/iexpress.py
+-rw-r--r--   0        0        0      107 2024-05-16 22:10:50.934848 core_commands-0.5.0/core_commands/cmd/IF.py
+-rw-r--r--   0        0        0      119 2024-05-16 22:10:06.980534 core_commands-0.5.0/core_commands/cmd/ipconfig.py
+-rw-r--r--   0        0        0      113 2024-05-16 22:08:20.378088 core_commands-0.5.0/core_commands/cmd/klist.py
+-rw-r--r--   0        0        0      113 2024-05-16 22:07:59.899665 core_commands-0.5.0/core_commands/cmd/label.py
+-rw-r--r--   0        0        0      114 2024-05-16 22:06:01.146683 core_commands-0.5.0/core_commands/cmd/lodctr.py
+-rw-r--r--   0        0        0      115 2024-05-16 22:04:36.383465 core_commands-0.5.0/core_commands/cmd/logman.py
+-rw-r--r--   0        0        0      114 2024-05-16 22:33:24.623576 core_commands-0.5.0/core_commands/cmd/logoff.py
+-rw-r--r--   0        0        0      116 2024-05-16 21:51:27.760023 core_commands-0.5.0/core_commands/cmd/makecab.py
+-rw-r--r--   0        0        0      124 2024-05-16 22:33:19.132023 core_commands-0.5.0/core_commands/cmd/manage_bde.py
+-rw-r--r--   0        0        0      116 2024-05-16 21:48:50.272681 core_commands-0.5.0/core_commands/cmd/mbr2gpt.py
+-rw-r--r--   0        0        0      106 2024-05-16 21:47:46.173340 core_commands-0.5.0/core_commands/cmd/md.py
+-rw-r--r--   0        0        0      434 2023-11-26 13:45:26.083270 core_commands-0.5.0/core_commands/cmd/mkdir.py
+-rw-r--r--   0        0        0      114 2024-05-16 21:46:52.933085 core_commands-0.5.0/core_commands/cmd/mklink.py
+-rw-r--r--   0        0        0      110 2024-05-16 14:27:28.674678 core_commands-0.5.0/core_commands/cmd/mode.py
+-rw-r--r--   0        0        0      110 2024-05-16 14:26:52.192783 core_commands-0.5.0/core_commands/cmd/more.py
+-rw-r--r--   0        0        0      118 2024-05-16 14:25:59.566813 core_commands-0.5.0/core_commands/cmd/mountvol.py
+-rw-r--r--   0        0        0      110 2024-05-16 14:24:55.941635 core_commands-0.5.0/core_commands/cmd/move.py
+-rw-r--r--   0        0        0      118 2024-05-16 14:24:20.524170 core_commands-0.5.0/core_commands/cmd/moveuser.py
+-rw-r--r--   0        0        0      108 2024-05-16 14:23:39.892973 core_commands-0.5.0/core_commands/cmd/msg.py
+-rw-r--r--   0        0        0      116 2024-05-16 14:22:50.943172 core_commands-0.5.0/core_commands/cmd/msiexec.py
+-rw-r--r--   0        0        0      118 2024-05-16 14:21:58.964635 core_commands-0.5.0/core_commands/cmd/msinfo32.py
+-rw-r--r--   0        0        0      112 2024-05-16 14:20:59.255404 core_commands-0.5.0/core_commands/cmd/mstsc.py
+-rw-r--r--   0        0        0      120 2024-05-16 14:18:25.153728 core_commands-0.5.0/core_commands/cmd/nbtstat.py
+-rw-r--r--   0        0        0      108 2024-05-16 14:19:48.705124 core_commands-0.5.0/core_commands/cmd/net.py
+-rw-r--r--   0        0        0      112 2024-05-16 14:18:12.815221 core_commands-0.5.0/core_commands/cmd/netsh.py
+-rw-r--r--   0        0        0      116 2024-05-16 14:12:22.149263 core_commands-0.5.0/core_commands/cmd/netstat.py
+-rw-r--r--   0        0        0      114 2024-05-16 14:11:31.112607 core_commands-0.5.0/core_commands/cmd/nltest.py
+-rw-r--r--   0        0        0      118 2024-05-16 14:10:27.156396 core_commands-0.5.0/core_commands/cmd/nslookup.py
+-rw-r--r--   0        0        0      120 2024-05-16 14:08:45.392646 core_commands-0.5.0/core_commands/cmd/openfiles.py
+-rw-r--r--   0        0        0      110 2024-05-16 14:07:18.340905 core_commands-0.5.0/core_commands/cmd/path.py
+-rw-r--r--   0        0        0      118 2024-05-16 14:05:29.729715 core_commands-0.5.0/core_commands/cmd/pathping.py
+-rw-r--r--   0        0        0      112 2024-05-16 14:04:39.172543 core_commands-0.5.0/core_commands/cmd/pause.py
+-rw-r--r--   0        0        0      110 2024-05-16 13:58:05.327762 core_commands-0.5.0/core_commands/cmd/ping.py
+-rw-r--r--   0        0        0      114 2024-05-16 13:51:43.674514 core_commands-0.5.0/core_commands/cmd/pktmon.py
+-rw-r--r--   0        0        0      116 2024-05-16 13:50:29.444668 core_commands-0.5.0/core_commands/cmd/pnputil.py
+-rw-r--r--   0        0        0      110 2024-05-16 13:49:43.299492 core_commands-0.5.0/core_commands/cmd/popd.py
+-rw-r--r--   0        0        0      118 2024-05-16 13:48:41.307103 core_commands-0.5.0/core_commands/cmd/powercfg.py
+-rw-r--r--   0        0        0      112 2024-05-16 13:47:44.103660 core_commands-0.5.0/core_commands/cmd/PRINT.py
+-rw-r--r--   0        0        0      114 2024-05-16 13:44:38.304221 core_commands-0.5.0/core_commands/cmd/prompt.py
+-rw-r--r--   0        0        0      112 2024-05-16 13:41:17.235202 core_commands-0.5.0/core_commands/cmd/pushd.py
+-rw-r--r--   0        0        0      116 2024-05-16 13:38:11.856178 core_commands-0.5.0/core_commands/cmd/qappsrv.py
+-rw-r--r--   0        0        0      118 2024-05-16 13:40:11.633067 core_commands-0.5.0/core_commands/cmd/qprocess.py
+-rw-r--r--   0        0        0      112 2024-05-16 13:36:46.694069 core_commands-0.5.0/core_commands/cmd/quser.py
+-rw-r--r--   0        0        0      116 2024-05-16 13:39:14.405193 core_commands-0.5.0/core_commands/cmd/qwinsta.py
+-rw-r--r--   0        0        0      116 2024-05-15 07:49:51.558895 core_commands-0.5.0/core_commands/cmd/rasdial.py
+-rw-r--r--   0        0        0      118 2024-05-15 07:48:50.308178 core_commands-0.5.0/core_commands/cmd/rasphone.py
+-rw-r--r--   0        0        0      106 2024-05-15 07:48:06.998865 core_commands-0.5.0/core_commands/cmd/rd.py
+-rw-r--r--   0        0        0      118 2024-05-15 07:47:27.474122 core_commands-0.5.0/core_commands/cmd/reagentc.py
+-rw-r--r--   0        0        0      116 2024-05-15 07:46:21.079033 core_commands-0.5.0/core_commands/cmd/recover.py
+-rw-r--r--   0        0        0      108 2024-05-15 07:45:44.639638 core_commands-0.5.0/core_commands/cmd/reg.py
+-rw-r--r--   0        0        0      116 2024-05-15 07:44:40.256724 core_commands-0.5.0/core_commands/cmd/regedit.py
+-rw-r--r--   0        0        0      114 2024-05-15 07:41:47.226554 core_commands-0.5.0/core_commands/cmd/regini.py
+-rw-r--r--   0        0        0      118 2024-05-15 07:43:01.768840 core_commands-0.5.0/core_commands/cmd/regsvr32.py
+-rw-r--r--   0        0        0      108 2024-05-15 07:38:57.625494 core_commands-0.5.0/core_commands/cmd/ren.py
+-rw-r--r--   0        0        0      116 2024-05-15 07:37:57.752194 core_commands-0.5.0/core_commands/cmd/replace.py
+-rw-r--r--   0        0        0      112 2024-05-15 07:37:15.264630 core_commands-0.5.0/core_commands/cmd/reset.py
+-rw-r--r--   0        0        0      112 2024-05-15 07:35:51.172301 core_commands-0.5.0/core_commands/cmd/rmdir.py
+-rw-r--r--   0        0        0      118 2024-05-15 07:33:57.257618 core_commands-0.5.0/core_commands/cmd/rmtshare.py
+-rw-r--r--   0        0        0      118 2024-05-15 07:32:41.096207 core_commands-0.5.0/core_commands/cmd/robocopy.py
+-rw-r--r--   0        0        0      112 2024-05-15 07:30:17.805368 core_commands-0.5.0/core_commands/cmd/route.py
+-rw-r--r--   0        0        0      112 2024-05-15 07:28:41.090861 core_commands-0.5.0/core_commands/cmd/runas.py
+-rw-r--r--   0        0        0      118 2024-05-15 07:26:48.008140 core_commands-0.5.0/core_commands/cmd/rundll32.py
+-rw-r--r--   0        0        0      106 2024-05-15 07:25:44.587590 core_commands-0.5.0/core_commands/cmd/sc.py
+-rw-r--r--   0        0        0      118 2024-05-15 07:25:04.900258 core_commands-0.5.0/core_commands/cmd/schtasks.py
+-rw-r--r--   0        0        0      126 2024-05-15 07:23:38.753776 core_commands-0.5.0/core_commands/cmd/scriptrunner.py
+-rw-r--r--   0        0        0      108 2024-05-15 07:22:39.041092 core_commands-0.5.0/core_commands/cmd/set.py
+-rw-r--r--   0        0        0      118 2024-05-15 07:29:03.018930 core_commands-0.5.0/core_commands/cmd/setlocal.py
+-rw-r--r--   0        0        0      114 2024-05-15 07:19:50.787977 core_commands-0.5.0/core_commands/cmd/setspn.py
+-rw-r--r--   0        0        0      110 2024-05-15 07:18:47.456237 core_commands-0.5.0/core_commands/cmd/setx.py
+-rw-r--r--   0        0        0      108 2024-05-15 07:17:55.822420 core_commands-0.5.0/core_commands/cmd/sfc.py
+-rw-r--r--   0        0        0      112 2024-05-15 07:16:13.656814 core_commands-0.5.0/core_commands/cmd/shift.py
+-rw-r--r--   0        0        0      118 2024-05-15 07:13:58.093718 core_commands-0.5.0/core_commands/cmd/shutdown.py
+-rw-r--r--   0        0        0      112 2024-05-15 07:12:40.311743 core_commands-0.5.0/core_commands/cmd/sleep.py
+-rw-r--r--   0        0        0      112 2024-05-15 07:12:04.713116 core_commands-0.5.0/core_commands/cmd/slmgr.py
+-rw-r--r--   0        0        0      110 2024-05-15 07:09:27.050592 core_commands-0.5.0/core_commands/cmd/sort.py
+-rw-r--r--   0        0        0      108 2024-05-15 07:07:17.406769 core_commands-0.5.0/core_commands/cmd/ssh.py
+-rw-r--r--   0        0        0      120 2024-05-15 07:04:51.866458 core_commands-0.5.0/core_commands/cmd/start.py
+-rw-r--r--   0        0        0      120 2024-05-15 07:04:58.874060 core_commands-0.5.0/core_commands/cmd/subst.py
+-rw-r--r--   0        0        0      118 2024-05-13 10:42:38.002909 core_commands-0.5.0/core_commands/cmd/sxstrace.py
+-rw-r--r--   0        0        0      122 2024-05-13 10:40:06.945956 core_commands-0.5.0/core_commands/cmd/systeminfo.py
+-rw-r--r--   0        0        0      116 2024-05-13 10:33:13.132928 core_commands-0.5.0/core_commands/cmd/takeown.py
+-rw-r--r--   0        0        0      108 2024-05-13 10:31:25.961989 core_commands-0.5.0/core_commands/cmd/tar.py
+-rw-r--r--   0        0        0      118 2024-05-13 10:26:46.127252 core_commands-0.5.0/core_commands/cmd/taskkill.py
+-rw-r--r--   0        0        0      118 2024-05-13 10:30:41.416311 core_commands-0.5.0/core_commands/cmd/tasklist.py
+-rw-r--r--   0        0        0      110 2024-05-13 10:25:35.472919 core_commands-0.5.0/core_commands/cmd/time.py
+-rw-r--r--   0        0        0      116 2024-05-13 10:22:41.274008 core_commands-0.5.0/core_commands/cmd/timeout.py
+-rw-r--r--   0        0        0      112 2024-05-13 10:21:59.680410 core_commands-0.5.0/core_commands/cmd/title.py
+-rw-r--r--   0        0        0      116 2024-05-13 10:15:02.470580 core_commands-0.5.0/core_commands/cmd/tracert.py
+-rw-r--r--   0        0        0      110 2024-05-13 10:14:07.433996 core_commands-0.5.0/core_commands/cmd/tree.py
+-rw-r--r--   0        0        0      118 2024-05-13 10:11:06.179157 core_commands-0.5.0/core_commands/cmd/tsdiscon.py
+-rw-r--r--   0        0        0      114 2024-05-13 10:09:54.726987 core_commands-0.5.0/core_commands/cmd/tskill.py
+-rw-r--r--   0        0        0      103 2024-05-13 10:06:55.262094 core_commands-0.5.0/core_commands/cmd/type.py
+-rw-r--r--   0        0        0      118 2024-05-13 10:04:02.485498 core_commands-0.5.0/core_commands/cmd/typeperf.py
+-rw-r--r--   0        0        0      114 2024-05-13 10:09:59.568652 core_commands-0.5.0/core_commands/cmd/tzutil.py
+-rw-r--r--   0        0        0       81 2024-04-26 23:34:26.835037 core_commands-0.5.0/core_commands/cmd/ver.py
+-rw-r--r--   0        0        0      158 2024-04-26 23:57:32.523142 core_commands-0.5.0/core_commands/cmd/verify.py
+-rw-r--r--   0        0        0      108 2024-05-13 09:59:14.052405 core_commands-0.5.0/core_commands/cmd/vol.py
+-rw-r--r--   0        0        0      118 2024-05-13 10:10:02.566618 core_commands-0.5.0/core_commands/cmd/vssadmin.py
+-rw-r--r--   0        0        0      107 2024-04-26 10:41:32.743320 core_commands-0.5.0/core_commands/cmd/w32tm.py
+-rw-r--r--   0        0        0       98 2024-04-26 11:00:05.864162 core_commands-0.5.0/core_commands/cmd/waitfor.py
+-rw-r--r--   0        0        0      111 2024-04-26 23:26:24.217463 core_commands-0.5.0/core_commands/cmd/wbadmin.py
+-rw-r--r--   0        0        0      149 2024-04-26 23:25:22.564346 core_commands-0.5.0/core_commands/cmd/wecutil.py
+-rw-r--r--   0        0        0      113 2024-04-26 23:22:14.346255 core_commands-0.5.0/core_commands/cmd/wevtutil.py
+-rw-r--r--   0        0        0      241 2024-04-26 10:02:55.946106 core_commands-0.5.0/core_commands/cmd/where.py
+-rw-r--r--   0        0        0      217 2024-04-26 09:54:04.254430 core_commands-0.5.0/core_commands/cmd/whoami.py
+-rw-r--r--   0        0        0      117 2024-04-26 23:27:44.659390 core_commands-0.5.0/core_commands/cmd/windiff.py
+-rw-r--r--   0        0        0      198 2024-04-26 09:43:50.036526 core_commands-0.5.0/core_commands/cmd/winget.py
+-rw-r--r--   0        0        0      124 2024-05-13 00:50:36.809216 core_commands-0.5.0/core_commands/cmd/winmgmt.py
+-rw-r--r--   0        0        0      163 2024-05-13 00:43:03.903554 core_commands-0.5.0/core_commands/cmd/winrm.py
+-rw-r--r--   0        0        0      164 2024-05-13 00:41:51.967787 core_commands-0.5.0/core_commands/cmd/winrs.py
+-rw-r--r--   0        0        0      160 2024-05-13 00:39:07.209074 core_commands-0.5.0/core_commands/cmd/wmic.py
+-rw-r--r--   0        0        0      103 2024-04-26 10:43:30.309215 core_commands-0.5.0/core_commands/cmd/wpr.py
+-rw-r--r--   0        0        0      338 2024-04-26 10:40:42.176790 core_commands-0.5.0/core_commands/cmd/wt.py
+-rw-r--r--   0        0        0      177 2024-05-13 00:29:41.547394 core_commands-0.5.0/core_commands/cmd/wuauclt.py
+-rw-r--r--   0        0        0      129 2024-05-13 00:33:49.389094 core_commands-0.5.0/core_commands/cmd/wusa.py
+-rw-r--r--   0        0        0      277 2024-04-26 23:32:19.197506 core_commands-0.5.0/core_commands/cmd/xcopy.py
+-rw-r--r--   0        0        0        0 2023-08-15 15:36:53.392178 core_commands-0.5.0/core_commands/commands/winrar,py
+-rw-r--r--   0        0        0      185 2024-04-26 09:24:52.311676 core_commands-0.5.0/core_commands/powershell/command_powershell.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:16:20.617692 core_commands-0.5.0/core_commands/powershell/powershell.py
+-rw-r--r--   0        0        0      383 2024-05-17 15:36:03.566330 core_commands-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-21 14:03:17.437817 core_commands-0.5.0/README.md
+-rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 core_commands-0.5.0/PKG-INFO
```

### Comparing `core_commands-0.4.4/core_commands/cmd/call.py` & `core_commands-0.5.0/core_commands/cmd/call.py`

 * *Files identical despite different names*

### Comparing `core_commands-0.4.4/core_commands/cmd/color.py` & `core_commands-0.5.0/core_commands/cmd/color.py`

 * *Files identical despite different names*

### Comparing `core_commands-0.4.4/core_commands/cmd/DEL.py` & `core_commands-0.5.0/core_commands/cmd/DEL.py`

 * *Files identical despite different names*

