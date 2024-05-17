# Comparing `tmp/multidecoder-1.3.3.tar.gz` & `tmp/multidecoder-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidecoder-1.3.3.tar", last modified: Wed Apr 24 19:26:38 2024, max compression
+gzip compressed data, was "multidecoder-1.3.4.tar", last modified: Fri May 17 00:08:15 2024, max compression
```

## Comparing `multidecoder-1.3.3.tar` & `multidecoder-1.3.4.tar`

### file list

```diff
@@ -1,209 +1,212 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 19:26:38.595048 multidecoder-1.3.3/
--rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-04-24 19:26:06.000000 multidecoder-1.3.3/.git-blame-ignore-revs
--rw-r--r--   0 vsts      (1001) docker     (127)     2097 2024-04-24 19:26:06.000000 multidecoder-1.3.3/.gitignore
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 19:26:38.547047 multidecoder-1.3.3/.vscode/
--rw-r--r--   0 vsts      (1001) docker     (127)      616 2024-04-24 19:26:06.000000 multidecoder-1.3.3/.vscode/settings.json
--rw-r--r--   0 vsts      (1001) docker     (127)     1390 2024-04-24 19:26:06.000000 multidecoder-1.3.3/LICENSE.md
--rw-r--r--   0 vsts      (1001) docker     (127)      109 2024-04-24 19:26:06.000000 multidecoder-1.3.3/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     2739 2024-04-24 19:26:38.595048 multidecoder-1.3.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2049 2024-04-24 19:26:06.000000 multidecoder-1.3.3/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 19:26:38.547047 multidecoder-1.3.3/pipelines/
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-24 19:26:06.000000 multidecoder-1.3.3/pipelines/azure-tests.yaml
--rw-r--r--   0 vsts      (1001) docker     (127)     1255 2024-04-24 19:26:06.000000 multidecoder-1.3.3/pipelines/publish.yaml
--rw-r--r--   0 vsts      (1001) docker     (127)      658 2024-04-24 19:26:06.000000 multidecoder-1.3.3/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)      929 2024-04-24 19:26:38.599048 multidecoder-1.3.3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)       69 2024-04-24 19:26:06.000000 multidecoder-1.3.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 19:26:38.543047 multidecoder-1.3.3/src/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 19:26:38.547047 multidecoder-1.3.3/src/multidecoder/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1641 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      411 2024-04-24 19:26:38.000000 multidecoder-1.3.3/src/multidecoder/_version.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 19:26:38.551047 multidecoder-1.3.3/src/multidecoder/decoders/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/decoders/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4389 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/decoders/base64.py
--rw-r--r--   0 vsts      (1001) docker     (127)      569 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/decoders/chr.py
--rw-r--r--   0 vsts      (1001) docker     (127)      548 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/decoders/codec.py
--rw-r--r--   0 vsts      (1001) docker     (127)      955 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/decoders/concat.py
--rw-r--r--   0 vsts      (1001) docker     (127)      591 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/decoders/filename.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1613 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/decoders/hex.py
--rw-r--r--   0 vsts      (1001) docker     (127)      497 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/decoders/javascript.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12324 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/decoders/network.py
--rw-r--r--   0 vsts      (1001) docker     (127)      550 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/decoders/path.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1651 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/decoders/pe_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1976 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/decoders/replace.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6227 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/decoders/shell.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1597 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/decoders/vba.py
--rw-r--r--   0 vsts      (1001) docker     (127)      702 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/decoders/xml.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21889 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/domains.py
--rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/hit.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1211 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/json_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1181 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keyword.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 19:26:38.559047 multidecoder-1.3.3/src/multidecoder/keywords/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 19:26:38.591048 multidecoder-1.3.3/src/multidecoder/keywords/api/
--rw-r--r--   0 vsts      (1001) docker     (127)     4040 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.advapi32
--rw-r--r--   0 vsts      (1001) docker     (127)       23 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.apphelp
--rw-r--r--   0 vsts      (1001) docker     (127)     1212 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.atl
--rw-r--r--   0 vsts      (1001) docker     (127)      243 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.atl80
--rw-r--r--   0 vsts      (1001) docker     (127)      229 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.atl90
--rw-r--r--   0 vsts      (1001) docker     (127)      429 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.au3zip
--rw-r--r--   0 vsts      (1001) docker     (127)      162 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.avicap32
--rw-r--r--   0 vsts      (1001) docker     (127)      196 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.cabinet
--rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.clbcatq
--rw-r--r--   0 vsts      (1001) docker     (127)       56 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.cmdial32
--rw-r--r--   0 vsts      (1001) docker     (127)      177 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.comctl32
--rw-r--r--   0 vsts      (1001) docker     (127)       91 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.credui
--rw-r--r--   0 vsts      (1001) docker     (127)      197 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.cryptbase
--rw-r--r--   0 vsts      (1001) docker     (127)       26 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.cryptdll
--rw-r--r--   0 vsts      (1001) docker     (127)       24 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.cscapi
--rw-r--r--   0 vsts      (1001) docker     (127)      610 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.dbghelp
--rw-r--r--   0 vsts      (1001) docker     (127)       79 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.devmgr
--rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.dnsapi
--rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.drprov
--rw-r--r--   0 vsts      (1001) docker     (127)      225 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.dsound
--rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.dsuiext
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.esent
--rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.fveapi
--rw-r--r--   0 vsts      (1001) docker     (127)      127 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.fwpuclnt
--rw-r--r--   0 vsts      (1001) docker     (127)     1913 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.gdi32
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.gina
--rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.icmp
--rw-r--r--   0 vsts      (1001) docker     (127)     1254 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.imagehlp
--rw-r--r--   0 vsts      (1001) docker     (127)     1005 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.iphlpapi
--rw-r--r--   0 vsts      (1001) docker     (127)    19404 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.kernel32
--rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.kernelbase
--rw-r--r--   0 vsts      (1001) docker     (127)     2218 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.libeay32
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.lsasrv
--rw-r--r--   0 vsts      (1001) docker     (127)      265 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.mapi32
--rw-r--r--   0 vsts      (1001) docker     (127)     1968 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.mfc42
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.mpr
--rw-r--r--   0 vsts      (1001) docker     (127)      143 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.mprapi
--rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.msacm32
--rw-r--r--   0 vsts      (1001) docker     (127)       81 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.msasn1
--rw-r--r--   0 vsts      (1001) docker     (127)       53 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.mscoree
--rw-r--r--   0 vsts      (1001) docker     (127)     4043 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.msi
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.msimg32
--rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.mspdb80
--rw-r--r--   0 vsts      (1001) docker     (127)      520 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.mssign32
--rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.msutb
--rw-r--r--   0 vsts      (1001) docker     (127)     1527 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.msvbvm60
--rw-r--r--   0 vsts      (1001) docker     (127)     3448 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.msvcrt
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.msvfw32
--rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.mswsock
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.mydocs
--rw-r--r--   0 vsts      (1001) docker     (127)      525 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.nddeapi
--rw-r--r--   0 vsts      (1001) docker     (127)     1276 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.netapi32
--rw-r--r--   0 vsts      (1001) docker     (127)       20 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.netplwiz
--rw-r--r--   0 vsts      (1001) docker     (127)     4660 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.ntdll
--rw-r--r--   0 vsts      (1001) docker     (127)      197 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.ntdsapi
--rw-r--r--   0 vsts      (1001) docker     (127)     1137 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.ntoskrnl
--rw-r--r--   0 vsts      (1001) docker     (127)       43 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.ntshrui
--rw-r--r--   0 vsts      (1001) docker     (127)     1599 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.odbc32
--rw-r--r--   0 vsts      (1001) docker     (127)      970 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.odbccp32
--rw-r--r--   0 vsts      (1001) docker     (127)       55 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.odbctrac
--rw-r--r--   0 vsts      (1001) docker     (127)      829 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.ole32
--rw-r--r--   0 vsts      (1001) docker     (127)      641 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.oleaut32
--rw-r--r--   0 vsts      (1001) docker     (127)       58 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.oledlg
--rw-r--r--   0 vsts      (1001) docker     (127)      167 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.onex
--rw-r--r--   0 vsts      (1001) docker     (127)      587 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.packet
--rw-r--r--   0 vsts      (1001) docker     (127)      222 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.pdh
--rw-r--r--   0 vsts      (1001) docker     (127)     2236 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.powrprof
--rw-r--r--   0 vsts      (1001) docker     (127)      455 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.psapi
--rw-r--r--   0 vsts      (1001) docker     (127)       40 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.pstorec
--rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.query
--rw-r--r--   0 vsts      (1001) docker     (127)       29 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.rasapi32
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.rastapi
--rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.riched20
--rw-r--r--   0 vsts      (1001) docker     (127)     1207 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.rpcrt4
--rw-r--r--   0 vsts      (1001) docker     (127)       99 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.scarddlg
--rw-r--r--   0 vsts      (1001) docker     (127)     1561 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.scecli
--rw-r--r--   0 vsts      (1001) docker     (127)      729 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.se
--rw-r--r--   0 vsts      (1001) docker     (127)      166 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.secur32
--rw-r--r--   0 vsts      (1001) docker     (127)       14 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.sensapi
--rw-r--r--   0 vsts      (1001) docker     (127)      239 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.setupapi
--rw-r--r--   0 vsts      (1001) docker     (127)      123 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.sfc
--rw-r--r--   0 vsts      (1001) docker     (127)     3672 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.shell32
--rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.shimgvw
--rw-r--r--   0 vsts      (1001) docker     (127)      544 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.shlwapi
--rw-r--r--   0 vsts      (1001) docker     (127)       26 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.shsvcs
--rw-r--r--   0 vsts      (1001) docker     (127)     1328 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.ssleay32
--rw-r--r--   0 vsts      (1001) docker     (127)       86 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.unknown
--rw-r--r--   0 vsts      (1001) docker     (127)     1068 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.urlmon
--rw-r--r--   0 vsts      (1001) docker     (127)     1564 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.user32
--rw-r--r--   0 vsts      (1001) docker     (127)      309 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.userenv
--rw-r--r--   0 vsts      (1001) docker     (127)      114 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.usp10
--rw-r--r--   0 vsts      (1001) docker     (127)       60 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.version
--rw-r--r--   0 vsts      (1001) docker     (127)      312 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.winhttp
--rw-r--r--   0 vsts      (1001) docker     (127)      928 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.wininet
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.winmm
--rw-r--r--   0 vsts      (1001) docker     (127)      219 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.winscard
--rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.winshfhc
--rw-r--r--   0 vsts      (1001) docker     (127)     1994 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.winsock
--rw-r--r--   0 vsts      (1001) docker     (127)      254 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.winspool
--rw-r--r--   0 vsts      (1001) docker     (127)     3887 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.winsta
--rw-r--r--   0 vsts      (1001) docker     (127)       14 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.wintrust
--rw-r--r--   0 vsts      (1001) docker     (127)       55 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.wlanapi
--rw-r--r--   0 vsts      (1001) docker     (127)      249 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.wldap32
--rw-r--r--   0 vsts      (1001) docker     (127)      266 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.wship6
--rw-r--r--   0 vsts      (1001) docker     (127)      754 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.wsnmp32
--rw-r--r--   0 vsts      (1001) docker     (127)      490 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/api/api.wtsapi32
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/archive
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/av.name
--rw-r--r--   0 vsts      (1001) docker     (127)      503 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/cryptography
--rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/debugger.device.name
--rw-r--r--   0 vsts      (1001) docker     (127)      168 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/enable_content
--rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/environment.windows
--rw-r--r--   0 vsts      (1001) docker     (127)      634 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/event
--rw-r--r--   0 vsts      (1001) docker     (127)      517 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/guid
--rw-r--r--   0 vsts      (1001) docker     (127)     1091 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/key
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/network.protocol
--rw-r--r--   0 vsts      (1001) docker     (127)      532 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/network.string
--rw-r--r--   0 vsts      (1001) docker     (127)     1812 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/oid
--rw-r--r--   0 vsts      (1001) docker     (127)     2674 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/os_name
--rw-r--r--   0 vsts      (1001) docker     (127)     1476 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/powershell.cmdlet
--rw-r--r--   0 vsts      (1001) docker     (127)      873 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/privilege
--rw-r--r--   0 vsts      (1001) docker     (127)     1038 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/ransomware.string
--rw-r--r--   0 vsts      (1001) docker     (127)      263 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/sandbox.id
--rw-r--r--   0 vsts      (1001) docker     (127)      902 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/security_identifier
--rw-r--r--   0 vsts      (1001) docker     (127)      151 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/user_agent
--rw-r--r--   0 vsts      (1001) docker     (127)       53 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/vba.name
--rw-r--r--   0 vsts      (1001) docker     (127)     2164 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords/windows.registry
--rw-r--r--   0 vsts      (1001) docker     (127)    22786 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/keywords_to_review.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     2950 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/multidecoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3777 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/node.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/py.typed
--rw-r--r--   0 vsts      (1001) docker     (127)     1938 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/query.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2440 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/registry.py
--rw-r--r--   0 vsts      (1001) docker     (127)      465 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/string_helper.py
--rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-04-24 19:26:06.000000 multidecoder-1.3.3/src/multidecoder/xor_helper.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 19:26:38.595048 multidecoder-1.3.3/src/multidecoder.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2739 2024-04-24 19:26:38.000000 multidecoder-1.3.3/src/multidecoder.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     7266 2024-04-24 19:26:38.000000 multidecoder-1.3.3/src/multidecoder.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-24 19:26:38.000000 multidecoder-1.3.3/src/multidecoder.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       60 2024-04-24 19:26:38.000000 multidecoder-1.3.3/src/multidecoder.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-24 19:26:16.000000 multidecoder-1.3.3/src/multidecoder.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-04-24 19:26:38.000000 multidecoder-1.3.3/src/multidecoder.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-04-24 19:26:38.000000 multidecoder-1.3.3/src/multidecoder.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 19:26:38.591048 multidecoder-1.3.3/stubs/
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-24 19:26:06.000000 multidecoder-1.3.3/stubs/pefile.pyi
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 19:26:38.591048 multidecoder-1.3.3/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-24 19:26:06.000000 multidecoder-1.3.3/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)        9 2024-04-24 19:26:06.000000 multidecoder-1.3.3/tests/requirements.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 19:26:38.595048 multidecoder-1.3.3/tests/test_decoders/
--rw-r--r--   0 vsts      (1001) docker     (127)     2953 2024-04-24 19:26:06.000000 multidecoder-1.3.3/tests/test_decoders/test_base64.py
--rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-04-24 19:26:06.000000 multidecoder-1.3.3/tests/test_decoders/test_chr.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2149 2024-04-24 19:26:06.000000 multidecoder-1.3.3/tests/test_decoders/test_concat.py
--rw-r--r--   0 vsts      (1001) docker     (127)      564 2024-04-24 19:26:06.000000 multidecoder-1.3.3/tests/test_decoders/test_encoding.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-04-24 19:26:06.000000 multidecoder-1.3.3/tests/test_decoders/test_filename.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1644 2024-04-24 19:26:06.000000 multidecoder-1.3.3/tests/test_decoders/test_hex.py
--rw-r--r--   0 vsts      (1001) docker     (127)      305 2024-04-24 19:26:06.000000 multidecoder-1.3.3/tests/test_decoders/test_javascript.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10927 2024-04-24 19:26:06.000000 multidecoder-1.3.3/tests/test_decoders/test_network.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1014 2024-04-24 19:26:06.000000 multidecoder-1.3.3/tests/test_decoders/test_path.py
--rw-r--r--   0 vsts      (1001) docker     (127)      502 2024-04-24 19:26:06.000000 multidecoder-1.3.3/tests/test_decoders/test_pe_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)      943 2024-04-24 19:26:06.000000 multidecoder-1.3.3/tests/test_decoders/test_replace.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10165 2024-04-24 19:26:06.000000 multidecoder-1.3.3/tests/test_decoders/test_shell.py
--rw-r--r--   0 vsts      (1001) docker     (127)      960 2024-04-24 19:26:06.000000 multidecoder-1.3.3/tests/test_decoders/test_vba.py
--rw-r--r--   0 vsts      (1001) docker     (127)      702 2024-04-24 19:26:06.000000 multidecoder-1.3.3/tests/test_decoders/test_xml.py
--rw-r--r--   0 vsts      (1001) docker     (127)      892 2024-04-24 19:26:06.000000 multidecoder-1.3.3/tests/test_multidecoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)      914 2024-04-24 19:26:06.000000 multidecoder-1.3.3/tests/test_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)      809 2024-04-24 19:26:06.000000 multidecoder-1.3.3/tests/test_xor_helper.py
--rw-r--r--   0 vsts      (1001) docker     (127)       69 2024-04-24 19:26:06.000000 multidecoder-1.3.3/tox.ini
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.349407 multidecoder-1.3.4/
+-rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-05-17 00:07:40.000000 multidecoder-1.3.4/.git-blame-ignore-revs
+-rw-r--r--   0 vsts      (1001) docker     (127)     2097 2024-05-17 00:07:40.000000 multidecoder-1.3.4/.gitignore
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.293406 multidecoder-1.3.4/.vscode/
+-rw-r--r--   0 vsts      (1001) docker     (127)      616 2024-05-17 00:07:40.000000 multidecoder-1.3.4/.vscode/settings.json
+-rw-r--r--   0 vsts      (1001) docker     (127)     1390 2024-05-17 00:07:40.000000 multidecoder-1.3.4/LICENSE.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      109 2024-05-17 00:07:40.000000 multidecoder-1.3.4/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     2739 2024-05-17 00:08:15.349407 multidecoder-1.3.4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2049 2024-05-17 00:07:40.000000 multidecoder-1.3.4/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.297406 multidecoder-1.3.4/pipelines/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-05-17 00:07:40.000000 multidecoder-1.3.4/pipelines/azure-tests.yaml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1255 2024-05-17 00:07:40.000000 multidecoder-1.3.4/pipelines/publish.yaml
+-rw-r--r--   0 vsts      (1001) docker     (127)      658 2024-05-17 00:07:40.000000 multidecoder-1.3.4/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)      929 2024-05-17 00:08:15.349407 multidecoder-1.3.4/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)       69 2024-05-17 00:07:40.000000 multidecoder-1.3.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.293406 multidecoder-1.3.4/src/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.297406 multidecoder-1.3.4/src/multidecoder/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1641 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      411 2024-05-17 00:08:15.000000 multidecoder-1.3.4/src/multidecoder/_version.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.301406 multidecoder-1.3.4/src/multidecoder/decoders/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4389 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/base64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      569 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/chr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      633 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/codec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      999 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/concat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      591 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/filename.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1613 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/hex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      497 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/javascript.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13035 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/network.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      550 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/path.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1651 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/pe_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1976 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/replace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      431 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/reverse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6227 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/shell.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1597 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/vba.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      702 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/decoders/xml.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21889 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/domains.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/hit.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1211 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/json_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1181 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keyword.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.309406 multidecoder-1.3.4/src/multidecoder/keywords/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.341407 multidecoder-1.3.4/src/multidecoder/keywords/api/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4040 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.advapi32
+-rw-r--r--   0 vsts      (1001) docker     (127)       23 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.apphelp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1212 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.atl
+-rw-r--r--   0 vsts      (1001) docker     (127)      243 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.atl80
+-rw-r--r--   0 vsts      (1001) docker     (127)      229 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.atl90
+-rw-r--r--   0 vsts      (1001) docker     (127)      429 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.au3zip
+-rw-r--r--   0 vsts      (1001) docker     (127)      162 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.avicap32
+-rw-r--r--   0 vsts      (1001) docker     (127)      196 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.cabinet
+-rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.clbcatq
+-rw-r--r--   0 vsts      (1001) docker     (127)       56 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.cmdial32
+-rw-r--r--   0 vsts      (1001) docker     (127)      177 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.comctl32
+-rw-r--r--   0 vsts      (1001) docker     (127)       91 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.credui
+-rw-r--r--   0 vsts      (1001) docker     (127)      197 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.cryptbase
+-rw-r--r--   0 vsts      (1001) docker     (127)       26 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.cryptdll
+-rw-r--r--   0 vsts      (1001) docker     (127)       24 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.cscapi
+-rw-r--r--   0 vsts      (1001) docker     (127)      610 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.dbghelp
+-rw-r--r--   0 vsts      (1001) docker     (127)       79 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.devmgr
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.dnsapi
+-rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.drprov
+-rw-r--r--   0 vsts      (1001) docker     (127)      225 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.dsound
+-rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.dsuiext
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.esent
+-rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.fveapi
+-rw-r--r--   0 vsts      (1001) docker     (127)      127 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.fwpuclnt
+-rw-r--r--   0 vsts      (1001) docker     (127)     1913 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.gdi32
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.gina
+-rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.icmp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1254 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.imagehlp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1005 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.iphlpapi
+-rw-r--r--   0 vsts      (1001) docker     (127)    19404 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.kernel32
+-rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.kernelbase
+-rw-r--r--   0 vsts      (1001) docker     (127)     2218 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.libeay32
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.lsasrv
+-rw-r--r--   0 vsts      (1001) docker     (127)      265 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.mapi32
+-rw-r--r--   0 vsts      (1001) docker     (127)     1968 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.mfc42
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.mpr
+-rw-r--r--   0 vsts      (1001) docker     (127)      143 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.mprapi
+-rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.msacm32
+-rw-r--r--   0 vsts      (1001) docker     (127)       81 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.msasn1
+-rw-r--r--   0 vsts      (1001) docker     (127)       53 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.mscoree
+-rw-r--r--   0 vsts      (1001) docker     (127)     4043 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.msi
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.msimg32
+-rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.mspdb80
+-rw-r--r--   0 vsts      (1001) docker     (127)      520 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.mssign32
+-rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.msutb
+-rw-r--r--   0 vsts      (1001) docker     (127)     1527 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.msvbvm60
+-rw-r--r--   0 vsts      (1001) docker     (127)     3448 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.msvcrt
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.msvfw32
+-rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.mswsock
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.mydocs
+-rw-r--r--   0 vsts      (1001) docker     (127)      525 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.nddeapi
+-rw-r--r--   0 vsts      (1001) docker     (127)     1276 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.netapi32
+-rw-r--r--   0 vsts      (1001) docker     (127)       20 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.netplwiz
+-rw-r--r--   0 vsts      (1001) docker     (127)     4660 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.ntdll
+-rw-r--r--   0 vsts      (1001) docker     (127)      197 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.ntdsapi
+-rw-r--r--   0 vsts      (1001) docker     (127)     1137 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.ntoskrnl
+-rw-r--r--   0 vsts      (1001) docker     (127)       43 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.ntshrui
+-rw-r--r--   0 vsts      (1001) docker     (127)     1599 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.odbc32
+-rw-r--r--   0 vsts      (1001) docker     (127)      970 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.odbccp32
+-rw-r--r--   0 vsts      (1001) docker     (127)       55 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.odbctrac
+-rw-r--r--   0 vsts      (1001) docker     (127)      829 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.ole32
+-rw-r--r--   0 vsts      (1001) docker     (127)      641 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.oleaut32
+-rw-r--r--   0 vsts      (1001) docker     (127)       58 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.oledlg
+-rw-r--r--   0 vsts      (1001) docker     (127)      167 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.onex
+-rw-r--r--   0 vsts      (1001) docker     (127)      587 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.packet
+-rw-r--r--   0 vsts      (1001) docker     (127)      222 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.pdh
+-rw-r--r--   0 vsts      (1001) docker     (127)     2236 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.powrprof
+-rw-r--r--   0 vsts      (1001) docker     (127)      455 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.psapi
+-rw-r--r--   0 vsts      (1001) docker     (127)       40 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.pstorec
+-rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.query
+-rw-r--r--   0 vsts      (1001) docker     (127)       29 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.rasapi32
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.rastapi
+-rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.riched20
+-rw-r--r--   0 vsts      (1001) docker     (127)     1207 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.rpcrt4
+-rw-r--r--   0 vsts      (1001) docker     (127)       99 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.scarddlg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1561 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.scecli
+-rw-r--r--   0 vsts      (1001) docker     (127)      729 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.se
+-rw-r--r--   0 vsts      (1001) docker     (127)      166 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.secur32
+-rw-r--r--   0 vsts      (1001) docker     (127)       14 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.sensapi
+-rw-r--r--   0 vsts      (1001) docker     (127)      239 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.setupapi
+-rw-r--r--   0 vsts      (1001) docker     (127)      123 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.sfc
+-rw-r--r--   0 vsts      (1001) docker     (127)     3672 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.shell32
+-rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.shimgvw
+-rw-r--r--   0 vsts      (1001) docker     (127)      544 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.shlwapi
+-rw-r--r--   0 vsts      (1001) docker     (127)       26 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.shsvcs
+-rw-r--r--   0 vsts      (1001) docker     (127)     1328 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.ssleay32
+-rw-r--r--   0 vsts      (1001) docker     (127)       86 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.unknown
+-rw-r--r--   0 vsts      (1001) docker     (127)     1068 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.urlmon
+-rw-r--r--   0 vsts      (1001) docker     (127)     1564 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.user32
+-rw-r--r--   0 vsts      (1001) docker     (127)      309 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.userenv
+-rw-r--r--   0 vsts      (1001) docker     (127)      114 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.usp10
+-rw-r--r--   0 vsts      (1001) docker     (127)       60 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.version
+-rw-r--r--   0 vsts      (1001) docker     (127)      312 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.winhttp
+-rw-r--r--   0 vsts      (1001) docker     (127)      928 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.wininet
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.winmm
+-rw-r--r--   0 vsts      (1001) docker     (127)      219 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.winscard
+-rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.winshfhc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1994 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.winsock
+-rw-r--r--   0 vsts      (1001) docker     (127)      254 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.winspool
+-rw-r--r--   0 vsts      (1001) docker     (127)     3887 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.winsta
+-rw-r--r--   0 vsts      (1001) docker     (127)       14 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.wintrust
+-rw-r--r--   0 vsts      (1001) docker     (127)       55 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.wlanapi
+-rw-r--r--   0 vsts      (1001) docker     (127)      249 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.wldap32
+-rw-r--r--   0 vsts      (1001) docker     (127)      266 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.wship6
+-rw-r--r--   0 vsts      (1001) docker     (127)      754 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.wsnmp32
+-rw-r--r--   0 vsts      (1001) docker     (127)      490 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/api/api.wtsapi32
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/archive
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/av.name
+-rw-r--r--   0 vsts      (1001) docker     (127)      503 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/cryptography
+-rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/debugger.device.name
+-rw-r--r--   0 vsts      (1001) docker     (127)      168 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/enable_content
+-rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/environment.windows
+-rw-r--r--   0 vsts      (1001) docker     (127)      634 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/event
+-rw-r--r--   0 vsts      (1001) docker     (127)      517 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/guid
+-rw-r--r--   0 vsts      (1001) docker     (127)     1091 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/key
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/network.protocol
+-rw-r--r--   0 vsts      (1001) docker     (127)      532 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/network.string
+-rw-r--r--   0 vsts      (1001) docker     (127)     1812 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/oid
+-rw-r--r--   0 vsts      (1001) docker     (127)     2674 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/os_name
+-rw-r--r--   0 vsts      (1001) docker     (127)     1476 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/powershell.cmdlet
+-rw-r--r--   0 vsts      (1001) docker     (127)      873 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/privilege
+-rw-r--r--   0 vsts      (1001) docker     (127)     1038 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/ransomware.string
+-rw-r--r--   0 vsts      (1001) docker     (127)      263 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/sandbox.id
+-rw-r--r--   0 vsts      (1001) docker     (127)      902 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/security_identifier
+-rw-r--r--   0 vsts      (1001) docker     (127)      151 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/user_agent
+-rw-r--r--   0 vsts      (1001) docker     (127)       53 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/vba.name
+-rw-r--r--   0 vsts      (1001) docker     (127)     2164 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords/windows.registry
+-rw-r--r--   0 vsts      (1001) docker     (127)    22786 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/keywords_to_review.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     2998 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/multidecoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3777 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (127)     1938 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/query.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2440 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      465 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/string_helper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-05-17 00:07:40.000000 multidecoder-1.3.4/src/multidecoder/xor_helper.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.349407 multidecoder-1.3.4/src/multidecoder.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2739 2024-05-17 00:08:15.000000 multidecoder-1.3.4/src/multidecoder.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     7373 2024-05-17 00:08:15.000000 multidecoder-1.3.4/src/multidecoder.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-17 00:08:15.000000 multidecoder-1.3.4/src/multidecoder.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       60 2024-05-17 00:08:15.000000 multidecoder-1.3.4/src/multidecoder.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-17 00:07:53.000000 multidecoder-1.3.4/src/multidecoder.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-05-17 00:08:15.000000 multidecoder-1.3.4/src/multidecoder.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-05-17 00:08:15.000000 multidecoder-1.3.4/src/multidecoder.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.341407 multidecoder-1.3.4/stubs/
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-17 00:07:40.000000 multidecoder-1.3.4/stubs/pefile.pyi
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.341407 multidecoder-1.3.4/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        9 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/requirements.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:08:15.345407 multidecoder-1.3.4/tests/test_decoders/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2953 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_base64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_chr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      397 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_codec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2149 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_concat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      564 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_encoding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_filename.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1644 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_hex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      305 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_javascript.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11797 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_network.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1014 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_path.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      502 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_pe_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      943 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_replace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      394 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_reverse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10165 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_shell.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      960 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_vba.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      702 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_decoders/test_xml.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      892 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_multidecoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      914 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      809 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tests/test_xor_helper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       69 2024-05-17 00:07:40.000000 multidecoder-1.3.4/tox.ini
```

### Comparing `multidecoder-1.3.3/.gitignore` & `multidecoder-1.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/.vscode/settings.json` & `multidecoder-1.3.4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/LICENSE.md` & `multidecoder-1.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/PKG-INFO` & `multidecoder-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidecoder
-Version: 1.3.3
+Version: 1.3.4
 Summary: A context preserving IOC extraction library
 Home-page: https://github.com/CybercentreCanada/Multidecoder
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CybercentreCanada/Multidecoder/issues
 Keywords: malware,analysis,gc,canada,cse-cst,cse,cst,cyber,cccs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: multidecoder Version: 1.3.3 Summary: A context
