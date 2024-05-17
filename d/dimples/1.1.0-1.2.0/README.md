# Comparing `tmp/dimples-1.1.0.tar.gz` & `tmp/dimples-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimples-1.1.0.tar", last modified: Wed May 15 19:36:14 2024, max compression
+gzip compressed data, was "dist/dimples-1.2.0.tar", last modified: Fri May 17 17:33:06 2024, max compression
```

## Comparing `dimples-1.1.0.tar` & `dimples-1.2.0.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2024-05-15 19:36:14.000000 dimples-1.1.0/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-1.1.0/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples/
--rw-r--r--   0 moky       (501) staff       (20)     8913 2024-04-11 15:45:18.000000 dimples-1.1.0/dimples/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples/client/
--rw-r--r--   0 moky       (501) staff       (20)     1977 2023-12-05 04:36:14.000000 dimples-1.1.0/dimples/client/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10946 2024-05-07 03:48:04.000000 dimples-1.1.0/dimples/client/archivist.py
--rw-r--r--   0 moky       (501) staff       (20)     3862 2024-04-24 03:33:53.000000 dimples-1.1.0/dimples/client/checkpoint.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples/client/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     2287 2023-10-29 13:43:35.000000 dimples-1.1.0/dimples/client/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     1952 2024-05-07 03:28:52.000000 dimples-1.1.0/dimples/client/cpu/commands.py
--rw-r--r--   0 moky       (501) staff       (20)     4803 2023-10-29 13:43:46.000000 dimples-1.1.0/dimples/client/cpu/creator.py
--rw-r--r--   0 moky       (501) staff       (20)     9096 2024-05-07 16:12:33.000000 dimples-1.1.0/dimples/client/cpu/group.py
--rw-r--r--   0 moky       (501) staff       (20)     2173 2024-05-07 03:32:12.000000 dimples-1.1.0/dimples/client/cpu/grp_expel.py
--rw-r--r--   0 moky       (501) staff       (20)     5937 2024-05-07 03:34:38.000000 dimples-1.1.0/dimples/client/cpu/grp_invite.py
--rw-r--r--   0 moky       (501) staff       (20)     3998 2024-05-07 03:35:17.000000 dimples-1.1.0/dimples/client/cpu/grp_join.py
--rw-r--r--   0 moky       (501) staff       (20)     4177 2024-05-07 03:35:53.000000 dimples-1.1.0/dimples/client/cpu/grp_query.py
--rw-r--r--   0 moky       (501) staff       (20)     4388 2024-05-07 03:36:21.000000 dimples-1.1.0/dimples/client/cpu/grp_quit.py
--rw-r--r--   0 moky       (501) staff       (20)     5711 2024-05-07 03:36:56.000000 dimples-1.1.0/dimples/client/cpu/grp_reset.py
--rw-r--r--   0 moky       (501) staff       (20)     4086 2024-05-07 03:37:19.000000 dimples-1.1.0/dimples/client/cpu/grp_resign.py
--rw-r--r--   0 moky       (501) staff       (20)     5184 2024-05-07 03:50:13.000000 dimples-1.1.0/dimples/client/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     6404 2024-05-06 19:03:39.000000 dimples-1.1.0/dimples/client/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     9059 2024-05-07 03:49:36.000000 dimples-1.1.0/dimples/client/messenger.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples/client/network/
--rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-1.1.0/dimples/client/network/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7030 2024-05-09 20:14:55.000000 dimples-1.1.0/dimples/client/network/session.py
--rw-r--r--   0 moky       (501) staff       (20)     9328 2024-05-15 16:23:08.000000 dimples-1.1.0/dimples/client/network/state.py
--rw-r--r--   0 moky       (501) staff       (20)     9501 2024-03-06 17:49:03.000000 dimples-1.1.0/dimples/client/network/transition.py
--rw-r--r--   0 moky       (501) staff       (20)     9296 2024-05-07 03:57:08.000000 dimples-1.1.0/dimples/client/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     6077 2024-05-07 04:00:01.000000 dimples-1.1.0/dimples/client/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5551 2024-05-15 16:00:09.000000 dimples-1.1.0/dimples/client/terminal.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples/common/
--rw-r--r--   0 moky       (501) staff       (20)     2652 2024-04-11 16:03:38.000000 dimples-1.1.0/dimples/common/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3520 2023-10-19 02:46:00.000000 dimples-1.1.0/dimples/common/anonymous.py
--rw-r--r--   0 moky       (501) staff       (20)     5771 2023-10-13 10:02:36.000000 dimples-1.1.0/dimples/common/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     7930 2024-05-06 18:08:29.000000 dimples-1.1.0/dimples/common/archivist.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples/common/compat/
--rw-r--r--   0 moky       (501) staff       (20)     2751 2023-10-13 16:15:07.000000 dimples-1.1.0/dimples/common/compat/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3806 2023-10-15 03:29:15.000000 dimples-1.1.0/dimples/common/compat/btc.py
--rw-r--r--   0 moky       (501) staff       (20)     6666 2023-10-15 03:31:01.000000 dimples-1.1.0/dimples/common/compat/compatible.py
--rw-r--r--   0 moky       (501) staff       (20)     2572 2023-10-13 10:09:19.000000 dimples-1.1.0/dimples/common/compat/entity.py
--rw-r--r--   0 moky       (501) staff       (20)     6277 2023-10-17 15:21:36.000000 dimples-1.1.0/dimples/common/compat/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     6192 2023-10-13 10:09:24.000000 dimples-1.1.0/dimples/common/compat/network.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples/common/dbi/
--rw-r--r--   0 moky       (501) staff       (20)     2146 2023-10-15 04:04:22.000000 dimples-1.1.0/dimples/common/dbi/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7648 2024-05-06 18:49:56.000000 dimples-1.1.0/dimples/common/dbi/account.py
--rw-r--r--   0 moky       (501) staff       (20)     2735 2024-05-06 18:36:11.000000 dimples-1.1.0/dimples/common/dbi/message.py
--rw-r--r--   0 moky       (501) staff       (20)     8007 2024-05-06 18:03:43.000000 dimples-1.1.0/dimples/common/dbi/session.py
--rw-r--r--   0 moky       (501) staff       (20)     8591 2024-05-07 18:41:02.000000 dimples-1.1.0/dimples/common/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     9209 2024-05-07 18:48:04.000000 dimples-1.1.0/dimples/common/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     8616 2024-05-06 18:15:14.000000 dimples-1.1.0/dimples/common/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     2999 2024-05-07 18:46:08.000000 dimples-1.1.0/dimples/common/processer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples/common/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     2695 2023-10-29 10:59:58.000000 dimples-1.1.0/dimples/common/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3426 2023-10-13 12:48:25.000000 dimples-1.1.0/dimples/common/protocol/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     2611 2023-10-29 11:52:51.000000 dimples-1.1.0/dimples/common/protocol/block.py
--rw-r--r--   0 moky       (501) staff       (20)     5211 2023-10-13 12:47:14.000000 dimples-1.1.0/dimples/common/protocol/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4897 2023-12-03 07:02:16.000000 dimples-1.1.0/dimples/common/protocol/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2619 2023-10-29 11:53:00.000000 dimples-1.1.0/dimples/common/protocol/mute.py
--rw-r--r--   0 moky       (501) staff       (20)     2620 2023-10-13 12:45:16.000000 dimples-1.1.0/dimples/common/protocol/report.py
--rw-r--r--   0 moky       (501) staff       (20)     6346 2024-05-06 18:17:07.000000 dimples-1.1.0/dimples/common/register.py
--rw-r--r--   0 moky       (501) staff       (20)     4591 2024-05-07 18:47:41.000000 dimples-1.1.0/dimples/common/session.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples/conn/
--rw-r--r--   0 moky       (501) staff       (20)     4508 2024-05-14 15:03:49.000000 dimples-1.1.0/dimples/conn/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6270 2024-05-14 16:29:47.000000 dimples-1.1.0/dimples/conn/flexible.py
--rw-r--r--   0 moky       (501) staff       (20)    10956 2024-05-14 15:09:23.000000 dimples-1.1.0/dimples/conn/gate.py
--rw-r--r--   0 moky       (501) staff       (20)    12264 2024-05-15 19:21:42.000000 dimples-1.1.0/dimples/conn/gatekeeper.py
--rw-r--r--   0 moky       (501) staff       (20)    10810 2024-05-14 15:15:47.000000 dimples-1.1.0/dimples/conn/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     8002 2024-05-14 15:15:53.000000 dimples-1.1.0/dimples/conn/mtp.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples/conn/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     1916 2024-05-14 15:15:34.000000 dimples-1.1.0/dimples/conn/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8771 2024-04-23 09:39:58.000000 dimples-1.1.0/dimples/conn/protocol/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     8992 2024-05-14 15:42:00.000000 dimples-1.1.0/dimples/conn/protocol/ws.py
--rw-r--r--   0 moky       (501) staff       (20)     6444 2024-04-24 03:34:40.000000 dimples-1.1.0/dimples/conn/queue.py
--rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-1.1.0/dimples/conn/seeker.py
--rw-r--r--   0 moky       (501) staff       (20)     4294 2024-05-14 15:17:10.000000 dimples-1.1.0/dimples/conn/session.py
--rw-r--r--   0 moky       (501) staff       (20)     7920 2024-05-14 16:13:17.000000 dimples-1.1.0/dimples/conn/ws.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples/database/
--rw-r--r--   0 moky       (501) staff       (20)     2812 2023-10-15 04:57:38.000000 dimples-1.1.0/dimples/database/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8179 2024-05-06 18:51:03.000000 dimples-1.1.0/dimples/database/account.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples/database/dos/
--rw-r--r--   0 moky       (501) staff       (20)     1949 2023-10-14 04:19:29.000000 dimples-1.1.0/dimples/database/dos/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4692 2024-05-14 14:54:42.000000 dimples-1.1.0/dimples/database/dos/base.py
--rw-r--r--   0 moky       (501) staff       (20)     6360 2024-05-06 18:30:09.000000 dimples-1.1.0/dimples/database/dos/document.py
--rw-r--r--   0 moky       (501) staff       (20)     5247 2024-05-06 18:21:39.000000 dimples-1.1.0/dimples/database/dos/group.py
--rw-r--r--   0 moky       (501) staff       (20)     6045 2024-05-06 18:50:27.000000 dimples-1.1.0/dimples/database/dos/group_history.py
--rw-r--r--   0 moky       (501) staff       (20)     2789 2024-05-06 18:39:54.000000 dimples-1.1.0/dimples/database/dos/group_keys.py
--rw-r--r--   0 moky       (501) staff       (20)     3101 2024-05-06 18:24:21.000000 dimples-1.1.0/dimples/database/dos/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2646 2024-05-06 18:24:29.000000 dimples-1.1.0/dimples/database/dos/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5553 2024-05-06 18:24:46.000000 dimples-1.1.0/dimples/database/dos/private.py
--rw-r--r--   0 moky       (501) staff       (20)     8045 2024-05-06 18:26:43.000000 dimples-1.1.0/dimples/database/dos/station.py
--rw-r--r--   0 moky       (501) staff       (20)     2941 2024-05-06 18:27:02.000000 dimples-1.1.0/dimples/database/dos/user.py
--rw-r--r--   0 moky       (501) staff       (20)     3760 2024-05-06 18:51:40.000000 dimples-1.1.0/dimples/database/message.py
--rw-r--r--   0 moky       (501) staff       (20)     4436 2024-05-06 18:53:13.000000 dimples-1.1.0/dimples/database/session.py
--rw-r--r--   0 moky       (501) staff       (20)     3132 2024-05-06 18:27:39.000000 dimples-1.1.0/dimples/database/t_cipherkey.py
--rw-r--r--   0 moky       (501) staff       (20)     4147 2024-05-06 18:30:39.000000 dimples-1.1.0/dimples/database/t_document.py
--rw-r--r--   0 moky       (501) staff       (20)     6567 2024-05-06 18:31:50.000000 dimples-1.1.0/dimples/database/t_group.py
--rw-r--r--   0 moky       (501) staff       (20)     5809 2024-05-06 18:50:47.000000 dimples-1.1.0/dimples/database/t_group_history.py
--rw-r--r--   0 moky       (501) staff       (20)     4295 2024-05-06 18:41:59.000000 dimples-1.1.0/dimples/database/t_group_keys.py
--rw-r--r--   0 moky       (501) staff       (20)     4246 2024-05-06 18:41:59.000000 dimples-1.1.0/dimples/database/t_login.py
--rw-r--r--   0 moky       (501) staff       (20)     4405 2024-05-06 18:39:12.000000 dimples-1.1.0/dimples/database/t_message.py
--rw-r--r--   0 moky       (501) staff       (20)     3756 2024-05-06 18:41:59.000000 dimples-1.1.0/dimples/database/t_meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5909 2024-05-06 18:42:32.000000 dimples-1.1.0/dimples/database/t_private.py
--rw-r--r--   0 moky       (501) staff       (20)     6845 2024-05-06 18:44:20.000000 dimples-1.1.0/dimples/database/t_station.py
--rw-r--r--   0 moky       (501) staff       (20)     3578 2024-05-06 18:45:26.000000 dimples-1.1.0/dimples/database/t_user.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples/edge/
--rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-1.1.0/dimples/edge/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    16017 2024-05-15 18:48:43.000000 dimples-1.1.0/dimples/edge/octopus.py
--rw-r--r--   0 moky       (501) staff       (20)     6161 2024-05-15 16:34:13.000000 dimples-1.1.0/dimples/edge/shared.py
--rw-r--r--   0 moky       (501) staff       (20)     2897 2024-05-15 16:03:03.000000 dimples-1.1.0/dimples/edge/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples/group/
--rw-r--r--   0 moky       (501) staff       (20)     1874 2023-10-18 14:55:15.000000 dimples-1.1.0/dimples/group/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6217 2024-05-06 18:55:34.000000 dimples-1.1.0/dimples/group/admin.py
--rw-r--r--   0 moky       (501) staff       (20)     7191 2024-05-06 19:06:23.000000 dimples-1.1.0/dimples/group/builder.py
--rw-r--r--   0 moky       (501) staff       (20)     7337 2024-05-06 19:05:04.000000 dimples-1.1.0/dimples/group/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)    12302 2024-05-06 19:12:10.000000 dimples-1.1.0/dimples/group/emitter.py
--rw-r--r--   0 moky       (501) staff       (20)     5275 2024-05-06 18:58:53.000000 dimples-1.1.0/dimples/group/helper.py
--rw-r--r--   0 moky       (501) staff       (20)    16535 2024-05-06 19:16:50.000000 dimples-1.1.0/dimples/group/manager.py
--rw-r--r--   0 moky       (501) staff       (20)     5084 2024-05-06 19:10:38.000000 dimples-1.1.0/dimples/group/packer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples/register/
--rw-r--r--   0 moky       (501) staff       (20)     1441 2024-04-25 15:20:32.000000 dimples-1.1.0/dimples/register/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10595 2024-05-10 10:25:00.000000 dimples-1.1.0/dimples/register/base.py
--rw-r--r--   0 moky       (501) staff       (20)     8248 2024-05-10 10:25:44.000000 dimples-1.1.0/dimples/register/ext.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3901 2024-05-14 14:54:42.000000 dimples-1.1.0/dimples/register/run.py
--rw-r--r--   0 moky       (501) staff       (20)     4151 2024-05-07 17:52:52.000000 dimples-1.1.0/dimples/register/shared.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples/server/
--rw-r--r--   0 moky       (501) staff       (20)     2448 2024-02-17 14:40:02.000000 dimples-1.1.0/dimples/server/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7502 2024-05-07 17:25:09.000000 dimples-1.1.0/dimples/server/archivist.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples/server/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     1779 2023-07-05 16:57:44.000000 dimples-1.1.0/dimples/server/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2729 2024-05-07 04:03:19.000000 dimples-1.1.0/dimples/server/cpu/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     4857 2024-05-07 04:03:27.000000 dimples-1.1.0/dimples/server/cpu/document.py
--rw-r--r--   0 moky       (501) staff       (20)     4035 2024-05-07 04:22:27.000000 dimples-1.1.0/dimples/server/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4234 2024-05-07 04:22:59.000000 dimples-1.1.0/dimples/server/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     3539 2024-05-07 04:23:05.000000 dimples-1.1.0/dimples/server/cpu/report.py
--rw-r--r--   0 moky       (501) staff       (20)    17709 2024-05-15 19:24:25.000000 dimples-1.1.0/dimples/server/dispatcher.py
--rw-r--r--   0 moky       (501) staff       (20)     4574 2024-05-07 17:29:24.000000 dimples-1.1.0/dimples/server/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     6584 2024-05-07 04:15:23.000000 dimples-1.1.0/dimples/server/packer.py
--rw-r--r--   0 moky       (501) staff       (20)    14023 2024-05-07 18:39:52.000000 dimples-1.1.0/dimples/server/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5487 2024-05-15 18:45:11.000000 dimples-1.1.0/dimples/server/push.py
--rw-r--r--   0 moky       (501) staff       (20)     9709 2024-05-15 19:26:41.000000 dimples-1.1.0/dimples/server/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-1.1.0/dimples/server/session_center.py
--rw-r--r--   0 moky       (501) staff       (20)    10121 2023-12-05 04:21:35.000000 dimples-1.1.0/dimples/server/trace.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples/station/
--rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-1.1.0/dimples/station/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3029 2024-05-10 14:24:22.000000 dimples-1.1.0/dimples/station/handler.py
--rw-r--r--   0 moky       (501) staff       (20)     7523 2024-05-15 16:32:16.000000 dimples-1.1.0/dimples/station/shared.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3755 2024-05-09 16:42:05.000000 dimples-1.1.0/dimples/station/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples/utils/
--rw-r--r--   0 moky       (501) staff       (20)     5465 2024-05-15 19:28:18.000000 dimples-1.1.0/dimples/utils/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6512 2024-05-14 14:54:42.000000 dimples-1.1.0/dimples/utils/cache.py
--rw-r--r--   0 moky       (501) staff       (20)     6696 2024-04-23 09:37:33.000000 dimples-1.1.0/dimples/utils/config.py
--rw-r--r--   0 moky       (501) staff       (20)     7057 2024-05-14 14:54:42.000000 dimples-1.1.0/dimples/utils/dos.py
--rw-r--r--   0 moky       (501) staff       (20)     2761 2023-10-13 09:39:33.000000 dimples-1.1.0/dimples/utils/log.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)     3980 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)      118 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples.egg-info/entry_points.txt
--rw-r--r--   0 moky       (501) staff       (20)      104 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        8 2024-05-15 19:36:14.000000 dimples-1.1.0/dimples.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-15 19:36:14.000000 dimples-1.1.0/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1671 2024-05-15 19:23:14.000000 dimples-1.1.0/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2024-05-17 17:33:06.000000 dimples-1.2.0/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-1.2.0/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/
+-rw-r--r--   0 moky       (501) staff       (20)     8913 2024-04-11 15:45:18.000000 dimples-1.2.0/dimples/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/client/
+-rw-r--r--   0 moky       (501) staff       (20)     1977 2023-12-05 04:36:14.000000 dimples-1.2.0/dimples/client/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10946 2024-05-07 03:48:04.000000 dimples-1.2.0/dimples/client/archivist.py
+-rw-r--r--   0 moky       (501) staff       (20)     3862 2024-04-24 03:33:53.000000 dimples-1.2.0/dimples/client/checkpoint.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/client/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     2287 2023-10-29 13:43:35.000000 dimples-1.2.0/dimples/client/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     1952 2024-05-07 03:28:52.000000 dimples-1.2.0/dimples/client/cpu/commands.py
+-rw-r--r--   0 moky       (501) staff       (20)     4803 2023-10-29 13:43:46.000000 dimples-1.2.0/dimples/client/cpu/creator.py
+-rw-r--r--   0 moky       (501) staff       (20)     9096 2024-05-07 16:12:33.000000 dimples-1.2.0/dimples/client/cpu/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     2173 2024-05-07 03:32:12.000000 dimples-1.2.0/dimples/client/cpu/grp_expel.py
+-rw-r--r--   0 moky       (501) staff       (20)     5937 2024-05-07 03:34:38.000000 dimples-1.2.0/dimples/client/cpu/grp_invite.py
+-rw-r--r--   0 moky       (501) staff       (20)     3998 2024-05-07 03:35:17.000000 dimples-1.2.0/dimples/client/cpu/grp_join.py
+-rw-r--r--   0 moky       (501) staff       (20)     4177 2024-05-07 03:35:53.000000 dimples-1.2.0/dimples/client/cpu/grp_query.py
+-rw-r--r--   0 moky       (501) staff       (20)     4388 2024-05-07 03:36:21.000000 dimples-1.2.0/dimples/client/cpu/grp_quit.py
+-rw-r--r--   0 moky       (501) staff       (20)     5711 2024-05-07 03:36:56.000000 dimples-1.2.0/dimples/client/cpu/grp_reset.py
+-rw-r--r--   0 moky       (501) staff       (20)     4086 2024-05-07 03:37:19.000000 dimples-1.2.0/dimples/client/cpu/grp_resign.py
+-rw-r--r--   0 moky       (501) staff       (20)     5184 2024-05-07 03:50:13.000000 dimples-1.2.0/dimples/client/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     6404 2024-05-06 19:03:39.000000 dimples-1.2.0/dimples/client/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     9059 2024-05-07 03:49:36.000000 dimples-1.2.0/dimples/client/messenger.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/client/network/
+-rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-1.2.0/dimples/client/network/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7030 2024-05-09 20:14:55.000000 dimples-1.2.0/dimples/client/network/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     9334 2024-05-17 15:29:08.000000 dimples-1.2.0/dimples/client/network/state.py
+-rw-r--r--   0 moky       (501) staff       (20)     9501 2024-03-06 17:49:03.000000 dimples-1.2.0/dimples/client/network/transition.py
+-rw-r--r--   0 moky       (501) staff       (20)     9296 2024-05-07 03:57:08.000000 dimples-1.2.0/dimples/client/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     6077 2024-05-07 04:00:01.000000 dimples-1.2.0/dimples/client/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5497 2024-05-17 16:36:59.000000 dimples-1.2.0/dimples/client/terminal.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/common/
+-rw-r--r--   0 moky       (501) staff       (20)     2652 2024-04-11 16:03:38.000000 dimples-1.2.0/dimples/common/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3520 2023-10-19 02:46:00.000000 dimples-1.2.0/dimples/common/anonymous.py
+-rw-r--r--   0 moky       (501) staff       (20)     5771 2023-10-13 10:02:36.000000 dimples-1.2.0/dimples/common/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     7930 2024-05-06 18:08:29.000000 dimples-1.2.0/dimples/common/archivist.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/common/compat/
+-rw-r--r--   0 moky       (501) staff       (20)     2751 2023-10-13 16:15:07.000000 dimples-1.2.0/dimples/common/compat/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3806 2023-10-15 03:29:15.000000 dimples-1.2.0/dimples/common/compat/btc.py
+-rw-r--r--   0 moky       (501) staff       (20)     6666 2023-10-15 03:31:01.000000 dimples-1.2.0/dimples/common/compat/compatible.py
+-rw-r--r--   0 moky       (501) staff       (20)     2572 2023-10-13 10:09:19.000000 dimples-1.2.0/dimples/common/compat/entity.py
+-rw-r--r--   0 moky       (501) staff       (20)     6277 2023-10-17 15:21:36.000000 dimples-1.2.0/dimples/common/compat/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     6192 2023-10-13 10:09:24.000000 dimples-1.2.0/dimples/common/compat/network.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/common/dbi/
+-rw-r--r--   0 moky       (501) staff       (20)     2146 2023-10-15 04:04:22.000000 dimples-1.2.0/dimples/common/dbi/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7648 2024-05-06 18:49:56.000000 dimples-1.2.0/dimples/common/dbi/account.py
+-rw-r--r--   0 moky       (501) staff       (20)     2735 2024-05-06 18:36:11.000000 dimples-1.2.0/dimples/common/dbi/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     8062 2024-05-17 16:09:01.000000 dimples-1.2.0/dimples/common/dbi/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     8591 2024-05-07 18:41:02.000000 dimples-1.2.0/dimples/common/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     9209 2024-05-07 18:48:04.000000 dimples-1.2.0/dimples/common/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     8616 2024-05-06 18:15:14.000000 dimples-1.2.0/dimples/common/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     2999 2024-05-07 18:46:08.000000 dimples-1.2.0/dimples/common/processer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/common/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     2695 2023-10-29 10:59:58.000000 dimples-1.2.0/dimples/common/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3426 2023-10-13 12:48:25.000000 dimples-1.2.0/dimples/common/protocol/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     2611 2023-10-29 11:52:51.000000 dimples-1.2.0/dimples/common/protocol/block.py
+-rw-r--r--   0 moky       (501) staff       (20)     5211 2023-10-13 12:47:14.000000 dimples-1.2.0/dimples/common/protocol/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4897 2023-12-03 07:02:16.000000 dimples-1.2.0/dimples/common/protocol/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2619 2023-10-29 11:53:00.000000 dimples-1.2.0/dimples/common/protocol/mute.py
+-rw-r--r--   0 moky       (501) staff       (20)     2620 2023-10-13 12:45:16.000000 dimples-1.2.0/dimples/common/protocol/report.py
+-rw-r--r--   0 moky       (501) staff       (20)     6346 2024-05-06 18:17:07.000000 dimples-1.2.0/dimples/common/register.py
+-rw-r--r--   0 moky       (501) staff       (20)     4591 2024-05-07 18:47:41.000000 dimples-1.2.0/dimples/common/session.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/conn/
+-rw-r--r--   0 moky       (501) staff       (20)     4508 2024-05-14 15:03:49.000000 dimples-1.2.0/dimples/conn/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6276 2024-05-17 15:29:08.000000 dimples-1.2.0/dimples/conn/flexible.py
+-rw-r--r--   0 moky       (501) staff       (20)    10956 2024-05-14 15:09:23.000000 dimples-1.2.0/dimples/conn/gate.py
+-rw-r--r--   0 moky       (501) staff       (20)    12264 2024-05-15 19:21:42.000000 dimples-1.2.0/dimples/conn/gatekeeper.py
+-rw-r--r--   0 moky       (501) staff       (20)    10810 2024-05-14 15:15:47.000000 dimples-1.2.0/dimples/conn/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     8002 2024-05-14 15:15:53.000000 dimples-1.2.0/dimples/conn/mtp.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/conn/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     1916 2024-05-14 15:15:34.000000 dimples-1.2.0/dimples/conn/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8771 2024-04-23 09:39:58.000000 dimples-1.2.0/dimples/conn/protocol/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     8992 2024-05-14 15:42:00.000000 dimples-1.2.0/dimples/conn/protocol/ws.py
+-rw-r--r--   0 moky       (501) staff       (20)     6452 2024-05-16 07:26:50.000000 dimples-1.2.0/dimples/conn/queue.py
+-rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-1.2.0/dimples/conn/seeker.py
+-rw-r--r--   0 moky       (501) staff       (20)     4407 2024-05-16 07:24:50.000000 dimples-1.2.0/dimples/conn/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     7926 2024-05-17 15:29:08.000000 dimples-1.2.0/dimples/conn/ws.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/database/
+-rw-r--r--   0 moky       (501) staff       (20)     2812 2023-10-15 04:57:38.000000 dimples-1.2.0/dimples/database/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8179 2024-05-06 18:51:03.000000 dimples-1.2.0/dimples/database/account.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/database/dos/
+-rw-r--r--   0 moky       (501) staff       (20)     1949 2023-10-14 04:19:29.000000 dimples-1.2.0/dimples/database/dos/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4692 2024-05-14 14:54:42.000000 dimples-1.2.0/dimples/database/dos/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     6360 2024-05-06 18:30:09.000000 dimples-1.2.0/dimples/database/dos/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     5247 2024-05-06 18:21:39.000000 dimples-1.2.0/dimples/database/dos/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     6045 2024-05-06 18:50:27.000000 dimples-1.2.0/dimples/database/dos/group_history.py
+-rw-r--r--   0 moky       (501) staff       (20)     2789 2024-05-06 18:39:54.000000 dimples-1.2.0/dimples/database/dos/group_keys.py
+-rw-r--r--   0 moky       (501) staff       (20)     3101 2024-05-06 18:24:21.000000 dimples-1.2.0/dimples/database/dos/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2646 2024-05-06 18:24:29.000000 dimples-1.2.0/dimples/database/dos/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5553 2024-05-06 18:24:46.000000 dimples-1.2.0/dimples/database/dos/private.py
+-rw-r--r--   0 moky       (501) staff       (20)     8045 2024-05-06 18:26:43.000000 dimples-1.2.0/dimples/database/dos/station.py
+-rw-r--r--   0 moky       (501) staff       (20)     2941 2024-05-06 18:27:02.000000 dimples-1.2.0/dimples/database/dos/user.py
+-rw-r--r--   0 moky       (501) staff       (20)     3760 2024-05-06 18:51:40.000000 dimples-1.2.0/dimples/database/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     4436 2024-05-06 18:53:13.000000 dimples-1.2.0/dimples/database/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     3132 2024-05-06 18:27:39.000000 dimples-1.2.0/dimples/database/t_cipherkey.py
+-rw-r--r--   0 moky       (501) staff       (20)     4147 2024-05-06 18:30:39.000000 dimples-1.2.0/dimples/database/t_document.py
+-rw-r--r--   0 moky       (501) staff       (20)     6567 2024-05-06 18:31:50.000000 dimples-1.2.0/dimples/database/t_group.py
+-rw-r--r--   0 moky       (501) staff       (20)     5809 2024-05-06 18:50:47.000000 dimples-1.2.0/dimples/database/t_group_history.py
+-rw-r--r--   0 moky       (501) staff       (20)     4295 2024-05-06 18:41:59.000000 dimples-1.2.0/dimples/database/t_group_keys.py
+-rw-r--r--   0 moky       (501) staff       (20)     4246 2024-05-06 18:41:59.000000 dimples-1.2.0/dimples/database/t_login.py
+-rw-r--r--   0 moky       (501) staff       (20)     4405 2024-05-06 18:39:12.000000 dimples-1.2.0/dimples/database/t_message.py
+-rw-r--r--   0 moky       (501) staff       (20)     3756 2024-05-06 18:41:59.000000 dimples-1.2.0/dimples/database/t_meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5909 2024-05-06 18:42:32.000000 dimples-1.2.0/dimples/database/t_private.py
+-rw-r--r--   0 moky       (501) staff       (20)     6845 2024-05-06 18:44:20.000000 dimples-1.2.0/dimples/database/t_station.py
+-rw-r--r--   0 moky       (501) staff       (20)     3578 2024-05-06 18:45:26.000000 dimples-1.2.0/dimples/database/t_user.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/edge/
+-rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-1.2.0/dimples/edge/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    16117 2024-05-17 16:38:00.000000 dimples-1.2.0/dimples/edge/octopus.py
+-rw-r--r--   0 moky       (501) staff       (20)     6161 2024-05-15 16:34:13.000000 dimples-1.2.0/dimples/edge/shared.py
+-rw-r--r--   0 moky       (501) staff       (20)     2854 2024-05-17 16:40:17.000000 dimples-1.2.0/dimples/edge/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/group/
+-rw-r--r--   0 moky       (501) staff       (20)     1874 2023-10-18 14:55:15.000000 dimples-1.2.0/dimples/group/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6217 2024-05-06 18:55:34.000000 dimples-1.2.0/dimples/group/admin.py
+-rw-r--r--   0 moky       (501) staff       (20)     7191 2024-05-06 19:06:23.000000 dimples-1.2.0/dimples/group/builder.py
+-rw-r--r--   0 moky       (501) staff       (20)     7337 2024-05-06 19:05:04.000000 dimples-1.2.0/dimples/group/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)    12302 2024-05-06 19:12:10.000000 dimples-1.2.0/dimples/group/emitter.py
+-rw-r--r--   0 moky       (501) staff       (20)     5351 2024-05-16 07:07:02.000000 dimples-1.2.0/dimples/group/helper.py
+-rw-r--r--   0 moky       (501) staff       (20)    16535 2024-05-06 19:16:50.000000 dimples-1.2.0/dimples/group/manager.py
+-rw-r--r--   0 moky       (501) staff       (20)     5084 2024-05-06 19:10:38.000000 dimples-1.2.0/dimples/group/packer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/register/
+-rw-r--r--   0 moky       (501) staff       (20)     1441 2024-04-25 15:20:32.000000 dimples-1.2.0/dimples/register/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10595 2024-05-10 10:25:00.000000 dimples-1.2.0/dimples/register/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     8248 2024-05-10 10:25:44.000000 dimples-1.2.0/dimples/register/ext.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3901 2024-05-14 14:54:42.000000 dimples-1.2.0/dimples/register/run.py
+-rw-r--r--   0 moky       (501) staff       (20)     4151 2024-05-07 17:52:52.000000 dimples-1.2.0/dimples/register/shared.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/server/
+-rw-r--r--   0 moky       (501) staff       (20)     2448 2024-02-17 14:40:02.000000 dimples-1.2.0/dimples/server/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7502 2024-05-07 17:25:09.000000 dimples-1.2.0/dimples/server/archivist.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/server/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     1779 2023-07-05 16:57:44.000000 dimples-1.2.0/dimples/server/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2729 2024-05-07 04:03:19.000000 dimples-1.2.0/dimples/server/cpu/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     4857 2024-05-07 04:03:27.000000 dimples-1.2.0/dimples/server/cpu/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     4035 2024-05-07 04:22:27.000000 dimples-1.2.0/dimples/server/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4234 2024-05-07 04:22:59.000000 dimples-1.2.0/dimples/server/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     3539 2024-05-07 04:23:05.000000 dimples-1.2.0/dimples/server/cpu/report.py
+-rw-r--r--   0 moky       (501) staff       (20)    17809 2024-05-17 16:24:28.000000 dimples-1.2.0/dimples/server/dispatcher.py
+-rw-r--r--   0 moky       (501) staff       (20)     4574 2024-05-07 17:29:24.000000 dimples-1.2.0/dimples/server/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     6584 2024-05-07 04:15:23.000000 dimples-1.2.0/dimples/server/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)    14023 2024-05-07 18:39:52.000000 dimples-1.2.0/dimples/server/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5587 2024-05-17 16:32:27.000000 dimples-1.2.0/dimples/server/push.py
+-rw-r--r--   0 moky       (501) staff       (20)     9537 2024-05-17 16:43:59.000000 dimples-1.2.0/dimples/server/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-1.2.0/dimples/server/session_center.py
+-rw-r--r--   0 moky       (501) staff       (20)    10121 2023-12-05 04:21:35.000000 dimples-1.2.0/dimples/server/trace.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/station/
+-rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-1.2.0/dimples/station/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3112 2024-05-17 16:55:26.000000 dimples-1.2.0/dimples/station/handler.py
+-rw-r--r--   0 moky       (501) staff       (20)     7523 2024-05-15 16:32:16.000000 dimples-1.2.0/dimples/station/shared.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3755 2024-05-09 16:42:05.000000 dimples-1.2.0/dimples/station/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples/utils/
+-rw-r--r--   0 moky       (501) staff       (20)     4722 2024-05-17 15:32:17.000000 dimples-1.2.0/dimples/utils/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6250 2024-05-17 15:44:13.000000 dimples-1.2.0/dimples/utils/cache.py
+-rw-r--r--   0 moky       (501) staff       (20)     6696 2024-04-23 09:37:33.000000 dimples-1.2.0/dimples/utils/config.py
+-rw-r--r--   0 moky       (501) staff       (20)     7057 2024-05-14 14:54:42.000000 dimples-1.2.0/dimples/utils/dos.py
+-rw-r--r--   0 moky       (501) staff       (20)     2761 2023-10-13 09:39:33.000000 dimples-1.2.0/dimples/utils/log.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)     3980 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)      118 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples.egg-info/entry_points.txt
+-rw-r--r--   0 moky       (501) staff       (20)      104 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        8 2024-05-17 17:33:06.000000 dimples-1.2.0/dimples.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-17 17:33:06.000000 dimples-1.2.0/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1671 2024-05-17 16:46:53.000000 dimples-1.2.0/setup.py
```

### Comparing `dimples-1.1.0/PKG-INFO` & `dimples-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 1.1.0
+Version: 1.2.0
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-1.1.0/README.md` & `dimples-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/__init__.py` & `dimples-1.2.0/dimples/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/__init__.py` & `dimples-1.2.0/dimples/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/archivist.py` & `dimples-1.2.0/dimples/client/archivist.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/checkpoint.py` & `dimples-1.2.0/dimples/client/checkpoint.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/cpu/__init__.py` & `dimples-1.2.0/dimples/client/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/cpu/commands.py` & `dimples-1.2.0/dimples/client/cpu/commands.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/cpu/creator.py` & `dimples-1.2.0/dimples/client/cpu/creator.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/cpu/group.py` & `dimples-1.2.0/dimples/client/cpu/group.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/cpu/grp_expel.py` & `dimples-1.2.0/dimples/client/cpu/grp_expel.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/cpu/grp_invite.py` & `dimples-1.2.0/dimples/client/cpu/grp_invite.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/cpu/grp_join.py` & `dimples-1.2.0/dimples/client/cpu/grp_join.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/cpu/grp_query.py` & `dimples-1.2.0/dimples/client/cpu/grp_query.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/cpu/grp_quit.py` & `dimples-1.2.0/dimples/client/cpu/grp_quit.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/cpu/grp_reset.py` & `dimples-1.2.0/dimples/client/cpu/grp_reset.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/cpu/grp_resign.py` & `dimples-1.2.0/dimples/client/cpu/grp_resign.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/cpu/handshake.py` & `dimples-1.2.0/dimples/client/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/facebook.py` & `dimples-1.2.0/dimples/client/facebook.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/messenger.py` & `dimples-1.2.0/dimples/client/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/network/__init__.py` & `dimples-1.2.0/dimples/client/network/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/network/session.py` & `dimples-1.2.0/dimples/client/network/session.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/network/state.py` & `dimples-1.2.0/dimples/client/network/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import weakref
 from abc import ABC
 from enum import IntEnum
 from typing import Optional, Union
 
 from dimsdk import ID
 
