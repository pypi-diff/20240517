# Comparing `tmp/vdg-0.2.2.tar.gz` & `tmp/vdg-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdg-0.2.2.tar", last modified: Sat May 11 23:25:46 2024, max compression
+gzip compressed data, was "vdg-0.2.4.tar", last modified: Fri May 17 09:12:56 2024, max compression
```

## Comparing `vdg-0.2.2.tar` & `vdg-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:25:46.529606 vdg-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-11 23:25:40.000000 vdg-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-11 23:25:40.000000 vdg-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-11 23:25:46.529606 vdg-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-11 23:25:40.000000 vdg-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 23:25:46.529606 vdg-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-11 23:25:40.000000 vdg-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:25:46.529606 vdg-0.2.2/vdg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 23:25:40.000000 vdg-0.2.2/vdg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-11 23:25:40.000000 vdg-0.2.2/vdg/core.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1110 2024-05-11 23:25:40.000000 vdg-0.2.2/vdg/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:25:46.529606 vdg-0.2.2/vdg/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-11 23:25:40.000000 vdg-0.2.2/vdg/templates/html.template
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-11 23:25:40.000000 vdg-0.2.2/vdg/templates/main.template
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-11 23:25:40.000000 vdg-0.2.2/vdg/templates/titles.template
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-11 23:25:40.000000 vdg-0.2.2/vdg/templates/yaml.template
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-11 23:25:40.000000 vdg-0.2.2/vdg/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-11 23:25:40.000000 vdg-0.2.2/vdg/yaml_preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:25:46.529606 vdg-0.2.2/vdg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-11 23:25:46.000000 vdg-0.2.2/vdg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-11 23:25:46.000000 vdg-0.2.2/vdg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 23:25:46.000000 vdg-0.2.2/vdg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 23:25:46.000000 vdg-0.2.2/vdg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-11 23:25:46.000000 vdg-0.2.2/vdg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:12:56.596294 vdg-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-17 09:12:51.000000 vdg-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-17 09:12:51.000000 vdg-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-17 09:12:56.592295 vdg-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-17 09:12:51.000000 vdg-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 09:12:56.596294 vdg-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-17 09:12:51.000000 vdg-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:12:56.592295 vdg-0.2.4/vdg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:12:51.000000 vdg-0.2.4/vdg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-17 09:12:51.000000 vdg-0.2.4/vdg/core.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1110 2024-05-17 09:12:51.000000 vdg-0.2.4/vdg/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:12:56.592295 vdg-0.2.4/vdg/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-17 09:12:51.000000 vdg-0.2.4/vdg/templates/html.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-17 09:12:51.000000 vdg-0.2.4/vdg/templates/main.template
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-17 09:12:51.000000 vdg-0.2.4/vdg/templates/old_page_upd.template
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-17 09:12:51.000000 vdg-0.2.4/vdg/templates/titles.template
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-17 09:12:51.000000 vdg-0.2.4/vdg/templates/yaml.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-17 09:12:51.000000 vdg-0.2.4/vdg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-17 09:12:51.000000 vdg-0.2.4/vdg/yaml_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:12:56.592295 vdg-0.2.4/vdg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-17 09:12:56.000000 vdg-0.2.4/vdg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-17 09:12:56.000000 vdg-0.2.4/vdg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:12:56.000000 vdg-0.2.4/vdg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 09:12:56.000000 vdg-0.2.4/vdg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-17 09:12:56.000000 vdg-0.2.4/vdg.egg-info/top_level.txt
```

### Comparing `vdg-0.2.2/LICENSE` & `vdg-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vdg-0.2.2/PKG-INFO` & `vdg-0.2.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdg
-Version: 0.2.2
+Version: 0.2.4
 Summary: VCB-Studio Draft Generator 发布稿生成器
 Author: diazchika
 Author-email: halberd-civic.0c@icloud.com
 Project-URL: github, https://github.com/diazchika/vdg
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vdg-0.2.2/README.md` & `vdg-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `vdg-0.2.2/setup.py` & `vdg-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="vdg",
-    version="0.2.2",
+    version="0.2.4",
     author="diazchika",
     author_email="halberd-civic.0c@icloud.com",
     description="VCB-Studio Draft Generator 发布稿生成器",
     long_description=read('README.md'),
     packages=find_packages(),
     include_package_data=True,
     package_data={
```

### Comparing `vdg-0.2.2/vdg/main.py` & `vdg-0.2.4/vdg/main.py`

 * *Files identical despite different names*

### Comparing `vdg-0.2.2/vdg/templates/html.template` & `vdg-0.2.4/vdg/templates/html.template`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 <p>
     <img src="{{ 图片链接800px }}" /><br />
     <br />
 
