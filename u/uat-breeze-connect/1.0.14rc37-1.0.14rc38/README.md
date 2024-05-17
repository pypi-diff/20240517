# Comparing `tmp/uat_breeze_connect-1.0.14rc37.tar.gz` & `tmp/uat_breeze_connect-1.0.14rc38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uat_breeze_connect-1.0.14rc37.tar", last modified: Thu Apr 25 08:26:08 2024, max compression
+gzip compressed data, was "dist\uat_breeze_connect-1.0.14rc38.tar", last modified: Fri May 17 10:03:51 2024, max compression
```

## Comparing `uat_breeze_connect-1.0.14rc37.tar` & `uat_breeze_connect-1.0.14rc38.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 08:26:08.846939 uat_breeze_connect-1.0.14rc37/
--rw-rw-rw-   0        0        0     1100 2024-04-25 08:21:17.000000 uat_breeze_connect-1.0.14rc37/LICENSE
--rw-rw-rw-   0        0        0    19998 2024-04-25 08:26:08.846939 uat_breeze_connect-1.0.14rc37/PKG-INFO
--rw-rw-rw-   0        0        0    19463 2024-04-25 08:25:27.000000 uat_breeze_connect-1.0.14rc37/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 08:26:08.815024 uat_breeze_connect-1.0.14rc37/breeze_connect/
--rw-rw-rw-   0        0        0       55 2024-04-25 08:21:17.000000 uat_breeze_connect-1.0.14rc37/breeze_connect/__init__.py
--rw-rw-rw-   0        0        0    98442 2024-04-25 08:24:34.000000 uat_breeze_connect-1.0.14rc37/breeze_connect/breeze_connect.py
--rw-rw-rw-   0        0        0       42 2024-04-25 08:26:08.848932 uat_breeze_connect-1.0.14rc37/setup.cfg
--rw-rw-rw-   0        0        0      758 2024-04-25 08:25:27.000000 uat_breeze_connect-1.0.14rc37/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:26:08.844943 uat_breeze_connect-1.0.14rc37/uat_breeze_connect.egg-info/
--rw-rw-rw-   0        0        0    19998 2024-04-25 08:26:08.000000 uat_breeze_connect-1.0.14rc37/uat_breeze_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-04-25 08:26:08.000000 uat_breeze_connect-1.0.14rc37/uat_breeze_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 08:26:08.000000 uat_breeze_connect-1.0.14rc37/uat_breeze_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-25 08:26:08.000000 uat_breeze_connect-1.0.14rc37/uat_breeze_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-25 08:26:08.000000 uat_breeze_connect-1.0.14rc37/uat_breeze_connect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 10:03:51.660234 uat_breeze_connect-1.0.14rc38/
+-rw-rw-rw-   0        0        0     1100 2024-05-17 09:48:40.000000 uat_breeze_connect-1.0.14rc38/LICENSE
+-rw-rw-rw-   0        0        0    20013 2024-05-17 10:03:51.659972 uat_breeze_connect-1.0.14rc38/PKG-INFO
+-rw-rw-rw-   0        0        0    19478 2024-05-17 10:03:38.000000 uat_breeze_connect-1.0.14rc38/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 10:03:51.555112 uat_breeze_connect-1.0.14rc38/breeze_connect/
+-rw-rw-rw-   0        0        0       55 2024-05-17 09:48:41.000000 uat_breeze_connect-1.0.14rc38/breeze_connect/__init__.py
+-rw-rw-rw-   0        0        0    98442 2024-05-17 10:02:30.000000 uat_breeze_connect-1.0.14rc38/breeze_connect/breeze_connect.py
+-rw-rw-rw-   0        0        0       42 2024-05-17 10:03:51.685066 uat_breeze_connect-1.0.14rc38/setup.cfg
+-rw-rw-rw-   0        0        0      758 2024-05-17 09:52:01.000000 uat_breeze_connect-1.0.14rc38/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:03:51.657841 uat_breeze_connect-1.0.14rc38/uat_breeze_connect.egg-info/
+-rw-rw-rw-   0        0        0    20013 2024-05-17 10:03:51.000000 uat_breeze_connect-1.0.14rc38/uat_breeze_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-17 10:03:51.000000 uat_breeze_connect-1.0.14rc38/uat_breeze_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 10:03:51.000000 uat_breeze_connect-1.0.14rc38/uat_breeze_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-17 10:03:51.000000 uat_breeze_connect-1.0.14rc38/uat_breeze_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-17 10:03:51.000000 uat_breeze_connect-1.0.14rc38/uat_breeze_connect.egg-info/top_level.txt
```

### Comparing `uat_breeze_connect-1.0.14rc37/LICENSE` & `uat_breeze_connect-1.0.14rc38/LICENSE`

 * *Files identical despite different names*

### Comparing `uat_breeze_connect-1.0.14rc37/PKG-INFO` & `uat_breeze_connect-1.0.14rc38/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uat-breeze-connect
-Version: 1.0.14rc37
+Version: 1.0.14rc38
 Summary: UAT Breeze Connect
 Home-page: https://github.com/pypa/sampleproject
 Author: UAT Breeze Connect
 Author-email: test@mail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,15 @@
 ```
 pip install --upgrade uat-breeze-connect
 ```
 
 Or, You can also install the specific release version via pip
 
 ```
-pip install uat-breeze-connect==1.0.14rc37
+pip install uat-breeze-connect==1.0.14rc38
 ```
 
 ## Websocket Usage
 <h4 id="#Web_socket">Websocket Usage</h4>
 
 ```python
 from breeze_connect import BreezeConnect
@@ -430,15 +430,15 @@
 <a href="#index">Back to Index</a>
 <hr>
 
 # square_off
 
 <h4 id="square_off1">Square off an Equity Margin Order</h4>
 <pre><code class="python" style="color:green;">breeze.square_off(exchange_code="NSE",
-                    product="margin",
+                    product_type="margin",
                     stock_code="NIFTY",
                     quantity="10",
                     price="0",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
@@ -448,30 +448,30 @@
                     cover_quantity="",
                     open_quantity="",
                     margin_amount="")</code></pre>
 # Note: Please refer get_portfolio_positions() for settlement id and margin_amount
 
 <h4 id="square_off2">Square off an FNO Futures Order</h4>
 <pre><code class="python" style="color:green;">breeze.square_off(exchange_code="NFO",
-                    product="futures",
+                    product_type="futures",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
                     quantity="50",
                     price="0",
                     validity_date="2022-08-12T06:00:00.000Z",
                     trade_password="",
                     disclosed_quantity="0")</code></pre>
 
 <h4 id="square_off3">Square off an FNO Options Order</h4>
 <pre><code class="python" style="color:green;">breeze.square_off(exchange_code="NFO",
-                    product="options",
+                    product_type="options",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     right="Call",
                     strike_price="16850",
                     action="sell",
                     order_type="market",
                     validity="day",
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: uat-breeze-connect Version: 1.0.14rc37 Summary: UAT
+Metadata-Version: 2.1 Name: uat-breeze-connect Version: 1.0.14rc38 Summary: UAT
 Breeze Connect Home-page: https://github.com/pypa/sampleproject Author: UAT
 Breeze Connect Author-email: test@mail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: python-socketio
 [client] Requires-Dist: requests Requires-Dist: pandas # Index
     * _U_A_T___B_r_e_e_z_e___C_o_n_n_e_c_t___S_D_K
@@ -40,15 +40,15 @@
 You must install the virtualenv package via pip ``` pip install virtualenv ```
 You should create breeze virtual environment via virtualenv ``` virtualenv -
 p python3 breeze_venv ``` And then, You can activate virtual environment via
 source ``` source breeze_venv/bin/activate ``` ## Installing the client
 ****** IInnssttaalllliinngg tthhee cclliieenntt ******
 You can install the latest release via pip ``` pip install --upgrade uat-
 breeze-connect ``` Or, You can also install the specific release version via
-pip ``` pip install uat-breeze-connect==1.0.14rc37 ``` ## Websocket Usage
+pip ``` pip install uat-breeze-connect==1.0.14rc38 ``` ## Websocket Usage
 ****** WWeebbssoocckkeett UUssaaggee ******
 ```python from breeze_connect import BreezeConnect # Initialize SDK breeze =
 BreezeConnect(api_key="your_api_key") # Obtain your session key from https://
 uatapi.icicidirect.com/apiuser/login?api_key=YOUR_API_KEY # Incase your api-key
 has special characters(like +,=,!) then encode the api key before using in the
 url as shown below. import urllib print("https://uatapi.icicidirect.com/
 apiuser/login?api_key="+urllib.parse.quote_plus("your_api_key")) # Generate
@@ -291,15 +291,15 @@
                     right="call",
                     strike_price="16850")
 _B_a_c_k_ _t_o_ _I_n_d_e_x
 ===============================================================================
 # square_off
 ****** SSqquuaarree ooffff aann EEqquuiittyy MMaarrggiinn OOrrddeerr ******
 breeze.square_off(exchange_code="NSE",
-                    product="margin",
+                    product_type="margin",
                     stock_code="NIFTY",
                     quantity="10",
                     price="0",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
@@ -309,29 +309,29 @@
                     cover_quantity="",
                     open_quantity="",
                     margin_amount="")
 # Note: Please refer get_portfolio_positions() for settlement id and
 margin_amount
 ****** SSqquuaarree ooffff aann FFNNOO FFuuttuurreess OOrrddeerr ******
 breeze.square_off(exchange_code="NFO",
-                    product="futures",
+                    product_type="futures",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
                     quantity="50",
                     price="0",
                     validity_date="2022-08-12T06:00:00.000Z",
                     trade_password="",
                     disclosed_quantity="0")
 ****** SSqquuaarree ooffff aann FFNNOO OOppttiioonnss OOrrddeerr ******
 breeze.square_off(exchange_code="NFO",
-                    product="options",
+                    product_type="options",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     right="Call",
                     strike_price="16850",
                     action="sell",
                     order_type="market",
                     validity="day",
```

### Comparing `uat_breeze_connect-1.0.14rc37/README.md` & `uat_breeze_connect-1.0.14rc38/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 ```
 pip install --upgrade uat-breeze-connect
 ```
 
 Or, You can also install the specific release version via pip
 
 ```
-pip install uat-breeze-connect==1.0.14rc37
+pip install uat-breeze-connect==1.0.14rc38
 ```
 
 ## Websocket Usage
 <h4 id="#Web_socket">Websocket Usage</h4>
 
 ```python
 from breeze_connect import BreezeConnect
@@ -413,15 +413,15 @@
 <a href="#index">Back to Index</a>
 <hr>
 
 # square_off
 
 <h4 id="square_off1">Square off an Equity Margin Order</h4>
 <pre><code class="python" style="color:green;">breeze.square_off(exchange_code="NSE",
-                    product="margin",
+                    product_type="margin",
                     stock_code="NIFTY",
                     quantity="10",
                     price="0",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
@@ -431,30 +431,30 @@
                     cover_quantity="",
                     open_quantity="",
                     margin_amount="")</code></pre>
 # Note: Please refer get_portfolio_positions() for settlement id and margin_amount
 
 <h4 id="square_off2">Square off an FNO Futures Order</h4>
 <pre><code class="python" style="color:green;">breeze.square_off(exchange_code="NFO",
-                    product="futures",
+                    product_type="futures",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
                     quantity="50",
                     price="0",
                     validity_date="2022-08-12T06:00:00.000Z",
                     trade_password="",
                     disclosed_quantity="0")</code></pre>
 
 <h4 id="square_off3">Square off an FNO Options Order</h4>
 <pre><code class="python" style="color:green;">breeze.square_off(exchange_code="NFO",
-                    product="options",
+                    product_type="options",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     right="Call",
                     strike_price="16850",
                     action="sell",
                     order_type="market",
                     validity="day",
```

#### html2text {}

```diff
@@ -34,15 +34,15 @@
 You must install the virtualenv package via pip ``` pip install virtualenv ```
 You should create breeze virtual environment via virtualenv ``` virtualenv -
 p python3 breeze_venv ``` And then, You can activate virtual environment via
 source ``` source breeze_venv/bin/activate ``` ## Installing the client
 ****** IInnssttaalllliinngg tthhee cclliieenntt ******
 You can install the latest release via pip ``` pip install --upgrade uat-
 breeze-connect ``` Or, You can also install the specific release version via
-pip ``` pip install uat-breeze-connect==1.0.14rc37 ``` ## Websocket Usage
+pip ``` pip install uat-breeze-connect==1.0.14rc38 ``` ## Websocket Usage
 ****** WWeebbssoocckkeett UUssaaggee ******
 ```python from breeze_connect import BreezeConnect # Initialize SDK breeze =
 BreezeConnect(api_key="your_api_key") # Obtain your session key from https://
 uatapi.icicidirect.com/apiuser/login?api_key=YOUR_API_KEY # Incase your api-key
 has special characters(like +,=,!) then encode the api key before using in the
 url as shown below. import urllib print("https://uatapi.icicidirect.com/
 apiuser/login?api_key="+urllib.parse.quote_plus("your_api_key")) # Generate
@@ -285,15 +285,15 @@
                     right="call",
                     strike_price="16850")
 _B_a_c_k_ _t_o_ _I_n_d_e_x
 ===============================================================================
 # square_off
 ****** SSqquuaarree ooffff aann EEqquuiittyy MMaarrggiinn OOrrddeerr ******
 breeze.square_off(exchange_code="NSE",
-                    product="margin",
+                    product_type="margin",
                     stock_code="NIFTY",
                     quantity="10",
                     price="0",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
@@ -303,29 +303,29 @@
                     cover_quantity="",
                     open_quantity="",
                     margin_amount="")
 # Note: Please refer get_portfolio_positions() for settlement id and
 margin_amount
 ****** SSqquuaarree ooffff aann FFNNOO FFuuttuurreess OOrrddeerr ******
 breeze.square_off(exchange_code="NFO",
-                    product="futures",
+                    product_type="futures",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
                     quantity="50",
                     price="0",
                     validity_date="2022-08-12T06:00:00.000Z",
                     trade_password="",
                     disclosed_quantity="0")
 ****** SSqquuaarree ooffff aann FFNNOO OOppttiioonnss OOrrddeerr ******
 breeze.square_off(exchange_code="NFO",
-                    product="options",
+                    product_type="options",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     right="Call",
                     strike_price="16850",
                     action="sell",
                     order_type="market",
                     validity="day",
```

### Comparing `uat_breeze_connect-1.0.14rc37/breeze_connect/breeze_connect.py` & `uat_breeze_connect-1.0.14rc38/breeze_connect/breeze_connect.py`

 * *Files identical despite different names*

### Comparing `uat_breeze_connect-1.0.14rc37/setup.py` & `uat_breeze_connect-1.0.14rc38/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="uat-breeze-connect",
-    version="1.0.14rc37",
+    version="1.0.14rc38",
     author="UAT Breeze Connect",
     author_email="test@mail.com",
     description="UAT Breeze Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['python-socketio[client]','requests','pandas'],
     url="https://github.com/pypa/sampleproject",
```

### Comparing `uat_breeze_connect-1.0.14rc37/uat_breeze_connect.egg-info/PKG-INFO` & `uat_breeze_connect-1.0.14rc38/uat_breeze_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uat-breeze-connect
-Version: 1.0.14rc37
+Version: 1.0.14rc38
 Summary: UAT Breeze Connect
 Home-page: https://github.com/pypa/sampleproject
 Author: UAT Breeze Connect
 Author-email: test@mail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,15 @@
 ```
 pip install --upgrade uat-breeze-connect
 ```
 
 Or, You can also install the specific release version via pip
 
 ```
-pip install uat-breeze-connect==1.0.14rc37
+pip install uat-breeze-connect==1.0.14rc38
 ```
 
 ## Websocket Usage
 <h4 id="#Web_socket">Websocket Usage</h4>
 
 ```python
 from breeze_connect import BreezeConnect
@@ -430,15 +430,15 @@
 <a href="#index">Back to Index</a>
 <hr>
 
 # square_off
 
 <h4 id="square_off1">Square off an Equity Margin Order</h4>
 <pre><code class="python" style="color:green;">breeze.square_off(exchange_code="NSE",
-                    product="margin",
+                    product_type="margin",
                     stock_code="NIFTY",
                     quantity="10",
                     price="0",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
@@ -448,30 +448,30 @@
                     cover_quantity="",
                     open_quantity="",
                     margin_amount="")</code></pre>
 # Note: Please refer get_portfolio_positions() for settlement id and margin_amount
 
 <h4 id="square_off2">Square off an FNO Futures Order</h4>
 <pre><code class="python" style="color:green;">breeze.square_off(exchange_code="NFO",
-                    product="futures",
+                    product_type="futures",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
                     quantity="50",
                     price="0",
                     validity_date="2022-08-12T06:00:00.000Z",
                     trade_password="",
                     disclosed_quantity="0")</code></pre>
 
 <h4 id="square_off3">Square off an FNO Options Order</h4>
 <pre><code class="python" style="color:green;">breeze.square_off(exchange_code="NFO",
-                    product="options",
+                    product_type="options",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     right="Call",
                     strike_price="16850",
                     action="sell",
                     order_type="market",
                     validity="day",
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: uat-breeze-connect Version: 1.0.14rc37 Summary: UAT
+Metadata-Version: 2.1 Name: uat-breeze-connect Version: 1.0.14rc38 Summary: UAT
 Breeze Connect Home-page: https://github.com/pypa/sampleproject Author: UAT
 Breeze Connect Author-email: test@mail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: python-socketio
 [client] Requires-Dist: requests Requires-Dist: pandas # Index
     * _U_A_T___B_r_e_e_z_e___C_o_n_n_e_c_t___S_D_K
@@ -40,15 +40,15 @@
 You must install the virtualenv package via pip ``` pip install virtualenv ```
 You should create breeze virtual environment via virtualenv ``` virtualenv -
 p python3 breeze_venv ``` And then, You can activate virtual environment via
 source ``` source breeze_venv/bin/activate ``` ## Installing the client
 ****** IInnssttaalllliinngg tthhee cclliieenntt ******
 You can install the latest release via pip ``` pip install --upgrade uat-
 breeze-connect ``` Or, You can also install the specific release version via
-pip ``` pip install uat-breeze-connect==1.0.14rc37 ``` ## Websocket Usage
+pip ``` pip install uat-breeze-connect==1.0.14rc38 ``` ## Websocket Usage
 ****** WWeebbssoocckkeett UUssaaggee ******
 ```python from breeze_connect import BreezeConnect # Initialize SDK breeze =
 BreezeConnect(api_key="your_api_key") # Obtain your session key from https://
 uatapi.icicidirect.com/apiuser/login?api_key=YOUR_API_KEY # Incase your api-key
 has special characters(like +,=,!) then encode the api key before using in the
 url as shown below. import urllib print("https://uatapi.icicidirect.com/
 apiuser/login?api_key="+urllib.parse.quote_plus("your_api_key")) # Generate
@@ -291,15 +291,15 @@
                     right="call",
                     strike_price="16850")
 _B_a_c_k_ _t_o_ _I_n_d_e_x
 ===============================================================================
 # square_off
 ****** SSqquuaarree ooffff aann EEqquuiittyy MMaarrggiinn OOrrddeerr ******
 breeze.square_off(exchange_code="NSE",
-                    product="margin",
+                    product_type="margin",
                     stock_code="NIFTY",
                     quantity="10",
                     price="0",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
@@ -309,29 +309,29 @@
                     cover_quantity="",
                     open_quantity="",
                     margin_amount="")
 # Note: Please refer get_portfolio_positions() for settlement id and
 margin_amount
 ****** SSqquuaarree ooffff aann FFNNOO FFuuttuurreess OOrrddeerr ******
 breeze.square_off(exchange_code="NFO",
-                    product="futures",
+                    product_type="futures",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     action="sell",
                     order_type="market",
                     validity="day",
                     stoploss="0",
                     quantity="50",
                     price="0",
                     validity_date="2022-08-12T06:00:00.000Z",
                     trade_password="",
                     disclosed_quantity="0")
 ****** SSqquuaarree ooffff aann FFNNOO OOppttiioonnss OOrrddeerr ******
 breeze.square_off(exchange_code="NFO",
-                    product="options",
+                    product_type="options",
                     stock_code="ICIBAN",
                     expiry_date="2022-08-25T06:00:00.000Z",
                     right="Call",
                     strike_price="16850",
                     action="sell",
                     order_type="market",
                     validity="day",
```

