# Comparing `tmp/g2p-mix-0.4.2.tar.gz` & `tmp/g2p-mix-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2p-mix-0.4.2.tar", last modified: Sat May 11 10:41:10 2024, max compression
+gzip compressed data, was "g2p-mix-0.4.5.tar", last modified: Fri May 17 06:07:00 2024, max compression
```

## Comparing `g2p-mix-0.4.2.tar` & `g2p-mix-0.4.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:41:10.368895 g2p-mix-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-11 10:41:10.368895 g2p-mix-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:41:10.360895 g2p-mix-0.4.2/g2p_mix/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/g2p_eng.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/g2p_jyut.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/g2p_mix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/g2p_pth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:41:10.360895 g2p-mix-0.4.2/g2p_mix/nltk_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:41:10.360895 g2p-mix-0.4.2/g2p_mix/nltk_data/corpora/
--rw-r--r--   0 runner    (1001) docker     (127)   896069 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/nltk_data/corpora/cmudict.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:41:10.364895 g2p-mix-0.4.2/g2p_mix/nltk_data/taggers/
--rw-r--r--   0 runner    (1001) docker     (127)  2526731 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    11066 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix/tone_sandhi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:41:10.360895 g2p-mix-0.4.2/g2p_mix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/g2p_mix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 10:41:10.368895 g2p-mix-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-11 10:41:10.000000 g2p-mix-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:07:00.516299 g2p-mix-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-17 06:06:59.000000 g2p-mix-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-17 06:06:59.000000 g2p-mix-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-17 06:07:00.516299 g2p-mix-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-17 06:06:59.000000 g2p-mix-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 06:06:59.000000 g2p-mix-0.4.5/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:07:00.512299 g2p-mix-0.4.5/g2p_mix/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-17 06:06:59.000000 g2p-mix-0.4.5/g2p_mix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-17 06:06:59.000000 g2p-mix-0.4.5/g2p_mix/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-17 06:06:59.000000 g2p-mix-0.4.5/g2p_mix/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-17 06:06:59.000000 g2p-mix-0.4.5/g2p_mix/g2p_eng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-17 06:06:59.000000 g2p-mix-0.4.5/g2p_mix/g2p_jyut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-17 06:06:59.000000 g2p-mix-0.4.5/g2p_mix/g2p_mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-17 06:06:59.000000 g2p-mix-0.4.5/g2p_mix/g2p_pth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:07:00.508299 g2p-mix-0.4.5/g2p_mix/nltk_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:07:00.512299 g2p-mix-0.4.5/g2p_mix/nltk_data/corpora/
+-rw-r--r--   0 runner    (1001) docker     (127)   896069 2024-05-17 06:06:59.000000 g2p-mix-0.4.5/g2p_mix/nltk_data/corpora/cmudict.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:07:00.512299 g2p-mix-0.4.5/g2p_mix/nltk_data/taggers/
+-rw-r--r--   0 runner    (1001) docker     (127)  2526731 2024-05-17 06:06:59.000000 g2p-mix-0.4.5/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-17 06:06:59.000000 g2p-mix-0.4.5/g2p_mix/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-05-17 06:06:59.000000 g2p-mix-0.4.5/g2p_mix/tone_sandhi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:07:00.512299 g2p-mix-0.4.5/g2p_mix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-17 06:07:00.000000 g2p-mix-0.4.5/g2p_mix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-17 06:07:00.000000 g2p-mix-0.4.5/g2p_mix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:07:00.000000 g2p-mix-0.4.5/g2p_mix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-17 06:07:00.000000 g2p-mix-0.4.5/g2p_mix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-17 06:07:00.000000 g2p-mix-0.4.5/g2p_mix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 06:07:00.000000 g2p-mix-0.4.5/g2p_mix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-17 06:06:59.000000 g2p-mix-0.4.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 06:07:00.516299 g2p-mix-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-17 06:06:59.000000 g2p-mix-0.4.5/setup.py
```

### Comparing `g2p-mix-0.4.2/LICENSE` & `g2p-mix-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.2/PKG-INFO` & `g2p-mix-0.4.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p-mix
-Version: 0.4.2
+Version: 0.4.5
 Summary: G2P mix
 Home-page: https://github.com/pengzhendong/g2p-mix
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -52,20 +52,22 @@
 ### Cantonese
 
 ```python
 >>> G2pMix(jyut=True).g2p("你这个idea, 不太make sense。")
 ```
 
 ```json
-{"word": "你", "phones": ["n", "ei5"], "lang": "ZH"}
-{"word": "這", "phones": ["z", "e3"], "lang": "ZH"}
-{"word": "個", "phones": ["g", "o3"], "lang": "ZH"}
-{"word": "idea", "phones": ["AY0", "D", "IY1", "AH0"], "lang": "EN"}
-{"word": ",", "phones": ",", "lang": "SYM"}
-{"word": "不", "phones": ["b", "at1"], "lang": "ZH"}
-{"word": "太", "phones": ["t", "aai3"], "lang": "ZH"}
-{"word": "make", "phones": ["M", "EY1", "K"], "lang": "EN"}
-{"word": "sense", "phones": ["S", "EH1", "N", "S"], "lang": "EN"}
-{"word": "。", "phones": "。", "lang": "SYM"}
+[
+  { "word": "你", "phones": ["n", "ei5"], "lang": "ZH" }
+  { "word": "這", "phones": ["z", "e3"], "lang": "ZH" }
+  { "word": "個", "phones": ["g", "o3"], "lang": "ZH" }
+  { "word": "idea", "phones": ["AY0", "D", "IY1", "AH0"], "lang": "EN" }
+  { "word": ",", "phones": ",", "lang": "SYM" }
+  { "word": "不", "phones": ["b", "at1"], "lang": "ZH" }
+  { "word": "太", "phones": ["t", "aai3"], "lang": "ZH" }
+  { "word": "make", "phones": ["M", "EY1", "K"], "lang": "EN" }
+  { "word": "sense", "phones": ["S", "EH1", "N", "S"], "lang": "EN" }
+  { "word": "。", "phones": "。", "lang": "SYM" }
+]
 ```
