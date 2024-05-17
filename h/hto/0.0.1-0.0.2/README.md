# Comparing `tmp/hto-0.0.1.tar.gz` & `tmp/hto-0.0.2.tar.gz`

## Comparing `hto-0.0.1.tar` & `hto-0.0.2.tar`

### file list

```diff
@@ -1,938 +1,9 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 hto-0.0.1/hto/__about__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hto-0.0.1/hto/__init__.py
--rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 hto-0.0.1/hto/__main__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hto-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 hto-0.0.1/venv/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 hto-0.0.1/venv/bin/Activate.ps1
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 hto-0.0.1/venv/bin/activate
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 hto-0.0.1/venv/bin/activate.csh
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 hto-0.0.1/venv/bin/activate.fish
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 hto-0.0.1/venv/bin/distro
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 hto-0.0.1/venv/bin/httpx
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 hto-0.0.1/venv/bin/pip
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 hto-0.0.1/venv/bin/pip3
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 hto-0.0.1/venv/bin/pip3.12
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/bin/python -> /usr/bin/python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/bin/python3.12 -> python
--rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 hto-0.0.1/venv/bin/simple-term-menu
--rw-r--r--   0        0        0    91584 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/simple_term_menu.py
--rw-r--r--   0        0        0   122293 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/typing_extensions.py
--rw-r--r--   0        0        0    12151 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/annotated_types/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/annotated_types/py.typed
--rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/annotated_types/test_cases.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/annotated_types-0.6.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    12879 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/annotated_types-0.6.0.dist-info/METADATA
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/annotated_types-0.6.0.dist-info/RECORD
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/annotated_types-0.6.0.dist-info/WHEEL
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/annotated_types-0.6.0.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/__init__.py
--rw-r--r--   0        0        0    15749 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/from_thread.py
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/lowlevel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/py.typed
--rw-r--r--   0        0        0     5386 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/pytest_plugin.py
--rw-r--r--   0        0        0     9535 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/to_process.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/to_thread.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/_backends/__init__.py
--rw-r--r--   0        0        0    81968 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/_backends/_asyncio.py
--rw-r--r--   0        0        0    35642 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/_backends/_trio.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/_core/__init__.py
--rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/_core/_eventloop.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/_core/_exceptions.py
--rw-r--r--   0        0        0    19512 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/_core/_fileio.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/_core/_resources.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/_core/_signals.py
--rw-r--r--   0        0        0    24048 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/_core/_sockets.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/_core/_streams.py
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/_core/_subprocesses.py
--rw-r--r--   0        0        0    18444 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/_core/_synchronization.py
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/_core/_tasks.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/_core/_testing.py
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/_core/_typedattr.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/abc/__init__.py
--rw-r--r--   0        0        0    10097 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/abc/_eventloop.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/abc/_resources.py
--rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/abc/_sockets.py
--rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/abc/_streams.py
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/abc/_subprocesses.py
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/abc/_tasks.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/abc/_testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/streams/__init__.py
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/streams/buffered.py
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/streams/file.py
--rw-r--r--   0        0        0     9296 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/streams/memory.py
--rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/streams/stapled.py
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/streams/text.py
--rw-r--r--   0        0        0    12752 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio/streams/tls.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio-4.3.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio-4.3.0.dist-info/LICENSE
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio-4.3.0.dist-info/METADATA
--rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio-4.3.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio-4.3.0.dist-info/WHEEL
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio-4.3.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/anyio-4.3.0.dist-info/top_level.txt
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/certifi/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/certifi/__main__.py
--rw-r--r--   0        0        0   292541 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/certifi/cacert.pem
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/certifi/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/certifi/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/INSTALLER
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/LICENSE
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/METADATA
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/certifi-2024.2.2.dist-info/top_level.txt
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/distro/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/distro/__main__.py
--rw-r--r--   0        0        0    49430 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/distro/distro.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/distro/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/distro-1.9.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    11325 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/distro-1.9.0.dist-info/LICENSE
--rw-r--r--   0        0        0     6791 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/distro-1.9.0.dist-info/METADATA
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/distro-1.9.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/distro-1.9.0.dist-info/WHEEL
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/distro-1.9.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/distro-1.9.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/__init__.py
--rw-r--r--   0        0        0    62500 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_base_client.py
--rw-r--r--   0        0        0    15320 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_compat.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_constants.py
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_files.py
--rw-r--r--   0        0        0    16432 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_qs.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_resource.py
--rw-r--r--   0        0        0    27935 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_response.py
--rw-r--r--   0        0        0     9316 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_streaming.py
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_types.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/py.typed
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_utils/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_utils/_logs.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_utils/_sync.py
--rw-r--r--   0        0        0    12805 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_utils/_typing.py
--rw-r--r--   0        0        0    11105 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/lib/.keep
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/lib/chat_completion_chunk.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/resources/__init__.py
--rw-r--r--   0        0        0     9494 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/resources/models.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/resources/audio/__init__.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/resources/audio/audio.py
--rw-r--r--   0        0        0    10893 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/resources/audio/transcriptions.py
--rw-r--r--   0        0        0     8857 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/resources/audio/translations.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/resources/chat/__init__.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/resources/chat/chat.py
--rw-r--r--   0        0        0    18464 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/resources/chat/completions.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/types/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/types/model.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/types/model_list.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/types/translation.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/types/audio/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/types/audio/transcription.py
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/types/audio/transcription_create_params.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/types/audio/translation_create_params.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/types/chat/__init__.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/types/chat/chat_completion.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq/types/chat/completion_create_params.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq-0.5.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    12180 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq-0.5.0.dist-info/METADATA
--rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq-0.5.0.dist-info/RECORD
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq-0.5.0.dist-info/WHEEL
--rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/groq-0.5.0.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/__init__.py
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/_abnf.py
--rw-r--r--   0        0        0    26539 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/_connection.py
--rw-r--r--   0        0        0    11816 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/_events.py
--rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/_headers.py
--rw-r--r--   0        0        0     8383 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/_readers.py
--rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/_receivebuffer.py
--rw-r--r--   0        0        0    13300 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/_state.py
--rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/_util.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/_version.py
--rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/_writers.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/tests/__init__.py
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/tests/helpers.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/tests/test_against_stdlib_http.py
--rw-r--r--   0        0        0    38720 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/tests/test_connection.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/tests/test_events.py
--rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/tests/test_headers.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/tests/test_helpers.py
--rw-r--r--   0        0        0    16386 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/tests/test_io.py
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/tests/test_receivebuffer.py
--rw-r--r--   0        0        0     8928 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/tests/test_state.py
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/tests/test_util.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11/tests/data/test-file
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11-0.14.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11-0.14.0.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     8175 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11-0.14.0.dist-info/METADATA
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11-0.14.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11-0.14.0.dist-info/WHEEL
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/h11-0.14.0.dist-info/top_level.txt
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/hto/__about__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/hto/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/hto-0.0.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/hto-0.0.1.dist-info/METADATA
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/hto-0.0.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/hto-0.0.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/hto-0.0.1.dist-info/WHEEL
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/hto-0.0.1.dist-info/direct_url.json
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/hto-0.0.1.dist-info/licenses/LICENSE.txt
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/__init__.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_api.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_exceptions.py
--rw-r--r--   0        0        0    16614 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_models.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_ssl.py
--rw-r--r--   0        0        0     9464 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_synchronization.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_trace.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/py.typed
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_async/__init__.py
--rw-r--r--   0        0        0     8484 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_async/connection.py
--rw-r--r--   0        0        0    15609 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_async/connection_pool.py
--rw-r--r--   0        0        0    13978 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_async/http11.py
--rw-r--r--   0        0        0    23881 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_async/http2.py
--rw-r--r--   0        0        0    14851 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_async/http_proxy.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_async/interfaces.py
--rw-r--r--   0        0        0    13934 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_async/socks_proxy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_backends/__init__.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_backends/anyio.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_backends/auto.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_backends/base.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_backends/mock.py
--rw-r--r--   0        0        0     8086 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_backends/sync.py
--rw-r--r--   0        0        0     6078 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_backends/trio.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_sync/__init__.py
--rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_sync/connection.py
--rw-r--r--   0        0        0    15277 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_sync/connection_pool.py
--rw-r--r--   0        0        0    13564 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_sync/http11.py
--rw-r--r--   0        0        0    23345 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_sync/http2.py
--rw-r--r--   0        0        0    14613 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_sync/http_proxy.py
--rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_sync/interfaces.py
--rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore/_sync/socks_proxy.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore-1.0.5.dist-info/INSTALLER
--rw-r--r--   0        0        0    20969 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore-1.0.5.dist-info/METADATA
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore-1.0.5.dist-info/RECORD
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore-1.0.5.dist-info/WHEEL
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpcore-1.0.5.dist-info/licenses/LICENSE.md
--rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/__init__.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/__version__.py
--rw-r--r--   0        0        0    12928 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_api.py
--rw-r--r--   0        0        0    11830 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_auth.py
--rw-r--r--   0        0        0    67490 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_client.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_compat.py
--rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_config.py
--rw-r--r--   0        0        0     8047 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_content.py
--rw-r--r--   0        0        0     9904 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_decoders.py
--rw-r--r--   0        0        0     7922 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_exceptions.py
--rw-r--r--   0        0        0    15635 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_main.py
--rw-r--r--   0        0        0    42303 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_models.py
--rw-r--r--   0        0        0     8885 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_multipart.py
--rw-r--r--   0        0        0     5618 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_status_codes.py
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_types.py
--rw-r--r--   0        0        0    17720 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_urlparse.py
--rw-r--r--   0        0        0    21783 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_urls.py
--rw-r--r--   0        0        0    13858 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_transports/__init__.py
--rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_transports/asgi.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_transports/base.py
--rw-r--r--   0        0        0    13290 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_transports/default.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_transports/mock.py
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx/_transports/wsgi.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx-0.27.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     7184 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx-0.27.0.dist-info/METADATA
--rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx-0.27.0.dist-info/RECORD
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx-0.27.0.dist-info/WHEEL
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx-0.27.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/httpx-0.27.0.dist-info/licenses/LICENSE.md
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/idna/__init__.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/idna/compat.py
--rw-r--r--   0        0        0    12663 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/idna/core.py
--rw-r--r--   0        0        0    78320 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/idna/package_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/idna/py.typed
--rw-r--r--   0        0        0   206503 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/idna/uts46data.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/idna-3.7.dist-info/INSTALLER
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/idna-3.7.dist-info/LICENSE.md
--rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/idna-3.7.dist-info/METADATA
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/idna-3.7.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/idna-3.7.dist-info/WHEEL
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/__init__.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/__main__.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/__pip-runner__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/py.typed
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/__init__.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/build_env.py
--rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/cache.py
--rw-r--r--   0        0        0    14006 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/configuration.py
--rw-r--r--   0        0        0    23634 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/main.py
--rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0        0        0     8378 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0        0        0    11801 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0        0        0    30064 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0        0        0    18369 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0        0        0    28782 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0        0        0    12450 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0        0        0    16590 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0        0        0    37843 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0        0        0    25907 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0        0        0    10035 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0        0        0     7456 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/models/index.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0        0        0    20777 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/models/link.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0        0        0    20541 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/network/download.py
--rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0        0        0    18698 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/network/session.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0        0        0    28128 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0        0        0    27311 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0        0        0    19018 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0        0        0    17790 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0        0        0    35460 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0        0        0    24551 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0        0        0    24025 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0        0        0    21052 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0        0        0    32292 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0        0        0    12592 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/_jaraco_text.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0        0        0    23623 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0        0        0    18121 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0        0        0    22787 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/six.py
--rw-r--r--   0        0        0   111130 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/cachecontrol/py.typed
--rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0        0        0   281617 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/certifi/py.typed
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/py.typed
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/resultdict.py
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0        0        0    41487 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0        0        0    51965 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0        0        0    20797 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0        0        0    51767 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0        0        0    39693 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0        0        0    18315 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distlib/scripts.py
--rw-r--r--   0        0        0    97792 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distlib/t32.exe
--rw-r--r--   0        0        0   182784 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distlib/t64-arm.exe
--rw-r--r--   0        0        0   108032 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0        0        0    67530 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0        0        0    23747 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distlib/version.py
--rw-r--r--   0        0        0    91648 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distlib/w32.exe
--rw-r--r--   0        0        0   168448 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distlib/w64-arm.exe
--rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0        0        0    43958 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/distro/py.typed
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/idna/py.typed
--rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0        0        0   109364 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0        0        0    20155 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/platformdirs/py.typed
--rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0        0        0    34618 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35610 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    12130 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0        0        0    72281 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    53424 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   224445 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    38646 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pyparsing/py.typed
--rw-r--r--   0        0        0    26692 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13488 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10646 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    24215 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0        0        0    19697 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0        0        0    33460 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/resolvelib/py.typed
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/_fileno.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/_null_file.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0        0        0    99218 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/py.typed
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0        0        0    35173 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/tenacity/py.typed
--rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/tomli/py.typed
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/truststore/__init__.py
--rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/truststore/_api.py
--rw-r--r--   0        0        0    17694 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/truststore/_macos.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/truststore/_openssl.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/truststore/_ssl_constants.py
--rw-r--r--   0        0        0    17468 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/truststore/_windows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/truststore/py.typed
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0        0        0    39990 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0        0        0    19752 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0        0        0    22013 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip-24.0.dist-info/AUTHORS.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip-24.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip-24.0.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip-24.0.dist-info/METADATA
--rw-r--r--   0        0        0    78936 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip-24.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip-24.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip-24.0.dist-info/WHEEL
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip-24.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pip-24.0.dist-info/top_level.txt
--rw-r--r--   0        0        0    13178 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/__init__.py
--rw-r--r--   0        0        0    11913 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_migration.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/alias_generators.py
--rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/aliases.py
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/annotated_handlers.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/class_validators.py
--rw-r--r--   0        0        0    21493 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/color.py
--rw-r--r--   0        0        0    32206 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/config.py
--rw-r--r--   0        0        0    13450 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/dataclasses.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/datetime_parse.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/decorator.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/env_settings.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/error_wrappers.py
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/errors.py
--rw-r--r--   0        0        0    49922 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/fields.py
--rw-r--r--   0        0        0    14635 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/functional_serializers.py
--rw-r--r--   0        0        0    24322 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/functional_validators.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/generics.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/json.py
--rw-r--r--   0        0        0   105243 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/json_schema.py
--rw-r--r--   0        0        0    69938 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/main.py
--rw-r--r--   0        0        0    55574 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/mypy.py
--rw-r--r--   0        0        0    22461 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/networks.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/py.typed
--rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/root_model.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/schema.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/tools.py
--rw-r--r--   0        0        0    18834 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/type_adapter.py
--rw-r--r--   0        0        0    94034 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/types.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/typing.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/utils.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/validate_call_decorator.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/validators.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/version.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/warnings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/__init__.py
--rw-r--r--   0        0        0    12208 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_config.py
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_core_metadata.py
--rw-r--r--   0        0        0    24268 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_core_utils.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_dataclasses.py
--rw-r--r--   0        0        0    30623 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_decorators.py
--rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_decorators_v1.py
--rw-r--r--   0        0        0    26435 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_discriminated_union.py
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_docs_extraction.py
--rw-r--r--   0        0        0    14184 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_fields.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_forward_ref.py
--rw-r--r--   0        0        0   101871 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_generate_schema.py
--rw-r--r--   0        0        0    22218 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_generics.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_git.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_internal_dataclass.py
--rw-r--r--   0        0        0    17271 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_known_annotated_metadata.py
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_mock_val_ser.py
--rw-r--r--   0        0        0    31789 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_model_construction.py
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_repr.py
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_schema_generation_shared.py
--rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_signature.py
--rw-r--r--   0        0        0    28696 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_std_types_schema.py
--rw-r--r--   0        0        0    18863 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_typing_extra.py
--rw-r--r--   0        0        0    12668 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_utils.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_validate_call.py
--rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/_internal/_validators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/deprecated/__init__.py
--rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/deprecated/class_validators.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/deprecated/config.py
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/deprecated/copy_internals.py
--rw-r--r--   0        0        0    10778 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/deprecated/decorator.py
--rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/deprecated/json.py
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/deprecated/parse.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/deprecated/tools.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/plugin/__init__.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/plugin/_loader.py
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/plugin/_schema_validator.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/__init__.py
--rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/_hypothesis_plugin.py
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/annotated_types.py
--rw-r--r--   0        0        0    14595 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/class_validators.py
--rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/color.py
--rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/config.py
--rw-r--r--   0        0        0    18073 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/dataclasses.py
--rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/datetime_parse.py
--rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/decorator.py
--rw-r--r--   0        0        0    14039 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/env_settings.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/error_wrappers.py
--rw-r--r--   0        0        0    17693 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/errors.py
--rw-r--r--   0        0        0    50485 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/fields.py
--rw-r--r--   0        0        0    17805 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/generics.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/json.py
--rw-r--r--   0        0        0    44376 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/main.py
--rw-r--r--   0        0        0    38737 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/mypy.py
--rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/networks.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/py.typed
--rw-r--r--   0        0        0    47614 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/schema.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/tools.py
--rw-r--r--   0        0        0    35379 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/types.py
--rw-r--r--   0        0        0    18996 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/typing.py
--rw-r--r--   0        0        0    25809 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/utils.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/v1.py
--rw-r--r--   0        0        0    21887 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/validators.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic/v1/version.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic-2.7.1.dist-info/INSTALLER
--rw-r--r--   0        0        0   107323 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic-2.7.1.dist-info/METADATA
--rw-r--r--   0        0        0    14460 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic-2.7.1.dist-info/RECORD
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic-2.7.1.dist-info/WHEEL
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic-2.7.1.dist-info/licenses/LICENSE
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic_core/__init__.py
--rwxr-xr-x   0        0        0  5104408 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic_core/_pydantic_core.cpython-312-x86_64-linux-gnu.so
--rw-r--r--   0        0        0    35226 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic_core/_pydantic_core.pyi
--rw-r--r--   0        0        0   137407 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic_core/core_schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic_core/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic_core-2.18.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic_core-2.18.2.dist-info/METADATA
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic_core-2.18.2.dist-info/RECORD
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic_core-2.18.2.dist-info/WHEEL
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/pydantic_core-2.18.2.dist-info/license_files/LICENSE
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/simple_term_menu-1.6.4.dist-info/INSTALLER
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/simple_term_menu-1.6.4.dist-info/LICENSE
--rw-r--r--   0        0        0    29718 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/simple_term_menu-1.6.4.dist-info/METADATA
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/simple_term_menu-1.6.4.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/simple_term_menu-1.6.4.dist-info/WHEEL
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/simple_term_menu-1.6.4.dist-info/entry_points.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/simple_term_menu-1.6.4.dist-info/top_level.txt
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/sniffio/__init__.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/sniffio/_impl.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/sniffio/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/sniffio/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/sniffio/_tests/__init__.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/sniffio/_tests/test_sniffio.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/sniffio-1.3.1.dist-info/INSTALLER
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/sniffio-1.3.1.dist-info/LICENSE
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/sniffio-1.3.1.dist-info/LICENSE.APACHE2
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/sniffio-1.3.1.dist-info/LICENSE.MIT
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/sniffio-1.3.1.dist-info/METADATA
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/sniffio-1.3.1.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/sniffio-1.3.1.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/sniffio-1.3.1.dist-info/top_level.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/typing_extensions-4.11.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    13936 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/typing_extensions-4.11.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/typing_extensions-4.11.0.dist-info/METADATA
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/typing_extensions-4.11.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 hto-0.0.1/venv/lib/python3.12/site-packages/typing_extensions-4.11.0.dist-info/WHEEL
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 hto-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 hto-0.0.1/README.md
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 hto-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 hto-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 hto-0.0.2/hto/__about__.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hto-0.0.2/hto/__init__.py
+-rw-r--r--   0        0        0     6903 2020-02-02 00:00:00.000000 hto-0.0.2/hto/__main__.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hto-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 hto-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 hto-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 hto-0.0.2/README.md
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 hto-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 hto-0.0.2/PKG-INFO
```