+Metadata-Version: 2.1 Name: multidecoder Version: 1.3.4 Summary: A context
 preserving IOC extraction library Home-page: https://github.com/
 CybercentreCanada/Multidecoder Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca License: MIT Project-URL: Bug Tracker,
 https://github.com/CybercentreCanada/Multidecoder/issues Keywords:
 malware,analysis,gc,canada,cse-cst,cse,cst,cyber,cccs Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
```

### Comparing `multidecoder-1.3.3/README.md` & `multidecoder-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/pipelines/azure-tests.yaml` & `multidecoder-1.3.4/pipelines/azure-tests.yaml`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/pipelines/publish.yaml` & `multidecoder-1.3.4/pipelines/publish.yaml`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/pyproject.toml` & `multidecoder-1.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/setup.cfg` & `multidecoder-1.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/__main__.py` & `multidecoder-1.3.4/src/multidecoder/__main__.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/decoders/base64.py` & `multidecoder-1.3.4/src/multidecoder/decoders/base64.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/decoders/chr.py` & `multidecoder-1.3.4/src/multidecoder/decoders/chr.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/decoders/codec.py` & `multidecoder-1.3.4/src/multidecoder/decoders/codec.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """
 Character encodings
 """
+
 from __future__ import annotations
 
 import regex as re
 
 from multidecoder.node import Node
 from multidecoder.registry import decoder
 