-from startrek.fsm import Runner
+from startrek.skywalker import Runner
 from startrek.fsm import Context, BaseTransition, BaseState, AutoMachine
 from startrek import Docker, DockerStatus
 
 # from .session import ClientSession
 
 
 class StateMachine(AutoMachine, Context):
```

### Comparing `dimples-1.1.0/dimples/client/network/transition.py` & `dimples-1.2.0/dimples/client/network/transition.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/packer.py` & `dimples-1.2.0/dimples/client/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/processor.py` & `dimples-1.2.0/dimples/client/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/client/terminal.py` & `dimples-1.2.0/dimples/client/terminal.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     Client
 """
 
 import time
 
 from dimples import EntityType
 
-from ..utils import DaemonRunner, Logging
+from ..utils import Logging
+from ..utils import Runner
 from ..utils import StateDelegate
 
 from .network import ClientSession
 from .network import StateMachine, SessionState
 from .network.state import StateOrder
 
 from .messenger import ClientMessenger
@@ -47,15 +48,15 @@
 class DeviceMixin:
 
     @property
     def user_agent(self) -> str:
         return 'DIMP/0.4 (Client; Linux; en-US) DIMCoreKit/0.9 (Terminal) DIM-by-GSP/1.0'
 
 
-class Terminal(DaemonRunner, DeviceMixin, Logging, StateDelegate):
+class Terminal(Runner, DeviceMixin, Logging, StateDelegate):
 
     def __init__(self, messenger: ClientMessenger):
         super().__init__(interval=60)
         self.__messenger = messenger
         # default online time
         self.__last_time = time.time()
 
@@ -70,23 +71,21 @@
     @property  # Override
     def running(self) -> bool:
         if super().running:
             return self.session.running
 
     # Override
     async def setup(self):
-        await super().setup()
         session = self.session
         session.fsm.delegate = self
         await session.start()
 
     # Override
     async def finish(self):
         await self.session.stop()
-        await super().finish()
 
     # Override
     async def process(self) -> bool:
         now = time.time()
         if now < (self.__last_time + 300):
             # last sent within 5 minutes
             return False
```

### Comparing `dimples-1.1.0/dimples/common/__init__.py` & `dimples-1.2.0/dimples/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/anonymous.py` & `dimples-1.2.0/dimples/common/anonymous.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/ans.py` & `dimples-1.2.0/dimples/common/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/archivist.py` & `dimples-1.2.0/dimples/common/archivist.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/compat/__init__.py` & `dimples-1.2.0/dimples/common/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/compat/btc.py` & `dimples-1.2.0/dimples/common/compat/btc.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/compat/compatible.py` & `dimples-1.2.0/dimples/common/compat/compatible.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/compat/entity.py` & `dimples-1.2.0/dimples/common/compat/entity.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/compat/meta.py` & `dimples-1.2.0/dimples/common/compat/meta.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/compat/network.py` & `dimples-1.2.0/dimples/common/compat/network.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/dbi/__init__.py` & `dimples-1.2.0/dimples/common/dbi/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/dbi/account.py` & `dimples-1.2.0/dimples/common/dbi/account.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/dbi/message.py` & `dimples-1.2.0/dimples/common/dbi/message.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/dbi/session.py` & `dimples-1.2.0/dimples/common/dbi/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,19 +209,21 @@
 
     @abstractmethod
     async def all_stations(self, provider: ID) -> List[StationInfo]:
         """ get list of (host, port, SP_ID, chosen) """
         raise NotImplemented
 
     @abstractmethod
-    async def add_station(self, identifier: Optional[ID], host: str, port: int, provider: ID, chosen: int = 0) -> bool:
+    async def add_station(self, identifier: Optional[ID], host: str, port: int, provider: ID,
+                          chosen: int = 0) -> bool:
         raise NotImplemented
 
     @abstractmethod
-    async def update_station(self, identifier: Optional[ID], host: str, port: int, provider: ID, chosen: int = None) -> bool:
+    async def update_station(self, identifier: Optional[ID], host: str, port: int, provider: ID,
+                             chosen: int = None) -> bool:
         raise NotImplemented
 
     @abstractmethod
     async def remove_station(self, host: str, port: int, provider: ID) -> bool:
         raise NotImplemented
 
     @abstractmethod
```

### Comparing `dimples-1.1.0/dimples/common/facebook.py` & `dimples-1.2.0/dimples/common/facebook.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/messenger.py` & `dimples-1.2.0/dimples/common/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/packer.py` & `dimples-1.2.0/dimples/common/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/processer.py` & `dimples-1.2.0/dimples/common/processer.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/protocol/__init__.py` & `dimples-1.2.0/dimples/common/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/protocol/ans.py` & `dimples-1.2.0/dimples/common/protocol/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/protocol/block.py` & `dimples-1.2.0/dimples/common/protocol/block.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/protocol/handshake.py` & `dimples-1.2.0/dimples/common/protocol/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/protocol/login.py` & `dimples-1.2.0/dimples/common/protocol/login.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/protocol/mute.py` & `dimples-1.2.0/dimples/common/protocol/mute.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/protocol/report.py` & `dimples-1.2.0/dimples/common/protocol/report.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/register.py` & `dimples-1.2.0/dimples/common/register.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/common/session.py` & `dimples-1.2.0/dimples/common/session.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/conn/__init__.py` & `dimples-1.2.0/dimples/conn/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/conn/flexible.py` & `dimples-1.2.0/dimples/conn/flexible.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 from typing import Optional, Union, List
 
 from startrek.types import SocketAddress
-from startrek.fsm import Runner
+from startrek.skywalker import Runner
 from startrek import Connection
 from startrek import Arrival, Departure
 from startrek import StarDocker
 
 from .protocol import DeparturePacker
 
 from .ws import WSDocker
```

### Comparing `dimples-1.1.0/dimples/conn/gate.py` & `dimples-1.2.0/dimples/conn/gate.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/conn/gatekeeper.py` & `dimples-1.2.0/dimples/conn/gatekeeper.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/conn/mars.py` & `dimples-1.2.0/dimples/conn/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/conn/mtp.py` & `dimples-1.2.0/dimples/conn/mtp.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/conn/protocol/__init__.py` & `dimples-1.2.0/dimples/conn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/conn/protocol/mars.py` & `dimples-1.2.0/dimples/conn/protocol/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/conn/protocol/ws.py` & `dimples-1.2.0/dimples/conn/protocol/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/conn/queue.py` & `dimples-1.2.0/dimples/conn/queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,18 +108,18 @@
                 # 1.1. create new array for this priority
                 fleet = []
                 self.__fleets[priority] = fleet
                 # 1.2. insert the priority in a sorted list
                 self.__insert(priority=priority)
             else:
                 # 1.3. check duplicated
-                signature = msg.get('signature')
                 for wrapper in fleet:
                     item = wrapper.msg
                     if self.__is_duplicated(item, msg):
+                        signature = msg.get('signature')
                         print('[QUEUE] duplicated message: %s' % signature)
                         return False
             # 2. append with wrapper
             wrapper = MessageWrapper(msg=msg, ship=ship)
             fleet.append(wrapper)
             return True
```

### Comparing `dimples-1.1.0/dimples/conn/seeker.py` & `dimples-1.2.0/dimples/conn/seeker.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/conn/session.py` & `dimples-1.2.0/dimples/conn/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,17 @@
     @messenger.setter
     def messenger(self, transceiver: CommonMessenger):
         self.__messenger = None if transceiver is None else weakref.ref(transceiver)
 
     # Override
     async def queue_message_package(self, msg: ReliableMessage, data: bytes, priority: int = 0) -> bool:
         ship = await self._docker_pack(payload=data, priority=priority)
-        if ship is not None:
+        if ship is None:
+            self.error(msg='failed to pack msg: %s -> %s, %s' % (msg.sender, msg.receiver, msg.group))
+        else:
             return self._queue_append(msg=msg, ship=ship)
 
     #
     #   Transmitter
     #
 
     # Override
```

### Comparing `dimples-1.1.0/dimples/conn/ws.py` & `dimples-1.2.0/dimples/conn/ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # ==============================================================================
 
 import socket
 import threading
 from typing import Optional, List, Tuple
 
 from startrek.types import SocketAddress
-from startrek.fsm import Runner
+from startrek.skywalker import Runner
 from startrek import Arrival, Departure
 from startrek import ArrivalShip, DepartureShip, DeparturePriority
 from startrek import BaseConnection, BaseChannel
 
 from tcp import PlainDocker
 
 from .protocol import WebSocket
```

### Comparing `dimples-1.1.0/dimples/database/__init__.py` & `dimples-1.2.0/dimples/database/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/account.py` & `dimples-1.2.0/dimples/database/account.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/dos/__init__.py` & `dimples-1.2.0/dimples/database/dos/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/dos/base.py` & `dimples-1.2.0/dimples/database/dos/base.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/dos/document.py` & `dimples-1.2.0/dimples/database/dos/document.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/dos/group.py` & `dimples-1.2.0/dimples/database/dos/group.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/dos/group_history.py` & `dimples-1.2.0/dimples/database/dos/group_history.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/dos/group_keys.py` & `dimples-1.2.0/dimples/database/dos/group_keys.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/dos/login.py` & `dimples-1.2.0/dimples/database/dos/login.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/dos/meta.py` & `dimples-1.2.0/dimples/database/dos/meta.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/dos/private.py` & `dimples-1.2.0/dimples/database/dos/private.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/dos/station.py` & `dimples-1.2.0/dimples/database/dos/station.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/dos/user.py` & `dimples-1.2.0/dimples/database/dos/user.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/message.py` & `dimples-1.2.0/dimples/database/message.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/session.py` & `dimples-1.2.0/dimples/database/session.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/t_cipherkey.py` & `dimples-1.2.0/dimples/database/t_cipherkey.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/t_document.py` & `dimples-1.2.0/dimples/database/t_document.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/t_group.py` & `dimples-1.2.0/dimples/database/t_group.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/t_group_history.py` & `dimples-1.2.0/dimples/database/t_group_history.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/t_group_keys.py` & `dimples-1.2.0/dimples/database/t_group_keys.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/t_login.py` & `dimples-1.2.0/dimples/database/t_login.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/t_message.py` & `dimples-1.2.0/dimples/database/t_message.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/t_meta.py` & `dimples-1.2.0/dimples/database/t_meta.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/t_private.py` & `dimples-1.2.0/dimples/database/t_private.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/t_station.py` & `dimples-1.2.0/dimples/database/t_station.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/database/t_user.py` & `dimples-1.2.0/dimples/database/t_user.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/edge/__init__.py` & `dimples-1.2.0/dimples/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/edge/octopus.py` & `dimples-1.2.0/dimples/edge/octopus.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 from dimsdk import ContentType
 from dimsdk import EntityType, ID
 from dimsdk import ReliableMessage
 from dimsdk import Station
 
 from ..utils import Log, Logging
-from ..utils import Runner, DaemonRunner
+from ..utils import Runner
 from ..utils import get_msg_sig
 from ..common import ProviderInfo
 from ..common import MessageDBI, SessionDBI
 from ..common import HandshakeCommand
 
 from ..client import ClientSession
 from ..client import ClientFacebook
@@ -54,15 +54,15 @@
 from ..client import ClientMessageProcessor
 from ..client import Terminal
 
 from .shared import GlobalVariable
 from .shared import create_session
 
 
-class Octopus(DaemonRunner, Logging):
+class Octopus(Runner, Logging):
 
     def __init__(self, shared: GlobalVariable, local_host: str = '127.0.0.1', local_port: int = 9394):
         super().__init__(interval=60)
         self.__shared = shared
         self.__inner = self.create_inner_terminal(host=local_host, port=local_port)
         self.__outers: Set[Terminal] = set()
         self.__outer_map = weakref.WeakValueDictionary()
@@ -139,14 +139,22 @@
             outers = set(self.__outers)
         for out in outers:
             await out.stop()
         # 3. stop runner
         await super().stop()
 
     # Override
+    async def setup(self):
+        pass
+
+    # Override
+    async def finish(self):
+        pass
+
+    # Override
     async def process(self) -> bool:
         # get all neighbor stations
         db = self.database
         providers = await db.all_providers()
         assert len(providers) > 0, 'service provider not found'
         gsp = providers[0].identifier
         neighbors = await db.all_stations(provider=gsp)
@@ -376,15 +384,15 @@
     session.messenger = messenger
     return messenger
 
 
 def create_terminal(messenger: OctopusMessenger) -> Terminal:
     terminal = Terminal(messenger=messenger)
     messenger.terminal = terminal
-    Runner.thread_run(terminal)
+    Runner.thread_run(runner=terminal)
     return terminal
 
 
 async def update_station(station: Station, database: SessionDBI):
     Log.info(msg='update station: %s' % station)
     # SP ID
     provider = station.provider
```

### Comparing `dimples-1.1.0/dimples/edge/shared.py` & `dimples-1.2.0/dimples/edge/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/edge/start.py` & `dimples-1.2.0/dimples/edge/start.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,13 @@
     shared.facebook = facebook
     # create & start octopus
     host = config.station_host
     port = config.station_port
     assert host is not None and port > 0, 'station config error: %s' % config
     octopus = Octopus(shared=shared, local_host=host, local_port=port)
     await octopus.start()
-    while octopus.running:
-        await Runner.sleep(seconds=1.0)
+    await octopus.run()
     Log.warning(msg='bot stopped: %s' % octopus)
 
 
 if __name__ == '__main__':
     Runner.sync_run(main=main())
```

### Comparing `dimples-1.1.0/dimples/group/__init__.py` & `dimples-1.2.0/dimples/group/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/group/admin.py` & `dimples-1.2.0/dimples/group/admin.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/group/builder.py` & `dimples-1.2.0/dimples/group/builder.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/group/delegate.py` & `dimples-1.2.0/dimples/group/delegate.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/group/emitter.py` & `dimples-1.2.0/dimples/group/emitter.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/group/helper.py` & `dimples-1.2.0/dimples/group/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         return self.delegate.facebook.archivist.database
 
     #
     #   Group History Command
     #
 
     async def save_group_history(self, group: ID, content: GroupCommand, message: ReliableMessage) -> bool:
-        if self.is_expired(content=content):
+        if await self.is_expired(content=content):
             self.warning(msg='drop expired command: %s, %s => %s' % (content.cmd, message.sender, group))
             return False
         # check command time
         cmd_time = content.time
         if cmd_time is None:
             self.error(msg='group command error: %s' % content)
         else:
@@ -110,14 +110,15 @@
             if doc is None:
                 self.error(msg='group document not exists: %s' % group)
                 return True
             return is_before(old_time=doc.time, new_time=content.time)
         # membership command, check with reset command
         cmd, _ = await self.get_reset_command_message(group=group)
         if cmd is None:  # or msg is None:
+            self.error(msg='"reset" command not found: %s' % content)
             return False
         return is_before(old_time=cmd.time, new_time=content.time)
 
     # noinspection PyMethodMayBeStatic
     def members_from_command(self, content: GroupCommand) -> List[ID]:
         # get from 'members'
         members = content.members
```

### Comparing `dimples-1.1.0/dimples/group/manager.py` & `dimples-1.2.0/dimples/group/manager.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/group/packer.py` & `dimples-1.2.0/dimples/group/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/register/__init__.py` & `dimples-1.2.0/dimples/register/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/register/base.py` & `dimples-1.2.0/dimples/register/base.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/register/ext.py` & `dimples-1.2.0/dimples/register/ext.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/register/run.py` & `dimples-1.2.0/dimples/register/run.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/register/shared.py` & `dimples-1.2.0/dimples/register/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/server/__init__.py` & `dimples-1.2.0/dimples/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/server/archivist.py` & `dimples-1.2.0/dimples/server/archivist.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/server/cpu/__init__.py` & `dimples-1.2.0/dimples/server/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/server/cpu/ans.py` & `dimples-1.2.0/dimples/server/cpu/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/server/cpu/document.py` & `dimples-1.2.0/dimples/server/cpu/document.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/server/cpu/handshake.py` & `dimples-1.2.0/dimples/server/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/server/cpu/login.py` & `dimples-1.2.0/dimples/server/cpu/login.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/server/cpu/report.py` & `dimples-1.2.0/dimples/server/cpu/report.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/server/dispatcher.py` & `dimples-1.2.0/dimples/server/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from typing import Optional, Set, List
 
 from dimsdk import EntityType, ID, EVERYONE
 from dimsdk import Station
 from dimsdk import Content, ReceiptCommand
 from dimsdk import ReliableMessage
 
-from ..utils import Singleton, Log, Logging, Runner, DaemonRunner
+from ..utils import Singleton, Log, Logging, Runner
 from ..common import CommonFacebook
 from ..common import MessageDBI, SessionDBI
 from ..common import ReliableMessageDBI
 from ..common import LoginCommand
 
 from .session_center import SessionCenter
 from .push import PushCenter
@@ -130,15 +130,15 @@
         runner = self.__roamer
         if runner is None:
             db = self.mdb
             assert db is not None, 'dispatcher not initialized'
             runner = Roamer(database=db)
             self.__roamer = runner
             # Runner.async_run(coroutine=runner.start())
-            Runner.thread_run(runner)
+            Runner.thread_run(runner=runner)
         return runner
 
     def add_roaming(self, user: ID, station: ID) -> bool:
         """ Add roaming user with station """
         roamer = self.roamer
         return roamer.add_roaming(user=user, station=station)
 
@@ -271,15 +271,15 @@
 
     def __init__(self, user: ID, station: ID):
         super().__init__()
         self.user = user
         self.station = station
 
 
-class Roamer(DaemonRunner, Logging):
+class Roamer(Runner, Logging):
     """ Delegate for redirect cached messages to roamed station """
 
     def __init__(self, database: MessageDBI):
         super().__init__(interval=Runner.INTERVAL_SLOW)
         self.__database = database
         # roaming (user id => station id)
         self.__queue: List[RoamingInfo] = []
@@ -307,14 +307,22 @@
         :return: False on error
         """
         info = RoamingInfo(user=user, station=station)
         self.__append(info=info)
         return True
 
     # Override
