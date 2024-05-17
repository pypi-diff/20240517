# Comparing `tmp/cmap-0.2.0.tar.gz` & `tmp/cmap-0.2.1.tar.gz`

## Comparing `cmap-0.2.0.tar` & `cmap-0.2.1.tar`

### file list

```diff
@@ -1,200 +1,200 @@
--rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 cmap-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/__init__.py
--rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/_catalog.py
--rw-r--r--   0        0        0    21048 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/_color.py
--rw-r--r--   0        0        0    54457 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/_colormap.py
--rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/_external.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/_png.py
--rw-r--r--   0        0        0    16225 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/__init__.py
--rw-r--r--   0        0        0    47598 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/bids/__init__.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/bids/record.json
--rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/chrisluts/record.json
--rw-r--r--   0        0        0     9433 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cividis/__init__.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cividis/record.json
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmap/record.json
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/__init__.py
--rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/algae.py
--rw-r--r--   0        0        0    17227 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/amp.py
--rw-r--r--   0        0        0    22339 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/balance.py
--rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/curl.py
--rw-r--r--   0        0        0    11180 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/deep.py
--rw-r--r--   0        0        0    22376 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/delta.py
--rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/dense.py
--rw-r--r--   0        0        0    17153 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/diff.py
--rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/haline.py
--rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/ice.py
--rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/matter.py
--rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/oxy.py
--rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/phase.py
--rw-r--r--   0        0        0    17189 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/rain.py
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/record.json
--rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/solar.py
--rw-r--r--   0        0        0    17281 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/speed.py
--rw-r--r--   0        0        0    21589 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/tarn.py
--rw-r--r--   0        0        0    17165 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/tempo.py
--rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/thermal.py
--rw-r--r--   0        0        0    17171 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/topo.py
--rw-r--r--   0        0        0    11193 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cmocean/turbid.py
--rw-r--r--   0        0        0    39760 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorbrewer/__init__.py
--rw-r--r--   0        0        0    45183 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorbrewer/record.json
--rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C1.py
--rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C10.py
--rw-r--r--   0        0        0     9105 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C11.py
--rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C2.py
--rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C3.py
--rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C4.py
--rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C5.py
--rw-r--r--   0        0        0     8395 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C6.py
--rw-r--r--   0        0        0     8689 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C7.py
--rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C8.py
--rw-r--r--   0        0        0     9142 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_C9.py
--rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBC1.py
--rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBC2.py
--rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBD1.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBD2.py
--rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBL1.py
--rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBL2.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBL3.py
--rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBL4.py
--rw-r--r--   0        0        0     9145 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBTC1.py
--rw-r--r--   0        0        0     9087 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBTC2.py
--rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBTD1.py
--rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBTL1.py
--rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBTL2.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBTL3.py
--rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_CBTL4.py
--rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D1.py
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D10.py
--rw-r--r--   0        0        0     9088 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D11.py
--rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D12.py
--rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D13.py
--rw-r--r--   0        0        0     9168 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D1A.py
--rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D2.py
--rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D3.py
--rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D4.py
--rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D5.py
--rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D6.py
--rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D7.py
--rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D8.py
--rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_D9.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_I1.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_I2.py
--rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_I3.py
--rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L1.py
--rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L10.py
--rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L11.py
--rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L12.py
--rw-r--r--   0        0        0     8173 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L13.py
--rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L14.py
--rw-r--r--   0        0        0     9096 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L15.py
--rw-r--r--   0        0        0     9125 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L16.py
--rw-r--r--   0        0        0     9138 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L17.py
--rw-r--r--   0        0        0     9134 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L18.py
--rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L19.py
--rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L2.py
--rw-r--r--   0        0        0     9149 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L20.py
--rw-r--r--   0        0        0     8152 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L3.py
--rw-r--r--   0        0        0     8021 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L4.py
--rw-r--r--   0        0        0     9108 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L5.py
--rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L6.py
--rw-r--r--   0        0        0     9072 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L7.py
--rw-r--r--   0        0        0     9149 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L8.py
--rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_L9.py
--rw-r--r--   0        0        0     9007 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_R1.py
--rw-r--r--   0        0        0     8697 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_R2.py
--rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_R3.py
--rw-r--r--   0        0        0     9143 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/CET_R4.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/__init__.py
--rw-r--r--   0        0        0    19690 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/colorcet/record.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/__init__.py
--rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/acton.py
--rw-r--r--   0        0        0     9197 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/bam.py
--rw-r--r--   0        0        0     9215 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/bamO.py
--rw-r--r--   0        0        0     9214 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/bamako.py
--rw-r--r--   0        0        0     9224 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/batlow.py
--rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/batlowK.py
--rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/batlowW.py
--rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/berlin.py
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/bilbao.py
--rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/broc.py
--rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/brocO.py
--rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/buda.py
--rw-r--r--   0        0        0     9215 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/bukavu.py
--rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/cork.py
--rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/corkO.py
--rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/davos.py
--rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/devon.py
--rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/fes.py
--rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/grayC.py
--rw-r--r--   0        0        0     9216 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/hawaii.py
--rw-r--r--   0        0        0     9227 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/imola.py
--rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/lajolla.py
--rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/lapaz.py
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/lisbon.py
--rw-r--r--   0        0        0     9196 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/nuuk.py
--rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/oleron.py
--rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/oslo.py
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/record.json
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/roma.py
--rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/romaO.py
--rw-r--r--   0        0        0     9212 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/tofino.py
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/tokyo.py
--rw-r--r--   0        0        0     9172 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/turku.py
--rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/vanimo.py
--rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/vik.py
--rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/crameri/vikO.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cubehelix/__init__.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/cubehelix/record.json
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/glasbey/__init__.py
--rw-r--r--   0        0        0     8584 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/glasbey/_glasbey.py
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/glasbey/_grids.py
--rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/glasbey/_internals.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/glasbey/prebuilt.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/glasbey/record.json
--rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/gnuplot/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/gnuplot/record.json
--rw-r--r--   0        0        0     8749 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/google/__init__.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/google/record.json
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/imagej/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/imagej/record.json
--rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/matlab/__init__.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/matlab/record.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/matplotlib/_CMRmap.py
--rw-r--r--   0        0        0    45911 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/matplotlib/__init__.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/matplotlib/_coolwarm.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/matplotlib/_wistia.py
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/matplotlib/record.json
--rw-r--r--   0        0        0    64086 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/seaborn/__init__.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/seaborn/record.json
--rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/tableau/__init__.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/tableau/record.json
--rw-r--r--   0        0        0    12471 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/tol/__init__.py
--rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/tol/record.json
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/vispy/__init__.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/vispy/record.json
--rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/yorick/__init__.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 cmap-0.2.0/src/cmap/data/yorick/record.json
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 cmap-0.2.0/tests/test_catalog.py
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 cmap-0.2.0/tests/test_color.py
--rw-r--r--   0        0        0     7864 2020-02-02 00:00:00.000000 cmap-0.2.0/tests/test_colormap.py
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 cmap-0.2.0/tests/test_data.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 cmap-0.2.0/tests/test_glasbey.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 cmap-0.2.0/tests/test_model_fields.py
--rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 cmap-0.2.0/tests/test_third_party.py
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 cmap-0.2.0/tests/test_utils.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 cmap-0.2.0/.gitignore
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 cmap-0.2.0/README.md
--rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 cmap-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 cmap-0.2.0/LICENSE/LICENSE
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 cmap-0.2.0/LICENSE/LICENSE_CMOCEAN
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 cmap-0.2.0/LICENSE/LICENSE_COLORBREWER
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cmap-0.2.0/LICENSE/LICENSE_COLORCET
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cmap-0.2.0/LICENSE/LICENSE_CRAMERI
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 cmap-0.2.0/LICENSE/LICENSE_CVIDIS
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cmap-0.2.0/LICENSE/LICENSE_GLASBEY
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 cmap-0.2.0/LICENSE/LICENSE_TOL
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 cmap-0.2.0/LICENSE/LICENSE_WISTIA
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 cmap-0.2.0/LICENSE/LICENSE_YORICK
--rw-r--r--   0        0        0    10578 2020-02-02 00:00:00.000000 cmap-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 cmap-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/__init__.py
+-rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/_catalog.py
+-rw-r--r--   0        0        0    21048 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/_color.py
+-rw-r--r--   0        0        0    57414 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/_colormap.py
+-rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/_external.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/_png.py
+-rw-r--r--   0        0        0    16225 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/__init__.py
+-rw-r--r--   0        0        0    47598 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/bids/__init__.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/bids/record.json
+-rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/chrisluts/record.json
+-rw-r--r--   0        0        0     9433 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cividis/__init__.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cividis/record.json
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmap/record.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/__init__.py
+-rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/algae.py
+-rw-r--r--   0        0        0    17227 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/amp.py
+-rw-r--r--   0        0        0    22339 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/balance.py
+-rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/curl.py
+-rw-r--r--   0        0        0    11180 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/deep.py
+-rw-r--r--   0        0        0    22376 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/delta.py
+-rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/dense.py
+-rw-r--r--   0        0        0    17153 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/diff.py
+-rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/haline.py
+-rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/ice.py
+-rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/matter.py
+-rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/oxy.py
+-rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/phase.py
+-rw-r--r--   0        0        0    17189 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/rain.py
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/record.json
+-rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/solar.py
+-rw-r--r--   0        0        0    17281 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/speed.py
+-rw-r--r--   0        0        0    21589 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/tarn.py
+-rw-r--r--   0        0        0    17165 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/tempo.py
+-rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/thermal.py
+-rw-r--r--   0        0        0    17171 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/topo.py
+-rw-r--r--   0        0        0    11193 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cmocean/turbid.py
+-rw-r--r--   0        0        0    39760 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorbrewer/__init__.py
+-rw-r--r--   0        0        0    45183 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorbrewer/record.json
+-rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_C1.py
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_C10.py
+-rw-r--r--   0        0        0     9105 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_C11.py
+-rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_C2.py
+-rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_C3.py
+-rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_C4.py
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_C5.py
+-rw-r--r--   0        0        0     8395 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_C6.py
+-rw-r--r--   0        0        0     8689 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_C7.py
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_C8.py
+-rw-r--r--   0        0        0     9142 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_C9.py
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_CBC1.py
+-rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_CBC2.py
+-rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_CBD1.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_CBD2.py
+-rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_CBL1.py
+-rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_CBL2.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_CBL3.py
+-rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_CBL4.py
+-rw-r--r--   0        0        0     9145 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_CBTC1.py
+-rw-r--r--   0        0        0     9087 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_CBTC2.py
+-rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_CBTD1.py
+-rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_CBTL1.py
+-rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_CBTL2.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_CBTL3.py
+-rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_CBTL4.py
+-rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_D1.py
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_D10.py
+-rw-r--r--   0        0        0     9088 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_D11.py
+-rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_D12.py
+-rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_D13.py
+-rw-r--r--   0        0        0     9168 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_D1A.py
+-rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_D2.py
+-rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_D3.py
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_D4.py
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_D5.py
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_D6.py
+-rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_D7.py
+-rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_D8.py
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_D9.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_I1.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_I2.py
+-rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_I3.py
+-rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_L1.py
+-rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_L10.py
+-rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_L11.py
+-rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_L12.py
+-rw-r--r--   0        0        0     8173 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_L13.py
+-rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_L14.py
+-rw-r--r--   0        0        0     9096 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_L15.py
+-rw-r--r--   0        0        0     9125 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_L16.py
+-rw-r--r--   0        0        0     9138 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_L17.py
+-rw-r--r--   0        0        0     9134 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_L18.py
+-rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_L19.py
+-rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_L2.py
+-rw-r--r--   0        0        0     9149 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_L20.py
+-rw-r--r--   0        0        0     8152 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_L3.py
+-rw-r--r--   0        0        0     8021 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_L4.py
+-rw-r--r--   0        0        0     9108 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_L5.py
+-rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_L6.py
+-rw-r--r--   0        0        0     9072 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_L7.py
+-rw-r--r--   0        0        0     9149 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_L8.py
+-rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_L9.py
+-rw-r--r--   0        0        0     9007 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_R1.py
+-rw-r--r--   0        0        0     8697 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_R2.py
+-rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_R3.py
+-rw-r--r--   0        0        0     9143 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/CET_R4.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/__init__.py
+-rw-r--r--   0        0        0    19690 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/colorcet/record.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/__init__.py
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/acton.py
+-rw-r--r--   0        0        0     9197 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/bam.py
+-rw-r--r--   0        0        0     9215 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/bamO.py
+-rw-r--r--   0        0        0     9214 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/bamako.py
+-rw-r--r--   0        0        0     9224 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/batlow.py
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/batlowK.py
+-rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/batlowW.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/berlin.py
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/bilbao.py
+-rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/broc.py
+-rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/brocO.py
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/buda.py
+-rw-r--r--   0        0        0     9215 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/bukavu.py
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/cork.py
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/corkO.py
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/davos.py
+-rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/devon.py
+-rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/fes.py
+-rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/grayC.py
+-rw-r--r--   0        0        0     9216 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/hawaii.py
+-rw-r--r--   0        0        0     9227 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/imola.py
+-rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/lajolla.py
+-rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/lapaz.py
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/lisbon.py
+-rw-r--r--   0        0        0     9196 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/nuuk.py
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/oleron.py
+-rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/oslo.py
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/record.json
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/roma.py
+-rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/romaO.py
+-rw-r--r--   0        0        0     9212 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/tofino.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/tokyo.py
+-rw-r--r--   0        0        0     9172 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/turku.py
+-rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/vanimo.py
+-rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/vik.py
+-rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/crameri/vikO.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cubehelix/__init__.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/cubehelix/record.json
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/glasbey/__init__.py
+-rw-r--r--   0        0        0     8584 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/glasbey/_glasbey.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/glasbey/_grids.py
+-rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/glasbey/_internals.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/glasbey/prebuilt.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/glasbey/record.json
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/gnuplot/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/gnuplot/record.json
+-rw-r--r--   0        0        0     8749 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/google/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/google/record.json
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/imagej/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/imagej/record.json
+-rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/matlab/__init__.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/matlab/record.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/matplotlib/_CMRmap.py
+-rw-r--r--   0        0        0    45911 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/matplotlib/__init__.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/matplotlib/_coolwarm.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/matplotlib/_wistia.py
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/matplotlib/record.json
+-rw-r--r--   0        0        0    64086 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/seaborn/__init__.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/seaborn/record.json
+-rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/tableau/__init__.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/tableau/record.json
+-rw-r--r--   0        0        0    12471 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/tol/__init__.py
+-rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/tol/record.json
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/vispy/__init__.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/vispy/record.json
+-rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/yorick/__init__.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 cmap-0.2.1/src/cmap/data/yorick/record.json
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 cmap-0.2.1/tests/test_catalog.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 cmap-0.2.1/tests/test_color.py
+-rw-r--r--   0        0        0     7864 2020-02-02 00:00:00.000000 cmap-0.2.1/tests/test_colormap.py
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 cmap-0.2.1/tests/test_data.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 cmap-0.2.1/tests/test_glasbey.py
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 cmap-0.2.1/tests/test_model_fields.py
+-rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 cmap-0.2.1/tests/test_third_party.py
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 cmap-0.2.1/tests/test_utils.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 cmap-0.2.1/.gitignore
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 cmap-0.2.1/README.md
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 cmap-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 cmap-0.2.1/LICENSE/LICENSE
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 cmap-0.2.1/LICENSE/LICENSE_CMOCEAN
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 cmap-0.2.1/LICENSE/LICENSE_COLORBREWER
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cmap-0.2.1/LICENSE/LICENSE_COLORCET
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cmap-0.2.1/LICENSE/LICENSE_CRAMERI
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 cmap-0.2.1/LICENSE/LICENSE_CVIDIS
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cmap-0.2.1/LICENSE/LICENSE_GLASBEY
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 cmap-0.2.1/LICENSE/LICENSE_TOL
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 cmap-0.2.1/LICENSE/LICENSE_WISTIA
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 cmap-0.2.1/LICENSE/LICENSE_YORICK
+-rw-r--r--   0        0        0    10578 2020-02-02 00:00:00.000000 cmap-0.2.1/PKG-INFO
```

