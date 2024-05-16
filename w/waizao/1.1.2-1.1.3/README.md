# Comparing `tmp/waizao-1.1.2.tar.gz` & `tmp/waizao-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waizao-1.1.2.tar", last modified: Mon Apr  1 11:04:46 2024, max compression
+gzip compressed data, was "waizao-1.1.3.tar", last modified: Thu May 16 22:06:06 2024, max compression
```

## Comparing `waizao-1.1.2.tar` & `waizao-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 11:04:46.451170 waizao-1.1.2/
--rw-rw-rw-   0        0        0    11558 2024-03-28 14:33:13.000000 waizao-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     6310 2024-04-01 11:04:46.450172 waizao-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5496 2024-03-30 13:22:28.000000 waizao-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-01 11:04:46.451170 waizao-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1775 2024-04-01 10:58:03.000000 waizao-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:04:46.440197 waizao-1.1.2/waizao/
--rw-rw-rw-   0        0        0     1237 2024-04-01 11:04:38.000000 waizao-1.1.2/waizao/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:04:46.448176 waizao-1.1.2/waizao/api/
--rw-rw-rw-   0        0        0        0 2024-03-28 14:43:18.000000 waizao-1.1.2/waizao/api/__init__.py
--rw-rw-rw-   0        0        0   607700 2024-03-30 01:55:42.000000 waizao-1.1.2/waizao/api/stock_api.py
--rw-rw-rw-   0        0        0     1001 2024-03-29 13:07:25.000000 waizao-1.1.2/waizao/export_tool.py
--rw-rw-rw-   0        0        0     2574 2024-04-01 10:58:03.000000 waizao-1.1.2/waizao/stock_api_demo.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:04:46.449175 waizao-1.1.2/waizao.egg-info/
--rw-rw-rw-   0        0        0     6310 2024-04-01 11:04:46.000000 waizao-1.1.2/waizao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2024-04-01 11:04:46.000000 waizao-1.1.2/waizao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 11:04:46.000000 waizao-1.1.2/waizao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-01 11:04:46.000000 waizao-1.1.2/waizao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-01 11:04:46.000000 waizao-1.1.2/waizao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 22:06:06.164430 waizao-1.1.3/
+-rw-rw-rw-   0        0        0    11558 2024-03-28 14:33:13.000000 waizao-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     6652 2024-05-16 22:06:06.163395 waizao-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5838 2024-05-16 21:59:02.000000 waizao-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 22:06:06.164778 waizao-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1775 2024-04-01 10:58:03.000000 waizao-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 22:06:06.150351 waizao-1.1.3/waizao/
+-rw-rw-rw-   0        0        0     1237 2024-05-16 22:00:04.000000 waizao-1.1.3/waizao/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 22:06:06.161660 waizao-1.1.3/waizao/api/
+-rw-rw-rw-   0        0        0        0 2024-03-28 14:43:18.000000 waizao-1.1.3/waizao/api/__init__.py
+-rw-rw-rw-   0        0        0     1290 2024-05-16 16:25:37.000000 waizao-1.1.3/waizao/api/spider_api.py
+-rw-rw-rw-   0        0        0   607700 2024-03-30 01:55:42.000000 waizao-1.1.3/waizao/api/stock_api.py
+-rw-rw-rw-   0        0        0     2708 2024-05-16 21:59:02.000000 waizao-1.1.3/waizao/api_demo.py
+-rw-rw-rw-   0        0        0     1001 2024-03-29 13:07:25.000000 waizao-1.1.3/waizao/export_tool.py
+drwxrwxrwx   0        0        0        0 2024-05-16 22:06:06.162802 waizao-1.1.3/waizao.egg-info/
+-rw-rw-rw-   0        0        0     6652 2024-05-16 22:06:06.000000 waizao-1.1.3/waizao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2024-05-16 22:06:06.000000 waizao-1.1.3/waizao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 22:06:06.000000 waizao-1.1.3/waizao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-16 22:06:06.000000 waizao-1.1.3/waizao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 22:06:06.000000 waizao-1.1.3/waizao.egg-info/top_level.txt
```

### Comparing `waizao-1.1.2/LICENSE` & `waizao-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `waizao-1.1.2/PKG-INFO` & `waizao-1.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waizao
-Version: 1.1.2
+Version: 1.1.3
 Summary: Simple financial data interface library for Python!
 Home-page: http://waizaowang.com/
 Author: waizaowang
 Author-email: waizaowang@163.com
 Keywords: waizao,futures,fund,bond,index,finance,spider,quant,quantitative,investment,trading,data
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -27,73 +27,99 @@
   </a>
 </p>
 
 <p align=center>
    歪枣网，提供全面、准确、稳定的财经数据
 </p>
 
-##  前言
+## 前言
+
 本人80后理工科程序猿一枚，2015年初随波入流，进入股市。到目前为止，总收益仍有亏损，但股市虐我千百遍，我待股市如初恋。
 理想很丰满，现实很骨干。也许在股市这条道路上不会顺畅，但我会坚持。<br>
 我不是专家、不是财经达人，我只是千千万万散户中的一位。我会用文字来记录我对股市的理解，记录我增长的理财知识，记录一位普通的小散在股市中的成长经历。
 我会定期更新我建立的投资体系、近期积累的金融知识、股市投资的持仓盈亏等，不断成长，与诸位共勉。<br>
 一些指数类的ETF，尤其是像创业板、沪深300这类宽基指数，波动相对稳定，存在一定周期性，挖掘财经数据是存在一定价值的，这是歪哥相信的，也是一直在探索的。<br>
 
 ## 项目介绍
+
 歪枣网终于和大家见面了，非常感谢有大家的一路支持！<br>
 歪枣网提供的财经数据下载接口，主要用于财经研究，解决大家在财经研究中数据获取的问题。<br>
 通过歪枣网，能快速获取沪深股票、港股、大盘指数、基金净值、基金排行等财经数据，财经接口将提供Txt、Gson、Csv文件等多种数据形式，方便分析人员快速分析数据。<br>
 力求给大家提供更高效、全面、稳定的财经数据服务，让大家不用再担心财经数据源，专心进行策略研究，提升投资收益。<br>
 希望歪枣网提供的财经数据接口能给大家在投资上带来些许方便，在探索财富奥秘、追求财富自由的道路上，也希望有大家相伴。
 
 ## 财经数据
+
 采集数据范围包括沪深京A股、沪深京B股、港股、美股、黄金、汇率、Reits、沪深指数、香港指数、全球指数、债券指数、场内基金、沪深债券、行业板块、概念板块、地域板块等范围列表。<br>
 其中行业数据包括行业板块、概念板块、地域板块；场内基金包括ETF基金和LOF基金。<br>
 主要数据包括：<br>
+
 - 股票分钟数据，包括一分钟数据
 - 股票时线数据，包括5分钟、15分钟、30分钟、60分钟数据。
 - 股票日线数据，包括日线、周线、月线数据
 - 成分股数据，包括行业板块成分股、主要指数成分股数据。
 - 每日行情数据，每天股票各种指标数据采集，内盘、外盘、资金流向等
 - 分时成交Level2数据
 - 实时数据，提供交易日当天实时交易数据<br>
-更多数据请访问网站：[歪枣网](http://www.waizaowang.com/)
-
+  更多数据请访问网站：[歪枣网](http://www.waizaowang.com/)
 
 ## 项目特点
+
 主要功能包括:<br>
 1、选择模式，网站左上角菜单栏可以选择模式，包括文档模式、浏览模式、图表模式。
+
 - 文档模式：提供接口十分详细的说明文档，详细展示了接口的入参、出参，包括字段的含义以及相关说明。
 - 浏览模式：提供可视化获取数据的操作界面，用户获取数据完全可以在界面上操作，并且根据用户的操作，在页面下方可以实时生成获取数据的代码。
 - 图表模式：提供股票数据的绘图功能，包括生成曲线图和柱状图。
 
 2、支持过滤条件，可以灵活的设置过滤条件，定制返回数据，不需要用户二次开发去过滤数据。 <br>
 3、接口搜索，展示所有接口信息，可以使用 Ctrl+F 快捷键，搜索你所需要的数据字段。<br>
 4、支持的请求类型，支持GET方法和POST方法，且两种请求方式的路径和入参均相同。<br>
 5、接口更新信息，包括接口更新周期、接口最后更新时间、接口更新耗时会在页面上更新。<br><br>
 ![image](./doc/images/apiOne.png)
 ![image](./doc/images/apiTwo.png)
 ![image](./doc/images/apiThree.png)
 
-
 ## 项目地址
+
 目前项目托管在 Gitee 和 Github 平台上中，欢迎大家 Star 和 Fork 支持~ <br>
-Gitee地址： <br>
-Java SDK：https://gitee.com/waizao/StockApiJava <br>
-Python SDK:https://gitee.com/waizao/StockApiPython <br>
-Github地址： <br>
-Java SDK：https://github.com/waizao/StockApiJava <br>
-Python SDK:https://github.com/waizao/StockApiPython <br>
 
-[社区论坛](http://bbs.waizaowang.com/) <br>
-[二次开发手册](http://www.waizaowang.com/wiki/index.html#_%E4%BA%8C%E6%AC%A1%E5%BC%80%E5%8F%91)<br>
+### Java SDK :
+
+Gitee地址：https://gitee.com/waizao/StockApiJava <br>
+Github地址：https://github.com/waizao/StockApiJava <br>
+
+#### 初始化:
+
+``` maven
+<dependency>
+    <groupId>io.gitee.waizao</groupId>
+    <artifactId>openapi</artifactId>
+    <version>1.1.3</version>
+</dependency>
+```
+
+### Python SDK:
+
+Gitee地址：https://gitee.com/waizao/StockApiPython <br>
+Github地址：:https://github.com/waizao/StockApiPython <br>
+
+#### 初始化:
+
+```shell
+pip install waizao -i http://mirrors.aliyun.com/pypi/simple/ --trusted-host=mirrors.aliyun.com  --upgrade
+```
 
 ## 关注&交流
-为了方便小伙伴们沟通交流，创建了QQ群 (加群备注：歪枣网) ，目前项目还存在很多不足之处，欢迎各位大佬进群进行交流，为了防止广告进入，希望加群的时候能添加备注，谢谢~<br>
+
+为了方便小伙伴们沟通交流，创建了QQ群 (加群备注：歪枣网)
+，目前项目还存在很多不足之处，欢迎各位大佬进群进行交流，为了防止广告进入，希望加群的时候能添加备注，谢谢~<br>
 如遇问题联系作者，邮箱：waizaowang@163.com <br>
+[社区论坛](http://bbs.waizaowang.com/) <br>
+[二次开发手册](http://www.waizaowang.com/wiki/index.html#_%E4%BA%8C%E6%AC%A1%E5%BC%80%E5%8F%91)<br>
 
 |                                微信公众号                                 | QQ群【推荐】                                                                                  |
 |:--------------------------------------------------------------------:|------------------------------------------------------------------------------------------|
 | <img src="./doc/images/gongzhonghao.png" width="200" height="200" /> | <img src="./doc/images/qqGroup.png" width="200"  height="200" /> |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waizao Version: 1.1.2 Summary: Simple financial
+Metadata-Version: 2.1 Name: waizao Version: 1.1.3 Summary: Simple financial
 data interface library for Python! Home-page: http://waizaowang.com/ Author:
 waizaowang Author-email: waizaowang@163.com Keywords:
 waizao,futures,fund,bond,index,finance,spider,quant,quantitative,investment,trading,data
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: License :: OSI Approved :: MIT License
@@ -50,24 +50,25 @@
 å¿«æ·é®ï¼æç´¢ä½ æéè¦çæ°æ®å­æ®µã
 4ãæ¯æçè¯·æ±ç±»åï¼æ¯æGETæ¹æ³åPOSTæ¹æ³ï¼ä¸ä¸¤ç§è¯·æ±æ¹å¼çè·¯å¾åå¥ååç¸åã
 5ãæ¥å£æ´æ°ä¿¡æ¯ï¼åæ¬æ¥å£æ´æ°å¨æãæ¥å£æåæ´æ°æ¶é´ãæ¥å£æ´æ°èæ¶ä¼å¨é¡µé¢ä¸æ´æ°ã
 
 ![image](./doc/images/apiOne.png) ![image](./doc/images/apiTwo.png) ![image](./
 doc/images/apiThree.png) ## é¡¹ç®å°å ç®åé¡¹ç®æç®¡å¨ Gitee å Github
 å¹³å°ä¸ä¸­ï¼æ¬¢è¿å¤§å®¶ Star å Fork æ¯æ~
-Giteeå°åï¼
-Java SDKï¼https://gitee.com/waizao/StockApiJava
-Python SDK:https://gitee.com/waizao/StockApiPython
-Githubå°åï¼
-Java SDKï¼https://github.com/waizao/StockApiJava
-Python SDK:https://github.com/waizao/StockApiPython
-[ç¤¾åºè®ºå](http://bbs.waizaowang.com/)
-[äºæ¬¡å¼åæå](http://www.waizaowang.com/wiki/
-index.html#_%E4%BA%8C%E6%AC%A1%E5%BC%80%E5%8F%91)
-## å³æ³¨&äº¤æµ ä¸ºäºæ¹ä¾¿å°ä¼ä¼´ä»¬æ²éäº¤æµï¼åå»ºäºQQç¾¤
+### Java SDK : Giteeå°åï¼https://gitee.com/waizao/StockApiJava
+Githubå°åï¼https://github.com/waizao/StockApiJava
+#### åå§å: ``` maven io.gitee.waizao openapi 1.1.3 ``` ### Python SDK:
+Giteeå°åï¼https://gitee.com/waizao/StockApiPython
+Githubå°åï¼:https://github.com/waizao/StockApiPython
+#### åå§å: ```shell pip install waizao -i http://mirrors.aliyun.com/pypi/
+simple/ --trusted-host=mirrors.aliyun.com --upgrade ``` ## å³æ³¨&äº¤æµ
+ä¸ºäºæ¹ä¾¿å°ä¼ä¼´ä»¬æ²éäº¤æµï¼åå»ºäºQQç¾¤
 (å ç¾¤å¤æ³¨ï¼æ­ªæ£ç½)
 ï¼ç®åé¡¹ç®è¿å­å¨å¾å¤ä¸è¶³ä¹å¤ï¼æ¬¢è¿åä½å¤§ä½¬è¿ç¾¤è¿è¡äº¤æµï¼ä¸ºäºé²æ­¢å¹¿åè¿å¥ï¼å¸æå ç¾¤çæ¶åè½æ·»å å¤æ³¨ï¼è°¢è°¢~
 å¦éé®é¢èç³»ä½èï¼é®ç®±ï¼waizaowang@163.com
+[ç¤¾åºè®ºå](http://bbs.waizaowang.com/)
+[äºæ¬¡å¼åæå](http://www.waizaowang.com/wiki/
+index.html#_%E4%BA%8C%E6%AC%A1%E5%BC%80%E5%8F%91)
 | å¾®ä¿¡å¬ä¼å· | QQç¾¤ãæ¨èã | |:-------------------------------------
 -------------------------------:|----------------------------------------------
 --------------------------------------------| | [./doc/images/
 gongzhonghao.png]| [./doc/images/qqGroup.png]|
```

