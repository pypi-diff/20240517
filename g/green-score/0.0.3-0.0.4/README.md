# Comparing `tmp/green_score-0.0.3.tar.gz` & `tmp/green_score-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "green_score-0.0.3.tar", last modified: Fri May 17 05:04:48 2024, max compression
+gzip compressed data, was "green_score-0.0.4.tar", last modified: Fri May 17 18:25:26 2024, max compression
```

## Comparing `green_score-0.0.3.tar` & `green_score-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2024-05-17 05:04:48.544066 green_score-0.0.3/
--rw-rw-r--   0 jb        (1000) jb        (1000)     3529 2024-05-17 05:04:48.544066 green_score-0.0.3/PKG-INFO
--rw-rw-r--   0 jb        (1000) jb        (1000)     3208 2024-05-16 17:03:12.000000 green_score-0.0.3/README.md
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2024-05-17 05:04:48.544066 green_score-0.0.3/green_score/
--rw-rw-r--   0 jb        (1000) jb        (1000)       25 2024-05-16 16:46:03.000000 green_score-0.0.3/green_score/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    12798 2024-05-17 05:03:50.000000 green_score-0.0.3/green_score/green.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3460 2024-05-17 04:33:11.000000 green_score-0.0.3/green_score/utils.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2024-05-17 05:04:48.544066 green_score-0.0.3/green_score.egg-info/
--rw-rw-r--   0 jb        (1000) jb        (1000)     3529 2024-05-17 05:04:48.000000 green_score-0.0.3/green_score.egg-info/PKG-INFO
--rw-rw-r--   0 jb        (1000) jb        (1000)      292 2024-05-17 05:04:48.000000 green_score-0.0.3/green_score.egg-info/SOURCES.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)        1 2024-05-17 05:04:48.000000 green_score-0.0.3/green_score.egg-info/dependency_links.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)        1 2024-05-16 16:55:48.000000 green_score-0.0.3/green_score.egg-info/not-zip-safe
--rw-rw-r--   0 jb        (1000) jb        (1000)       71 2024-05-17 05:04:48.000000 green_score-0.0.3/green_score.egg-info/requires.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)       12 2024-05-17 05:04:48.000000 green_score-0.0.3/green_score.egg-info/top_level.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)       38 2024-05-17 05:04:48.544066 green_score-0.0.3/setup.cfg
--rw-rw-r--   0 jb        (1000) jb        (1000)      687 2024-05-17 05:04:30.000000 green_score-0.0.3/setup.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2024-05-17 18:25:26.624196 green_score-0.0.4/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3529 2024-05-17 18:25:26.624196 green_score-0.0.4/PKG-INFO
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3208 2024-05-16 17:03:12.000000 green_score-0.0.4/README.md
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2024-05-17 18:25:26.620195 green_score-0.0.4/green_score/
+-rw-rw-r--   0 jb        (1000) jb        (1000)       25 2024-05-16 16:46:03.000000 green_score-0.0.4/green_score/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    13009 2024-05-17 18:24:22.000000 green_score-0.0.4/green_score/green.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3460 2024-05-17 04:33:11.000000 green_score-0.0.4/green_score/utils.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2024-05-17 18:25:26.624196 green_score-0.0.4/green_score.egg-info/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3529 2024-05-17 18:25:26.000000 green_score-0.0.4/green_score.egg-info/PKG-INFO
+-rw-rw-r--   0 jb        (1000) jb        (1000)      292 2024-05-17 18:25:26.000000 green_score-0.0.4/green_score.egg-info/SOURCES.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)        1 2024-05-17 18:25:26.000000 green_score-0.0.4/green_score.egg-info/dependency_links.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)        1 2024-05-16 16:55:48.000000 green_score-0.0.4/green_score.egg-info/not-zip-safe
+-rw-rw-r--   0 jb        (1000) jb        (1000)       71 2024-05-17 18:25:26.000000 green_score-0.0.4/green_score.egg-info/requires.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)       12 2024-05-17 18:25:26.000000 green_score-0.0.4/green_score.egg-info/top_level.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)       38 2024-05-17 18:25:26.624196 green_score-0.0.4/setup.cfg
+-rw-rw-r--   0 jb        (1000) jb        (1000)      687 2024-05-17 18:25:12.000000 green_score-0.0.4/setup.py
```

### Comparing `green_score-0.0.3/PKG-INFO` & `green_score-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: green_score
-Version: 0.0.3
+Version: 0.0.4
 Author: Jean-Benoit Delbrouck
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `green_score-0.0.3/README.md` & `green_score-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `green_score-0.0.3/green_score/green.py` & `green_score-0.0.4/green_score/green.py`

 * *Files 3% similar despite different names*

```diff
@@ -230,42 +230,44 @@
         Returns:
             tuple: Mean green score, tensor of green scores, and list of processed responses.
         """
         assert len(refs) == len(hyps)
 
         with torch.no_grad():
             pairs_to_process = []
-            indices_to_process = []
             final_scores = torch.zeros(len(refs))
+            output_ids_dict = {}
 
+            # Iterate over ref-hyp pairs and populate final_scores and pairs_to_process
             for i, (ref, hyp) in enumerate(zip(refs, hyps)):
                 if (ref, hyp) in pair_to_reward_dict:
-                    final_scores[i] = pair_to_reward_dict[(ref, hyp)]
+                    final_scores[i], output_ids = pair_to_reward_dict[(ref, hyp)]
+                    output_ids_dict[i] = output_ids
                 else:
-                    pairs_to_process.append((ref, hyp))
-                    indices_to_process.append(i)
+                    pairs_to_process.append((ref, hyp, i))
 
             if pairs_to_process:
-                batch = [make_prompt(ref, hyp) for ref, hyp in pairs_to_process]
+                batch = [make_prompt(ref, hyp) for ref, hyp, _ in pairs_to_process]
                 batch = [[{"from": "human", "value": prompt}, {"from": "gpt", "value": ""}] for prompt in batch]
                 batch = tokenize_batch_as_chat(self.tokenizer, batch)
 
                 greens_tensor, output_ids = self.model(batch['input_ids'], batch['attention_mask'])
 
                 if len(greens_tensor) == len(pairs_to_process):
-                    for i, (ref, hyp) in enumerate(pairs_to_process):
-                        score = greens_tensor[i]
-                        pair_to_reward_dict[(ref, hyp)] = score
-                        final_scores[indices_to_process[i]] = score
+                    for (ref, hyp, idx), score, out_id in zip(pairs_to_process, greens_tensor, output_ids):
+                        pair_to_reward_dict[(ref, hyp)] = (score, out_id)
+                        final_scores[idx] = score
+                        output_ids_dict[idx] = out_id
                 else:
                     print("An inconsistency was detected in processing pairs.")
 
-            mean_green = final_scores.mean()
-            responses = self.tokenizer.batch_decode(output_ids, skip_special_tokens=True)
+            responses = [output_ids_dict[i] for i in range(len(refs))]
+            responses = self.tokenizer.batch_decode(responses, skip_special_tokens=True)
 
+            mean_green = final_scores.mean()
             return mean_green, final_scores, process_responses(responses)
 
 
 if __name__ == '__main__':
     model = GREEN(
         model_id_or_path="StanfordAIMI/GREEN",
         do_sample=False,  # should be always False
```

### Comparing `green_score-0.0.3/green_score/utils.py` & `green_score-0.0.4/green_score/utils.py`

 * *Files identical despite different names*

### Comparing `green_score-0.0.3/green_score.egg-info/PKG-INFO` & `green_score-0.0.4/green_score.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: green-score
-Version: 0.0.3
+Version: 0.0.4
 Author: Jean-Benoit Delbrouck
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `green_score-0.0.3/setup.py` & `green_score-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='green_score',
-    version='0.0.3',
+    version='0.0.4',
     author='Jean-Benoit Delbrouck',
     license='MIT',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

