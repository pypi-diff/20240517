# Comparing `tmp/ccxt-idax-adapter-4.3.25.tar.gz` & `tmp/ccxt-idax-adapter-4.3.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccxt-idax-adapter-4.3.25.tar", last modified: Wed May 15 10:08:27 2024, max compression
+gzip compressed data, was "ccxt-idax-adapter-4.3.26.tar", last modified: Fri May 17 08:41:31 2024, max compression
```

## Comparing `ccxt-idax-adapter-4.3.25.tar` & `ccxt-idax-adapter-4.3.26.tar`

### file list

```diff
@@ -1,578 +1,578 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.698065 ccxt-idax-adapter-4.3.25/
--rw-rw-rw-   0        0        0     1068 2024-05-15 10:03:58.000000 ccxt-idax-adapter-4.3.25/LICENSE.txt
--rw-rw-rw-   0        0        0      101 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.25/MANIFEST.in
--rw-rw-rw-   0        0        0     2759 2024-05-15 10:08:27.698065 ccxt-idax-adapter-4.3.25/PKG-INFO
--rw-rw-rw-   0        0        0   102253 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.25/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:26.667533 ccxt-idax-adapter-4.3.25/ccxt/
--rw-rw-rw-   0        0        0    15933 2024-05-15 10:03:23.000000 ccxt-idax-adapter-4.3.25/ccxt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:26.901101 ccxt-idax-adapter-4.3.25/ccxt/abstract/
--rw-rw-rw-   0        0        0        0 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/__init__.py
--rw-rw-rw-   0        0        0     1448 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/ace.py
--rw-rw-rw-   0        0        0    10382 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/alpaca.py
--rw-rw-rw-   0        0        0    11394 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/ascendex.py
--rw-rw-rw-   0        0        0    15601 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bequant.py
--rw-rw-rw-   0        0        0     4895 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bigone.py
--rw-rw-rw-   0        0        0    92208 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/binance.py
--rw-rw-rw-   0        0        0    92208 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/binancecoinm.py
--rw-rw-rw-   0        0        0    98928 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/binanceus.py
--rw-rw-rw-   0        0        0    92208 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/binanceusdm.py
--rw-rw-rw-   0        0        0    16032 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bingx.py
--rw-rw-rw-   0        0        0     2830 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bit2c.py
--rw-rw-rw-   0        0        0     2735 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bitbank.py
--rw-rw-rw-   0        0        0     5820 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bitbay.py
--rw-rw-rw-   0        0        0     4082 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bitbns.py
--rw-rw-rw-   0        0        0    15601 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bitcoincom.py
--rw-rw-rw-   0        0        0     7605 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bitfinex.py
--rw-rw-rw-   0        0        0    19194 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bitfinex2.py
--rw-rw-rw-   0        0        0     3576 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bitflyer.py
--rw-rw-rw-   0        0        0    90336 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bitget.py
--rw-rw-rw-   0        0        0     3443 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bithumb.py
--rw-rw-rw-   0        0        0    14031 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bitmart.py
--rw-rw-rw-   0        0        0    10774 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bitmex.py
--rw-rw-rw-   0        0        0     3295 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bitopro.py
--rw-rw-rw-   0        0        0     3859 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bitpanda.py
--rw-rw-rw-   0        0        0     9379 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bitrue.py
--rw-rw-rw-   0        0        0     4025 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bitso.py
--rw-rw-rw-   0        0        0    27930 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bitstamp.py
--rw-rw-rw-   0        0        0     3478 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bitteam.py
--rw-rw-rw-   0        0        0     2357 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bitvavo.py
--rw-rw-rw-   0        0        0     2024 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bl3p.py
--rw-rw-rw-   0        0        0     2638 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/blockchaincom.py
--rw-rw-rw-   0        0        0     4217 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/blofin.py
--rw-rw-rw-   0        0        0     1380 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/btcalpha.py
--rw-rw-rw-   0        0        0      849 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/btcbox.py
--rw-rw-rw-   0        0        0     3690 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/btcmarkets.py
--rw-rw-rw-   0        0        0     1777 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/btcturk.py
--rw-rw-rw-   0        0        0    48923 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/bybit.py
--rw-rw-rw-   0        0        0     3311 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/cex.py
--rw-rw-rw-   0        0        0    15507 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/coinbase.py
--rw-rw-rw-   0        0        0     4770 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/coinbaseinternational.py
--rw-rw-rw-   0        0        0     7162 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/coinbasepro.py
--rw-rw-rw-   0        0        0     3417 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/coincheck.py
--rw-rw-rw-   0        0        0    34678 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/coinex.py
--rw-rw-rw-   0        0        0     6538 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/coinlist.py
--rw-rw-rw-   0        0        0     6842 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/coinmate.py
--rw-rw-rw-   0        0        0     3975 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/coinmetro.py
--rw-rw-rw-   0        0        0     8291 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/coinone.py
--rw-rw-rw-   0        0        0     8007 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/coinsph.py
--rw-rw-rw-   0        0        0     2707 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/coinspot.py
--rw-rw-rw-   0        0        0    18475 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/cryptocom.py
--rw-rw-rw-   0        0        0     7563 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/currencycom.py
--rw-rw-rw-   0        0        0     5107 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/delta.py
--rw-rw-rw-   0        0        0    15499 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/deribit.py
--rw-rw-rw-   0        0        0    11452 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/digifinex.py
--rw-rw-rw-   0        0        0     6177 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/exmo.py
--rw-rw-rw-   0        0        0    15601 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/fmfwio.py
--rw-rw-rw-   0        0        0    41994 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/gate.py
--rw-rw-rw-   0        0        0    41994 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/gateio.py
--rw-rw-rw-   0        0        0     6915 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/gemini.py
--rw-rw-rw-   0        0        0    15601 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/hitbtc.py
--rw-rw-rw-   0        0        0    15601 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/hitbtc3.py
--rw-rw-rw-   0        0        0     2906 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/hollaex.py
--rw-rw-rw-   0        0        0    99311 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/htx.py
--rw-rw-rw-   0        0        0    99311 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/huobi.py
--rw-rw-rw-   0        0        0    14331 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/huobijp.py
--rw-rw-rw-   0        0        0      240 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/hyperliquid.py
--rw-rw-rw-   0        0        0     1743 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/idax.py
--rw-rw-rw-   0        0        0     2129 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/idex.py
--rw-rw-rw-   0        0        0     4165 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/independentreserve.py
--rw-rw-rw-   0        0        0     2488 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/indodax.py
--rw-rw-rw-   0        0        0     5877 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/kraken.py
--rw-rw-rw-   0        0        0     3537 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/krakenfutures.py
--rw-rw-rw-   0        0        0    25491 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/kucoin.py
--rw-rw-rw-   0        0        0    28204 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/kucoinfutures.py
--rw-rw-rw-   0        0        0    24579 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/kuna.py
--rw-rw-rw-   0        0        0     7168 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/latoken.py
--rw-rw-rw-   0        0        0     8675 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/lbank.py
--rw-rw-rw-   0        0        0     3619 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/luno.py
--rw-rw-rw-   0        0        0     2960 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/lykke.py
--rw-rw-rw-   0        0        0     2357 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/mercado.py
--rw-rw-rw-   0        0        0    25902 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/mexc.py
--rw-rw-rw-   0        0        0    11878 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/ndax.py
--rw-rw-rw-   0        0        0     3093 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/novadax.py
--rw-rw-rw-   0        0        0     1721 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/oceanex.py
--rw-rw-rw-   0        0        0     9414 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/okcoin.py
--rw-rw-rw-   0        0        0    46458 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/okx.py
--rw-rw-rw-   0        0        0     3859 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/onetrading.py
--rw-rw-rw-   0        0        0     2054 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/p2b.py
--rw-rw-rw-   0        0        0     2843 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/paymium.py
--rw-rw-rw-   0        0        0    15203 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/phemex.py
--rw-rw-rw-   0        0        0     8073 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/poloniex.py
--rw-rw-rw-   0        0        0     5219 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/poloniexfutures.py
--rw-rw-rw-   0        0        0     1969 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/probit.py
--rw-rw-rw-   0        0        0     5875 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/timex.py
--rw-rw-rw-   0        0        0     4094 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/tokocrypto.py
--rw-rw-rw-   0        0        0     1372 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/tradeogre.py
--rw-rw-rw-   0        0        0     3576 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/upbit.py
--rw-rw-rw-   0        0        0    19631 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/wavesexchange.py
--rw-rw-rw-   0        0        0     2782 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/wazirx.py
--rw-rw-rw-   0        0        0    10977 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/whitebit.py
--rw-rw-rw-   0        0        0    10368 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/woo.py
--rw-rw-rw-   0        0        0    16016 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/woofipro.py
--rw-rw-rw-   0        0        0     1339 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/yobit.py
--rw-rw-rw-   0        0        0     3935 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/zaif.py
--rw-rw-rw-   0        0        0     5820 2024-05-15 10:03:48.000000 ccxt-idax-adapter-4.3.25/ccxt/abstract/zonda.py
--rw-rw-rw-   0        0        0    41656 2024-05-09 07:22:32.000000 ccxt-idax-adapter-4.3.25/ccxt/ace.py
--rw-rw-rw-   0        0        0    47215 2024-05-05 05:05:27.000000 ccxt-idax-adapter-4.3.25/ccxt/alpaca.py
--rw-rw-rw-   0        0        0   151471 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/ascendex.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.195774 ccxt-idax-adapter-4.3.25/ccxt/async_support/
--rw-rw-rw-   0        0        0    15706 2024-05-15 10:03:23.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/__init__.py
--rw-rw-rw-   0        0        0    41880 2024-05-09 07:22:32.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/ace.py
--rw-rw-rw-   0        0        0    47427 2024-05-05 05:05:27.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/alpaca.py
--rw-rw-rw-   0        0        0   152259 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/ascendex.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.202017 ccxt-idax-adapter-4.3.25/ccxt/async_support/base/
--rw-rw-rw-   0        0        0       67 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/base/__init__.py
--rw-rw-rw-   0        0        0   108636 2024-05-15 10:05:03.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/base/exchange.py
--rw-rw-rw-   0        0        0     1847 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/base/throttler.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.222694 ccxt-idax-adapter-4.3.25/ccxt/async_support/base/ws/
--rw-rw-rw-   0        0        0     1791 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/base/ws/__init__.py
--rw-rw-rw-   0        0        0     5751 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/base/ws/aiohttp_client.py
--rw-rw-rw-   0        0        0     8100 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/base/ws/cache.py
--rw-rw-rw-   0        0        0     7289 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/base/ws/client.py
--rw-rw-rw-   0        0        0     3864 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/base/ws/fast_client.py
--rw-rw-rw-   0        0        0     1499 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/base/ws/functions.py
--rw-rw-rw-   0        0        0     2067 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/base/ws/future.py
--rw-rw-rw-   0        0        0     2894 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/base/ws/order_book.py
--rw-rw-rw-   0        0        0     6478 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/base/ws/order_book_side.py
--rw-rw-rw-   0        0        0     1188 2024-05-09 07:22:35.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bequant.py
--rw-rw-rw-   0        0        0    92663 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bigone.py
--rw-rw-rw-   0        0        0   620262 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/binance.py
--rw-rw-rw-   0        0        0     1683 2024-05-09 07:23:11.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/binancecoinm.py
--rw-rw-rw-   0        0        0     9177 2024-05-09 07:23:12.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/binanceus.py
--rw-rw-rw-   0        0        0     2518 2024-05-09 07:23:12.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/binanceusdm.py
--rw-rw-rw-   0        0        0   185869 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bingx.py
--rw-rw-rw-   0        0        0    37119 2024-05-09 07:23:14.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bit2c.py
--rw-rw-rw-   0        0        0    42105 2024-05-09 07:23:15.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bitbank.py
--rw-rw-rw-   0        0        0      492 2024-05-09 07:23:15.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bitbay.py
--rw-rw-rw-   0        0        0    48391 2024-05-09 07:23:16.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bitbns.py
--rw-rw-rw-   0        0        0      516 2024-05-09 07:23:16.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bitcoincom.py
--rw-rw-rw-   0        0        0    72718 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bitfinex.py
--rw-rw-rw-   0        0        0   159249 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bitfinex2.py
--rw-rw-rw-   0        0        0    41705 2024-05-09 07:23:21.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bitflyer.py
--rw-rw-rw-   0        0        0   424141 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bitget.py
--rw-rw-rw-   0        0        0    45764 2024-05-09 07:23:59.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bithumb.py
--rw-rw-rw-   0        0        0   200057 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bitmart.py
--rw-rw-rw-   0        0        0   127162 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bitmex.py
--rw-rw-rw-   0        0        0    68926 2024-05-09 07:24:20.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bitopro.py
--rw-rw-rw-   0        0        0      485 2024-05-09 07:24:20.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bitpanda.py
--rw-rw-rw-   0        0        0   136878 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bitrue.py
--rw-rw-rw-   0        0        0    71271 2024-05-09 07:24:31.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bitso.py
--rw-rw-rw-   0        0        0    92735 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bitstamp.py
--rw-rw-rw-   0        0        0   102358 2024-05-09 07:24:44.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bitteam.py
--rw-rw-rw-   0        0        0    92011 2024-05-09 07:24:49.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bitvavo.py
--rw-rw-rw-   0        0        0    20611 2024-05-09 07:24:50.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bl3p.py
--rw-rw-rw-   0        0        0    49191 2024-05-09 07:24:52.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/blockchaincom.py
--rw-rw-rw-   0        0        0    99837 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/blofin.py
--rw-rw-rw-   0        0        0    36979 2024-05-09 07:24:58.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/btcalpha.py
--rw-rw-rw-   0        0        0    23686 2024-05-09 07:24:59.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/btcbox.py
--rw-rw-rw-   0        0        0    51834 2024-05-09 07:25:01.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/btcmarkets.py
--rw-rw-rw-   0        0        0    36875 2024-05-09 07:25:02.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/btcturk.py
--rw-rw-rw-   0        0        0   414323 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/bybit.py
--rw-rw-rw-   0        0        0    70280 2024-05-09 07:25:37.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/cex.py
--rw-rw-rw-   0        0        0   213105 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/coinbase.py
--rw-rw-rw-   0        0        0    87794 2024-05-05 05:05:27.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/coinbaseinternational.py
--rw-rw-rw-   0        0        0    79177 2024-05-09 07:25:53.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/coinbasepro.py
--rw-rw-rw-   0        0        0    35870 2024-05-09 07:25:56.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/coincheck.py
--rw-rw-rw-   0        0        0   260077 2024-05-14 02:14:32.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/coinex.py
--rw-rw-rw-   0        0        0   103628 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/coinlist.py
--rw-rw-rw-   0        0        0    46212 2024-05-09 07:26:16.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/coinmate.py
--rw-rw-rw-   0        0        0    81020 2024-05-09 07:26:20.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/coinmetro.py
--rw-rw-rw-   0        0        0    47138 2024-05-09 07:26:23.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/coinone.py
--rw-rw-rw-   0        0        0    91066 2024-05-09 07:26:29.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/coinsph.py
--rw-rw-rw-   0        0        0    23766 2024-05-09 07:26:30.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/coinspot.py
--rw-rw-rw-   0        0        0   130329 2024-05-09 07:26:38.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/cryptocom.py
--rw-rw-rw-   0        0        0    87236 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/currencycom.py
--rw-rw-rw-   0        0        0   151119 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/delta.py
--rw-rw-rw-   0        0        0   161375 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/deribit.py
--rw-rw-rw-   0        0        0   169017 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/digifinex.py
--rw-rw-rw-   0        0        0   115087 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/exmo.py
--rw-rw-rw-   0        0        0     1250 2024-05-09 07:27:10.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/fmfwio.py
--rw-rw-rw-   0        0        0   321536 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/gate.py
--rw-rw-rw-   0        0        0      459 2024-05-09 07:27:31.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/gateio.py
--rw-rw-rw-   0        0        0    81171 2024-05-09 07:27:36.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/gemini.py
--rw-rw-rw-   0        0        0   154094 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/hitbtc.py
--rw-rw-rw-   0        0        0      469 2024-05-09 07:27:46.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/hitbtc3.py
--rw-rw-rw-   0        0        0    76379 2024-05-09 07:27:48.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/hollaex.py
--rw-rw-rw-   0        0        0   422813 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/htx.py
--rw-rw-rw-   0        0        0      452 2024-05-09 07:28:52.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/huobi.py
--rw-rw-rw-   0        0        0    88468 2024-05-09 07:28:56.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/huobijp.py
--rw-rw-rw-   0        0        0   101215 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/hyperliquid.py
--rw-rw-rw-   0        0        0    23950 2024-05-15 10:05:01.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/idax.py
--rw-rw-rw-   0        0        0    73474 2024-05-09 07:43:23.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/idex.py
--rw-rw-rw-   0        0        0    32435 2024-05-09 07:43:23.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/independentreserve.py
--rw-rw-rw-   0        0        0    52229 2024-05-09 07:43:24.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/indodax.py
--rw-rw-rw-   0        0        0   126074 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/kraken.py
--rw-rw-rw-   0        0        0   117323 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/krakenfutures.py
--rw-rw-rw-   0        0        0   218810 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/kucoin.py
--rw-rw-rw-   0        0        0   124965 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/kucoinfutures.py
--rw-rw-rw-   0        0        0    96407 2024-05-09 07:43:41.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/kuna.py
--rw-rw-rw-   0        0        0    79673 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/latoken.py
--rw-rw-rw-   0        0        0   115887 2024-05-09 07:43:44.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/lbank.py
--rw-rw-rw-   0        0        0    46225 2024-05-09 07:43:45.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/luno.py
--rw-rw-rw-   0        0        0    51384 2024-05-09 07:43:45.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/lykke.py
--rw-rw-rw-   0        0        0    35581 2024-05-09 07:43:46.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/mercado.py
--rw-rw-rw-   0        0        0   242037 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/mexc.py
--rw-rw-rw-   0        0        0   109125 2024-05-09 07:43:58.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/ndax.py
--rw-rw-rw-   0        0        0    64608 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/novadax.py
--rw-rw-rw-   0        0        0    38180 2024-05-09 07:44:01.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/oceanex.py
--rw-rw-rw-   0        0        0   151675 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/okcoin.py
--rw-rw-rw-   0        0        0   378644 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/okx.py
--rw-rw-rw-   0        0        0    88565 2024-05-09 07:44:52.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/onetrading.py
--rw-rw-rw-   0        0        0    54455 2024-05-09 07:44:53.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/p2b.py
--rw-rw-rw-   0        0        0    24432 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/paymium.py
--rw-rw-rw-   0        0        0   221405 2024-05-14 02:14:32.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/phemex.py
--rw-rw-rw-   0        0        0   102539 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/poloniex.py
--rw-rw-rw-   0        0        0    78185 2024-05-09 07:45:14.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/poloniexfutures.py
--rw-rw-rw-   0        0        0    76771 2024-05-09 07:45:18.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/probit.py
--rw-rw-rw-   0        0        0    71649 2024-05-09 07:45:23.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/timex.py
--rw-rw-rw-   0        0        0   123375 2024-05-09 07:45:36.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/tokocrypto.py
--rw-rw-rw-   0        0        0    24094 2024-05-09 07:45:37.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/tradeogre.py
--rw-rw-rw-   0        0        0    82093 2024-05-09 07:45:41.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/upbit.py
--rw-rw-rw-   0        0        0   114153 2024-05-09 07:45:49.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/wavesexchange.py
--rw-rw-rw-   0        0        0    51644 2024-05-09 07:45:52.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/wazirx.py
--rw-rw-rw-   0        0        0   115022 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/whitebit.py
--rw-rw-rw-   0        0        0   140354 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/woo.py
--rw-rw-rw-   0        0        0   115547 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/woofipro.py
--rw-rw-rw-   0        0        0    53506 2024-05-09 07:46:07.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/yobit.py
--rw-rw-rw-   0        0        0    28161 2024-05-09 07:46:09.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/zaif.py
--rw-rw-rw-   0        0        0    80912 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/async_support/zonda.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.235503 ccxt-idax-adapter-4.3.25/ccxt/base/
--rw-rw-rw-   0        0        0     1320 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/base/__init__.py
--rw-rw-rw-   0        0        0     6634 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/base/decimal_to_precision.py
--rw-rw-rw-   0        0        0     4264 2024-05-15 10:05:03.000000 ccxt-idax-adapter-4.3.25/ccxt/base/errors.py
--rw-rw-rw-   0        0        0   278172 2024-05-15 10:05:03.000000 ccxt-idax-adapter-4.3.25/ccxt/base/exchange.py
--rw-rw-rw-   0        0        0     8565 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/base/precise.py
--rw-rw-rw-   0        0        0     9027 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/base/types.py
--rw-rw-rw-   0        0        0     1174 2024-05-09 07:22:35.000000 ccxt-idax-adapter-4.3.25/ccxt/bequant.py
--rw-rw-rw-   0        0        0    92209 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/bigone.py
--rw-rw-rw-   0        0        0   617552 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/binance.py
--rw-rw-rw-   0        0        0     1645 2024-05-09 07:23:11.000000 ccxt-idax-adapter-4.3.25/ccxt/binancecoinm.py
--rw-rw-rw-   0        0        0     9163 2024-05-09 07:23:12.000000 ccxt-idax-adapter-4.3.25/ccxt/binanceus.py
--rw-rw-rw-   0        0        0     2480 2024-05-09 07:23:12.000000 ccxt-idax-adapter-4.3.25/ccxt/binanceusdm.py
--rw-rw-rw-   0        0        0   184833 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/bingx.py
--rw-rw-rw-   0        0        0    36907 2024-05-09 07:23:14.000000 ccxt-idax-adapter-4.3.25/ccxt/bit2c.py
--rw-rw-rw-   0        0        0    41845 2024-05-09 07:23:15.000000 ccxt-idax-adapter-4.3.25/ccxt/bitbank.py
--rw-rw-rw-   0        0        0      478 2024-05-09 07:23:15.000000 ccxt-idax-adapter-4.3.25/ccxt/bitbay.py
--rw-rw-rw-   0        0        0    48137 2024-05-09 07:23:16.000000 ccxt-idax-adapter-4.3.25/ccxt/bitbns.py
--rw-rw-rw-   0        0        0      502 2024-05-09 07:23:16.000000 ccxt-idax-adapter-4.3.25/ccxt/bitcoincom.py
--rw-rw-rw-   0        0        0    72278 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/bitfinex.py
--rw-rw-rw-   0        0        0   158515 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/bitfinex2.py
--rw-rw-rw-   0        0        0    41397 2024-05-09 07:23:21.000000 ccxt-idax-adapter-4.3.25/ccxt/bitflyer.py
--rw-rw-rw-   0        0        0   422517 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/bitget.py
--rw-rw-rw-   0        0        0    45534 2024-05-09 07:23:59.000000 ccxt-idax-adapter-4.3.25/ccxt/bithumb.py
--rw-rw-rw-   0        0        0   199137 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/bitmart.py
--rw-rw-rw-   0        0        0   126584 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/bitmex.py
--rw-rw-rw-   0        0        0    68522 2024-05-09 07:24:20.000000 ccxt-idax-adapter-4.3.25/ccxt/bitopro.py
--rw-rw-rw-   0        0        0      471 2024-05-09 07:24:20.000000 ccxt-idax-adapter-4.3.25/ccxt/bitpanda.py
--rw-rw-rw-   0        0        0   136220 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/bitrue.py
--rw-rw-rw-   0        0        0    70885 2024-05-09 07:24:31.000000 ccxt-idax-adapter-4.3.25/ccxt/bitso.py
--rw-rw-rw-   0        0        0    92235 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/bitstamp.py
--rw-rw-rw-   0        0        0   102026 2024-05-09 07:24:44.000000 ccxt-idax-adapter-4.3.25/ccxt/bitteam.py
--rw-rw-rw-   0        0        0    91577 2024-05-09 07:24:49.000000 ccxt-idax-adapter-4.3.25/ccxt/bitvavo.py
--rw-rw-rw-   0        0        0    20483 2024-05-09 07:24:50.000000 ccxt-idax-adapter-4.3.25/ccxt/bl3p.py
--rw-rw-rw-   0        0        0    48799 2024-05-09 07:24:52.000000 ccxt-idax-adapter-4.3.25/ccxt/blockchaincom.py
--rw-rw-rw-   0        0        0    99253 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/blofin.py
--rw-rw-rw-   0        0        0    36701 2024-05-09 07:24:58.000000 ccxt-idax-adapter-4.3.25/ccxt/btcalpha.py
--rw-rw-rw-   0        0        0    23492 2024-05-09 07:24:59.000000 ccxt-idax-adapter-4.3.25/ccxt/btcbox.py
--rw-rw-rw-   0        0        0    51484 2024-05-09 07:25:01.000000 ccxt-idax-adapter-4.3.25/ccxt/btcmarkets.py
--rw-rw-rw-   0        0        0    36657 2024-05-09 07:25:02.000000 ccxt-idax-adapter-4.3.25/ccxt/btcturk.py
--rw-rw-rw-   0        0        0   412519 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/bybit.py
--rw-rw-rw-   0        0        0    69930 2024-05-09 07:25:37.000000 ccxt-idax-adapter-4.3.25/ccxt/cex.py
--rw-rw-rw-   0        0        0   211999 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/coinbase.py
--rw-rw-rw-   0        0        0    87240 2024-05-05 05:05:27.000000 ccxt-idax-adapter-4.3.25/ccxt/coinbaseinternational.py
--rw-rw-rw-   0        0        0    78671 2024-05-09 07:25:53.000000 ccxt-idax-adapter-4.3.25/ccxt/coinbasepro.py
--rw-rw-rw-   0        0        0    35664 2024-05-09 07:25:56.000000 ccxt-idax-adapter-4.3.25/ccxt/coincheck.py
--rw-rw-rw-   0        0        0   258783 2024-05-14 02:14:32.000000 ccxt-idax-adapter-4.3.25/ccxt/coinex.py
--rw-rw-rw-   0        0        0   103140 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/coinlist.py
--rw-rw-rw-   0        0        0    45946 2024-05-09 07:26:16.000000 ccxt-idax-adapter-4.3.25/ccxt/coinmate.py
--rw-rw-rw-   0        0        0    80700 2024-05-09 07:26:20.000000 ccxt-idax-adapter-4.3.25/ccxt/coinmetro.py
--rw-rw-rw-   0        0        0    46896 2024-05-09 07:26:23.000000 ccxt-idax-adapter-4.3.25/ccxt/coinone.py
--rw-rw-rw-   0        0        0    90632 2024-05-09 07:26:29.000000 ccxt-idax-adapter-4.3.25/ccxt/coinsph.py
--rw-rw-rw-   0        0        0    23614 2024-05-09 07:26:30.000000 ccxt-idax-adapter-4.3.25/ccxt/coinspot.py
--rw-rw-rw-   0        0        0   129757 2024-05-09 07:26:38.000000 ccxt-idax-adapter-4.3.25/ccxt/cryptocom.py
--rw-rw-rw-   0        0        0    86814 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/currencycom.py
--rw-rw-rw-   0        0        0   150511 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/delta.py
--rw-rw-rw-   0        0        0   160599 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/deribit.py
--rw-rw-rw-   0        0        0   168047 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/digifinex.py
--rw-rw-rw-   0        0        0   114455 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/exmo.py
--rw-rw-rw-   0        0        0     1236 2024-05-09 07:27:10.000000 ccxt-idax-adapter-4.3.25/ccxt/fmfwio.py
--rw-rw-rw-   0        0        0   319858 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/gate.py
--rw-rw-rw-   0        0        0      445 2024-05-09 07:27:31.000000 ccxt-idax-adapter-4.3.25/ccxt/gateio.py
--rw-rw-rw-   0        0        0    80658 2024-05-09 07:27:36.000000 ccxt-idax-adapter-4.3.25/ccxt/gemini.py
--rw-rw-rw-   0        0        0   153048 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/hitbtc.py
--rw-rw-rw-   0        0        0      455 2024-05-09 07:27:46.000000 ccxt-idax-adapter-4.3.25/ccxt/hitbtc3.py
--rw-rw-rw-   0        0        0    75945 2024-05-09 07:27:48.000000 ccxt-idax-adapter-4.3.25/ccxt/hollaex.py
--rw-rw-rw-   0        0        0   420457 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/htx.py
--rw-rw-rw-   0        0        0      438 2024-05-09 07:28:52.000000 ccxt-idax-adapter-4.3.25/ccxt/huobi.py
--rw-rw-rw-   0        0        0    87968 2024-05-09 07:28:56.000000 ccxt-idax-adapter-4.3.25/ccxt/huobijp.py
--rw-rw-rw-   0        0        0   100695 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/hyperliquid.py
--rw-rw-rw-   0        0        0    23664 2024-05-15 10:05:01.000000 ccxt-idax-adapter-4.3.25/ccxt/idax.py
--rw-rw-rw-   0        0        0    72998 2024-05-09 07:43:23.000000 ccxt-idax-adapter-4.3.25/ccxt/idex.py
--rw-rw-rw-   0        0        0    32175 2024-05-09 07:43:23.000000 ccxt-idax-adapter-4.3.25/ccxt/independentreserve.py
--rw-rw-rw-   0        0        0    51921 2024-05-09 07:43:24.000000 ccxt-idax-adapter-4.3.25/ccxt/indodax.py
--rw-rw-rw-   0        0        0   125472 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/kraken.py
--rw-rw-rw-   0        0        0   116835 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/krakenfutures.py
--rw-rw-rw-   0        0        0   217738 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/kucoin.py
--rw-rw-rw-   0        0        0   124327 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/kucoinfutures.py
--rw-rw-rw-   0        0        0    95991 2024-05-09 07:43:41.000000 ccxt-idax-adapter-4.3.25/ccxt/kuna.py
--rw-rw-rw-   0        0        0    79197 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/latoken.py
--rw-rw-rw-   0        0        0   115175 2024-05-09 07:43:44.000000 ccxt-idax-adapter-4.3.25/ccxt/lbank.py
--rw-rw-rw-   0        0        0    45887 2024-05-09 07:43:45.000000 ccxt-idax-adapter-4.3.25/ccxt/luno.py
--rw-rw-rw-   0        0        0    51070 2024-05-09 07:43:45.000000 ccxt-idax-adapter-4.3.25/ccxt/lykke.py
--rw-rw-rw-   0        0        0    35339 2024-05-09 07:43:46.000000 ccxt-idax-adapter-4.3.25/ccxt/mercado.py
--rw-rw-rw-   0        0        0   240859 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/mexc.py
--rw-rw-rw-   0        0        0   108601 2024-05-09 07:43:58.000000 ccxt-idax-adapter-4.3.25/ccxt/ndax.py
--rw-rw-rw-   0        0        0    64240 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/novadax.py
--rw-rw-rw-   0        0        0    37860 2024-05-09 07:44:01.000000 ccxt-idax-adapter-4.3.25/ccxt/oceanex.py
--rw-rw-rw-   0        0        0   151151 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/okcoin.py
--rw-rw-rw-   0        0        0   377057 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/okx.py
--rw-rw-rw-   0        0        0    88113 2024-05-09 07:44:52.000000 ccxt-idax-adapter-4.3.25/ccxt/onetrading.py
--rw-rw-rw-   0        0        0    54213 2024-05-09 07:44:53.000000 ccxt-idax-adapter-4.3.25/ccxt/p2b.py
--rw-rw-rw-   0        0        0    24244 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/paymium.py
--rw-rw-rw-   0        0        0   220593 2024-05-14 02:14:32.000000 ccxt-idax-adapter-4.3.25/ccxt/phemex.py
--rw-rw-rw-   0        0        0   101991 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/poloniex.py
--rw-rw-rw-   0        0        0    77799 2024-05-09 07:45:14.000000 ccxt-idax-adapter-4.3.25/ccxt/poloniexfutures.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.405292 ccxt-idax-adapter-4.3.25/ccxt/pro/
--rw-rw-rw-   0        0        0     7201 2024-05-15 10:03:23.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/__init__.py
--rw-rw-rw-   0        0        0    27167 2024-05-09 08:11:45.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/alpaca.py
--rw-rw-rw-   0        0        0    35432 2024-05-09 08:11:46.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/ascendex.py
--rw-rw-rw-   0        0        0     1351 2024-05-09 08:11:46.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/bequant.py
--rw-rw-rw-   0        0        0   152488 2024-05-09 08:11:48.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/binance.py
--rw-rw-rw-   0        0        0      976 2024-05-09 08:11:48.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/binancecoinm.py
--rw-rw-rw-   0        0        0     2321 2024-05-09 08:11:48.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/binanceus.py
--rw-rw-rw-   0        0        0     1357 2024-05-09 08:11:48.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/binanceusdm.py
--rw-rw-rw-   0        0        0    42110 2024-05-09 08:11:49.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/bingx.py
--rw-rw-rw-   0        0        0     1181 2024-05-09 08:11:49.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/bitcoincom.py
--rw-rw-rw-   0        0        0    24826 2024-05-09 08:11:49.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/bitfinex.py
--rw-rw-rw-   0        0        0    42834 2024-05-08 04:04:46.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/bitfinex2.py
--rw-rw-rw-   0        0        0    72217 2024-05-09 08:11:50.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/bitget.py
--rw-rw-rw-   0        0        0    16799 2024-05-09 08:11:50.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/bithumb.py
--rw-rw-rw-   0        0        0    62382 2024-05-09 08:11:51.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/bitmart.py
--rw-rw-rw-   0        0        0    68956 2024-05-09 08:11:52.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/bitmex.py
--rw-rw-rw-   0        0        0    18724 2024-05-09 08:11:52.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/bitopro.py
--rw-rw-rw-   0        0        0      415 2024-05-09 08:11:52.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/bitpanda.py
--rw-rw-rw-   0        0        0    16448 2024-05-09 08:11:52.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/bitrue.py
--rw-rw-rw-   0        0        0    20886 2024-05-09 08:11:52.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/bitstamp.py
--rw-rw-rw-   0        0        0    56145 2024-05-08 04:04:46.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/bitvavo.py
--rw-rw-rw-   0        0        0    29560 2024-05-09 08:11:53.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/blockchaincom.py
--rw-rw-rw-   0        0        0    85098 2024-05-08 04:04:46.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/bybit.py
--rw-rw-rw-   0        0        0    58380 2024-05-09 08:11:53.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/cex.py
--rw-rw-rw-   0        0        0    29324 2024-05-09 08:11:54.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/coinbase.py
--rw-rw-rw-   0        0        0    25794 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/coinbaseinternational.py
--rw-rw-rw-   0        0        0    38945 2024-05-09 08:11:55.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/coinbasepro.py
--rw-rw-rw-   0        0        0     7789 2024-05-09 08:11:55.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/coincheck.py
--rw-rw-rw-   0        0        0    45042 2024-05-09 08:11:55.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/coinex.py
--rw-rw-rw-   0        0        0    15652 2024-05-09 08:11:55.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/coinone.py
--rw-rw-rw-   0        0        0    42643 2024-05-09 08:11:56.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/cryptocom.py
--rw-rw-rw-   0        0        0    22355 2024-05-09 08:11:56.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/currencycom.py
--rw-rw-rw-   0        0        0    41035 2024-05-09 08:11:57.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/deribit.py
--rw-rw-rw-   0        0        0    24527 2024-05-09 08:11:57.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/exmo.py
--rw-rw-rw-   0        0        0    52489 2024-05-09 08:11:58.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/gate.py
--rw-rw-rw-   0        0        0      391 2024-05-09 08:11:58.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/gateio.py
--rw-rw-rw-   0        0        0    36641 2024-05-09 08:11:58.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/gemini.py
--rw-rw-rw-   0        0        0    56284 2024-05-05 05:05:27.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/hitbtc.py
--rw-rw-rw-   0        0        0    21957 2024-05-09 08:11:59.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/hollaex.py
--rw-rw-rw-   0        0        0    96052 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/htx.py
--rw-rw-rw-   0        0        0      385 2024-05-09 08:11:59.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/huobi.py
--rw-rw-rw-   0        0        0    23174 2024-05-09 08:11:59.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/huobijp.py
--rw-rw-rw-   0        0        0    20791 2024-05-09 08:11:59.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/hyperliquid.py
--rw-rw-rw-   0        0        0    10082 2024-05-15 02:39:22.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/idax.py
--rw-rw-rw-   0        0        0    28282 2024-05-09 08:11:59.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/idex.py
--rw-rw-rw-   0        0        0    11179 2024-05-08 04:04:46.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/independentreserve.py
--rw-rw-rw-   0        0        0    60764 2024-05-08 04:04:46.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/kraken.py
--rw-rw-rw-   0        0        0    63917 2024-05-09 08:12:00.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/krakenfutures.py
--rw-rw-rw-   0        0        0    50705 2024-05-09 08:12:01.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/kucoin.py
--rw-rw-rw-   0        0        0    50026 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/kucoinfutures.py
--rw-rw-rw-   0        0        0    35105 2024-05-09 08:12:02.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/lbank.py
--rw-rw-rw-   0        0        0    12348 2024-05-09 08:12:02.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/luno.py
--rw-rw-rw-   0        0        0    43183 2024-05-09 08:12:03.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/mexc.py
--rw-rw-rw-   0        0        0    22643 2024-05-09 08:12:03.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/ndax.py
--rw-rw-rw-   0        0        0    30385 2024-05-09 08:12:03.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/okcoin.py
--rw-rw-rw-   0        0        0    72786 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/okx.py
--rw-rw-rw-   0        0        0    54634 2024-05-09 08:12:04.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/onetrading.py
--rw-rw-rw-   0        0        0    17877 2024-05-09 08:12:04.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/p2b.py
--rw-rw-rw-   0        0        0    61032 2024-05-09 08:12:05.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/phemex.py
--rw-rw-rw-   0        0        0    51235 2024-05-05 05:05:27.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/poloniex.py
--rw-rw-rw-   0        0        0    41652 2024-05-09 08:12:05.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/poloniexfutures.py
--rw-rw-rw-   0        0        0    22822 2024-05-09 08:12:06.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/probit.py
--rw-rw-rw-   0        0        0     9654 2024-05-09 08:12:06.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/upbit.py
--rw-rw-rw-   0        0        0    30043 2024-05-09 08:12:06.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/wazirx.py
--rw-rw-rw-   0        0        0    35021 2024-05-09 08:12:07.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/whitebit.py
--rw-rw-rw-   0        0        0    43584 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/woo.py
--rw-rw-rw-   0        0        0    48892 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/pro/woofipro.py
--rw-rw-rw-   0        0        0    76379 2024-05-09 07:45:18.000000 ccxt-idax-adapter-4.3.25/ccxt/probit.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.407347 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/
--rw-rw-rw-   0        0        0       84 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.426283 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/
--rw-rw-rw-   0        0        0      594 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/__init__.py
--rw-rw-rw-   0        0        0    18461 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/_version.py
--rw-rw-rw-   0        0        0     1886 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/curves.py
--rw-rw-rw-   0        0        0     6942 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/der.py
--rw-rw-rw-   0        0        0    11336 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/ecdsa.py
--rw-rw-rw-   0        0        0     5517 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/ellipticcurve.py
--rw-rw-rw-   0        0        0    14201 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/keys.py
--rw-rw-rw-   0        0        0    13468 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/numbertheory.py
--rw-rw-rw-   0        0        0     2572 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/rfc6979.py
--rw-rw-rw-   0        0        0    10037 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/util.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.427877 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/
--rw-rw-rw-   0        0        0      171 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.449120 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/
--rw-rw-rw-   0        0        0      276 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/__init__.py
--rw-rw-rw-   0        0        0      490 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/abi.py
--rw-rw-rw-   0        0        0     4861 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/base.py
--rw-rw-rw-   0        0        0     6871 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/codec.py
--rw-rw-rw-   0        0        0       51 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/constants.py
--rw-rw-rw-   0        0        0    16828 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/decoding.py
--rw-rw-rw-   0        0        0    20162 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/encoding.py
--rw-rw-rw-   0        0        0     2941 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/exceptions.py
--rw-rw-rw-   0        0        0    12358 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/grammar.py
--rw-rw-rw-   0        0        0      387 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/packed.py
--rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/py.typed
--rw-rw-rw-   0        0        0    19329 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/registry.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.453144 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/tools/
--rw-rw-rw-   0        0        0       65 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/tools/__init__.py
--rw-rw-rw-   0        0        0     5742 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.461785 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/utils/
--rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/utils/__init__.py
--rw-rw-rw-   0        0        0     2097 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/utils/numeric.py
--rw-rw-rw-   0        0        0      426 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/utils/padding.py
--rw-rw-rw-   0        0        0      436 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/utils/string.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.467499 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/account/
--rw-rw-rw-   0        0        0       48 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/account/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.474824 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/account/encode_typed_data/
--rw-rw-rw-   0        0        0       80 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/account/encode_typed_data/__init__.py
--rw-rw-rw-   0        0        0     7126 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py
--rw-rw-rw-   0        0        0      982 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py
--rw-rw-rw-   0        0        0    10588 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/account/messages.py
--rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/account/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.482370 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/hexbytes/
--rw-rw-rw-   0        0        0       60 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/hexbytes/__init__.py
--rw-rw-rw-   0        0        0     1687 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/hexbytes/_utils.py
--rw-rw-rw-   0        0        0     1768 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/hexbytes/main.py
--rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/hexbytes/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.502272 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/typing/
--rw-rw-rw-   0        0        0      913 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/typing/__init__.py
--rw-rw-rw-   0        0        0       85 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/typing/abi.py
--rw-rw-rw-   0        0        0      191 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/typing/bls.py
--rw-rw-rw-   0        0        0       71 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/typing/discovery.py
--rw-rw-rw-   0        0        0      117 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/typing/encoding.py
--rw-rw-rw-   0        0        0      458 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/typing/enums.py
--rw-rw-rw-   0        0        0      173 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/typing/ethpm.py
--rw-rw-rw-   0        0        0      546 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/typing/evm.py
--rw-rw-rw-   0        0        0    20845 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/typing/networks.py
--rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/typing/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.543561 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/
--rw-rw-rw-   0        0        0     2162 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/__init__.py
--rw-rw-rw-   0        0        0     2123 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/abi.py
--rw-rw-rw-   0        0        0     4364 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/address.py
--rw-rw-rw-   0        0        0     4342 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/applicators.py
--rw-rw-rw-   0        0        0     5498 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/conversions.py
--rw-rw-rw-   0        0        0     3021 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/currency.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.546162 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/curried/
--rw-rw-rw-   0        0        0     6398 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/curried/__init__.py
--rw-rw-rw-   0        0        0      499 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/debug.py
--rw-rw-rw-   0        0        0     3997 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/decorators.py
--rw-rw-rw-   0        0        0      199 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/encoding.py
--rw-rw-rw-   0        0        0      110 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/exceptions.py
--rw-rw-rw-   0        0        0     2100 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/functional.py
--rw-rw-rw-   0        0        0     1826 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/hexadecimal.py
--rw-rw-rw-   0        0        0     4137 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/humanize.py
--rw-rw-rw-   0        0        0     5155 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/logging.py
--rw-rw-rw-   0        0        0      842 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/module_loading.py
--rw-rw-rw-   0        0        0     1190 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/numeric.py
--rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/py.typed
--rw-rw-rw-   0        0        0     1001 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/toolz.py
--rw-rw-rw-   0        0        0     1074 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/types.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.550192 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/typing/
--rw-rw-rw-   0        0        0      325 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/typing/__init__.py
--rw-rw-rw-   0        0        0      189 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/typing/misc.py
--rw-rw-rw-   0        0        0     1757 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/units.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.553797 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/keccak/
--rw-rw-rw-   0        0        0       45 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/keccak/__init__.py
--rw-rw-rw-   0        0        0     6934 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/keccak/keccak.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.562840 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/msgpack/
--rw-rw-rw-   0        0        0     1077 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/msgpack/__init__.py
--rw-rw-rw-   0        0        0     1081 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/msgpack/exceptions.py
--rw-rw-rw-   0        0        0     5629 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/msgpack/ext.py
--rw-rw-rw-   0        0        0    33175 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/msgpack/fallback.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.577087 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/parsimonious/
--rw-rw-rw-   0        0        0      385 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/parsimonious/__init__.py
--rw-rw-rw-   0        0        0     3603 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/parsimonious/exceptions.py
--rw-rw-rw-   0        0        0    16864 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/parsimonious/expressions.py
--rw-rw-rw-   0        0        0    19190 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/parsimonious/grammar.py
--rw-rw-rw-   0        0        0    13084 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/parsimonious/nodes.py
--rw-rw-rw-   0        0        0     1087 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/parsimonious/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.598447 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/
--rw-rw-rw-   0        0        0      374 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/__init__.py
--rw-rw-rw-   0        0        0    20555 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/_signatures.py
--rw-rw-rw-   0        0        0    18447 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/_version.py
--rw-rw-rw-   0        0        0      997 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/compatibility.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.605081 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/curried/
--rw-rw-rw-   0        0        0     2226 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/curried/__init__.py
--rw-rw-rw-   0        0        0      344 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/curried/exceptions.py
--rw-rw-rw-   0        0        0      525 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/curried/operator.py
--rw-rw-rw-   0        0        0     8955 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/dicttoolz.py
--rw-rw-rw-   0        0        0    29821 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/functoolz.py
--rw-rw-rw-   0        0        0    27612 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/itertoolz.py
--rw-rw-rw-   0        0        0     1256 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/recipes.py
--rw-rw-rw-   0        0        0      139 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.611009 ccxt-idax-adapter-4.3.25/ccxt/test/
--rw-rw-rw-   0        0        0      141 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.681107 ccxt-idax-adapter-4.3.25/ccxt/test/base/
--rw-rw-rw-   0        0        0     1889 2024-05-15 10:05:05.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/__init__.py
--rw-rw-rw-   0        0        0      978 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_account.py
--rw-rw-rw-   0        0        0     2931 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_balance.py
--rw-rw-rw-   0        0        0     1808 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_borrow_interest.py
--rw-rw-rw-   0        0        0     1500 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_borrow_rate.py
--rw-rw-rw-   0        0        0     1177 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_calculate_fee.py
--rw-rw-rw-   0        0        0     7702 2024-05-15 10:05:03.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_crypto.py
--rw-rw-rw-   0        0        0     4472 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_currency.py
--rw-rw-rw-   0        0        0     5634 2024-05-15 10:05:03.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_datetime.py
--rw-rw-rw-   0        0        0    20934 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_decimal_to_precision.py
--rw-rw-rw-   0        0        0     1402 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_deep_extend.py
--rw-rw-rw-   0        0        0     2452 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_deposit_withdrawal.py
--rw-rw-rw-   0        0        0     3592 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_exchange_datetime_functions.py
--rw-rw-rw-   0        0        0     1351 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_funding_rate_history.py
--rw-rw-rw-   0        0        0     1332 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_last_price.py
--rw-rw-rw-   0        0        0     2289 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_ledger_entry.py
--rw-rw-rw-   0        0        0     2154 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_ledger_item.py
--rw-rw-rw-   0        0        0     1656 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_leverage_tier.py
--rw-rw-rw-   0        0        0      869 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_margin_mode.py
--rw-rw-rw-   0        0        0     1730 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_margin_modification.py
--rw-rw-rw-   0        0        0    11632 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_market.py
--rw-rw-rw-   0        0        0    22083 2024-05-15 10:05:03.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_number.py
--rw-rw-rw-   0        0        0     2036 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_ohlcv.py
--rw-rw-rw-   0        0        0     1547 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_open_interest.py
--rw-rw-rw-   0        0        0     3964 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_order.py
--rw-rw-rw-   0        0        0     3949 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_order_book.py
--rw-rw-rw-   0        0        0     3884 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_position.py
--rw-rw-rw-   0        0        0    19998 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_shared_methods.py
--rw-rw-rw-   0        0        0      722 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_status.py
--rw-rw-rw-   0        0        0     3123 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_throttle.py
--rw-rw-rw-   0        0        0     5810 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_ticker.py
--rw-rw-rw-   0        0        0     2336 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_trade.py
--rw-rw-rw-   0        0        0     1066 2024-05-15 10:05:40.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_trading_fee.py
--rw-rw-rw-   0        0        0     1434 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.25/ccxt/test/base/test_transaction.py
--rw-rw-rw-   0        0        0    80043 2024-05-15 10:05:05.000000 ccxt-idax-adapter-4.3.25/ccxt/test/test_async.py
--rw-rw-rw-   0        0        0    79000 2024-05-15 10:05:05.000000 ccxt-idax-adapter-4.3.25/ccxt/test/test_sync.py
--rw-rw-rw-   0        0        0    71287 2024-05-09 07:45:23.000000 ccxt-idax-adapter-4.3.25/ccxt/timex.py
--rw-rw-rw-   0        0        0   123013 2024-05-09 07:45:36.000000 ccxt-idax-adapter-4.3.25/ccxt/tokocrypto.py
--rw-rw-rw-   0        0        0    23900 2024-05-09 07:45:37.000000 ccxt-idax-adapter-4.3.25/ccxt/tradeogre.py
--rw-rw-rw-   0        0        0    81611 2024-05-09 07:45:41.000000 ccxt-idax-adapter-4.3.25/ccxt/upbit.py
--rw-rw-rw-   0        0        0   113603 2024-05-09 07:45:49.000000 ccxt-idax-adapter-4.3.25/ccxt/wavesexchange.py
--rw-rw-rw-   0        0        0    51342 2024-05-09 07:45:52.000000 ccxt-idax-adapter-4.3.25/ccxt/wazirx.py
--rw-rw-rw-   0        0        0   114402 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/whitebit.py
--rw-rw-rw-   0        0        0   139464 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/woo.py
--rw-rw-rw-   0        0        0   114867 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/woofipro.py
--rw-rw-rw-   0        0        0    53222 2024-05-09 07:46:07.000000 ccxt-idax-adapter-4.3.25/ccxt/yobit.py
--rw-rw-rw-   0        0        0    27979 2024-05-09 07:46:09.000000 ccxt-idax-adapter-4.3.25/ccxt/zaif.py
--rw-rw-rw-   0        0        0    80598 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.25/ccxt/zonda.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:27.694045 ccxt-idax-adapter-4.3.25/ccxt_idax_adapter.egg-info/
--rw-rw-rw-   0        0        0     2759 2024-05-15 10:08:26.000000 ccxt-idax-adapter-4.3.25/ccxt_idax_adapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    15934 2024-05-15 10:08:26.000000 ccxt-idax-adapter-4.3.25/ccxt_idax_adapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 10:08:26.000000 ccxt-idax-adapter-4.3.25/ccxt_idax_adapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      218 2024-05-15 10:08:26.000000 ccxt-idax-adapter-4.3.25/ccxt_idax_adapter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-15 10:08:26.000000 ccxt-idax-adapter-4.3.25/ccxt_idax_adapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12486 2024-05-15 10:08:14.000000 ccxt-idax-adapter-4.3.25/package.json
--rw-rw-rw-   0        0        0      226 2024-05-15 10:08:27.700065 ccxt-idax-adapter-4.3.25/setup.cfg
--rw-rw-rw-   0        0        0     3071 2024-05-09 09:58:59.000000 ccxt-idax-adapter-4.3.25/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.888776 ccxt-idax-adapter-4.3.26/
+-rw-rw-rw-   0        0        0     1068 2024-05-17 08:36:52.000000 ccxt-idax-adapter-4.3.26/LICENSE.txt
+-rw-rw-rw-   0        0        0      101 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.26/MANIFEST.in
+-rw-rw-rw-   0        0        0     2821 2024-05-17 08:41:31.887777 ccxt-idax-adapter-4.3.26/PKG-INFO
+-rw-rw-rw-   0        0        0   102253 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.26/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.365562 ccxt-idax-adapter-4.3.26/ccxt/
+-rw-rw-rw-   0        0        0    15933 2024-05-17 08:36:26.000000 ccxt-idax-adapter-4.3.26/ccxt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.477539 ccxt-idax-adapter-4.3.26/ccxt/abstract/
+-rw-rw-rw-   0        0        0        0 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/__init__.py
+-rw-rw-rw-   0        0        0     1448 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/ace.py
+-rw-rw-rw-   0        0        0    10382 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/alpaca.py
+-rw-rw-rw-   0        0        0    11394 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/ascendex.py
+-rw-rw-rw-   0        0        0    15601 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bequant.py
+-rw-rw-rw-   0        0        0     4895 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bigone.py
+-rw-rw-rw-   0        0        0    92208 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/binance.py
+-rw-rw-rw-   0        0        0    92208 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/binancecoinm.py
+-rw-rw-rw-   0        0        0    98928 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/binanceus.py
+-rw-rw-rw-   0        0        0    92208 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/binanceusdm.py
+-rw-rw-rw-   0        0        0    16032 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bingx.py
+-rw-rw-rw-   0        0        0     2830 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bit2c.py
+-rw-rw-rw-   0        0        0     2735 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bitbank.py
+-rw-rw-rw-   0        0        0     5820 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bitbay.py
+-rw-rw-rw-   0        0        0     4082 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bitbns.py
+-rw-rw-rw-   0        0        0    15601 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bitcoincom.py
+-rw-rw-rw-   0        0        0     7605 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bitfinex.py
+-rw-rw-rw-   0        0        0    19194 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bitfinex2.py
+-rw-rw-rw-   0        0        0     3576 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bitflyer.py
+-rw-rw-rw-   0        0        0    90336 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bitget.py
+-rw-rw-rw-   0        0        0     3443 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bithumb.py
+-rw-rw-rw-   0        0        0    14031 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bitmart.py
+-rw-rw-rw-   0        0        0    10774 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bitmex.py
+-rw-rw-rw-   0        0        0     3295 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bitopro.py
+-rw-rw-rw-   0        0        0     3859 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bitpanda.py
+-rw-rw-rw-   0        0        0     9379 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bitrue.py
+-rw-rw-rw-   0        0        0     4025 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bitso.py
+-rw-rw-rw-   0        0        0    27930 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bitstamp.py
+-rw-rw-rw-   0        0        0     3478 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bitteam.py
+-rw-rw-rw-   0        0        0     2357 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bitvavo.py
+-rw-rw-rw-   0        0        0     2024 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bl3p.py
+-rw-rw-rw-   0        0        0     2638 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/blockchaincom.py
+-rw-rw-rw-   0        0        0     4217 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/blofin.py
+-rw-rw-rw-   0        0        0     1380 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/btcalpha.py
+-rw-rw-rw-   0        0        0      849 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/btcbox.py
+-rw-rw-rw-   0        0        0     3690 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/btcmarkets.py
+-rw-rw-rw-   0        0        0     1777 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/btcturk.py
+-rw-rw-rw-   0        0        0    48923 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/bybit.py
+-rw-rw-rw-   0        0        0     3311 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/cex.py
+-rw-rw-rw-   0        0        0    15507 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/coinbase.py
+-rw-rw-rw-   0        0        0     4770 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/coinbaseinternational.py
+-rw-rw-rw-   0        0        0     7162 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/coinbasepro.py
+-rw-rw-rw-   0        0        0     3417 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/coincheck.py
+-rw-rw-rw-   0        0        0    34678 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/coinex.py
+-rw-rw-rw-   0        0        0     6538 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/coinlist.py
+-rw-rw-rw-   0        0        0     6842 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/coinmate.py
+-rw-rw-rw-   0        0        0     3975 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/coinmetro.py
+-rw-rw-rw-   0        0        0     8291 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/coinone.py
+-rw-rw-rw-   0        0        0     8007 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/coinsph.py
+-rw-rw-rw-   0        0        0     2707 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/coinspot.py
+-rw-rw-rw-   0        0        0    18475 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/cryptocom.py
+-rw-rw-rw-   0        0        0     7563 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/currencycom.py
+-rw-rw-rw-   0        0        0     5107 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/delta.py
+-rw-rw-rw-   0        0        0    15499 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/deribit.py
+-rw-rw-rw-   0        0        0    11452 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/digifinex.py
+-rw-rw-rw-   0        0        0     6177 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/exmo.py
+-rw-rw-rw-   0        0        0    15601 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/fmfwio.py
+-rw-rw-rw-   0        0        0    41994 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/gate.py
+-rw-rw-rw-   0        0        0    41994 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/gateio.py
+-rw-rw-rw-   0        0        0     6915 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/gemini.py
+-rw-rw-rw-   0        0        0    15601 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/hitbtc.py
+-rw-rw-rw-   0        0        0    15601 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/hitbtc3.py
+-rw-rw-rw-   0        0        0     2906 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/hollaex.py
+-rw-rw-rw-   0        0        0    99311 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/htx.py
+-rw-rw-rw-   0        0        0    99311 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/huobi.py
+-rw-rw-rw-   0        0        0    14331 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/huobijp.py
+-rw-rw-rw-   0        0        0      240 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/hyperliquid.py
+-rw-rw-rw-   0        0        0     1743 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/idax.py
+-rw-rw-rw-   0        0        0     2129 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/idex.py
+-rw-rw-rw-   0        0        0     4165 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/independentreserve.py
+-rw-rw-rw-   0        0        0     2488 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/indodax.py
+-rw-rw-rw-   0        0        0     5877 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/kraken.py
+-rw-rw-rw-   0        0        0     3537 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/krakenfutures.py
+-rw-rw-rw-   0        0        0    25491 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/kucoin.py
+-rw-rw-rw-   0        0        0    28204 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/kucoinfutures.py
+-rw-rw-rw-   0        0        0    24579 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/kuna.py
+-rw-rw-rw-   0        0        0     7168 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/latoken.py
+-rw-rw-rw-   0        0        0     8675 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/lbank.py
+-rw-rw-rw-   0        0        0     3619 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/luno.py
+-rw-rw-rw-   0        0        0     2960 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/lykke.py
+-rw-rw-rw-   0        0        0     2357 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/mercado.py
+-rw-rw-rw-   0        0        0    25902 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/mexc.py
+-rw-rw-rw-   0        0        0    11878 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/ndax.py
+-rw-rw-rw-   0        0        0     3093 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/novadax.py
+-rw-rw-rw-   0        0        0     1721 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/oceanex.py
+-rw-rw-rw-   0        0        0     9414 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/okcoin.py
+-rw-rw-rw-   0        0        0    46458 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/okx.py
+-rw-rw-rw-   0        0        0     3859 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/onetrading.py
+-rw-rw-rw-   0        0        0     2054 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/p2b.py
+-rw-rw-rw-   0        0        0     2843 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/paymium.py
+-rw-rw-rw-   0        0        0    15203 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/phemex.py
+-rw-rw-rw-   0        0        0     8073 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/poloniex.py
+-rw-rw-rw-   0        0        0     5219 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/poloniexfutures.py
+-rw-rw-rw-   0        0        0     1969 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/probit.py
+-rw-rw-rw-   0        0        0     5875 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/timex.py
+-rw-rw-rw-   0        0        0     4094 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/tokocrypto.py
+-rw-rw-rw-   0        0        0     1372 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/tradeogre.py
+-rw-rw-rw-   0        0        0     3576 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/upbit.py
+-rw-rw-rw-   0        0        0    19631 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/wavesexchange.py
+-rw-rw-rw-   0        0        0     2782 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/wazirx.py
+-rw-rw-rw-   0        0        0    10977 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/whitebit.py
+-rw-rw-rw-   0        0        0    10368 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/woo.py
+-rw-rw-rw-   0        0        0    16016 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/woofipro.py
+-rw-rw-rw-   0        0        0     1339 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/yobit.py
+-rw-rw-rw-   0        0        0     3935 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/zaif.py
+-rw-rw-rw-   0        0        0     5820 2024-05-17 08:36:43.000000 ccxt-idax-adapter-4.3.26/ccxt/abstract/zonda.py
+-rw-rw-rw-   0        0        0    41656 2024-05-09 07:22:32.000000 ccxt-idax-adapter-4.3.26/ccxt/ace.py
+-rw-rw-rw-   0        0        0    47215 2024-05-05 05:05:27.000000 ccxt-idax-adapter-4.3.26/ccxt/alpaca.py
+-rw-rw-rw-   0        0        0   151471 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/ascendex.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.605944 ccxt-idax-adapter-4.3.26/ccxt/async_support/
+-rw-rw-rw-   0        0        0    15706 2024-05-17 08:36:26.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/__init__.py
+-rw-rw-rw-   0        0        0    41880 2024-05-09 07:22:32.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/ace.py
+-rw-rw-rw-   0        0        0    47427 2024-05-05 05:05:27.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/alpaca.py
+-rw-rw-rw-   0        0        0   152259 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/ascendex.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.609375 ccxt-idax-adapter-4.3.26/ccxt/async_support/base/
+-rw-rw-rw-   0        0        0       67 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/base/__init__.py
+-rw-rw-rw-   0        0        0   108636 2024-05-17 08:37:42.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/base/exchange.py
+-rw-rw-rw-   0        0        0     1847 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/base/throttler.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.619464 ccxt-idax-adapter-4.3.26/ccxt/async_support/base/ws/
+-rw-rw-rw-   0        0        0     1791 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/base/ws/__init__.py
+-rw-rw-rw-   0        0        0     5751 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/base/ws/aiohttp_client.py
+-rw-rw-rw-   0        0        0     8100 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/base/ws/cache.py
+-rw-rw-rw-   0        0        0     7289 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/base/ws/client.py
+-rw-rw-rw-   0        0        0     3864 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/base/ws/fast_client.py
+-rw-rw-rw-   0        0        0     1499 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/base/ws/functions.py
+-rw-rw-rw-   0        0        0     2067 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/base/ws/future.py
+-rw-rw-rw-   0        0        0     2894 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/base/ws/order_book.py
+-rw-rw-rw-   0        0        0     6478 2024-05-03 06:32:44.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/base/ws/order_book_side.py
+-rw-rw-rw-   0        0        0     1188 2024-05-09 07:22:35.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bequant.py
+-rw-rw-rw-   0        0        0    92663 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bigone.py
+-rw-rw-rw-   0        0        0   620262 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/binance.py
+-rw-rw-rw-   0        0        0     1683 2024-05-09 07:23:11.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/binancecoinm.py
+-rw-rw-rw-   0        0        0     9177 2024-05-09 07:23:12.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/binanceus.py
+-rw-rw-rw-   0        0        0     2518 2024-05-09 07:23:12.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/binanceusdm.py
+-rw-rw-rw-   0        0        0   185869 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bingx.py
+-rw-rw-rw-   0        0        0    37119 2024-05-09 07:23:14.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bit2c.py
+-rw-rw-rw-   0        0        0    42105 2024-05-09 07:23:15.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bitbank.py
+-rw-rw-rw-   0        0        0      492 2024-05-09 07:23:15.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bitbay.py
+-rw-rw-rw-   0        0        0    48391 2024-05-09 07:23:16.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bitbns.py
+-rw-rw-rw-   0        0        0      516 2024-05-09 07:23:16.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bitcoincom.py
+-rw-rw-rw-   0        0        0    72718 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bitfinex.py
+-rw-rw-rw-   0        0        0   159249 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bitfinex2.py
+-rw-rw-rw-   0        0        0    41705 2024-05-09 07:23:21.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bitflyer.py
+-rw-rw-rw-   0        0        0   424141 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bitget.py
+-rw-rw-rw-   0        0        0    45764 2024-05-09 07:23:59.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bithumb.py
+-rw-rw-rw-   0        0        0   200057 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bitmart.py
+-rw-rw-rw-   0        0        0   127162 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bitmex.py
+-rw-rw-rw-   0        0        0    68926 2024-05-09 07:24:20.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bitopro.py
+-rw-rw-rw-   0        0        0      485 2024-05-09 07:24:20.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bitpanda.py
+-rw-rw-rw-   0        0        0   136878 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bitrue.py
+-rw-rw-rw-   0        0        0    71271 2024-05-09 07:24:31.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bitso.py
+-rw-rw-rw-   0        0        0    92735 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bitstamp.py
+-rw-rw-rw-   0        0        0   102358 2024-05-09 07:24:44.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bitteam.py
+-rw-rw-rw-   0        0        0    92011 2024-05-09 07:24:49.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bitvavo.py
+-rw-rw-rw-   0        0        0    20611 2024-05-09 07:24:50.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bl3p.py
+-rw-rw-rw-   0        0        0    49191 2024-05-09 07:24:52.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/blockchaincom.py
+-rw-rw-rw-   0        0        0    99837 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/blofin.py
+-rw-rw-rw-   0        0        0    36979 2024-05-09 07:24:58.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/btcalpha.py
+-rw-rw-rw-   0        0        0    23686 2024-05-09 07:24:59.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/btcbox.py
+-rw-rw-rw-   0        0        0    51834 2024-05-09 07:25:01.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/btcmarkets.py
+-rw-rw-rw-   0        0        0    36875 2024-05-09 07:25:02.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/btcturk.py
+-rw-rw-rw-   0        0        0   414323 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/bybit.py
+-rw-rw-rw-   0        0        0    70280 2024-05-09 07:25:37.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/cex.py
+-rw-rw-rw-   0        0        0   213105 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/coinbase.py
+-rw-rw-rw-   0        0        0    87794 2024-05-05 05:05:27.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/coinbaseinternational.py
+-rw-rw-rw-   0        0        0    79177 2024-05-09 07:25:53.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/coinbasepro.py
+-rw-rw-rw-   0        0        0    35870 2024-05-09 07:25:56.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/coincheck.py
+-rw-rw-rw-   0        0        0   260077 2024-05-14 02:14:32.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/coinex.py
+-rw-rw-rw-   0        0        0   103628 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/coinlist.py
+-rw-rw-rw-   0        0        0    46212 2024-05-09 07:26:16.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/coinmate.py
+-rw-rw-rw-   0        0        0    81020 2024-05-09 07:26:20.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/coinmetro.py
+-rw-rw-rw-   0        0        0    47138 2024-05-09 07:26:23.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/coinone.py
+-rw-rw-rw-   0        0        0    91066 2024-05-09 07:26:29.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/coinsph.py
+-rw-rw-rw-   0        0        0    23766 2024-05-09 07:26:30.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/coinspot.py
+-rw-rw-rw-   0        0        0   130329 2024-05-09 07:26:38.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/cryptocom.py
+-rw-rw-rw-   0        0        0    87236 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/currencycom.py
+-rw-rw-rw-   0        0        0   151119 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/delta.py
+-rw-rw-rw-   0        0        0   161375 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/deribit.py
+-rw-rw-rw-   0        0        0   169017 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/digifinex.py
+-rw-rw-rw-   0        0        0   115087 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/exmo.py
+-rw-rw-rw-   0        0        0     1250 2024-05-09 07:27:10.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/fmfwio.py
+-rw-rw-rw-   0        0        0   321536 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/gate.py
+-rw-rw-rw-   0        0        0      459 2024-05-09 07:27:31.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/gateio.py
+-rw-rw-rw-   0        0        0    81171 2024-05-09 07:27:36.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/gemini.py
+-rw-rw-rw-   0        0        0   154094 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/hitbtc.py
+-rw-rw-rw-   0        0        0      469 2024-05-09 07:27:46.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/hitbtc3.py
+-rw-rw-rw-   0        0        0    76379 2024-05-09 07:27:48.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/hollaex.py
+-rw-rw-rw-   0        0        0   422813 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/htx.py
+-rw-rw-rw-   0        0        0      452 2024-05-09 07:28:52.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/huobi.py
+-rw-rw-rw-   0        0        0    88468 2024-05-09 07:28:56.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/huobijp.py
+-rw-rw-rw-   0        0        0   101215 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/hyperliquid.py
+-rw-rw-rw-   0        0        0    24209 2024-05-17 08:37:40.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/idax.py
+-rw-rw-rw-   0        0        0    73474 2024-05-09 07:43:23.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/idex.py
+-rw-rw-rw-   0        0        0    32435 2024-05-09 07:43:23.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/independentreserve.py
+-rw-rw-rw-   0        0        0    52229 2024-05-09 07:43:24.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/indodax.py
+-rw-rw-rw-   0        0        0   126074 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/kraken.py
+-rw-rw-rw-   0        0        0   117323 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/krakenfutures.py
+-rw-rw-rw-   0        0        0   218810 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/kucoin.py
+-rw-rw-rw-   0        0        0   124965 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/kucoinfutures.py
+-rw-rw-rw-   0        0        0    96407 2024-05-09 07:43:41.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/kuna.py
+-rw-rw-rw-   0        0        0    79673 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/latoken.py
+-rw-rw-rw-   0        0        0   115887 2024-05-09 07:43:44.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/lbank.py
+-rw-rw-rw-   0        0        0    46225 2024-05-09 07:43:45.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/luno.py
+-rw-rw-rw-   0        0        0    51384 2024-05-09 07:43:45.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/lykke.py
+-rw-rw-rw-   0        0        0    35581 2024-05-09 07:43:46.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/mercado.py
+-rw-rw-rw-   0        0        0   242037 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/mexc.py
+-rw-rw-rw-   0        0        0   109125 2024-05-09 07:43:58.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/ndax.py
+-rw-rw-rw-   0        0        0    64608 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/novadax.py
+-rw-rw-rw-   0        0        0    38180 2024-05-09 07:44:01.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/oceanex.py
+-rw-rw-rw-   0        0        0   151675 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/okcoin.py
+-rw-rw-rw-   0        0        0   378644 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/okx.py
+-rw-rw-rw-   0        0        0    88565 2024-05-09 07:44:52.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/onetrading.py
+-rw-rw-rw-   0        0        0    54455 2024-05-09 07:44:53.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/p2b.py
+-rw-rw-rw-   0        0        0    24432 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/paymium.py
+-rw-rw-rw-   0        0        0   221405 2024-05-14 02:14:32.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/phemex.py
+-rw-rw-rw-   0        0        0   102539 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/poloniex.py
+-rw-rw-rw-   0        0        0    78185 2024-05-09 07:45:14.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/poloniexfutures.py
+-rw-rw-rw-   0        0        0    76771 2024-05-09 07:45:18.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/probit.py
+-rw-rw-rw-   0        0        0    71649 2024-05-09 07:45:23.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/timex.py
+-rw-rw-rw-   0        0        0   123375 2024-05-09 07:45:36.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/tokocrypto.py
+-rw-rw-rw-   0        0        0    24094 2024-05-09 07:45:37.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/tradeogre.py
+-rw-rw-rw-   0        0        0    82093 2024-05-09 07:45:41.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/upbit.py
+-rw-rw-rw-   0        0        0   114153 2024-05-09 07:45:49.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/wavesexchange.py
+-rw-rw-rw-   0        0        0    51644 2024-05-09 07:45:52.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/wazirx.py
+-rw-rw-rw-   0        0        0   115022 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/whitebit.py
+-rw-rw-rw-   0        0        0   140354 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/woo.py
+-rw-rw-rw-   0        0        0   115547 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/woofipro.py
+-rw-rw-rw-   0        0        0    53506 2024-05-09 07:46:07.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/yobit.py
+-rw-rw-rw-   0        0        0    28161 2024-05-09 07:46:09.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/zaif.py
+-rw-rw-rw-   0        0        0    80912 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/async_support/zonda.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.625967 ccxt-idax-adapter-4.3.26/ccxt/base/
+-rw-rw-rw-   0        0        0     1320 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/base/__init__.py
+-rw-rw-rw-   0        0        0     6634 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/base/decimal_to_precision.py
+-rw-rw-rw-   0        0        0     4264 2024-05-17 08:37:42.000000 ccxt-idax-adapter-4.3.26/ccxt/base/errors.py
+-rw-rw-rw-   0        0        0   278172 2024-05-17 08:37:42.000000 ccxt-idax-adapter-4.3.26/ccxt/base/exchange.py
+-rw-rw-rw-   0        0        0     8565 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/base/precise.py
+-rw-rw-rw-   0        0        0     9027 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/base/types.py
+-rw-rw-rw-   0        0        0     1174 2024-05-09 07:22:35.000000 ccxt-idax-adapter-4.3.26/ccxt/bequant.py
+-rw-rw-rw-   0        0        0    92209 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/bigone.py
+-rw-rw-rw-   0        0        0   617552 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/binance.py
+-rw-rw-rw-   0        0        0     1645 2024-05-09 07:23:11.000000 ccxt-idax-adapter-4.3.26/ccxt/binancecoinm.py
+-rw-rw-rw-   0        0        0     9163 2024-05-09 07:23:12.000000 ccxt-idax-adapter-4.3.26/ccxt/binanceus.py
+-rw-rw-rw-   0        0        0     2480 2024-05-09 07:23:12.000000 ccxt-idax-adapter-4.3.26/ccxt/binanceusdm.py
+-rw-rw-rw-   0        0        0   184833 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/bingx.py
+-rw-rw-rw-   0        0        0    36907 2024-05-09 07:23:14.000000 ccxt-idax-adapter-4.3.26/ccxt/bit2c.py
+-rw-rw-rw-   0        0        0    41845 2024-05-09 07:23:15.000000 ccxt-idax-adapter-4.3.26/ccxt/bitbank.py
+-rw-rw-rw-   0        0        0      478 2024-05-09 07:23:15.000000 ccxt-idax-adapter-4.3.26/ccxt/bitbay.py
+-rw-rw-rw-   0        0        0    48137 2024-05-09 07:23:16.000000 ccxt-idax-adapter-4.3.26/ccxt/bitbns.py
+-rw-rw-rw-   0        0        0      502 2024-05-09 07:23:16.000000 ccxt-idax-adapter-4.3.26/ccxt/bitcoincom.py
+-rw-rw-rw-   0        0        0    72278 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/bitfinex.py
+-rw-rw-rw-   0        0        0   158515 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/bitfinex2.py
+-rw-rw-rw-   0        0        0    41397 2024-05-09 07:23:21.000000 ccxt-idax-adapter-4.3.26/ccxt/bitflyer.py
+-rw-rw-rw-   0        0        0   422517 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/bitget.py
+-rw-rw-rw-   0        0        0    45534 2024-05-09 07:23:59.000000 ccxt-idax-adapter-4.3.26/ccxt/bithumb.py
+-rw-rw-rw-   0        0        0   199137 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/bitmart.py
+-rw-rw-rw-   0        0        0   126584 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/bitmex.py
+-rw-rw-rw-   0        0        0    68522 2024-05-09 07:24:20.000000 ccxt-idax-adapter-4.3.26/ccxt/bitopro.py
+-rw-rw-rw-   0        0        0      471 2024-05-09 07:24:20.000000 ccxt-idax-adapter-4.3.26/ccxt/bitpanda.py
+-rw-rw-rw-   0        0        0   136220 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/bitrue.py
+-rw-rw-rw-   0        0        0    70885 2024-05-09 07:24:31.000000 ccxt-idax-adapter-4.3.26/ccxt/bitso.py
+-rw-rw-rw-   0        0        0    92235 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/bitstamp.py
+-rw-rw-rw-   0        0        0   102026 2024-05-09 07:24:44.000000 ccxt-idax-adapter-4.3.26/ccxt/bitteam.py
+-rw-rw-rw-   0        0        0    91577 2024-05-09 07:24:49.000000 ccxt-idax-adapter-4.3.26/ccxt/bitvavo.py
+-rw-rw-rw-   0        0        0    20483 2024-05-09 07:24:50.000000 ccxt-idax-adapter-4.3.26/ccxt/bl3p.py
+-rw-rw-rw-   0        0        0    48799 2024-05-09 07:24:52.000000 ccxt-idax-adapter-4.3.26/ccxt/blockchaincom.py
+-rw-rw-rw-   0        0        0    99253 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/blofin.py
+-rw-rw-rw-   0        0        0    36701 2024-05-09 07:24:58.000000 ccxt-idax-adapter-4.3.26/ccxt/btcalpha.py
+-rw-rw-rw-   0        0        0    23492 2024-05-09 07:24:59.000000 ccxt-idax-adapter-4.3.26/ccxt/btcbox.py
+-rw-rw-rw-   0        0        0    51484 2024-05-09 07:25:01.000000 ccxt-idax-adapter-4.3.26/ccxt/btcmarkets.py
+-rw-rw-rw-   0        0        0    36657 2024-05-09 07:25:02.000000 ccxt-idax-adapter-4.3.26/ccxt/btcturk.py
+-rw-rw-rw-   0        0        0   412519 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/bybit.py
+-rw-rw-rw-   0        0        0    69930 2024-05-09 07:25:37.000000 ccxt-idax-adapter-4.3.26/ccxt/cex.py
+-rw-rw-rw-   0        0        0   211999 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/coinbase.py
+-rw-rw-rw-   0        0        0    87240 2024-05-05 05:05:27.000000 ccxt-idax-adapter-4.3.26/ccxt/coinbaseinternational.py
+-rw-rw-rw-   0        0        0    78671 2024-05-09 07:25:53.000000 ccxt-idax-adapter-4.3.26/ccxt/coinbasepro.py
+-rw-rw-rw-   0        0        0    35664 2024-05-09 07:25:56.000000 ccxt-idax-adapter-4.3.26/ccxt/coincheck.py
+-rw-rw-rw-   0        0        0   258783 2024-05-14 02:14:32.000000 ccxt-idax-adapter-4.3.26/ccxt/coinex.py
+-rw-rw-rw-   0        0        0   103140 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/coinlist.py
+-rw-rw-rw-   0        0        0    45946 2024-05-09 07:26:16.000000 ccxt-idax-adapter-4.3.26/ccxt/coinmate.py
+-rw-rw-rw-   0        0        0    80700 2024-05-09 07:26:20.000000 ccxt-idax-adapter-4.3.26/ccxt/coinmetro.py
+-rw-rw-rw-   0        0        0    46896 2024-05-09 07:26:23.000000 ccxt-idax-adapter-4.3.26/ccxt/coinone.py
+-rw-rw-rw-   0        0        0    90632 2024-05-09 07:26:29.000000 ccxt-idax-adapter-4.3.26/ccxt/coinsph.py
+-rw-rw-rw-   0        0        0    23614 2024-05-09 07:26:30.000000 ccxt-idax-adapter-4.3.26/ccxt/coinspot.py
+-rw-rw-rw-   0        0        0   129757 2024-05-09 07:26:38.000000 ccxt-idax-adapter-4.3.26/ccxt/cryptocom.py
+-rw-rw-rw-   0        0        0    86814 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/currencycom.py
+-rw-rw-rw-   0        0        0   150511 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/delta.py
+-rw-rw-rw-   0        0        0   160599 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/deribit.py
+-rw-rw-rw-   0        0        0   168047 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/digifinex.py
+-rw-rw-rw-   0        0        0   114455 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/exmo.py
+-rw-rw-rw-   0        0        0     1236 2024-05-09 07:27:10.000000 ccxt-idax-adapter-4.3.26/ccxt/fmfwio.py
+-rw-rw-rw-   0        0        0   319858 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/gate.py
+-rw-rw-rw-   0        0        0      445 2024-05-09 07:27:31.000000 ccxt-idax-adapter-4.3.26/ccxt/gateio.py
+-rw-rw-rw-   0        0        0    80658 2024-05-09 07:27:36.000000 ccxt-idax-adapter-4.3.26/ccxt/gemini.py
+-rw-rw-rw-   0        0        0   153048 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/hitbtc.py
+-rw-rw-rw-   0        0        0      455 2024-05-09 07:27:46.000000 ccxt-idax-adapter-4.3.26/ccxt/hitbtc3.py
+-rw-rw-rw-   0        0        0    75945 2024-05-09 07:27:48.000000 ccxt-idax-adapter-4.3.26/ccxt/hollaex.py
+-rw-rw-rw-   0        0        0   420457 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/htx.py
+-rw-rw-rw-   0        0        0      438 2024-05-09 07:28:52.000000 ccxt-idax-adapter-4.3.26/ccxt/huobi.py
+-rw-rw-rw-   0        0        0    87968 2024-05-09 07:28:56.000000 ccxt-idax-adapter-4.3.26/ccxt/huobijp.py
+-rw-rw-rw-   0        0        0   100695 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/hyperliquid.py
+-rw-rw-rw-   0        0        0    23917 2024-05-17 08:37:40.000000 ccxt-idax-adapter-4.3.26/ccxt/idax.py
+-rw-rw-rw-   0        0        0    72998 2024-05-09 07:43:23.000000 ccxt-idax-adapter-4.3.26/ccxt/idex.py
+-rw-rw-rw-   0        0        0    32175 2024-05-09 07:43:23.000000 ccxt-idax-adapter-4.3.26/ccxt/independentreserve.py
+-rw-rw-rw-   0        0        0    51921 2024-05-09 07:43:24.000000 ccxt-idax-adapter-4.3.26/ccxt/indodax.py
+-rw-rw-rw-   0        0        0   125472 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/kraken.py
+-rw-rw-rw-   0        0        0   116835 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/krakenfutures.py
+-rw-rw-rw-   0        0        0   217738 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/kucoin.py
+-rw-rw-rw-   0        0        0   124327 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/kucoinfutures.py
+-rw-rw-rw-   0        0        0    95991 2024-05-09 07:43:41.000000 ccxt-idax-adapter-4.3.26/ccxt/kuna.py
+-rw-rw-rw-   0        0        0    79197 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/latoken.py
+-rw-rw-rw-   0        0        0   115175 2024-05-09 07:43:44.000000 ccxt-idax-adapter-4.3.26/ccxt/lbank.py
+-rw-rw-rw-   0        0        0    45887 2024-05-09 07:43:45.000000 ccxt-idax-adapter-4.3.26/ccxt/luno.py
+-rw-rw-rw-   0        0        0    51070 2024-05-09 07:43:45.000000 ccxt-idax-adapter-4.3.26/ccxt/lykke.py
+-rw-rw-rw-   0        0        0    35339 2024-05-09 07:43:46.000000 ccxt-idax-adapter-4.3.26/ccxt/mercado.py
+-rw-rw-rw-   0        0        0   240859 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/mexc.py
+-rw-rw-rw-   0        0        0   108601 2024-05-09 07:43:58.000000 ccxt-idax-adapter-4.3.26/ccxt/ndax.py
+-rw-rw-rw-   0        0        0    64240 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/novadax.py
+-rw-rw-rw-   0        0        0    37860 2024-05-09 07:44:01.000000 ccxt-idax-adapter-4.3.26/ccxt/oceanex.py
+-rw-rw-rw-   0        0        0   151151 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/okcoin.py
+-rw-rw-rw-   0        0        0   377057 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/okx.py
+-rw-rw-rw-   0        0        0    88113 2024-05-09 07:44:52.000000 ccxt-idax-adapter-4.3.26/ccxt/onetrading.py
+-rw-rw-rw-   0        0        0    54213 2024-05-09 07:44:53.000000 ccxt-idax-adapter-4.3.26/ccxt/p2b.py
+-rw-rw-rw-   0        0        0    24244 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/paymium.py
+-rw-rw-rw-   0        0        0   220593 2024-05-14 02:14:32.000000 ccxt-idax-adapter-4.3.26/ccxt/phemex.py
+-rw-rw-rw-   0        0        0   101991 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/poloniex.py
+-rw-rw-rw-   0        0        0    77799 2024-05-09 07:45:14.000000 ccxt-idax-adapter-4.3.26/ccxt/poloniexfutures.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.701923 ccxt-idax-adapter-4.3.26/ccxt/pro/
+-rw-rw-rw-   0        0        0     7201 2024-05-17 08:36:26.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/__init__.py
+-rw-rw-rw-   0        0        0    27167 2024-05-09 08:11:45.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/alpaca.py
+-rw-rw-rw-   0        0        0    35432 2024-05-09 08:11:46.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/ascendex.py
+-rw-rw-rw-   0        0        0     1351 2024-05-09 08:11:46.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/bequant.py
+-rw-rw-rw-   0        0        0   152488 2024-05-09 08:11:48.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/binance.py
+-rw-rw-rw-   0        0        0      976 2024-05-09 08:11:48.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/binancecoinm.py
+-rw-rw-rw-   0        0        0     2321 2024-05-09 08:11:48.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/binanceus.py
+-rw-rw-rw-   0        0        0     1357 2024-05-09 08:11:48.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/binanceusdm.py
+-rw-rw-rw-   0        0        0    42110 2024-05-09 08:11:49.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/bingx.py
+-rw-rw-rw-   0        0        0     1181 2024-05-09 08:11:49.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/bitcoincom.py
+-rw-rw-rw-   0        0        0    24826 2024-05-09 08:11:49.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/bitfinex.py
+-rw-rw-rw-   0        0        0    42834 2024-05-08 04:04:46.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/bitfinex2.py
+-rw-rw-rw-   0        0        0    72217 2024-05-09 08:11:50.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/bitget.py
+-rw-rw-rw-   0        0        0    16799 2024-05-09 08:11:50.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/bithumb.py
+-rw-rw-rw-   0        0        0    62382 2024-05-09 08:11:51.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/bitmart.py
+-rw-rw-rw-   0        0        0    68956 2024-05-09 08:11:52.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/bitmex.py
+-rw-rw-rw-   0        0        0    18724 2024-05-09 08:11:52.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/bitopro.py
+-rw-rw-rw-   0        0        0      415 2024-05-09 08:11:52.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/bitpanda.py
+-rw-rw-rw-   0        0        0    16448 2024-05-09 08:11:52.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/bitrue.py
+-rw-rw-rw-   0        0        0    20886 2024-05-09 08:11:52.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/bitstamp.py
+-rw-rw-rw-   0        0        0    56145 2024-05-08 04:04:46.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/bitvavo.py
+-rw-rw-rw-   0        0        0    29560 2024-05-09 08:11:53.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/blockchaincom.py
+-rw-rw-rw-   0        0        0    85098 2024-05-08 04:04:46.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/bybit.py
+-rw-rw-rw-   0        0        0    58380 2024-05-09 08:11:53.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/cex.py
+-rw-rw-rw-   0        0        0    29324 2024-05-09 08:11:54.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/coinbase.py
+-rw-rw-rw-   0        0        0    25794 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/coinbaseinternational.py
+-rw-rw-rw-   0        0        0    38945 2024-05-09 08:11:55.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/coinbasepro.py
+-rw-rw-rw-   0        0        0     7789 2024-05-09 08:11:55.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/coincheck.py
+-rw-rw-rw-   0        0        0    45042 2024-05-09 08:11:55.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/coinex.py
+-rw-rw-rw-   0        0        0    15652 2024-05-09 08:11:55.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/coinone.py
+-rw-rw-rw-   0        0        0    42643 2024-05-09 08:11:56.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/cryptocom.py
+-rw-rw-rw-   0        0        0    22355 2024-05-09 08:11:56.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/currencycom.py
+-rw-rw-rw-   0        0        0    41035 2024-05-09 08:11:57.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/deribit.py
+-rw-rw-rw-   0        0        0    24527 2024-05-09 08:11:57.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/exmo.py
+-rw-rw-rw-   0        0        0    52489 2024-05-09 08:11:58.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/gate.py
+-rw-rw-rw-   0        0        0      391 2024-05-09 08:11:58.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/gateio.py
+-rw-rw-rw-   0        0        0    36641 2024-05-09 08:11:58.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/gemini.py
+-rw-rw-rw-   0        0        0    56284 2024-05-05 05:05:27.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/hitbtc.py
+-rw-rw-rw-   0        0        0    21957 2024-05-09 08:11:59.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/hollaex.py
+-rw-rw-rw-   0        0        0    96052 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/htx.py
+-rw-rw-rw-   0        0        0      385 2024-05-09 08:11:59.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/huobi.py
+-rw-rw-rw-   0        0        0    23174 2024-05-09 08:11:59.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/huobijp.py
+-rw-rw-rw-   0        0        0    20791 2024-05-09 08:11:59.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/hyperliquid.py
+-rw-rw-rw-   0        0        0    10082 2024-05-15 02:39:22.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/idax.py
+-rw-rw-rw-   0        0        0    28282 2024-05-09 08:11:59.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/idex.py
+-rw-rw-rw-   0        0        0    11179 2024-05-08 04:04:46.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/independentreserve.py
+-rw-rw-rw-   0        0        0    60764 2024-05-08 04:04:46.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/kraken.py
+-rw-rw-rw-   0        0        0    63917 2024-05-09 08:12:00.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/krakenfutures.py
+-rw-rw-rw-   0        0        0    50705 2024-05-09 08:12:01.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/kucoin.py
+-rw-rw-rw-   0        0        0    50026 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/kucoinfutures.py
+-rw-rw-rw-   0        0        0    35105 2024-05-09 08:12:02.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/lbank.py
+-rw-rw-rw-   0        0        0    12348 2024-05-09 08:12:02.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/luno.py
+-rw-rw-rw-   0        0        0    43183 2024-05-09 08:12:03.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/mexc.py
+-rw-rw-rw-   0        0        0    22643 2024-05-09 08:12:03.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/ndax.py
+-rw-rw-rw-   0        0        0    30385 2024-05-09 08:12:03.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/okcoin.py
+-rw-rw-rw-   0        0        0    72786 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/okx.py
+-rw-rw-rw-   0        0        0    54634 2024-05-09 08:12:04.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/onetrading.py
+-rw-rw-rw-   0        0        0    17877 2024-05-09 08:12:04.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/p2b.py
+-rw-rw-rw-   0        0        0    61032 2024-05-09 08:12:05.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/phemex.py
+-rw-rw-rw-   0        0        0    51235 2024-05-05 05:05:27.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/poloniex.py
+-rw-rw-rw-   0        0        0    41652 2024-05-09 08:12:05.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/poloniexfutures.py
+-rw-rw-rw-   0        0        0    22822 2024-05-09 08:12:06.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/probit.py
+-rw-rw-rw-   0        0        0     9654 2024-05-09 08:12:06.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/upbit.py
+-rw-rw-rw-   0        0        0    30043 2024-05-09 08:12:06.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/wazirx.py
+-rw-rw-rw-   0        0        0    35021 2024-05-09 08:12:07.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/whitebit.py
+-rw-rw-rw-   0        0        0    43584 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/woo.py
+-rw-rw-rw-   0        0        0    48892 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/pro/woofipro.py
+-rw-rw-rw-   0        0        0    76379 2024-05-09 07:45:18.000000 ccxt-idax-adapter-4.3.26/ccxt/probit.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.703228 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/
+-rw-rw-rw-   0        0        0       84 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.719015 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/
+-rw-rw-rw-   0        0        0      594 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/__init__.py
+-rw-rw-rw-   0        0        0    18461 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/_version.py
+-rw-rw-rw-   0        0        0     1886 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/curves.py
+-rw-rw-rw-   0        0        0     6942 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/der.py
+-rw-rw-rw-   0        0        0    11336 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/ecdsa.py
+-rw-rw-rw-   0        0        0     5517 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/ellipticcurve.py
+-rw-rw-rw-   0        0        0    14201 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/keys.py
+-rw-rw-rw-   0        0        0    13468 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/numbertheory.py
+-rw-rw-rw-   0        0        0     2572 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/rfc6979.py
+-rw-rw-rw-   0        0        0    10037 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/util.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.720014 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/
+-rw-rw-rw-   0        0        0      171 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.734213 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/
+-rw-rw-rw-   0        0        0      276 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/__init__.py
+-rw-rw-rw-   0        0        0      490 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/abi.py
+-rw-rw-rw-   0        0        0     4861 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/base.py
+-rw-rw-rw-   0        0        0     6871 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/codec.py
+-rw-rw-rw-   0        0        0       51 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/constants.py
+-rw-rw-rw-   0        0        0    16828 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/decoding.py
+-rw-rw-rw-   0        0        0    20162 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/encoding.py
+-rw-rw-rw-   0        0        0     2941 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/exceptions.py
+-rw-rw-rw-   0        0        0    12358 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/grammar.py
+-rw-rw-rw-   0        0        0      387 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/packed.py
+-rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/py.typed
+-rw-rw-rw-   0        0        0    19329 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/registry.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.736237 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/tools/
+-rw-rw-rw-   0        0        0       65 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/tools/__init__.py
+-rw-rw-rw-   0        0        0     5742 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.739321 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/utils/__init__.py
+-rw-rw-rw-   0        0        0     2097 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/utils/numeric.py
+-rw-rw-rw-   0        0        0      426 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/utils/padding.py
+-rw-rw-rw-   0        0        0      436 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/utils/string.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.742944 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/account/
+-rw-rw-rw-   0        0        0       48 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/account/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.746098 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/account/encode_typed_data/
+-rw-rw-rw-   0        0        0       80 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/account/encode_typed_data/__init__.py
+-rw-rw-rw-   0        0        0     7126 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py
+-rw-rw-rw-   0        0        0      982 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py
+-rw-rw-rw-   0        0        0    10588 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/account/messages.py
+-rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/account/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.750378 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/hexbytes/
+-rw-rw-rw-   0        0        0       60 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/hexbytes/__init__.py
+-rw-rw-rw-   0        0        0     1687 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/hexbytes/_utils.py
+-rw-rw-rw-   0        0        0     1768 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/hexbytes/main.py
+-rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/hexbytes/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.760394 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/typing/
+-rw-rw-rw-   0        0        0      913 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/typing/__init__.py
+-rw-rw-rw-   0        0        0       85 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/typing/abi.py
+-rw-rw-rw-   0        0        0      191 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/typing/bls.py
+-rw-rw-rw-   0        0        0       71 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/typing/discovery.py
+-rw-rw-rw-   0        0        0      117 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/typing/encoding.py
+-rw-rw-rw-   0        0        0      458 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/typing/enums.py
+-rw-rw-rw-   0        0        0      173 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/typing/ethpm.py
+-rw-rw-rw-   0        0        0      546 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/typing/evm.py
+-rw-rw-rw-   0        0        0    20845 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/typing/networks.py
+-rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/typing/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.790493 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/
+-rw-rw-rw-   0        0        0     2162 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/__init__.py
+-rw-rw-rw-   0        0        0     2123 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/abi.py
+-rw-rw-rw-   0        0        0     4364 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/address.py
+-rw-rw-rw-   0        0        0     4342 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/applicators.py
+-rw-rw-rw-   0        0        0     5498 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/conversions.py
+-rw-rw-rw-   0        0        0     3021 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/currency.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.792554 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/curried/
+-rw-rw-rw-   0        0        0     6398 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/curried/__init__.py
+-rw-rw-rw-   0        0        0      499 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/debug.py
+-rw-rw-rw-   0        0        0     3997 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/decorators.py
+-rw-rw-rw-   0        0        0      199 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/encoding.py
+-rw-rw-rw-   0        0        0      110 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/exceptions.py
+-rw-rw-rw-   0        0        0     2100 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/functional.py
+-rw-rw-rw-   0        0        0     1826 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/hexadecimal.py
+-rw-rw-rw-   0        0        0     4137 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/humanize.py
+-rw-rw-rw-   0        0        0     5155 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/logging.py
+-rw-rw-rw-   0        0        0      842 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/module_loading.py
+-rw-rw-rw-   0        0        0     1190 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/numeric.py
+-rw-rw-rw-   0        0        0        0 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/py.typed
+-rw-rw-rw-   0        0        0     1001 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/toolz.py
+-rw-rw-rw-   0        0        0     1074 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/types.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.795681 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/typing/
+-rw-rw-rw-   0        0        0      325 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/typing/__init__.py
+-rw-rw-rw-   0        0        0      189 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/typing/misc.py
+-rw-rw-rw-   0        0        0     1757 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/units.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.798690 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/keccak/
+-rw-rw-rw-   0        0        0       45 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/keccak/__init__.py
+-rw-rw-rw-   0        0        0     6934 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/keccak/keccak.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.805808 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/msgpack/
+-rw-rw-rw-   0        0        0     1077 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/msgpack/__init__.py
+-rw-rw-rw-   0        0        0     1081 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/msgpack/exceptions.py
+-rw-rw-rw-   0        0        0     5629 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/msgpack/ext.py
+-rw-rw-rw-   0        0        0    33175 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/msgpack/fallback.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.819371 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/parsimonious/
+-rw-rw-rw-   0        0        0      385 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/parsimonious/__init__.py
+-rw-rw-rw-   0        0        0     3603 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/parsimonious/exceptions.py
+-rw-rw-rw-   0        0        0    16864 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/parsimonious/expressions.py
+-rw-rw-rw-   0        0        0    19190 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/parsimonious/grammar.py
+-rw-rw-rw-   0        0        0    13084 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/parsimonious/nodes.py
+-rw-rw-rw-   0        0        0     1087 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/parsimonious/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.831808 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/
+-rw-rw-rw-   0        0        0      374 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/__init__.py
+-rw-rw-rw-   0        0        0    20555 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/_signatures.py
+-rw-rw-rw-   0        0        0    18447 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/_version.py
+-rw-rw-rw-   0        0        0      997 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/compatibility.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.834919 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/curried/
+-rw-rw-rw-   0        0        0     2226 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/curried/__init__.py
+-rw-rw-rw-   0        0        0      344 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/curried/exceptions.py
+-rw-rw-rw-   0        0        0      525 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/curried/operator.py
+-rw-rw-rw-   0        0        0     8955 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/dicttoolz.py
+-rw-rw-rw-   0        0        0    29821 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/functoolz.py
+-rw-rw-rw-   0        0        0    27612 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/itertoolz.py
+-rw-rw-rw-   0        0        0     1256 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/recipes.py
+-rw-rw-rw-   0        0        0      139 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.836915 ccxt-idax-adapter-4.3.26/ccxt/test/
+-rw-rw-rw-   0        0        0      141 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.878931 ccxt-idax-adapter-4.3.26/ccxt/test/base/
+-rw-rw-rw-   0        0        0     1889 2024-05-17 08:37:43.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/__init__.py
+-rw-rw-rw-   0        0        0      978 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_account.py
+-rw-rw-rw-   0        0        0     2931 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_balance.py
+-rw-rw-rw-   0        0        0     1808 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_borrow_interest.py
+-rw-rw-rw-   0        0        0     1500 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_borrow_rate.py
+-rw-rw-rw-   0        0        0     1177 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_calculate_fee.py
+-rw-rw-rw-   0        0        0     7702 2024-05-17 08:37:42.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_crypto.py
+-rw-rw-rw-   0        0        0     4472 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_currency.py
+-rw-rw-rw-   0        0        0     5634 2024-05-17 08:37:42.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_datetime.py
+-rw-rw-rw-   0        0        0    20934 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_decimal_to_precision.py
+-rw-rw-rw-   0        0        0     1402 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_deep_extend.py
+-rw-rw-rw-   0        0        0     2452 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_deposit_withdrawal.py
+-rw-rw-rw-   0        0        0     3592 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_exchange_datetime_functions.py
+-rw-rw-rw-   0        0        0     1351 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_funding_rate_history.py
+-rw-rw-rw-   0        0        0     1332 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_last_price.py
+-rw-rw-rw-   0        0        0     2289 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_ledger_entry.py
+-rw-rw-rw-   0        0        0     2154 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_ledger_item.py
+-rw-rw-rw-   0        0        0     1656 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_leverage_tier.py
+-rw-rw-rw-   0        0        0      869 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_margin_mode.py
+-rw-rw-rw-   0        0        0     1730 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_margin_modification.py
+-rw-rw-rw-   0        0        0    11632 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_market.py
+-rw-rw-rw-   0        0        0    22083 2024-05-17 08:37:42.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_number.py
+-rw-rw-rw-   0        0        0     2036 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_ohlcv.py
+-rw-rw-rw-   0        0        0     1547 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_open_interest.py
+-rw-rw-rw-   0        0        0     3964 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_order.py
+-rw-rw-rw-   0        0        0     3949 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_order_book.py
+-rw-rw-rw-   0        0        0     3884 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_position.py
+-rw-rw-rw-   0        0        0    19998 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_shared_methods.py
+-rw-rw-rw-   0        0        0      722 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_status.py
+-rw-rw-rw-   0        0        0     3123 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_throttle.py
+-rw-rw-rw-   0        0        0     5810 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_ticker.py
+-rw-rw-rw-   0        0        0     2336 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_trade.py
+-rw-rw-rw-   0        0        0     1066 2024-05-17 08:38:15.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_trading_fee.py
+-rw-rw-rw-   0        0        0     1434 2024-05-03 06:32:45.000000 ccxt-idax-adapter-4.3.26/ccxt/test/base/test_transaction.py
+-rw-rw-rw-   0        0        0    80043 2024-05-17 08:37:43.000000 ccxt-idax-adapter-4.3.26/ccxt/test/test_async.py
+-rw-rw-rw-   0        0        0    79000 2024-05-17 08:37:43.000000 ccxt-idax-adapter-4.3.26/ccxt/test/test_sync.py
+-rw-rw-rw-   0        0        0    71287 2024-05-09 07:45:23.000000 ccxt-idax-adapter-4.3.26/ccxt/timex.py
+-rw-rw-rw-   0        0        0   123013 2024-05-09 07:45:36.000000 ccxt-idax-adapter-4.3.26/ccxt/tokocrypto.py
+-rw-rw-rw-   0        0        0    23900 2024-05-09 07:45:37.000000 ccxt-idax-adapter-4.3.26/ccxt/tradeogre.py
+-rw-rw-rw-   0        0        0    81611 2024-05-09 07:45:41.000000 ccxt-idax-adapter-4.3.26/ccxt/upbit.py
+-rw-rw-rw-   0        0        0   113603 2024-05-09 07:45:49.000000 ccxt-idax-adapter-4.3.26/ccxt/wavesexchange.py
+-rw-rw-rw-   0        0        0    51342 2024-05-09 07:45:52.000000 ccxt-idax-adapter-4.3.26/ccxt/wazirx.py
+-rw-rw-rw-   0        0        0   114402 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/whitebit.py
+-rw-rw-rw-   0        0        0   139464 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/woo.py
+-rw-rw-rw-   0        0        0   114867 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/woofipro.py
+-rw-rw-rw-   0        0        0    53222 2024-05-09 07:46:07.000000 ccxt-idax-adapter-4.3.26/ccxt/yobit.py
+-rw-rw-rw-   0        0        0    27979 2024-05-09 07:46:09.000000 ccxt-idax-adapter-4.3.26/ccxt/zaif.py
+-rw-rw-rw-   0        0        0    80598 2024-05-13 08:17:22.000000 ccxt-idax-adapter-4.3.26/ccxt/zonda.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:41:31.885739 ccxt-idax-adapter-4.3.26/ccxt_idax_adapter.egg-info/
+-rw-rw-rw-   0        0        0     2821 2024-05-17 08:41:31.000000 ccxt-idax-adapter-4.3.26/ccxt_idax_adapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    15934 2024-05-17 08:41:31.000000 ccxt-idax-adapter-4.3.26/ccxt_idax_adapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 08:41:31.000000 ccxt-idax-adapter-4.3.26/ccxt_idax_adapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      218 2024-05-17 08:41:31.000000 ccxt-idax-adapter-4.3.26/ccxt_idax_adapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-17 08:41:31.000000 ccxt-idax-adapter-4.3.26/ccxt_idax_adapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12489 2024-05-17 08:41:25.000000 ccxt-idax-adapter-4.3.26/package.json
+-rw-rw-rw-   0        0        0      226 2024-05-17 08:41:31.889770 ccxt-idax-adapter-4.3.26/setup.cfg
+-rw-rw-rw-   0        0        0     3071 2024-05-09 09:58:59.000000 ccxt-idax-adapter-4.3.26/setup.py
```

### Comparing `ccxt-idax-adapter-4.3.25/LICENSE.txt` & `ccxt-idax-adapter-4.3.26/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/PKG-INFO` & `ccxt-idax-adapter-4.3.26/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ccxt-idax-adapter
-Version: 4.3.25
-Summary: Custom fork of ccxt
+Version: 4.3.26
+Summary: Custom version of ccxt
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://github.com/ccxt/ccxt/wiki
 Project-URL: Discord, https://discord.gg/ccxt
