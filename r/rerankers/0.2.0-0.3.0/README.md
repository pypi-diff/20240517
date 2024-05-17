# Comparing `tmp/rerankers-0.2.0.tar.gz` & `tmp/rerankers-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rerankers-0.2.0.tar", last modified: Fri Apr 12 15:35:50 2024, max compression
+gzip compressed data, was "rerankers-0.3.0.tar", last modified: Fri May 17 14:14:52 2024, max compression
```

## Comparing `rerankers-0.2.0.tar` & `rerankers-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-12 15:35:50.095461 rerankers-0.2.0/
--rw-r--r--   0 bclavie    (501) staff       (20)    11309 2024-03-14 14:24:04.000000 rerankers-0.2.0/LICENSE
--rw-r--r--   0 bclavie    (501) staff       (20)    21497 2024-04-12 15:35:50.095249 rerankers-0.2.0/PKG-INFO
--rw-r--r--   0 bclavie    (501) staff       (20)     6732 2024-03-20 13:21:15.000000 rerankers-0.2.0/README.md
--rw-r--r--   0 bclavie    (501) staff       (20)     1591 2024-04-12 15:35:29.000000 rerankers-0.2.0/pyproject.toml
-drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-12 15:35:50.090579 rerankers-0.2.0/rerankers/
--rw-r--r--   0 bclavie    (501) staff       (20)       86 2024-04-12 15:35:36.000000 rerankers-0.2.0/rerankers/__init__.py
-drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-12 15:35:50.091372 rerankers-0.2.0/rerankers/integrations/
--rw-r--r--   0 bclavie    (501) staff       (20)        0 2024-03-14 14:24:04.000000 rerankers-0.2.0/rerankers/integrations/__init__.py
--rw-r--r--   0 bclavie    (501) staff       (20)     1153 2024-03-19 21:00:12.000000 rerankers-0.2.0/rerankers/integrations/langchain.py
-drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-12 15:35:50.093300 rerankers-0.2.0/rerankers/models/
--rw-r--r--   0 bclavie    (501) staff       (20)      927 2024-04-12 15:23:15.000000 rerankers-0.2.0/rerankers/models/__init__.py
--rw-r--r--   0 bclavie    (501) staff       (20)     3537 2024-04-12 15:23:15.000000 rerankers-0.2.0/rerankers/models/api_rankers.py
--rw-r--r--   0 bclavie    (501) staff       (20)     8695 2024-03-14 14:24:04.000000 rerankers-0.2.0/rerankers/models/colbert_ranker.py
--rw-r--r--   0 bclavie    (501) staff       (20)     2052 2024-04-12 15:23:15.000000 rerankers-0.2.0/rerankers/models/flashrank_ranker.py
--rw-r--r--   0 bclavie    (501) staff       (20)     1466 2024-04-12 15:35:13.000000 rerankers-0.2.0/rerankers/models/ranker.py
--rw-r--r--   0 bclavie    (501) staff       (20)     5654 2024-03-14 14:24:04.000000 rerankers-0.2.0/rerankers/models/rankgpt_rankers.py
--rw-r--r--   0 bclavie    (501) staff       (20)       28 2024-03-14 14:24:04.000000 rerankers-0.2.0/rerankers/models/rankllm.py
--rw-r--r--   0 bclavie    (501) staff       (20)    10177 2024-03-14 14:24:04.000000 rerankers-0.2.0/rerankers/models/t5ranker.py
--rw-r--r--   0 bclavie    (501) staff       (20)     3185 2024-04-12 14:38:14.000000 rerankers-0.2.0/rerankers/models/transformer_ranker.py
--rw-r--r--   0 bclavie    (501) staff       (20)     6921 2024-04-12 15:23:15.000000 rerankers-0.2.0/rerankers/reranker.py
--rw-r--r--   0 bclavie    (501) staff       (20)     1478 2024-03-14 14:24:04.000000 rerankers-0.2.0/rerankers/results.py
--rw-r--r--   0 bclavie    (501) staff       (20)     2394 2024-03-14 14:24:04.000000 rerankers-0.2.0/rerankers/utils.py
-drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-12 15:35:50.094049 rerankers-0.2.0/rerankers.egg-info/
--rw-r--r--   0 bclavie    (501) staff       (20)    21497 2024-04-12 15:35:50.000000 rerankers-0.2.0/rerankers.egg-info/PKG-INFO
--rw-r--r--   0 bclavie    (501) staff       (20)      688 2024-04-12 15:35:50.000000 rerankers-0.2.0/rerankers.egg-info/SOURCES.txt
--rw-r--r--   0 bclavie    (501) staff       (20)        1 2024-04-12 15:35:50.000000 rerankers-0.2.0/rerankers.egg-info/dependency_links.txt
--rw-r--r--   0 bclavie    (501) staff       (20)      270 2024-04-12 15:35:50.000000 rerankers-0.2.0/rerankers.egg-info/requires.txt
--rw-r--r--   0 bclavie    (501) staff       (20)       10 2024-04-12 15:35:50.000000 rerankers-0.2.0/rerankers.egg-info/top_level.txt
--rw-r--r--   0 bclavie    (501) staff       (20)       38 2024-04-12 15:35:50.095663 rerankers-0.2.0/setup.cfg
-drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-04-12 15:35:50.093880 rerankers-0.2.0/tests/
--rw-r--r--   0 bclavie    (501) staff       (20)     1225 2024-03-14 14:24:04.000000 rerankers-0.2.0/tests/test_crossenc.py
--rw-r--r--   0 bclavie    (501) staff       (20)      943 2024-03-14 14:24:04.000000 rerankers-0.2.0/tests/test_results.py
+drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-05-17 14:14:52.245684 rerankers-0.3.0/
+-rw-r--r--   0 bclavie    (501) staff       (20)    11309 2024-03-14 14:24:04.000000 rerankers-0.3.0/LICENSE
+-rw-r--r--   0 bclavie    (501) staff       (20)    25865 2024-05-17 14:14:52.245260 rerankers-0.3.0/PKG-INFO
+-rw-r--r--   0 bclavie    (501) staff       (20)    10960 2024-05-17 14:12:41.000000 rerankers-0.3.0/README.md
+-rw-r--r--   0 bclavie    (501) staff       (20)     1690 2024-05-17 14:13:08.000000 rerankers-0.3.0/pyproject.toml
+drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-05-17 14:14:52.239490 rerankers-0.3.0/rerankers/
+-rw-r--r--   0 bclavie    (501) staff       (20)      139 2024-05-17 14:11:48.000000 rerankers-0.3.0/rerankers/__init__.py
+-rw-r--r--   0 bclavie    (501) staff       (20)      410 2024-05-16 14:42:29.000000 rerankers-0.3.0/rerankers/documents.py
+drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-05-17 14:14:52.240474 rerankers-0.3.0/rerankers/integrations/
+-rw-r--r--   0 bclavie    (501) staff       (20)        0 2024-03-14 14:24:04.000000 rerankers-0.3.0/rerankers/integrations/__init__.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     1153 2024-05-16 14:38:52.000000 rerankers-0.3.0/rerankers/integrations/langchain.py
+drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-05-17 14:14:52.242771 rerankers-0.3.0/rerankers/models/
+-rw-r--r--   0 bclavie    (501) staff       (20)     1080 2024-05-17 14:11:48.000000 rerankers-0.3.0/rerankers/models/__init__.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     3592 2024-05-16 14:42:29.000000 rerankers-0.3.0/rerankers/models/api_rankers.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     8725 2024-05-16 14:42:29.000000 rerankers-0.3.0/rerankers/models/colbert_ranker.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     2093 2024-05-17 14:11:48.000000 rerankers-0.3.0/rerankers/models/flashrank_ranker.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     1552 2024-05-16 14:42:29.000000 rerankers-0.3.0/rerankers/models/ranker.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     5810 2024-05-17 14:11:48.000000 rerankers-0.3.0/rerankers/models/rankgpt_rankers.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     2498 2024-05-17 14:11:48.000000 rerankers-0.3.0/rerankers/models/rankllm_ranker.py
+-rw-r--r--   0 bclavie    (501) staff       (20)    10228 2024-05-16 14:42:29.000000 rerankers-0.3.0/rerankers/models/t5ranker.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     3361 2024-05-16 14:42:29.000000 rerankers-0.3.0/rerankers/models/transformer_ranker.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     7601 2024-05-17 14:11:48.000000 rerankers-0.3.0/rerankers/reranker.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     2040 2024-05-17 08:33:50.000000 rerankers-0.3.0/rerankers/results.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     4015 2024-05-16 14:42:29.000000 rerankers-0.3.0/rerankers/utils.py
+drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-05-17 14:14:52.243860 rerankers-0.3.0/rerankers.egg-info/
+-rw-r--r--   0 bclavie    (501) staff       (20)    25865 2024-05-17 14:14:52.000000 rerankers-0.3.0/rerankers.egg-info/PKG-INFO
+-rw-r--r--   0 bclavie    (501) staff       (20)      718 2024-05-17 14:14:52.000000 rerankers-0.3.0/rerankers.egg-info/SOURCES.txt
+-rw-r--r--   0 bclavie    (501) staff       (20)        1 2024-05-17 14:14:52.000000 rerankers-0.3.0/rerankers.egg-info/dependency_links.txt
+-rw-r--r--   0 bclavie    (501) staff       (20)      331 2024-05-17 14:14:52.000000 rerankers-0.3.0/rerankers.egg-info/requires.txt
+-rw-r--r--   0 bclavie    (501) staff       (20)       10 2024-05-17 14:14:52.000000 rerankers-0.3.0/rerankers.egg-info/top_level.txt
+-rw-r--r--   0 bclavie    (501) staff       (20)       38 2024-05-17 14:14:52.245735 rerankers-0.3.0/setup.cfg
+drwxr-xr-x   0 bclavie    (501) staff       (20)        0 2024-05-17 14:14:52.243278 rerankers-0.3.0/tests/
+-rw-r--r--   0 bclavie    (501) staff       (20)     1263 2024-05-16 14:42:29.000000 rerankers-0.3.0/tests/test_crossenc.py
+-rw-r--r--   0 bclavie    (501) staff       (20)     1029 2024-05-16 14:42:29.000000 rerankers-0.3.0/tests/test_results.py
```

### Comparing `rerankers-0.2.0/LICENSE` & `rerankers-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rerankers-0.2.0/PKG-INFO` & `rerankers-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rerankers
-Version: 0.2.0
+Version: 0.3.0
 Summary: A unified API for various document re-ranking models.
 Author-email: Ben Clavié <bc@answer.ai>
 Maintainer-email: Ben Clavié <bc@answer.ai>
 License:  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -201,15 +201,15 @@
                http://www.apache.org/licenses/LICENSE-2.0
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
-Project-URL: Homepage, https://github.com/bclavie/rerankers
+Project-URL: Homepage, https://github.com/answerdotai/rerankers
 Keywords: reranking,retrieval,rag,nlp
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -223,25 +223,28 @@
 Requires-Dist: transformers; extra == "all"
 Requires-Dist: torch; extra == "all"
 Requires-Dist: litellm; extra == "all"
 Requires-Dist: requests; extra == "all"
 Requires-Dist: sentencepiece; extra == "all"
 Requires-Dist: protobuf; extra == "all"
 Requires-Dist: flashrank; extra == "all"
