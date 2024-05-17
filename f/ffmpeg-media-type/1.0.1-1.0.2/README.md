# Comparing `tmp/ffmpeg_media_type-1.0.1.tar.gz` & `tmp/ffmpeg_media_type-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg_media_type-1.0.1.tar", max compression
+gzip compressed data, was "ffmpeg_media_type-1.0.2.tar", max compression
```

## Comparing `ffmpeg_media_type-1.0.1.tar` & `ffmpeg_media_type-1.0.2.tar`

### file list

```diff
@@ -1,424 +1,424 @@
--rw-r--r--   0        0        0     1066 2024-04-19 08:34:42.533021 ffmpeg_media_type-1.0.1/LICENSE
--rw-r--r--   0        0        0     6131 2024-04-19 08:34:42.537021 ffmpeg_media_type-1.0.1/README.md
--rw-r--r--   0        0        0     1889 2024-04-19 08:34:58.013232 ffmpeg_media_type-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      234 2024-04-19 08:34:42.537021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/__init__.py
--rw-r--r--   0        0        0      192 2024-04-19 08:34:42.537021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/3dostr.json
--rw-r--r--   0        0        0      216 2024-04-19 08:34:42.537021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/3g2.json
--rw-r--r--   0        0        0      214 2024-04-19 08:34:42.537021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/3gp.json
--rw-r--r--   0        0        0      192 2024-04-19 08:34:42.537021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/4xm.json
--rw-r--r--   0        0        0      214 2024-04-19 08:34:42.537021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/a64.json
--rw-r--r--   0        0        0      203 2024-04-19 08:34:42.537021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/aa.json
--rw-r--r--   0        0        0      218 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/aac.json
--rw-r--r--   0        0        0      189 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/aax.json
--rw-r--r--   0        0        0      203 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ac3.json
--rw-r--r--   0        0        0      201 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ac4.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ace.json
--rw-r--r--   0        0        0      195 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/acm.json
--rw-r--r--   0        0        0      198 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/act.json
--rw-r--r--   0        0        0      201 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/adf.json
--rw-r--r--   0        0        0      192 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/adp.json
--rw-r--r--   0        0        0      201 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ads.json
--rw-r--r--   0        0        0      235 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/adts.json
--rw-r--r--   0        0        0      197 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/adx.json
--rw-r--r--   0        0        0      197 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/aea.json
--rw-r--r--   0        0        0      185 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/afc.json
--rw-r--r--   0        0        0      236 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/aiff.json
--rw-r--r--   0        0        0      189 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/aix.json
--rw-r--r--   0        0        0      198 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/alaw.json
--rw-r--r--   0        0        0      208 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/alias_pix.json
--rw-r--r--   0        0        0      216 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/alp.json
--rw-r--r--   0        0        0      204 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/amr.json
--rw-r--r--   0        0        0      189 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/amrnb.json
--rw-r--r--   0        0        0      189 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/amrwb.json
--rw-r--r--   0        0        0      210 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/amv.json
--rw-r--r--   0        0        0      199 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/anm.json
--rw-r--r--   0        0        0      191 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/apac.json
--rw-r--r--   0        0        0      185 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/apc.json
--rw-r--r--   0        0        0      210 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ape.json
--rw-r--r--   0        0        0      214 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/apm.json
--rw-r--r--   0        0        0      230 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/apng.json
--rw-r--r--   0        0        0      239 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/aptx.json
--rw-r--r--   0        0        0      250 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/aptx_hd.json
--rw-r--r--   0        0        0      203 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/aqtitle.json
--rw-r--r--   0        0        0      209 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/argo_asf.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/argo_brp.json
--rw-r--r--   0        0        0      213 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/argo_cvg.json
--rw-r--r--   0        0        0      263 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/asf.json
--rw-r--r--   0        0        0      219 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/asf_o.json
--rw-r--r--   0        0        0      271 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/asf_stream.json
--rw-r--r--   0        0        0      229 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ass.json
--rw-r--r--   0        0        0      215 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ast.json
--rw-r--r--   0        0        0      205 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/au.json
--rw-r--r--   0        0        0      221 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/audiotoolbox.json
--rw-r--r--   0        0        0      193 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/av1.json
--rw-r--r--   0        0        0      211 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/avfoundation.json
--rw-r--r--   0        0        0      233 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/avi.json
--rw-r--r--   0        0        0      201 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/avif.json
--rw-r--r--   0        0        0      242 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/avm2.json
--rw-r--r--   0        0        0      209 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/avr.json
--rw-r--r--   0        0        0      206 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/avs.json
--rw-r--r--   0        0        0      222 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/avs2.json
--rw-r--r--   0        0        0      206 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/avs3.json
--rw-r--r--   0        0        0      207 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/bethsoftvid.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/bfi.json
--rw-r--r--   0        0        0      221 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/bfstm.json
--rw-r--r--   0        0        0      188 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/bin.json
--rw-r--r--   0        0        0      182 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/bink.json
--rw-r--r--   0        0        0      196 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/binka.json
--rw-r--r--   0        0        0      215 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/bit.json
--rw-r--r--   0        0        0      203 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/bitpacked.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/bmp_pipe.json
--rw-r--r--   0        0        0      198 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/bmv.json
--rw-r--r--   0        0        0      192 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/boa.json
--rw-r--r--   0        0        0      192 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/bonk.json
--rw-r--r--   0        0        0      202 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/brender_pix.json
--rw-r--r--   0        0        0      218 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/brstm.json
--rw-r--r--   0        0        0      190 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/c93.json
--rw-r--r--   0        0        0      230 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/caf.json
--rw-r--r--   0        0        0      235 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/cavsvideo.json
--rw-r--r--   0        0        0      193 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/cdg.json
--rw-r--r--   0        0        0      210 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/cdxl.json
--rw-r--r--   0        0        0      190 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/cine.json
--rw-r--r--   0        0        0      205 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/codec2.json
--rw-r--r--   0        0        0      204 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/codec2raw.json
--rw-r--r--   0        0        0      208 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/concat.json
--rw-r--r--   0        0        0      205 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/crc.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/cri_pipe.json
--rw-r--r--   0        0        0      199 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/dash.json
--rw-r--r--   0        0        0      185 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/data.json
--rw-r--r--   0        0        0      215 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/daud.json
--rw-r--r--   0        0        0      195 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/dcstr.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/dds_pipe.json
--rw-r--r--   0        0        0      193 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/derf.json
--rw-r--r--   0        0        0      193 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/dfa.json
--rw-r--r--   0        0        0      201 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/dfpwm.json
--rw-r--r--   0        0        0      192 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/dhav.json
--rw-r--r--   0        0        0      204 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/dirac.json
--rw-r--r--   0        0        0      221 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/dnxhd.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/dpx_pipe.json
--rw-r--r--   0        0        0      198 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/dsf.json
--rw-r--r--   0        0        0      215 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/dsicin.json
--rw-r--r--   0        0        0      211 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/dss.json
--rw-r--r--   0        0        0      202 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/dts.json
--rw-r--r--   0        0        0      196 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/dtshd.json
--rw-r--r--   0        0        0      220 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/dv.json
--rw-r--r--   0        0        0      190 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/dvbsub.json
--rw-r--r--   0        0        0      186 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/dvbtxt.json
--rw-r--r--   0        0        0      224 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/dvd.json
--rw-r--r--   0        0        0      180 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/dxa.json
--rw-r--r--   0        0        0      202 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ea.json
--rw-r--r--   0        0        0      210 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ea_cdata.json
--rw-r--r--   0        0        0      216 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/eac3.json
--rw-r--r--   0        0        0      214 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/epaf.json
--rw-r--r--   0        0        0      197 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/evc.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/exr_pipe.json
--rw-r--r--   0        0        0      223 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/f32be.json
--rw-r--r--   0        0        0      226 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/f32le.json
--rw-r--r--   0        0        0      225 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/f4v.json
--rw-r--r--   0        0        0      223 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/f64be.json
--rw-r--r--   0        0        0      226 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/f64le.json
--rw-r--r--   0        0        0      214 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ffmetadata.json
--rw-r--r--   0        0        0      201 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/fifo.json
--rw-r--r--   0        0        0      198 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/fifo_test.json
--rw-r--r--   0        0        0      224 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/film_cpk.json
--rw-r--r--   0        0        0      210 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/filmstrip.json
--rw-r--r--   0        0        0      218 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/fits.json
--rw-r--r--   0        0        0      210 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/flac.json
--rw-r--r--   0        0        0      199 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/flic.json
--rw-r--r--   0        0        0      216 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/flv.json
--rw-r--r--   0        0        0      215 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/framecrc.json
--rw-r--r--   0        0        0      222 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/framehash.json
--rw-r--r--   0        0        0      220 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/framemd5.json
--rw-r--r--   0        0        0      190 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/frm.json
--rw-r--r--   0        0        0      198 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/fsb.json
--rw-r--r--   0        0        0      211 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/fwse.json
--rw-r--r--   0        0        0      219 2024-04-19 08:34:42.541021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/g722.json
--rw-r--r--   0        0        0      228 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/g723_1.json
--rw-r--r--   0        0        0      228 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/g726.json
--rw-r--r--   0        0        0      236 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/g726le.json
--rw-r--r--   0        0        0      208 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/g729.json
--rw-r--r--   0        0        0      198 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/gdv.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/gem_pipe.json
--rw-r--r--   0        0        0      198 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/genh.json
--rw-r--r--   0        0        0      237 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/gif.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/gif_pipe.json
--rw-r--r--   0        0        0      202 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/gsm.json
--rw-r--r--   0        0        0      229 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/gxf.json
--rw-r--r--   0        0        0      208 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/h261.json
--rw-r--r--   0        0        0      208 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/h263.json
--rw-r--r--   0        0        0      224 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/h264.json
--rw-r--r--   0        0        0      207 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/hash.json
--rw-r--r--   0        0        0      189 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/hca.json
--rw-r--r--   0        0        0      192 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/hcom.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/hdr_pipe.json
--rw-r--r--   0        0        0      193 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/hds.json
--rw-r--r--   0        0        0      216 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/hevc.json
--rw-r--r--   0        0        0      214 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/hls.json
--rw-r--r--   0        0        0      188 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/hnm.json
--rw-r--r--   0        0        0      214 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ico.json
--rw-r--r--   0        0        0      191 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/idcin.json
--rw-r--r--   0        0        0      195 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/idf.json
--rw-r--r--   0        0        0      206 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/iff.json
--rw-r--r--   0        0        0      194 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ifv.json
--rw-r--r--   0        0        0      208 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ilbc.json
--rw-r--r--   0        0        0      495 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/image2.json
--rw-r--r--   0        0        0      209 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/image2pipe.json
--rw-r--r--   0        0        0      210 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/imf.json
--rw-r--r--   0        0        0      207 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ingenient.json
--rw-r--r--   0        0        0      194 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ipmovie.json
--rw-r--r--   0        0        0      244 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ipod.json
--rw-r--r--   0        0        0      195 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ipu.json
--rw-r--r--   0        0        0      232 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ircam.json
--rw-r--r--   0        0        0      236 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ismv.json
--rw-r--r--   0        0        0      187 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/iss.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/iv8.json
--rw-r--r--   0        0        0      191 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ivf.json
--rw-r--r--   0        0        0      212 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ivr.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/j2k_pipe.json
--rw-r--r--   0        0        0      228 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/jacosub.json
--rw-r--r--   0        0        0      202 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/jpeg_pipe.json
--rw-r--r--   0        0        0      206 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/jpegls_pipe.json
--rw-r--r--   0        0        0      206 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/jpegxl_anim.json
--rw-r--r--   0        0        0      206 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/jpegxl_pipe.json
--rw-r--r--   0        0        0      194 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/jv.json
--rw-r--r--   0        0        0      193 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/kux.json
--rw-r--r--   0        0        0      227 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/kvag.json
--rw-r--r--   0        0        0      210 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/laf.json
--rw-r--r--   0        0        0      219 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/latm.json
--rw-r--r--   0        0        0      211 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/lavfi.json
--rw-r--r--   0        0        0      214 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/live_flv.json
--rw-r--r--   0        0        0      188 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/lmlm4.json
--rw-r--r--   0        0        0      198 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/loas.json
--rw-r--r--   0        0        0      191 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/lrc.json
--rw-r--r--   0        0        0      199 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/luodat.json
--rw-r--r--   0        0        0      185 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/lvf.json
--rw-r--r--   0        0        0      199 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/lxf.json
--rw-r--r--   0        0        0      202 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/m4v.json
--rw-r--r--   0        0        0      237 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/matroska,webm.json
--rw-r--r--   0        0        0      221 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/matroska.json
--rw-r--r--   0        0        0      198 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mca.json
--rw-r--r--   0        0        0      192 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mcc.json
--rw-r--r--   0        0        0      205 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/md5.json
--rw-r--r--   0        0        0      212 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mgsts.json
--rw-r--r--   0        0        0      225 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/microdvd.json
--rw-r--r--   0        0        0      233 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mjpeg.json
--rw-r--r--   0        0        0      209 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mjpeg_2000.json
--rw-r--r--   0        0        0      256 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mkvtimestamp_v2.json
--rw-r--r--   0        0        0      191 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mlp.json
--rw-r--r--   0        0        0      202 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mlv.json
--rw-r--r--   0        0        0      199 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mm.json
--rw-r--r--   0        0        0      219 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mmf.json
--rw-r--r--   0        0        0      197 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mods.json
--rw-r--r--   0        0        0      203 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/moflex.json
--rw-r--r--   0        0        0      304 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mov,mp4,m4a,3gp,3g2,mj2.json
--rw-r--r--   0        0        0      204 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mov.json
--rw-r--r--   0        0        0      233 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mp2.json
--rw-r--r--   0        0        0      242 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mp3.json
--rw-r--r--   0        0        0      218 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mp4.json
--rw-r--r--   0        0        0      190 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mpc.json
--rw-r--r--   0        0        0      190 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mpc8.json
--rw-r--r--   0        0        0      249 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mpeg.json
--rw-r--r--   0        0        0      240 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mpeg1video.json
--rw-r--r--   0        0        0      215 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mpeg2video.json
--rw-r--r--   0        0        0      261 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mpegts.json
--rw-r--r--   0        0        0      220 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mpegtsraw.json
--rw-r--r--   0        0        0      197 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mpegvideo.json
--rw-r--r--   0        0        0      234 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mpjpeg.json
--rw-r--r--   0        0        0      205 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mpl2.json
--rw-r--r--   0        0        0      201 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mpsub.json
--rw-r--r--   0        0        0      194 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/msf.json
--rw-r--r--   0        0        0      203 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/msnwctcp.json
--rw-r--r--   0        0        0      199 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/msp.json
--rw-r--r--   0        0        0      199 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mtaf.json
--rw-r--r--   0        0        0      180 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mtv.json
--rw-r--r--   0        0        0      201 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mulaw.json
--rw-r--r--   0        0        0      196 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/musx.json
--rw-r--r--   0        0        0      198 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mv.json
--rw-r--r--   0        0        0      199 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mvi.json
--rw-r--r--   0        0        0      245 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mxf.json
--rw-r--r--   0        0        0      258 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mxf_d10.json
--rw-r--r--   0        0        0      273 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mxf_opatom.json
--rw-r--r--   0        0        0      192 2024-04-19 08:34:42.545021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/mxg.json
--rw-r--r--   0        0        0      193 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/nc.json
--rw-r--r--   0        0        0      225 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/nistsphere.json
--rw-r--r--   0        0        0      209 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/nsp.json
--rw-r--r--   0        0        0      201 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/nsv.json
--rw-r--r--   0        0        0      216 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/null.json
--rw-r--r--   0        0        0      206 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/nut.json
--rw-r--r--   0        0        0      188 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/nuv.json
--rw-r--r--   0        0        0      204 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/obu.json
--rw-r--r--   0        0        0      204 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/oga.json
--rw-r--r--   0        0        0      211 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ogg.json
--rw-r--r--   0        0        0      212 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ogv.json
--rw-r--r--   0        0        0      229 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/oma.json
--rw-r--r--   0        0        0      205 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/opus.json
--rw-r--r--   0        0        0      189 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/osq.json
--rw-r--r--   0        0        0      213 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/paf.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/pam_pipe.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/pbm_pipe.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/pcx_pipe.json
--rw-r--r--   0        0        0      196 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/pdv.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/pfm_pipe.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/pgm_pipe.json
--rw-r--r--   0        0        0      206 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/pgmyuv_pipe.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/pgx_pipe.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/phm_pipe.json
--rw-r--r--   0        0        0      208 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/photocd_pipe.json
--rw-r--r--   0        0        0      206 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/pictor_pipe.json
--rw-r--r--   0        0        0      226 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/pjs.json
--rw-r--r--   0        0        0      201 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/pmp.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/png_pipe.json
--rw-r--r--   0        0        0      208 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/pp_bnk.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ppm_pipe.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/psd_pipe.json
--rw-r--r--   0        0        0      220 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/psp.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/psxstr.json
--rw-r--r--   0        0        0      192 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/pva.json
--rw-r--r--   0        0        0      209 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/pvf.json
--rw-r--r--   0        0        0      180 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/qcp.json
--rw-r--r--   0        0        0      204 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/qdraw_pipe.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/qoi_pipe.json
--rw-r--r--   0        0        0      188 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/r3d.json
--rw-r--r--   0        0        0      225 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/rawvideo.json
--rw-r--r--   0        0        0      210 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/realtext.json
--rw-r--r--   0        0        0      195 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/redspark.json
--rw-r--r--   0        0        0      196 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/rka.json
--rw-r--r--   0        0        0      180 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/rl2.json
--rw-r--r--   0        0        0      216 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/rm.json
--rw-r--r--   0        0        0      202 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/roq.json
--rw-r--r--   0        0        0      190 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/rpl.json
--rw-r--r--   0        0        0      194 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/rsd.json
--rw-r--r--   0        0        0      206 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/rso.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/rtp.json
--rw-r--r--   0        0        0      216 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/rtp_mpegts.json
--rw-r--r--   0        0        0      196 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/rtsp.json
--rw-r--r--   0        0        0      215 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/s16be.json
--rw-r--r--   0        0        0      222 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/s16le.json
--rw-r--r--   0        0        0      215 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/s24be.json
--rw-r--r--   0        0        0      218 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/s24le.json
--rw-r--r--   0        0        0      215 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/s32be.json
--rw-r--r--   0        0        0      218 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/s32le.json
--rw-r--r--   0        0        0      189 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/s337m.json
--rw-r--r--   0        0        0      201 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/s8.json
--rw-r--r--   0        0        0      211 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/sami.json
--rw-r--r--   0        0        0      194 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/sap.json
--rw-r--r--   0        0        0      210 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/sbc.json
--rw-r--r--   0        0        0      210 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/sbg.json
--rw-r--r--   0        0        0      206 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/scc.json
--rw-r--r--   0        0        0      192 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/scd.json
--rw-r--r--   0        0        0      208 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/sdl,sdl2.json
--rw-r--r--   0        0        0      193 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/sdns.json
--rw-r--r--   0        0        0      180 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/sdp.json
--rw-r--r--   0        0        0      188 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/sdr2.json
--rw-r--r--   0        0        0      207 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/sds.json
--rw-r--r--   0        0        0      202 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/sdx.json
--rw-r--r--   0        0        0      188 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/segment.json
--rw-r--r--   0        0        0      247 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ser.json
--rw-r--r--   0        0        0      202 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/sga.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/sgi_pipe.json
--rw-r--r--   0        0        0      193 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/shn.json
--rw-r--r--   0        0        0      207 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/siff.json
--rw-r--r--   0        0        0      217 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/simbiosis_imx.json
--rw-r--r--   0        0        0      198 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/sln.json
--rw-r--r--   0        0        0      213 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/smjpeg.json
--rw-r--r--   0        0        0      184 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/smk.json
--rw-r--r--   0        0        0      218 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/smoothstreaming.json
--rw-r--r--   0        0        0      194 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/smush.json
--rw-r--r--   0        0        0      187 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/sol.json
--rw-r--r--   0        0        0      217 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/sox.json
--rw-r--r--   0        0        0      223 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/spdif.json
--rw-r--r--   0        0        0      205 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/spx.json
--rw-r--r--   0        0        0      216 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/srt.json
--rw-r--r--   0        0        0      204 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/stl.json
--rw-r--r--   0        0        0      220 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/stream_segment,ssegment.json
--rw-r--r--   0        0        0      224 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/streamhash.json
--rw-r--r--   0        0        0      213 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/subviewer.json
--rw-r--r--   0        0        0      217 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/subviewer1.json
--rw-r--r--   0        0        0      208 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/sunrast_pipe.json
--rw-r--r--   0        0        0      244 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/sup.json
--rw-r--r--   0        0        0      199 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/svag.json
--rw-r--r--   0        0        0      222 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/svcd.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/svg_pipe.json
--rw-r--r--   0        0        0      192 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/svs.json
--rw-r--r--   0        0        0      238 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/swf.json
--rw-r--r--   0        0        0      189 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/tak.json
--rw-r--r--   0        0        0      203 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/tedcaptions.json
--rw-r--r--   0        0        0      195 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/tee.json
--rw-r--r--   0        0        0      180 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/thp.json
--rw-r--r--   0        0        0      203 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/tiertexseq.json
--rw-r--r--   0        0        0      202 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/tiff_pipe.json
--rw-r--r--   0        0        0      189 2024-04-19 08:34:42.549021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/tmv.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/truehd.json
--rw-r--r--   0        0        0      211 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/tta.json
--rw-r--r--   0        0        0      206 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ttml.json
--rw-r--r--   0        0        0      245 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/tty.json
--rw-r--r--   0        0        0      206 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/txd.json
--rw-r--r--   0        0        0      190 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/ty.json
--rw-r--r--   0        0        0      217 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/u16be.json
--rw-r--r--   0        0        0      224 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/u16le.json
--rw-r--r--   0        0        0      217 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/u24be.json
--rw-r--r--   0        0        0      220 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/u24le.json
--rw-r--r--   0        0        0      217 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/u32be.json
--rw-r--r--   0        0        0      220 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/u32le.json
--rw-r--r--   0        0        0      203 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/u8.json
--rw-r--r--   0        0        0      230 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/uncodedframecrc.json
--rw-r--r--   0        0        0      189 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/usm.json
--rw-r--r--   0        0        0      209 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/v210.json
--rw-r--r--   0        0        0      211 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/v210x.json
--rw-r--r--   0        0        0      194 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/vag.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/vbn_pipe.json
--rw-r--r--   0        0        0      198 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/vc1.json
--rw-r--r--   0        0        0      208 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/vc1test.json
--rw-r--r--   0        0        0      242 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/vcd.json
--rw-r--r--   0        0        0      204 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/vidc.json
--rw-r--r--   0        0        0      192 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/vividas.json
--rw-r--r--   0        0        0      187 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/vivo.json
--rw-r--r--   0        0        0      187 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/vmd.json
--rw-r--r--   0        0        0      220 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/vob.json
--rw-r--r--   0        0        0      207 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/vobsub.json
--rw-r--r--   0        0        0      215 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/voc.json
--rw-r--r--   0        0        0      194 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/vpk.json
--rw-r--r--   0        0        0      203 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/vplayer.json
--rw-r--r--   0        0        0      251 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/vqf.json
--rw-r--r--   0        0        0      218 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/vvc.json
--rw-r--r--   0        0        0      201 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/w64.json
--rw-r--r--   0        0        0      194 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/wady.json
--rw-r--r--   0        0        0      228 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/wav.json
--rw-r--r--   0        0        0      201 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/wavarc.json
--rw-r--r--   0        0        0      206 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/wc3movie.json
--rw-r--r--   0        0        0      205 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/webm.json
--rw-r--r--   0        0        0      215 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/webm_chunk.json
--rw-r--r--   0        0        0      229 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/webm_dash_manifest.json
--rw-r--r--   0        0        0      192 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/webp.json
--rw-r--r--   0        0        0      202 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/webp_pipe.json
--rw-r--r--   0        0        0      207 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/webvtt.json
--rw-r--r--   0        0        0      217 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/wsaud.json
--rw-r--r--   0        0        0      212 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/wsd.json
--rw-r--r--   0        0        0      199 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/wsvqa.json
--rw-r--r--   0        0        0      218 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/wtv.json
--rw-r--r--   0        0        0      212 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/wv.json
--rw-r--r--   0        0        0      190 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/wve.json
--rw-r--r--   0        0        0      210 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/x11grab.json
--rw-r--r--   0        0        0      184 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/xa.json
--rw-r--r--   0        0        0      205 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/xbin.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/xbm_pipe.json
--rw-r--r--   0        0        0      192 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/xmd.json
--rw-r--r--   0        0        0      195 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/xmv.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/xpm_pipe.json
--rw-r--r--   0        0        0      197 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/xvag.json
--rw-r--r--   0        0        0      200 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/xwd_pipe.json
--rw-r--r--   0        0        0      192 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/xwma.json
--rw-r--r--   0        0        0      195 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/yop.json
--rw-r--r--   0        0        0      218 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/cache/yuv4mpegpipe.json
--rw-r--r--   0        0        0      101 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/exceptions.py
--rw-r--r--   0        0        0     3412 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/info.py
--rw-r--r--   0        0        0        0 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/py.typed
--rw-r--r--   0        0        0     3387 2024-04-19 08:34:42.553021 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/schema.py
--rw-r--r--   0        0        0        0 2024-04-19 08:34:42.657022 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/utils/__init__.py
--rw-r--r--   0        0        0     1015 2024-04-19 08:34:42.657022 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/utils/cache.py
--rw-r--r--   0        0        0      909 2024-04-19 08:34:42.657022 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/utils/ffprobe.py
--rw-r--r--   0        0        0     4858 2024-04-19 08:34:42.657022 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/utils/hotfix_webp.py
--rw-r--r--   0        0        0     1008 2024-04-19 08:34:42.657022 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/utils/loader.py
--rw-r--r--   0        0        0     1130 2024-04-19 08:34:42.657022 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/utils/shell.py
--rw-r--r--   0        0        0     1275 2024-04-19 08:34:42.657022 ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/utils/thumbnail.py
--rw-r--r--   0        0        0     7093 1970-01-01 00:00:00.000000 ffmpeg_media_type-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-14 09:30:20.807381 ffmpeg_media_type-1.0.2/LICENSE
+-rw-r--r--   0        0        0     6131 2024-05-14 09:30:20.807381 ffmpeg_media_type-1.0.2/README.md
+-rw-r--r--   0        0        0     1893 2024-05-14 09:30:37.695446 ffmpeg_media_type-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      234 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/__init__.py
+-rw-r--r--   0        0        0      192 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/3dostr.json
+-rw-r--r--   0        0        0      216 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/3g2.json
+-rw-r--r--   0        0        0      214 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/3gp.json
+-rw-r--r--   0        0        0      192 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/4xm.json
+-rw-r--r--   0        0        0      214 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/a64.json
+-rw-r--r--   0        0        0      203 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/aa.json
+-rw-r--r--   0        0        0      218 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/aac.json
+-rw-r--r--   0        0        0      189 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/aax.json
+-rw-r--r--   0        0        0      203 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ac3.json
+-rw-r--r--   0        0        0      201 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ac4.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ace.json
+-rw-r--r--   0        0        0      195 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/acm.json
+-rw-r--r--   0        0        0      198 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/act.json
+-rw-r--r--   0        0        0      201 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/adf.json
+-rw-r--r--   0        0        0      192 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/adp.json
+-rw-r--r--   0        0        0      201 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ads.json
+-rw-r--r--   0        0        0      235 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/adts.json
+-rw-r--r--   0        0        0      197 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/adx.json
+-rw-r--r--   0        0        0      197 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/aea.json
+-rw-r--r--   0        0        0      185 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/afc.json
+-rw-r--r--   0        0        0      236 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/aiff.json
+-rw-r--r--   0        0        0      189 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/aix.json
+-rw-r--r--   0        0        0      198 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/alaw.json
+-rw-r--r--   0        0        0      208 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/alias_pix.json
+-rw-r--r--   0        0        0      216 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/alp.json
+-rw-r--r--   0        0        0      204 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/amr.json
+-rw-r--r--   0        0        0      189 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/amrnb.json
+-rw-r--r--   0        0        0      189 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/amrwb.json
+-rw-r--r--   0        0        0      210 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/amv.json
+-rw-r--r--   0        0        0      199 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/anm.json
+-rw-r--r--   0        0        0      191 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/apac.json
+-rw-r--r--   0        0        0      185 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/apc.json
+-rw-r--r--   0        0        0      210 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ape.json
+-rw-r--r--   0        0        0      214 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/apm.json
+-rw-r--r--   0        0        0      230 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/apng.json
+-rw-r--r--   0        0        0      239 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/aptx.json
+-rw-r--r--   0        0        0      250 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/aptx_hd.json
+-rw-r--r--   0        0        0      203 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/aqtitle.json
+-rw-r--r--   0        0        0      209 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/argo_asf.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/argo_brp.json
+-rw-r--r--   0        0        0      213 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/argo_cvg.json
+-rw-r--r--   0        0        0      263 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/asf.json
+-rw-r--r--   0        0        0      219 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/asf_o.json
+-rw-r--r--   0        0        0      271 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/asf_stream.json
+-rw-r--r--   0        0        0      229 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ass.json
+-rw-r--r--   0        0        0      215 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ast.json
+-rw-r--r--   0        0        0      205 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/au.json
+-rw-r--r--   0        0        0      221 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/audiotoolbox.json
+-rw-r--r--   0        0        0      193 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/av1.json
+-rw-r--r--   0        0        0      211 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/avfoundation.json
+-rw-r--r--   0        0        0      233 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/avi.json
+-rw-r--r--   0        0        0      201 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/avif.json
+-rw-r--r--   0        0        0      242 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/avm2.json
+-rw-r--r--   0        0        0      209 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/avr.json
+-rw-r--r--   0        0        0      206 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/avs.json
+-rw-r--r--   0        0        0      222 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/avs2.json
+-rw-r--r--   0        0        0      206 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/avs3.json
+-rw-r--r--   0        0        0      207 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/bethsoftvid.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/bfi.json
+-rw-r--r--   0        0        0      221 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/bfstm.json
+-rw-r--r--   0        0        0      188 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/bin.json
+-rw-r--r--   0        0        0      182 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/bink.json
+-rw-r--r--   0        0        0      196 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/binka.json
+-rw-r--r--   0        0        0      215 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/bit.json
+-rw-r--r--   0        0        0      203 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/bitpacked.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/bmp_pipe.json
+-rw-r--r--   0        0        0      198 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/bmv.json
+-rw-r--r--   0        0        0      192 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/boa.json
+-rw-r--r--   0        0        0      192 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/bonk.json
+-rw-r--r--   0        0        0      202 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/brender_pix.json
+-rw-r--r--   0        0        0      218 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/brstm.json
+-rw-r--r--   0        0        0      190 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/c93.json
+-rw-r--r--   0        0        0      230 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/caf.json
+-rw-r--r--   0        0        0      235 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/cavsvideo.json
+-rw-r--r--   0        0        0      193 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/cdg.json
+-rw-r--r--   0        0        0      210 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/cdxl.json
+-rw-r--r--   0        0        0      190 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/cine.json
+-rw-r--r--   0        0        0      205 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/codec2.json
+-rw-r--r--   0        0        0      204 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/codec2raw.json
+-rw-r--r--   0        0        0      208 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/concat.json
+-rw-r--r--   0        0        0      205 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/crc.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/cri_pipe.json
+-rw-r--r--   0        0        0      199 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/dash.json
+-rw-r--r--   0        0        0      185 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/data.json
+-rw-r--r--   0        0        0      215 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/daud.json
+-rw-r--r--   0        0        0      195 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/dcstr.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/dds_pipe.json
+-rw-r--r--   0        0        0      193 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/derf.json
+-rw-r--r--   0        0        0      193 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/dfa.json
+-rw-r--r--   0        0        0      201 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/dfpwm.json
+-rw-r--r--   0        0        0      192 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/dhav.json
+-rw-r--r--   0        0        0      204 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/dirac.json
+-rw-r--r--   0        0        0      221 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/dnxhd.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/dpx_pipe.json
+-rw-r--r--   0        0        0      198 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/dsf.json
+-rw-r--r--   0        0        0      215 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/dsicin.json
+-rw-r--r--   0        0        0      211 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/dss.json
+-rw-r--r--   0        0        0      202 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/dts.json
+-rw-r--r--   0        0        0      196 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/dtshd.json
+-rw-r--r--   0        0        0      220 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/dv.json
+-rw-r--r--   0        0        0      190 2024-05-14 09:30:20.811380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/dvbsub.json
+-rw-r--r--   0        0        0      186 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/dvbtxt.json
+-rw-r--r--   0        0        0      224 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/dvd.json
+-rw-r--r--   0        0        0      180 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/dxa.json
+-rw-r--r--   0        0        0      202 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ea.json
+-rw-r--r--   0        0        0      210 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ea_cdata.json
+-rw-r--r--   0        0        0      216 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/eac3.json
+-rw-r--r--   0        0        0      214 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/epaf.json
+-rw-r--r--   0        0        0      197 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/evc.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/exr_pipe.json
+-rw-r--r--   0        0        0      223 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/f32be.json
+-rw-r--r--   0        0        0      226 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/f32le.json
+-rw-r--r--   0        0        0      225 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/f4v.json
+-rw-r--r--   0        0        0      223 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/f64be.json
+-rw-r--r--   0        0        0      226 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/f64le.json
+-rw-r--r--   0        0        0      214 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ffmetadata.json
+-rw-r--r--   0        0        0      201 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/fifo.json
+-rw-r--r--   0        0        0      198 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/fifo_test.json
+-rw-r--r--   0        0        0      224 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/film_cpk.json
+-rw-r--r--   0        0        0      210 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/filmstrip.json
+-rw-r--r--   0        0        0      218 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/fits.json
+-rw-r--r--   0        0        0      210 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/flac.json
+-rw-r--r--   0        0        0      199 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/flic.json
+-rw-r--r--   0        0        0      216 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/flv.json
+-rw-r--r--   0        0        0      215 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/framecrc.json
+-rw-r--r--   0        0        0      222 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/framehash.json
+-rw-r--r--   0        0        0      220 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/framemd5.json
+-rw-r--r--   0        0        0      190 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/frm.json
+-rw-r--r--   0        0        0      198 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/fsb.json
+-rw-r--r--   0        0        0      211 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/fwse.json
+-rw-r--r--   0        0        0      219 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/g722.json
+-rw-r--r--   0        0        0      228 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/g723_1.json
+-rw-r--r--   0        0        0      228 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/g726.json
+-rw-r--r--   0        0        0      236 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/g726le.json
+-rw-r--r--   0        0        0      208 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/g729.json
+-rw-r--r--   0        0        0      198 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/gdv.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/gem_pipe.json
+-rw-r--r--   0        0        0      198 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/genh.json
+-rw-r--r--   0        0        0      237 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/gif.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/gif_pipe.json
+-rw-r--r--   0        0        0      202 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/gsm.json
+-rw-r--r--   0        0        0      229 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/gxf.json
+-rw-r--r--   0        0        0      208 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/h261.json
+-rw-r--r--   0        0        0      208 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/h263.json
+-rw-r--r--   0        0        0      224 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/h264.json
+-rw-r--r--   0        0        0      207 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/hash.json
+-rw-r--r--   0        0        0      189 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/hca.json
+-rw-r--r--   0        0        0      192 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/hcom.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/hdr_pipe.json
+-rw-r--r--   0        0        0      193 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/hds.json
+-rw-r--r--   0        0        0      216 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/hevc.json
+-rw-r--r--   0        0        0      214 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/hls.json
+-rw-r--r--   0        0        0      188 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/hnm.json
+-rw-r--r--   0        0        0      214 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ico.json
+-rw-r--r--   0        0        0      191 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/idcin.json
+-rw-r--r--   0        0        0      195 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/idf.json
+-rw-r--r--   0        0        0      206 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/iff.json
+-rw-r--r--   0        0        0      194 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ifv.json
+-rw-r--r--   0        0        0      208 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ilbc.json
+-rw-r--r--   0        0        0      495 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/image2.json
+-rw-r--r--   0        0        0      209 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/image2pipe.json
+-rw-r--r--   0        0        0      210 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/imf.json
+-rw-r--r--   0        0        0      207 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ingenient.json
+-rw-r--r--   0        0        0      194 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ipmovie.json
+-rw-r--r--   0        0        0      244 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ipod.json
+-rw-r--r--   0        0        0      195 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ipu.json
+-rw-r--r--   0        0        0      232 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ircam.json
+-rw-r--r--   0        0        0      236 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ismv.json
+-rw-r--r--   0        0        0      187 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/iss.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/iv8.json
+-rw-r--r--   0        0        0      191 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ivf.json
+-rw-r--r--   0        0        0      212 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ivr.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/j2k_pipe.json
+-rw-r--r--   0        0        0      228 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/jacosub.json
+-rw-r--r--   0        0        0      202 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/jpeg_pipe.json
+-rw-r--r--   0        0        0      206 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/jpegls_pipe.json
+-rw-r--r--   0        0        0      206 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/jpegxl_anim.json
+-rw-r--r--   0        0        0      206 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/jpegxl_pipe.json
+-rw-r--r--   0        0        0      194 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/jv.json
+-rw-r--r--   0        0        0      193 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/kux.json
+-rw-r--r--   0        0        0      227 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/kvag.json
+-rw-r--r--   0        0        0      210 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/laf.json
+-rw-r--r--   0        0        0      219 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/latm.json
+-rw-r--r--   0        0        0      211 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/lavfi.json
+-rw-r--r--   0        0        0      214 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/live_flv.json
+-rw-r--r--   0        0        0      188 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/lmlm4.json
+-rw-r--r--   0        0        0      198 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/loas.json
+-rw-r--r--   0        0        0      191 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/lrc.json
+-rw-r--r--   0        0        0      199 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/luodat.json
+-rw-r--r--   0        0        0      185 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/lvf.json
+-rw-r--r--   0        0        0      199 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/lxf.json
+-rw-r--r--   0        0        0      202 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/m4v.json
+-rw-r--r--   0        0        0      237 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/matroska,webm.json
+-rw-r--r--   0        0        0      221 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/matroska.json
+-rw-r--r--   0        0        0      198 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mca.json
+-rw-r--r--   0        0        0      192 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mcc.json
+-rw-r--r--   0        0        0      205 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/md5.json
+-rw-r--r--   0        0        0      212 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mgsts.json
+-rw-r--r--   0        0        0      225 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/microdvd.json
+-rw-r--r--   0        0        0      233 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mjpeg.json
+-rw-r--r--   0        0        0      209 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mjpeg_2000.json
+-rw-r--r--   0        0        0      256 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mkvtimestamp_v2.json
+-rw-r--r--   0        0        0      191 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mlp.json
+-rw-r--r--   0        0        0      202 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mlv.json
+-rw-r--r--   0        0        0      199 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mm.json
+-rw-r--r--   0        0        0      219 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mmf.json
+-rw-r--r--   0        0        0      197 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mods.json
+-rw-r--r--   0        0        0      203 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/moflex.json
+-rw-r--r--   0        0        0      304 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mov,mp4,m4a,3gp,3g2,mj2.json
+-rw-r--r--   0        0        0      204 2024-05-14 09:30:20.815380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mov.json
+-rw-r--r--   0        0        0      233 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mp2.json
+-rw-r--r--   0        0        0      242 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mp3.json
+-rw-r--r--   0        0        0      218 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mp4.json
+-rw-r--r--   0        0        0      190 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mpc.json
+-rw-r--r--   0        0        0      190 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mpc8.json
+-rw-r--r--   0        0        0      249 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mpeg.json
+-rw-r--r--   0        0        0      240 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mpeg1video.json
+-rw-r--r--   0        0        0      215 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mpeg2video.json
+-rw-r--r--   0        0        0      261 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mpegts.json
+-rw-r--r--   0        0        0      220 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mpegtsraw.json
+-rw-r--r--   0        0        0      197 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mpegvideo.json
+-rw-r--r--   0        0        0      234 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mpjpeg.json
+-rw-r--r--   0        0        0      205 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mpl2.json
+-rw-r--r--   0        0        0      201 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mpsub.json
+-rw-r--r--   0        0        0      194 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/msf.json
+-rw-r--r--   0        0        0      203 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/msnwctcp.json
+-rw-r--r--   0        0        0      199 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/msp.json
+-rw-r--r--   0        0        0      199 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mtaf.json
+-rw-r--r--   0        0        0      180 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mtv.json
+-rw-r--r--   0        0        0      201 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mulaw.json
+-rw-r--r--   0        0        0      196 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/musx.json
+-rw-r--r--   0        0        0      198 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mv.json
+-rw-r--r--   0        0        0      199 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mvi.json
+-rw-r--r--   0        0        0      245 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mxf.json
+-rw-r--r--   0        0        0      258 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mxf_d10.json
+-rw-r--r--   0        0        0      273 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mxf_opatom.json
+-rw-r--r--   0        0        0      192 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/mxg.json
+-rw-r--r--   0        0        0      193 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/nc.json
+-rw-r--r--   0        0        0      225 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/nistsphere.json
+-rw-r--r--   0        0        0      209 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/nsp.json
+-rw-r--r--   0        0        0      201 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/nsv.json
+-rw-r--r--   0        0        0      216 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/null.json
+-rw-r--r--   0        0        0      206 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/nut.json
+-rw-r--r--   0        0        0      188 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/nuv.json
+-rw-r--r--   0        0        0      204 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/obu.json
+-rw-r--r--   0        0        0      204 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/oga.json
+-rw-r--r--   0        0        0      211 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ogg.json
+-rw-r--r--   0        0        0      212 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ogv.json
+-rw-r--r--   0        0        0      229 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/oma.json
+-rw-r--r--   0        0        0      205 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/opus.json
+-rw-r--r--   0        0        0      189 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/osq.json
+-rw-r--r--   0        0        0      213 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/paf.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/pam_pipe.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/pbm_pipe.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/pcx_pipe.json
+-rw-r--r--   0        0        0      196 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/pdv.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/pfm_pipe.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/pgm_pipe.json
+-rw-r--r--   0        0        0      206 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/pgmyuv_pipe.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/pgx_pipe.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/phm_pipe.json
+-rw-r--r--   0        0        0      208 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/photocd_pipe.json
+-rw-r--r--   0        0        0      206 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/pictor_pipe.json
+-rw-r--r--   0        0        0      226 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/pjs.json
+-rw-r--r--   0        0        0      201 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/pmp.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/png_pipe.json
+-rw-r--r--   0        0        0      208 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/pp_bnk.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ppm_pipe.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/psd_pipe.json
+-rw-r--r--   0        0        0      220 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/psp.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/psxstr.json
+-rw-r--r--   0        0        0      192 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/pva.json
+-rw-r--r--   0        0        0      209 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/pvf.json
+-rw-r--r--   0        0        0      180 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/qcp.json
+-rw-r--r--   0        0        0      204 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/qdraw_pipe.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/qoi_pipe.json
+-rw-r--r--   0        0        0      188 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/r3d.json
+-rw-r--r--   0        0        0      225 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/rawvideo.json
+-rw-r--r--   0        0        0      210 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/realtext.json
+-rw-r--r--   0        0        0      195 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/redspark.json
+-rw-r--r--   0        0        0      196 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/rka.json
+-rw-r--r--   0        0        0      180 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/rl2.json
+-rw-r--r--   0        0        0      216 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/rm.json
+-rw-r--r--   0        0        0      202 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/roq.json
+-rw-r--r--   0        0        0      190 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/rpl.json
+-rw-r--r--   0        0        0      194 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/rsd.json
+-rw-r--r--   0        0        0      206 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/rso.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/rtp.json
+-rw-r--r--   0        0        0      216 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/rtp_mpegts.json
+-rw-r--r--   0        0        0      196 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/rtsp.json
+-rw-r--r--   0        0        0      215 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/s16be.json
+-rw-r--r--   0        0        0      222 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/s16le.json
+-rw-r--r--   0        0        0      215 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/s24be.json
+-rw-r--r--   0        0        0      218 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/s24le.json
+-rw-r--r--   0        0        0      215 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/s32be.json
+-rw-r--r--   0        0        0      218 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/s32le.json
+-rw-r--r--   0        0        0      189 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/s337m.json
+-rw-r--r--   0        0        0      201 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/s8.json
+-rw-r--r--   0        0        0      211 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/sami.json
+-rw-r--r--   0        0        0      194 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/sap.json
+-rw-r--r--   0        0        0      210 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/sbc.json
+-rw-r--r--   0        0        0      210 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/sbg.json
+-rw-r--r--   0        0        0      206 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/scc.json
+-rw-r--r--   0        0        0      192 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/scd.json
+-rw-r--r--   0        0        0      208 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/sdl,sdl2.json
+-rw-r--r--   0        0        0      193 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/sdns.json
+-rw-r--r--   0        0        0      180 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/sdp.json
+-rw-r--r--   0        0        0      188 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/sdr2.json
+-rw-r--r--   0        0        0      207 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/sds.json
+-rw-r--r--   0        0        0      202 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/sdx.json
+-rw-r--r--   0        0        0      188 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/segment.json
+-rw-r--r--   0        0        0      247 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ser.json
+-rw-r--r--   0        0        0      202 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/sga.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/sgi_pipe.json
+-rw-r--r--   0        0        0      193 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/shn.json
+-rw-r--r--   0        0        0      207 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/siff.json
+-rw-r--r--   0        0        0      217 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/simbiosis_imx.json
+-rw-r--r--   0        0        0      198 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/sln.json
+-rw-r--r--   0        0        0      213 2024-05-14 09:30:20.819380 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/smjpeg.json
+-rw-r--r--   0        0        0      184 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/smk.json
+-rw-r--r--   0        0        0      218 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/smoothstreaming.json
+-rw-r--r--   0        0        0      194 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/smush.json
+-rw-r--r--   0        0        0      187 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/sol.json
+-rw-r--r--   0        0        0      217 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/sox.json
+-rw-r--r--   0        0        0      223 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/spdif.json
+-rw-r--r--   0        0        0      205 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/spx.json
+-rw-r--r--   0        0        0      216 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/srt.json
+-rw-r--r--   0        0        0      204 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/stl.json
+-rw-r--r--   0        0        0      220 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/stream_segment,ssegment.json
+-rw-r--r--   0        0        0      224 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/streamhash.json
+-rw-r--r--   0        0        0      213 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/subviewer.json
+-rw-r--r--   0        0        0      217 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/subviewer1.json
+-rw-r--r--   0        0        0      208 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/sunrast_pipe.json
+-rw-r--r--   0        0        0      244 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/sup.json
+-rw-r--r--   0        0        0      199 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/svag.json
+-rw-r--r--   0        0        0      222 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/svcd.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/svg_pipe.json
+-rw-r--r--   0        0        0      192 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/svs.json
+-rw-r--r--   0        0        0      238 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/swf.json
+-rw-r--r--   0        0        0      189 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/tak.json
+-rw-r--r--   0        0        0      203 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/tedcaptions.json
+-rw-r--r--   0        0        0      195 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/tee.json
+-rw-r--r--   0        0        0      180 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/thp.json
+-rw-r--r--   0        0        0      203 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/tiertexseq.json
+-rw-r--r--   0        0        0      202 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/tiff_pipe.json
+-rw-r--r--   0        0        0      189 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/tmv.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/truehd.json
+-rw-r--r--   0        0        0      211 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/tta.json
+-rw-r--r--   0        0        0      206 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ttml.json
+-rw-r--r--   0        0        0      245 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/tty.json
+-rw-r--r--   0        0        0      206 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/txd.json
+-rw-r--r--   0        0        0      190 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/ty.json
+-rw-r--r--   0        0        0      217 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/u16be.json
+-rw-r--r--   0        0        0      224 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/u16le.json
+-rw-r--r--   0        0        0      217 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/u24be.json
+-rw-r--r--   0        0        0      220 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/u24le.json
+-rw-r--r--   0        0        0      217 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/u32be.json
+-rw-r--r--   0        0        0      220 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/u32le.json
+-rw-r--r--   0        0        0      203 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/u8.json
+-rw-r--r--   0        0        0      230 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/uncodedframecrc.json
+-rw-r--r--   0        0        0      189 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/usm.json
+-rw-r--r--   0        0        0      209 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/v210.json
+-rw-r--r--   0        0        0      211 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/v210x.json
+-rw-r--r--   0        0        0      194 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/vag.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/vbn_pipe.json
+-rw-r--r--   0        0        0      198 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/vc1.json
+-rw-r--r--   0        0        0      208 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/vc1test.json
+-rw-r--r--   0        0        0      242 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/vcd.json
+-rw-r--r--   0        0        0      204 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/vidc.json
+-rw-r--r--   0        0        0      192 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/vividas.json
+-rw-r--r--   0        0        0      187 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/vivo.json
+-rw-r--r--   0        0        0      187 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/vmd.json
+-rw-r--r--   0        0        0      220 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/vob.json
+-rw-r--r--   0        0        0      207 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/vobsub.json
+-rw-r--r--   0        0        0      215 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/voc.json
+-rw-r--r--   0        0        0      194 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/vpk.json
+-rw-r--r--   0        0        0      203 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/vplayer.json
+-rw-r--r--   0        0        0      251 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/vqf.json
+-rw-r--r--   0        0        0      218 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/vvc.json
+-rw-r--r--   0        0        0      201 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/w64.json
+-rw-r--r--   0        0        0      194 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/wady.json
+-rw-r--r--   0        0        0      228 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/wav.json
+-rw-r--r--   0        0        0      201 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/wavarc.json
+-rw-r--r--   0        0        0      206 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/wc3movie.json
+-rw-r--r--   0        0        0      205 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/webm.json
+-rw-r--r--   0        0        0      215 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/webm_chunk.json
+-rw-r--r--   0        0        0      229 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/webm_dash_manifest.json
+-rw-r--r--   0        0        0      192 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/webp.json
+-rw-r--r--   0        0        0      202 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/webp_pipe.json
+-rw-r--r--   0        0        0      207 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/webvtt.json
+-rw-r--r--   0        0        0      217 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/wsaud.json
+-rw-r--r--   0        0        0      212 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/wsd.json
+-rw-r--r--   0        0        0      199 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/wsvqa.json
+-rw-r--r--   0        0        0      218 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/wtv.json
+-rw-r--r--   0        0        0      212 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/wv.json
+-rw-r--r--   0        0        0      190 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/wve.json
+-rw-r--r--   0        0        0      210 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/x11grab.json
+-rw-r--r--   0        0        0      184 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/xa.json
+-rw-r--r--   0        0        0      205 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/xbin.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/xbm_pipe.json
+-rw-r--r--   0        0        0      192 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/xmd.json
+-rw-r--r--   0        0        0      195 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/xmv.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/xpm_pipe.json
+-rw-r--r--   0        0        0      197 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/xvag.json
+-rw-r--r--   0        0        0      200 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/xwd_pipe.json
+-rw-r--r--   0        0        0      192 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/xwma.json
+-rw-r--r--   0        0        0      195 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/yop.json
+-rw-r--r--   0        0        0      218 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/cache/yuv4mpegpipe.json
+-rw-r--r--   0        0        0      101 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/exceptions.py
+-rw-r--r--   0        0        0     3463 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/info.py
+-rw-r--r--   0        0        0        0 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/py.typed
+-rw-r--r--   0        0        0     3387 2024-05-14 09:30:20.823381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/schema.py
+-rw-r--r--   0        0        0        0 2024-05-14 09:30:20.927381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/utils/__init__.py
+-rw-r--r--   0        0        0     1015 2024-05-14 09:30:20.927381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/utils/cache.py
+-rw-r--r--   0        0        0      909 2024-05-14 09:30:20.927381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/utils/ffprobe.py
+-rw-r--r--   0        0        0     4858 2024-05-14 09:30:20.927381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/utils/hotfix_webp.py
+-rw-r--r--   0        0        0     1008 2024-05-14 09:30:20.927381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/utils/loader.py
+-rw-r--r--   0        0        0     1130 2024-05-14 09:30:20.927381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/utils/shell.py
+-rw-r--r--   0        0        0     1275 2024-05-14 09:30:20.927381 ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/utils/thumbnail.py
+-rw-r--r--   0        0        0     7093 1970-01-01 00:00:00.000000 ffmpeg_media_type-1.0.2/PKG-INFO
```

### Comparing `ffmpeg_media_type-1.0.1/LICENSE` & `ffmpeg_media_type-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-1.0.1/README.md` & `ffmpeg_media_type-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-1.0.1/pyproject.toml` & `ffmpeg_media_type-1.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ffmpeg-media-type"
-version = "1.0.1"
+version = "1.0.2"
 description = "ffmpeg-media-type is a Python library that utilizes FFmpeg to extract crucial details from media files, such as duration, width, and height. With seamless integration of 100% typehint support, it offers a user-friendly interface for easy access to media file information."
 authors = ["lucemia <lucemia@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "ffmpeg_media_type", from = "src" }]
 include = ["ffmpeg_media_type/py.typed", "ffmpeg_media_type/cache/*.json"]
 exclude = ["**/tests", "**/test_data", "**/conftest.py"]
 keywords = ["ffmpeg", "ffprobe", "video", "image", "audio", "media", "mimetype", "mp4", "mp3", "mov", "webm"]
@@ -32,15 +32,15 @@
 
 # test
 pre-commit = "^3.3.3"
 mypy = "^1.4.1"
 syrupy = "^4.0.5"
 pytest = "^7.4.0"
 pytest-vcr = "^1.0.2"
-pytest-cov = "^4.1.0"
+pytest-cov = ">=4.1,<6.0"
 
 # Doc
 mkdocs = "*"
 markdown-callouts = "^0.4.0"
 mkdocs-material = "^9.5.9"
 mkdocstrings = "^0.24.0"
 mkdocstrings-python = "^1.8.0"
```

### Comparing `ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/info.py` & `ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from pathlib import Path
 from urllib.parse import urlparse
 
 from .schema import FFMpegSupport, MediaInfo
 from .utils.cache import load
 from .utils.ffprobe import ffprobe
 from .utils.thumbnail import generate_thumbnail
 
@@ -36,27 +37,28 @@
     "mjpeg": ("jpg", "jpeg", "mjpeg"),
 }
 """
 Dictionary mapping codec names to common file extensions.
 """
 
 