@@ -43,8 +43,10 @@
 Requires-Dist: yarl>=1.7.2; python_version >= "3.5.2"
 Provides-Extra: qa
 Requires-Dist: ruff==0.0.292; extra == "qa"
 Requires-Dist: tox>=4.8.0; extra == "qa"
 Provides-Extra: type
 Requires-Dist: mypy==1.6.1; extra == "type"
 
-This is a fork of [ccxt](https://github.com/ccxt/ccxt) for [idax](https://www.idax.exchange).
+# Non official version of an open source project
+
+This is a custom fork of [ccxt](https://github.com/ccxt/ccxt) for [idax](https://www.idax.exchange).
```

### Comparing `ccxt-idax-adapter-4.3.25/README.rst` & `ccxt-idax-adapter-4.3.26/README.rst`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/__init__.py` & `ccxt-idax-adapter-4.3.26/ccxt/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/ace.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/alpaca.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/ascendex.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bequant.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bigone.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/binance.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/binancecoinm.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/binanceus.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/binanceusdm.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bingx.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bit2c.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bitbank.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bitbay.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bitbay.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bitbns.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bitcoincom.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bitfinex.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bitfinex2.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bitflyer.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bitget.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bithumb.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bitmart.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bitmex.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bitopro.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bitpanda.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bitrue.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bitso.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bitstamp.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bitteam.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bitteam.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bitvavo.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bl3p.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/blockchaincom.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/blofin.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/blofin.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/btcalpha.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/btcbox.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/btcmarkets.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/btcturk.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/bybit.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/cex.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/coinbase.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/coinbaseinternational.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/coinbasepro.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/coincheck.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/coinex.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/coinlist.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/coinlist.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/coinmate.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/coinmetro.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/coinmetro.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/coinone.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/coinsph.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/coinspot.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/cryptocom.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/currencycom.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/delta.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/deribit.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/digifinex.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/exmo.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/fmfwio.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/gate.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/gateio.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/gateio.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/gemini.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/hitbtc.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/hitbtc3.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/hollaex.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/htx.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/huobi.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/huobijp.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/idax.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/idax.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/idex.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/independentreserve.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/indodax.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/kraken.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/krakenfutures.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/kucoin.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/kucoinfutures.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/kuna.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/latoken.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/lbank.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/luno.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/lykke.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/mercado.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/mexc.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/ndax.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/novadax.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/oceanex.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/okcoin.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/okx.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/onetrading.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/p2b.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/paymium.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/phemex.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/poloniex.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/poloniexfutures.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/probit.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/timex.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/tokocrypto.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/tradeogre.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/tradeogre.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/upbit.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/wavesexchange.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/wazirx.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/whitebit.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/woo.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/woofipro.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/woofipro.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/yobit.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/zaif.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/abstract/zonda.py` & `ccxt-idax-adapter-4.3.26/ccxt/abstract/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/ace.py` & `ccxt-idax-adapter-4.3.26/ccxt/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/alpaca.py` & `ccxt-idax-adapter-4.3.26/ccxt/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/ascendex.py` & `ccxt-idax-adapter-4.3.26/ccxt/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/__init__.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/ace.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/alpaca.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/ascendex.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/base/exchange.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/base/exchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/base/throttler.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/base/throttler.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/base/ws/__init__.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/base/ws/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/base/ws/aiohttp_client.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/base/ws/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/base/ws/cache.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/base/ws/cache.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/base/ws/client.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/base/ws/client.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/base/ws/fast_client.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/base/ws/fast_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/base/ws/functions.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/base/ws/functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/base/ws/future.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/base/ws/future.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/base/ws/order_book.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/base/ws/order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/base/ws/order_book_side.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/base/ws/order_book_side.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bequant.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bigone.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/binance.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/binancecoinm.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/binanceus.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/binanceusdm.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bingx.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bit2c.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bitbank.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bitbns.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bitcoincom.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bitfinex.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bitfinex2.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bitflyer.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bitget.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bithumb.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bitmart.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bitmex.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bitopro.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bitrue.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bitso.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bitstamp.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bitteam.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bitteam.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bitvavo.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bl3p.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/blockchaincom.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/blofin.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/blofin.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/btcalpha.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/btcbox.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/btcmarkets.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/btcturk.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/bybit.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/cex.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/coinbase.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/coinbaseinternational.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/coinbasepro.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/coincheck.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/coinex.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/coinlist.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/coinlist.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/coinmate.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/coinmetro.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/coinmetro.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/coinone.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/coinsph.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/coinspot.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/cryptocom.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/currencycom.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/delta.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/deribit.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/digifinex.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/exmo.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/fmfwio.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/gate.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/gemini.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/hitbtc.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/hollaex.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/htx.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/huobijp.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/hyperliquid.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/idax.py` & `ccxt-idax-adapter-4.3.26/ccxt/idax.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 
 # PLEASE DO NOT EDIT THIS FILE, IT IS GENERATED AND WILL BE OVERWRITTEN:
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
-from ccxt.async_support.base.exchange import Exchange
+from ccxt.base.exchange import Exchange
 from ccxt.abstract.idax import ImplicitAPI
-import asyncio
 import hashlib
 from ccxt.base.types import Any, Balances, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade
 from typing import List
 from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
@@ -31,14 +30,16 @@
             'name': 'Idax',
             'countries': ['MN'],  # Mongolia
             # 12000 per minute => 200 per second
             # 1000ms / 200 = 5
             'rateLimit': 5,
             'certified': False,
             'pro': True,
+            'adjustForTimeDifference': True,
+            'timeDifference': 0,
             'has': {
                 'CORS': None,
                 'spot': True,
                 'margin': None,  # soon
                 'swap': False,
                 'future': None,  # soon
                 'option': False,
@@ -170,27 +171,29 @@
                     '-2015': AuthenticationError,
                     '-2016': OrderNotFillable,
                     '-2017': InsufficientFunds,
                 },
             },
         })
 
-    async def fetch_markets(self, params={}) -> List[Market]:
+    def fetch_markets(self, params={}) -> List[Market]:
         promises = [
             # Will add fetchFuturesMarkets(params) later
             self.fetch_spot_markets(params),
         ]
-        awaitedPromises = await asyncio.gather(*promises)
+        awaitedPromises = promises
         result = []
         for i in range(0, len(awaitedPromises)):
             result = self.array_concat(result, awaitedPromises[i])
+        if self.options['adjustForTimeDifference']:
+            self.load_time_difference()
         return result
 
-    async def fetch_spot_markets(self, params={}) -> List[Market]:
-        response = await self.sapiPublicGetSymbols()
+    def fetch_spot_markets(self, params={}) -> List[Market]:
+        response = self.sapiPublicGetSymbols()
         #
         # spot
         #
         #     {
         #         "symbols":[
         #             {
         #                 "symbol":"shib1321usdt",
@@ -267,39 +270,39 @@
                 'precision': {
                     'amount': amountPrecision,
                     'price': pricePrecision,
                 },
             })
         return result
 
-    async def fetch_ticker(self, symbol: str, params={}) -> Ticker:
-        await self.load_markets()
+    def fetch_ticker(self, symbol: str, params={}) -> Ticker:
+        self.load_markets()
         market = self.market(symbol)
         marketId = market['id']
         request = {
             'symbol': marketId,
         }
-        response = await self.sapiPublicGetTicker(self.deep_extend(request, params))
+        response = self.sapiPublicGetTicker(self.deep_extend(request, params))
         return self.parse_ticker(response, market)
 
-    async def fetch_tickers(self, symbols: Strings = None, params={}) -> Tickers:
-        await self.load_markets()
+    def fetch_tickers(self, symbols: Strings = None, params={}) -> Tickers:
+        self.load_markets()
         result = {}
         symbols = self.market_symbols(symbols, None, True, True, True)
         if symbols is None:
             return {}
         length = len(symbols)
         for i in range(0, length):
             symbol = symbols[i]
             market = self.market(symbol)
             marketId = market['id']
             request = {
                 'symbol': marketId,
             }
-            response = await self.sapiPublicGetTicker(self.deep_extend(request, params))
+            response = self.sapiPublicGetTicker(self.deep_extend(request, params))
             ticker = self.parse_ticker(response, market)
             result[marketId] = ticker
         return result
 
     def parse_ticker(self, response, market: Market) -> Ticker:
         symbol = market['symbol']
         high = self.safe_number(response, 'high')
@@ -334,66 +337,66 @@
             'datetime': self.iso8601(timestamp),
             'bidVolume': None,
             'askVolume': None,
             'average': average,
             'info': response,
         }, market)
 
-    async def fetch_time(self, params={}) -> float:
-        response = await self.sapiPublicGetTime(params)
+    def fetch_time(self, params={}) -> float:
+        response = self.sapiPublicGetTime(params)
         return self.safe_number(response, 'serverTime')
 
-    async def fetch_order_book(self, symbol: str, limit: Int = None, params={}) -> OrderBook:
-        await self.load_markets()
+    def fetch_order_book(self, symbol: str, limit: Int = None, params={}) -> OrderBook:
+        self.load_markets()
         market = self.market(symbol)
         marketId = market['id']
         request = {
             'symbol': marketId,
         }
         if limit is not None:
             request['limit'] = limit
-        time = await self.fetch_time()
-        response = await self.sapiPublicGetDepth(self.deep_extend(request, params))
+        time = self.fetch_time()
+        response = self.sapiPublicGetDepth(self.deep_extend(request, params))
         return self.parse_order_book(response, symbol, time)
 
-    async def fetch_ohlcv(self, symbol: str, timeframe='1m', since: Int = None, limit: Int = None, params={}) -> List[list]:
-        await self.load_markets()
+    def fetch_ohlcv(self, symbol: str, timeframe='1m', since: Int = None, limit: Int = None, params={}) -> List[list]:
+        self.load_markets()
         market = self.market(symbol)
         marketId = market['id']
         interval = self.safe_string(self.timeframes, timeframe)
         request = {
             'symbol': marketId,
             'interval': interval,
         }
         if limit is not None:
             request['limit'] = limit
         if since is not None:
             request['startTime'] = since
-        response = await self.sapiPublicGetKlines(self.deep_extend(request, params))
+        response = self.sapiPublicGetKlines(self.deep_extend(request, params))
         return self.parse_ohlcvs(response, market, timeframe, since, limit)
 
     def parse_ohlcv(self, ohlcv: Any, market: Market) -> list:
         timestamp = self.safe_number(ohlcv, 'idx')
         open = self.safe_number(ohlcv, 'open')
         high = self.safe_number(ohlcv, 'high')
         low = self.safe_number(ohlcv, 'low')
         close = self.safe_number(ohlcv, 'close')
         vol = self.safe_number(ohlcv, 'vol')
         return [timestamp, open, high, low, close, vol]
 
-    async def fetch_trades(self, symbol: str, since: Int = None, limit: Int = None, params={}) -> List[Trade]:
-        await self.load_markets()
+    def fetch_trades(self, symbol: str, since: Int = None, limit: Int = None, params={}) -> List[Trade]:
+        self.load_markets()
         market = self.market(symbol)
         marketId = market['id']
         request = {
             'symbol': marketId,
         }
         if limit is not None:
             request['limit'] = limit
-        response = await self.sapiPublicGetTrades(self.deep_extend(request, params))
+        response = self.sapiPublicGetTrades(self.deep_extend(request, params))
         trades = self.safe_list(response, 'list')
         return self.parse_trades(trades, market)
 
     def parse_trade(self, trade: object, market: Market = None) -> Trade:
         amount = self.safe_number(trade, 'qty')
         timestamp = self.safe_number(trade, 'time')
         datetime = self.iso8601(timestamp)
@@ -425,14 +428,17 @@
             'side': side,
             'symbol': symbol,
             'takerOrMaker': takerOrMaker,
             'cost': None,
             'fee': None,
         })
 
+    def nonce(self):
+        return self.milliseconds() - self.options['timeDifference']
+
     def sign(self, path, api='public', method='GET', params={}, headers=None, body=None):
         headers = {
             'Content-Type': 'application/json',
         }
         bodyString = ''
         if 'body' in params:
             body = params['body']
@@ -443,31 +449,31 @@
             paramsString = '?' + self.urlencode(params)
         url = self.urls['api'][api]
         url += '/' + path
         if paramsString != '':
             url = url + paramsString
         # Will modify it when support for futures and margins are being implemented
         if api == 'sapiPrivate':
-            timestamp = self.number_to_string(self.milliseconds())
+            timestamp = self.number_to_string(self.nonce())
             hashData = timestamp + method + '/sapi/v1/' + path + paramsString + bodyString
             signature = self.hmac(self.encode(hashData), self.encode(self.secret), hashlib.sha256)
             headers['X-CH-APIKEY'] = self.apiKey
             headers['X-CH-SIGN'] = signature
             headers['X-CH-TS'] = timestamp
         obj = {
             'url': url,
             'method': method,
             'body': body,
             'headers': headers,
         }
         return obj
 
-    async def fetch_balance(self, params={}) -> Balances:
-        await self.load_markets()
-        response = await self.sapiPrivateGetAccount()
+    def fetch_balance(self, params={}) -> Balances:
+        self.load_markets()
+        response = self.sapiPrivateGetAccount()
         return self.parse_balance(response)
 
     def parse_balance(self, response: Any) -> Balances:
         list = self.safe_list(response, 'balances')
         balances = {
             'info': response,
         }
@@ -485,30 +491,30 @@
             }
         timestamp = self.milliseconds()
         datetime = self.iso8601(timestamp)
         balances['timestamp'] = timestamp
         balances['datetime'] = datetime
         return balances
 
-    async def create_order(self, symbol: str, type: OrderType, side: OrderSide, amount: float, price: Num = None, params={}) -> Order:
-        await self.load_markets()
+    def create_order(self, symbol: str, type: OrderType, side: OrderSide, amount: float, price: Num = None, params={}) -> Order:
+        self.load_markets()
         market = self.market(symbol)
         marketId = market['id']
         clientOrderId = self.safe_string(params, 'clientOrderId')
         request = {
             'symbol': marketId,
             'volume': amount,
             'side': side.upper(),
             'type': type.upper(),
             'price': price,
         }
         if clientOrderId is not None:
             request['clientOrderId'] = clientOrderId
         params['body'] = request
-        response = await self.sapiPrivatePostOrder(params)
+        response = self.sapiPrivatePostOrder(params)
         return self.parse_order(response, market)
 
     def parse_order(self, order: Any, market: Market) -> Order:
         id = None
         if 'orderIdString' in order:
             id = self.safe_string(order, 'orderIdString')
         else:
@@ -564,24 +570,24 @@
             'CANCELED': 'canceled',
             'PENDING_CANCEL': 'canceled',
             'REJECTED': 'rejected',
             'FILLED': 'closed',
         }
         return dict[status]
 
-    async def cancel_order(self, id: str, symbol: Str = None, params={}) -> Order:
-        await self.load_markets()
+    def cancel_order(self, id: str, symbol: Str = None, params={}) -> Order:
+        self.load_markets()
         market = self.market(symbol)
         marketId = market['id']
         request = {
             'orderId': id,
             'symbol': marketId,
         }
         params['body'] = request
-        response = await self.sapiPrivatePostCancel(params)
+        response = self.sapiPrivatePostCancel(params)
         return self.parse_canceled_order(response, market)
 
     def parse_canceled_order(self, response, market: Market) -> Order:
         id = self.safe_number(response, 'orderId')
         marketId = self.safe_string(response, 'symbol')
         symbol = self.safe_symbol(marketId, market)
         status = self.safe_string(response, 'status')
@@ -592,44 +598,44 @@
             orderStatus = 'rejected'
         return self.safe_order({
             'id': id,
             'symbol': symbol,
             'status': orderStatus,
         }, market)
 
-    async def fetch_order(self, id: str, symbol: Str = None, params={}) -> Order:
-        await self.load_markets()
+    def fetch_order(self, id: str, symbol: Str = None, params={}) -> Order:
+        self.load_markets()
         market = self.market(symbol)
         marketId = market['id']
         request = {
             'orderId': id,
             'symbol': marketId,
         }
-        response = await self.sapiPrivateGetOrder(self.extend(request, params))
+        response = self.sapiPrivateGetOrder(self.extend(request, params))
         return self.parse_order(response, market)
 
-    async def fetch_open_orders(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Order]:
-        await self.load_markets()
+    def fetch_open_orders(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Order]:
+        self.load_markets()
         market = self.market(symbol)
         marketId = market['id']
         request = {
             'symbol': marketId,
             'limit': limit,
         }
         if limit is not None:
             request['limit'] = limit
-        response = await self.sapiPrivateGetOpenOrders(self.deep_extend(request, params))
+        response = self.sapiPrivateGetOpenOrders(self.deep_extend(request, params))
         arr = self.safe_list(response, 'list', [])
         return self.parse_orders(arr, market)
 
-    async def fetch_my_trades(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Trade]:
-        await self.load_markets()
+    def fetch_my_trades(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Trade]:
+        self.load_markets()
         market = self.market(symbol)
         marketId = market['id']
         request = {
             'symbol': marketId,
         }
         if limit is not None:
             request['limit'] = limit
-        response = await self.sapiPrivateGetMyTrades(self.extend(request, params))
+        response = self.sapiPrivateGetMyTrades(self.extend(request, params))
         trades = self.safe_list(response, 'list')
         return self.parse_trades(trades, market)
```

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/idex.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/independentreserve.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/indodax.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/kraken.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/krakenfutures.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/kucoin.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/kucoinfutures.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/kuna.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/latoken.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/lbank.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/luno.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/lykke.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/mercado.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/mexc.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/ndax.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/novadax.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/oceanex.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/okcoin.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/okx.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/onetrading.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/p2b.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/paymium.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/phemex.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/poloniex.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/poloniexfutures.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/probit.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/timex.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/tokocrypto.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/tradeogre.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/tradeogre.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/upbit.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/wavesexchange.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/wazirx.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/whitebit.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/woo.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/woofipro.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/woofipro.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/yobit.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/zaif.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/async_support/zonda.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/base/__init__.py` & `ccxt-idax-adapter-4.3.26/ccxt/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/base/decimal_to_precision.py` & `ccxt-idax-adapter-4.3.26/ccxt/base/decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/base/errors.py` & `ccxt-idax-adapter-4.3.26/ccxt/base/errors.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/base/exchange.py` & `ccxt-idax-adapter-4.3.26/ccxt/base/exchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/base/precise.py` & `ccxt-idax-adapter-4.3.26/ccxt/base/precise.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/base/types.py` & `ccxt-idax-adapter-4.3.26/ccxt/base/types.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bequant.py` & `ccxt-idax-adapter-4.3.26/ccxt/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bigone.py` & `ccxt-idax-adapter-4.3.26/ccxt/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/binance.py` & `ccxt-idax-adapter-4.3.26/ccxt/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/binancecoinm.py` & `ccxt-idax-adapter-4.3.26/ccxt/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/binanceus.py` & `ccxt-idax-adapter-4.3.26/ccxt/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/binanceusdm.py` & `ccxt-idax-adapter-4.3.26/ccxt/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bingx.py` & `ccxt-idax-adapter-4.3.26/ccxt/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bit2c.py` & `ccxt-idax-adapter-4.3.26/ccxt/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bitbank.py` & `ccxt-idax-adapter-4.3.26/ccxt/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bitbns.py` & `ccxt-idax-adapter-4.3.26/ccxt/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bitfinex.py` & `ccxt-idax-adapter-4.3.26/ccxt/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bitfinex2.py` & `ccxt-idax-adapter-4.3.26/ccxt/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bitflyer.py` & `ccxt-idax-adapter-4.3.26/ccxt/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bitget.py` & `ccxt-idax-adapter-4.3.26/ccxt/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bithumb.py` & `ccxt-idax-adapter-4.3.26/ccxt/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bitmart.py` & `ccxt-idax-adapter-4.3.26/ccxt/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bitmex.py` & `ccxt-idax-adapter-4.3.26/ccxt/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bitopro.py` & `ccxt-idax-adapter-4.3.26/ccxt/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bitrue.py` & `ccxt-idax-adapter-4.3.26/ccxt/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bitso.py` & `ccxt-idax-adapter-4.3.26/ccxt/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bitstamp.py` & `ccxt-idax-adapter-4.3.26/ccxt/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bitteam.py` & `ccxt-idax-adapter-4.3.26/ccxt/bitteam.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bitvavo.py` & `ccxt-idax-adapter-4.3.26/ccxt/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bl3p.py` & `ccxt-idax-adapter-4.3.26/ccxt/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/blockchaincom.py` & `ccxt-idax-adapter-4.3.26/ccxt/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/blofin.py` & `ccxt-idax-adapter-4.3.26/ccxt/blofin.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/btcalpha.py` & `ccxt-idax-adapter-4.3.26/ccxt/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/btcbox.py` & `ccxt-idax-adapter-4.3.26/ccxt/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/btcmarkets.py` & `ccxt-idax-adapter-4.3.26/ccxt/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/btcturk.py` & `ccxt-idax-adapter-4.3.26/ccxt/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/bybit.py` & `ccxt-idax-adapter-4.3.26/ccxt/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/cex.py` & `ccxt-idax-adapter-4.3.26/ccxt/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/coinbase.py` & `ccxt-idax-adapter-4.3.26/ccxt/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/coinbaseinternational.py` & `ccxt-idax-adapter-4.3.26/ccxt/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/coinbasepro.py` & `ccxt-idax-adapter-4.3.26/ccxt/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/coincheck.py` & `ccxt-idax-adapter-4.3.26/ccxt/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/coinex.py` & `ccxt-idax-adapter-4.3.26/ccxt/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/coinlist.py` & `ccxt-idax-adapter-4.3.26/ccxt/coinlist.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/coinmate.py` & `ccxt-idax-adapter-4.3.26/ccxt/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/coinmetro.py` & `ccxt-idax-adapter-4.3.26/ccxt/coinmetro.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/coinone.py` & `ccxt-idax-adapter-4.3.26/ccxt/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/coinsph.py` & `ccxt-idax-adapter-4.3.26/ccxt/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/coinspot.py` & `ccxt-idax-adapter-4.3.26/ccxt/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/cryptocom.py` & `ccxt-idax-adapter-4.3.26/ccxt/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/currencycom.py` & `ccxt-idax-adapter-4.3.26/ccxt/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/delta.py` & `ccxt-idax-adapter-4.3.26/ccxt/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/deribit.py` & `ccxt-idax-adapter-4.3.26/ccxt/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/digifinex.py` & `ccxt-idax-adapter-4.3.26/ccxt/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/exmo.py` & `ccxt-idax-adapter-4.3.26/ccxt/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/fmfwio.py` & `ccxt-idax-adapter-4.3.26/ccxt/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/gate.py` & `ccxt-idax-adapter-4.3.26/ccxt/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/gemini.py` & `ccxt-idax-adapter-4.3.26/ccxt/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/hitbtc.py` & `ccxt-idax-adapter-4.3.26/ccxt/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/hollaex.py` & `ccxt-idax-adapter-4.3.26/ccxt/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/htx.py` & `ccxt-idax-adapter-4.3.26/ccxt/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/huobijp.py` & `ccxt-idax-adapter-4.3.26/ccxt/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/hyperliquid.py` & `ccxt-idax-adapter-4.3.26/ccxt/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/idax.py` & `ccxt-idax-adapter-4.3.26/ccxt/async_support/idax.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 
 # PLEASE DO NOT EDIT THIS FILE, IT IS GENERATED AND WILL BE OVERWRITTEN:
 # https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
 
-from ccxt.base.exchange import Exchange
+from ccxt.async_support.base.exchange import Exchange
 from ccxt.abstract.idax import ImplicitAPI
+import asyncio
 import hashlib
 from ccxt.base.types import Any, Balances, Int, Market, Num, Order, OrderBook, OrderSide, OrderType, Str, Strings, Ticker, Tickers, Trade
 from typing import List
 from ccxt.base.errors import AuthenticationError
 from ccxt.base.errors import BadRequest
 from ccxt.base.errors import BadSymbol
 from ccxt.base.errors import InsufficientFunds
@@ -30,14 +31,16 @@
             'name': 'Idax',
             'countries': ['MN'],  # Mongolia
             # 12000 per minute => 200 per second
             # 1000ms / 200 = 5
             'rateLimit': 5,
             'certified': False,
             'pro': True,
+            'adjustForTimeDifference': True,
+            'timeDifference': 0,
             'has': {
                 'CORS': None,
                 'spot': True,
                 'margin': None,  # soon
                 'swap': False,
                 'future': None,  # soon
                 'option': False,
@@ -169,27 +172,29 @@
                     '-2015': AuthenticationError,
                     '-2016': OrderNotFillable,
                     '-2017': InsufficientFunds,
                 },
             },
         })
 