-{% if 分行生成 %}
-    {{ 中文 }} {{ 内容性质 }}<br />
-    {{ ENGLISH }} {{ 内容性质 }}<br />
-    {{ 日本語 }} {{ 内容性质 }}<br />
+{% for title in 正文中片名 %}
+{% if title["分行生成"] %}
+    {{ title["中文"] }} {{ title["内容性质"] }}<br />
+    {{ title["ENGLISH"] }} {{ title["内容性质"] }}<br />
+    {{ title["日本語"] }} {{ title["内容性质"] }}<br />
 {% else %}
-    {{ 中文 }} / {{ ENGLISH }} / {{ 日本語 }} {{ 内容性质 }}<br />
+    {{ title["中文"] }} / {{ title["ENGLISH"] }} / {{ title["日本語"] }} {{ title["内容性质"] }}<br />
 {% endif %}
     <br />
+{% endfor %}
 
 {% if 内嵌字幕 %}
     {{ 内嵌字幕信息 }}<br />
     {{ 内嵌字幕信息英文 }}<br />
 {% endif %}
 
 {% if 评论音轨与外挂音频 %}
@@ -21,26 +23,24 @@
     {{ 评论音轨与外挂音频信息英文 }}<br />
 {% endif %}
 {% if 评论音轨与外挂音频 or 内嵌字幕 %}
     <br />
 {% endif %}
 
 {% if 合作组 %}
-    {{ 合作组信息 }}<br />
-    {{ 合作组信息英文 }}<br />
-{% endif %}
-{% if 合作组 %}
+    这个项目与 <strong>{{合作组中文}}</strong> 合作，感谢他们精心制作的字幕。<br />
+    This project is in collaboration with <strong>{{合作组英文}}</strong>. Thanks to them for elaborating Chinese subtitles.<br />
     <br />
 {% endif %}
 
     {{ 画质吐槽_HTML }}
     {{ 画质吐槽英文_HTML }}
     <br />
 
-{% if 发布吐槽_HTML != '' %}
+{% if 发布吐槽 %}
     {{发布吐槽_HTML}}
     <br />
 {% endif %}
 </p>
 <hr />
 
 {% if not 重发 %}
@@ -77,35 +77,37 @@
 {{对比图HTML}}
 {% endif %}
 
 {% if 重发 %}
 <p>
     重发修正：<br />
     {{重发修正_HTML}}
+    <br />
     Reseed comment:<br />
     {{重发修正英文_HTML}}
+    <br />
 </p>
 <hr />
 <p>
     感谢所有参与制作者 / Thanks to our participating members: <br>
     总监 / Script: {{总监}} <br>
     压制 / Encode: {{压制}} <br>
     整理 / Collate: {{整理}} <br>
     发布 / Upload: {{发布}} <br>
     分流 / Seed: VCB-Studio CDN 分流成员 <br>
     <br>
 
     感谢所有资源提供者 / Thanks to all resource providers: <br />
-    {{来源感谢}}
+    {{来源感谢_HTML}}
     <br>
 </p>
 <hr />
 <p>
     本次发布来自 VCB-Studio 旧作重发计划。我们会不定期重发过去发布过的合集，或为补充做种，或为修正制作错漏，或为整合系列合集。<br />
-    This is a release of VCB-Studio Reseed Project. We would re-upload pervious torrents from time to time, to resurrect old torrents with few seeders, to correct errors/omissions, or to batch separate releases that belong to a same series. <br />
+    This is a release of VCB-Studio Reseed Project. We would re-upload previous torrents from time to time, to resurrect old torrents with few seeders, to correct errors/omissions, or to batch separate releases that belong to a same series. <br />
     <br />
 </p>
 <hr />
 <p>
     播放器教程索引： <a href="https://vcb-s.com/archives/16639" target="_blank">VCB-Studio 播放器推荐</a><br />
     中文字幕分享区： <a href="https://bbs.acgrip.com/" target="_blank">Anime 分享论坛</a><br />
     项目计划与列表： <a href="https://vcb-s.com/archives/138" target="_blank">VCB-Studio 项目列表</a><br />
```

#### html2text {}

```diff
@@ -1,25 +1,29 @@
 [{{ å¾çé¾æ¥800px }}]
 
-{% if åè¡çæ %} {{ ä¸­æ }} {{ åå®¹æ§è´¨ }}
-{{ ENGLISH }} {{ åå®¹æ§è´¨ }}
-{{ æ¥æ¬èª }} {{ åå®¹æ§è´¨ }}
-{% else %} {{ ä¸­æ }} / {{ ENGLISH }} / {{ æ¥æ¬èª }} {{ åå®¹æ§è´¨ }}
+{% for title in æ­£æä¸­çå %} {% if title["åè¡çæ"] %} {{ title
+["ä¸­æ"] }} {{ title["åå®¹æ§è´¨"] }}
+{{ title["ENGLISH"] }} {{ title["åå®¹æ§è´¨"] }}
+{{ title["æ¥æ¬èª"] }} {{ title["åå®¹æ§è´¨"] }}
+{% else %} {{ title["ä¸­æ"] }} / {{ title["ENGLISH"] }} / {{ title
+["æ¥æ¬èª"] }} {{ title["åå®¹æ§è´¨"] }}
 {% endif %}