-def detect(uri: str) -> MediaInfo:
+def detect(uri: str | Path) -> MediaInfo:
     """
     Detect the media type of a file.
 
     Args:
         uri: the URI of the file
 
     Returns:
         the media type information
 
     Raises:
         FfmpegMediaTypeError: If the ffmpeg command fails.
     """
+    uri = str(uri)
     info = ffprobe(uri)
     current_ext = extract_file_extension_from_uri(uri)
 
     format_name = info.format.format_name
     duration = info.format.duration
 
     # NOTE: handle ffmpeg's image compatibility
```

### Comparing `ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/schema.py` & `ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/schema.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/utils/cache.py` & `ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/utils/ffprobe.py` & `ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/utils/ffprobe.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/utils/hotfix_webp.py` & `ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/utils/hotfix_webp.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/utils/loader.py` & `ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/utils/loader.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/utils/shell.py` & `ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/utils/shell.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-1.0.1/src/ffmpeg_media_type/utils/thumbnail.py` & `ffmpeg_media_type-1.0.2/src/ffmpeg_media_type/utils/thumbnail.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-1.0.1/PKG-INFO` & `ffmpeg_media_type-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-media-type
-Version: 1.0.1
+Version: 1.0.2
 Summary: ffmpeg-media-type is a Python library that utilizes FFmpeg to extract crucial details from media files, such as duration, width, and height. With seamless integration of 100% typehint support, it offers a user-friendly interface for easy access to media file information.
 Keywords: ffmpeg,ffprobe,video,image,audio,media,mimetype,mp4,mp3,mov,webm
 Author: lucemia
 Author-email: lucemia@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