+    async def setup(self):
+        pass
+
+    # Override
+    async def finish(self):
+        pass
+
+    # Override
     async def process(self) -> bool:
         info = self.__next()
         if info is None:
             # nothing to do
             return False
         receiver = info.user
         roaming = info.station
```

### Comparing `dimples-1.1.0/dimples/server/messenger.py` & `dimples-1.2.0/dimples/server/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/server/packer.py` & `dimples-1.2.0/dimples/server/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/server/processor.py` & `dimples-1.2.0/dimples/server/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/server/push.py` & `dimples-1.2.0/dimples/server/push.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import threading
 import time
 from abc import ABC, abstractmethod
 from typing import Optional, List, Dict
 
 from dimsdk import ID, ReliableMessage
 
-from ..utils import Runner, DaemonRunner
+from ..utils import Runner
 from ..utils import Singleton, Logging
 
 
 class MessageQueue(Logging):
 
     def __init__(self):
         super().__init__()
@@ -113,23 +113,23 @@
     @abstractmethod
     async def process(self, messages: List[ReliableMessage]) -> bool:
         """ build and push notification for a batch of messages """
         raise NotImplemented
 
 
 @Singleton
-class PushCenter(DaemonRunner, Logging):
+class PushCenter(Runner, Logging):
 
     def __init__(self):
         super().__init__(interval=Runner.INTERVAL_SLOW)
         self.__queue = MessageQueue()
         self.__keeper = BadgeKeeper()
         self.__service: Optional[PushService] = None
         # Runner.async_run(coroutine=self.start())