-UTF16_RE = rb"(?s)(?:[^\x00-\x08\x0e-\x1f\x7f-\x9f]\x00){14,}"
+UTF16_RE = (
+    rb"(?s)(?:[^\x00-\x08\x0e-\x1f\x7f-\x9f]\x00){7,}"
+    rb"(?:\x00\x00(?:\x00\x00)?(?:[^\x00-\x08\x0e-\x1f\x7f-\x9f]\x00){7,})*"
+)
 
 
 @decoder
 def find_utf16(data: bytes) -> list[Node]:
     """Find utf-16 and convert it to utf-8"""
     return [
         Node(
```

### Comparing `multidecoder-1.3.3/src/multidecoder/decoders/concat.py` & `multidecoder-1.3.4/src/multidecoder/decoders/concat.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 
 DOUBLE_QUOTE_ESCAPES = rb'\\""|""|\\"|`"'
 # Single or double quoted strings with various possible escapes for ' or "
 DOUBLE_QUOTE_STRING_RE = rb'"(?:' + DOUBLE_QUOTE_ESCAPES + rb'|[^"])*"'
 SINGLE_QUOTE_STRING_RE = rb"'(?:[^']|'')*'"
 STRING_RE = rb"(?:" + DOUBLE_QUOTE_STRING_RE + rb"|" + SINGLE_QUOTE_STRING_RE + rb")"
 # _ is VB line continuation character
-CONCAT_RE = rb"(?:" + STRING_RE + rb"[\s_]*(?:&|\+|&amp;)[\s_]*)+" + STRING_RE
+CONCAT_SPACER_RE = rb"[\s_]*(?:&|\+|&amp;)[\s_]*"
+CONCAT_RE = rb"(?:" + STRING_RE + CONCAT_SPACER_RE + rb")+" + STRING_RE
 
 
 @decoder
 def find_concat(data: bytes) -> list[Node]:
     """Find and decode string concatenation"""
     return [
         Node(
             "string",
-            b"".join(string[1:-1] for string in re.findall(STRING_RE, match.group())),
+            re.sub(rb"['\"]" + CONCAT_SPACER_RE + rb"['\"]", b"", match.group())[1:-1],
             "concatenation",
             match.start(),
             match.end(),
         )
         for match in re.finditer(CONCAT_RE, data)
     ]
```

### Comparing `multidecoder-1.3.3/src/multidecoder/decoders/filename.py` & `multidecoder-1.3.4/src/multidecoder/decoders/filename.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/decoders/hex.py` & `multidecoder-1.3.4/src/multidecoder/decoders/hex.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/decoders/network.py` & `multidecoder-1.3.4/src/multidecoder/decoders/network.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,24 @@
     return bool(split.scheme and split.hostname and split.scheme in (b"http", b"https", b"ftp"))
 
 
 # Decoders
 @decoder
 def find_domains(data: bytes) -> list[Node]:
     """Find domains in data"""
-    return [match_to_hit(DOMAIN_TYPE, match) for match in re.finditer(DOMAIN_RE, data) if is_domain(match.group())]
+    # Common domain false positives
+    domain_fpos = {b"wscript.shell", b"system.io"}
+    return [
+        match_to_hit(DOMAIN_TYPE, match)
+        for match in re.finditer(DOMAIN_RE, data)
+        if is_domain(match.group())
+        and len(match.group()) >= 6
+        and not re.match(b"[a-z]+[.][A-Z][a-z]+", match.group())
+        and match.group().lower() not in domain_fpos
+    ]
 
 
 @decoder
 def find_emails(data: bytes) -> list[Node]:
     """Find email addresses in data"""
     return [match_to_hit(EMAIL_TYPE, match) for match in re.finditer(EMAIL_RE, data) if is_domain(match.group(1))]
 
@@ -118,18 +127,23 @@
 def find_ips(data: bytes) -> list[Node]:
     """Find ip addresses in data"""
     out = []
     for match in re.finditer(IP_RE, data):
         ip = match.group()
         if not is_ip(ip):
             continue
+        if all(byte in b"0x." for byte in ip):
+            continue  # 0.0.0.0
+        if ip.endswith((b".0", b".255")):
+            continue  # Class C network identifier or broadcast address
         start, end = match.span()
         if data[start - 3 : start] == b"<t>" and data[end : end + 4] == b"</t>":
             continue  # xml section numbering
-        if data[start - 8 : start - 1] == b"Version" and data[start - 1 : start] in (b"\0", b"="):
+        offset = data.rfind(b"Version", max(start - 10, 0), start)
+        if offset >= 0 and re.match(rb"[\x00=\s]+$", data[offset + 7 : start]):
             continue  # version number, not an ip address
         out.append(parse_ip(match.group()).shift(match.start()))
     return out
 
 
 @decoder
 def find_urls(data: bytes) -> list[Node]:
@@ -141,19 +155,25 @@
         ord("("): ord(")"),
     }
     out = []
     for match in re.finditer(URL_RE, data):
         group = match.group()
         start, end = match.span()
         prev = data[start - 1]
-        if start != 0 and prev in contexts:
+        if start == 0:
+            pass  # No context
+        elif group[prev : prev + 1] == b"0":
+            # Pascal string in PE file
+            end = start + prev
+            group = group[:prev]
+        elif prev in contexts:
             close = group.find(contexts[prev])
             if close > -1:
-                end = close
-                group = group[:end]
+                end = start + close
+                group = group[:close]
         if not is_url(group):
             continue
         out.append(
             Node(
                 URL_TYPE,
                 *normalize_percent_encoding(group),
                 start,
```

### Comparing `multidecoder-1.3.3/src/multidecoder/decoders/path.py` & `multidecoder-1.3.4/src/multidecoder/decoders/path.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/decoders/pe_file.py` & `multidecoder-1.3.4/src/multidecoder/decoders/pe_file.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/decoders/replace.py` & `multidecoder-1.3.4/src/multidecoder/decoders/replace.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/decoders/shell.py` & `multidecoder-1.3.4/src/multidecoder/decoders/shell.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/decoders/vba.py` & `multidecoder-1.3.4/src/multidecoder/decoders/vba.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/decoders/xml.py` & `multidecoder-1.3.4/src/multidecoder/decoders/xml.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/domains.py` & `multidecoder-1.3.4/src/multidecoder/domains.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/hit.py` & `multidecoder-1.3.4/src/multidecoder/hit.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/json_conversion.py` & `multidecoder-1.3.4/src/multidecoder/json_conversion.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keyword.py` & `multidecoder-1.3.4/src/multidecoder/keyword.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.advapi32` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.advapi32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.atl` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.atl`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.dbghelp` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.dbghelp`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.gdi32` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.gdi32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.imagehlp` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.imagehlp`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.iphlpapi` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.iphlpapi`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.kernel32` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.kernel32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.libeay32` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.libeay32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.mfc42` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.mfc42`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.msi` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.msi`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.mssign32` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.mssign32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.msvbvm60` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.msvbvm60`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.msvcrt` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.msvcrt`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.nddeapi` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.nddeapi`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.netapi32` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.netapi32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.ntdll` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.ntdll`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.ntoskrnl` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.ntoskrnl`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.odbc32` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.odbc32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.odbccp32` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.odbccp32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.ole32` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.ole32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.oleaut32` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.oleaut32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.packet` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.packet`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.powrprof` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.powrprof`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.rpcrt4` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.rpcrt4`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.scecli` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.scecli`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.se` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.se`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.shell32` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.shell32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.shlwapi` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.shlwapi`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.ssleay32` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.ssleay32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.urlmon` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.urlmon`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.user32` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.user32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.wininet` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.wininet`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.winsock` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.winsock`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.winsta` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.winsta`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/api/api.wsnmp32` & `multidecoder-1.3.4/src/multidecoder/keywords/api/api.wsnmp32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/event` & `multidecoder-1.3.4/src/multidecoder/keywords/event`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/guid` & `multidecoder-1.3.4/src/multidecoder/keywords/guid`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/key` & `multidecoder-1.3.4/src/multidecoder/keywords/key`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/network.string` & `multidecoder-1.3.4/src/multidecoder/keywords/network.string`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/oid` & `multidecoder-1.3.4/src/multidecoder/keywords/oid`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/os_name` & `multidecoder-1.3.4/src/multidecoder/keywords/os_name`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/powershell.cmdlet` & `multidecoder-1.3.4/src/multidecoder/keywords/powershell.cmdlet`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/privilege` & `multidecoder-1.3.4/src/multidecoder/keywords/privilege`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/ransomware.string` & `multidecoder-1.3.4/src/multidecoder/keywords/ransomware.string`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/security_identifier` & `multidecoder-1.3.4/src/multidecoder/keywords/security_identifier`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords/windows.registry` & `multidecoder-1.3.4/src/multidecoder/keywords/windows.registry`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/keywords_to_review.txt` & `multidecoder-1.3.4/src/multidecoder/keywords_to_review.txt`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/multidecoder.py` & `multidecoder-1.3.4/src/multidecoder/multidecoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,16 @@
         for hit in results:
             # Ignore values if in a decoded context
             if hit.end <= decode_end:
                 continue
             # Return to the context that contains the current hit
             while hit.end > offset + len(node.value):
                 offset -= node.start
-                node = stack.pop()
+                if stack:  # Todo: Log here
+                    node = stack.pop()
             hit.shift(-offset)
             # Prevent analyzer rematching its own decoded output
             if hit.start == 0 and hit.value == node.value and hit.type == node.type:
                 continue
             hit.parent = node
             node.children.append(hit)
```

### Comparing `multidecoder-1.3.3/src/multidecoder/node.py` & `multidecoder-1.3.4/src/multidecoder/node.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/query.py` & `multidecoder-1.3.4/src/multidecoder/query.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/registry.py` & `multidecoder-1.3.4/src/multidecoder/registry.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder/xor_helper.py` & `multidecoder-1.3.4/src/multidecoder/xor_helper.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/src/multidecoder.egg-info/PKG-INFO` & `multidecoder-1.3.4/src/multidecoder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidecoder
-Version: 1.3.3
+Version: 1.3.4
 Summary: A context preserving IOC extraction library
 Home-page: https://github.com/CybercentreCanada/Multidecoder
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CybercentreCanada/Multidecoder/issues
 Keywords: malware,analysis,gc,canada,cse-cst,cse,cst,cyber,cccs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: multidecoder Version: 1.3.3 Summary: A context
+Metadata-Version: 2.1 Name: multidecoder Version: 1.3.4 Summary: A context
 preserving IOC extraction library Home-page: https://github.com/
 CybercentreCanada/Multidecoder Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca License: MIT Project-URL: Bug Tracker,
 https://github.com/CybercentreCanada/Multidecoder/issues Keywords:
 malware,analysis,gc,canada,cse-cst,cse,cst,cyber,cccs Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
```

### Comparing `multidecoder-1.3.3/src/multidecoder.egg-info/SOURCES.txt` & `multidecoder-1.3.4/src/multidecoder.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 src/multidecoder/decoders/filename.py
 src/multidecoder/decoders/hex.py
 src/multidecoder/decoders/javascript.py
 src/multidecoder/decoders/network.py
 src/multidecoder/decoders/path.py
 src/multidecoder/decoders/pe_file.py
 src/multidecoder/decoders/replace.py
+src/multidecoder/decoders/reverse.py
 src/multidecoder/decoders/shell.py
 src/multidecoder/decoders/vba.py
 src/multidecoder/decoders/xml.py
 src/multidecoder/keywords/archive
 src/multidecoder/keywords/av.name
 src/multidecoder/keywords/cryptography
 src/multidecoder/keywords/debugger.device.name
@@ -178,19 +179,21 @@
 tests/__init__.py
 tests/requirements.txt
 tests/test_multidecoder.py
 tests/test_node.py
 tests/test_xor_helper.py
 tests/test_decoders/test_base64.py
 tests/test_decoders/test_chr.py
+tests/test_decoders/test_codec.py
 tests/test_decoders/test_concat.py
 tests/test_decoders/test_encoding.py
 tests/test_decoders/test_filename.py
 tests/test_decoders/test_hex.py
 tests/test_decoders/test_javascript.py
 tests/test_decoders/test_network.py
 tests/test_decoders/test_path.py
 tests/test_decoders/test_pe_file.py
 tests/test_decoders/test_replace.py
+tests/test_decoders/test_reverse.py
 tests/test_decoders/test_shell.py
 tests/test_decoders/test_vba.py
 tests/test_decoders/test_xml.py
```

### Comparing `multidecoder-1.3.3/tests/test_decoders/test_base64.py` & `multidecoder-1.3.4/tests/test_decoders/test_base64.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/tests/test_decoders/test_chr.py` & `multidecoder-1.3.4/tests/test_decoders/test_chr.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/tests/test_decoders/test_concat.py` & `multidecoder-1.3.4/tests/test_decoders/test_concat.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/tests/test_decoders/test_encoding.py` & `multidecoder-1.3.4/tests/test_decoders/test_encoding.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/tests/test_decoders/test_hex.py` & `multidecoder-1.3.4/tests/test_decoders/test_hex.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/tests/test_decoders/test_network.py` & `multidecoder-1.3.4/tests/test_decoders/test_network.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import pytest
 from multidecoder.decoders.network import (
     DOMAIN_RE,
     EMAIL_RE,
     IP_RE,
     URL_RE,
-    # find_domains,
+    find_domains,
     find_ips,
     find_urls,
     is_domain,
     is_url,
     parse_ip,
 )
 from multidecoder.node import Node
@@ -77,15 +77,25 @@
 
 def test_parse_ip():
     assert parse_ip(b"8.8.8.8") == Node("network.ip", b"8.8.8.8", "", 0, 7)
 
 
 @pytest.mark.parametrize(
     "data",
-    [b"<si><t>1.1.1.4</t></si>", b"ProductVersion\x004.0.0.0\x00", b"FileVersion\x004.0.0.0\x00", b"Version=4.0.0.0"],
+    [
+        b"<si><t>1.1.1.4</t></si>",
+        b"ProductVersion\x004.0.0.0\x00",
+        b"FileVersion\x004.0.0.0\x00",
+        b"Version=4.0.0.0",
+        b"0.0.0.0",
+        b"Version\x00\x0012.3.0.0\x00",
+        b"Version = 4.0.0.0",
+        b"1.0.0.0",
+        b"1.0.0.255",
+    ],
 )
 def test_find_ips_false_positives(data):
     assert find_ips(data) == []
 
 
 # Domain ----------------------------------------
 
@@ -154,14 +164,24 @@
     ],
 )
 def test_DOMAIN_RE_context(data, domain):
     """Test that DOMAIN_RE matches in context"""
     assert re.search(DOMAIN_RE, data).group() == domain
 
 
+@pytest.mark.parametrize(
+    "data",
+    [
+        b"K.cA",
+    ],
+)
+def test_find_domaind_fpos(data):
+    assert find_domains(data) == []
+
+
 # Email -----------------------------------------
 
 
 def test_email_re():
     assert re.match(EMAIL_RE, b"a_name@gmail.com")
 
 
@@ -283,22 +303,22 @@
                         Node("network.domain", b"example.com", "", 8, 19),
                         Node("network.url.path", b"/path'),.;still_url", "", 19, 38),
                     ],
                 )
             ],
         ),
         (
-            b"'https://example.com/path'after_the_url",
+            b"                              'https://example.com/path'after_the_url",
             [
                 Node(
                     "network.url",
                     b"https://example.com/path",
                     "",
-                    1,
-                    24,
+                    31,
+                    55,
                     children=[
                         Node("network.url.scheme", b"https", "", 0, 5),
                         Node("network.domain", b"example.com", "", 8, 19),
                         Node("network.url.path", b"/path", "", 19, 24),
                     ],
                 )
             ],
@@ -332,11 +352,27 @@
                     children=[
                         Node("network.url.scheme", b"https", "", 0, 5),
                         Node("network.domain", b"example.com", "", 8, 19),
                     ],
                 )
             ],
         ),