-    def fetch_markets(self, params={}) -> List[Market]:
+    async def fetch_markets(self, params={}) -> List[Market]:
         promises = [
             # Will add fetchFuturesMarkets(params) later
             self.fetch_spot_markets(params),
         ]
-        awaitedPromises = promises
+        awaitedPromises = await asyncio.gather(*promises)
         result = []
         for i in range(0, len(awaitedPromises)):
             result = self.array_concat(result, awaitedPromises[i])
+        if self.options['adjustForTimeDifference']:
+            await self.load_time_difference()
         return result
 
-    def fetch_spot_markets(self, params={}) -> List[Market]:
-        response = self.sapiPublicGetSymbols()
+    async def fetch_spot_markets(self, params={}) -> List[Market]:
+        response = await self.sapiPublicGetSymbols()
         #
         # spot
         #
         #     {
         #         "symbols":[
         #             {
         #                 "symbol":"shib1321usdt",
@@ -266,39 +271,39 @@
                 'precision': {
                     'amount': amountPrecision,
                     'price': pricePrecision,
                 },
             })
         return result
 
-    def fetch_ticker(self, symbol: str, params={}) -> Ticker:
-        self.load_markets()
+    async def fetch_ticker(self, symbol: str, params={}) -> Ticker:
+        await self.load_markets()
         market = self.market(symbol)
         marketId = market['id']
         request = {
             'symbol': marketId,
         }