### Comparing `cmap-0.2.0/CHANGELOG.md` & `cmap-0.2.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 # Changelog
 
-## [v0.2.0](https://github.com/tlambert03/cmap/tree/v0.2.0) (2024-04-28)
+## [v0.2.1](https://github.com/tlambert03/cmap/tree/v0.2.1) (2024-05-17)
 
-[Full Changelog](https://github.com/tlambert03/cmap/compare/v0.2.0...v0.2.0)
+[Full Changelog](https://github.com/tlambert03/cmap/compare/v0.2.0...v0.2.1)
 
 **Implemented enhancements:**
 
-- feat: add shifted method [\#52](https://github.com/tlambert03/cmap/pull/52) ([tlambert03](https://github.com/tlambert03))
-- feat: add over/under/bad colors [\#50](https://github.com/tlambert03/cmap/pull/50) ([tlambert03](https://github.com/tlambert03))
-- feat: add Paul Tol's colormaps [\#48](https://github.com/tlambert03/cmap/pull/48) ([Jhsmit](https://github.com/Jhsmit))
-
-**Fixed bugs:**
-
-- fix: fix interpolation argument preservation in custom colormaps [\#47](https://github.com/tlambert03/cmap/pull/47) ([tlambert03](https://github.com/tlambert03))
+- Expose `Colormap.num_colors` and document usage for cycling through qualitative colormaps  [\#55](https://github.com/tlambert03/cmap/pull/55) ([andy-sweet](https://github.com/andy-sweet))
 
 **Documentation:**
 
-- docs: use natsort for docs [\#51](https://github.com/tlambert03/cmap/pull/51) ([tlambert03](https://github.com/tlambert03))
-
-**Merged pull requests:**
+- docs: make colormap attributes more visible [\#56](https://github.com/tlambert03/cmap/pull/56) ([tlambert03](https://github.com/tlambert03))
 
-- ci\(dependabot\): bump softprops/action-gh-release from 1 to 2 [\#42](https://github.com/tlambert03/cmap/pull/42) ([dependabot[bot]](https://github.com/apps/dependabot))
-- chore: use ruff instead of black [\#41](https://github.com/tlambert03/cmap/pull/41) ([tlambert03](https://github.com/tlambert03))
-
-## [v0.2.0](https://github.com/tlambert03/cmap/tree/v0.2.0) (2024-03-09)
+## [v0.2.0](https://github.com/tlambert03/cmap/tree/v0.2.0) (2024-04-28)
 
 [Full Changelog](https://github.com/tlambert03/cmap/compare/v0.1.3...v0.2.0)
 
 **Implemented enhancements:**
 
+- feat: add shifted method [\#52](https://github.com/tlambert03/cmap/pull/52) ([tlambert03](https://github.com/tlambert03))
+- feat: add over/under/bad colors [\#50](https://github.com/tlambert03/cmap/pull/50) ([tlambert03](https://github.com/tlambert03))
+- feat: add Paul Tol's colormaps [\#48](https://github.com/tlambert03/cmap/pull/48) ([Jhsmit](https://github.com/Jhsmit))
 - feat: add support for pyqtgraph [\#32](https://github.com/tlambert03/cmap/pull/32) ([tlambert03](https://github.com/tlambert03))
 
 **Fixed bugs:**
 
+- fix: fix interpolation argument preservation in custom colormaps [\#47](https://github.com/tlambert03/cmap/pull/47) ([tlambert03](https://github.com/tlambert03))
 - fix: misc fixes for pydantic deprecations and other breakages [\#38](https://github.com/tlambert03/cmap/pull/38) ([tlambert03](https://github.com/tlambert03))
 
+**Documentation:**
+
+- docs: use natsort for docs [\#51](https://github.com/tlambert03/cmap/pull/51) ([tlambert03](https://github.com/tlambert03))
+
 **Merged pull requests:**
 
+- ci\(dependabot\): bump softprops/action-gh-release from 1 to 2 [\#42](https://github.com/tlambert03/cmap/pull/42) ([dependabot[bot]](https://github.com/apps/dependabot))
+- chore: use ruff instead of black [\#41](https://github.com/tlambert03/cmap/pull/41) ([tlambert03](https://github.com/tlambert03))
 - test: Add test\_min extra and make sure tests run with bare minimum [\#40](https://github.com/tlambert03/cmap/pull/40) ([tlambert03](https://github.com/tlambert03))
 - ci\(dependabot\): bump aganders3/headless-gui from 2.1 to 2.2 [\#37](https://github.com/tlambert03/cmap/pull/37) ([dependabot[bot]](https://github.com/apps/dependabot))
 - ci\(dependabot\): bump codecov/codecov-action from 3 to 4 [\#36](https://github.com/tlambert03/cmap/pull/36) ([dependabot[bot]](https://github.com/apps/dependabot))
 - ci\(dependabot\): bump actions/setup-python from 4 to 5 [\#34](https://github.com/tlambert03/cmap/pull/34) ([dependabot[bot]](https://github.com/apps/dependabot))
 - ci\(dependabot\): bump aganders3/headless-gui from 1.2 to 2.1 [\#33](https://github.com/tlambert03/cmap/pull/33) ([dependabot[bot]](https://github.com/apps/dependabot))
 
 ## [v0.1.3](https://github.com/tlambert03/cmap/tree/v0.1.3) (2023-12-04)
```

### Comparing `cmap-0.2.0/src/cmap/__init__.py` & `cmap-0.2.1/src/cmap/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 try:
     __version__ = version("cmap")
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "uninstalled"
 
 
 from ._color import HSLA, HSVA, RGBA, RGBA8, Color
-from ._colormap import Colormap
+from ._colormap import Colormap, ColorStops
 
 if TYPE_CHECKING:
     from ._catalog import CatalogItem
 
     class Catalog(Mapping[str, CatalogItem]):
         """Catalog of available colormaps."""
 
@@ -58,16 +58,17 @@
         def resolve(self, name: str) -> str:
             """Return the fully qualified, normalized name of a colormap or alias."""
 
 else:
     from ._catalog import Catalog, CatalogItem
 
 __all__ = [
+    "Catalog",
+    "CatalogItem",
     "Color",
     "Colormap",
-    "CatalogItem",
-    "Catalog",
+    "ColorStops",
     "HSLA",
     "HSVA",
     "RGBA",
     "RGBA8",
 ]
```

### Comparing `cmap-0.2.0/src/cmap/_catalog.py` & `cmap-0.2.1/src/cmap/_catalog.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/_color.py` & `cmap-0.2.1/src/cmap/_color.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/_colormap.py` & `cmap-0.2.1/src/cmap/_colormap.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,18 @@
 
 BAD_COLOR = (0.0, 0.0, 0.0, 0.0)
 
 
 class Colormap:
     """A colormap is a mapping from scalar values to RGB(A) colors.
 
+    The primary way to apply a colormap to data is to call the colormap object with
+    scalar values, which will return an array of RGBA colors.  See
+    [`Colormap.__call__`][cmap.Colormap.__call__] for details.
+
     Parameters
     ----------
     value : Color | ColorStop | Iterable[Color | ColorStop] | dict[float, Color]
         The color data to use for the colormap. Can be a single color, a single
         color stop, a sequence of colors and/or color stops, or a dictionary
         mapping scalar values to colors.
 
@@ -127,15 +131,73 @@
         "over_color",
         "under_color",
         "_initialized",
         "_lut_cache",
         "__weakref__",
     )
 
-    #: ColorStops dett
+    color_stops: ColorStops
+    """The color stops in the colormap.
+
+    This object is a sequence of color stops: a color
+    (RGBA) and a scalar position (0-1) in the gradient.  This is the primary data
+    structure used to represent the colormap. See [`ColorStops`][cmap.ColorStops]
+    docstring for more information.
+    """
+
+    name: str
+    """A display name for the colormap.
+
+    If not provided explicitly, and if the colormap is a catalog colormap, this
+    will be set to `"namespace:name"`.  If not a catalog colormap, it will be set
+    to the `identifier`, or fallback to `"custom colormap"`.
+    """
+
+    identifier: str
+    """An identifier for the colormaps.
+
+    If not provided, it will be generated from `name` by discarding any
+    characters that are not alphanumeric, spaces, dashes, or underscores, converting
+    to lowercase, replacing spaces and dashes with underscores, and prefacing with
+    `"_"` if the first character is a digit.
+    """
+
+    category: str | None
+    """An optional category for the colormap.
+
+    If not provided, and if the colormap is a catalog colormap, this will be set to
+    the category of the colormap.
+    """
+
+    interpolation: Interpolation
+    """The interpolation mode to use when mapping scalar values to colors.
+
+    Either `"linear"` or `"nearest"`, where `"linear"` is the default.
+    """
+
+    under_color: Color | None
+    """A color to use for values below 0 when converting scalars to colors.
+
+    If provided, and `Colormap.lut` is called with `with_over_under=True`, `under_color`
+    will be the third-to-last color in the LUT (`lut[-3]`).
+    """
+
+    over_color: Color | None
+    """A color to use for values above 1 when converting scalars to colors.
+
+    If provided, and `Colormap.lut` is called with `with_over_under=True`, `over_color`
+    will be the second-to-last color in the LUT (`lut[-2]`).
+    """
+
+    bad_color: Color | None
+    """A color to use for missing/bad values when converting scalars to colors.
+
+    If provided, and `Colormap.lut` is called with `with_over_under=True`, `bad_color`
+    will be the last color in the LUT (`lut[-1]`).
+    """
 
     _catalog_instance: Catalog | None = None
 
     @classmethod
     def catalog(cls) -> Catalog:
         """Return the global colormaps catalog."""
         if cls._catalog_instance is None:
@@ -193,20 +255,20 @@
         else:
             stops = _parse_colorstops(value)
 
         name = name or identifier
         if not name:
             name = value if isinstance(value, str) else "custom colormap"
 
-        self.interpolation: Interpolation = _norm_interp(interpolation)
+        self.interpolation = _norm_interp(interpolation)
         stops._interpolation = self.interpolation
-        self.color_stops: ColorStops = stops
-        self.name: str = name
-        self.identifier: str = _make_identifier(identifier or name)
-        self.category: str | None = category
+        self.color_stops = stops
+        self.name = name
+        self.identifier = _make_identifier(identifier or name)
+        self.category = category
 
         self.under_color = None if under is None else Color(under)
         self.over_color = None if over is None else Color(over)
         self.bad_color = None if bad is None else Color(bad)
 
         self._lut_cache: dict[LutCacheKey, np.ndarray] = {}
         self._initialized = True
@@ -407,15 +469,15 @@
 
         Yields
         ------
         color: Color
             Color objects.
         """
         if N is None:
-            N = len(self.color_stops)
+            N = self.num_colors
         nums = np.linspace(0, 1, N) if isinstance(N, int) else np.asarray(N)
         for c in self(nums, N=len(nums)):
             yield Color(c)
 
     def reversed(self, name: str | None = None) -> Colormap:
         """Return a new Colormap, with reversed colors.
 
@@ -506,14 +568,19 @@
             90deg, rgb(0, 0, 255) 0%, rgb(255, 0, 0) 50%, rgb(0, 255, 0) 100%
         );
         """
         return self.color_stops.to_css(
             max_stops=max_stops, angle=angle, radial=radial, as_hex=as_hex
         )
 
+    @property
+    def num_colors(self) -> int:
+        """The number of colors in this colormap."""
+        return len(self.color_stops)
+
     def __setattr__(self, _name: str, _value: Any) -> None:
         if getattr(self, "_initialized", False):
             raise AttributeError("Colormap is immutable")
         object.__setattr__(self, _name, _value)
 
     def __reduce__(self) -> str | tuple[Any, ...]:
         # for pickle
@@ -533,15 +600,15 @@
             and self.bad_color == other.bad_color
             and self.interpolation == other.interpolation
         )
 
     # -------------------------- reprs ----------------------------------
 
     def __repr__(self) -> str:
-        return f"Colormap(name={self.name!r}, <{len(self.color_stops)} colors>)"
+        return f"Colormap(name={self.name!r}, <{self.num_colors} colors>)"
 
     def _repr_png_(
         self, *, width: int = 512, height: int = 48, img: np.ndarray | None = None
     ) -> bytes:
         """Generate a PNG representation of the Colormap."""
         from ._png import encode_png
 
@@ -691,15 +758,18 @@
 
     def to_pyqtgraph(self) -> pyqtgraph.ColorMap:
         """Return a `pyqtgraph.ColorMap`."""
         return _external.to_pyqtgraph(self)
 
 
 class ColorStop(NamedTuple):
-    """A color stop in a color gradient."""
+    """A color stop in a color gradient.
+
+    Just a named tuple with a `position` (`float`) and a `color` (`cmap.Color`).
+    """
 
     position: float
     color: Color
 
 
 def _norm_interp(interp: Interpolation | bool | str | None) -> Interpolation:
     if isinstance(interp, bool):
@@ -785,16 +855,23 @@
             raise ValueError("lut_func must return RGB or RGBA values")
         return cast("np.ndarray", colors)
 
     @classmethod
     def parse(cls, colors: ColorStopsLike) -> ColorStops:
         """Parse any colorstops-like object into a ColorStops object.
 
-        This is the more flexible constructor.
-        see `_parse_colorstops` docstring for details.
+        Each item in `colors` can be a color, or a 2-tuple of (position, color), where
+        position (the "stop" along a color gradient) is a float between 0 and 1.  Where
+        not provided, color positions will be evenly distributed between neighboring
+        specified positions (if `fill_mode` is 'neighboring') or will be replaced with
+        `index / (len(colors)-1)` (if `fill_mode` is 'fractional').
+
+        Colors can be expressed as anything that can be converted to a Color, including
+        a string, or 3/4-sequence of RGB(A) values.
+
 
         Parameters
         ----------
         colors : str | Iterable[Any]
             Colors and (optional) stop positions.
 
         Returns
```

### Comparing `cmap-0.2.0/src/cmap/_external.py` & `cmap-0.2.1/src/cmap/_external.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,17 @@
                 raise ValueError(
                     "matplotlib 3.8.0 has a bug that prevents creating a colormap "
                     "from only two colors.  Please upgrade or downgrade matplotlib."
                 ) from e
             raise
 
     return mpl_cm.with_extremes(
-        bad=cm.bad_color,  # type: ignore
-        over=cm.over_color,  # type: ignore
-        under=cm.under_color,  # type: ignore
+        bad=cm.bad_color,
+        over=cm.over_color,
+        under=cm.under_color,
     )
 
 
 def to_vispy(cm: Colormap) -> VispyColormap:
     """Return a vispy colormap."""
     from vispy.color import Colormap
```

### Comparing `cmap-0.2.0/src/cmap/_png.py` & `cmap-0.2.1/src/cmap/_png.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/_util.py` & `cmap-0.2.1/src/cmap/_util.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/bids/__init__.py` & `cmap-0.2.1/src/cmap/data/bids/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/bids/record.json` & `cmap-0.2.1/src/cmap/data/bids/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/chrisluts/record.json` & `cmap-0.2.1/src/cmap/data/chrisluts/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cividis/__init__.py` & `cmap-0.2.1/src/cmap/data/cividis/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cividis/record.json` & `cmap-0.2.1/src/cmap/data/cividis/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmap/record.json` & `cmap-0.2.1/src/cmap/data/cmap/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/algae.py` & `cmap-0.2.1/src/cmap/data/cmocean/algae.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/amp.py` & `cmap-0.2.1/src/cmap/data/cmocean/amp.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/balance.py` & `cmap-0.2.1/src/cmap/data/cmocean/balance.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/curl.py` & `cmap-0.2.1/src/cmap/data/cmocean/curl.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/deep.py` & `cmap-0.2.1/src/cmap/data/cmocean/deep.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/delta.py` & `cmap-0.2.1/src/cmap/data/cmocean/delta.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/dense.py` & `cmap-0.2.1/src/cmap/data/cmocean/dense.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/diff.py` & `cmap-0.2.1/src/cmap/data/cmocean/diff.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/haline.py` & `cmap-0.2.1/src/cmap/data/cmocean/haline.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/ice.py` & `cmap-0.2.1/src/cmap/data/cmocean/ice.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/matter.py` & `cmap-0.2.1/src/cmap/data/cmocean/matter.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/oxy.py` & `cmap-0.2.1/src/cmap/data/cmocean/oxy.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/phase.py` & `cmap-0.2.1/src/cmap/data/cmocean/phase.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/rain.py` & `cmap-0.2.1/src/cmap/data/cmocean/rain.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/record.json` & `cmap-0.2.1/src/cmap/data/cmocean/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/solar.py` & `cmap-0.2.1/src/cmap/data/cmocean/solar.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/speed.py` & `cmap-0.2.1/src/cmap/data/cmocean/speed.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/tarn.py` & `cmap-0.2.1/src/cmap/data/cmocean/tarn.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/tempo.py` & `cmap-0.2.1/src/cmap/data/cmocean/tempo.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/thermal.py` & `cmap-0.2.1/src/cmap/data/cmocean/thermal.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/topo.py` & `cmap-0.2.1/src/cmap/data/cmocean/topo.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cmocean/turbid.py` & `cmap-0.2.1/src/cmap/data/cmocean/turbid.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorbrewer/__init__.py` & `cmap-0.2.1/src/cmap/data/colorbrewer/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorbrewer/record.json` & `cmap-0.2.1/src/cmap/data/colorbrewer/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_C1.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_C1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_C10.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_C10.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_C11.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_C11.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_C2.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_C2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_C3.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_C3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_C4.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_C4.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_C5.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_C5.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_C6.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_C6.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_C7.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_C7.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_C8.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_C8.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_C9.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_C9.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_CBC1.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_CBC1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_CBC2.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_CBC2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_CBD1.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_CBD1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_CBD2.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_CBD2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_CBL1.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_CBL1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_CBL2.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_CBL2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_CBL3.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_CBL3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_CBL4.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_CBL4.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_CBTC1.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_CBTC1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_CBTC2.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_CBTC2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_CBTD1.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_CBTD1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_CBTL1.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_CBTL1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_CBTL2.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_CBTL2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_CBTL3.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_CBTL3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_CBTL4.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_CBTL4.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_D1.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_D1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_D10.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_D10.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_D11.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_D11.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_D12.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_D12.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_D13.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_D13.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_D1A.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_D1A.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_D2.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_D2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_D3.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_D3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_D4.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_D4.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_D5.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_D5.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_D6.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_D6.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_D7.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_D7.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_D8.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_D8.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_D9.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_D9.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_I1.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_I1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_I2.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_I2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_I3.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_I3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_L1.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_L1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_L10.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_L10.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_L11.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_L11.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_L12.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_L12.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_L13.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_L13.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_L14.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_L14.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_L15.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_L15.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_L16.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_L16.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_L17.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_L17.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_L18.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_L18.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_L19.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_L19.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_L2.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_L2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_L20.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_L20.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_L3.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_L3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_L4.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_L4.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_L5.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_L5.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_L6.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_L6.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_L7.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_L7.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_L8.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_L8.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_L9.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_L9.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_R1.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_R1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_R2.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_R2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_R3.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_R3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/CET_R4.py` & `cmap-0.2.1/src/cmap/data/colorcet/CET_R4.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/__init__.py` & `cmap-0.2.1/src/cmap/data/colorcet/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/colorcet/record.json` & `cmap-0.2.1/src/cmap/data/colorcet/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/acton.py` & `cmap-0.2.1/src/cmap/data/crameri/acton.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/bam.py` & `cmap-0.2.1/src/cmap/data/crameri/bam.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/bamO.py` & `cmap-0.2.1/src/cmap/data/crameri/bamO.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/bamako.py` & `cmap-0.2.1/src/cmap/data/crameri/bamako.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/batlow.py` & `cmap-0.2.1/src/cmap/data/crameri/batlow.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/batlowK.py` & `cmap-0.2.1/src/cmap/data/crameri/batlowK.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/batlowW.py` & `cmap-0.2.1/src/cmap/data/crameri/batlowW.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/berlin.py` & `cmap-0.2.1/src/cmap/data/crameri/berlin.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/bilbao.py` & `cmap-0.2.1/src/cmap/data/crameri/bilbao.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/broc.py` & `cmap-0.2.1/src/cmap/data/crameri/broc.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/brocO.py` & `cmap-0.2.1/src/cmap/data/crameri/brocO.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/buda.py` & `cmap-0.2.1/src/cmap/data/crameri/buda.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/bukavu.py` & `cmap-0.2.1/src/cmap/data/crameri/bukavu.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/cork.py` & `cmap-0.2.1/src/cmap/data/crameri/cork.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/corkO.py` & `cmap-0.2.1/src/cmap/data/crameri/corkO.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/davos.py` & `cmap-0.2.1/src/cmap/data/crameri/davos.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/devon.py` & `cmap-0.2.1/src/cmap/data/crameri/devon.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/fes.py` & `cmap-0.2.1/src/cmap/data/crameri/fes.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/grayC.py` & `cmap-0.2.1/src/cmap/data/crameri/grayC.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/hawaii.py` & `cmap-0.2.1/src/cmap/data/crameri/hawaii.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/imola.py` & `cmap-0.2.1/src/cmap/data/crameri/imola.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/lajolla.py` & `cmap-0.2.1/src/cmap/data/crameri/lajolla.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/lapaz.py` & `cmap-0.2.1/src/cmap/data/crameri/lapaz.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/lisbon.py` & `cmap-0.2.1/src/cmap/data/crameri/lisbon.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/nuuk.py` & `cmap-0.2.1/src/cmap/data/crameri/nuuk.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/oleron.py` & `cmap-0.2.1/src/cmap/data/crameri/oleron.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/oslo.py` & `cmap-0.2.1/src/cmap/data/crameri/oslo.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/record.json` & `cmap-0.2.1/src/cmap/data/crameri/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/roma.py` & `cmap-0.2.1/src/cmap/data/crameri/roma.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/romaO.py` & `cmap-0.2.1/src/cmap/data/crameri/romaO.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/tofino.py` & `cmap-0.2.1/src/cmap/data/crameri/tofino.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/tokyo.py` & `cmap-0.2.1/src/cmap/data/crameri/tokyo.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/turku.py` & `cmap-0.2.1/src/cmap/data/crameri/turku.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/vanimo.py` & `cmap-0.2.1/src/cmap/data/crameri/vanimo.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/vik.py` & `cmap-0.2.1/src/cmap/data/crameri/vik.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/crameri/vikO.py` & `cmap-0.2.1/src/cmap/data/crameri/vikO.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/cubehelix/__init__.py` & `cmap-0.2.1/src/cmap/data/cubehelix/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/glasbey/__init__.py` & `cmap-0.2.1/src/cmap/data/glasbey/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/glasbey/_glasbey.py` & `cmap-0.2.1/src/cmap/data/glasbey/_glasbey.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/glasbey/_grids.py` & `cmap-0.2.1/src/cmap/data/glasbey/_grids.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/glasbey/_internals.py` & `cmap-0.2.1/src/cmap/data/glasbey/_internals.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/glasbey/prebuilt.py` & `cmap-0.2.1/src/cmap/data/glasbey/prebuilt.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/gnuplot/__init__.py` & `cmap-0.2.1/src/cmap/data/gnuplot/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/gnuplot/record.json` & `cmap-0.2.1/src/cmap/data/gnuplot/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/google/__init__.py` & `cmap-0.2.1/src/cmap/data/google/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/google/record.json` & `cmap-0.2.1/src/cmap/data/google/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/imagej/__init__.py` & `cmap-0.2.1/src/cmap/data/imagej/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/imagej/record.json` & `cmap-0.2.1/src/cmap/data/imagej/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/matlab/__init__.py` & `cmap-0.2.1/src/cmap/data/matlab/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/matlab/record.json` & `cmap-0.2.1/src/cmap/data/matlab/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/matplotlib/_CMRmap.py` & `cmap-0.2.1/src/cmap/data/matplotlib/_CMRmap.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/matplotlib/__init__.py` & `cmap-0.2.1/src/cmap/data/matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/matplotlib/_coolwarm.py` & `cmap-0.2.1/src/cmap/data/matplotlib/_coolwarm.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/matplotlib/_wistia.py` & `cmap-0.2.1/src/cmap/data/matplotlib/_wistia.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/matplotlib/record.json` & `cmap-0.2.1/src/cmap/data/matplotlib/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/seaborn/__init__.py` & `cmap-0.2.1/src/cmap/data/seaborn/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/seaborn/record.json` & `cmap-0.2.1/src/cmap/data/seaborn/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/tableau/__init__.py` & `cmap-0.2.1/src/cmap/data/tableau/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/tableau/record.json` & `cmap-0.2.1/src/cmap/data/tableau/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/tol/__init__.py` & `cmap-0.2.1/src/cmap/data/tol/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/tol/record.json` & `cmap-0.2.1/src/cmap/data/tol/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/vispy/__init__.py` & `cmap-0.2.1/src/cmap/data/vispy/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/vispy/record.json` & `cmap-0.2.1/src/cmap/data/vispy/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/yorick/__init__.py` & `cmap-0.2.1/src/cmap/data/yorick/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/src/cmap/data/yorick/record.json` & `cmap-0.2.1/src/cmap/data/yorick/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/tests/test_catalog.py` & `cmap-0.2.1/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/tests/test_color.py` & `cmap-0.2.1/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/tests/test_colormap.py` & `cmap-0.2.1/tests/test_colormap.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/tests/test_data.py` & `cmap-0.2.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/tests/test_glasbey.py` & `cmap-0.2.1/tests/test_glasbey.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/tests/test_model_fields.py` & `cmap-0.2.1/tests/test_model_fields.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/tests/test_third_party.py` & `cmap-0.2.1/tests/test_third_party.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/tests/test_utils.py` & `cmap-0.2.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/.gitignore` & `cmap-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/README.md` & `cmap-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/pyproject.toml` & `cmap-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/LICENSE/LICENSE` & `cmap-0.2.1/LICENSE/LICENSE`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/LICENSE/LICENSE_CMOCEAN` & `cmap-0.2.1/LICENSE/LICENSE_CMOCEAN`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/LICENSE/LICENSE_COLORBREWER` & `cmap-0.2.1/LICENSE/LICENSE_COLORBREWER`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/LICENSE/LICENSE_CRAMERI` & `cmap-0.2.1/LICENSE/LICENSE_CRAMERI`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/LICENSE/LICENSE_CVIDIS` & `cmap-0.2.1/LICENSE/LICENSE_CVIDIS`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/LICENSE/LICENSE_GLASBEY` & `cmap-0.2.1/LICENSE/LICENSE_GLASBEY`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/LICENSE/LICENSE_TOL` & `cmap-0.2.1/LICENSE/LICENSE_TOL`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/LICENSE/LICENSE_WISTIA` & `cmap-0.2.1/LICENSE/LICENSE_WISTIA`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/LICENSE/LICENSE_YORICK` & `cmap-0.2.1/LICENSE/LICENSE_YORICK`

 * *Files identical despite different names*

### Comparing `cmap-0.2.0/PKG-INFO` & `cmap-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cmap
-Version: 0.2.0
+Version: 0.2.1
 Summary: Scientific colormaps for python, without dependencies
 Project-URL: Homepage, https://github.com/tlambert03/cmap
 Project-URL: Repository, https://github.com/tlambert03/cmap
 Project-URL: Bug Tracker, https://github.com/tlambert03/cmap/issues
 Project-URL: Documentation, https://cmap-docs.rtfd.io/
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
```