### Comparing `waizao-1.1.2/README.md` & `waizao-1.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,73 +6,99 @@
   </a>
 </p>
 
 <p align=center>
    歪枣网，提供全面、准确、稳定的财经数据
 </p>
 
-##  前言
+## 前言
+
 本人80后理工科程序猿一枚，2015年初随波入流，进入股市。到目前为止，总收益仍有亏损，但股市虐我千百遍，我待股市如初恋。
 理想很丰满，现实很骨干。也许在股市这条道路上不会顺畅，但我会坚持。<br>
 我不是专家、不是财经达人，我只是千千万万散户中的一位。我会用文字来记录我对股市的理解，记录我增长的理财知识，记录一位普通的小散在股市中的成长经历。
 我会定期更新我建立的投资体系、近期积累的金融知识、股市投资的持仓盈亏等，不断成长，与诸位共勉。<br>
 一些指数类的ETF，尤其是像创业板、沪深300这类宽基指数，波动相对稳定，存在一定周期性，挖掘财经数据是存在一定价值的，这是歪哥相信的，也是一直在探索的。<br>
 
 ## 项目介绍
+
 歪枣网终于和大家见面了，非常感谢有大家的一路支持！<br>
 歪枣网提供的财经数据下载接口，主要用于财经研究，解决大家在财经研究中数据获取的问题。<br>
 通过歪枣网，能快速获取沪深股票、港股、大盘指数、基金净值、基金排行等财经数据，财经接口将提供Txt、Gson、Csv文件等多种数据形式，方便分析人员快速分析数据。<br>
 力求给大家提供更高效、全面、稳定的财经数据服务，让大家不用再担心财经数据源，专心进行策略研究，提升投资收益。<br>
 希望歪枣网提供的财经数据接口能给大家在投资上带来些许方便，在探索财富奥秘、追求财富自由的道路上，也希望有大家相伴。
 
 ## 财经数据