-        Runner.thread_run(self)
+        Runner.thread_run(runner=self)
 
     @property
     def service(self) -> Optional[PushService]:
         return self.__service
 
     @service.setter
     def service(self, pusher: PushService):
@@ -146,14 +146,22 @@
 
     def push_notification(self, msg: ReliableMessage):
         """ Push notification for msg receiver """
         queue = self.__queue
         queue.add_message(msg=msg)
 
     # Override
+    async def setup(self):
+        pass
+
+    # Override
+    async def finish(self):
+        pass
+
+    # Override
     async def process(self) -> bool:
         # 1. get waiting messages
         queue = self.__queue
         messages = queue.get_messages()
         if messages is None:
             # nothing to do now, return False to have a rest
             return False
```

### Comparing `dimples-1.1.0/dimples/server/session.py` & `dimples-1.2.0/dimples/server/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,33 +92,26 @@
     # Override
     def set_identifier(self, identifier: ID) -> bool:
         old = self.identifier
         if super().set_identifier(identifier=identifier):
             session_change_id(session=self, new_id=identifier, old_id=old)
             # load cached message asynchronously
             crt = load_cached_messages(session=self)
-            # Runner.async_run(coroutine=crt)
-            Runner.thread_run(crt)
+            Runner.async_run(coroutine=crt)
             return True
 
     # Override
     def set_active(self, active: bool, when: float = None) -> bool:
         if super().set_active(active=active, when=when):
             session_change_active(session=self, active=active)
             # load cached message asynchronously
             crt = load_cached_messages(session=self)