```

### Comparing `g2p-mix-0.4.2/g2p_mix/__init__.py` & `g2p-mix-0.4.5/g2p_mix/__init__.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.2/g2p_mix/cli.py` & `g2p-mix-0.4.5/g2p_mix/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 import click
 
 from g2p_mix import G2pMix
 
 
 @click.command()
 @click.argument("text")
+@click.option("--jyut/--no-jyut", default=False)
 @click.option("--sandhi/--no-sandhi", default=True)
-def main(text, sandhi):
-    g2per = G2pMix()
-    res = g2per.g2p(text, sandhi=sandhi)
+@click.option("--return-seg/--no-return-seg", default=False)
+def main(text, jyut, sandhi, return_seg):
+    g2per = G2pMix(jyut)
+    res = g2per.g2p(text, sandhi, return_seg)
     print(res)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `g2p-mix-0.4.2/g2p_mix/g2p_eng.py` & `g2p-mix-0.4.5/g2p_mix/g2p_eng.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         # 大写单词长度小于等于 3，按字母念
         if word.isupper() and len(word) <= 3:
             # e.g. "IT" => "I T"
             return self.g2p_abbr(word)
         # 单词在 CMU dict 中，按照 CMU dict 念
         if word.lower() in self.cmudict:
             return self.cmudict[word.lower()][0]
-        # 小写 oov 长度小于等于 3，大小 oov 长度小于等于 4，按字母念
+        # 小写 oov 长度小于等于 3，大写 oov 长度小于等于 4，按字母念
         # e.g. tts => t t s, WFST => W F S T
         if (word.islower() and len(word) <= 3) or (word.isupper() and len(word) <= 4):
             return self.g2p_abbr(word)
         # 其他 OOV 先转小写，用 wordsegment 分词
         # e.g. wifi => wifi, autojs => auto js
         bpes = wordsegment.segment(word.lower())
         # 无法分词则让 g2p_en 预测
```

### Comparing `g2p-mix-0.4.2/g2p_mix/g2p_jyut.py` & `g2p-mix-0.4.5/g2p_mix/g2p_jyut.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.2/g2p_mix/g2p_mix.py` & `g2p-mix-0.4.5/g2p_mix/g2p_mix.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.2/g2p_mix/g2p_pth.py` & `g2p-mix-0.4.5/g2p_mix/g2p_pth.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 from functools import partial
 
 from jieba import posseg
-from pypinyin import Style
+from pypinyin import Style, load_phrases_dict, load_single_dict
 from pypinyin.contrib.tone_convert import to_initials, to_finals
 from pypinyin.converter import UltimateConverter
 
 from .constants import POSTNASALS
 from .tone_sandhi import ToneSandhi
 
 
@@ -52,25 +52,25 @@
         )
         self.strict = strict
         self.sandhi = ToneSandhi().modified_tone
         # load dict to fix some badcase of pypinyin
         self.load_dict()
 
     def load_dict(self):
-        # 为、曾、更、长
         # from pypinyin.constants import PINYIN_DICT
         # print(hex(ord("为")), PINYIN_DICT[ord("为")])