+
 采集数据范围包括沪深京A股、沪深京B股、港股、美股、黄金、汇率、Reits、沪深指数、香港指数、全球指数、债券指数、场内基金、沪深债券、行业板块、概念板块、地域板块等范围列表。<br>
 其中行业数据包括行业板块、概念板块、地域板块；场内基金包括ETF基金和LOF基金。<br>
 主要数据包括：<br>
+
 - 股票分钟数据，包括一分钟数据
 - 股票时线数据，包括5分钟、15分钟、30分钟、60分钟数据。
 - 股票日线数据，包括日线、周线、月线数据
 - 成分股数据，包括行业板块成分股、主要指数成分股数据。
 - 每日行情数据，每天股票各种指标数据采集，内盘、外盘、资金流向等
 - 分时成交Level2数据
 - 实时数据，提供交易日当天实时交易数据<br>
-更多数据请访问网站：[歪枣网](http://www.waizaowang.com/)
-
+  更多数据请访问网站：[歪枣网](http://www.waizaowang.com/)
 
 ## 项目特点
+
 主要功能包括:<br>
 1、选择模式，网站左上角菜单栏可以选择模式，包括文档模式、浏览模式、图表模式。
+
 - 文档模式：提供接口十分详细的说明文档，详细展示了接口的入参、出参，包括字段的含义以及相关说明。
 - 浏览模式：提供可视化获取数据的操作界面，用户获取数据完全可以在界面上操作，并且根据用户的操作，在页面下方可以实时生成获取数据的代码。
 - 图表模式：提供股票数据的绘图功能，包括生成曲线图和柱状图。
 
 2、支持过滤条件，可以灵活的设置过滤条件，定制返回数据，不需要用户二次开发去过滤数据。 <br>
 3、接口搜索，展示所有接口信息，可以使用 Ctrl+F 快捷键，搜索你所需要的数据字段。<br>
 4、支持的请求类型，支持GET方法和POST方法，且两种请求方式的路径和入参均相同。<br>
 5、接口更新信息，包括接口更新周期、接口最后更新时间、接口更新耗时会在页面上更新。<br><br>
 ![image](./doc/images/apiOne.png)
 ![image](./doc/images/apiTwo.png)
 ![image](./doc/images/apiThree.png)
 
-
 ## 项目地址
+
 目前项目托管在 Gitee 和 Github 平台上中，欢迎大家 Star 和 Fork 支持~ <br>
-Gitee地址： <br>
-Java SDK：https://gitee.com/waizao/StockApiJava <br>
-Python SDK:https://gitee.com/waizao/StockApiPython <br>
-Github地址： <br>
-Java SDK：https://github.com/waizao/StockApiJava <br>
-Python SDK:https://github.com/waizao/StockApiPython <br>
 
-[社区论坛](http://bbs.waizaowang.com/) <br>
-[二次开发手册](http://www.waizaowang.com/wiki/index.html#_%E4%BA%8C%E6%AC%A1%E5%BC%80%E5%8F%91)<br>
+### Java SDK :
+
+Gitee地址：https://gitee.com/waizao/StockApiJava <br>
+Github地址：https://github.com/waizao/StockApiJava <br>
+
+#### 初始化:
+
+``` maven
+<dependency>
+    <groupId>io.gitee.waizao</groupId>
+    <artifactId>openapi</artifactId>
+    <version>1.1.3</version>
+</dependency>
+```
+
+### Python SDK:
+
+Gitee地址：https://gitee.com/waizao/StockApiPython <br>
+Github地址：:https://github.com/waizao/StockApiPython <br>
+
+#### 初始化:
+
+```shell
+pip install waizao -i http://mirrors.aliyun.com/pypi/simple/ --trusted-host=mirrors.aliyun.com  --upgrade
+```
 
 ## 关注&交流
-为了方便小伙伴们沟通交流，创建了QQ群 (加群备注：歪枣网) ，目前项目还存在很多不足之处，欢迎各位大佬进群进行交流，为了防止广告进入，希望加群的时候能添加备注，谢谢~<br>
+
+为了方便小伙伴们沟通交流，创建了QQ群 (加群备注：歪枣网)
+，目前项目还存在很多不足之处，欢迎各位大佬进群进行交流，为了防止广告进入，希望加群的时候能添加备注，谢谢~<br>
 如遇问题联系作者，邮箱：waizaowang@163.com <br>
+[社区论坛](http://bbs.waizaowang.com/) <br>
+[二次开发手册](http://www.waizaowang.com/wiki/index.html#_%E4%BA%8C%E6%AC%A1%E5%BC%80%E5%8F%91)<br>
 
 |                                微信公众号                                 | QQ群【推荐】                                                                                  |
 |:--------------------------------------------------------------------:|------------------------------------------------------------------------------------------|
 | <img src="./doc/images/gongzhonghao.png" width="200" height="200" /> | <img src="./doc/images/qqGroup.png" width="200"  height="200" /> |
```

#### html2text {}

```diff
@@ -40,24 +40,25 @@
 å¿«æ·é®ï¼æç´¢ä½ æéè¦çæ°æ®å­æ®µã
 4ãæ¯æçè¯·æ±ç±»åï¼æ¯æGETæ¹æ³åPOSTæ¹æ³ï¼ä¸ä¸¤ç§è¯·æ±æ¹å¼çè·¯å¾åå¥ååç¸åã
 5ãæ¥å£æ´æ°ä¿¡æ¯ï¼åæ¬æ¥å£æ´æ°å¨æãæ¥å£æåæ´æ°æ¶é´ãæ¥å£æ´æ°èæ¶ä¼å¨é¡µé¢ä¸æ´æ°ã
 
 ![image](./doc/images/apiOne.png) ![image](./doc/images/apiTwo.png) ![image](./
 doc/images/apiThree.png) ## é¡¹ç®å°å ç®åé¡¹ç®æç®¡å¨ Gitee å Github
 å¹³å°ä¸ä¸­ï¼æ¬¢è¿å¤§å®¶ Star å Fork æ¯æ~
-Giteeå°åï¼
-Java SDKï¼https://gitee.com/waizao/StockApiJava
-Python SDK:https://gitee.com/waizao/StockApiPython
-Githubå°åï¼
-Java SDKï¼https://github.com/waizao/StockApiJava
-Python SDK:https://github.com/waizao/StockApiPython
-[ç¤¾åºè®ºå](http://bbs.waizaowang.com/)
-[äºæ¬¡å¼åæå](http://www.waizaowang.com/wiki/
-index.html#_%E4%BA%8C%E6%AC%A1%E5%BC%80%E5%8F%91)
-## å³æ³¨&äº¤æµ ä¸ºäºæ¹ä¾¿å°ä¼ä¼´ä»¬æ²éäº¤æµï¼åå»ºäºQQç¾¤
+### Java SDK : Giteeå°åï¼https://gitee.com/waizao/StockApiJava
+Githubå°åï¼https://github.com/waizao/StockApiJava
+#### åå§å: ``` maven io.gitee.waizao openapi 1.1.3 ``` ### Python SDK:
+Giteeå°åï¼https://gitee.com/waizao/StockApiPython
+Githubå°åï¼:https://github.com/waizao/StockApiPython
+#### åå§å: ```shell pip install waizao -i http://mirrors.aliyun.com/pypi/
+simple/ --trusted-host=mirrors.aliyun.com --upgrade ``` ## å³æ³¨&äº¤æµ
+ä¸ºäºæ¹ä¾¿å°ä¼ä¼´ä»¬æ²éäº¤æµï¼åå»ºäºQQç¾¤
 (å ç¾¤å¤æ³¨ï¼æ­ªæ£ç½)
 ï¼ç®åé¡¹ç®è¿å­å¨å¾å¤ä¸è¶³ä¹å¤ï¼æ¬¢è¿åä½å¤§ä½¬è¿ç¾¤è¿è¡äº¤æµï¼ä¸ºäºé²æ­¢å¹¿åè¿å¥ï¼å¸æå ç¾¤çæ¶åè½æ·»å å¤æ³¨ï¼è°¢è°¢~
 å¦éé®é¢èç³»ä½èï¼é®ç®±ï¼waizaowang@163.com
+[ç¤¾åºè®ºå](http://bbs.waizaowang.com/)
+[äºæ¬¡å¼åæå](http://www.waizaowang.com/wiki/
+index.html#_%E4%BA%8C%E6%AC%A1%E5%BC%80%E5%8F%91)
 | å¾®ä¿¡å¬ä¼å· | QQç¾¤ãæ¨èã | |:-------------------------------------
 -------------------------------:|----------------------------------------------
 --------------------------------------------| | [./doc/images/
 gongzhonghao.png]| [./doc/images/qqGroup.png]|
```

### Comparing `waizao-1.1.2/setup.py` & `waizao-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `waizao-1.1.2/waizao/__init__.py` & `waizao-1.1.3/waizao/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 歪枣网终于和大家见面了，非常感谢有大家的一路支持！
 歪枣网提供的财经数据下载接口，主要用于财经研究，解决大家在财经研究中数据获取的问题。
 通过歪枣网，能快速获取沪深股票、港股、大盘指数、基金净值、基金排行等财经数据，财经接口将提供Txt、Gson、Csv文件等多种数据形式，方便分析人员快速分析数据。
 力求给大家提供更高效、全面、稳定的财经数据服务，让大家不用再担心财经数据源，专心进行策略研究，提升投资收益。
 希望歪枣网提供的财经数据接口能给大家在投资上带来些许方便，在探索财富奥秘、追求财富自由的道路上，也希望有大家相伴。
 """
 
-__version__ = "1.1.2"
+__version__ = "1.1.3"
 __author__ = "waizaowang"
 
 import sys
 import warnings
 
 import pandas as pd
```

### Comparing `waizao-1.1.2/waizao/api/stock_api.py` & `waizao-1.1.3/waizao/api/stock_api.py`

 * *Files identical despite different names*

### Comparing `waizao-1.1.2/waizao/export_tool.py` & `waizao-1.1.3/waizao/export_tool.py`

 * *Files identical despite different names*

### Comparing `waizao-1.1.2/waizao/stock_api_demo.py` & `waizao-1.1.3/waizao/api_demo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import os
 
 from waizao import export_tool
+from waizao.api import spider_api
 from waizao.api import stock_api
 
 """
 1、stock_api.py中函数名与歪枣网开发文档中接口请求URL名称保持一致，方便查找。采用驼峰命名法
 2、spider_api.py中定义了一些行情数据抓取方法
 """
 
 if __name__ == '__main__':
     print("StockApiDemo")
-    token: str = "e80da5d374d50461fd52080d43a0f591"  # 歪枣网（www.waizaowang.com）上登录后获取Token
+    token: str = ""  # 歪枣网（www.waizaowang.com）上登录后获取Token
+
+    #买卖五档，盘口数据
+    data_list: [] = spider_api.get_pankou("sz000001,sh600000,bj833171")
+    print(data_list)
 
     # 请求日线数据，返回JSON格式
     data: str = stock_api.getDayKLine(
         1,
         "all",  # 请求A股所有股票
         101,
         1,
```

### Comparing `waizao-1.1.2/waizao.egg-info/PKG-INFO` & `waizao-1.1.3/waizao.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waizao
-Version: 1.1.2
+Version: 1.1.3
 Summary: Simple financial data interface library for Python!
 Home-page: http://waizaowang.com/
 Author: waizaowang
 Author-email: waizaowang@163.com
 Keywords: waizao,futures,fund,bond,index,finance,spider,quant,quantitative,investment,trading,data
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -27,73 +27,99 @@
   </a>
 </p>
 
 <p align=center>
    歪枣网，提供全面、准确、稳定的财经数据
 </p>
 
-##  前言
+## 前言
+
 本人80后理工科程序猿一枚，2015年初随波入流，进入股市。到目前为止，总收益仍有亏损，但股市虐我千百遍，我待股市如初恋。
 理想很丰满，现实很骨干。也许在股市这条道路上不会顺畅，但我会坚持。<br>
 我不是专家、不是财经达人，我只是千千万万散户中的一位。我会用文字来记录我对股市的理解，记录我增长的理财知识，记录一位普通的小散在股市中的成长经历。
 我会定期更新我建立的投资体系、近期积累的金融知识、股市投资的持仓盈亏等，不断成长，与诸位共勉。<br>
 一些指数类的ETF，尤其是像创业板、沪深300这类宽基指数，波动相对稳定，存在一定周期性，挖掘财经数据是存在一定价值的，这是歪哥相信的，也是一直在探索的。<br>
 
 ## 项目介绍
+
 歪枣网终于和大家见面了，非常感谢有大家的一路支持！<br>
 歪枣网提供的财经数据下载接口，主要用于财经研究，解决大家在财经研究中数据获取的问题。<br>
 通过歪枣网，能快速获取沪深股票、港股、大盘指数、基金净值、基金排行等财经数据，财经接口将提供Txt、Gson、Csv文件等多种数据形式，方便分析人员快速分析数据。<br>
 力求给大家提供更高效、全面、稳定的财经数据服务，让大家不用再担心财经数据源，专心进行策略研究，提升投资收益。<br>
 希望歪枣网提供的财经数据接口能给大家在投资上带来些许方便，在探索财富奥秘、追求财富自由的道路上，也希望有大家相伴。
 
 ## 财经数据
+
 采集数据范围包括沪深京A股、沪深京B股、港股、美股、黄金、汇率、Reits、沪深指数、香港指数、全球指数、债券指数、场内基金、沪深债券、行业板块、概念板块、地域板块等范围列表。<br>
 其中行业数据包括行业板块、概念板块、地域板块；场内基金包括ETF基金和LOF基金。<br>
 主要数据包括：<br>
+
 - 股票分钟数据，包括一分钟数据
 - 股票时线数据，包括5分钟、15分钟、30分钟、60分钟数据。
 - 股票日线数据，包括日线、周线、月线数据
 - 成分股数据，包括行业板块成分股、主要指数成分股数据。
 - 每日行情数据，每天股票各种指标数据采集，内盘、外盘、资金流向等
 - 分时成交Level2数据
 - 实时数据，提供交易日当天实时交易数据<br>
-更多数据请访问网站：[歪枣网](http://www.waizaowang.com/)
-
+  更多数据请访问网站：[歪枣网](http://www.waizaowang.com/)
 
 ## 项目特点
+
 主要功能包括:<br>
 1、选择模式，网站左上角菜单栏可以选择模式，包括文档模式、浏览模式、图表模式。
+
 - 文档模式：提供接口十分详细的说明文档，详细展示了接口的入参、出参，包括字段的含义以及相关说明。
 - 浏览模式：提供可视化获取数据的操作界面，用户获取数据完全可以在界面上操作，并且根据用户的操作，在页面下方可以实时生成获取数据的代码。
 - 图表模式：提供股票数据的绘图功能，包括生成曲线图和柱状图。
 
 2、支持过滤条件，可以灵活的设置过滤条件，定制返回数据，不需要用户二次开发去过滤数据。 <br>
 3、接口搜索，展示所有接口信息，可以使用 Ctrl+F 快捷键，搜索你所需要的数据字段。<br>
 4、支持的请求类型，支持GET方法和POST方法，且两种请求方式的路径和入参均相同。<br>
 5、接口更新信息，包括接口更新周期、接口最后更新时间、接口更新耗时会在页面上更新。<br><br>
 ![image](./doc/images/apiOne.png)
 ![image](./doc/images/apiTwo.png)
 ![image](./doc/images/apiThree.png)
 
-
 ## 项目地址
+
 目前项目托管在 Gitee 和 Github 平台上中，欢迎大家 Star 和 Fork 支持~ <br>
-Gitee地址： <br>
-Java SDK：https://gitee.com/waizao/StockApiJava <br>
-Python SDK:https://gitee.com/waizao/StockApiPython <br>
-Github地址： <br>
-Java SDK：https://github.com/waizao/StockApiJava <br>
-Python SDK:https://github.com/waizao/StockApiPython <br>
 
-[社区论坛](http://bbs.waizaowang.com/) <br>
-[二次开发手册](http://www.waizaowang.com/wiki/index.html#_%E4%BA%8C%E6%AC%A1%E5%BC%80%E5%8F%91)<br>
+### Java SDK :
+
+Gitee地址：https://gitee.com/waizao/StockApiJava <br>
+Github地址：https://github.com/waizao/StockApiJava <br>
+
+#### 初始化:
+
+``` maven
+<dependency>
+    <groupId>io.gitee.waizao</groupId>
+    <artifactId>openapi</artifactId>
+    <version>1.1.3</version>
+</dependency>
+```
+
+### Python SDK:
+
+Gitee地址：https://gitee.com/waizao/StockApiPython <br>
+Github地址：:https://github.com/waizao/StockApiPython <br>
+
+#### 初始化:
+
+```shell
+pip install waizao -i http://mirrors.aliyun.com/pypi/simple/ --trusted-host=mirrors.aliyun.com  --upgrade
+```
 
 ## 关注&交流
-为了方便小伙伴们沟通交流，创建了QQ群 (加群备注：歪枣网) ，目前项目还存在很多不足之处，欢迎各位大佬进群进行交流，为了防止广告进入，希望加群的时候能添加备注，谢谢~<br>
+
+为了方便小伙伴们沟通交流，创建了QQ群 (加群备注：歪枣网)
+，目前项目还存在很多不足之处，欢迎各位大佬进群进行交流，为了防止广告进入，希望加群的时候能添加备注，谢谢~<br>
 如遇问题联系作者，邮箱：waizaowang@163.com <br>
+[社区论坛](http://bbs.waizaowang.com/) <br>
+[二次开发手册](http://www.waizaowang.com/wiki/index.html#_%E4%BA%8C%E6%AC%A1%E5%BC%80%E5%8F%91)<br>
 
 |                                微信公众号                                 | QQ群【推荐】                                                                                  |
 |:--------------------------------------------------------------------:|------------------------------------------------------------------------------------------|
 | <img src="./doc/images/gongzhonghao.png" width="200" height="200" /> | <img src="./doc/images/qqGroup.png" width="200"  height="200" /> |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waizao Version: 1.1.2 Summary: Simple financial
+Metadata-Version: 2.1 Name: waizao Version: 1.1.3 Summary: Simple financial
 data interface library for Python! Home-page: http://waizaowang.com/ Author:
 waizaowang Author-email: waizaowang@163.com Keywords:
 waizao,futures,fund,bond,index,finance,spider,quant,quantitative,investment,trading,data
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: License :: OSI Approved :: MIT License
@@ -50,24 +50,25 @@
 å¿«æ·é®ï¼æç´¢ä½ æéè¦çæ°æ®å­æ®µã
 4ãæ¯æçè¯·æ±ç±»åï¼æ¯æGETæ¹æ³åPOSTæ¹æ³ï¼ä¸ä¸¤ç§è¯·æ±æ¹å¼çè·¯å¾åå¥ååç¸åã
 5ãæ¥å£æ´æ°ä¿¡æ¯ï¼åæ¬æ¥å£æ´æ°å¨æãæ¥å£æåæ´æ°æ¶é´ãæ¥å£æ´æ°èæ¶ä¼å¨é¡µé¢ä¸æ´æ°ã
 
 ![image](./doc/images/apiOne.png) ![image](./doc/images/apiTwo.png) ![image](./
 doc/images/apiThree.png) ## é¡¹ç®å°å ç®åé¡¹ç®æç®¡å¨ Gitee å Github
 å¹³å°ä¸ä¸­ï¼æ¬¢è¿å¤§å®¶ Star å Fork æ¯æ~
-Giteeå°åï¼
-Java SDKï¼https://gitee.com/waizao/StockApiJava
-Python SDK:https://gitee.com/waizao/StockApiPython
-Githubå°åï¼
-Java SDKï¼https://github.com/waizao/StockApiJava
-Python SDK:https://github.com/waizao/StockApiPython
-[ç¤¾åºè®ºå](http://bbs.waizaowang.com/)
-[äºæ¬¡å¼åæå](http://www.waizaowang.com/wiki/
-index.html#_%E4%BA%8C%E6%AC%A1%E5%BC%80%E5%8F%91)
-## å³æ³¨&äº¤æµ ä¸ºäºæ¹ä¾¿å°ä¼ä¼´ä»¬æ²éäº¤æµï¼åå»ºäºQQç¾¤
+### Java SDK : Giteeå°åï¼https://gitee.com/waizao/StockApiJava
+Githubå°åï¼https://github.com/waizao/StockApiJava
+#### åå§å: ``` maven io.gitee.waizao openapi 1.1.3 ``` ### Python SDK:
+Giteeå°åï¼https://gitee.com/waizao/StockApiPython
+Githubå°åï¼:https://github.com/waizao/StockApiPython
+#### åå§å: ```shell pip install waizao -i http://mirrors.aliyun.com/pypi/
+simple/ --trusted-host=mirrors.aliyun.com --upgrade ``` ## å³æ³¨&äº¤æµ
+ä¸ºäºæ¹ä¾¿å°ä¼ä¼´ä»¬æ²éäº¤æµï¼åå»ºäºQQç¾¤
 (å ç¾¤å¤æ³¨ï¼æ­ªæ£ç½)
 ï¼ç®åé¡¹ç®è¿å­å¨å¾å¤ä¸è¶³ä¹å¤ï¼æ¬¢è¿åä½å¤§ä½¬è¿ç¾¤è¿è¡äº¤æµï¼ä¸ºäºé²æ­¢å¹¿åè¿å¥ï¼å¸æå ç¾¤çæ¶åè½æ·»å å¤æ³¨ï¼è°¢è°¢~
 å¦éé®é¢èç³»ä½èï¼é®ç®±ï¼waizaowang@163.com
+[ç¤¾åºè®ºå](http://bbs.waizaowang.com/)
+[äºæ¬¡å¼åæå](http://www.waizaowang.com/wiki/
+index.html#_%E4%BA%8C%E6%AC%A1%E5%BC%80%E5%8F%91)
 | å¾®ä¿¡å¬ä¼å· | QQç¾¤ãæ¨èã | |:-------------------------------------
 -------------------------------:|----------------------------------------------
 --------------------------------------------| | [./doc/images/
 gongzhonghao.png]| [./doc/images/qqGroup.png]|
```