-        response = self.sapiPublicGetTicker(self.deep_extend(request, params))
+        response = await self.sapiPublicGetTicker(self.deep_extend(request, params))
         return self.parse_ticker(response, market)
 
-    def fetch_tickers(self, symbols: Strings = None, params={}) -> Tickers:
-        self.load_markets()
+    async def fetch_tickers(self, symbols: Strings = None, params={}) -> Tickers:
+        await self.load_markets()
         result = {}
         symbols = self.market_symbols(symbols, None, True, True, True)
         if symbols is None:
             return {}
         length = len(symbols)
         for i in range(0, length):
             symbol = symbols[i]
             market = self.market(symbol)
             marketId = market['id']
             request = {
                 'symbol': marketId,
             }
-            response = self.sapiPublicGetTicker(self.deep_extend(request, params))
+            response = await self.sapiPublicGetTicker(self.deep_extend(request, params))
             ticker = self.parse_ticker(response, market)
             result[marketId] = ticker
         return result
 
     def parse_ticker(self, response, market: Market) -> Ticker:
         symbol = market['symbol']
         high = self.safe_number(response, 'high')
@@ -333,66 +338,66 @@
             'datetime': self.iso8601(timestamp),
             'bidVolume': None,
             'askVolume': None,
             'average': average,
             'info': response,
         }, market)
 