+Requires-Dist: rank-llm; python_version >= "3.10" and extra == "all"
 Provides-Extra: transformers
 Requires-Dist: transformers; extra == "transformers"
 Requires-Dist: torch; extra == "transformers"
 Requires-Dist: sentencepiece; extra == "transformers"
 Requires-Dist: protobuf; extra == "transformers"
 Provides-Extra: api
 Requires-Dist: requests; extra == "api"
 Provides-Extra: gpt
 Requires-Dist: litellm; extra == "gpt"
 Provides-Extra: flashrank
 Requires-Dist: flashrank; extra == "flashrank"
+Provides-Extra: rankllm
+Requires-Dist: rank-llm; extra == "rankllm"
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ipyprogress; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: ranx; extra == "dev"
@@ -260,15 +263,17 @@
 
 ---
 
 Welcome to `rerankers`! Our goal is to provide users with a simple API to use any reranking models.
 
 ## Updates
 
-- v0.1.2: 🆕 Voyage reranking API
+- v0.3.0: 🆕 Many changes! Experimental support for RankLLM, directly backed by the [rank-llm library](https://github.com/castorini/rank_llm). A new `Document` object, courtesy of joint-work by [@bclavie](https://github.com/bclavie) and [Anmol6](https://github.com/Anmol6). This object is transparent, but now offers support for `metadata` stored alongside each document. Many small QoL changes (RankedResults can be itered on directly...)
+- v0.2.0: [FlashRank](https://github.com/PrithivirajDamodaran/FlashRank) rerankers, Basic async support thanks to [@tarunamasa](https://github.com/tarunamasa), MixedBread.ai reranking API
+- v0.1.2: Voyage reranking API
 - v0.1.1: Langchain integration fixed!
 - v0.1.0: Initial release
 
 ## Why `rerankers`?
 
 Rerankers are an important part of any retrieval architecture, but they're also often more obscure than other parts of the pipeline.
 
@@ -301,29 +306,42 @@
 
 # RankGPT
 pip install "rerankers[gpt]"
 
 # API-based rerankers (Cohere, Jina, soon MixedBread)
 pip install "rerankers[api]"
 
+# FlashRank rerankers (ONNX-optimised, very fast on CPU)
+pip install "rerankers[fastrank]"
+
+# RankLLM rerankers (better RankGPT + support for local models such as RankZephyr and RankVicuna)
+# Note: RankLLM is only supported on Python 3.10+! This will not work with Python 3.9
+pip install "rerankers[rankllm]"
+
 # All of the above
 pip install "rerankers[all]"
 ```
 
 ## Usage
 
 Load any supported reranker in a single line, regardless of the architecture:
 ```python
 from rerankers import Reranker
 
 # Cross-encoder default. You can specify a 'lang' parameter to load a multilingual version!
 ranker = Reranker('cross-encoder')
 
 # Specific cross-encoder
-ranker = Reranker('mixedbread-ai/mxbai-rerank-xlarge-v1', model_type='cross-encoder')
+ranker = Reranker('mixedbread-ai/mxbai-rerank-large-v1', model_type='cross-encoder')
+
+# FlashRank default. You can specify a 'lang' parameter to load a multilingual version!
+ranker = Reranker('flashrank')
+
+# Specific flashrank model.
+ranker = Reranker('ce-esci-MiniLM-L12-v2', model_type='flashrank')
 
 # Default T5 Seq2Seq reranker
 ranker = Reranker("t5")
 
 # Specific T5 Seq2Seq reranker
 ranker = Reranker("unicamp-dl/InRanker-base", model_type = "t5")
 
@@ -341,39 +359,88 @@
 
 # RankGPT3-turbo
 ranker = Reranker("rankgpt3", api_key = API_KEY)
 
 # RankGPT with another LLM provider
 ranker = Reranker("MY_LLM_NAME" (check litellm docs), model_type = "rankgpt", api_key = API_KEY)
 
+# RankLLM with default GPT (GPT-4o)
+ranker = Reranker("rankllm", api_key = API_KEY)
+
+# RankLLM with specified GPT models
+ranker = Reranker('gpt-4-turbo', model_type="rankllm", api_key = API_KEY)
+
+# EXPERIMENTAL: RankLLM with RankZephyr
+ranker = Reranker('rankzephyr')
+
 # ColBERTv2 reranker
 ranker = Reranker("colbert")
 
 # ... Or a non-default colbert model:
 ranker = Reranker(model_name_or_path, model_type = "colbert")
 
+# Flashrank
+ranker = Reranker('flashrank')
+
+# ... Or a specific model
+ranker = Reranker('ms-marco-TinyBERT-L-2-v2', model_type='flashrank')
+
 ```
 
 _Rerankers will always try to infer the model you're trying to use based on its name, but it's always safer to pass a `model_type` argument to it if you can!_
 
 Then, regardless of which reranker is loaded, use the loaded model to rank a query against documents:
 
 ```python
 > results = ranker.rank(query="I love you", docs=["I hate you", "I really like you"], doc_ids=[0,1])
 > results
-RankedResults(results=[Result(doc_id=1, text='I really like you', score=0.26170814, rank=1), Result(doc_id=0, text='I hate you', score=0.079210326, rank=2)], query='I love you', has_scores=True)
+RankedResults(results=[Result(document=Document(text='I really like you', doc_id=0), score=-2.453125, rank=1), Result(document=Document(text='I hate you', doc_id=1), score=-4.14453125, rank=2)], query='I love you', has_scores=True)
 ```
 
 You don't need to pass `doc_ids`! If not provided, they'll be auto-generated as integers corresponding to the index of a document in `docs`.
 
+
+You're free to pass metadata too, and it'll be stored with the documents. It'll also be accessible in the results object:
+
+```python
+> results = ranker.rank(query="I love you", docs=["I hate you", "I really like you"], doc_ids=[0,1], metadata=[{'source': 'twitter'}, {'source': 'reddit'}])
+> results
+RankedResults(results=[Result(document=Document(text='I really like you', doc_id=0, metadata={'source': 'twitter'}), score=-2.453125, rank=1), Result(document=Document(text='I hate you', doc_id=1, metadata={'source': 'reddit'}), score=-4.14453125, rank=2)], query='I love you', has_scores=True)
+```
+
+If you'd like your code to be a bit cleaner, you can also directly construct `Document` objects yourself, and pass those instead. In that case, you don't need to pass separate `doc_ids` and `metadata`:
+
+```python
+> from rerankers import Document
+> docs = [Document(text="I really like you", doc_id=0, metadata={'source': 'twitter'}), Document(text="I hate you", doc_id=1, metadata={'source': 'reddit'})]
+> results = ranker.rank(query="I love you", docs=docs)
+> results
+RankedResults(results=[Result(document=Document(text='I really like you', doc_id=0, metadata={'source': 'twitter'}), score=-2.453125, rank=1), Result(document=Document(text='I hate you', doc_id=1, metadata={'source': 'reddit'}), score=-4.14453125, rank=2)], query='I love you', has_scores=True)
+```
+
+You can also use `rank_async`, which is essentially just a wrapper to turn `rank()` into a coroutine. The result will be the same:
+
+```python
+> results = await ranker.rank_async(query="I love you", docs=["I hate you", "I really like you"], doc_ids=[0,1])
+> results
+RankedResults(results=[Result(document=Document(text='I really like you', doc_id=0, metadata={'source': 'twitter'}), score=-2.453125, rank=1), Result(document=Document(text='I hate you', doc_id=1, metadata={'source': 'reddit'}), score=-4.14453125, rank=2)], query='I love you', has_scores=True)
+```
+
 All rerankers will return a `RankedResults` object, which is a pydantic object containing a list of `Result` objects and some other useful information, such as the original query. You can retrieve the top `k` results from it by running `top_k()`:
 
 ```python
 > results.top_k(1)
-[Result(doc_id=1, text='I really like you', score=0.26170814, rank=1)]
+[Result(Document(doc_id=1, text='I really like you', metadata={}), score=0.26170814, rank=1)]
+```
+
+The Result objects are transparent when trying to access the documents they store, as `Document` objects simply exist as an easy way to store IDs and metadata. If you want to access a given result's text or metadata, you can directly access it as a property:
+
+```python
+> results.top_k(1)[0].text
+'I really like you'
 ```
 
 And that's all you need to know to get started quickly! Check out the overview notebook for more information on the API and the different models, or the langchain example to see how to integrate this in your langchain pipeline.
 
 
 ## Features
 
@@ -382,22 +449,22 @@
 - 🟠 Implemented, but not fully fledged
 - 📍 Not supported but intended to be in the future
 - ⭐ Same as above, but **important**.
 - ❌ Not supported & not currently planned
 
 Models:
 - ✅ Any standard SentenceTransformer or Transformers cross-encoder
-- 🟠 RankGPT (Implemented using original repo, but missing the rankllm's repo improvements)
+- ✅ RankGPT (Available both via the original RankGPT implementation and the improved RankLLM one)
 - ✅ T5-based pointwise rankers (InRanker, MonoT5...)
-- ✅ Cohere API rerankers
-- ✅ Jina API rerankers
+- ✅ Cohere, Jina, Voyage and MixedBread API rerankers
+- ✅ [FlashRank](https://github.com/PrithivirajDamodaran/FlashRank) rerankers (ONNX-optimised models, very fast on CPU)
 - 🟠 ColBERT-based reranker - not a model initially designed for reranking, but quite strong (Implementation could be optimised and is from a third-party implementation.)
-- 📍 MixedBread API (Reranking API not yet released)
-- 📍⭐ RankLLM/RankZephyr (Proper RankLLM implementation will replace the RankGPT one, and introduce RankZephyr support)
+- 🟠⭐ RankLLM/RankZephyr: supported by wrapping the [rank-llm library](https://github.com/castorini/rank_llm) library! Support for RankZephyr/RankVicuna is untested, but RankLLM + GPT models fully works!
 - 📍 LiT5
 
 Features:
+- ✅ Metadata!
 - ✅ Reranking 
 - ✅ Consistency notebooks to ensure performance on `scifact` matches the litterature for any given model implementation (Except RankGPT, where results are harder to reproduce).
+- ✅ ONNX runtime support --> Offered through [FlashRank](https://github.com/PrithivirajDamodaran/FlashRank) -- in line with the philosophy of the lib, we won't reinvent the wheel when @PrithivirajDamodaran is doing amazing work!
 - 📍 Training on Python >=3.10 (via interfacing with other libraries)
-- 📍 ONNX runtime support --> Unlikely to be immediate
 - ❌(📍Maybe?) Training via rerankers directly
```

### Comparing `rerankers-0.2.0/pyproject.toml` & `rerankers-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "rerankers.integrations",
 ]
 
 [project]
 name = "rerankers" 
 
 
-version = "0.2.0"
+version = "0.3.0"
 
 description = "A unified API for various document re-ranking models."
 
 readme = "README.md"
 
 requires-python = ">=3.8"
 
@@ -48,16 +48,26 @@
 
 dependencies = [
   "pydantic",
   "tqdm",
 ]
 
 [project.optional-dependencies]
-all = ["transformers", "torch", "litellm", "requests", "sentencepiece", "protobuf", "flashrank"]
+all = [
+    "transformers",
+    "torch",
+    "litellm",
+    "requests",
+    "sentencepiece",
+    "protobuf",
+    "flashrank",
+    "rank-llm; python_version >= '3.10'"
+]
 transformers = ["transformers", "torch", "sentencepiece", "protobuf"]
 api = ["requests"]
 gpt = ["litellm"]
 flashrank = ["flashrank"]
+rankllm = ["rank-llm"]
 dev = ["ruff", "isort", "pytest", "ipyprogress", "ipython", "ranx", "ir_datasets", "srsly"]
 
 [project.urls]
-"Homepage" = "https://github.com/bclavie/rerankers"
+"Homepage" = "https://github.com/answerdotai/rerankers"
```

### Comparing `rerankers-0.2.0/rerankers/integrations/langchain.py` & `rerankers-0.3.0/rerankers/integrations/langchain.py`

 * *Files identical despite different names*

### Comparing `rerankers-0.2.0/rerankers/models/__init__.py` & `rerankers-0.3.0/rerankers/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,7 +34,14 @@
 
 try:
     from rerankers.models.flashrank_ranker import FlashRankRanker
 
     AVAILABLE_RANKERS["FlashRankRanker"] = FlashRankRanker
 except ImportError:
     pass
+
+try:
+    from rerankers.models.rankllm_ranker import RankLLMRanker
+
+    AVAILABLE_RANKERS["RankLLMRanker"] = RankLLMRanker
+except ImportError:
+    pass
```

### Comparing `rerankers-0.2.0/rerankers/models/api_rankers.py` & `rerankers-0.3.0/rerankers/models/api_rankers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import Union, List, Optional
 from rerankers.models.ranker import BaseRanker
 from rerankers.results import RankedResults, Result
-from rerankers.utils import ensure_docids, ensure_docs_list
+from rerankers.utils import prep_docs
+from rerankers.documents import Document
+
 
 import requests
 import json
 
 
 URLS = {
     "cohere": "https://api.cohere.ai/v1/rerank",
@@ -25,78 +27,80 @@
         self.headers = {
             "accept": "application/json",
             "content-type": "application/json",
             "Authorization": f"Bearer {self.api_key}",
         }
         self.url = URLS[self.api_provider]
 
+
     def _get_document_text(self, r: dict) -> str:
         if self.api_provider == "voyage":
             return r["document"]
         elif self.api_provider == "mixedbread.ai":
             return r["input"]
         else:
             return r["document"]["text"]
 
     def _get_score(self, r: dict) -> float:
         if self.api_provider == "mixedbread.ai":
             return r["score"]
         return r["relevance_score"]
 
     def _parse_response(
-        self, response: dict, doc_ids: Union[List[str], List[int]]
+        self, response: dict,  docs: List[Document],
     ) -> RankedResults:
         ranked_docs = []
         results_key = (
             "results"
             if self.api_provider not in ["voyage", "mixedbread.ai"]
             else "data"
         )
         print(response)
 
         for i, r in enumerate(response[results_key]):
             ranked_docs.append(
                 Result(
-                    doc_id=doc_ids[r["index"]],
+                    document=docs[r["index"]],
                     text=self._get_document_text(r),
                     score=self._get_score(r),
                     rank=i + 1,
                 )
             )
 
         return ranked_docs
 
     def rank(
         self,
         query: str,
-        docs: Union[str, List[str]],
+        docs: Union[str, List[str], Document, List[Document]],
         doc_ids: Optional[Union[List[str], List[int]]] = None,
+        metadata: Optional[List[dict]] = None,
     ) -> RankedResults:
-        docs = ensure_docs_list(docs)
-        doc_ids = ensure_docids(doc_ids, len(docs))
+        docs = prep_docs(docs, doc_ids, metadata)
         payload = self._format_payload(query, docs)
         response = requests.post(self.url, headers=self.headers, data=payload)
-        results = self._parse_response(response.json(), doc_ids)
+        results = self._parse_response(response.json(), docs)
         return RankedResults(results=results, query=query, has_scores=True)
 
+
     def _format_payload(self, query: str, docs: List[str]) -> str:
         top_key = (
             "top_n" if self.api_provider not in ["voyage", "mixedbread.ai"] else "top_k"
         )
         documents_key = "documents" if self.api_provider != "mixedbread.ai" else "input"
         return_documents_key = (
             "return_documents"
             if self.api_provider != "mixedbread.ai"
             else "return_input"
         )
 
         payload = {
             "model": self.model,
             "query": query,
-            documents_key: docs,
+            documents_key: [d.text for d in docs],
             top_key: len(docs),
             return_documents_key: True,
         }
         return json.dumps(payload)
 
     def score(self, query: str, doc: str) -> float:
         payload = self._format_payload(query, [doc])
```

### Comparing `rerankers-0.2.0/rerankers/models/colbert_ranker.py` & `rerankers-0.3.0/rerankers/models/colbert_ranker.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,17 @@
 
 import torch
 from transformers import AutoModel, AutoTokenizer
 from typing import List, Optional, Union
 from math import ceil
 
 from rerankers.models.ranker import BaseRanker
+from rerankers.documents import Document
 from rerankers.results import RankedResults, Result
-from rerankers.utils import (
-    vprint,
-    get_device,
-    get_dtype,
-    ensure_docids,
-    ensure_docs_list,
-)
+from rerankers.utils import vprint, get_device, get_dtype, prep_docs
 
 
 def _insert_token(
     output: dict,
     insert_token_id: int,
     insert_position: int = 1,
     token_type_id: int = 0,
@@ -118,24 +113,25 @@
             document_token
         )  # type: ignore
         self.normalize = True
 
     def rank(
         self,
         query: str,
-        docs: List[str],
+        docs: Union[Document, str, List[Document], List[str]],
         doc_ids: Optional[Union[List[str], List[int]]] = None,
+        metadata: Optional[List[dict]] = None,
     ) -> RankedResults:
-        docs = ensure_docs_list(docs)
-        doc_ids = ensure_docids(doc_ids, len(docs))
-        scores = self._colbert_rank(query, docs)
+        docs = prep_docs(docs, doc_ids, metadata)
+
+        scores = self._colbert_rank(query, [d.text for d in docs])
         ranked_results = [
-            Result(doc_id=doc_id, text=doc, score=score, rank=idx + 1)
-            for idx, (doc_id, doc, score) in enumerate(
-                sorted(zip(doc_ids, docs, scores), key=lambda x: x[2], reverse=True)
+            Result(document=doc, score=score, rank=idx + 1)
+            for idx, (doc, score) in enumerate(
+                sorted(zip(docs, scores), key=lambda x: x[1], reverse=True)
             )
         ]
         return RankedResults(results=ranked_results, query=query, has_scores=True)
 
     def score(self, query: str, doc: str) -> float:
         scores = self._colbert_rank(query, [doc])
         return scores[0] if scores else 0.0
```

### Comparing `rerankers-0.2.0/rerankers/models/flashrank_ranker.py` & `rerankers-0.3.0/rerankers/models/flashrank_ranker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from rerankers.models.ranker import BaseRanker
 
 from flashrank import Ranker, RerankRequest
 
 
 from typing import Union, List, Optional, Tuple
-from rerankers.utils import (
-    vprint,
-    ensure_docids,
-    ensure_docs_list,
-)
+from rerankers.utils import vprint, prep_docs
 from rerankers.results import RankedResults, Result
+from rerankers.documents import Document
 
 
 class FlashRankRanker(BaseRanker):
     def __init__(
         self,
         model_name_or_path: str,
         verbose: int = 1,
@@ -30,28 +27,29 @@
         return self.tokenizer(
             inputs, return_tensors="pt", padding=True, truncation=True
         ).to(self.device)
 
     def rank(
         self,
         query: str,
-        docs: List[str],
-        doc_ids: Optional[List[Union[str, int]]] = None,
+        docs: Union[str, List[str], Document, List[Document]],
+        doc_ids: Optional[Union[List[str], List[int]]] = None,
+        metadata: Optional[List[dict]] = None,
     ) -> RankedResults:
-        docs = ensure_docs_list(docs)
-        doc_ids = ensure_docids(doc_ids, len(docs))
-        passages = [{"id": doc_id, "text": doc} for doc_id, doc in zip(doc_ids, docs)]
+        docs = prep_docs(docs, doc_ids, metadata)
+        passages = [
+            {"id": doc_idx, "text": doc.text} for doc_idx, doc in enumerate(docs)
+        ]
 
         rerank_request = RerankRequest(query=query, passages=passages)
         flashrank_results = self.model.rerank(rerank_request)
 
         ranked_results = [
             Result(
-                doc_id=result["id"],
-                text=result["text"],
+                document=docs[idx],
                 score=result["score"],
                 rank=idx + 1,
             )
             for idx, result in enumerate(flashrank_results)
         ]
         return RankedResults(results=ranked_results, query=query, has_scores=True)
```

### Comparing `rerankers-0.2.0/rerankers/models/ranker.py` & `rerankers-0.3.0/rerankers/models/ranker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from abc import ABC, abstractmethod
-from typing import List, Optional, Union
-from rerankers.results import RankedResults
 from asyncio import get_event_loop
 from functools import partial
+from typing import List, Optional, Union
+from rerankers.results import RankedResults
+from rerankers.documents import Document
+
 
 class BaseRanker(ABC):
     @abstractmethod
     def __init__(self, model_name_or_path: str, verbose: int):
         pass
 
     @abstractmethod
     def score(self, query: str, doc: str) -> float:
         pass
 
     @abstractmethod
     def rank(
         self,
         query: str,
-        docs: List[str],
-        doc_ids: Optional[Union[List[str], str]] = None,
+        docs: Union[str, List[str], Document, List[Document]],
+        doc_ids: Optional[Union[List[str], List[int]]] = None,
     ) -> RankedResults:
         """
         End-to-end reranking of documents.
         """
         pass
 
     async def rank_async(
```

### Comparing `rerankers-0.2.0/rerankers/models/rankgpt_rankers.py` & `rerankers-0.3.0/rerankers/models/rankgpt_rankers.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 - make_item() added
 - Packaging it onto RankGPTRanker"""
 
 import copy
 from typing import Optional, Union, List, Dict
 from litellm import completion
 from rerankers.models.ranker import BaseRanker
+from rerankers.documents import Document
 from rerankers.results import RankedResults, Result
-from rerankers.utils import vprint, ensure_docids, ensure_docs_list
+from rerankers.utils import vprint, prep_docs
 
 
 def get_prefix_prompt(query, num):
     return [
         {
             "role": "system",
             "content": "You are RankGPT, an intelligent assistant that can rank passages based on their relevancy to the query.",
@@ -121,37 +122,41 @@
             api_key=self.api_key, model=self.model, messages=messages, temperature=0
         )
         return response.choices[0].message.content
 
     def rank(
         self,
         query: str,
-        docs: Union[str, List[str]],
+        docs: Union[str, List[str], Document, List[Document]],
         doc_ids: Optional[Union[List[str], List[int]]] = None,
+        metadata: Optional[List[dict]] = None,
         rank_start: int = 0,
         rank_end: int = 0,
     ) -> RankedResults:
-        docs = ensure_docs_list(docs)
-        doc_ids = ensure_docids(doc_ids, len(docs))
-        item = make_item(query, docs)
+        docs = prep_docs(docs, doc_ids, metadata)
+
+        item = make_item(query, [d.text for d in docs])
         messages = create_permutation_instruction(
             item=item,
             rank_start=rank_start,
             rank_end=rank_end,
             lang=self.lang,
         )
         vprint(f"Querying model {self.model} with via LiteLLM...", self.verbose)
         permutation = self._query_llm(messages)
         item = receive_permutation(
             item, permutation, rank_start=rank_start, rank_end=rank_end
         )
         ranked_docs = []
         for idx, doc in enumerate(item["hits"]):
             ranked_docs.append(
-                Result(doc_id=doc_ids[idx], text=doc["content"], rank=idx + 1)
+                Result(
+                    document=list(filter(lambda x: x.text == doc["content"], docs))[0],
+                    rank=idx + 1,
+                )
             )
         ranked_results = RankedResults(
             results=ranked_docs, query=query, has_scores=False
         )
         return ranked_results
 
     def score(self):
```

### Comparing `rerankers-0.2.0/rerankers/models/t5ranker.py` & `rerankers-0.3.0/rerankers/models/t5ranker.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 from typing import List, Optional, Union
 from math import ceil
 
 import torch
 from tqdm.auto import tqdm
 from transformers import AutoModelForSeq2SeqLM, AutoTokenizer
 from rerankers.models.ranker import BaseRanker
+from rerankers.documents import Document
+
 
 import torch
 
 from rerankers.results import RankedResults, Result
 from rerankers.utils import (
     vprint,
     get_device,
     get_dtype,
-    ensure_docids,
-    ensure_docs_list,
+    prep_docs,
     get_chunks,
 )
 
 PREDICTION_TOKENS = {
     "default": ["▁false", "▁true"],
     "castorini/monot5-base-msmarco": ["▁false", "▁true"],
     "castorini/monot5-base-msmarco-10k": ["▁false", "▁true"],
@@ -129,27 +130,27 @@
             )
         else:
             vprint("Returning normalised scores...", self.verbose)
 
     def rank(
         self,
         query: str,
-        docs: List[str],
+        docs: Union[str, List[str], Document, List[Document]],
         doc_ids: Optional[Union[List[str], List[int]]] = None,
+        metadata: Optional[List[dict]] = None,
     ) -> RankedResults:
         """
         Ranks a list of documents based on their relevance to the query.
         """
-        docs = ensure_docs_list(docs)
-        doc_ids = ensure_docids(doc_ids, len(docs))
-        scores = self._get_scores(query, docs)
+        docs = prep_docs(docs, doc_ids, metadata)
+        scores = self._get_scores(query, [d.text for d in docs])
         ranked_results = [
-            Result(doc_id=doc_id, text=doc, score=score, rank=idx + 1)
-            for idx, (doc_id, doc, score) in enumerate(
-                sorted(zip(doc_ids, docs, scores), key=lambda x: x[2], reverse=True)
+            Result(document=doc, score=score, rank=idx + 1)
+            for idx, (doc, score) in enumerate(
+                sorted(zip(docs, scores), key=lambda x: x[1], reverse=True)
             )
         ]
         return RankedResults(results=ranked_results, query=query, has_scores=True)
 
     def score(self, query: str, doc: str) -> float:
         """
         Scores a single document's relevance to a query.
```

### Comparing `rerankers-0.2.0/rerankers/models/transformer_ranker.py` & `rerankers-0.3.0/rerankers/models/transformer_ranker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from rerankers.models.ranker import BaseRanker
+from rerankers.documents import Document
+
 
 import torch
 from typing import Union, List, Optional, Tuple
 from transformers import (
     AutoModelForSequenceClassification,
     AutoTokenizer,
 )
 from rerankers.utils import (
     vprint,
     get_device,
     get_dtype,
-    ensure_docids,
-    ensure_docs_list,
+    prep_docs,
 )
 from rerankers.results import RankedResults, Result
 
 
 class TransformerRanker(BaseRanker):
     def __init__(
         self,
@@ -44,21 +45,21 @@
             inputs, return_tensors="pt", padding=True, truncation=True
         ).to(self.device)
 
     @torch.no_grad()
     def rank(
         self,
         query: str,
-        docs: List[str],
-        doc_ids: Optional[List[Union[str, int]]] = None,
+        docs: Union[str, List[str], Document, List[Document]],
+        doc_ids: Optional[Union[List[str], List[int]]] = None,
+        metadata: Optional[List[dict]] = None,
         batch_size: Optional[int] = None,
     ) -> RankedResults:
-        docs = ensure_docs_list(docs)
-        doc_ids = ensure_docids(doc_ids, len(docs))
-        inputs = [(query, doc) for doc in docs]
+        docs = prep_docs(docs, doc_ids, metadata)
+        inputs = [(query, doc.text) for doc in docs]
 
         # Override self.batch_size if explicitely set
         if batch_size is None:
             batch_size = self.batch_size
         batched_inputs = [
             inputs[i : i + batch_size] for i in range(0, len(inputs), batch_size)
         ]
@@ -67,21 +68,24 @@
             tokenized_inputs = self.tokenize(batch)
             batch_scores = self.model(**tokenized_inputs).logits.squeeze()
             batch_scores = batch_scores.detach().cpu().numpy().tolist()
             if isinstance(batch_scores, float):  # Handling the case of single score
                 scores.append(batch_scores)
             else:
                 scores.extend(batch_scores)
-        ranked_results = [
-            Result(doc_id=doc_id, text=doc, score=score, rank=idx + 1)
-            for idx, (doc_id, doc, score) in enumerate(
-                sorted(zip(doc_ids, docs, scores), key=lambda x: x[2], reverse=True)
-            )
-        ]
-        return RankedResults(results=ranked_results, query=query, has_scores=True)
+        if len(scores) == 1:
+            return Result(document=docs[0], score=scores[0])
+        else:
+            ranked_results = [
+                Result(document=doc, score=score, rank=idx + 1)
+                for idx, (doc, score) in enumerate(
+                    sorted(zip(docs, scores), key=lambda x: x[1], reverse=True)
+                )
+            ]
+            return RankedResults(results=ranked_results, query=query, has_scores=True)
 
     @torch.no_grad()
     def score(self, query: str, doc: str) -> float:
         inputs = self.tokenize((query, doc))
         outputs = self.model(**inputs)
         score = outputs.logits.squeeze().detach().cpu().numpy().astype(float)
         return score
```

### Comparing `rerankers-0.2.0/rerankers/reranker.py` & `rerankers-0.3.0/rerankers/reranker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Optional
+import warnings
 from rerankers.models import AVAILABLE_RANKERS
 from rerankers.models.ranker import BaseRanker
 from rerankers.utils import vprint
 
 DEFAULTS = {
     "jina": {"en": "jina-reranker-v1-base-en"},
     "cohere": {"en": "rerank-english-v3.0", "other": "rerank-multilingual-v3.0"},
@@ -17,14 +18,15 @@
     "t5": {"en": "unicamp-dl/InRanker-base", "other": "unicamp-dl/mt5-base-mmarco-v2"},
     "lit5": {
         "en": "castorini/LiT5-Distill-base",
     },
     "rankgpt": {"en": "gpt-4-turbo-preview", "other": "gpt-4-turbo-preview"},
     "rankgpt3": {"en": "gpt-3.5-turbo", "other": "gpt-3.5-turbo"},
     "rankgpt4": {"en": "gpt-4", "other": "gpt-4"},
+    "rankllm": {"en": "gpt-4o", "other": "gpt-4o"},
     "colbert": {
         "en": "colbert-ir/colbertv2.0",
         "fr": "bclavie/FraColBERTv2",
         "ja": "bclavie/JaColBERTv2",
         "es": "AdrienB134/ColBERTv2.0-spanish-mmarcoES",
     },
     "flashrank": {"en": "ms-marco-MiniLM-L-12-v2", "other": "ms-marco-MultiBERT-L-12"},
@@ -34,14 +36,15 @@
     "TransformerRanker": "transformers",
     "T5Ranker": "transformers",
     "LiT5Ranker": "lit5",
     "RankGPTRanker": "gpt",
     "APIRanker": "api",
     "ColBERTRanker": "transformers",
     "FlashRankRanker": "flashrank",
+    "RankLLMRanker": "rankllm",
 }
 
 PROVIDERS = ["cohere", "jina", "voyage", "mixedbread.ai"]
 
 
 def _get_api_provider(model_name: str, model_type: Optional[str] = None) -> str:
     if model_type in PROVIDERS or any(provider in model_name for provider in PROVIDERS):
@@ -68,33 +71,43 @@
             "voyage": "APIRanker",
             "rankgpt": "RankGPTRanker",
             "lit5": "LiT5Ranker",
             "t5": "T5Ranker",
             "colbert": "ColBERTRanker",
             "cross-encoder": "TransformerRanker",
             "flashrank": "FlashRankRanker",
+            "rankllm": "RankLLMRanker",
         }
         return model_mapping.get(explicit_model_type, explicit_model_type)
     else:
         model_name = model_name.lower()
         model_mapping = {
             "lit5": "LiT5Ranker",
             "t5": "T5Ranker",
             "inranker": "T5Ranker",
+            "rankllm": "RankLLMRanker",
+            "rankgpt": "RankGPTRanker",
             "gpt": "RankGPTRanker",
             "zephyr": "RankZephyr",
             "colbert": "ColBERTRanker",
             "cohere": "APIRanker",
             "jina": "APIRanker",
             "voyage": "APIRanker",
             "ms-marco-minilm-l-12-v2": "FlashRankRanker",
             "ms-marco-multibert-l-12": "FlashRankRanker",
+            "vicuna": "RankLLMRanker",
+            "zephyr": "RankLLMRanker",
         }
         for key, value in model_mapping.items():
             if key in model_name:
+                if key == "gpt":
+                    warnings.warn(
+                        "The key 'gpt' currently defaults to the rough rankGPT implementation. From version 0.0.5 onwards, 'gpt' will default to RankLLM instead. Please specify the 'rankgpt' `model_type` if you want to keep the current behaviour",
+                        DeprecationWarning,
+                    )
                 return value
         if (
             any(
                 keyword in model_name
                 for keyword in ["minilm", "bert", "cross-encoders/"]
             )
             and "/" in model_name
```

### Comparing `rerankers-0.2.0/rerankers.egg-info/PKG-INFO` & `rerankers-0.3.0/rerankers.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rerankers
-Version: 0.2.0
+Version: 0.3.0
 Summary: A unified API for various document re-ranking models.
 Author-email: Ben Clavié <bc@answer.ai>
 Maintainer-email: Ben Clavié <bc@answer.ai>
 License:  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -201,15 +201,15 @@
                http://www.apache.org/licenses/LICENSE-2.0
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
-Project-URL: Homepage, https://github.com/bclavie/rerankers
+Project-URL: Homepage, https://github.com/answerdotai/rerankers
 Keywords: reranking,retrieval,rag,nlp
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -223,25 +223,28 @@
 Requires-Dist: transformers; extra == "all"
 Requires-Dist: torch; extra == "all"
 Requires-Dist: litellm; extra == "all"
 Requires-Dist: requests; extra == "all"
 Requires-Dist: sentencepiece; extra == "all"
 Requires-Dist: protobuf; extra == "all"
 Requires-Dist: flashrank; extra == "all"
+Requires-Dist: rank-llm; python_version >= "3.10" and extra == "all"
 Provides-Extra: transformers
 Requires-Dist: transformers; extra == "transformers"
 Requires-Dist: torch; extra == "transformers"
 Requires-Dist: sentencepiece; extra == "transformers"
 Requires-Dist: protobuf; extra == "transformers"
 Provides-Extra: api
 Requires-Dist: requests; extra == "api"
 Provides-Extra: gpt
 Requires-Dist: litellm; extra == "gpt"
 Provides-Extra: flashrank
 Requires-Dist: flashrank; extra == "flashrank"
+Provides-Extra: rankllm
+Requires-Dist: rank-llm; extra == "rankllm"
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ipyprogress; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: ranx; extra == "dev"
@@ -260,15 +263,17 @@
 
 ---
 
 Welcome to `rerankers`! Our goal is to provide users with a simple API to use any reranking models.
 
 ## Updates
 
-- v0.1.2: 🆕 Voyage reranking API
+- v0.3.0: 🆕 Many changes! Experimental support for RankLLM, directly backed by the [rank-llm library](https://github.com/castorini/rank_llm). A new `Document` object, courtesy of joint-work by [@bclavie](https://github.com/bclavie) and [Anmol6](https://github.com/Anmol6). This object is transparent, but now offers support for `metadata` stored alongside each document. Many small QoL changes (RankedResults can be itered on directly...)
+- v0.2.0: [FlashRank](https://github.com/PrithivirajDamodaran/FlashRank) rerankers, Basic async support thanks to [@tarunamasa](https://github.com/tarunamasa), MixedBread.ai reranking API
+- v0.1.2: Voyage reranking API
 - v0.1.1: Langchain integration fixed!
 - v0.1.0: Initial release
 
 ## Why `rerankers`?
 
 Rerankers are an important part of any retrieval architecture, but they're also often more obscure than other parts of the pipeline.
 
@@ -301,29 +306,42 @@
 
 # RankGPT
 pip install "rerankers[gpt]"
 
 # API-based rerankers (Cohere, Jina, soon MixedBread)
 pip install "rerankers[api]"
 
+# FlashRank rerankers (ONNX-optimised, very fast on CPU)
+pip install "rerankers[fastrank]"
+
+# RankLLM rerankers (better RankGPT + support for local models such as RankZephyr and RankVicuna)
+# Note: RankLLM is only supported on Python 3.10+! This will not work with Python 3.9
+pip install "rerankers[rankllm]"
+
 # All of the above
 pip install "rerankers[all]"
 ```
 
 ## Usage
 
 Load any supported reranker in a single line, regardless of the architecture:
 ```python
 from rerankers import Reranker
 
 # Cross-encoder default. You can specify a 'lang' parameter to load a multilingual version!
 ranker = Reranker('cross-encoder')
 
 # Specific cross-encoder
-ranker = Reranker('mixedbread-ai/mxbai-rerank-xlarge-v1', model_type='cross-encoder')
+ranker = Reranker('mixedbread-ai/mxbai-rerank-large-v1', model_type='cross-encoder')
+
+# FlashRank default. You can specify a 'lang' parameter to load a multilingual version!
+ranker = Reranker('flashrank')
+
+# Specific flashrank model.
+ranker = Reranker('ce-esci-MiniLM-L12-v2', model_type='flashrank')
 
 # Default T5 Seq2Seq reranker
 ranker = Reranker("t5")
 
 # Specific T5 Seq2Seq reranker
 ranker = Reranker("unicamp-dl/InRanker-base", model_type = "t5")
 
@@ -341,39 +359,88 @@
 
 # RankGPT3-turbo
 ranker = Reranker("rankgpt3", api_key = API_KEY)
 
 # RankGPT with another LLM provider
 ranker = Reranker("MY_LLM_NAME" (check litellm docs), model_type = "rankgpt", api_key = API_KEY)
 
+# RankLLM with default GPT (GPT-4o)
+ranker = Reranker("rankllm", api_key = API_KEY)
+
+# RankLLM with specified GPT models
+ranker = Reranker('gpt-4-turbo', model_type="rankllm", api_key = API_KEY)
+
+# EXPERIMENTAL: RankLLM with RankZephyr
+ranker = Reranker('rankzephyr')
+
 # ColBERTv2 reranker
 ranker = Reranker("colbert")
 
 # ... Or a non-default colbert model:
 ranker = Reranker(model_name_or_path, model_type = "colbert")
 
+# Flashrank
+ranker = Reranker('flashrank')
+
+# ... Or a specific model
+ranker = Reranker('ms-marco-TinyBERT-L-2-v2', model_type='flashrank')
+
 ```
 
 _Rerankers will always try to infer the model you're trying to use based on its name, but it's always safer to pass a `model_type` argument to it if you can!_
 
 Then, regardless of which reranker is loaded, use the loaded model to rank a query against documents:
 
 ```python
 > results = ranker.rank(query="I love you", docs=["I hate you", "I really like you"], doc_ids=[0,1])
 > results
-RankedResults(results=[Result(doc_id=1, text='I really like you', score=0.26170814, rank=1), Result(doc_id=0, text='I hate you', score=0.079210326, rank=2)], query='I love you', has_scores=True)
+RankedResults(results=[Result(document=Document(text='I really like you', doc_id=0), score=-2.453125, rank=1), Result(document=Document(text='I hate you', doc_id=1), score=-4.14453125, rank=2)], query='I love you', has_scores=True)
 ```
 
 You don't need to pass `doc_ids`! If not provided, they'll be auto-generated as integers corresponding to the index of a document in `docs`.
 
+
+You're free to pass metadata too, and it'll be stored with the documents. It'll also be accessible in the results object:
+
+```python
+> results = ranker.rank(query="I love you", docs=["I hate you", "I really like you"], doc_ids=[0,1], metadata=[{'source': 'twitter'}, {'source': 'reddit'}])
+> results
+RankedResults(results=[Result(document=Document(text='I really like you', doc_id=0, metadata={'source': 'twitter'}), score=-2.453125, rank=1), Result(document=Document(text='I hate you', doc_id=1, metadata={'source': 'reddit'}), score=-4.14453125, rank=2)], query='I love you', has_scores=True)
+```
+
+If you'd like your code to be a bit cleaner, you can also directly construct `Document` objects yourself, and pass those instead. In that case, you don't need to pass separate `doc_ids` and `metadata`:
+
+```python
+> from rerankers import Document
+> docs = [Document(text="I really like you", doc_id=0, metadata={'source': 'twitter'}), Document(text="I hate you", doc_id=1, metadata={'source': 'reddit'})]
+> results = ranker.rank(query="I love you", docs=docs)
+> results
+RankedResults(results=[Result(document=Document(text='I really like you', doc_id=0, metadata={'source': 'twitter'}), score=-2.453125, rank=1), Result(document=Document(text='I hate you', doc_id=1, metadata={'source': 'reddit'}), score=-4.14453125, rank=2)], query='I love you', has_scores=True)
+```
+
+You can also use `rank_async`, which is essentially just a wrapper to turn `rank()` into a coroutine. The result will be the same:
+
+```python
+> results = await ranker.rank_async(query="I love you", docs=["I hate you", "I really like you"], doc_ids=[0,1])
+> results
+RankedResults(results=[Result(document=Document(text='I really like you', doc_id=0, metadata={'source': 'twitter'}), score=-2.453125, rank=1), Result(document=Document(text='I hate you', doc_id=1, metadata={'source': 'reddit'}), score=-4.14453125, rank=2)], query='I love you', has_scores=True)
+```
+
 All rerankers will return a `RankedResults` object, which is a pydantic object containing a list of `Result` objects and some other useful information, such as the original query. You can retrieve the top `k` results from it by running `top_k()`:
 
 ```python
 > results.top_k(1)
-[Result(doc_id=1, text='I really like you', score=0.26170814, rank=1)]
+[Result(Document(doc_id=1, text='I really like you', metadata={}), score=0.26170814, rank=1)]
+```
+
+The Result objects are transparent when trying to access the documents they store, as `Document` objects simply exist as an easy way to store IDs and metadata. If you want to access a given result's text or metadata, you can directly access it as a property:
+
+```python
+> results.top_k(1)[0].text
+'I really like you'
 ```
 
 And that's all you need to know to get started quickly! Check out the overview notebook for more information on the API and the different models, or the langchain example to see how to integrate this in your langchain pipeline.
 
 
 ## Features
 
@@ -382,22 +449,22 @@
 - 🟠 Implemented, but not fully fledged
 - 📍 Not supported but intended to be in the future
 - ⭐ Same as above, but **important**.
 - ❌ Not supported & not currently planned
 
 Models:
 - ✅ Any standard SentenceTransformer or Transformers cross-encoder
-- 🟠 RankGPT (Implemented using original repo, but missing the rankllm's repo improvements)
+- ✅ RankGPT (Available both via the original RankGPT implementation and the improved RankLLM one)
 - ✅ T5-based pointwise rankers (InRanker, MonoT5...)
-- ✅ Cohere API rerankers
-- ✅ Jina API rerankers
+- ✅ Cohere, Jina, Voyage and MixedBread API rerankers
+- ✅ [FlashRank](https://github.com/PrithivirajDamodaran/FlashRank) rerankers (ONNX-optimised models, very fast on CPU)
 - 🟠 ColBERT-based reranker - not a model initially designed for reranking, but quite strong (Implementation could be optimised and is from a third-party implementation.)
-- 📍 MixedBread API (Reranking API not yet released)
-- 📍⭐ RankLLM/RankZephyr (Proper RankLLM implementation will replace the RankGPT one, and introduce RankZephyr support)
+- 🟠⭐ RankLLM/RankZephyr: supported by wrapping the [rank-llm library](https://github.com/castorini/rank_llm) library! Support for RankZephyr/RankVicuna is untested, but RankLLM + GPT models fully works!
 - 📍 LiT5
 
 Features:
+- ✅ Metadata!
 - ✅ Reranking 
 - ✅ Consistency notebooks to ensure performance on `scifact` matches the litterature for any given model implementation (Except RankGPT, where results are harder to reproduce).
+- ✅ ONNX runtime support --> Offered through [FlashRank](https://github.com/PrithivirajDamodaran/FlashRank) -- in line with the philosophy of the lib, we won't reinvent the wheel when @PrithivirajDamodaran is doing amazing work!
 - 📍 Training on Python >=3.10 (via interfacing with other libraries)
-- 📍 ONNX runtime support --> Unlikely to be immediate
 - ❌(📍Maybe?) Training via rerankers directly
```

### Comparing `rerankers-0.2.0/rerankers.egg-info/SOURCES.txt` & `rerankers-0.3.0/rerankers.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 rerankers/__init__.py
+rerankers/documents.py
 rerankers/reranker.py
 rerankers/results.py
 rerankers/utils.py
 rerankers.egg-info/PKG-INFO
 rerankers.egg-info/SOURCES.txt
 rerankers.egg-info/dependency_links.txt
 rerankers.egg-info/requires.txt
@@ -14,12 +15,12 @@
 rerankers/integrations/langchain.py
 rerankers/models/__init__.py
 rerankers/models/api_rankers.py
 rerankers/models/colbert_ranker.py
 rerankers/models/flashrank_ranker.py
 rerankers/models/ranker.py
 rerankers/models/rankgpt_rankers.py
-rerankers/models/rankllm.py
+rerankers/models/rankllm_ranker.py
 rerankers/models/t5ranker.py
 rerankers/models/transformer_ranker.py
 tests/test_crossenc.py
 tests/test_results.py
```

### Comparing `rerankers-0.2.0/tests/test_crossenc.py` & `rerankers-0.3.0/tests/test_crossenc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 from unittest.mock import patch
 import torch
 from rerankers import Reranker
 from rerankers.models.transformer_ranker import TransformerRanker
 from rerankers.results import Result, RankedResults
-
+from rerankers.documents import Document
 
 @patch("rerankers.models.transformer_ranker.TransformerRanker.rank")
 def test_transformer_ranker_rank(mock_rank):
     query = "Gone with the wind is an absolute masterpiece"
     docs = [
         "Gone with the wind is a masterclass in bad storytelling.",
         "Gone with the wind is an all-time classic",
     ]
     expected_results = RankedResults(
         results=[
             Result(
-                doc_id=1,
-                text="Gone with the wind is an all-time classic",
+                document=Document(id=1, text="Gone with the wind is an all-time classic"),
                 score=1.6181640625,
                 rank=1,
             ),
             Result(
-                doc_id=0,
-                text="Gone with the wind is a masterclass in bad storytelling.",
+                document=Document(id=0, text="Gone with the wind is a masterclass in bad storytelling."),
                 score=0.88427734375,
                 rank=2,
             ),
         ],
         query=query,
         has_scores=True,
     )
```

### Comparing `rerankers-0.2.0/tests/test_results.py` & `rerankers-0.3.0/tests/test_results.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import pytest
 from rerankers.results import Result, RankedResults
+from rerankers.documents import Document
 
 
 def test_ranked_results_functions():
     results = RankedResults(
         results=[
-            Result(doc_id=0, text="Doc 0", score=0.9, rank=2),
-            Result(doc_id=1, text="Doc 1", score=0.95, rank=1),
+            Result(document=Document(id=0, text="Doc 0"), score=0.9, rank=2),
+            Result(document=Document(id=1, text="Doc 1"), score=0.95, rank=1),
         ],
         query="Test Query",
         has_scores=True,
     )
     assert results.results_count() == 2
     top_k = results.top_k(1)
     assert len(top_k) == 1
     assert top_k[0].doc_id == 1
     assert results.get_score_by_docid(0) == 0.9
 
 
 def test_result_attributes():
-    result = Result(doc_id=1, text="Doc 1", score=0.95, rank=1)
+    result = Result(document=Document(id=1, text="Doc 1"), score=0.95, rank=1)
     assert result.doc_id == 1
     assert result.text == "Doc 1"
     assert result.score == 0.95
     assert result.rank == 1
 
 
 def test_result_validation_error():
```