### Comparing `hto-0.0.1/hto/__main__.py` & `hto-0.0.2/hto/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import os
 import click
 import json
 import sys
 import platform
 from simple_term_menu import TerminalMenu
 import typer
-from groq import Groq
+import groq
 import rich.console
 import rich.prompt
 import subprocess
 from rich.markdown import Markdown
 
-client = Groq(
-    api_key=os.environ.get("GROQ_API_KEY"),
-)
+try:
+    client = groq.Groq(
+        api_key=os.environ.get("GROQ_API_KEY"),
+    )
+except groq.GroqError:
+    print("Please set GROQ_API_KEY environment variable.")
+    sys.exit(1)
 
 app = typer.Typer()
 
 
 class AIClient:
     def __init__(self, *, system_prompt: str, model_name: str = "llama3-70b-8192"):
         console = rich.console.Console()
```

### Comparing `hto-0.0.1/venv/lib/python3.12/site-packages/annotated_types-0.6.0.dist-info/licenses/LICENSE` & `hto-0.0.2/LICENSE.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,9 @@
-The MIT License (MIT)
+MIT License
 
-Copyright (c) 2022 the contributors
+Copyright (c) 2024-present Danial Keimasi <danialkeimasi@gmail.com>
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `hto-0.0.1/venv/lib/python3.12/site-packages/hto-0.0.1.dist-info/METADATA` & `hto-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hto
-Version: 0.0.1
+Version: 0.0.2
 Summary: Ask AI for help you in your terminal.
 Project-URL: Documentation, https://github.com/danialkeimasi/hto#readme
 Project-URL: Issues, https://github.com/danialkeimasi/hto/issues
 Project-URL: Source, https://github.com/danialkeimasi/hto
 Author-email: Danial Keimasi <danialkeimasi@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -15,15 +15,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: groq==0.5.0
+Requires-Dist: rich==13.7.1
 Requires-Dist: simple-term-menu==1.6.4
+Requires-Dist: typer==0.12.3
 Description-Content-Type: text/markdown
 
 # hto
 
 [![PyPI - Version](https://img.shields.io/pypi/v/hto.svg)](https://pypi.org/project/hto)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hto.svg)](https://pypi.org/project/hto)
```

### Comparing `hto-0.0.1/pyproject.toml` & `hto-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 ]
 
 [project.urls]
 Documentation = "https://github.com/danialkeimasi/hto#readme"
 Issues = "https://github.com/danialkeimasi/hto/issues"
 Source = "https://github.com/danialkeimasi/hto"
 
+[project.scripts]
+hto = "hto.__main__:app"
+
 [tool.hatch.version]
 path = "hto/__about__.py"
 
 [tool.hatch.envs.types]
 extra-dependencies = [
   "mypy>=1.0.0",
 ]
```