-            # Runner.async_run(coroutine=crt)
-            Runner.thread_run(crt)
+            Runner.async_run(coroutine=crt)
             return True
 
-    # Override
-    async def start(self):
-        await super().start()
-        await self.run()
-
     #
     #   Docker Delegate
     #
 
     # Override
     async def docker_status_changed(self, previous: DockerStatus, current: DockerStatus, docker: Docker):
         # super().docker_status_changed(previous=previous, current=current, docker=docker)
```

### Comparing `dimples-1.1.0/dimples/server/session_center.py` & `dimples-1.2.0/dimples/server/session_center.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/server/trace.py` & `dimples-1.2.0/dimples/server/trace.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/station/__init__.py` & `dimples-1.2.0/dimples/station/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/station/handler.py` & `dimples-1.2.0/dimples/station/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,28 +60,31 @@
         self.info(msg='request finished: %s' % str(self.client_address))
 
     # Override
     def handle(self):
         super().handle()
         try:
             self.info(msg='session started: %s' % str(self.client_address))
-            Runner.sync_run(main=start_session(client_address=self.client_address, request=self.request))
+            crt = _start_session(client_address=self.client_address, request=self.request)
+            Runner.sync_run(main=crt)
             self.info(msg='session finished: %s' % str(self.client_address))
         except Exception as error:
             self.error(msg='request handler error: %s' % error)
             traceback.print_exc()
 
 