-{% if ååµå­å¹ %} {{ ååµå­å¹ä¿¡æ¯ }}
+{% endfor %} {% if ååµå­å¹ %} {{ ååµå­å¹ä¿¡æ¯ }}
 {{ ååµå­å¹ä¿¡æ¯è±æ }}
 {% endif %} {% if è¯è®ºé³è½¨ä¸å¤æé³é¢ %} {
 { è¯è®ºé³è½¨ä¸å¤æé³é¢ä¿¡æ¯ }}
 {{ è¯è®ºé³è½¨ä¸å¤æé³é¢ä¿¡æ¯è±æ }}
 {% endif %} {% if è¯è®ºé³è½¨ä¸å¤æé³é¢ or ååµå­å¹ %}
-{% endif %} {% if åä½ç» %} {{ åä½ç»ä¿¡æ¯ }}
-{{ åä½ç»ä¿¡æ¯è±æ }}
-{% endif %} {% if åä½ç» %}
+{% endif %} {% if åä½ç» %} è¿ä¸ªé¡¹ç®ä¸ {{{{?å???ä?½??ç?»??ä?¸?­?æ??}}}}
+åä½ï¼æè°¢ä»ä»¬ç²¾å¿å¶ä½çå­å¹ã
+This project is in collaboration with {{{{?å???ä?½??ç?»??è??±?æ??}}}}. Thanks to them for
+elaborating Chinese subtitles.
+
 {% endif %} {{ ç»è´¨åæ§½_HTML }} {{ ç»è´¨åæ§½è±æ_HTML }}
-{% if åå¸åæ§½_HTML != '' %} {{åå¸åæ§½_HTML}}
+{% if åå¸åæ§½ %} {{åå¸åæ§½_HTML}}
 {% endif %}
 ===============================================================================
 {% if not éå %}
 æè°¢ææåä¸å¶ä½è / Thanks to our participating members:
 æ»ç / Script: {{æ»ç}}
 åå¶ / Encode: {{åå¶}}
 æ´ç / Collate: {{æ´ç}}
@@ -43,30 +47,31 @@
 ä¸­æå­å¹åäº«åºï¼ _A_n_i_m_e_ _å___ä_º_«_è_®_º_å__
 é¡¹ç®è®¡åä¸åè¡¨ï¼ _V_C_B_-_S_t_u_d_i_o_ _é_¡_¹_ç__®_å___è_¡_¨
 ç¹æ®æ ¼å¼ä¸è¯´æï¼ _W_e_b_P_ _æ__«_å__¾_è_¯_´_æ__
 
 ===============================================================================
 {{å¯¹æ¯å¾HTML}} {% endif %} {% if éå %}
 éåä¿®æ­£ï¼
-{{éåä¿®æ­£_HTML}} Reseed comment:
+{{éåä¿®æ­£_HTML}}
+Reseed comment:
 {{éåä¿®æ­£è±æ_HTML}}
 ===============================================================================
 æè°¢ææåä¸å¶ä½è / Thanks to our participating members:
 æ»ç / Script: {{æ»ç}}
 åå¶ / Encode: {{åå¶}}
 æ´ç / Collate: {{æ´ç}}
 åå¸ / Upload: {{åå¸}}
 åæµ / Seed: VCB-Studio CDN åæµæå
 
 æè°¢ææèµæºæä¾è / Thanks to all resource providers:
-{{æ¥æºæè°¢}}
+{{æ¥æºæè°¢_HTML}}
 ===============================================================================
 æ¬æ¬¡åå¸æ¥èª VCB-Studio
 æ§ä½éåè®¡åãæä»¬ä¼ä¸å®æéåè¿å»åå¸è¿çåéï¼æä¸ºè¡¥ååç§ï¼æä¸ºä¿®æ­£å¶ä½éæ¼ï¼æä¸ºæ´åç³»ååéã
-This is a release of VCB-Studio Reseed Project. We would re-upload pervious
+This is a release of VCB-Studio Reseed Project. We would re-upload previous
 torrents from time to time, to resurrect old torrents with few seeders, to
 correct errors/omissions, or to batch separate releases that belong to a same
 series.
 
 ===============================================================================
 æ­æ¾å¨æç¨ç´¢å¼ï¼ _V_C_B_-_S_t_u_d_i_o_ _æ__­_æ__¾_å__¨_æ__¨_è__
 ä¸­æå­å¹åäº«åºï¼ _A_n_i_m_e_ _å___ä_º_«_è_®_º_å__
```

### Comparing `vdg-0.2.2/vdg.egg-info/PKG-INFO` & `vdg-0.2.4/vdg.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdg
-Version: 0.2.2
+Version: 0.2.4
 Summary: VCB-Studio Draft Generator 发布稿生成器
 Author: diazchika
 Author-email: halberd-civic.0c@icloud.com
 Project-URL: github, https://github.com/diazchika/vdg
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