-    def fetch_time(self, params={}) -> float:
-        response = self.sapiPublicGetTime(params)
+    async def fetch_time(self, params={}) -> float:
+        response = await self.sapiPublicGetTime(params)
         return self.safe_number(response, 'serverTime')
 
-    def fetch_order_book(self, symbol: str, limit: Int = None, params={}) -> OrderBook:
-        self.load_markets()
+    async def fetch_order_book(self, symbol: str, limit: Int = None, params={}) -> OrderBook:
+        await self.load_markets()
         market = self.market(symbol)
         marketId = market['id']
         request = {
             'symbol': marketId,
         }
         if limit is not None:
             request['limit'] = limit
-        time = self.fetch_time()
-        response = self.sapiPublicGetDepth(self.deep_extend(request, params))
+        time = await self.fetch_time()
+        response = await self.sapiPublicGetDepth(self.deep_extend(request, params))
         return self.parse_order_book(response, symbol, time)
 
-    def fetch_ohlcv(self, symbol: str, timeframe='1m', since: Int = None, limit: Int = None, params={}) -> List[list]:
-        self.load_markets()
+    async def fetch_ohlcv(self, symbol: str, timeframe='1m', since: Int = None, limit: Int = None, params={}) -> List[list]:
+        await self.load_markets()
         market = self.market(symbol)
         marketId = market['id']
         interval = self.safe_string(self.timeframes, timeframe)
         request = {
             'symbol': marketId,
             'interval': interval,
         }
         if limit is not None:
             request['limit'] = limit
         if since is not None:
             request['startTime'] = since