-async def start_session(client_address, request):
+async def _start_session(client_address, request):
     shared = GlobalVariable()
     session = ServerSession(remote=client_address, sock=request, database=shared.sdb)
     messenger = create_messenger(facebook=shared.facebook, database=shared.mdb, session=session)
     center = SessionCenter()
     # setup
     center.add_session(session=session)
     try:
         # handle
         await session.start()
+        await session.run()
+        # await session.stop()
     finally:
         # finish
         center.remove_session(session=session)
     return messenger
```

### Comparing `dimples-1.1.0/dimples/station/shared.py` & `dimples-1.2.0/dimples/station/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/station/start.py` & `dimples-1.2.0/dimples/station/start.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/utils/__init__.py` & `dimples-1.2.0/dimples/utils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
     I'm too lazy to write codes for demo project, so I borrow some utils here
     from the <dimsdk> packages, but I don't suggest you to do it also, because
     I won't promise these private utils will not be changed. Hia hia~ :P
                                              -- Albert Moky @ Jan. 23, 2019
 """
 
-import threading
 from typing import Optional, List, Dict
 
 from dimsdk import md5, sha1, sha256, keccak256, ripemd160
 from dimsdk import base64_encode, base64_decode, base58_encode, base58_decode
 from dimsdk import hex_encode, hex_decode
 from dimsdk import utf8_encode, utf8_decode
 from dimsdk import json_encode, json_decode
@@ -47,19 +46,18 @@
 from dimsdk import Converter
 from dimsdk import DateTime
 from dimsdk import ReliableMessage
 from dimsdk import DocumentHelper
 
 from dimplugins.crypto.aes import random_bytes
 
-from startrek.fsm import Singleton
-from startrek.fsm import Runnable, Runner, Daemon, DaemonRunner
+from startrek.skywalker import Singleton
+from startrek.skywalker import Runnable, Runner, Daemon
 from startrek.fsm import Delegate as StateDelegate
-from startrek.net.channel import get_remote_address, get_local_address
-
+from startrek.net.socket import get_remote_address, get_local_address
 
 from .log import Log, Logging
 from .dos import Path, File, TextFile, JSONFile
 from .cache import CachePool, CacheHolder, CacheManager
 
 from .config import Config
 
@@ -119,15 +117,15 @@
     'utf8_encode', 'utf8_decode',
     'json_encode', 'json_decode',
 
     'random_bytes',
 
     'Converter',
 
-    'Runnable', 'Runner', 'Daemon', 'DaemonRunner',
+    'Runnable', 'Runner', 'Daemon',
     'StateDelegate',
 
     'get_remote_address', 'get_local_address',
 
 
     'Singleton',
     'Log', 'Logging',
@@ -139,41 +137,7 @@
     'Config',
 
     'is_before',
     'get_msg_sig', 'get_msg_info',
     'template_replace',
 
 ]
-
-
-#
-#   Patch for Runner
-#
-async def _run_forever(runner: Runner):
-    await runner.start()
-    while True:
-        await Runner.sleep(seconds=2.0)
-        if not runner.running:
-            break
-    Log.warning(msg='runner stopped: %s' % runner)
-
-
-def _start_runner(runner: Runner):
-    Runner.sync_run(main=_run_forever(runner=runner))
-
-
-def _start_coroutine(coroutine):
-    Runner.sync_run(main=coroutine)
-
-
-def _bg_run(target):
-    if isinstance(target, Runner):
-        fn = _start_runner
-    else:
-        fn = _start_coroutine
-    thr = threading.Thread(target=fn, args=(target,), daemon=True)
-    thr.start()
-    return thr
-
-
-""" Run coroutine in background thread """
-Runner.thread_run = _bg_run
```

### Comparing `dimples-1.1.0/dimples/utils/cache.py` & `dimples-1.2.0/dimples/utils/cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,18 +27,20 @@
     Database module
     ~~~~~~~~~~~~~~~
 
 """
 
 from typing import TypeVar, Generic, Optional, Dict, Set, Tuple
 