-        from pypinyin import load_single_dict
-
-        load_single_dict({ord("长"): "cha2ng,zha4ng"}, "tone2")
-        load_single_dict({ord("为"): "we4i,we2i"}, "tone2")
-        # from pypinyin import load_phrases_dict
-        # load_phrases_dict({"长时间": [["cha2ng"], ["shi2"], ["jia1n"]]}, "tone2")
-        # from pypinyin_dict.pinyin_data import zdic
-        # zdic.load()  # 汉典
+        dirname = os.path.dirname(__file__)
+        for line in open(f"{dirname}/dict/single.txt", encoding="utf-8"):
+            char, pinyins = line.strip().split(maxsplit=1)
+            load_single_dict({ord(char): pinyins})
+        for line in open(f"{dirname}/dict/phrases.txt", encoding="utf-8"):
+            word, pinyins = line.strip().split(maxsplit=1)
+            pinyins = pinyins.split()
+            assert len(word) == len(pinyins)
+            load_phrases_dict({word: [[pinyin] for pinyin in pinyins]})
 
     def parse(self, pinyin):
         if pinyin[:-1] in POSTNASALS:
             initial = ""
             final = POSTNASALS[pinyin[:-1]]
         else:
             initial = to_initials(pinyin, strict=self.strict)
```

### Comparing `g2p-mix-0.4.2/g2p_mix/nltk_data/corpora/cmudict.zip` & `g2p-mix-0.4.5/g2p_mix/nltk_data/corpora/cmudict.zip`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.2/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip` & `g2p-mix-0.4.5/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.2/g2p_mix/token.py` & `g2p-mix-0.4.5/g2p_mix/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 
-from .g2p_eng import G2pEn
 from pypinyin.constants import RE_HANS
 
+from .g2p_eng import G2pEn
+
 
 g2p_en = G2pEn()
 
 
 class Token:
     def __init__(self, word, pos=None, phones=None):
         self.word = word
```

### Comparing `g2p-mix-0.4.2/g2p_mix/tone_sandhi.py` & `g2p-mix-0.4.5/g2p_mix/tone_sandhi.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import jieba
 
-from .token import Token
-
 
 class ToneSandhi:
     def __init__(self):
         self.digits = list("零一二三四五六七八九十")
         self.neural_tone_words = (
             "麻烦 麻利 鸳鸯 高粱 骨头 骆驼 马虎 首饰 馒头 馄饨 风筝 难为 队伍 阔气 闺女 门道 锄头 铺盖 铃铛 铁匠 钥匙 里脊 里头 部分 "
             "那么 道士 造化 迷糊 连累 这么 这个 运气 过去 软和 转悠 踏实 跳蚤 跟头 趔趄 财主 豆腐 讲究 记性 记号 认识 规矩 见识 裁缝 "
```

### Comparing `g2p-mix-0.4.2/g2p_mix.egg-info/PKG-INFO` & `g2p-mix-0.4.5/g2p_mix.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p-mix
-Version: 0.4.2
+Version: 0.4.5
 Summary: G2P mix
 Home-page: https://github.com/pengzhendong/g2p-mix
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -52,20 +52,22 @@
 ### Cantonese
 
 ```python
 >>> G2pMix(jyut=True).g2p("你这个idea, 不太make sense。")
 ```
 
 ```json
-{"word": "你", "phones": ["n", "ei5"], "lang": "ZH"}
-{"word": "這", "phones": ["z", "e3"], "lang": "ZH"}
-{"word": "個", "phones": ["g", "o3"], "lang": "ZH"}
-{"word": "idea", "phones": ["AY0", "D", "IY1", "AH0"], "lang": "EN"}
-{"word": ",", "phones": ",", "lang": "SYM"}
-{"word": "不", "phones": ["b", "at1"], "lang": "ZH"}
-{"word": "太", "phones": ["t", "aai3"], "lang": "ZH"}
-{"word": "make", "phones": ["M", "EY1", "K"], "lang": "EN"}
-{"word": "sense", "phones": ["S", "EH1", "N", "S"], "lang": "EN"}
-{"word": "。", "phones": "。", "lang": "SYM"}
+[
+  { "word": "你", "phones": ["n", "ei5"], "lang": "ZH" }
+  { "word": "這", "phones": ["z", "e3"], "lang": "ZH" }
+  { "word": "個", "phones": ["g", "o3"], "lang": "ZH" }
+  { "word": "idea", "phones": ["AY0", "D", "IY1", "AH0"], "lang": "EN" }
+  { "word": ",", "phones": ",", "lang": "SYM" }
+  { "word": "不", "phones": ["b", "at1"], "lang": "ZH" }
+  { "word": "太", "phones": ["t", "aai3"], "lang": "ZH" }
+  { "word": "make", "phones": ["M", "EY1", "K"], "lang": "EN" }
+  { "word": "sense", "phones": ["S", "EH1", "N", "S"], "lang": "EN" }
+  { "word": "。", "phones": "。", "lang": "SYM" }
+]
 ```
```

### Comparing `g2p-mix-0.4.2/g2p_mix.egg-info/SOURCES.txt` & `g2p-mix-0.4.5/g2p_mix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.2/setup.py` & `g2p-mix-0.4.5/setup.py`

 * *Files identical despite different names*