-        response = self.sapiPublicGetKlines(self.deep_extend(request, params))
+        response = await self.sapiPublicGetKlines(self.deep_extend(request, params))
         return self.parse_ohlcvs(response, market, timeframe, since, limit)
 
     def parse_ohlcv(self, ohlcv: Any, market: Market) -> list:
         timestamp = self.safe_number(ohlcv, 'idx')
         open = self.safe_number(ohlcv, 'open')
         high = self.safe_number(ohlcv, 'high')
         low = self.safe_number(ohlcv, 'low')
         close = self.safe_number(ohlcv, 'close')
         vol = self.safe_number(ohlcv, 'vol')
         return [timestamp, open, high, low, close, vol]
 
-    def fetch_trades(self, symbol: str, since: Int = None, limit: Int = None, params={}) -> List[Trade]:
-        self.load_markets()
+    async def fetch_trades(self, symbol: str, since: Int = None, limit: Int = None, params={}) -> List[Trade]:
+        await self.load_markets()
         market = self.market(symbol)
         marketId = market['id']
         request = {
             'symbol': marketId,
         }
         if limit is not None:
             request['limit'] = limit
-        response = self.sapiPublicGetTrades(self.deep_extend(request, params))
+        response = await self.sapiPublicGetTrades(self.deep_extend(request, params))
         trades = self.safe_list(response, 'list')
         return self.parse_trades(trades, market)
 
     def parse_trade(self, trade: object, market: Market = None) -> Trade:
         amount = self.safe_number(trade, 'qty')
         timestamp = self.safe_number(trade, 'time')
         datetime = self.iso8601(timestamp)