-from startrek.fsm import Singleton
-from startrek.fsm import Runnable, Runner, Daemon
+from startrek.skywalker import Singleton
+from startrek.skywalker import Runner
 from dimsdk import DateTime
 
+from .log import Logging
+
 
 K = TypeVar('K')
 V = TypeVar('V')
 
 
 class CacheHolder(Generic[V]):
 
@@ -129,52 +131,45 @@
                 # remove expired holders
                 self.__holders.pop(key, None)
                 count += 1
         return count
 
 
 @Singleton
-class CacheManager(Runnable):
+class CacheManager(Runner, Logging):
 
     def __init__(self):
+        super().__init__(interval=2.0)
         self.__pools: Dict[str, CachePool] = {}  # name -> pool
-        # thread for cleaning caches
-        self.__running = True
-        self.__daemon = Daemon(target=self)
-        self.__daemon.start()
+        self.__next_time = DateTime.now()
+        # Runner.async_run(coroutine=self.start())
+        Runner.thread_run(runner=self)
 
-    @property
-    def running(self) -> bool:
-        return self.__running
+    # Override
+    async def setup(self):
+        pass
 
-    async def stop(self):
-        # 1. mark this gate to stopped
-        self.__running = False
-        # 2. waiting for the gate to stop
-        await Runner.sleep(seconds=5)
-        # 3. cancel the async task
-        self.__daemon.stop()
+    # Override
+    async def finish(self):
+        pass
 
     # Override