+        (
+            b"                    \x13https://example.com0thisisaftertheendoftheurl",
+            [
+                Node(
+                    "network.url",
+                    b"https://example.com",
+                    "",
+                    21,
+                    40,
+                    children=[
+                        Node("network.url.scheme", b"https", "", 0, 5),
+                        Node("network.domain", b"example.com", "", 8, 19),
+                    ],
+                )
+            ],
+        ),
     ],
 )
 def test_find_url(data, urls):
     assert find_urls(data) == urls
```

### Comparing `multidecoder-1.3.3/tests/test_decoders/test_path.py` & `multidecoder-1.3.4/tests/test_decoders/test_path.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/tests/test_decoders/test_replace.py` & `multidecoder-1.3.4/tests/test_decoders/test_replace.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/tests/test_decoders/test_shell.py` & `multidecoder-1.3.4/tests/test_decoders/test_shell.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/tests/test_decoders/test_vba.py` & `multidecoder-1.3.4/tests/test_decoders/test_vba.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/tests/test_decoders/test_xml.py` & `multidecoder-1.3.4/tests/test_decoders/test_xml.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/tests/test_multidecoder.py` & `multidecoder-1.3.4/tests/test_multidecoder.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/tests/test_node.py` & `multidecoder-1.3.4/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.3.3/tests/test_xor_helper.py` & `multidecoder-1.3.4/tests/test_xor_helper.py`

 * *Files identical despite different names*