@@ -424,14 +429,17 @@
             'side': side,
             'symbol': symbol,
             'takerOrMaker': takerOrMaker,
             'cost': None,
             'fee': None,
         })
 
+    def nonce(self):
+        return self.milliseconds() - self.options['timeDifference']
+
     def sign(self, path, api='public', method='GET', params={}, headers=None, body=None):
         headers = {
             'Content-Type': 'application/json',
         }
         bodyString = ''
         if 'body' in params:
             body = params['body']
@@ -442,31 +450,31 @@
             paramsString = '?' + self.urlencode(params)
         url = self.urls['api'][api]
         url += '/' + path
         if paramsString != '':
             url = url + paramsString
         # Will modify it when support for futures and margins are being implemented
         if api == 'sapiPrivate':
-            timestamp = self.number_to_string(self.milliseconds())
+            timestamp = self.number_to_string(self.nonce())
             hashData = timestamp + method + '/sapi/v1/' + path + paramsString + bodyString
             signature = self.hmac(self.encode(hashData), self.encode(self.secret), hashlib.sha256)
             headers['X-CH-APIKEY'] = self.apiKey
             headers['X-CH-SIGN'] = signature
             headers['X-CH-TS'] = timestamp
         obj = {
             'url': url,
             'method': method,
             'body': body,
             'headers': headers,
         }
         return obj
 