-    async def run(self):
-        next_time = 0
-        while self.running:
-            # try to purge each 5 minutes
-            now = DateTime.now()
-            if now < next_time:
-                await Runner.sleep(seconds=2)
-                continue
-            else:
-                next_time = DateTime(now.timestamp + 300)
-            try:
-                count = self.purge(now=now)
-                print('[MEM] purge %d item(s) from cache pools' % count)
-            except Exception as error:
-                print('[MEM] failed to purge cache: %s' % error)
-        print('[MEM] stop %s' % self)
+    async def process(self) -> bool:
+        # try to purge each 5 minutes
+        now = DateTime.now()
+        if now < self.__next_time:
+            return False
+        else:
+            self.__next_time = DateTime(now.timestamp + 300)
+        # purge
+        try:
+            count = self.purge(now=now)
+            self.info(msg='[MEM] purge %d item(s) from cache pools' % count)
+        except Exception as error:
+            self.error(msg='[MEM] failed to purge cache: %s' % error)
 
     def get_pool(self, name: str) -> CachePool[K, V]:
         """ get pool with name """
         pool = self.__pools.get(name)
         if pool is None:
             pool = CachePool()
             self.__pools[name] = pool
```

### Comparing `dimples-1.1.0/dimples/utils/config.py` & `dimples-1.2.0/dimples/utils/config.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/utils/dos.py` & `dimples-1.2.0/dimples/utils/dos.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples/utils/log.py` & `dimples-1.2.0/dimples/utils/log.py`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/dimples.egg-info/PKG-INFO` & `dimples-1.2.0/dimples.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 1.1.0
+Version: 1.2.0
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-1.1.0/dimples.egg-info/SOURCES.txt` & `dimples-1.2.0/dimples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dimples-1.1.0/setup.py` & `dimples-1.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     communications between accounts safely by end-to-end encryption.
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '1.1.0'
+__version__ = '1.2.0'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
@@ -54,12 +54,12 @@
         'dimplugins>=2.0.0',
 
         'dimsdk>=2.0.0',
         'dimp>=2.0.0',
         'dkd>=2.0.0',
         'mkm>=2.0.0',
 
-        'startrek>=2.0.0',
-        'tcp>=2.0.0',
-        'udp>=2.0.0',
+        'startrek>=2.1.0',
+        'tcp>=2.1.0',
+        'udp>=2.1.0',
     ]
 )
```