-    def fetch_balance(self, params={}) -> Balances:
-        self.load_markets()
-        response = self.sapiPrivateGetAccount()
+    async def fetch_balance(self, params={}) -> Balances:
+        await self.load_markets()
+        response = await self.sapiPrivateGetAccount()
         return self.parse_balance(response)
 
     def parse_balance(self, response: Any) -> Balances:
         list = self.safe_list(response, 'balances')
         balances = {
             'info': response,
         }
@@ -484,30 +492,30 @@
             }
         timestamp = self.milliseconds()
         datetime = self.iso8601(timestamp)
         balances['timestamp'] = timestamp
         balances['datetime'] = datetime
         return balances
 
-    def create_order(self, symbol: str, type: OrderType, side: OrderSide, amount: float, price: Num = None, params={}) -> Order:
-        self.load_markets()
+    async def create_order(self, symbol: str, type: OrderType, side: OrderSide, amount: float, price: Num = None, params={}) -> Order:
+        await self.load_markets()
         market = self.market(symbol)
         marketId = market['id']
         clientOrderId = self.safe_string(params, 'clientOrderId')
         request = {
             'symbol': marketId,
             'volume': amount,
             'side': side.upper(),
             'type': type.upper(),
             'price': price,
         }
         if clientOrderId is not None:
             request['clientOrderId'] = clientOrderId
         params['body'] = request
-        response = self.sapiPrivatePostOrder(params)
+        response = await self.sapiPrivatePostOrder(params)
         return self.parse_order(response, market)
 
     def parse_order(self, order: Any, market: Market) -> Order:
         id = None
         if 'orderIdString' in order:
             id = self.safe_string(order, 'orderIdString')
         else:
@@ -563,24 +571,24 @@
             'CANCELED': 'canceled',
             'PENDING_CANCEL': 'canceled',
             'REJECTED': 'rejected',
             'FILLED': 'closed',
         }
         return dict[status]
 
-    def cancel_order(self, id: str, symbol: Str = None, params={}) -> Order:
-        self.load_markets()
+    async def cancel_order(self, id: str, symbol: Str = None, params={}) -> Order:
+        await self.load_markets()
         market = self.market(symbol)
         marketId = market['id']
         request = {
             'orderId': id,
             'symbol': marketId,
         }
         params['body'] = request
-        response = self.sapiPrivatePostCancel(params)
+        response = await self.sapiPrivatePostCancel(params)
         return self.parse_canceled_order(response, market)
 
     def parse_canceled_order(self, response, market: Market) -> Order:
         id = self.safe_number(response, 'orderId')
         marketId = self.safe_string(response, 'symbol')
         symbol = self.safe_symbol(marketId, market)
         status = self.safe_string(response, 'status')
@@ -591,44 +599,44 @@
             orderStatus = 'rejected'
         return self.safe_order({
             'id': id,
             'symbol': symbol,
             'status': orderStatus,
         }, market)
 
-    def fetch_order(self, id: str, symbol: Str = None, params={}) -> Order:
-        self.load_markets()
+    async def fetch_order(self, id: str, symbol: Str = None, params={}) -> Order:
+        await self.load_markets()
         market = self.market(symbol)
         marketId = market['id']
         request = {
             'orderId': id,
             'symbol': marketId,
         }
-        response = self.sapiPrivateGetOrder(self.extend(request, params))
+        response = await self.sapiPrivateGetOrder(self.extend(request, params))
         return self.parse_order(response, market)
 
-    def fetch_open_orders(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Order]:
-        self.load_markets()
+    async def fetch_open_orders(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Order]:
+        await self.load_markets()
         market = self.market(symbol)
         marketId = market['id']
         request = {
             'symbol': marketId,
             'limit': limit,
         }
         if limit is not None:
             request['limit'] = limit
-        response = self.sapiPrivateGetOpenOrders(self.deep_extend(request, params))
+        response = await self.sapiPrivateGetOpenOrders(self.deep_extend(request, params))
         arr = self.safe_list(response, 'list', [])
         return self.parse_orders(arr, market)
 
-    def fetch_my_trades(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Trade]:
-        self.load_markets()
+    async def fetch_my_trades(self, symbol: Str = None, since: Int = None, limit: Int = None, params={}) -> List[Trade]:
+        await self.load_markets()
         market = self.market(symbol)
         marketId = market['id']
         request = {
             'symbol': marketId,
         }
         if limit is not None:
             request['limit'] = limit
-        response = self.sapiPrivateGetMyTrades(self.extend(request, params))
+        response = await self.sapiPrivateGetMyTrades(self.extend(request, params))
         trades = self.safe_list(response, 'list')
         return self.parse_trades(trades, market)
```

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/idex.py` & `ccxt-idax-adapter-4.3.26/ccxt/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/independentreserve.py` & `ccxt-idax-adapter-4.3.26/ccxt/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/indodax.py` & `ccxt-idax-adapter-4.3.26/ccxt/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/kraken.py` & `ccxt-idax-adapter-4.3.26/ccxt/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/krakenfutures.py` & `ccxt-idax-adapter-4.3.26/ccxt/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/kucoin.py` & `ccxt-idax-adapter-4.3.26/ccxt/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/kucoinfutures.py` & `ccxt-idax-adapter-4.3.26/ccxt/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/kuna.py` & `ccxt-idax-adapter-4.3.26/ccxt/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/latoken.py` & `ccxt-idax-adapter-4.3.26/ccxt/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/lbank.py` & `ccxt-idax-adapter-4.3.26/ccxt/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/luno.py` & `ccxt-idax-adapter-4.3.26/ccxt/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/lykke.py` & `ccxt-idax-adapter-4.3.26/ccxt/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/mercado.py` & `ccxt-idax-adapter-4.3.26/ccxt/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/mexc.py` & `ccxt-idax-adapter-4.3.26/ccxt/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/ndax.py` & `ccxt-idax-adapter-4.3.26/ccxt/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/novadax.py` & `ccxt-idax-adapter-4.3.26/ccxt/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/oceanex.py` & `ccxt-idax-adapter-4.3.26/ccxt/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/okcoin.py` & `ccxt-idax-adapter-4.3.26/ccxt/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/okx.py` & `ccxt-idax-adapter-4.3.26/ccxt/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/onetrading.py` & `ccxt-idax-adapter-4.3.26/ccxt/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/p2b.py` & `ccxt-idax-adapter-4.3.26/ccxt/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/paymium.py` & `ccxt-idax-adapter-4.3.26/ccxt/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/phemex.py` & `ccxt-idax-adapter-4.3.26/ccxt/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/poloniex.py` & `ccxt-idax-adapter-4.3.26/ccxt/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/poloniexfutures.py` & `ccxt-idax-adapter-4.3.26/ccxt/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/__init__.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/alpaca.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/ascendex.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/bequant.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/binance.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/binancecoinm.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/binanceus.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/binanceusdm.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/bingx.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/bitcoincom.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/bitfinex.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/bitfinex2.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/bitget.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/bithumb.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/bitmart.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/bitmex.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/bitopro.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/bitrue.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/bitstamp.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/bitvavo.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/blockchaincom.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/bybit.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/cex.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/coinbase.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/coinbaseinternational.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/coinbasepro.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/coincheck.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/coinex.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/coinone.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/cryptocom.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/currencycom.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/deribit.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/exmo.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/gate.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/gemini.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/hitbtc.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/hollaex.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/htx.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/huobijp.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/hyperliquid.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/idax.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/idax.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/idex.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/independentreserve.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/kraken.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/krakenfutures.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/kucoin.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/kucoinfutures.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/lbank.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/luno.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/mexc.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/ndax.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/okcoin.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/okx.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/onetrading.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/p2b.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/phemex.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/poloniex.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/poloniexfutures.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/probit.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/upbit.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/wazirx.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/whitebit.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/woo.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/pro/woofipro.py` & `ccxt-idax-adapter-4.3.26/ccxt/pro/woofipro.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/probit.py` & `ccxt-idax-adapter-4.3.26/ccxt/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/__init__.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/_version.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/_version.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/curves.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/curves.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/der.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/der.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/ecdsa.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/ecdsa.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/ellipticcurve.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/ellipticcurve.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/keys.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/keys.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/numbertheory.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/numbertheory.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/rfc6979.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/rfc6979.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ecdsa/util.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ecdsa/util.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/base.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/base.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/codec.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/codec.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/decoding.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/decoding.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/encoding.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/encoding.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/exceptions.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/grammar.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/grammar.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/registry.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/registry.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/abi/utils/numeric.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/abi/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/account/messages.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/account/messages.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/hexbytes/_utils.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/hexbytes/_utils.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/hexbytes/main.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/hexbytes/main.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/typing/__init__.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/typing/evm.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/typing/evm.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/typing/networks.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/typing/networks.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/__init__.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/abi.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/abi.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/address.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/address.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/applicators.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/applicators.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/conversions.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/conversions.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/currency.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/currency.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/curried/__init__.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/curried/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/decorators.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/functional.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/functional.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/hexadecimal.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/hexadecimal.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/humanize.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/logging.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/module_loading.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/numeric.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/toolz.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/toolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/types.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/types.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/ethereum/utils/units.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/ethereum/utils/units.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/keccak/keccak.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/keccak/keccak.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/msgpack/__init__.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/msgpack/exceptions.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/msgpack/ext.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/msgpack/fallback.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/parsimonious/exceptions.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/parsimonious/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/parsimonious/expressions.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/parsimonious/expressions.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/parsimonious/grammar.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/parsimonious/grammar.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/parsimonious/nodes.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/parsimonious/nodes.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/parsimonious/utils.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/parsimonious/utils.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/_signatures.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/_signatures.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/_version.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/_version.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/compatibility.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/compatibility.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/curried/__init__.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/curried/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/curried/operator.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/curried/operator.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/dicttoolz.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/dicttoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/functoolz.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/functoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/itertoolz.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/itertoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/static_dependencies/toolz/recipes.py` & `ccxt-idax-adapter-4.3.26/ccxt/static_dependencies/toolz/recipes.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/__init__.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_account.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_account.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_balance.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_balance.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_borrow_interest.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_borrow_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_borrow_rate.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_borrow_rate.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_calculate_fee.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_calculate_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_crypto.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_crypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_currency.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_currency.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_datetime.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_datetime.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_decimal_to_precision.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_deep_extend.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_deep_extend.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_deposit_withdrawal.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_deposit_withdrawal.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_exchange_datetime_functions.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_exchange_datetime_functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_funding_rate_history.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_funding_rate_history.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_last_price.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_last_price.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_ledger_entry.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_ledger_entry.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_ledger_item.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_ledger_item.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_leverage_tier.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_leverage_tier.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_margin_mode.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_margin_mode.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_margin_modification.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_margin_modification.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_market.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_market.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_number.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_number.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_ohlcv.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_ohlcv.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_open_interest.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_open_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_order.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_order.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_order_book.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_position.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_position.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_shared_methods.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_shared_methods.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_status.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_status.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_throttle.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_throttle.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_ticker.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_ticker.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_trade.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_trade.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_trading_fee.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_trading_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/base/test_transaction.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/base/test_transaction.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/test_async.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/test_async.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/test/test_sync.py` & `ccxt-idax-adapter-4.3.26/ccxt/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/timex.py` & `ccxt-idax-adapter-4.3.26/ccxt/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/tokocrypto.py` & `ccxt-idax-adapter-4.3.26/ccxt/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/tradeogre.py` & `ccxt-idax-adapter-4.3.26/ccxt/tradeogre.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/upbit.py` & `ccxt-idax-adapter-4.3.26/ccxt/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/wavesexchange.py` & `ccxt-idax-adapter-4.3.26/ccxt/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/wazirx.py` & `ccxt-idax-adapter-4.3.26/ccxt/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/whitebit.py` & `ccxt-idax-adapter-4.3.26/ccxt/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/woo.py` & `ccxt-idax-adapter-4.3.26/ccxt/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/woofipro.py` & `ccxt-idax-adapter-4.3.26/ccxt/woofipro.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/yobit.py` & `ccxt-idax-adapter-4.3.26/ccxt/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/zaif.py` & `ccxt-idax-adapter-4.3.26/ccxt/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt/zonda.py` & `ccxt-idax-adapter-4.3.26/ccxt/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/ccxt_idax_adapter.egg-info/PKG-INFO` & `ccxt-idax-adapter-4.3.26/ccxt_idax_adapter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ccxt-idax-adapter
-Version: 4.3.25
-Summary: Custom fork of ccxt
+Version: 4.3.26
+Summary: Custom version of ccxt
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://github.com/ccxt/ccxt/wiki
 Project-URL: Discord, https://discord.gg/ccxt
@@ -43,8 +43,10 @@
 Requires-Dist: yarl>=1.7.2; python_version >= "3.5.2"
 Provides-Extra: qa
 Requires-Dist: ruff==0.0.292; extra == "qa"
 Requires-Dist: tox>=4.8.0; extra == "qa"
 Provides-Extra: type
 Requires-Dist: mypy==1.6.1; extra == "type"
 
-This is a fork of [ccxt](https://github.com/ccxt/ccxt) for [idax](https://www.idax.exchange).
+# Non official version of an open source project
+
+This is a custom fork of [ccxt](https://github.com/ccxt/ccxt) for [idax](https://www.idax.exchange).
```

### Comparing `ccxt-idax-adapter-4.3.25/ccxt_idax_adapter.egg-info/SOURCES.txt` & `ccxt-idax-adapter-4.3.26/ccxt_idax_adapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccxt-idax-adapter-4.3.25/package.json` & `ccxt-idax-adapter-4.3.26/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'description'": "'Custom version of ccxt'", "'version'": "'4.3.26'"}*

```diff
@@ -14,15 +14,15 @@
         "logo": "https://opencollective.com/ccxt/logo.txt",
         "type": "opencollective",
         "url": "https://opencollective.com/ccxt"
     },
     "dependencies": {
         "ws": "^8.8.1"
     },
-    "description": "Custom fork of ccxt",
+    "description": "Custom version of ccxt",
     "devDependencies": {
         "@rollup/plugin-commonjs": "^21.0.3",
         "@rollup/plugin-json": "^4.1.0",
         "@rollup/plugin-node-resolve": "^15.2.3",
         "@types/node": "^18.15.11",
         "@typescript-eslint/eslint-plugin": "^5.30.5",
         "@typescript-eslint/parser": "^5.30.5",
@@ -268,9 +268,9 @@
         "update-links": "node build/update-links",
         "validate-types": "tsx build/validate-types.ts",
         "vss": "node build/vss"
     },
     "type": "module",
     "types": "./js/ccxt.d.ts",
     "unpkg": "dist/ccxt.browser.js",
-    "version": "4.3.25"
+    "version": "4.3.26"
 }
```

### Comparing `ccxt-idax-adapter-4.3.25/setup.py` & `ccxt-idax-adapter-4.3.26/setup.py`

 * *Files identical despite different names*

