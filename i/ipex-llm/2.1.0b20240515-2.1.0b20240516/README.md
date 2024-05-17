# Comparing `tmp/ipex_llm-2.1.0b20240515-py3-none-win_amd64.whl.zip` & `tmp/ipex_llm-2.1.0b20240516-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5368280 bytes, number of entries: 190
+Zip file size: 5367682 bytes, number of entries: 190
 -rw-------  2.0 unx     1898 b- defN 24-Mar-25 11:36 ipex_llm/__init__.py
 -rw-------  2.0 unx     6816 b- defN 24-Mar-25 11:36 ipex_llm/convert_model.py
 -rw-------  2.0 unx     3232 b- defN 24-May-07 15:07 ipex_llm/llm_patching.py
 -rw-------  2.0 unx     1177 b- defN 24-Mar-25 11:36 ipex_llm/models.py
 -rw-------  2.0 unx    12404 b- defN 24-Apr-18 12:34 ipex_llm/optimize.py
 -rw-------  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-chat.ps1
 -rwx------  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-cli.ps1
@@ -38,59 +38,59 @@
 -rw-------  2.0 unx     1189 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/__init__.py
 -rw-------  2.0 unx    13589 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/bigdlllm.py
 -rw-------  2.0 unx     7225 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/transformersembeddings.py
 -rw-------  2.0 unx     1636 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/__init__.py
 -rw-------  2.0 unx    24438 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/bigdlllm.py
 -rw-------  2.0 unx    10576 b- defN 24-Apr-03 15:07 ipex_llm/langchain/llms/transformersllm.py
 -rw-------  2.0 unx     7379 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/transformerspipelinellm.py
--rw-------  2.0 unx        0 b- defN 24-May-16 02:23 ipex_llm/libs/__init__.py
--rw-------  2.0 unx    36352 b- defN 24-May-16 02:23 ipex_llm/libs/bloom-api.dll
--rw-------  2.0 unx   473088 b- defN 24-May-16 02:23 ipex_llm/libs/bloom.dll
--rw-------  2.0 unx   854016 b- defN 24-May-16 02:23 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
--rw-------  2.0 unx   856576 b- defN 24-May-16 02:23 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
--rw-------  2.0 unx   844288 b- defN 24-May-16 02:23 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
--rw-------  2.0 unx    24576 b- defN 24-May-16 02:23 ipex_llm/libs/gptneox-api.dll
--rw-------  2.0 unx   532992 b- defN 24-May-16 02:23 ipex_llm/libs/gptneox.dll
--rw-------  2.0 unx   499712 b- defN 24-May-16 02:23 ipex_llm/libs/libbloom_avx.dll
--rw-------  2.0 unx   473600 b- defN 24-May-16 02:23 ipex_llm/libs/libbloom_vnni.dll
--rw-------  2.0 unx   559104 b- defN 24-May-16 02:23 ipex_llm/libs/libgptneox_avx.dll
--rw-------  2.0 unx   533504 b- defN 24-May-16 02:23 ipex_llm/libs/libgptneox_vnni.dll
--rw-------  2.0 unx   553472 b- defN 24-May-16 02:23 ipex_llm/libs/libllama_avx.dll
--rw-------  2.0 unx   527872 b- defN 24-May-16 02:23 ipex_llm/libs/libllama_vnni.dll
--rw-------  2.0 unx   590848 b- defN 24-May-16 02:23 ipex_llm/libs/libstarcoder_avx.dll
--rw-------  2.0 unx   564736 b- defN 24-May-16 02:23 ipex_llm/libs/libstarcoder_vnni.dll
--rw-------  2.0 unx    25088 b- defN 24-May-16 02:23 ipex_llm/libs/llama-api.dll
--rw-------  2.0 unx   526848 b- defN 24-May-16 02:23 ipex_llm/libs/llama.dll
--rw-------  2.0 unx   103424 b- defN 24-May-16 02:23 ipex_llm/libs/main-bloom.exe
--rw-------  2.0 unx   726016 b- defN 24-May-16 02:23 ipex_llm/libs/main-chatglm_vnni.exe
--rw-------  2.0 unx    98816 b- defN 24-May-16 02:23 ipex_llm/libs/main-gptneox.exe
--rw-------  2.0 unx    99840 b- defN 24-May-16 02:23 ipex_llm/libs/main-llama.exe
--rw-------  2.0 unx   157696 b- defN 24-May-16 02:23 ipex_llm/libs/main-starcoder.exe
--rw-------  2.0 unx   126464 b- defN 24-May-16 02:23 ipex_llm/libs/quantize-bloom.exe
--rw-------  2.0 unx   127488 b- defN 24-May-16 02:23 ipex_llm/libs/quantize-bloom_vnni.exe
--rw-------  2.0 unx   103936 b- defN 24-May-16 02:23 ipex_llm/libs/quantize-gptneox.exe
--rw-------  2.0 unx   104448 b- defN 24-May-16 02:23 ipex_llm/libs/quantize-gptneox_vnni.exe
--rw-------  2.0 unx   109056 b- defN 24-May-16 02:23 ipex_llm/libs/quantize-llama.exe
--rw-------  2.0 unx   110080 b- defN 24-May-16 02:23 ipex_llm/libs/quantize-llama_vnni.exe
--rw-------  2.0 unx   126976 b- defN 24-May-16 02:23 ipex_llm/libs/quantize-starcoder.exe
--rw-------  2.0 unx   128512 b- defN 24-May-16 02:23 ipex_llm/libs/quantize-starcoder_vnni.exe
--rw-------  2.0 unx    21504 b- defN 24-May-16 02:23 ipex_llm/libs/starcoder-api.dll
--rw-------  2.0 unx   564224 b- defN 24-May-16 02:23 ipex_llm/libs/starcoder.dll
+-rw-------  2.0 unx        0 b- defN 24-May-16 15:06 ipex_llm/libs/__init__.py
+-rw-------  2.0 unx    36352 b- defN 24-May-16 15:06 ipex_llm/libs/bloom-api.dll
+-rw-------  2.0 unx   473088 b- defN 24-May-16 15:06 ipex_llm/libs/bloom.dll
+-rw-------  2.0 unx   854016 b- defN 24-May-16 15:06 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
+-rw-------  2.0 unx   856576 b- defN 24-May-16 15:06 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
+-rw-------  2.0 unx   844288 b- defN 24-May-16 15:06 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
+-rw-------  2.0 unx    24576 b- defN 24-May-16 15:06 ipex_llm/libs/gptneox-api.dll
+-rw-------  2.0 unx   532992 b- defN 24-May-16 15:06 ipex_llm/libs/gptneox.dll
+-rw-------  2.0 unx   499712 b- defN 24-May-16 15:06 ipex_llm/libs/libbloom_avx.dll
+-rw-------  2.0 unx   473600 b- defN 24-May-16 15:06 ipex_llm/libs/libbloom_vnni.dll
+-rw-------  2.0 unx   559104 b- defN 24-May-16 15:06 ipex_llm/libs/libgptneox_avx.dll
+-rw-------  2.0 unx   533504 b- defN 24-May-16 15:06 ipex_llm/libs/libgptneox_vnni.dll
+-rw-------  2.0 unx   553472 b- defN 24-May-16 15:06 ipex_llm/libs/libllama_avx.dll
+-rw-------  2.0 unx   527872 b- defN 24-May-16 15:06 ipex_llm/libs/libllama_vnni.dll
+-rw-------  2.0 unx   590848 b- defN 24-May-16 15:06 ipex_llm/libs/libstarcoder_avx.dll
+-rw-------  2.0 unx   564736 b- defN 24-May-16 15:06 ipex_llm/libs/libstarcoder_vnni.dll
+-rw-------  2.0 unx    25088 b- defN 24-May-16 15:06 ipex_llm/libs/llama-api.dll
+-rw-------  2.0 unx   526848 b- defN 24-May-16 15:06 ipex_llm/libs/llama.dll
+-rw-------  2.0 unx   103424 b- defN 24-May-16 15:06 ipex_llm/libs/main-bloom.exe
+-rw-------  2.0 unx   726016 b- defN 24-May-16 15:06 ipex_llm/libs/main-chatglm_vnni.exe
+-rw-------  2.0 unx    98816 b- defN 24-May-16 15:06 ipex_llm/libs/main-gptneox.exe
+-rw-------  2.0 unx    99840 b- defN 24-May-16 15:06 ipex_llm/libs/main-llama.exe
+-rw-------  2.0 unx   157696 b- defN 24-May-16 15:06 ipex_llm/libs/main-starcoder.exe
+-rw-------  2.0 unx   126464 b- defN 24-May-16 15:06 ipex_llm/libs/quantize-bloom.exe
+-rw-------  2.0 unx   127488 b- defN 24-May-16 15:06 ipex_llm/libs/quantize-bloom_vnni.exe
+-rw-------  2.0 unx   103936 b- defN 24-May-16 15:06 ipex_llm/libs/quantize-gptneox.exe
+-rw-------  2.0 unx   104448 b- defN 24-May-16 15:06 ipex_llm/libs/quantize-gptneox_vnni.exe
+-rw-------  2.0 unx   109056 b- defN 24-May-16 15:06 ipex_llm/libs/quantize-llama.exe
+-rw-------  2.0 unx   110080 b- defN 24-May-16 15:06 ipex_llm/libs/quantize-llama_vnni.exe
+-rw-------  2.0 unx   126976 b- defN 24-May-16 15:06 ipex_llm/libs/quantize-starcoder.exe
+-rw-------  2.0 unx   128512 b- defN 24-May-16 15:06 ipex_llm/libs/quantize-starcoder_vnni.exe
+-rw-------  2.0 unx    21504 b- defN 24-May-16 15:06 ipex_llm/libs/starcoder-api.dll
+-rw-------  2.0 unx   564224 b- defN 24-May-16 15:06 ipex_llm/libs/starcoder.dll
 -rw-------  2.0 unx      874 b- defN 24-Mar-25 11:36 ipex_llm/llamaindex/__init__.py
 -rw-------  2.0 unx     1139 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/__init__.py
 -rw-------  2.0 unx    26314 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/bigdlllm.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/__init__.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/__init__.py
 -rw-------  2.0 unx    10084 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/bigdl_llm_model.py
 -rw-------  2.0 unx    19585 b- defN 24-May-16 02:22 ipex_llm/serving/fastchat/ipex_llm_worker.py
 -rw-------  2.0 unx    16649 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/model_worker.py
 -rw-------  2.0 unx    10801 b- defN 24-Apr-29 15:08 ipex_llm/serving/fastchat/vllm_worker.py
 -rw-------  2.0 unx     1005 b- defN 24-Mar-25 11:36 ipex_llm/transformers/__init__.py
 -rw-------  2.0 unx     1213 b- defN 24-Mar-25 11:36 ipex_llm/transformers/bmm.py
--rw-------  2.0 unx    75714 b- defN 24-May-16 02:22 ipex_llm/transformers/convert.py
+-rw-------  2.0 unx    75529 b- defN 24-May-16 15:06 ipex_llm/transformers/convert.py
 -rw-------  2.0 unx    14334 b- defN 24-Apr-26 15:08 ipex_llm/transformers/convert_ipex.py
 -rw-------  2.0 unx     4613 b- defN 24-Mar-25 11:36 ipex_llm/transformers/embedding.py
 -rw-------  2.0 unx     4247 b- defN 24-Apr-29 15:08 ipex_llm/transformers/kv.py
 -rw-------  2.0 unx     3289 b- defN 24-Apr-18 12:34 ipex_llm/transformers/lisa.py
 -rw-------  2.0 unx     6812 b- defN 24-May-13 15:08 ipex_llm/transformers/loader.py
 -rw-------  2.0 unx    15562 b- defN 24-May-16 02:22 ipex_llm/transformers/lookup.py
 -rw-------  2.0 unx    39846 b- defN 24-May-16 02:22 ipex_llm/transformers/low_bit_linear.py
@@ -129,44 +129,44 @@
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/transformers/gguf/models/model_implement/yuan2/__init__.py
 -rw-------  2.0 unx     2192 b- defN 24-Mar-25 11:36 ipex_llm/transformers/gguf/models/model_implement/yuan2/configuration_yuan.py
 -rw-------  2.0 unx    51084 b- defN 24-Mar-25 11:36 ipex_llm/transformers/gguf/models/model_implement/yuan2/yuan_hf_model.py
 -rw-------  2.0 unx     2658 b- defN 24-Mar-25 11:36 ipex_llm/transformers/layers/rope_embedding.py
 -rw-------  2.0 unx      584 b- defN 24-Mar-25 11:36 ipex_llm/transformers/models/__init__.py
 -rw-------  2.0 unx     7415 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/aquila.py
 -rw-------  2.0 unx    24239 b- defN 24-May-14 15:08 ipex_llm/transformers/models/baichuan.py
--rw-------  2.0 unx    29489 b- defN 24-May-10 15:07 ipex_llm/transformers/models/baichuan2.py
+-rw-------  2.0 unx    29360 b- defN 24-May-16 06:00 ipex_llm/transformers/models/baichuan2.py
 -rw-------  2.0 unx     6085 b- defN 24-Mar-25 11:36 ipex_llm/transformers/models/bert.py
 -rw-------  2.0 unx     8971 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/bloom.py
--rw-------  2.0 unx    13743 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/chatglm.py
--rw-------  2.0 unx    31837 b- defN 24-Apr-30 15:07 ipex_llm/transformers/models/chatglm2.py
+-rw-------  2.0 unx    14638 b- defN 24-May-16 15:06 ipex_llm/transformers/models/chatglm.py
+-rw-------  2.0 unx    31844 b- defN 24-May-16 06:00 ipex_llm/transformers/models/chatglm2.py
 -rw-------  2.0 unx     8697 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/chatglm2_32k.py
 -rw-------  2.0 unx    20978 b- defN 24-May-14 15:08 ipex_llm/transformers/models/cohere.py
 -rw-------  2.0 unx     8654 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/decilm.py
 -rw-------  2.0 unx    33549 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/falcon.py
 -rw-------  2.0 unx    12310 b- defN 24-Apr-19 15:09 ipex_llm/transformers/models/gemma.py
 -rw-------  2.0 unx     4342 b- defN 24-Mar-25 11:36 ipex_llm/transformers/models/gptbigcode.py
 -rw-------  2.0 unx    17973 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/gptj.py
 -rw-------  2.0 unx     6219 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/gptneox.py
 -rw-------  2.0 unx    11647 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/internlm.py
--rw-------  2.0 unx   101985 b- defN 24-May-16 02:22 ipex_llm/transformers/models/llama.py
+-rw-------  2.0 unx   108673 b- defN 24-May-16 15:06 ipex_llm/transformers/models/llama.py
 -rw-------  2.0 unx    54855 b- defN 24-May-14 15:08 ipex_llm/transformers/models/mistral.py
 -rw-------  2.0 unx    27151 b- defN 24-May-14 15:08 ipex_llm/transformers/models/mixtral.py
 -rw-------  2.0 unx     9540 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/mpt.py
 -rw-------  2.0 unx     7668 b- defN 24-Apr-29 15:08 ipex_llm/transformers/models/phi.py
--rw-------  2.0 unx    14199 b- defN 24-May-16 02:22 ipex_llm/transformers/models/phi3.py
+-rw-------  2.0 unx    11908 b- defN 24-May-16 15:06 ipex_llm/transformers/models/phi3.py
 -rw-------  2.0 unx     6268 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/phixtral.py
 -rw-------  2.0 unx    32210 b- defN 24-May-14 15:08 ipex_llm/transformers/models/qwen.py
 -rw-------  2.0 unx    37312 b- defN 24-May-14 15:08 ipex_llm/transformers/models/qwen2.py
--rw-------  2.0 unx    38484 b- defN 24-Apr-26 15:08 ipex_llm/transformers/models/qwen2_moe.py
+-rw-------  2.0 unx    38469 b- defN 24-May-16 06:00 ipex_llm/transformers/models/qwen2_moe.py
 -rw-------  2.0 unx    11712 b- defN 24-May-14 15:08 ipex_llm/transformers/models/qwen_vl.py
 -rw-------  2.0 unx     6135 b- defN 24-Mar-29 11:38 ipex_llm/transformers/models/rwkv4.py
 -rw-------  2.0 unx    10722 b- defN 24-Apr-09 15:06 ipex_llm/transformers/models/rwkv5.py
 -rw-------  2.0 unx    20911 b- defN 24-May-14 15:08 ipex_llm/transformers/models/stablelm.py
 -rw-------  2.0 unx     8805 b- defN 24-Apr-29 15:08 ipex_llm/transformers/models/starcoder2.py
--rw-------  2.0 unx    19638 b- defN 24-May-16 02:22 ipex_llm/transformers/models/utils.py
+-rw-------  2.0 unx    17396 b- defN 24-May-16 06:00 ipex_llm/transformers/models/utils.py
 -rw-------  2.0 unx    20200 b- defN 24-Apr-26 15:08 ipex_llm/transformers/models/yuan.py
 -rw-------  2.0 unx      874 b- defN 24-Mar-25 11:36 ipex_llm/utils/__init__.py
 -rw-------  2.0 unx   258647 b- defN 24-May-16 02:22 ipex_llm/utils/benchmark_util.py
 -rw-------  2.0 unx    18074 b- defN 24-Mar-25 11:36 ipex_llm/utils/convert_chatglm.py
 -rw-------  2.0 unx    72612 b- defN 24-Mar-25 11:36 ipex_llm/utils/convert_util.py
 -rw-------  2.0 unx     2093 b- defN 24-Mar-25 11:36 ipex_llm/utils/glibc_checker.py
 -rw-------  2.0 unx     2477 b- defN 24-Mar-25 11:36 ipex_llm/utils/ipex_importer.py
@@ -178,15 +178,15 @@
 -rw-------  2.0 unx     1763 b- defN 24-Mar-25 11:36 ipex_llm/utils/common/log4Error.py
 -rw-------  2.0 unx      585 b- defN 24-Apr-22 15:07 ipex_llm/vllm/__init__.py
 -rw-------  2.0 unx    18514 b- defN 24-Apr-26 15:08 ipex_llm/vllm/ipex_llm_gpu_executor.py
 -rw-------  2.0 unx     7208 b- defN 24-Apr-22 15:07 ipex_llm/vllm/model_convert.py
 -rw-------  2.0 unx      747 b- defN 24-Apr-22 15:07 ipex_llm/vllm/engine/__init__.py
 -rw-------  2.0 unx     5941 b- defN 24-Apr-26 15:08 ipex_llm/vllm/engine/engine.py
 -rw-------  2.0 unx    10564 b- defN 24-Apr-22 15:07 ipex_llm/vllm/entrypoints/openai/api_server.py
--rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240515.data/scripts/llm-chat.ps1
--rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240515.data/scripts/llm-cli.ps1
--rw-------  2.0 unx     4835 b- defN 24-May-16 02:23 ipex_llm-2.1.0b20240515.dist-info/METADATA
--rw-------  2.0 unx       98 b- defN 24-May-16 02:23 ipex_llm-2.1.0b20240515.dist-info/WHEEL
--rw-------  2.0 unx       61 b- defN 24-May-16 02:23 ipex_llm-2.1.0b20240515.dist-info/entry_points.txt
--rw-------  2.0 unx        9 b- defN 24-May-16 02:23 ipex_llm-2.1.0b20240515.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    18013 b- defN 24-May-16 02:23 ipex_llm-2.1.0b20240515.dist-info/RECORD
-190 files, 13309082 bytes uncompressed, 5339508 bytes compressed:  59.9%
+-rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240516.data/scripts/llm-chat.ps1
+-rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240516.data/scripts/llm-cli.ps1
+-rw-------  2.0 unx     4965 b- defN 24-May-16 15:07 ipex_llm-2.1.0b20240516.dist-info/METADATA
+-rw-------  2.0 unx       98 b- defN 24-May-16 15:07 ipex_llm-2.1.0b20240516.dist-info/WHEEL
+-rw-------  2.0 unx       61 b- defN 24-May-16 15:06 ipex_llm-2.1.0b20240516.dist-info/entry_points.txt
+-rw-------  2.0 unx        9 b- defN 24-May-16 15:06 ipex_llm-2.1.0b20240516.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    18013 b- defN 24-May-16 15:07 ipex_llm-2.1.0b20240516.dist-info/RECORD
+190 files, 13311940 bytes uncompressed, 5338910 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -543,29 +543,29 @@
 
 Filename: ipex_llm/vllm/engine/engine.py
 Comment: 
 
 Filename: ipex_llm/vllm/entrypoints/openai/api_server.py
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240515.data/scripts/llm-chat.ps1
+Filename: ipex_llm-2.1.0b20240516.data/scripts/llm-chat.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240515.data/scripts/llm-cli.ps1
+Filename: ipex_llm-2.1.0b20240516.data/scripts/llm-cli.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240515.dist-info/METADATA
+Filename: ipex_llm-2.1.0b20240516.dist-info/METADATA
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240515.dist-info/WHEEL
+Filename: ipex_llm-2.1.0b20240516.dist-info/WHEEL
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240515.dist-info/entry_points.txt
+Filename: ipex_llm-2.1.0b20240516.dist-info/entry_points.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240515.dist-info/top_level.txt
+Filename: ipex_llm-2.1.0b20240516.dist-info/top_level.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240515.dist-info/RECORD
+Filename: ipex_llm-2.1.0b20240516.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipex_llm/libs/bloom-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800036cc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu May 16 02:17:44 2024
+Time/Date		Thu May 16 15:02:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000003200
 SizeOfInitializedData	0000000000005e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000036cc
@@ -6375,16 +6375,17 @@
    180005621:	push   %rdx
    180005622:	add    %al,0x1(%rax)
    180005628:	pop    %rax
    180005629:	push   %rdx
    18000562a:	add    %al,0x1(%rax)
    180005630:	add    %al,(%rax)
    180005632:	add    %al,(%rax)
-   180005634:	enter  $0x456c,$0x66
-   180005638:	add    %al,(%rax)
+   180005634:	or     %ah,(%rax)
+   180005636:	rex.RX
+   180005637:	data16 add %al,(%rax)
    18000563a:	add    %al,(%rax)
    18000563c:	or     $0xe0000000,%eax
    180005641:	add    (%rax),%al
    180005643:	add    %cl,(%rcx,%rbx,2)
    180005646:	add    %al,(%rax)
    180005648:	or     $0x3f,%al
 	...
```

## ipex_llm/libs/bloom.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180055a28
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu May 16 02:17:44 2024
+Time/Date		Thu May 16 15:02:33 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000056000
 SizeOfInitializedData	00000000000bf400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000055a28
@@ -112392,18 +112392,17 @@
    18005e85d:	add    %al,(%rax)
    18005e85f:	add    %dh,0x76(%rax)
    18005e862:	add    $0x180,%eax
    18005e867:	add    %bh,0x76(%rax)
    18005e86a:	add    $0x180,%eax
    18005e86f:	add    %al,(%rax)
    18005e871:	add    %al,(%rax)
-   18005e873:	add    %cl,%al
-   18005e875:	insb   (%dx),%es:(%rdi)
-   18005e876:	rex.RB
-   18005e877:	data16 add %al,(%rax)
+   18005e873:	add    %cl,(%rcx)
+   18005e875:	and    %al,0x66(%rsi)
+   18005e878:	add    %al,(%rax)
    18005e87a:	add    %al,(%rax)
    18005e87c:	or     $0x50000000,%eax
    18005e881:	add    (%rax),%eax
    18005e883:	add    %ah,-0x5ffffa0e(%rax)
    18005e889:	out    %al,$0x5
 	...
    18005e8ff:	add    %dl,(%rax)
```

## ipex_llm/libs/gptneox-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002cbc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu May 16 02:17:44 2024
+Time/Date		Thu May 16 15:02:31 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002600
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002cbc
@@ -5058,15 +5058,16 @@
    1800049c0:	cmp    %al,0x0(%rdx)
    1800049c3:	addb   $0x0,(%rcx)
    1800049c6:	add    %al,(%rax)
    1800049c8:	rex
    1800049c9:	rex.X add %al,0x1(%rax)
    1800049d0:	add    %al,(%rax)
    1800049d2:	add    %al,(%rax)
-   1800049d4:	enter  $0x456c,$0x66
+   1800049d4:	(bad)
+   1800049d5:	and    %al,0x66(%rsi)
    1800049d8:	add    %al,(%rax)
    1800049da:	add    %al,(%rax)
    1800049dc:	or     $0xe0000000,%eax
    1800049e1:	add    (%rax),%al
    1800049e3:	add    %ah,0x0(%rsp,%rcx,2)
    1800049e7:	add    %ah,0x0(%rsi,%rsi,1)
 	...
```

## ipex_llm/libs/gptneox.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005d188
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu May 16 02:17:44 2024
+Time/Date		Thu May 16 15:02:33 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005da00
 SizeOfInitializedData	00000000000c6600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005d188
@@ -123776,16 +123776,17 @@
    18006611d:	add    %al,(%rax)
    18006611f:	add    %bh,0x18005f6(%rax)
    180066125:	add    %al,(%rax)
    180066127:	add    %al,%al
    180066129:	testb  $0x0,0x180(%rip)        # 0x1800662b0
    180066130:	add    %al,(%rax)
    180066132:	add    %al,(%rax)
-   180066134:	enter  $0x456c,$0x66
-   180066138:	add    %al,(%rax)
+   180066134:	or     %esp,(%rax)
+   180066136:	rex.RX
+   180066137:	data16 add %al,(%rax)
    18006613a:	add    %al,(%rax)
    18006613c:	or     $0x50000000,%eax
    180066141:	add    (%rax),%eax
    180066143:	add    %al,0x5b840006(%rbp,%rbp,2)
    18006614a:	(bad)
 	...
    18006617f:	add    %bh,%al
```

## ipex_llm/libs/libbloom_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005bba8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu May 16 02:00:39 2024
+Time/Date		Thu May 16 15:02:30 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c200
 SizeOfInitializedData	00000000000bfa00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005bba8
@@ -112361,30 +112361,32 @@
    180061eb9:	jae    0x180061ee8
    180061ebb:	jb     0x180061f32
    180061ebd:	outsb  %ds:(%rsi),(%dx)
    180061ebe:	outsb  %ds:(%rsi),(%dx)
    180061ebf:	gs jb  0x180061f1e
    180061ec2:	(bad)
    180061ec7:	sub    $0x6c697562,%eax
-   180061ecc:	fs sub $0x5c77656e,%eax
-   180061ed2:	pop    %rdi
-   180061ed3:	ja     0x180061f44
-   180061ed5:	jb     0x180061f42
-   180061ed7:	pop    %rsp
-   180061ed8:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180061edf:	insl   (%dx),%es:(%rdi)
-   180061ee0:	pop    %rsp
-   180061ee1:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180061ee8:	insl   (%dx),%es:(%rdi)
-   180061ee9:	pop    %rsp
-   180061eea:	jae    0x180061f5e
-   180061eec:	movsxd 0x67(%rdi,%riz,2),%ebx
-   180061ef0:	insl   (%dx),%es:(%rdi)
-   180061ef1:	insb   (%dx),%es:(%rdi)
-   180061ef2:	cs movsxd (%rax),%eax
+   180061ecc:	fs pop %rsp
+   180061ece:	pop    %rdi
+   180061ecf:	ja     0x180061f40
+   180061ed1:	jb     0x180061f3e
+   180061ed3:	pop    %rsp
+   180061ed4:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180061edb:	insl   (%dx),%es:(%rdi)
+   180061edc:	pop    %rsp
+   180061edd:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180061ee4:	insl   (%dx),%es:(%rdi)
+   180061ee5:	pop    %rsp
+   180061ee6:	jae    0x180061f5a
+   180061ee8:	movsxd 0x67(%rdi,%riz,2),%ebx
+   180061eec:	insl   (%dx),%es:(%rdi)
+   180061eed:	insb   (%dx),%es:(%rdi)
+   180061eee:	cs movsxd (%rax),%eax
+   180061ef1:	add    %al,(%rax)
+   180061ef3:	add    %al,(%rax)
    180061ef5:	add    %al,(%rax)
    180061ef7:	add    %al,0x47(%rdi)
    180061efa:	rex.WRB
    180061efb:	rex.WR pop %rdi
    180061efd:	push   %r11
    180061eff:	push   %rbx
    180061f00:	rex.RB push %r10
@@ -117907,16 +117909,17 @@
    18006578d:	add    %al,(%rax)
    18006578f:	add    %dh,-0x1a(%rax)
    180065792:	add    $0x180,%eax
    180065797:	add    %bh,-0x1a(%rax)
    18006579a:	add    $0x180,%eax
    18006579f:	add    %al,(%rax)
    1800657a1:	add    %al,(%rax)
-   1800657a3:	add    %al,%bh
-   1800657a5:	push   $0x6645
+   1800657a3:	add    %al,(%rsi)
+   1800657a5:	and    %al,0x66(%rsi)
+   1800657a8:	add    %al,(%rax)
    1800657aa:	add    %al,(%rax)
    1800657ac:	or     $0x50000000,%eax
    1800657b1:	add    (%rax),%eax
    1800657b3:	add    %ah,-0x5ffff99f(%rax)
    1800657b9:	rex.RXB (bad)
 	...
    1800657ff:	add    %dl,(%rax)
```

## ipex_llm/libs/libbloom_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180055c38
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu May 16 02:18:59 2024
+Time/Date		Thu May 16 15:03:26 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000056200
 SizeOfInitializedData	00000000000bf400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000055c38
@@ -112484,18 +112484,17 @@
    18005f83a:	add    $0x180,%eax
    18005f83f:	add    %dh,-0x7a(%rax)
    18005f842:	add    $0x180,%eax
    18005f847:	add    %bh,-0x7a(%rax)
    18005f84a:	add    $0x180,%eax
    18005f84f:	add    %al,(%rax)
    18005f851:	add    %al,(%rax)
-   18005f853:	add    %dl,(%rbx)
-   18005f855:	insl   (%dx),%es:(%rdi)
-   18005f856:	rex.RB
-   18005f857:	data16 add %al,(%rax)
+   18005f853:	add    %bh,(%rsi)
+   18005f855:	and    %al,0x66(%rsi)
+   18005f858:	add    %al,(%rax)
    18005f85a:	add    %al,(%rax)
    18005f85c:	or     $0x50000000,%eax
    18005f861:	add    (%rax),%eax
    18005f863:	add    %ah,(%rax)
    18005f865:	add    (%rsi),%al
    18005f867:	add    %ah,(%rax)
    18005f869:	call   0x18005f873
```

## ipex_llm/libs/libgptneox_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180063398
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu May 16 02:00:40 2024
+Time/Date		Thu May 16 15:02:30 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063c00
 SizeOfInitializedData	00000000000c6a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000063398
@@ -25383,15 +25383,15 @@
    180007cf0:	xor    %rsp,%rax
    180007cf3:	mov    %rax,0x50(%rsp)
    180007cf8:	mov    %r9,%rbp
    180007cfb:	mov    %r8,%rsi
    180007cfe:	mov    %rdx,%rbx
    180007d01:	mov    %rcx,%rdi
    180007d04:	mov    %rcx,0x28(%rsp)
-   180007d09:	lea    0x5dfa4(%rip),%r8        # 0x180065cb4
+   180007d09:	lea    0x5dfa0(%rip),%r8        # 0x180065cb0
    180007d10:	call   0x180007b70
    180007d15:	nop
    180007d16:	movl   $0xc470,0x14(%rdi)
    180007d1d:	movl   $0x1000,0x18(%rdi)
    180007d24:	movl   $0x1400,0x1c(%rdi)
    180007d2b:	movl   $0x28,0x20(%rdi)
    180007d32:	movl   $0x24,0x24(%rdi)
@@ -42253,15 +42253,15 @@
    1800176e3:	sub    $0x80,%rsp
    1800176ea:	mov    0x6dd97(%rip),%rax        # 0x180085488
    1800176f1:	xor    %rsp,%rax
    1800176f4:	mov    %rax,-0x8(%rbp)
    1800176f8:	mov    0x60(%rbp),%r13
    1800176fc:	mov    %r8,%r12
    1800176ff:	mov    %rcx,%rdi
-   180017702:	lea    0x4e5ab(%rip),%r8        # 0x180065cb4
+   180017702:	lea    0x4e5a7(%rip),%r8        # 0x180065cb0
    180017709:	lea    -0x28(%rbp),%rcx
    18001770d:	mov    %r9,%r15
    180017710:	call   0x180007b70
    180017715:	call   *0x4de0d(%rip)        # 0x180065528
    18001771b:	mov    -0x28(%rbp),%rbx
    18001771f:	lea    -0x50(%rbp),%rcx
    180017723:	xor    %r14d,%r14d
@@ -119353,36 +119353,38 @@
    1800657d9:	jae    0x180065808
    1800657db:	jb     0x180065852
    1800657dd:	outsb  %ds:(%rsi),(%dx)
    1800657de:	outsb  %ds:(%rsi),(%dx)
    1800657df:	gs jb  0x18006583e
    1800657e2:	(bad)
    1800657e7:	sub    $0x6c697562,%eax
-   1800657ec:	fs sub $0x5c77656e,%eax
-   1800657f2:	pop    %rdi
-   1800657f3:	ja     0x180065864
-   1800657f5:	jb     0x180065862
-   1800657f7:	pop    %rsp
-   1800657f8:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   1800657ff:	insl   (%dx),%es:(%rdi)
-   180065800:	pop    %rsp
-   180065801:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180065808:	insl   (%dx),%es:(%rdi)
-   180065809:	pop    %rsp
-   18006580a:	jae    0x18006587e
-   18006580c:	movsxd 0x70(%rdi,%riz,2),%ebx
-   180065810:	je     0x180065880
-   180065812:	outsl  %gs:(%rsi),(%dx)
-   180065814:	js     0x180065872
-   180065816:	addr32 jo 0x18006588d
-   180065819:	outsb  %ds:(%rsi),(%dx)
-   18006581a:	outsl  %gs:(%rsi),(%dx)
-   18006581c:	js     0x18006584b
-   18006581e:	jne    0x180065894
-   180065820:	imul   $0x0,0x68(%rsi,%rbp,1),%ebp
+   1800657ec:	fs pop %rsp
+   1800657ee:	pop    %rdi
+   1800657ef:	ja     0x180065860
+   1800657f1:	jb     0x18006585e
+   1800657f3:	pop    %rsp
+   1800657f4:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   1800657fb:	insl   (%dx),%es:(%rdi)
+   1800657fc:	pop    %rsp
+   1800657fd:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180065804:	insl   (%dx),%es:(%rdi)
+   180065805:	pop    %rsp
+   180065806:	jae    0x18006587a
+   180065808:	movsxd 0x70(%rdi,%riz,2),%ebx
+   18006580c:	je     0x18006587c
+   18006580e:	outsl  %gs:(%rsi),(%dx)
+   180065810:	js     0x18006586e
+   180065812:	addr32 jo 0x180065889
+   180065815:	outsb  %ds:(%rsi),(%dx)
+   180065816:	outsl  %gs:(%rsi),(%dx)
+   180065818:	js     0x180065847
+   18006581a:	jne    0x180065890
+   18006581c:	imul   $0x0,0x68(%rsi,%rbp,1),%ebp
+   180065824:	add    %al,(%rax)
+   180065826:	add    %al,(%rax)
    180065828:	rex.RXB push %r8
    18006582a:	push   %rsp
    18006582b:	rex.WRX
    18006582c:	rex.RB
    18006582d:	rex.WRXB pop %r8
    18006582f:	pop    %rdi
    180065830:	push   %r11
@@ -119751,37 +119753,39 @@
    180065c69:	jae    0x180065c98
    180065c6b:	jb     0x180065ce2
    180065c6d:	outsb  %ds:(%rsi),(%dx)
    180065c6e:	outsb  %ds:(%rsi),(%dx)
    180065c6f:	gs jb  0x180065cce
    180065c72:	(bad)
    180065c77:	sub    $0x6c697562,%eax
-   180065c7c:	fs sub $0x5c77656e,%eax
-   180065c82:	pop    %rdi
-   180065c83:	ja     0x180065cf4
-   180065c85:	jb     0x180065cf2
-   180065c87:	pop    %rsp
-   180065c88:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180065c8f:	insl   (%dx),%es:(%rdi)
-   180065c90:	pop    %rsp
-   180065c91:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180065c98:	insl   (%dx),%es:(%rdi)
-   180065c99:	pop    %rsp
-   180065c9a:	jae    0x180065d0e
-   180065c9c:	movsxd 0x70(%rdi,%riz,2),%ebx
-   180065ca0:	je     0x180065d10
-   180065ca2:	outsl  %gs:(%rsi),(%dx)
-   180065ca4:	js     0x180065d02
-   180065ca6:	addr32 jo 0x180065d1d
-   180065ca9:	outsb  %ds:(%rsi),(%dx)
-   180065caa:	outsl  %gs:(%rsi),(%dx)
-   180065cac:	js     0x180065cdc
-   180065cae:	movsxd 0x70(%rax),%esi
-   180065cb1:	add    %al,(%rax)
-   180065cb3:	add    %dh,0x62(%rdx)
+   180065c7c:	fs pop %rsp
+   180065c7e:	pop    %rdi
+   180065c7f:	ja     0x180065cf0
+   180065c81:	jb     0x180065cee
+   180065c83:	pop    %rsp
+   180065c84:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180065c8b:	insl   (%dx),%es:(%rdi)
+   180065c8c:	pop    %rsp
+   180065c8d:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180065c94:	insl   (%dx),%es:(%rdi)
+   180065c95:	pop    %rsp
+   180065c96:	jae    0x180065d0a
+   180065c98:	movsxd 0x70(%rdi,%riz,2),%ebx
+   180065c9c:	je     0x180065d0c
+   180065c9e:	outsl  %gs:(%rsi),(%dx)
+   180065ca0:	js     0x180065cfe
+   180065ca2:	addr32 jo 0x180065d19
+   180065ca5:	outsb  %ds:(%rsi),(%dx)
+   180065ca6:	outsl  %gs:(%rsi),(%dx)
+   180065ca8:	js     0x180065cd8
+   180065caa:	movsxd 0x70(%rax),%esi
+   180065cad:	add    %al,(%rax)
+   180065caf:	add    %dh,0x62(%rdx)
+   180065cb2:	add    %al,(%rax)
+   180065cb4:	add    %al,(%rax)
    180065cb6:	add    %al,(%rax)
    180065cb8:	(bad)
    180065cbd:	sub    $0x3a6d6c6c,%eax
    180065cc2:	and    %ch,0x61(%rdi,%rbp,2)
    180065cc6:	imul   $0x646f6d20,%fs:0x67(%rsi),%ebp
    180065cce:	gs insb (%dx),%es:(%rdi)
    180065cd0:	and    %ah,0x72(%rsi)
@@ -126119,30 +126123,32 @@
    180069f99:	jae    0x180069fc8
    180069f9b:	jb     0x18006a012
    180069f9d:	outsb  %ds:(%rsi),(%dx)
    180069f9e:	outsb  %ds:(%rsi),(%dx)
    180069f9f:	gs jb  0x180069ffe
    180069fa2:	(bad)
    180069fa7:	sub    $0x6c697562,%eax
-   180069fac:	fs sub $0x5c77656e,%eax
-   180069fb2:	pop    %rdi
-   180069fb3:	ja     0x18006a024
-   180069fb5:	jb     0x18006a022
-   180069fb7:	pop    %rsp
-   180069fb8:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180069fbf:	insl   (%dx),%es:(%rdi)
-   180069fc0:	pop    %rsp
-   180069fc1:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180069fc8:	insl   (%dx),%es:(%rdi)
-   180069fc9:	pop    %rsp
-   180069fca:	jae    0x18006a03e
-   180069fcc:	movsxd 0x67(%rdi,%riz,2),%ebx
-   180069fd0:	insl   (%dx),%es:(%rdi)
-   180069fd1:	insb   (%dx),%es:(%rdi)
-   180069fd2:	cs movsxd (%rax),%eax
+   180069fac:	fs pop %rsp
+   180069fae:	pop    %rdi
+   180069faf:	ja     0x18006a020
+   180069fb1:	jb     0x18006a01e
+   180069fb3:	pop    %rsp
+   180069fb4:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180069fbb:	insl   (%dx),%es:(%rdi)
+   180069fbc:	pop    %rsp
+   180069fbd:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180069fc4:	insl   (%dx),%es:(%rdi)
+   180069fc5:	pop    %rsp
+   180069fc6:	jae    0x18006a03a
+   180069fc8:	movsxd 0x67(%rdi,%riz,2),%ebx
+   180069fcc:	insl   (%dx),%es:(%rdi)
+   180069fcd:	insb   (%dx),%es:(%rdi)
+   180069fce:	cs movsxd (%rax),%eax
+   180069fd1:	add    %al,(%rax)
+   180069fd3:	add    %al,(%rax)
    180069fd5:	add    %al,(%rax)
    180069fd7:	add    %al,0x47(%rdi)
    180069fda:	rex.WRB
    180069fdb:	rex.WR pop %rdi
    180069fdd:	push   %r11
    180069fdf:	push   %rbx
    180069fe0:	rex.RB push %r10
@@ -129354,15 +129360,16 @@
    18006c057:	add    %al,%al
    18006c059:	push   %rsi
    18006c05a:	(bad)
    18006c05b:	addb   $0x0,(%rcx)
    18006c05e:	add    %al,(%rax)
    18006c060:	add    %al,(%rax)
    18006c062:	add    %al,(%rax)
-   18006c064:	enter  $0x4568,$0x66
+   18006c064:	(bad)
+   18006c065:	and    %al,0x66(%rsi)
    18006c068:	add    %al,(%rax)
    18006c06a:	add    %al,(%rax)
    18006c06c:	or     $0x50000000,%eax
    18006c071:	add    (%rax),%eax
    18006c073:	add    %al,-0x437bfffa(%rsp,%rcx,8)
    18006c07a:	(bad)
    18006c07b:	add    %al,(%rax)
```

## ipex_llm/libs/libgptneox_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005d398
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu May 16 02:19:00 2024
+Time/Date		Thu May 16 15:03:26 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005dc00
 SizeOfInitializedData	00000000000c6600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005d398
@@ -123925,17 +123925,16 @@
    1800660fd:	add    %al,(%rax)
    1800660ff:	add    %bh,0x18005f6(%rax)
    180066105:	add    %al,(%rax)
    180066107:	add    %al,%al
    180066109:	testb  $0x0,0x180(%rip)        # 0x180066290
    180066110:	add    %al,(%rax)
    180066112:	add    %al,(%rax)
-   180066114:	adc    $0x6d,%al
-   180066116:	rex.RB
-   180066117:	data16 add %al,(%rax)
+   180066114:	ds and %al,0x66(%rsi)
+   180066118:	add    %al,(%rax)
    18006611a:	add    %al,(%rax)
    18006611c:	or     $0x50000000,%eax
    180066121:	add    (%rax),%eax
    180066123:	add    %al,0x5d840006(%rbp,%rbp,2)
    18006612a:	(bad)
 	...
    18006617f:	add    %bh,%al
```

## ipex_llm/libs/libllama_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800620a8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu May 16 02:00:40 2024
+Time/Date		Thu May 16 15:02:30 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000062800
 SizeOfInitializedData	00000000000c6800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000620a8
@@ -25056,52 +25056,52 @@
    18000795d:	mov    %rax,%rcx
    180007960:	call   *0x5ccd2(%rip)        # 0x180064638
    180007966:	test   %eax,%eax
    180007968:	je     0x1800079a4
    18000796a:	mov    $0x2,%ecx
    18000796f:	call   *0x5cc9b(%rip)        # 0x180064610
    180007975:	mov    %rax,%rcx
-   180007978:	lea    0x5cf41(%rip),%rax        # 0x1800648c0
+   180007978:	lea    0x5cf39(%rip),%rax        # 0x1800648b8
    18000797f:	mov    %rax,0x20(%rsp)
    180007984:	mov    $0x65,%r9d
    18000798a:	lea    0x5ce7f(%rip),%r8        # 0x180064810
-   180007991:	lea    0x5ced0(%rip),%rdx        # 0x180064868
+   180007991:	lea    0x5cec8(%rip),%rdx        # 0x180064860
    180007998:	call   0x180015760
    18000799d:	call   *0x5cbb5(%rip)        # 0x180064558
    1800079a3:	int3
    1800079a4:	mov    (%rbx),%rcx
    1800079a7:	call   *0x5cc83(%rip)        # 0x180064630
    1800079ad:	cmp    $0xffffffffffffffff,%rax
    1800079b1:	jne    0x1800079eb
    1800079b3:	lea    0x3(%rax),%ecx
    1800079b6:	call   *0x5cc54(%rip)        # 0x180064610
    1800079bc:	mov    %rax,%rcx
-   1800079bf:	lea    0x5ceea(%rip),%rax        # 0x1800648b0
+   1800079bf:	lea    0x5cee2(%rip),%rax        # 0x1800648a8
    1800079c6:	mov    %rax,0x20(%rsp)
    1800079cb:	mov    $0x5b,%r9d
    1800079d1:	lea    0x5ce38(%rip),%r8        # 0x180064810
-   1800079d8:	lea    0x5ce89(%rip),%rdx        # 0x180064868
+   1800079d8:	lea    0x5ce81(%rip),%rdx        # 0x180064860
    1800079df:	call   0x180015760
    1800079e4:	call   *0x5cb6e(%rip)        # 0x180064558
    1800079ea:	int3
    1800079eb:	mov    %rax,0x8(%rbx)
    1800079ef:	xor    %r8d,%r8d
    1800079f2:	xor    %edx,%edx
    1800079f4:	mov    (%rbx),%rcx
    1800079f7:	call   *0x5cc3b(%rip)        # 0x180064638
    1800079fd:	test   %eax,%eax
    1800079ff:	je     0x180007a3b
    180007a01:	mov    $0x2,%ecx
    180007a06:	call   *0x5cc04(%rip)        # 0x180064610
    180007a0c:	mov    %rax,%rcx
-   180007a0f:	lea    0x5ceaa(%rip),%rax        # 0x1800648c0
+   180007a0f:	lea    0x5cea2(%rip),%rax        # 0x1800648b8
    180007a16:	mov    %rax,0x20(%rsp)
    180007a1b:	mov    $0x65,%r9d
    180007a21:	lea    0x5cde8(%rip),%r8        # 0x180064810
-   180007a28:	lea    0x5ce39(%rip),%rdx        # 0x180064868
+   180007a28:	lea    0x5ce31(%rip),%rdx        # 0x180064860
    180007a2f:	call   0x180015760
    180007a34:	call   *0x5cb1e(%rip)        # 0x180064558
    180007a3a:	int3
    180007a3b:	mov    %rbx,%rax
    180007a3e:	mov    0x68(%rsp),%rcx
    180007a43:	xor    %rsp,%rcx
    180007a46:	call   0x180061aa0
@@ -25110,15 +25110,15 @@
    180007a57:	pop    %rdi
    180007a58:	ret
    180007a59:	call   *0x5cad9(%rip)        # 0x180064538
    180007a5f:	mov    (%rax),%ecx
    180007a61:	call   *0x5cae9(%rip)        # 0x180064550
    180007a67:	mov    %rax,%r9
    180007a6a:	mov    %rdi,%r8
-   180007a6d:	lea    0x5ce24(%rip),%rdx        # 0x180064898
+   180007a6d:	lea    0x5ce1c(%rip),%rdx        # 0x180064890
    180007a74:	lea    0x48(%rsp),%rcx
    180007a79:	call   0x18000c010
    180007a7e:	nop
    180007a7f:	mov    %rax,%rdx
    180007a82:	lea    0x30(%rsp),%rcx
    180007a87:	call   0x1800086c0
    180007a8c:	lea    0x6accd(%rip),%rdx        # 0x180072760
@@ -25136,15 +25136,15 @@
    180007ab0:	xor    %rsp,%rax
    180007ab3:	mov    %rax,0x50(%rsp)
    180007ab8:	mov    %r9,%rbp
    180007abb:	mov    %r8,%rsi
    180007abe:	mov    %rdx,%rbx
    180007ac1:	mov    %rcx,%rdi
    180007ac4:	mov    %rcx,0x28(%rsp)
-   180007ac9:	lea    0x5d200(%rip),%r8        # 0x180064cd0
+   180007ac9:	lea    0x5d1fc(%rip),%r8        # 0x180064ccc
    180007ad0:	call   0x180007920
    180007ad5:	nop
    180007ad6:	movl   $0x7d00,0x14(%rdi)
    180007add:	movl   $0x200,0x18(%rdi)
    180007ae4:	movl   $0x1000,0x1c(%rdi)
    180007aeb:	movl   $0x100,0x20(%rdi)
    180007af2:	movl   $0x20,0x24(%rdi)
@@ -25155,15 +25155,15 @@
    180007b15:	lea    0x38(%rdi),%rcx
    180007b19:	call   0x1800085f0
    180007b1e:	nop
    180007b1f:	mov    $0x2,%ecx
    180007b24:	call   *0x5cae6(%rip)        # 0x180064610
    180007b2a:	mov    %rax,%rcx
    180007b2d:	mov    %rbx,%r8
-   180007b30:	lea    0x5d1a1(%rip),%rdx        # 0x180064cd8
+   180007b30:	lea    0x5d199(%rip),%rdx        # 0x180064cd0
    180007b37:	call   0x180015760
    180007b3c:	mov    $0x4,%r8d
    180007b42:	lea    0x20(%rsp),%rdx
    180007b47:	mov    %rdi,%rcx
    180007b4a:	call   0x180012ee0
    180007b4f:	mov    0x20(%rsp),%ebx
    180007b53:	cmp    $0x67676d6c,%ebx
@@ -25337,15 +25337,15 @@
    180007df2:	cmpq   $0x10,0x18(%rax)
    180007df7:	jb     0x180007dfc
    180007df9:	mov    (%rax),%rbx
    180007dfc:	mov    $0x2,%ecx
    180007e01:	call   *0x5c809(%rip)        # 0x180064610
    180007e07:	mov    %rax,%rcx
    180007e0a:	mov    %rbx,%r8
-   180007e0d:	lea    0x5cb5c(%rip),%rdx        # 0x180064970
+   180007e0d:	lea    0x5cb54(%rip),%rdx        # 0x180064968
    180007e14:	call   0x180015760
    180007e19:	mov    0x60(%rsp),%rdx
    180007e1e:	cmp    $0x10,%rdx
    180007e22:	jb     0x180007e59
    180007e24:	inc    %rdx
    180007e27:	mov    0x48(%rsp),%rcx
    180007e2c:	mov    %rcx,%rax
@@ -25373,15 +25373,15 @@
    180007e7f:	mov    %ebp,%edx
    180007e81:	lea    0x68(%rsp),%rcx
    180007e86:	call   0x18000eef0
    180007e8b:	nop
    180007e8c:	mov    %rax,%rcx
    180007e8f:	call   0x18000b8d0
    180007e94:	mov    %rax,%r8
-   180007e97:	lea    0x5cab2(%rip),%rdx        # 0x180064950
+   180007e97:	lea    0x5caaa(%rip),%rdx        # 0x180064948
    180007e9e:	lea    0x48(%rsp),%rcx
    180007ea3:	call   0x18000c010
    180007ea8:	nop
    180007ea9:	mov    %rax,%rdx
    180007eac:	lea    0x30(%rsp),%rcx
    180007eb1:	call   0x1800086c0
    180007eb6:	lea    0x6a8a3(%rip),%rdx        # 0x180072760
@@ -25391,15 +25391,15 @@
    180007ec8:	mov    %eax,%edx
    180007eca:	lea    0x48(%rsp),%rcx
    180007ecf:	call   0x18000eef0
    180007ed4:	nop
    180007ed5:	mov    %rax,%rcx
    180007ed8:	call   0x18000b8d0
    180007edd:	mov    %rax,%r8
-   180007ee0:	lea    0x5ca49(%rip),%rdx        # 0x180064930
+   180007ee0:	lea    0x5ca41(%rip),%rdx        # 0x180064928
    180007ee7:	lea    0x68(%rsp),%rcx
    180007eec:	call   0x18000c010
    180007ef1:	nop
    180007ef2:	mov    %rax,%rdx
    180007ef5:	lea    0x30(%rsp),%rcx
    180007efa:	call   0x1800086c0
    180007eff:	lea    0x6a85a(%rip),%rdx        # 0x180072760
@@ -27588,15 +27588,15 @@
    180009ae7:	cmpq   $0x10,0x18(%rax)
    180009aec:	jb     0x180009af1
    180009aee:	mov    (%rax),%rbx
    180009af1:	mov    $0x2,%ecx
    180009af6:	call   *0x5ab14(%rip)        # 0x180064610
    180009afc:	mov    %rax,%rcx
    180009aff:	mov    %rbx,%r8
-   180009b02:	lea    0x5ae97(%rip),%rdx        # 0x1800649a0
+   180009b02:	lea    0x5ae8f(%rip),%rdx        # 0x180064998
    180009b09:	call   0x180015760
    180009b0e:	mov    0x38(%rsp),%rdx
    180009b13:	cmp    $0x10,%rdx
    180009b17:	jb     0x180009b4f
    180009b19:	inc    %rdx
    180009b1c:	mov    0x20(%rsp),%rcx
    180009b21:	mov    %rcx,%rax
@@ -29876,15 +29876,15 @@
    18000b9c6:	mov    $0x2,%ecx
    18000b9cb:	call   *0x58c3f(%rip)        # 0x180064610
    18000b9d1:	mov    %rax,%rcx
    18000b9d4:	lea    0x5927d(%rip),%rax        # 0x180064c58
    18000b9db:	mov    %rax,0x20(%rsp)
    18000b9e0:	mov    $0x187,%r9d
    18000b9e6:	lea    0x59293(%rip),%r8        # 0x180064c80
-   18000b9ed:	lea    0x58e74(%rip),%rdx        # 0x180064868
+   18000b9ed:	lea    0x58e6c(%rip),%rdx        # 0x180064860
    18000b9f4:	call   0x180015760
    18000b9f9:	call   *0x58b59(%rip)        # 0x180064558
    18000b9ff:	int3
    18000ba00:	mov    0x3c(%r14),%ecx
    18000ba04:	test   %ecx,%ecx
    18000ba06:	je     0x18000ba65
    18000ba08:	sub    $0x1,%ecx
@@ -30497,19 +30497,19 @@
    18000c124:	mov    %r14,%rcx
    18000c127:	call   0x180019950
    18000c12c:	cmp    %r15d,%eax
    18000c12f:	je     0x18000c16b
    18000c131:	mov    $0x2,%ecx
    18000c136:	call   *0x584d4(%rip)        # 0x180064610
    18000c13c:	mov    %rax,%rcx
-   18000c13f:	lea    0x58742(%rip),%rax        # 0x180064888
+   18000c13f:	lea    0x5873a(%rip),%rax        # 0x180064880
    18000c146:	mov    %rax,0x20(%rsp)
    18000c14b:	mov    $0x40,%r9d
    18000c151:	lea    0x586b8(%rip),%r8        # 0x180064810
-   18000c158:	lea    0x58709(%rip),%rdx        # 0x180064868
+   18000c158:	lea    0x58701(%rip),%rdx        # 0x180064860
    18000c15f:	call   0x180015760
    18000c164:	call   *0x583ee(%rip)        # 0x180064558
    18000c16a:	int3
    18000c16b:	vpxor  %xmm0,%xmm0,%xmm0
    18000c16f:	vmovups %xmm0,0x0(%rbp)
    18000c174:	mov    %r12,0x10(%rbp)
    18000c178:	mov    %r12,0x18(%rbp)
@@ -30549,15 +30549,15 @@
    18000c1da:	mov    $0x2,%ecx
    18000c1df:	call   *0x5842b(%rip)        # 0x180064610
    18000c1e5:	mov    %rax,%rcx
    18000c1e8:	lea    0x585f9(%rip),%rax        # 0x1800647e8
    18000c1ef:	mov    %rax,0x20(%rsp)
    18000c1f4:	mov    $0x3d,%r9d
    18000c1fa:	lea    0x5860f(%rip),%r8        # 0x180064810
-   18000c201:	lea    0x58660(%rip),%rdx        # 0x180064868
+   18000c201:	lea    0x58658(%rip),%rdx        # 0x180064860
    18000c208:	call   0x180015760
    18000c20d:	call   *0x58345(%rip)        # 0x180064558
    18000c213:	int3
    18000c214:	call   0x18000b0f0
    18000c219:	int3
    18000c21a:	call   0x18000b540
    18000c21f:	int3
@@ -30647,15 +30647,15 @@
    18000c360:	mov    $0x2,%ecx
    18000c365:	call   *0x582a5(%rip)        # 0x180064610
    18000c36b:	mov    %rax,%rcx
    18000c36e:	lea    0x58c43(%rip),%rax        # 0x180064fb8
    18000c375:	mov    %rax,0x20(%rsp)
    18000c37a:	mov    $0x2b2,%r9d
    18000c380:	lea    0x588f9(%rip),%r8        # 0x180064c80
-   18000c387:	lea    0x584da(%rip),%rdx        # 0x180064868
+   18000c387:	lea    0x584d2(%rip),%rdx        # 0x180064860
    18000c38e:	call   0x180015760
    18000c393:	call   *0x581bf(%rip)        # 0x180064558
    18000c399:	int3
    18000c39a:	mov    (%r14),%r8d
    18000c39d:	mov    0x38(%rdi),%edx
    18000c3a0:	mov    0x80(%rbx),%rcx
    18000c3a7:	call   0x18003efc0
@@ -30671,15 +30671,15 @@
    18000c3cc:	mov    $0x2,%ecx
    18000c3d1:	call   *0x58239(%rip)        # 0x180064610
    18000c3d7:	mov    %rax,%rcx
    18000c3da:	lea    0x58bef(%rip),%rax        # 0x180064fd0
    18000c3e1:	mov    %rax,0x20(%rsp)
    18000c3e6:	mov    $0x2b6,%r9d
    18000c3ec:	lea    0x5888d(%rip),%r8        # 0x180064c80
-   18000c3f3:	lea    0x5846e(%rip),%rdx        # 0x180064868
+   18000c3f3:	lea    0x58466(%rip),%rdx        # 0x180064860
    18000c3fa:	call   0x180015760
    18000c3ff:	call   *0x58153(%rip)        # 0x180064558
    18000c405:	int3
    18000c406:	mov    %r13d,0x4(%rsi)
    18000c40a:	mov    %rsi,0x60(%rdi)
    18000c40e:	incq   0x78(%rbx)
    18000c412:	mov    %rsi,%rax
@@ -30753,16 +30753,16 @@
    18000c501:	mov    %rcx,%rbx
    18000c504:	jne    0x18000c540
    18000c506:	mov    $0x2,%ecx
    18000c50b:	call   *0x580ff(%rip)        # 0x180064610
    18000c511:	mov    $0x114,%r9d
    18000c517:	lea    0x582f2(%rip),%r8        # 0x180064810
    18000c51e:	mov    %rax,%rcx
-   18000c521:	lea    0x58340(%rip),%rdx        # 0x180064868
-   18000c528:	lea    0x584b5(%rip),%rax        # 0x1800649e4
+   18000c521:	lea    0x58338(%rip),%rdx        # 0x180064860
+   18000c528:	lea    0x584ad(%rip),%rax        # 0x1800649dc
    18000c52f:	mov    %rax,0x20(%rsp)
    18000c534:	call   0x180015760
    18000c539:	call   *0x58019(%rip)        # 0x180064558
    18000c53f:	int3
    18000c540:	cmpb   $0x0,0x10(%rcx)
    18000c544:	jne    0x18000c598
    18000c546:	lea    0x30(%rsp),%rcx
@@ -30979,16 +30979,16 @@
    18000c834:	add    $0x38,%rsp
    18000c838:	ret
    18000c839:	mov    $0x2,%ecx
    18000c83e:	call   *0x57dcc(%rip)        # 0x180064610
    18000c844:	mov    $0x10f,%r9d
    18000c84a:	lea    0x57fbf(%rip),%r8        # 0x180064810
    18000c851:	mov    %rax,%rcx
-   18000c854:	lea    0x5800d(%rip),%rdx        # 0x180064868
-   18000c85b:	lea    0x58166(%rip),%rax        # 0x1800649c8
+   18000c854:	lea    0x58005(%rip),%rdx        # 0x180064860
+   18000c85b:	lea    0x5815e(%rip),%rax        # 0x1800649c0
    18000c862:	mov    %rax,0x20(%rsp)
    18000c867:	call   0x180015760
    18000c86c:	call   *0x57ce6(%rip)        # 0x180064558
    18000c872:	int3
    18000c873:	int3
    18000c874:	int3
    18000c875:	int3
@@ -32489,15 +32489,15 @@
    18000e280:	mov    %rax,-0x30(%rbp)
    18000e284:	jne    0x18000e2c0
    18000e286:	mov    $0x2,%ecx
    18000e28b:	call   *0x5637f(%rip)        # 0x180064610
    18000e291:	mov    $0x4e8,%r9d
    18000e297:	lea    0x569e2(%rip),%r8        # 0x180064c80
    18000e29e:	mov    %rax,%rcx
-   18000e2a1:	lea    0x565c0(%rip),%rdx        # 0x180064868
+   18000e2a1:	lea    0x565b8(%rip),%rdx        # 0x180064860
    18000e2a8:	lea    0x57351(%rip),%rax        # 0x180065600
    18000e2af:	mov    %rax,0x20(%rsp)
    18000e2b4:	call   0x180015760
    18000e2b9:	call   *0x56299(%rip)        # 0x180064558
    18000e2bf:	int3
    18000e2c0:	mov    0x13e0(%r14),%ecx
    18000e2c7:	mov    0x13e4(%r14),%eax
@@ -33245,19 +33245,19 @@
    18000ef51:	mov    %rdi,0x10(%rbx)
    18000ef55:	mov    %rbx,%rcx
    18000ef58:	movq   $0xf,0x18(%rbx)
    18000ef60:	call   0x18000b5a0
    18000ef65:	mov    %rax,(%rbx)
    18000ef68:	movq   $0x15,0x10(%rbx)
    18000ef70:	movq   $0x1f,0x18(%rbx)
-   18000ef78:	vmovups 0x55998(%rip),%xmm0        # 0x180064918
+   18000ef78:	vmovups 0x55990(%rip),%xmm0        # 0x180064910
    18000ef80:	vmovups %xmm0,(%rax)
-   18000ef84:	mov    0x5599e(%rip),%ecx        # 0x180064928
+   18000ef84:	mov    0x55996(%rip),%ecx        # 0x180064920
    18000ef8a:	mov    %ecx,0x10(%rax)
-   18000ef8d:	movzbl 0x55998(%rip),%ecx        # 0x18006492c
+   18000ef8d:	movzbl 0x55990(%rip),%ecx        # 0x180064924
    18000ef94:	mov    %cl,0x14(%rax)
    18000ef97:	mov    %dil,0x15(%rax)
    18000ef9b:	jmp    0x18000efd1
    18000ef9d:	mov    0x40(%rsp),%rdx
    18000efa2:	lea    0x50(%rsp),%rcx
    18000efa7:	vpxor  %xmm1,%xmm1,%xmm1
    18000efab:	vmovdqu %xmm1,0x60(%rsp)
@@ -34952,15 +34952,15 @@
    180010b9e:	mov    $0x2,%ecx
    180010ba3:	call   *0x53a67(%rip)        # 0x180064610
    180010ba9:	mov    %rax,%rcx
    180010bac:	lea    0x53fc1(%rip),%rax        # 0x180064b74
    180010bb3:	mov    %rax,0x20(%rsp)
    180010bb8:	mov    $0x39e,%r9d
    180010bbe:	lea    0x540bb(%rip),%r8        # 0x180064c80
-   180010bc5:	lea    0x53c9c(%rip),%rdx        # 0x180064868
+   180010bc5:	lea    0x53c94(%rip),%rdx        # 0x180064860
    180010bcc:	call   0x180015760
    180010bd1:	call   *0x53981(%rip)        # 0x180064558
    180010bd7:	int3
    180010bd8:	lea    0x554f1(%rip),%rcx        # 0x1800660d0
    180010bdf:	call   0x180061248
    180010be4:	int3
    180010be5:	lea    0x547f4(%rip),%rdx        # 0x1800653e0
@@ -35838,48 +35838,48 @@
    1800119a2:	mov    $0x2,%ecx
    1800119a7:	call   *0x52c63(%rip)        # 0x180064610
    1800119ad:	mov    %rax,%rcx
    1800119b0:	lea    0x53489(%rip),%rax        # 0x180064e40
    1800119b7:	mov    %rax,0x20(%rsp)
    1800119bc:	mov    $0x25d,%r9d
    1800119c2:	lea    0x532b7(%rip),%r8        # 0x180064c80
-   1800119c9:	lea    0x52e98(%rip),%rdx        # 0x180064868
+   1800119c9:	lea    0x52e90(%rip),%rdx        # 0x180064860
    1800119d0:	call   0x180015760
    1800119d5:	call   *0x52b7d(%rip)        # 0x180064558
    1800119db:	int3
    1800119dc:	mov    $0x2,%ecx
    1800119e1:	call   *0x52c29(%rip)        # 0x180064610
    1800119e7:	mov    %rax,%rcx
-   1800119ea:	lea    0x52ecf(%rip),%rax        # 0x1800648c0
+   1800119ea:	lea    0x52ec7(%rip),%rax        # 0x1800648b8
    1800119f1:	mov    %rax,0x20(%rsp)
    1800119f6:	mov    $0x65,%r9d
    1800119fc:	lea    0x52e0d(%rip),%r8        # 0x180064810
-   180011a03:	lea    0x52e5e(%rip),%rdx        # 0x180064868
+   180011a03:	lea    0x52e56(%rip),%rdx        # 0x180064860
    180011a0a:	call   0x180015760
    180011a0f:	call   *0x52b43(%rip)        # 0x180064558
    180011a15:	int3
    180011a16:	mov    $0x2,%ecx
    180011a1b:	call   *0x52bef(%rip)        # 0x180064610
    180011a21:	mov    %rax,%rcx
-   180011a24:	lea    0x52e85(%rip),%rax        # 0x1800648b0
+   180011a24:	lea    0x52e7d(%rip),%rax        # 0x1800648a8
    180011a2b:	mov    %rax,0x20(%rsp)
    180011a30:	mov    $0x5b,%r9d
    180011a36:	lea    0x52dd3(%rip),%r8        # 0x180064810
-   180011a3d:	lea    0x52e24(%rip),%rdx        # 0x180064868
+   180011a3d:	lea    0x52e1c(%rip),%rdx        # 0x180064860
    180011a44:	call   0x180015760
    180011a49:	call   *0x52b09(%rip)        # 0x180064558
    180011a4f:	int3
    180011a50:	mov    $0x2,%ecx
    180011a55:	call   *0x52bb5(%rip)        # 0x180064610
    180011a5b:	mov    %rax,%rcx
    180011a5e:	lea    0x5310f(%rip),%rax        # 0x180064b74
    180011a65:	mov    %rax,0x20(%rsp)
    180011a6a:	mov    $0x255,%r9d
    180011a70:	lea    0x53209(%rip),%r8        # 0x180064c80
-   180011a77:	lea    0x52dea(%rip),%rdx        # 0x180064868
+   180011a77:	lea    0x52de2(%rip),%rdx        # 0x180064860
    180011a7e:	call   0x180015760
    180011a83:	call   *0x52acf(%rip)        # 0x180064558
    180011a89:	nop
    180011a8a:	mov    -0x50(%rbp),%rsi
    180011a8e:	jmp    0x180011aa9
    180011a90:	mov    0x100(%rbp),%rdi
    180011a97:	mov    0x40(%rsp),%rsi
@@ -36182,19 +36182,19 @@
    180011eeb:	test   %rsi,%rsi
    180011eee:	js     0x180011f31
    180011ef0:	vcvtsi2ss %rsi,%xmm1,%xmm1
    180011ef5:	jmp    0x180011f49
    180011ef7:	mov    $0x2,%ecx
    180011efc:	call   *0x5270e(%rip)        # 0x180064610
    180011f02:	mov    %rax,%rcx
-   180011f05:	lea    0x52abc(%rip),%rax        # 0x1800649c8
+   180011f05:	lea    0x52ab4(%rip),%rax        # 0x1800649c0
    180011f0c:	mov    %rax,0x20(%rsp)
    180011f11:	mov    $0x10f,%r9d
    180011f17:	lea    0x528f2(%rip),%r8        # 0x180064810
-   180011f1e:	lea    0x52943(%rip),%rdx        # 0x180064868
+   180011f1e:	lea    0x5293b(%rip),%rdx        # 0x180064860
    180011f25:	call   0x180015760
    180011f2a:	call   *0x52628(%rip)        # 0x180064558
    180011f30:	int3
    180011f31:	mov    %rsi,%rcx
    180011f34:	shr    $1,%rcx
    180011f37:	mov    %rsi,%rax
    180011f3a:	and    $0x1,%eax
@@ -36262,30 +36262,30 @@
    180012018:	cmp    %r13,%rbx
    18001201b:	je     0x1800120a2
    180012021:	mov    0xb0(%rsp),%r8
    180012029:	jmp    0x180011ed0
    18001202e:	mov    $0x2,%ecx
    180012033:	call   *0x525d7(%rip)        # 0x180064610
    180012039:	mov    %rax,%rcx
-   18001203c:	lea    0x529a1(%rip),%rax        # 0x1800649e4
+   18001203c:	lea    0x52999(%rip),%rax        # 0x1800649dc
    180012043:	mov    %rax,0x20(%rsp)
    180012048:	mov    $0x114,%r9d
    18001204e:	lea    0x527bb(%rip),%r8        # 0x180064810
-   180012055:	lea    0x5280c(%rip),%rdx        # 0x180064868
+   180012055:	lea    0x52804(%rip),%rdx        # 0x180064860
    18001205c:	call   0x180015760
    180012061:	call   *0x524f1(%rip)        # 0x180064558
    180012067:	int3
    180012068:	mov    $0x2,%ecx
    18001206d:	call   *0x5259d(%rip)        # 0x180064610
    180012073:	mov    %rax,%rcx
    180012076:	lea    0x52fa3(%rip),%rax        # 0x180065020
    18001207d:	mov    %rax,0x20(%rsp)
    180012082:	mov    $0x2e1,%r9d
    180012088:	lea    0x52bf1(%rip),%r8        # 0x180064c80
-   18001208f:	lea    0x527d2(%rip),%rdx        # 0x180064868
+   18001208f:	lea    0x527ca(%rip),%rdx        # 0x180064860
    180012096:	call   0x180015760
    18001209b:	call   *0x524b7(%rip)        # 0x180064558
    1800120a1:	int3
    1800120a2:	mov    0xa8(%rsp),%rbx
    1800120aa:	add    $0x60,%rsp
    1800120ae:	pop    %r15
    1800120b0:	pop    %r14
@@ -36319,15 +36319,15 @@
    1800120f8:	mov    $0x2,%ecx
    1800120fd:	call   *0x5250d(%rip)        # 0x180064610
    180012103:	mov    %rax,%rcx
    180012106:	lea    0x52f23(%rip),%rax        # 0x180065030
    18001210d:	mov    %rax,0x20(%rsp)
    180012112:	mov    $0x2ee,%r9d
    180012118:	lea    0x52b61(%rip),%r8        # 0x180064c80
-   18001211f:	lea    0x52742(%rip),%rdx        # 0x180064868
+   18001211f:	lea    0x5273a(%rip),%rdx        # 0x180064860
    180012126:	call   0x180015760
    18001212b:	call   *0x52427(%rip)        # 0x180064558
    180012131:	int3
    180012132:	movabs $0x4924924924924925,%rax
    18001213c:	imul   %rcx
    18001213f:	sar    $0x4,%rdx
    180012143:	mov    %rdx,%rax
@@ -36365,19 +36365,19 @@
    1800121c6:	mov    (%rbx),%rcx
    1800121c9:	call   *0x52469(%rip)        # 0x180064638
    1800121cf:	test   %eax,%eax
    1800121d1:	je     0x18001220d
    1800121d3:	mov    $0x2,%ecx
    1800121d8:	call   *0x52432(%rip)        # 0x180064610
    1800121de:	mov    %rax,%rcx
-   1800121e1:	lea    0x526d8(%rip),%rax        # 0x1800648c0
+   1800121e1:	lea    0x526d0(%rip),%rax        # 0x1800648b8
    1800121e8:	mov    %rax,0x20(%rsp)
    1800121ed:	mov    $0x65,%r9d
    1800121f3:	lea    0x52616(%rip),%r8        # 0x180064810
-   1800121fa:	lea    0x52667(%rip),%rdx        # 0x180064868
+   1800121fa:	lea    0x5265f(%rip),%rdx        # 0x180064860
    180012201:	call   0x180015760
    180012206:	call   *0x5234c(%rip)        # 0x180064558
    18001220c:	int3
    18001220d:	mov    0x58(%r14),%r8
    180012211:	mov    0x68(%r14),%rdx
    180012215:	mov    %rbx,%rcx
    180012218:	call   0x180012ee0
@@ -36418,26 +36418,26 @@
    18001229d:	mov    $0x2,%ecx
    1800122a2:	call   *0x52368(%rip)        # 0x180064610
    1800122a8:	mov    %rax,%rcx
    1800122ab:	lea    0x52d96(%rip),%rax        # 0x180065048
    1800122b2:	mov    %rax,0x20(%rsp)
    1800122b7:	mov    $0x2fc,%r9d
    1800122bd:	lea    0x529bc(%rip),%r8        # 0x180064c80
-   1800122c4:	lea    0x5259d(%rip),%rdx        # 0x180064868
+   1800122c4:	lea    0x52595(%rip),%rdx        # 0x180064860
    1800122cb:	call   0x180015760
    1800122d0:	call   *0x52282(%rip)        # 0x180064558
    1800122d6:	int3
    1800122d7:	mov    $0x2,%ecx
    1800122dc:	call   *0x5232e(%rip)        # 0x180064610
    1800122e2:	mov    %rax,%rcx
-   1800122e5:	lea    0x525d4(%rip),%rax        # 0x1800648c0
+   1800122e5:	lea    0x525cc(%rip),%rax        # 0x1800648b8
    1800122ec:	mov    %rax,0x20(%rsp)
    1800122f1:	mov    $0x65,%r9d
    1800122f7:	lea    0x52512(%rip),%r8        # 0x180064810
-   1800122fe:	lea    0x52563(%rip),%rdx        # 0x180064868
+   1800122fe:	lea    0x5255b(%rip),%rdx        # 0x180064860
    180012305:	call   0x180015760
    18001230a:	call   *0x52248(%rip)        # 0x180064558
    180012310:	int3
    180012311:	cmp    $0x1,%eax
    180012314:	jne    0x1800126cc
    18001231a:	mov    0x8(%rdx),%rcx
    18001231e:	sub    (%rdx),%rcx
@@ -36627,26 +36627,26 @@
    1800125fa:	mov    $0x2,%ecx
    1800125ff:	call   *0x5200b(%rip)        # 0x180064610
    180012605:	mov    %rax,%rcx
    180012608:	lea    0x52a51(%rip),%rax        # 0x180065060
    18001260f:	mov    %rax,0x20(%rsp)
    180012614:	mov    $0x313,%r9d
    18001261a:	lea    0x5265f(%rip),%r8        # 0x180064c80
-   180012621:	lea    0x52240(%rip),%rdx        # 0x180064868
+   180012621:	lea    0x52238(%rip),%rdx        # 0x180064860
    180012628:	call   0x180015760
    18001262d:	call   *0x51f25(%rip)        # 0x180064558
    180012633:	int3
    180012634:	mov    $0x2,%ecx
    180012639:	call   *0x51fd1(%rip)        # 0x180064610
    18001263f:	mov    %rax,%rcx
-   180012642:	lea    0x52277(%rip),%rax        # 0x1800648c0
+   180012642:	lea    0x5226f(%rip),%rax        # 0x1800648b8
    180012649:	mov    %rax,0x20(%rsp)
    18001264e:	mov    $0x65,%r9d
    180012654:	lea    0x521b5(%rip),%r8        # 0x180064810
-   18001265b:	lea    0x52206(%rip),%rdx        # 0x180064868
+   18001265b:	lea    0x521fe(%rip),%rdx        # 0x180064860
    180012662:	call   0x180015760
    180012667:	call   *0x51eeb(%rip)        # 0x180064558
    18001266d:	nop
    18001266e:	test   %r12,%r12
    180012671:	je     0x1800126cc
    180012673:	mov    %r12,%rbx
    180012676:	cmp    %rsi,%r12
@@ -37305,30 +37305,30 @@
    180012f40:	xor    %rsp,%rcx
    180012f43:	call   0x180061aa0
    180012f48:	add    $0x60,%rsp
    180012f4c:	pop    %rdi
    180012f4d:	pop    %rsi
    180012f4e:	pop    %rbx
    180012f4f:	ret
-   180012f50:	lea    0x51989(%rip),%rdx        # 0x1800648e0
+   180012f50:	lea    0x51981(%rip),%rdx        # 0x1800648d8
    180012f57:	lea    0x38(%rsp),%rcx
    180012f5c:	call   0x180007010
    180012f61:	nop
    180012f62:	mov    %rax,%rdx
    180012f65:	lea    0x20(%rsp),%rcx
    180012f6a:	call   0x1800086c0
    180012f6f:	lea    0x5f7ea(%rip),%rdx        # 0x180072760
    180012f76:	lea    0x20(%rsp),%rcx
    180012f7b:	call   0x180062612
    180012f80:	nop
    180012f81:	call   *0x515b1(%rip)        # 0x180064538
    180012f87:	mov    (%rax),%ecx
    180012f89:	call   *0x515c1(%rip)        # 0x180064550
    180012f8f:	mov    %rax,%r8
-   180012f92:	lea    0x51937(%rip),%rdx        # 0x1800648d0
+   180012f92:	lea    0x5192f(%rip),%rdx        # 0x1800648c8
    180012f99:	lea    0x38(%rsp),%rcx
    180012f9e:	call   0x18000c010
    180012fa3:	nop
    180012fa4:	mov    %rax,%rdx
    180012fa7:	lea    0x20(%rsp),%rcx
    180012fac:	call   0x1800086c0
    180012fb1:	lea    0x5f7a8(%rip),%rdx        # 0x180072760
@@ -37936,69 +37936,69 @@
    180013902:	call   0x180061484
    180013907:	mov    -0x48(%rbp),%r12
    18001390b:	mov    (%r12),%rcx
    18001390f:	jmp    0x180013010
    180013914:	mov    $0x2,%ecx
    180013919:	call   *0x50cf1(%rip)        # 0x180064610
    18001391f:	mov    %rax,%rcx
-   180013922:	lea    0x50f97(%rip),%rax        # 0x1800648c0
+   180013922:	lea    0x50f8f(%rip),%rax        # 0x1800648b8
    180013929:	mov    %rax,0x20(%rsp)
    18001392e:	mov    $0x65,%r9d
    180013934:	lea    0x50ed5(%rip),%r8        # 0x180064810
-   18001393b:	lea    0x50f26(%rip),%rdx        # 0x180064868
+   18001393b:	lea    0x50f1e(%rip),%rdx        # 0x180064860
    180013942:	call   0x180015760
    180013947:	call   *0x50c0b(%rip)        # 0x180064558
    18001394d:	int3
    18001394e:	mov    $0x2,%ecx
    180013953:	call   *0x50cb7(%rip)        # 0x180064610
    180013959:	mov    %rax,%rcx
-   18001395c:	lea    0x50f4d(%rip),%rax        # 0x1800648b0
+   18001395c:	lea    0x50f45(%rip),%rax        # 0x1800648a8
    180013963:	mov    %rax,0x20(%rsp)
    180013968:	mov    $0x5b,%r9d
    18001396e:	lea    0x50e9b(%rip),%r8        # 0x180064810
-   180013975:	lea    0x50eec(%rip),%rdx        # 0x180064868
+   180013975:	lea    0x50ee4(%rip),%rdx        # 0x180064860
    18001397c:	call   0x180015760
    180013981:	call   *0x50bd1(%rip)        # 0x180064558
    180013987:	nop
    180013988:	call   *0x50c12(%rip)        # 0x1800645a0
    18001398e:	nop
    18001398f:	call   *0x50c0b(%rip)        # 0x1800645a0
    180013995:	nop
    180013996:	call   *0x50c04(%rip)        # 0x1800645a0
    18001399c:	nop
    18001399d:	mov    $0x2,%ecx
    1800139a2:	call   *0x50c68(%rip)        # 0x180064610
    1800139a8:	mov    %rax,%rcx
-   1800139ab:	lea    0x50f0e(%rip),%rax        # 0x1800648c0
+   1800139ab:	lea    0x50f06(%rip),%rax        # 0x1800648b8
    1800139b2:	mov    %rax,0x20(%rsp)
    1800139b7:	mov    $0x65,%r9d
    1800139bd:	lea    0x50e4c(%rip),%r8        # 0x180064810
-   1800139c4:	lea    0x50e9d(%rip),%rdx        # 0x180064868
+   1800139c4:	lea    0x50e95(%rip),%rdx        # 0x180064860
    1800139cb:	call   0x180015760
    1800139d0:	call   *0x50b82(%rip)        # 0x180064558
    1800139d6:	int3
    1800139d7:	mov    $0x2,%ecx
    1800139dc:	call   *0x50c2e(%rip)        # 0x180064610
    1800139e2:	mov    %rax,%rcx
-   1800139e5:	lea    0x50ec4(%rip),%rax        # 0x1800648b0
+   1800139e5:	lea    0x50ebc(%rip),%rax        # 0x1800648a8
    1800139ec:	mov    %rax,0x20(%rsp)
    1800139f1:	mov    $0x5b,%r9d
    1800139f7:	lea    0x50e12(%rip),%r8        # 0x180064810
-   1800139fe:	lea    0x50e63(%rip),%rdx        # 0x180064868
+   1800139fe:	lea    0x50e5b(%rip),%rdx        # 0x180064860
    180013a05:	call   0x180015760
    180013a0a:	call   *0x50b48(%rip)        # 0x180064558
    180013a10:	nop
    180013a11:	mov    $0x2,%ecx
    180013a16:	call   *0x50bf4(%rip)        # 0x180064610
    180013a1c:	mov    %rax,%rcx
-   180013a1f:	lea    0x50e8a(%rip),%rax        # 0x1800648b0
+   180013a1f:	lea    0x50e82(%rip),%rax        # 0x1800648a8
    180013a26:	mov    %rax,0x20(%rsp)
    180013a2b:	mov    $0x5b,%r9d
    180013a31:	lea    0x50dd8(%rip),%r8        # 0x180064810
-   180013a38:	lea    0x50e29(%rip),%rdx        # 0x180064868
+   180013a38:	lea    0x50e21(%rip),%rdx        # 0x180064860
    180013a3f:	call   0x180015760
    180013a44:	call   *0x50b0e(%rip)        # 0x180064558
    180013a4a:	int3
    180013a4b:	mov    0x30(%rbp),%rcx
    180013a4f:	xor    %rsp,%rcx
    180013a52:	call   0x180061aa0
    180013a57:	mov    0x198(%rsp),%rbx
@@ -38018,30 +38018,30 @@
    180013a81:	lea    0x512d8(%rip),%rdx        # 0x180064d60
    180013a88:	lea    -0x10(%rbp),%rcx
    180013a8c:	call   0x18000c010
    180013a91:	lea    0x5edf8(%rip),%rdx        # 0x180072890
    180013a98:	lea    -0x10(%rbp),%rcx
    180013a9c:	call   0x180062612
    180013aa1:	nop
-   180013aa2:	lea    0x50e37(%rip),%rdx        # 0x1800648e0
+   180013aa2:	lea    0x50e2f(%rip),%rdx        # 0x1800648d8
    180013aa9:	lea    0x10(%rbp),%rcx
    180013aad:	call   0x180007010
    180013ab2:	nop
    180013ab3:	mov    %rax,%rdx
    180013ab6:	lea    -0x10(%rbp),%rcx
    180013aba:	call   0x1800086c0
    180013abf:	lea    0x5ec9a(%rip),%rdx        # 0x180072760
    180013ac6:	lea    -0x10(%rbp),%rcx
    180013aca:	call   0x180062612
    180013acf:	nop
    180013ad0:	call   *0x50a62(%rip)        # 0x180064538
    180013ad6:	mov    (%rax),%ecx
    180013ad8:	call   *0x50a72(%rip)        # 0x180064550
    180013ade:	mov    %rax,%r8
-   180013ae1:	lea    0x50de8(%rip),%rdx        # 0x1800648d0
+   180013ae1:	lea    0x50de0(%rip),%rdx        # 0x1800648c8
    180013ae8:	lea    0x10(%rbp),%rcx
    180013aec:	call   0x18000c010
    180013af1:	nop
    180013af2:	mov    %rax,%rdx
    180013af5:	lea    -0x10(%rbp),%rcx
    180013af9:	call   0x1800086c0
    180013afe:	lea    0x5ec5b(%rip),%rdx        # 0x180072760
@@ -38329,26 +38329,26 @@
    180013ef6:	vzeroupper
    180013ef9:	call   *0x506a1(%rip)        # 0x1800645a0
    180013eff:	nop
    180013f00:	call   *0x50632(%rip)        # 0x180064538
    180013f06:	mov    (%rax),%ecx
    180013f08:	call   *0x50642(%rip)        # 0x180064550
    180013f0e:	mov    %rax,%r8
-   180013f11:	lea    0x509b8(%rip),%rdx        # 0x1800648d0
+   180013f11:	lea    0x509b0(%rip),%rdx        # 0x1800648c8
    180013f18:	lea    -0x1(%rbp),%rcx
    180013f1c:	call   0x18000c010
    180013f21:	nop
    180013f22:	mov    %rax,%rdx
    180013f25:	lea    -0x39(%rbp),%rcx
    180013f29:	call   0x1800086c0
    180013f2e:	lea    0x5e82b(%rip),%rdx        # 0x180072760
    180013f35:	lea    -0x39(%rbp),%rcx
    180013f39:	call   0x180062612
    180013f3e:	nop
-   180013f3f:	lea    0x5099a(%rip),%rdx        # 0x1800648e0
+   180013f3f:	lea    0x50992(%rip),%rdx        # 0x1800648d8
    180013f46:	lea    -0x1(%rbp),%rcx
    180013f4a:	call   0x180007010
    180013f4f:	nop
    180013f50:	mov    %rax,%rdx
    180013f53:	lea    -0x39(%rbp),%rcx
    180013f57:	call   0x1800086c0
    180013f5c:	lea    0x5e7fd(%rip),%rdx        # 0x180072760
@@ -39827,15 +39827,15 @@
    18001530d:	pop    %rsi
    18001530e:	pop    %rbx
    18001530f:	ret
    180015310:	call   *0x4f222(%rip)        # 0x180064538
    180015316:	mov    (%rax),%ecx
    180015318:	call   *0x4f232(%rip)        # 0x180064550
    18001531e:	mov    %rax,%r8
-   180015321:	lea    0x4f5e0(%rip),%rdx        # 0x180064908
+   180015321:	lea    0x4f5d8(%rip),%rdx        # 0x180064900
    180015328:	lea    0x38(%rsp),%rcx
    18001532d:	call   0x18000c010
    180015332:	nop
    180015333:	mov    %rax,%rdx
    180015336:	lea    0x20(%rsp),%rcx
    18001533b:	call   0x1800086c0
    180015340:	lea    0x5d419(%rip),%rdx        # 0x180072760
@@ -39947,15 +39947,15 @@
    1800154c0:	pop    %r12
    1800154c2:	pop    %rdi
    1800154c3:	ret
    1800154c4:	call   *0x4f06e(%rip)        # 0x180064538
    1800154ca:	mov    (%rax),%ecx
    1800154cc:	call   *0x4f07e(%rip)        # 0x180064550
    1800154d2:	mov    %rax,%r8
-   1800154d5:	lea    0x4f42c(%rip),%rdx        # 0x180064908
+   1800154d5:	lea    0x4f424(%rip),%rdx        # 0x180064900
    1800154dc:	lea    0x40(%rsp),%rcx
    1800154e1:	call   0x18000c010
    1800154e6:	nop
    1800154e7:	mov    %rax,%rdx
    1800154ea:	lea    0x28(%rsp),%rcx
    1800154ef:	call   0x1800086c0
    1800154f4:	lea    0x5d265(%rip),%rdx        # 0x180072760
@@ -39964,15 +39964,15 @@
    180015505:	nop
    180015506:	call   0x18000b580
    18001550b:	int3
    18001550c:	call   *0x4f026(%rip)        # 0x180064538
    180015512:	mov    (%rax),%ecx
    180015514:	call   *0x4f036(%rip)        # 0x180064550
    18001551a:	mov    %rax,%r8
-   18001551d:	lea    0x4f3e4(%rip),%rdx        # 0x180064908
+   18001551d:	lea    0x4f3dc(%rip),%rdx        # 0x180064900
    180015524:	lea    0x40(%rsp),%rcx
    180015529:	call   0x18000c010
    18001552e:	nop
    18001552f:	mov    %rax,%rdx
    180015532:	lea    0x28(%rsp),%rcx
    180015537:	call   0x1800086c0
    18001553c:	lea    0x5d21d(%rip),%rdx        # 0x180072760
@@ -40534,15 +40534,15 @@
    180015d80:	cmp    %rcx,%r15
    180015d83:	jbe    0x180015dbf
    180015d85:	mov    $0x2,%ecx
    180015d8a:	call   *0x4e880(%rip)        # 0x180064610
    180015d90:	mov    $0xac1,%r9d
    180015d96:	lea    0x4eee3(%rip),%r8        # 0x180064c80
    180015d9d:	mov    %rax,%rcx
-   180015da0:	lea    0x4eac1(%rip),%rdx        # 0x180064868
+   180015da0:	lea    0x4eab9(%rip),%rdx        # 0x180064860
    180015da7:	lea    0x4ff9a(%rip),%rax        # 0x180065d48
    180015dae:	mov    %rax,0x20(%rsp)
    180015db3:	call   0x180015760
    180015db8:	call   *0x4e79a(%rip)        # 0x180064558
    180015dbe:	int3
    180015dbf:	mov    %r15,%rax
    180015dc2:	mov    0x18ff0(%rbp),%rcx
@@ -41173,15 +41173,15 @@
    180016742:	sub    $0xb8,%rsp
    180016749:	mov    0x6dd38(%rip),%rax        # 0x180084488
    180016750:	xor    %rsp,%rax
    180016753:	mov    %rax,-0x1(%rbp)
    180016757:	mov    0x7f(%rbp),%r13
    18001675b:	mov    %r8,%r12
    18001675e:	mov    %rcx,%rdi
-   180016761:	lea    0x4e568(%rip),%r8        # 0x180064cd0
+   180016761:	lea    0x4e564(%rip),%r8        # 0x180064ccc
    180016768:	lea    -0x21(%rbp),%rcx
    18001676c:	mov    %r9,%r15
    18001676f:	call   0x180007920
    180016774:	call   *0x4ddbe(%rip)        # 0x180064538
    18001677a:	mov    -0x21(%rbp),%rbx
    18001677e:	lea    -0x6d(%rbp),%rcx
    180016782:	xor    %r14d,%r14d
@@ -41278,16 +41278,16 @@
    180016922:	cmp    $0xffffffffffffffff,%rax
    180016926:	jne    0x180016960
    180016928:	lea    0x3(%rax),%ecx
    18001692b:	call   *0x4dcdf(%rip)        # 0x180064610
    180016931:	mov    $0x5b,%r9d
    180016937:	lea    0x4ded2(%rip),%r8        # 0x180064810
    18001693e:	mov    %rax,%rcx
-   180016941:	lea    0x4df20(%rip),%rdx        # 0x180064868
-   180016948:	lea    0x4df61(%rip),%rax        # 0x1800648b0
+   180016941:	lea    0x4df18(%rip),%rdx        # 0x180064860
+   180016948:	lea    0x4df59(%rip),%rax        # 0x1800648a8
    18001694f:	mov    %rax,0x20(%rsp)
    180016954:	call   0x180015760
    180016959:	call   *0x4dbf9(%rip)        # 0x180064558
    18001695f:	int3
    180016960:	mov    -0x19(%rbp),%rsi
    180016964:	mov    0x1540(%rdi),%r14
    18001696b:	sub    %rax,%rsi
@@ -41366,77 +41366,77 @@
    180016a99:	pop    %r13
    180016a9b:	pop    %r12
    180016a9d:	pop    %rdi
    180016a9e:	pop    %rsi
    180016a9f:	pop    %rbx
    180016aa0:	pop    %rbp
    180016aa1:	ret
-   180016aa2:	lea    0x4de37(%rip),%rdx        # 0x1800648e0
+   180016aa2:	lea    0x4de2f(%rip),%rdx        # 0x1800648d8
    180016aa9:	lea    -0x21(%rbp),%rcx
    180016aad:	call   0x180007010
    180016ab2:	mov    %rax,%rdx
    180016ab5:	lea    -0x69(%rbp),%rcx
    180016ab9:	call   0x1800086c0
    180016abe:	lea    0x5bc9b(%rip),%rdx        # 0x180072760
    180016ac5:	lea    -0x69(%rbp),%rcx
    180016ac9:	call   0x180062612
    180016ace:	int3
    180016acf:	call   *0x4da63(%rip)        # 0x180064538
    180016ad5:	mov    (%rax),%ecx
    180016ad7:	call   *0x4da73(%rip)        # 0x180064550
    180016add:	mov    %rax,%r8
-   180016ae0:	lea    0x4dde9(%rip),%rdx        # 0x1800648d0
+   180016ae0:	lea    0x4dde1(%rip),%rdx        # 0x1800648c8
    180016ae7:	lea    -0x21(%rbp),%rcx
    180016aeb:	call   0x18000c010
    180016af0:	mov    %rax,%rdx
    180016af3:	lea    -0x69(%rbp),%rcx
    180016af7:	call   0x1800086c0
    180016afc:	lea    0x5bc5d(%rip),%rdx        # 0x180072760
    180016b03:	lea    -0x69(%rbp),%rcx
    180016b07:	call   0x180062612
    180016b0c:	int3
-   180016b0d:	lea    0x4ddcc(%rip),%rdx        # 0x1800648e0
+   180016b0d:	lea    0x4ddc4(%rip),%rdx        # 0x1800648d8
    180016b14:	lea    -0x21(%rbp),%rcx
    180016b18:	call   0x180007010
    180016b1d:	mov    %rax,%rdx
    180016b20:	lea    -0x69(%rbp),%rcx
    180016b24:	call   0x1800086c0
    180016b29:	lea    0x5bc30(%rip),%rdx        # 0x180072760
    180016b30:	lea    -0x69(%rbp),%rcx
    180016b34:	call   0x180062612
    180016b39:	int3
    180016b3a:	call   *0x4d9f8(%rip)        # 0x180064538
    180016b40:	mov    (%rax),%ecx
    180016b42:	call   *0x4da08(%rip)        # 0x180064550
    180016b48:	mov    %rax,%r8
-   180016b4b:	lea    0x4dd7e(%rip),%rdx        # 0x1800648d0
+   180016b4b:	lea    0x4dd76(%rip),%rdx        # 0x1800648c8
    180016b52:	lea    -0x21(%rbp),%rcx
    180016b56:	call   0x18000c010
    180016b5b:	mov    %rax,%rdx
    180016b5e:	lea    -0x69(%rbp),%rcx
    180016b62:	call   0x1800086c0
    180016b67:	lea    0x5bbf2(%rip),%rdx        # 0x180072760
    180016b6e:	lea    -0x69(%rbp),%rcx
    180016b72:	call   0x180062612
    180016b77:	int3
-   180016b78:	lea    0x4dd61(%rip),%rdx        # 0x1800648e0
+   180016b78:	lea    0x4dd59(%rip),%rdx        # 0x1800648d8
    180016b7f:	lea    -0x21(%rbp),%rcx
    180016b83:	call   0x180007010
    180016b88:	mov    %rax,%rdx
    180016b8b:	lea    -0x69(%rbp),%rcx
    180016b8f:	call   0x1800086c0
    180016b94:	lea    0x5bbc5(%rip),%rdx        # 0x180072760
    180016b9b:	lea    -0x69(%rbp),%rcx
    180016b9f:	call   0x180062612
    180016ba4:	int3
    180016ba5:	call   *0x4d98d(%rip)        # 0x180064538
    180016bab:	mov    (%rax),%ecx
    180016bad:	call   *0x4d99d(%rip)        # 0x180064550
    180016bb3:	mov    %rax,%r8
-   180016bb6:	lea    0x4dd13(%rip),%rdx        # 0x1800648d0
+   180016bb6:	lea    0x4dd0b(%rip),%rdx        # 0x1800648c8
    180016bbd:	lea    -0x21(%rbp),%rcx
    180016bc1:	call   0x18000c010
    180016bc6:	mov    %rax,%rdx
    180016bc9:	lea    -0x69(%rbp),%rcx
    180016bcd:	call   0x1800086c0
    180016bd2:	lea    0x5bb87(%rip),%rdx        # 0x180072760
    180016bd9:	lea    -0x69(%rbp),%rcx
@@ -43592,85 +43592,85 @@
    180018b9d:	ret
    180018b9e:	call   *0x4b9fc(%rip)        # 0x1800645a0
    180018ba4:	int3
    180018ba5:	call   *0x4b98d(%rip)        # 0x180064538
    180018bab:	mov    (%rax),%ecx
    180018bad:	call   *0x4b99d(%rip)        # 0x180064550
    180018bb3:	mov    %rax,%r8
-   180018bb6:	lea    0x4bd4b(%rip),%rdx        # 0x180064908
+   180018bb6:	lea    0x4bd43(%rip),%rdx        # 0x180064900
    180018bbd:	lea    -0x38(%rbp),%rcx
    180018bc1:	call   0x18000c010
    180018bc6:	mov    %rax,%rdx
    180018bc9:	lea    -0x50(%rbp),%rcx
    180018bcd:	call   0x1800086c0
    180018bd2:	lea    0x59b87(%rip),%rdx        # 0x180072760
    180018bd9:	lea    -0x50(%rbp),%rcx
    180018bdd:	call   0x180062612
    180018be2:	int3
    180018be3:	call   *0x4b94f(%rip)        # 0x180064538
    180018be9:	mov    (%rax),%ecx
    180018beb:	call   *0x4b95f(%rip)        # 0x180064550
    180018bf1:	mov    %rax,%r8
-   180018bf4:	lea    0x4bd0d(%rip),%rdx        # 0x180064908
+   180018bf4:	lea    0x4bd05(%rip),%rdx        # 0x180064900
    180018bfb:	lea    -0x38(%rbp),%rcx
    180018bff:	call   0x18000c010
    180018c04:	mov    %rax,%rdx
    180018c07:	lea    -0x50(%rbp),%rcx
    180018c0b:	call   0x1800086c0
    180018c10:	lea    0x59b49(%rip),%rdx        # 0x180072760
    180018c17:	lea    -0x50(%rbp),%rcx
    180018c1b:	call   0x180062612
    180018c20:	int3
    180018c21:	call   *0x4b911(%rip)        # 0x180064538
    180018c27:	mov    (%rax),%ecx
    180018c29:	call   *0x4b921(%rip)        # 0x180064550
    180018c2f:	mov    %rax,%r8
-   180018c32:	lea    0x4bccf(%rip),%rdx        # 0x180064908
+   180018c32:	lea    0x4bcc7(%rip),%rdx        # 0x180064900
    180018c39:	lea    -0x38(%rbp),%rcx
    180018c3d:	call   0x18000c010
    180018c42:	mov    %rax,%rdx
    180018c45:	lea    -0x50(%rbp),%rcx
    180018c49:	call   0x1800086c0
    180018c4e:	lea    0x59b0b(%rip),%rdx        # 0x180072760
    180018c55:	lea    -0x50(%rbp),%rcx
    180018c59:	call   0x180062612
    180018c5e:	int3
    180018c5f:	call   *0x4b8d3(%rip)        # 0x180064538
    180018c65:	mov    (%rax),%ecx
    180018c67:	call   *0x4b8e3(%rip)        # 0x180064550
    180018c6d:	mov    %rax,%r8
-   180018c70:	lea    0x4bc91(%rip),%rdx        # 0x180064908
+   180018c70:	lea    0x4bc89(%rip),%rdx        # 0x180064900
    180018c77:	lea    -0x38(%rbp),%rcx
    180018c7b:	call   0x18000c010
    180018c80:	mov    %rax,%rdx
    180018c83:	lea    -0x50(%rbp),%rcx
    180018c87:	call   0x1800086c0
    180018c8c:	lea    0x59acd(%rip),%rdx        # 0x180072760
    180018c93:	lea    -0x50(%rbp),%rcx
    180018c97:	call   0x180062612
    180018c9c:	int3
    180018c9d:	call   *0x4b895(%rip)        # 0x180064538
    180018ca3:	mov    (%rax),%ecx
    180018ca5:	call   *0x4b8a5(%rip)        # 0x180064550
    180018cab:	mov    %rax,%r8
-   180018cae:	lea    0x4bc53(%rip),%rdx        # 0x180064908
+   180018cae:	lea    0x4bc4b(%rip),%rdx        # 0x180064900
    180018cb5:	lea    -0x38(%rbp),%rcx
    180018cb9:	call   0x18000c010
    180018cbe:	mov    %rax,%rdx
    180018cc1:	lea    -0x50(%rbp),%rcx
    180018cc5:	call   0x1800086c0
    180018cca:	lea    0x59a8f(%rip),%rdx        # 0x180072760
    180018cd1:	lea    -0x50(%rbp),%rcx
    180018cd5:	call   0x180062612
    180018cda:	int3
    180018cdb:	call   *0x4b857(%rip)        # 0x180064538
    180018ce1:	mov    (%rax),%ecx
    180018ce3:	call   *0x4b867(%rip)        # 0x180064550
    180018ce9:	mov    %rax,%r8
-   180018cec:	lea    0x4bc15(%rip),%rdx        # 0x180064908
+   180018cec:	lea    0x4bc0d(%rip),%rdx        # 0x180064900
    180018cf3:	lea    -0x38(%rbp),%rcx
    180018cf7:	call   0x18000c010
    180018cfc:	mov    %rax,%rdx
    180018cff:	lea    -0x50(%rbp),%rcx
    180018d03:	call   0x1800086c0
    180018d08:	lea    0x59a51(%rip),%rdx        # 0x180072760
    180018d0f:	lea    -0x50(%rbp),%rcx
@@ -43896,15 +43896,15 @@
    180019091:	test   %al,%al
    180019093:	je     0x1800190cf
    180019095:	mov    $0x2,%ecx
    18001909a:	call   *0x4b570(%rip)        # 0x180064610
    1800190a0:	mov    $0xad6,%r9d
    1800190a6:	lea    0x4bbd3(%rip),%r8        # 0x180064c80
    1800190ad:	mov    %rax,%rcx
-   1800190b0:	lea    0x4b7b1(%rip),%rdx        # 0x180064868
+   1800190b0:	lea    0x4b7a9(%rip),%rdx        # 0x180064860
    1800190b7:	lea    0x4cca2(%rip),%rax        # 0x180065d60
    1800190be:	mov    %rax,0x20(%rsp)
    1800190c3:	call   0x180015760
    1800190c8:	call   *0x4b48a(%rip)        # 0x180064558
    1800190ce:	int3
    1800190cf:	mov    0x17ff0(%rbp),%rax
    1800190d6:	movslq 0x4(%rax),%rcx
@@ -43935,15 +43935,15 @@
    18001916e:	cmp    %rdi,%rax
    180019171:	je     0x1800191ad
    180019173:	mov    $0x2,%ecx
    180019178:	call   *0x4b492(%rip)        # 0x180064610
    18001917e:	mov    $0xae1,%r9d
    180019184:	lea    0x4baf5(%rip),%r8        # 0x180064c80
    18001918b:	mov    %rax,%rcx
-   18001918e:	lea    0x4b6d3(%rip),%rdx        # 0x180064868
+   18001918e:	lea    0x4b6cb(%rip),%rdx        # 0x180064860
    180019195:	lea    0x4cbdc(%rip),%rax        # 0x180065d78
    18001919c:	mov    %rax,0x20(%rsp)
    1800191a1:	call   0x180015760
    1800191a6:	call   *0x4b3ac(%rip)        # 0x180064558
    1800191ac:	int3
    1800191ad:	test   %rbx,%rbx
    1800191b0:	je     0x1800191d0
@@ -43964,15 +43964,15 @@
    1800191f1:	cmp    %rdi,%rax
    1800191f4:	je     0x180019230
    1800191f6:	mov    $0x2,%ecx
    1800191fb:	call   *0x4b40f(%rip)        # 0x180064610
    180019201:	mov    $0xaf1,%r9d
    180019207:	lea    0x4ba72(%rip),%r8        # 0x180064c80
    18001920e:	mov    %rax,%rcx
-   180019211:	lea    0x4b650(%rip),%rdx        # 0x180064868
+   180019211:	lea    0x4b648(%rip),%rdx        # 0x180064860
    180019218:	lea    0x4cb81(%rip),%rax        # 0x180065da0
    18001921f:	mov    %rax,0x20(%rsp)
    180019224:	call   0x180015760
    180019229:	call   *0x4b329(%rip)        # 0x180064558
    18001922f:	int3
    180019230:	test   %rdi,%rdi
    180019233:	je     0x18001924b
@@ -43995,15 +43995,15 @@
    180019280:	cmp    %rax,0x1448(%r15)
    180019287:	je     0x1800192c3
    180019289:	mov    $0x2,%ecx
    18001928e:	call   *0x4b37c(%rip)        # 0x180064610
    180019294:	mov    $0xb08,%r9d
    18001929a:	lea    0x4b9df(%rip),%r8        # 0x180064c80
    1800192a1:	mov    %rax,%rcx
-   1800192a4:	lea    0x4b5bd(%rip),%rdx        # 0x180064868
+   1800192a4:	lea    0x4b5b5(%rip),%rdx        # 0x180064860
    1800192ab:	lea    0x4cb1e(%rip),%rax        # 0x180065dd0
    1800192b2:	mov    %rax,0x20(%rsp)
    1800192b7:	call   0x180015760
    1800192bc:	call   *0x4b296(%rip)        # 0x180064558
    1800192c2:	int3
    1800192c3:	mov    0x1428(%r15),%rcx
    1800192ca:	call   0x18003b060
@@ -44117,15 +44117,15 @@
    1800194c4:	cmp    %rcx,%rbx
    1800194c7:	jbe    0x180019503
    1800194c9:	mov    $0x2,%ecx
    1800194ce:	call   *0x4b13c(%rip)        # 0x180064610
    1800194d4:	mov    $0xb2f,%r9d
    1800194da:	lea    0x4b79f(%rip),%r8        # 0x180064c80
    1800194e1:	mov    %rax,%rcx
-   1800194e4:	lea    0x4b37d(%rip),%rdx        # 0x180064868
+   1800194e4:	lea    0x4b375(%rip),%rdx        # 0x180064860
    1800194eb:	lea    0x4c8fe(%rip),%rax        # 0x180065df0
    1800194f2:	mov    %rax,0x20(%rsp)
    1800194f7:	call   0x180015760
    1800194fc:	call   *0x4b056(%rip)        # 0x180064558
    180019502:	int3
    180019503:	mov    %rbx,%rax
    180019506:	mov    0x18ff0(%rbp),%rcx
@@ -117965,171 +117965,168 @@
    180064819:	jae    0x180064848
    18006481b:	jb     0x180064892
    18006481d:	outsb  %ds:(%rsi),(%dx)
    18006481e:	outsb  %ds:(%rsi),(%dx)
    18006481f:	gs jb  0x18006487e
    180064822:	(bad)
    180064827:	sub    $0x6c697562,%eax
-   18006482c:	fs sub $0x5c77656e,%eax
-   180064832:	pop    %rdi
-   180064833:	ja     0x1800648a4
-   180064835:	jb     0x1800648a2
-   180064837:	pop    %rsp
-   180064838:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18006483f:	insl   (%dx),%es:(%rdi)
-   180064840:	pop    %rsp
-   180064841:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180064848:	insl   (%dx),%es:(%rdi)
-   180064849:	pop    %rsp
-   18006484a:	jae    0x1800648be
-   18006484c:	movsxd 0x6c(%rsp,%rbp,2),%ebx
-   180064850:	(bad)
-   180064851:	insl   (%dx),%es:(%rdi)
+   18006482c:	fs pop %rsp
+   18006482e:	pop    %rdi
+   18006482f:	ja     0x1800648a0
+   180064831:	jb     0x18006489e
+   180064833:	pop    %rsp
+   180064834:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18006483b:	insl   (%dx),%es:(%rdi)
+   18006483c:	pop    %rsp
+   18006483d:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180064844:	insl   (%dx),%es:(%rdi)
+   180064845:	pop    %rsp
+   180064846:	jae    0x1800648ba
+   180064848:	movsxd 0x6c(%rsp,%rbp,2),%ebx
+   18006484c:	(bad)
+   18006484d:	insl   (%dx),%es:(%rdi)
+   18006484e:	(bad)
+   18006484f:	pop    %rsp
+   180064850:	insb   (%dx),%es:(%rdi)
+   180064851:	insb   (%dx),%es:(%rdi)
    180064852:	(bad)
-   180064853:	pop    %rsp
-   180064854:	insb   (%dx),%es:(%rdi)
-   180064855:	insb   (%dx),%es:(%rdi)
-   180064856:	(bad)
-   180064857:	insl   (%dx),%es:(%rdi)
-   180064858:	(bad)
-   180064859:	sub    $0x6c697475,%eax
-   18006485e:	cs push $0x0
-   180064864:	add    %al,(%rax)
-   180064866:	add    %al,(%rax)
-   180064868:	rex.WR
-   180064869:	rex.WR
-   18006486a:	rex.B
-   18006486b:	rex.WRB
-   18006486c:	pop    %r15
-   18006486e:	push   %r11
-   180064870:	push   %rbx
-   180064871:	rex.RB push %r10
-   180064873:	push   %rsp
-   180064874:	cmp    (%rax),%ah
-   180064876:	and    $0x64253a73,%eax
-   18006487b:	cmp    (%rax),%ah
-   18006487d:	and    $0xa73,%eax
-   180064882:	add    %al,(%rax)
-   180064884:	add    %al,(%rax)
-   180064886:	add    %al,(%rax)
-   180064888:	jae    0x1800648f3
-   18006488a:	jp     0x1800648f1
-   18006488c:	xor    (%rax),%ah
-   18006488e:	cmp    $0x6973203d,%eax
-   180064893:	jp     0x1800648fa
-   180064895:	add    %al,(%rax)
-   180064897:	add    %ah,0x61(%rsi)
-   18006489a:	imul   $0x206f7420,0x64(%rbp,%riz,2),%ebp
-   1800648a2:	outsl  %ds:(%rsi),(%dx)
-   1800648a3:	jo     0x18006490a
-   1800648a5:	outsb  %ds:(%rsi),(%dx)
-   1800648a6:	and    %ah,0x25203a73(%rip)        # 0x1a526831f
-   1800648ac:	jae    0x1800648ae
-   1800648ae:	add    %al,(%rax)
-   1800648b0:	jb     0x180064917
-   1800648b2:	je     0x1800648d4
-   1800648b4:	and    %edi,0x312d20(%rip)        # 0x1803775da
-   1800648ba:	add    %al,(%rax)
-   1800648bc:	add    %al,(%rax)
-   1800648be:	add    %al,(%rax)
-   1800648c0:	jb     0x180064927
-   1800648c2:	je     0x1800648e4
-   1800648c4:	cmp    $0x30203d,%eax
-   1800648c9:	add    %al,(%rax)
-   1800648cb:	add    %al,(%rax)
-   1800648cd:	add    %al,(%rax)
-   1800648cf:	add    %dh,0x65(%rdx)
-   1800648d2:	(bad)
-   1800648d3:	and    %ah,%fs:0x72(%rbp)
-   1800648d7:	jb     0x180064948
-   1800648d9:	jb     0x180064915
-   1800648db:	and    %ah,0x75000073(%rip)        # 0x1f5064954
-   1800648e1:	outsb  %ds:(%rsi),(%dx)
-   1800648e2:	gs js  0x180064955
-   1800648e5:	movsxd %gs:0x64(%rbp,%riz,2),%esi
-   1800648ea:	insb   (%dx),%es:(%rdi)
-   1800648eb:	jns    0x18006490d
-   1800648ed:	jb     0x180064954
-   1800648ef:	(bad)
-   1800648f0:	movsxd 0x65(%rax),%ebp
-   1800648f3:	and    %ah,%fs:0x6e(%rbp)
-   1800648f7:	and    %ch,%fs:0x66(%rdi)
-   1800648fb:	and    %ah,0x69(%rsi)
-   1800648fe:	insb   (%dx),%es:(%rdi)
-   1800648ff:	add    %al,%gs:(%rax)
-   180064902:	add    %al,(%rax)
-   180064904:	add    %al,(%rax)
-   180064906:	add    %al,(%rax)
-   180064908:	ja     0x18006497c
-   18006490a:	imul   $0x6f727265,0x20(%rbp,%riz,2),%esi
-   180064912:	jb     0x18006494e
-   180064914:	and    %ah,0x6f460073(%rip)        # 0x1ef4c498d
-   18006491a:	jb     0x180064989
-   18006491c:	(bad)
-   18006491d:	je     0x18006496c
-   18006491f:	gs jae 0x180064995
-   180064922:	(bad)
-   180064923:	and    %spl,%gs:0x61(%r14d)
-   180064929:	imul   $0x43000000,0x64(%rbp,%riz,2),%ebp
-   180064931:	jb     0x180064998
-   180064933:	(bad)
-   180064934:	je     0x18006499b
-   180064936:	imul   $0x69707061,0x4d(%rbp,%r12,2),%r13d
-   18006493f:	outsb  %ds:(%rsi),(%dx)
-   180064940:	and    %spl,0x61(%r14d)
-   180064945:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
-   18006494d:	add    %al,(%rax)
-   18006494f:	add    %cl,0x61(%rbp)
-   180064952:	jo     0x1800649aa
-   180064954:	imul   $0x6946664f,0x77(%rbp),%esp
-   18006495b:	insb   (%dx),%es:(%rdi)
-   18006495c:	and    %ah,%gs:0x61(%rsi)
-   180064960:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
+   180064853:	insl   (%dx),%es:(%rdi)
+   180064854:	(bad)
+   180064855:	sub    $0x6c697475,%eax
+   18006485a:	cs push $0x0
+   180064860:	rex.WR
+   180064861:	rex.WR
+   180064862:	rex.B
+   180064863:	rex.WRB
+   180064864:	pop    %r15
+   180064866:	push   %r11
+   180064868:	push   %rbx
+   180064869:	rex.RB push %r10
+   18006486b:	push   %rsp
+   18006486c:	cmp    (%rax),%ah
+   18006486e:	and    $0x64253a73,%eax
+   180064873:	cmp    (%rax),%ah
+   180064875:	and    $0xa73,%eax
+   18006487a:	add    %al,(%rax)
+   18006487c:	add    %al,(%rax)
+   18006487e:	add    %al,(%rax)
+   180064880:	jae    0x1800648eb
+   180064882:	jp     0x1800648e9
+   180064884:	xor    (%rax),%ah
+   180064886:	cmp    $0x6973203d,%eax
+   18006488b:	jp     0x1800648f2
+   18006488d:	add    %al,(%rax)
+   18006488f:	add    %ah,0x61(%rsi)
+   180064892:	imul   $0x206f7420,0x64(%rbp,%riz,2),%ebp
+   18006489a:	outsl  %ds:(%rsi),(%dx)
+   18006489b:	jo     0x180064902
+   18006489d:	outsb  %ds:(%rsi),(%dx)
+   18006489e:	and    %ah,0x25203a73(%rip)        # 0x1a5268317
+   1800648a4:	jae    0x1800648a6
+   1800648a6:	add    %al,(%rax)
+   1800648a8:	jb     0x18006490f
+   1800648aa:	je     0x1800648cc
+   1800648ac:	and    %edi,0x312d20(%rip)        # 0x1803775d2
+   1800648b2:	add    %al,(%rax)
+   1800648b4:	add    %al,(%rax)
+   1800648b6:	add    %al,(%rax)
+   1800648b8:	jb     0x18006491f
+   1800648ba:	je     0x1800648dc
+   1800648bc:	cmp    $0x30203d,%eax
+   1800648c1:	add    %al,(%rax)
+   1800648c3:	add    %al,(%rax)
+   1800648c5:	add    %al,(%rax)
+   1800648c7:	add    %dh,0x65(%rdx)
+   1800648ca:	(bad)
+   1800648cb:	and    %ah,%fs:0x72(%rbp)
+   1800648cf:	jb     0x180064940
+   1800648d1:	jb     0x18006490d
+   1800648d3:	and    %ah,0x75000073(%rip)        # 0x1f506494c
+   1800648d9:	outsb  %ds:(%rsi),(%dx)
+   1800648da:	gs js  0x18006494d
+   1800648dd:	movsxd %gs:0x64(%rbp,%riz,2),%esi
+   1800648e2:	insb   (%dx),%es:(%rdi)
+   1800648e3:	jns    0x180064905
+   1800648e5:	jb     0x18006494c
+   1800648e7:	(bad)
+   1800648e8:	movsxd 0x65(%rax),%ebp
+   1800648eb:	and    %ah,%fs:0x6e(%rbp)
+   1800648ef:	and    %ch,%fs:0x66(%rdi)
+   1800648f3:	and    %ah,0x69(%rsi)
+   1800648f6:	insb   (%dx),%es:(%rdi)
+   1800648f7:	add    %al,%gs:(%rax)
+   1800648fa:	add    %al,(%rax)
+   1800648fc:	add    %al,(%rax)
+   1800648fe:	add    %al,(%rax)
+   180064900:	ja     0x180064974
+   180064902:	imul   $0x6f727265,0x20(%rbp,%riz,2),%esi
+   18006490a:	jb     0x180064946
+   18006490c:	and    %ah,0x6f460073(%rip)        # 0x1ef4c4985
+   180064912:	jb     0x180064981
+   180064914:	(bad)
+   180064915:	je     0x180064964
+   180064917:	gs jae 0x18006498d
+   18006491a:	(bad)
+   18006491b:	and    %spl,%gs:0x61(%r14d)
+   180064921:	imul   $0x43000000,0x64(%rbp,%riz,2),%ebp
+   180064929:	jb     0x180064990
+   18006492b:	(bad)
+   18006492c:	je     0x180064993
+   18006492e:	imul   $0x69707061,0x4d(%rbp,%r12,2),%r13d
+   180064937:	outsb  %ds:(%rsi),(%dx)
+   180064938:	and    %spl,0x61(%r14d)
+   18006493d:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
+   180064945:	add    %al,(%rax)
+   180064947:	add    %cl,0x61(%rbp)
+   18006494a:	jo     0x1800649a2
+   18006494c:	imul   $0x6946664f,0x77(%rbp),%esp
+   180064953:	insb   (%dx),%es:(%rdi)
+   180064954:	and    %ah,%gs:0x61(%rsi)
+   180064958:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
+	...
+   180064968:	ja     0x1800649cb
+   18006496a:	jb     0x1800649da
+   18006496c:	imul   $0x7250203a,0x67(%rsi),%ebp
+   180064973:	gs data16 gs je 0x1800649db
+   180064978:	push   $0x74726956
+   18006497d:	jne    0x1800649e0
+   18006497f:	insb   (%dx),%es:(%rdi)
+   180064980:	rex.WRB
+   180064981:	gs insl (%dx),%es:(%rdi)
+   180064983:	outsl  %ds:(%rsi),(%dx)
+   180064984:	jb     0x1800649ff
+   180064986:	and    %ah,0x61(%rsi)
+   180064989:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
+   180064991:	or     (%rax),%al
+   180064993:	add    %al,(%rax)
+   180064995:	add    %al,(%rax)
+   180064997:	add    %dh,0x61(%rdi)
+   18006499a:	jb     0x180064a0a
+   18006499c:	imul   $0x6e55203a,0x67(%rsi),%ebp
+   1800649a3:	insl   (%dx),%es:(%rdi)
+   1800649a4:	(bad)
+   1800649a5:	jo     0x1800649fd
+   1800649a7:	imul   $0x6946664f,0x77(%rbp),%esp
+   1800649ae:	insb   (%dx),%es:(%rdi)
+   1800649af:	and    %ah,%gs:0x61(%rsi)
+   1800649b3:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
+   1800649bb:	or     (%rax),%al
+   1800649bd:	add    %al,(%rax)
+   1800649bf:	add    %ah,0x64(%rcx)
+   1800649c2:	fs jb  0x1800649e5
+   1800649c5:	cmp    $0x554e203d,%eax
+   1800649ca:	rex.WR
+   1800649cb:	rex.WR and %r12b,(%rsi)
+   1800649ce:	es and %dh,0x69(%rbx)
+   1800649d2:	jp     0x180064a39
+   1800649d4:	and    %bh,0x30203d(%rip)        # 0x180366a17
+   1800649da:	add    %al,(%rax)
+   1800649dc:	(bad)
+   1800649dd:	fs fs jb 0x1800649e1
 	...
-   180064970:	ja     0x1800649d3
-   180064972:	jb     0x1800649e2
-   180064974:	imul   $0x7250203a,0x67(%rsi),%ebp
-   18006497b:	gs data16 gs je 0x1800649e3
-   180064980:	push   $0x74726956
-   180064985:	jne    0x1800649e8
-   180064987:	insb   (%dx),%es:(%rdi)
-   180064988:	rex.WRB
-   180064989:	gs insl (%dx),%es:(%rdi)
-   18006498b:	outsl  %ds:(%rsi),(%dx)
-   18006498c:	jb     0x180064a07
-   18006498e:	and    %ah,0x61(%rsi)
-   180064991:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
-   180064999:	or     (%rax),%al
-   18006499b:	add    %al,(%rax)
-   18006499d:	add    %al,(%rax)
-   18006499f:	add    %dh,0x61(%rdi)
-   1800649a2:	jb     0x180064a12
-   1800649a4:	imul   $0x6e55203a,0x67(%rsi),%ebp
-   1800649ab:	insl   (%dx),%es:(%rdi)
-   1800649ac:	(bad)
-   1800649ad:	jo     0x180064a05
-   1800649af:	imul   $0x6946664f,0x77(%rbp),%esp
-   1800649b6:	insb   (%dx),%es:(%rdi)
-   1800649b7:	and    %ah,%gs:0x61(%rsi)
-   1800649bb:	imul   $0x7325203a,0x64(%rbp,%riz,2),%ebp
-   1800649c3:	or     (%rax),%al
-   1800649c5:	add    %al,(%rax)
-   1800649c7:	add    %ah,0x64(%rcx)
-   1800649ca:	fs jb  0x1800649ed
-   1800649cd:	cmp    $0x554e203d,%eax
-   1800649d2:	rex.WR
-   1800649d3:	rex.WR and %r12b,(%rsi)
-   1800649d6:	es and %dh,0x69(%rbx)
-   1800649da:	jp     0x180064a41
-   1800649dc:	and    %bh,0x30203d(%rip)        # 0x180366a1f
-   1800649e2:	add    %al,(%rax)
-   1800649e4:	(bad)
-   1800649e5:	fs fs jb 0x1800649e9
-   1800649e9:	add    %al,(%rax)
-   1800649eb:	add    %al,(%rax)
    1800649ed:	add    %al,(%rax)
    1800649ef:	add    %dh,0x61(%rdi)
    1800649f2:	jb     0x180064a62
    1800649f4:	imul   $0x6166203a,0x67(%rsi),%ebp
    1800649fb:	imul   $0x206f7420,0x64(%rbp,%riz,2),%ebp
    180064a03:	push   %rsi
    180064a04:	imul   $0x4c6c6175,0x74(%rdx),%esi
@@ -118354,53 +118351,50 @@
    180064c89:	jae    0x180064cb8
    180064c8b:	jb     0x180064d02
    180064c8d:	outsb  %ds:(%rsi),(%dx)
    180064c8e:	outsb  %ds:(%rsi),(%dx)
    180064c8f:	gs jb  0x180064cee
    180064c92:	(bad)
    180064c97:	sub    $0x6c697562,%eax
-   180064c9c:	fs sub $0x5c77656e,%eax
-   180064ca2:	pop    %rdi
-   180064ca3:	ja     0x180064d14
-   180064ca5:	jb     0x180064d12
-   180064ca7:	pop    %rsp
-   180064ca8:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180064caf:	insl   (%dx),%es:(%rdi)
-   180064cb0:	pop    %rsp
-   180064cb1:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   180064cb8:	insl   (%dx),%es:(%rdi)
-   180064cb9:	pop    %rsp
-   180064cba:	jae    0x180064d2e
-   180064cbc:	movsxd 0x6c(%rsp,%rbp,2),%ebx
-   180064cc0:	(bad)
-   180064cc1:	insl   (%dx),%es:(%rdi)
+   180064c9c:	fs pop %rsp
+   180064c9e:	pop    %rdi
+   180064c9f:	ja     0x180064d10
+   180064ca1:	jb     0x180064d0e
+   180064ca3:	pop    %rsp
+   180064ca4:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180064cab:	insl   (%dx),%es:(%rdi)
+   180064cac:	pop    %rsp
+   180064cad:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   180064cb4:	insl   (%dx),%es:(%rdi)
+   180064cb5:	pop    %rsp
+   180064cb6:	jae    0x180064d2a
+   180064cb8:	movsxd 0x6c(%rsp,%rbp,2),%ebx
+   180064cbc:	(bad)
+   180064cbd:	insl   (%dx),%es:(%rdi)
+   180064cbe:	(bad)
+   180064cbf:	pop    %rsp
+   180064cc0:	insb   (%dx),%es:(%rdi)
+   180064cc1:	insb   (%dx),%es:(%rdi)
    180064cc2:	(bad)
-   180064cc3:	pop    %rsp
-   180064cc4:	insb   (%dx),%es:(%rdi)
-   180064cc5:	insb   (%dx),%es:(%rdi)
-   180064cc6:	(bad)
-   180064cc7:	insl   (%dx),%es:(%rdi)
-   180064cc8:	(bad)
-   180064cc9:	cs movsxd 0x70(%rax),%esi
-   180064ccd:	add    %al,(%rax)
-   180064ccf:	add    %dh,0x62(%rdx)
-   180064cd2:	add    %al,(%rax)
-   180064cd4:	add    %al,(%rax)
-   180064cd6:	add    %al,(%rax)
-   180064cd8:	(bad)
-   180064cdd:	sub    $0x3a6d6c6c,%eax
-   180064ce2:	and    %ch,0x61(%rdi,%rbp,2)
-   180064ce6:	imul   $0x646f6d20,%fs:0x67(%rsi),%ebp
-   180064cee:	gs insb (%dx),%es:(%rdi)
-   180064cf0:	and    %ah,0x72(%rsi)
-   180064cf3:	outsl  %ds:(%rsi),(%dx)
-   180064cf4:	insl   (%dx),%es:(%rdi)
-   180064cf5:	and    %ah,0xa73(%rip)        # 0x18006576e
-   180064cfb:	add    %al,(%rax)
-   180064cfd:	add    %al,(%rax)
+   180064cc3:	insl   (%dx),%es:(%rdi)
+   180064cc4:	(bad)
+   180064cc5:	cs movsxd 0x70(%rax),%esi
+   180064cc9:	add    %al,(%rax)
+   180064ccb:	add    %dh,0x62(%rdx)
+   180064cce:	add    %al,(%rax)
+   180064cd0:	(bad)
+   180064cd5:	sub    $0x3a6d6c6c,%eax
+   180064cda:	and    %ch,0x61(%rdi,%rbp,2)
+   180064cde:	imul   $0x646f6d20,%fs:0x67(%rsi),%ebp
+   180064ce6:	gs insb (%dx),%es:(%rdi)
+   180064ce8:	and    %ah,0x72(%rsi)
+   180064ceb:	outsl  %ds:(%rsi),(%dx)
+   180064cec:	insl   (%dx),%es:(%rdi)
+   180064ced:	and    %ah,0xa73(%rip)        # 0x180065766
+	...
    180064cff:	add    %dh,0x6e(%rbp)
    180064d02:	imul   $0x77,0x6f(%rsi),%ebp
    180064d06:	outsb  %ds:(%rsi),(%dx)
    180064d07:	and    %ch,(%rax)
    180064d09:	insl   (%dx),%es:(%rdi)
    180064d0a:	(bad)
    180064d0b:	imul   $0x72657620,0x2c(%ebx),%esp
@@ -124868,30 +124862,32 @@
    180069089:	jae    0x1800690b8
    18006908b:	jb     0x180069102
    18006908d:	outsb  %ds:(%rsi),(%dx)
    18006908e:	outsb  %ds:(%rsi),(%dx)
    18006908f:	gs jb  0x1800690ee
    180069092:	(bad)
    180069097:	sub    $0x6c697562,%eax
-   18006909c:	fs sub $0x5c77656e,%eax
-   1800690a2:	pop    %rdi
-   1800690a3:	ja     0x180069114
-   1800690a5:	jb     0x180069112
-   1800690a7:	pop    %rsp
-   1800690a8:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   1800690af:	insl   (%dx),%es:(%rdi)
-   1800690b0:	pop    %rsp
-   1800690b1:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   1800690b8:	insl   (%dx),%es:(%rdi)
-   1800690b9:	pop    %rsp
-   1800690ba:	jae    0x18006912e
-   1800690bc:	movsxd 0x67(%rdi,%riz,2),%ebx
-   1800690c0:	insl   (%dx),%es:(%rdi)
-   1800690c1:	insb   (%dx),%es:(%rdi)
-   1800690c2:	cs movsxd (%rax),%eax
+   18006909c:	fs pop %rsp
+   18006909e:	pop    %rdi
+   18006909f:	ja     0x180069110
+   1800690a1:	jb     0x18006910e
+   1800690a3:	pop    %rsp
+   1800690a4:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   1800690ab:	insl   (%dx),%es:(%rdi)
+   1800690ac:	pop    %rsp
+   1800690ad:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   1800690b4:	insl   (%dx),%es:(%rdi)
+   1800690b5:	pop    %rsp
+   1800690b6:	jae    0x18006912a
+   1800690b8:	movsxd 0x67(%rdi,%riz,2),%ebx
+   1800690bc:	insl   (%dx),%es:(%rdi)
+   1800690bd:	insb   (%dx),%es:(%rdi)
+   1800690be:	cs movsxd (%rax),%eax
+   1800690c1:	add    %al,(%rax)
+   1800690c3:	add    %al,(%rax)
    1800690c5:	add    %al,(%rax)
    1800690c7:	add    %al,0x47(%rdi)
    1800690ca:	rex.WRB
    1800690cb:	rex.WR pop %rdi
    1800690cd:	push   %r11
    1800690cf:	push   %rbx
    1800690d0:	rex.RB push %r10
@@ -128093,15 +128089,16 @@
    18006b134:	add    %eax,(%rax)
    18006b136:	add    %al,(%rax)
    18006b138:	rolb   $1,0x6(%rsi)
    18006b13b:	addb   $0x0,(%rcx)
    18006b13e:	add    %al,(%rax)
    18006b140:	add    %al,(%rax)
    18006b142:	add    %al,(%rax)
-   18006b144:	enter  $0x4568,$0x66
+   18006b144:	(bad)
+   18006b145:	and    %al,0x66(%rsi)
    18006b148:	add    %al,(%rax)
    18006b14a:	add    %al,(%rax)
    18006b14c:	or     $0x50000000,%eax
    18006b151:	add    (%rax),%eax
    18006b153:	add    %al,-0x7ffff943(%rax)
    18006b159:	test   $0x6,%eax
 	...
```

## ipex_llm/libs/libllama_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005c0a8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu May 16 02:19:00 2024
+Time/Date		Thu May 16 15:03:26 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c800
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005c0a8
@@ -122578,15 +122578,17 @@
    1800651e0:	enter  $0x5e6,$0x80
    1800651e4:	add    %eax,(%rax)
    1800651e6:	add    %al,(%rax)
    1800651e8:	shl    $1,%dh
    1800651ea:	add    $0x180,%eax
    1800651ef:	add    %al,(%rax)
    1800651f1:	add    %al,(%rax)
-   1800651f3:	add    %dl,0x6645(,%rbp,2)
+   1800651f3:	add    %bh,(%rsi)
+   1800651f5:	and    %al,0x66(%rsi)
+   1800651f8:	add    %al,(%rax)
    1800651fa:	add    %al,(%rax)
    1800651fc:	or     $0x50000000,%eax
    180065201:	add    (%rax),%eax
    180065203:	add    %al,-0x7ffff9a2(%rax)
    180065209:	rex.WX (bad)
 	...
    18006527f:	add    %dh,%al
```

## ipex_llm/libs/libstarcoder_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180069508
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu May 16 02:00:40 2024
+Time/Date		Thu May 16 15:02:30 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000069c00
 SizeOfInitializedData	00000000000c8600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000069508
@@ -132477,30 +132477,32 @@
    18006ee19:	jae    0x18006ee48
    18006ee1b:	jb     0x18006ee92
    18006ee1d:	outsb  %ds:(%rsi),(%dx)
    18006ee1e:	outsb  %ds:(%rsi),(%dx)
    18006ee1f:	gs jb  0x18006ee7e
    18006ee22:	(bad)
    18006ee27:	sub    $0x6c697562,%eax
-   18006ee2c:	fs sub $0x5c77656e,%eax
-   18006ee32:	pop    %rdi
-   18006ee33:	ja     0x18006eea4
-   18006ee35:	jb     0x18006eea2
-   18006ee37:	pop    %rsp
-   18006ee38:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18006ee3f:	insl   (%dx),%es:(%rdi)
-   18006ee40:	pop    %rsp
-   18006ee41:	imul   $0x6c6c2d78,0x65(%rax),%esi
-   18006ee48:	insl   (%dx),%es:(%rdi)
-   18006ee49:	pop    %rsp
-   18006ee4a:	jae    0x18006eebe
-   18006ee4c:	movsxd 0x67(%rdi,%riz,2),%ebx
-   18006ee50:	insl   (%dx),%es:(%rdi)
-   18006ee51:	insb   (%dx),%es:(%rdi)
-   18006ee52:	cs movsxd (%rax),%eax
+   18006ee2c:	fs pop %rsp
+   18006ee2e:	pop    %rdi
+   18006ee2f:	ja     0x18006eea0
+   18006ee31:	jb     0x18006ee9e
+   18006ee33:	pop    %rsp
+   18006ee34:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18006ee3b:	insl   (%dx),%es:(%rdi)
+   18006ee3c:	pop    %rsp
+   18006ee3d:	imul   $0x6c6c2d78,0x65(%rax),%esi
+   18006ee44:	insl   (%dx),%es:(%rdi)
+   18006ee45:	pop    %rsp
+   18006ee46:	jae    0x18006eeba
+   18006ee48:	movsxd 0x67(%rdi,%riz,2),%ebx
+   18006ee4c:	insl   (%dx),%es:(%rdi)
+   18006ee4d:	insb   (%dx),%es:(%rdi)
+   18006ee4e:	cs movsxd (%rax),%eax
+   18006ee51:	add    %al,(%rax)
+   18006ee53:	add    %al,(%rax)
    18006ee55:	add    %al,(%rax)
    18006ee57:	add    %al,0x47(%rdi)
    18006ee5a:	rex.WRB
    18006ee5b:	rex.WR pop %rdi
    18006ee5d:	push   %r11
    18006ee5f:	push   %rbx
    18006ee60:	rex.RB push %r10
@@ -138528,15 +138530,16 @@
    180072c85:	add    %al,(%rax)
    180072c87:	add    %al,%al
    180072c89:	mov    $0x6,%dh
    180072c8b:	addb   $0x0,(%rcx)
    180072c8e:	add    %al,(%rax)
    180072c90:	add    %al,(%rax)
    180072c92:	add    %al,(%rax)
-   180072c94:	enter  $0x4568,$0x66
+   180072c94:	(bad)
+   180072c95:	and    %al,0x66(%rsi)
    180072c98:	add    %al,(%rax)
    180072c9a:	add    %al,(%rax)
    180072c9c:	or     $0x50000000,%eax
    180072ca1:	add    (%rax),%eax
    180072ca3:	add    %dl,0x3e(%rax)
    180072ca6:	(bad)
    180072ca7:	add    %dl,0x2e(%rax)
```

## ipex_llm/libs/libstarcoder_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180063598
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu May 16 02:18:59 2024
+Time/Date		Thu May 16 15:03:26 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063c00
 SizeOfInitializedData	00000000000c8000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000063598
@@ -133189,16 +133189,16 @@
    18006cd57:	add    %al,%al
    18006cd59:	push   %rsi
    18006cd5a:	(bad)
    18006cd5b:	addb   $0x0,(%rcx)
    18006cd5e:	add    %al,(%rax)
    18006cd60:	add    %al,(%rax)
    18006cd62:	add    %al,(%rax)
-   18006cd64:	adc    0x45(%rbp),%ebp
-   18006cd67:	data16 add %al,(%rax)
+   18006cd64:	ds and %al,0x66(%rsi)
+   18006cd68:	add    %al,(%rax)
    18006cd6a:	add    %al,(%rax)
    18006cd6c:	or     $0x50000000,%eax
    18006cd71:	add    (%rax),%eax
    18006cd73:	add    %dl,%al
    18006cd75:	fiadds (%rsi)
    18006cd77:	add    %dl,%al
    18006cd79:	(bad)
```

## ipex_llm/libs/llama-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002dac
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu May 16 02:17:44 2024
+Time/Date		Thu May 16 15:02:31 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002800
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002dac
@@ -5355,15 +5355,16 @@
    180004a20:	cmp    %al,0x0(%rdx)
    180004a23:	addb   $0x0,(%rcx)
    180004a26:	add    %al,(%rax)
    180004a28:	rex
    180004a29:	rex.X add %al,0x1(%rax)
    180004a30:	add    %al,(%rax)
    180004a32:	add    %al,(%rax)
-   180004a34:	enter  $0x456c,$0x66
+   180004a34:	(bad)
+   180004a35:	and    %al,0x66(%rsi)
    180004a38:	add    %al,(%rax)
    180004a3a:	add    %al,(%rax)
    180004a3c:	or     $0xe0000000,%eax
    180004a41:	add    (%rax),%al
    180004a43:	add    %ah,%ah
    180004a45:	rex.WR add %r8b,(%rax)
    180004a48:	in     $0x38,%al
```

## ipex_llm/libs/llama.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005be98
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu May 16 02:17:44 2024
+Time/Date		Thu May 16 15:02:33 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c600
 SizeOfInitializedData	00000000000c6200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005be98
@@ -122483,18 +122483,17 @@
    180065200:	enter  $0x5e6,$0x80
    180065204:	add    %eax,(%rax)
    180065206:	add    %al,(%rax)
    180065208:	shl    $1,%dh
    18006520a:	add    $0x180,%eax
    18006520f:	add    %al,(%rax)
    180065211:	add    %al,(%rax)
-   180065213:	add    %cl,%al
-   180065215:	insb   (%dx),%es:(%rdi)
-   180065216:	rex.RB
-   180065217:	data16 add %al,(%rax)
+   180065213:	add    %cl,(%rcx)
+   180065215:	and    %al,0x66(%rsi)
+   180065218:	add    %al,(%rax)
    18006521a:	add    %al,(%rax)
    18006521c:	or     $0x50000000,%eax
    180065221:	add    (%rax),%eax
    180065223:	add    %al,-0x7ffff9a2(%rax)
    180065229:	rex.W (bad)
 	...
    18006527f:	add    %dh,%al
```

## ipex_llm/libs/main-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001045c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu May 16 02:17:44 2024
+Time/Date		Thu May 16 15:02:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010800
 SizeOfInitializedData	0000000000008e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001045c
@@ -25509,16 +25509,17 @@
    140014ab0:	enter  $0x125,$0x40
    140014ab4:	add    %eax,(%rax)
    140014ab6:	add    %al,(%rax)
    140014ab8:	shlb   $1,0x14001(%rip)        # 0x140028abf
    140014abe:	add    %al,(%rax)
    140014ac0:	add    %al,(%rax)
    140014ac2:	add    %al,(%rax)
-   140014ac4:	enter  $0x456c,$0x66
-   140014ac8:	add    %al,(%rax)
+   140014ac4:	or     %ah,(%rax)
+   140014ac6:	rex.RX
+   140014ac7:	data16 add %al,(%rax)
    140014aca:	add    %al,(%rax)
    140014acc:	or     $0x20000000,%eax
    140014ad1:	add    (%rax),%eax
    140014ad3:	add    %cl,%ah
    140014ad5:	push   %rsp
    140014ad6:	add    %eax,(%rax)
    140014ad8:	int3
```

## ipex_llm/libs/main-chatglm_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400836cc
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu May 16 02:19:40 2024
+Time/Date		Thu May 16 15:03:54 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000087c00
 SizeOfInitializedData	00000000000cbe00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000836cc
@@ -189048,15 +189048,17 @@
    140093f25:	add    %al,(%rax)
    140093f27:	add    %al,(%rax)
    140093f29:	cltd
    140093f2a:	or     %al,0x1(%rax)
    140093f2d:	add    %al,(%rax)
    140093f2f:	add    %al,(%rax)
    140093f31:	add    %al,(%rax)
-   140093f33:	add    %bh,0x6645(,%rbp,2)
+   140093f33:	add    %bl,0x20(%rdx)
+   140093f36:	rex.RX
+   140093f37:	data16 add %al,(%rax)
    140093f3a:	add    %al,(%rax)
    140093f3c:	or     $0xcc000000,%eax
    140093f41:	add    (%rax),%eax
    140093f43:	add    %dl,-0x6ffff68d(%rax)
    140093f49:	movsxd (%rcx),%ecx
 	...
    140093f7f:	add    %al,0x1400977(%rax)
```

## ipex_llm/libs/main-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000ef6c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu May 16 02:17:43 2024
+Time/Date		Thu May 16 15:02:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f200
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000ef6c
@@ -24136,17 +24136,16 @@
    140013edf:	add    %ch,%al
    140013ee1:	adc    $0x14001,%eax
    140013ee6:	add    %al,(%rax)
    140013ee8:	lock adc $0x14001,%eax
    140013eee:	add    %al,(%rax)
    140013ef0:	add    %al,(%rax)
    140013ef2:	add    %al,(%rax)
-   140013ef4:	(bad)
-   140013ef5:	insb   (%dx),%es:(%rdi)
-   140013ef6:	rex.RB
+   140013ef4:	or     %ah,(%rax)
+   140013ef6:	rex.RX
    140013ef7:	data16 add %al,(%rax)
    140013efa:	add    %al,(%rax)
    140013efc:	or     $0x90000000,%eax
    140013f01:	add    (%rax),%eax
    140013f03:	add    %ch,0x1(%rcx,%rcx,2)
    140013f07:	add    %ch,0x1(%rdi,%rbp,1)
 	...
```

## ipex_llm/libs/main-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000f32c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu May 16 02:17:43 2024
+Time/Date		Thu May 16 15:02:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f600
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000f32c
@@ -24679,17 +24679,16 @@
    140013faf:	add    %ch,%al
    140013fb1:	adc    $0x14001,%eax
    140013fb6:	add    %al,(%rax)
    140013fb8:	lock adc $0x14001,%eax
    140013fbe:	add    %al,(%rax)
    140013fc0:	add    %al,(%rax)
    140013fc2:	add    %al,(%rax)
-   140013fc4:	(bad)
-   140013fc5:	insb   (%dx),%es:(%rdi)
-   140013fc6:	rex.RB
+   140013fc4:	or     %ah,(%rax)
+   140013fc6:	rex.RX
    140013fc7:	data16 add %al,(%rax)
    140013fca:	add    %al,(%rax)
    140013fcc:	or     $0x90000000,%eax
    140013fd1:	add    (%rax),%eax
    140013fd3:	add    %ch,%ah
    140013fd5:	add    %rax,(%r8)
    140013fd8:	in     (%dx),%al
```

## ipex_llm/libs/main-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001a85c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu May 16 02:17:44 2024
+Time/Date		Thu May 16 15:02:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000001b000
 SizeOfInitializedData	000000000000bc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001a85c
@@ -40341,18 +40341,17 @@
    14001f111:	movb   $0x40,(%rcx)
    14001f114:	add    %eax,(%rax)
    14001f116:	add    %al,(%rax)
    14001f118:	push   $0x14001c6
    14001f11d:	add    %al,(%rax)
    14001f11f:	add    %al,(%rax)
    14001f121:	add    %al,(%rax)
-   14001f123:	add    %cl,%al
-   14001f125:	insb   (%dx),%es:(%rdi)
-   14001f126:	rex.RB
-   14001f127:	data16 add %al,(%rax)
+   14001f123:	add    %cl,(%rax)
+   14001f125:	and    %al,0x66(%rsi)
+   14001f128:	add    %al,(%rax)
    14001f12a:	add    %al,(%rax)
    14001f12c:	or     $0x20000000,%eax
    14001f131:	add    (%rax),%eax
    14001f133:	add    %dl,(%rbx,%rax,1)
    14001f136:	add    (%rax),%al
    14001f138:	adc    $0xf7,%al
    14001f13a:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013918
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu May 16 02:17:44 2024
+Time/Date		Thu May 16 15:02:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013a00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013918
@@ -32232,18 +32232,17 @@
    140019225:	add    %al,(%rax)
    140019227:	add    %al,(%rax)
    140019229:	push   %rbp
    14001922a:	add    %eax,0x1(%rax)
    14001922d:	add    %al,(%rax)
    14001922f:	add    %al,(%rax)
    140019231:	add    %al,(%rax)
-   140019233:	add    %cl,%al
-   140019235:	insb   (%dx),%es:(%rdi)
-   140019236:	rex.RB
-   140019237:	data16 add %al,(%rax)
+   140019233:	add    %cl,(%rax)
+   140019235:	and    %al,0x66(%rsi)
+   140019238:	add    %al,(%rax)
    14001923a:	add    %al,(%rax)
    14001923c:	or     $0x20000000,%eax
    140019241:	add    (%rax),%eax
    140019243:	add    %dh,%al
    140019245:	movabs 0x18ff00001,%eax
 	...
    14001927e:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-bloom_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013b28
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu May 16 02:18:59 2024
+Time/Date		Thu May 16 15:03:26 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ad000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013b28
@@ -32374,18 +32374,17 @@
    140019205:	add    %al,(%rax)
    140019207:	add    %al,(%rax)
    140019209:	push   %rbp
    14001920a:	add    %eax,0x1(%rax)
    14001920d:	add    %al,(%rax)
    14001920f:	add    %al,(%rax)
    140019211:	add    %al,(%rax)
-   140019213:	add    %dl,(%rbx)
-   140019215:	insl   (%dx),%es:(%rdi)
-   140019216:	rex.RB
-   140019217:	data16 add %al,(%rax)
+   140019213:	add    %bh,(%rsi)
+   140019215:	and    %al,0x66(%rsi)
+   140019218:	add    %al,(%rax)
    14001921a:	add    %al,(%rax)
    14001921c:	or     $0x20000000,%eax
    140019221:	add    (%rax),%eax
    140019223:	add    %dh,%al
    140019225:	movabs 0x191f00001,%eax
 	...
    14001927e:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010988
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu May 16 02:17:42 2024
+Time/Date		Thu May 16 15:02:31 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010a00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010988
@@ -27175,18 +27175,17 @@
    140016020:	push   $0x1400123
    140016025:	add    %al,(%rax)
    140016027:	add    %dh,0x23(%rax)
    14001602a:	add    %eax,0x1(%rax)
    14001602d:	add    %al,(%rax)
    14001602f:	add    %al,(%rax)
    140016031:	add    %al,(%rax)
-   140016033:	add    %al,%dh
-   140016035:	insb   (%dx),%es:(%rdi)
-   140016036:	rex.RB
-   140016037:	data16 add %al,(%rax)
+   140016033:	add    %al,(%rdi)
+   140016035:	and    %al,0x66(%rsi)
+   140016038:	add    %al,(%rax)
    14001603a:	add    %al,(%rax)
    14001603c:	or     $0x90000000,%eax
    140016041:	add    (%rax),%eax
    140016043:	add    %ch,%al
    140016045:	add    %eax,%gs:(%rax)
    140016048:	call   0x1400161a0
 	...
```

## ipex_llm/libs/quantize-gptneox_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010b98
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu May 16 02:18:59 2024
+Time/Date		Thu May 16 15:03:25 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010c00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010b98
@@ -27317,20 +27317,17 @@
    140016000:	push   $0x1400123
    140016005:	add    %al,(%rax)
    140016007:	add    %dh,0x23(%rax)
    14001600a:	add    %eax,0x1(%rax)
    14001600d:	add    %al,(%rax)
    14001600f:	add    %al,(%rax)
    140016011:	add    %al,(%rax)
-   140016013:	add    %dl,(%rbx)
-   140016015:	insl   (%dx),%es:(%rdi)
-   140016016:	rex.RB
-   140016017:	data16 add %al,(%rax)
-   14001601a:	add    %al,(%rax)
-   14001601c:	or     $0x90000000,%eax
+   140016013:	add    %bh,0x664620(%rip)        # 0x14067a639
+   140016019:	add    %al,(%rax)
+   14001601b:	add    %cl,-0x70000000(%rip)        # 0xd0016021
    140016021:	add    (%rax),%eax
    140016023:	add    %ch,%al
    140016025:	add    %eax,%gs:(%rax)
    140016028:	call   0x140016182
 	...
    14001607d:	add    %al,(%rax)
    14001607f:	add    %bl,0x1400169(%rax)
```

## ipex_llm/libs/quantize-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400118e8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu May 16 02:17:42 2024
+Time/Date		Thu May 16 15:02:31 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011800
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000118e8
@@ -28461,18 +28461,17 @@
    1400170ed:	add    %al,(%rax)
    1400170ef:	add    %cl,0x1400133(%rax)
    1400170f5:	add    %al,(%rax)
    1400170f7:	add    %dl,0x1400133(%rax)
    1400170fd:	add    %al,(%rax)
    1400170ff:	add    %al,(%rax)
    140017101:	add    %al,(%rax)
-   140017103:	add    %al,%dh
-   140017105:	insb   (%dx),%es:(%rdi)
-   140017106:	rex.RB
-   140017107:	data16 add %al,(%rax)
+   140017103:	add    %al,(%rdi)
+   140017105:	and    %al,0x66(%rsi)
+   140017108:	add    %al,(%rax)
    14001710a:	add    %al,(%rax)
    14001710c:	or     $0x90000000,%eax
    140017111:	add    (%rax),%eax
    140017113:	add    %ch,%ah
    140017115:	jbe    0x140017118
    140017117:	add    %ch,%ah
    140017119:	(bad)
```

## ipex_llm/libs/quantize-llama_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140011af8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu May 16 02:18:59 2024
+Time/Date		Thu May 16 15:03:25 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011c00
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000011af8
@@ -28608,20 +28608,17 @@
    1400170cd:	add    %al,(%rax)
    1400170cf:	add    %cl,0x1400133(%rax)
    1400170d5:	add    %al,(%rax)
    1400170d7:	add    %dl,0x1400133(%rax)
    1400170dd:	add    %al,(%rax)
    1400170df:	add    %al,(%rax)
    1400170e1:	add    %al,(%rax)
-   1400170e3:	add    %dl,(%rbx)
-   1400170e5:	insl   (%dx),%es:(%rdi)
-   1400170e6:	rex.RB
-   1400170e7:	data16 add %al,(%rax)
-   1400170ea:	add    %al,(%rax)
-   1400170ec:	or     $0x90000000,%eax
+   1400170e3:	add    %bh,0x664620(%rip)        # 0x14067b709
+   1400170e9:	add    %al,(%rax)
+   1400170eb:	add    %cl,-0x70000000(%rip)        # 0xd00170f1
    1400170f1:	add    (%rax),%eax
    1400170f3:	add    %ch,0x1(%rsi,%rsi,2)
    1400170f7:	add    %ch,0x1(%rsi,%riz,2)
    1400170fb:	add    %al,(%rax)
    1400170fd:	add    %al,(%rax)
    1400170ff:	add    %ah,(%rax)
    140017101:	jp     0x140017104
```

## ipex_llm/libs/quantize-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013c70
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu May 16 02:17:43 2024
+Time/Date		Thu May 16 15:02:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013c70
@@ -32577,18 +32577,17 @@
    140019325:	add    %al,(%rax)
    140019327:	add    %al,(%rax)
    140019329:	push   %rbp
    14001932a:	add    %eax,0x1(%rax)
    14001932d:	add    %al,(%rax)
    14001932f:	add    %al,(%rax)
    140019331:	add    %al,(%rax)
-   140019333:	add    %al,%bh
-   140019335:	insb   (%dx),%es:(%rdi)
-   140019336:	rex.RB
-   140019337:	data16 add %al,(%rax)
+   140019333:	add    %cl,(%rax)
+   140019335:	and    %al,0x66(%rsi)
+   140019338:	add    %al,(%rax)
    14001933a:	add    %al,(%rax)
    14001933c:	or     $0x20000000,%eax
    140019341:	add    (%rax),%eax
    140019343:	add    %bh,%ah
    140019345:	movabs %al,0x192fc0001
 	...
    14001937e:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-starcoder_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013e80
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu May 16 02:18:59 2024
+Time/Date		Thu May 16 15:03:26 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013e00
 SizeOfInitializedData	00000000000ad200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013e80
@@ -32704,18 +32704,17 @@
    140019305:	add    %al,(%rax)
    140019307:	add    %al,(%rax)
    140019309:	push   %rbp
    14001930a:	add    %eax,0x1(%rax)
    14001930d:	add    %al,(%rax)
    14001930f:	add    %al,(%rax)
    140019311:	add    %al,(%rax)
-   140019313:	add    %dl,(%rbx)
-   140019315:	insl   (%dx),%es:(%rdi)
-   140019316:	rex.RB
-   140019317:	data16 add %al,(%rax)
+   140019313:	add    %bh,(%rsi)
+   140019315:	and    %al,0x66(%rsi)
+   140019318:	add    %al,(%rax)
    14001931a:	add    %al,(%rax)
    14001931c:	or     $0x20000000,%eax
    140019321:	add    (%rax),%eax
    140019323:	add    %bh,%ah
    140019325:	movabs %al,0x194fc0001
 	...
    14001937e:	add    %al,(%rax)
```

## ipex_llm/libs/starcoder-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018000277c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu May 16 02:17:44 2024
+Time/Date		Thu May 16 15:02:31 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002200
 SizeOfInitializedData	0000000000003400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000277c
@@ -4028,15 +4028,16 @@
    1800045f0:	cmp    %al,0x0(%rdx)
    1800045f3:	addb   $0x0,(%rcx)
    1800045f6:	add    %al,(%rax)
    1800045f8:	rex
    1800045f9:	rex.X add %al,0x1(%rax)
    180004600:	add    %al,(%rax)
    180004602:	add    %al,(%rax)
-   180004604:	enter  $0x456c,$0x66
+   180004604:	(bad)
+   180004605:	and    %al,0x66(%rsi)
    180004608:	add    %al,(%rax)
    18000460a:	add    %al,(%rax)
    18000460c:	or     $0xe0000000,%eax
    180004611:	add    (%rax),%al
    180004613:	add    %ah,%ah
    180004615:	rex.W add %al,(%rax)
    180004618:	in     $0x2e,%al
```

## ipex_llm/libs/starcoder.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180063388
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu May 16 02:17:44 2024
+Time/Date		Thu May 16 15:02:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063a00
 SizeOfInitializedData	00000000000c8000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000063388
@@ -133093,16 +133093,17 @@
    18006cd77:	add    %al,%al
    18006cd79:	push   %rsi
    18006cd7a:	(bad)
    18006cd7b:	addb   $0x0,(%rcx)
    18006cd7e:	add    %al,(%rax)
    18006cd80:	add    %al,(%rax)
    18006cd82:	add    %al,(%rax)
-   18006cd84:	enter  $0x456c,$0x66
-   18006cd88:	add    %al,(%rax)
+   18006cd84:	or     %ah,(%rax)
+   18006cd86:	rex.RX
+   18006cd87:	data16 add %al,(%rax)
    18006cd8a:	add    %al,(%rax)
    18006cd8c:	or     $0x50000000,%eax
    18006cd91:	add    (%rax),%eax
    18006cd93:	add    %dl,-0x21(%rax)
    18006cd96:	(bad)
    18006cd97:	add    %dl,-0x33(%rax)
    18006cd9a:	(bad)
```

## ipex_llm/transformers/convert.py

```diff
@@ -702,14 +702,16 @@
     if model.config.model_type == "starcoder2":
         from ipex_llm.transformers.models.starcoder2 import merge_qkv
         model.apply(merge_qkv)
     if model.config.model_type == "phi":
         from ipex_llm.transformers.models.phi import merge_qkv
         model.apply(merge_qkv)
     if model.config.model_type == "phi3":
+        from ipex_llm.transformers.models.phi3 import pre_compute_inv_freq
+        model.apply(pre_compute_inv_freq)
         from ipex_llm.transformers.models.phi3 import split_mlp
         model.apply(split_mlp)
     if model.config.model_type == "qwen":
         rope_base = model.config.rotary_emb_base
         from accelerate.big_modeling import init_empty_weights
 
         def split_qkv_proj_func(module):
@@ -958,23 +960,26 @@
                         llama_mlp_forward)
         convert_forward(model,
                         transformers.models.llama.modeling_llama.LlamaDecoderLayer,
                         llama_decoder_forward)
         if version.parse(trans_version) >= version.parse("4.36.0"):
             # transformers version >= 4.36.0
             from ipex_llm.transformers.models.llama import llama_attention_forward_4_38
-            from ipex_llm.transformers.models.llama import llama_model_forward_4_36
             if version.parse(trans_version) >= version.parse("4.38.0"):
-                from ipex_llm.transformers.models.llama import llama_attention_forward_4_38_original
-                # Todo: support llama_model_forward with transformers version >= 4.38.0
+                from ipex_llm.transformers.models.llama import llama_model_forward_4_38
+                convert_forward(
+                    model,
+                    transformers.models.llama.modeling_llama.LlamaModel,
+                    llama_model_forward_4_38)
                 convert_forward(
                     model,
                     transformers.models.llama.modeling_llama.LlamaAttention,
-                    llama_attention_forward_4_38_original)
+                    llama_attention_forward_4_38)
             else:
+                from ipex_llm.transformers.models.llama import llama_model_forward_4_36
                 convert_forward(
                     model,
                     transformers.models.llama.modeling_llama.LlamaModel,
                     llama_model_forward_4_36)
                 convert_forward(
                     model,
                     transformers.models.llama.modeling_llama.LlamaAttention,
@@ -1521,30 +1526,23 @@
         from ipex_llm.transformers.models.phi import model_forward
         convert_forward(model, module.PhiAttention, attention_forward)
         convert_forward(model, module.PhiModel, model_forward)
     elif model.config.model_type == "phi3":
         # for phi-3
         modeling_module_name = model.__class__.__module__
         module = importlib.import_module(modeling_module_name)
-        from ipex_llm.transformers.models.phi3 import su_scaled_rope_forward
-        convert_forward(model, module.Phi3SuScaledRotaryEmbedding, su_scaled_rope_forward)
         from ipex_llm.transformers.models.phi3 import attention_forward
         convert_forward(model, module.Phi3Attention, attention_forward)
         from ipex_llm.transformers.models.phi3 import mlp_forward
         convert_forward(model, module.Phi3MLP, mlp_forward)
         from ipex_llm.transformers.models.phi3 import model_forward_wrapper
         model_forward = model_forward_wrapper(module.Phi3Model.forward)
         convert_forward(model, module.Phi3Model, model_forward)
-        from ipex_llm.transformers.models.phi3 import Phi3RotaryEmbeddingCached
-        replace_RotaryEmbed(model, module.Phi3RotaryEmbedding, Phi3RotaryEmbeddingCached)
         from ipex_llm.transformers.models.phi3 import phi3_rms_norm_forward
-        convert_forward(
-            model,
-            module.Phi3RMSNorm,
-            phi3_rms_norm_forward)
+        convert_forward(model, module.Phi3RMSNorm, phi3_rms_norm_forward)
     elif model.config.model_type == 'yuan':
         modeling_module_name = model.__class__.__module__
         module = importlib.import_module(modeling_module_name)
         from ipex_llm.transformers.models.yuan import yuan_attention_forward
         # from ipex_llm.transformers.models.yuan import yuan_mlp_forward
         convert_forward(model,
                         module.YuanAttention,
```

## ipex_llm/transformers/models/baichuan2.py

```diff
@@ -24,18 +24,19 @@
 import torch.utils.checkpoint
 from torch.nn import functional as F
 from ipex_llm.ggml.quantize import ggml_tensor_qtype
 from ipex_llm.transformers.models.utils import init_fp8_kv_cache, append_fp8_kv_cache, \
     restore_fp8_kv_cache, use_quantize_kv_cache
 from ipex_llm.transformers.models.utils import init_kv_cache, extend_kv_cache, \
     append_kv_cache, is_enough_kv_cache_room_4_31
-from ipex_llm.transformers.models.utils import use_flash_attention, use_esimd_sdp
+from ipex_llm.transformers.models.utils import use_flash_attention, use_sdp
 from ipex_llm.transformers.models.utils import apply_rotary_pos_emb, SILU
 from ipex_llm.transformers.models.utils import apply_rotary_pos_emb_no_cache_xpu
 from ipex_llm.transformers.models.utils import mlp_fusion_check
+from ipex_llm.utils.common.log4Error import invalidInputError
 from transformers.utils import logging
 logger = logging.get_logger(__name__)
 
 try:
     from xformers import ops as xops
 except ImportError:
     xops = None
@@ -162,17 +163,16 @@
     else:
         k_cache, v_cache = past_key_value
     key_states, value_states = append_fp8_kv_cache(k_cache, v_cache,
                                                    key_states, value_states)
 
     past_key_value = (key_states, value_states) if use_cache else None
 
-    if attention_mask is not None:
-        if attention_mask.dtype == torch.bool:
-            attention_mask.masked_fill_(attention_mask.logical_not(), float("-inf"))
+    invalidInputError(attention_mask is None or attention_mask.dtype != torch.bool,
+                      "attention_mask's dtype cannot be bool")
 
     scaling_factor = 1 / math.sqrt(query_states.size(-1))
     if query_states.size(2) != 1 or device.type != 'xpu':
         key_states, value_states = restore_fp8_kv_cache(key_states, value_states,
                                                         query_states.dtype)
         if should_split_qkv_tensor(query_states, bsz, self.num_heads,
                                    q_len, kv_seq_len, output_attentions):
@@ -275,14 +275,17 @@
         new_key_states[:] = key_states
         new_value_states[:] = value_states
         key_states = new_key_states
         value_states = new_value_states
 
     past_key_value = (key_states, value_states) if use_cache else None
 
+    invalidInputError(attention_mask is None or attention_mask.dtype != torch.bool,
+                      "attention_mask's dtype cannot be bool")
+
     if xops is not None and self.training:
         attn_weights = None
         query_states = query_states.transpose(1, 2)
         key_states = key_states.transpose(1, 2)
         value_states = value_states.transpose(1, 2)
         attn_output = xops.memory_efficient_attention(
             query_states, key_states, value_states, attn_bias=xops.LowerTriangularMask()
@@ -292,25 +295,20 @@
                 use_flash_attention(query_states, key_states, attention_mask):
             attn_output = F.scaled_dot_product_attention(query_states.to(dtype=torch.float16),
                                                          key_states.to(dtype=torch.float16),
                                                          value_states.to(dtype=torch.float16),
                                                          is_causal=True)
             attn_weights = None
         elif not self.training and not hidden_states.requires_grad and \
-                use_esimd_sdp(q_len, key_states.shape[2], self.head_dim, query_states):
-            import linear_fp16_esimd
-            attn_output = linear_fp16_esimd.sdp_forward(query_states,
-                                                        key_states,
-                                                        value_states)
+                use_sdp(q_len, key_states.shape[2], self.head_dim, query_states):
+            import linear_q4_0
+            attn_output = linear_q4_0.sdp(query_states, key_states, value_states, attention_mask)
             attn_output = attn_output.view(query_states.shape)
             attn_weights = None
         else:
-            if attention_mask is not None:
-                if attention_mask.dtype == torch.bool:
-                    attention_mask.masked_fill_(attention_mask.logical_not(), float("-inf"))
             if should_split_qkv_tensor(query_states, bsz, self.num_heads,
                                        q_len, kv_seq_len, output_attentions):
                 attn_output, attn_weights = native_sdp_split_qkv_tensor(query_states,
                                                                         key_states,
                                                                         value_states,
                                                                         attention_mask)
             else:
```

## ipex_llm/transformers/models/chatglm.py

```diff
@@ -100,15 +100,15 @@
 
     if use_cache:
         present = (key_layer.permute(2, 0, 1, 3), value_layer.permute(2, 0, 1, 3))
     else:
         present = None
 
     pytorch_major_version = int(torch.__version__.split('.')[0])
-    if query_layer.size(0) > 1 and pytorch_major_version >= 2:
+    if pytorch_major_version >= 2:
         query_layer = query_layer.permute(1, 2, 0, 3)
         if attention_mask is None and query_layer.shape[2] == key_layer.shape[2]:
 
             if torch.is_autocast_cpu_enabled():
                 attention_mask = torch.ones(query_layer.shape[2],
                                             key_layer.shape[2],
                                             dtype=torch.bool).tril(diagonal=0)
@@ -125,26 +125,43 @@
             else:
                 context_layer = torch.nn.functional.scaled_dot_product_attention(query_layer,
                                                                                  key_layer,
                                                                                  value_layer,
                                                                                  attention_mask,
                                                                                  is_causal=True)
         else:
+            # attention_mask is not None only when past_key_value is not None and q_len > 1
             if attention_mask is not None:
+                attn_bias = torch.zeros(attention_mask.shape, dtype=query_layer.dtype,
+                                        device=query_layer.device)
                 attention_mask = ~attention_mask
-            attention_mask = attention_mask.masked_fill(~attention_mask, -float('inf'), )
+                if attention_mask.dtype == torch.bool:
+                    attn_bias.masked_fill_(attention_mask.logical_not(), float("-inf"))
+                else:
+                    attn_bias += attention_mask
+            else:
+                attn_bias = None
             if torch.is_autocast_cpu_enabled():
                 query_layer = query_layer.to(torch.get_autocast_cpu_dtype())
                 key_layer = key_layer.to(torch.get_autocast_cpu_dtype())
                 value_layer = value_layer.to(torch.get_autocast_cpu_dtype())
                 attention_mask = attention_mask.to(torch.get_autocast_cpu_dtype())
-            context_layer = torch.nn.functional.scaled_dot_product_attention(query_layer,
-                                                                             key_layer,
-                                                                             value_layer,
-                                                                             attention_mask)
+                context_layer = torch.nn.functional.scaled_dot_product_attention(query_layer,
+                                                                                 key_layer,
+                                                                                 value_layer,
+                                                                                 attention_mask)
+            else:
+                head_dim = query_layer.size(-1)
+                attn = torch.matmul(query_layer.to(key_layer.dtype),
+                                    key_layer.transpose(2, 3)) / math.sqrt(head_dim)
+                if attn_bias is not None:
+                    attn += attn_bias
+                attn = F.softmax(attn, dim=-1,
+                                 dtype=torch.float32).to(value_layer.dtype)
+                context_layer = torch.matmul(attn, value_layer)
         context_layer = context_layer.permute(2, 0, 1, 3)
         new_context_layer_shape = context_layer.size()[:-2] + (self.hidden_size_per_partition,)
         context_layer = context_layer.reshape(*new_context_layer_shape)
         attention_probs = None
 
     else:
         query_key_layer_scaling_coeff = float(layer_id + 1)
```

## ipex_llm/transformers/models/chatglm2.py

```diff
@@ -21,15 +21,15 @@
 import torch
 from typing import Optional, Tuple, List
 import torch.nn.functional as F
 from transformers.modeling_outputs import BaseModelOutputWithPast
 from ipex_llm.transformers.models.utils import init_kv_cache, extend_kv_cache, append_kv_cache
 from ipex_llm.transformers.models.utils import init_fp8_kv_cache, append_fp8_kv_cache, \
     restore_fp8_kv_cache, use_quantize_kv_cache
-from ipex_llm.transformers.models.utils import use_esimd_sdp
+from ipex_llm.transformers.models.utils import use_sdp
 
 
 import os
 
 KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 KV_CACHE_ALLOC_MIN_LENGTH = 512
 
@@ -554,33 +554,36 @@
                 context_layer = torch.cat(results, dim=1)
             else:
                 context_layer = F.scaled_dot_product_attention(query_layer.to(key_layer.dtype),
                                                                key_layer,
                                                                value_layer,
                                                                is_causal=True).to(key_layer.dtype)
         else:
-            if use_esimd_sdp(query_layer.shape[2], key_layer.shape[2],
-                             query_layer.shape[-1], query_layer):
-                import linear_fp16_esimd
-                attn_output = linear_fp16_esimd.sdp_forward(query_layer,
-                                                            key_layer,
-                                                            value_layer)
+            # attention_mask is not None only when past_key_value is not None and q_len > 1
+            if attention_mask is not None:
+                attn_bias = torch.zeros(attention_mask.shape, dtype=query_layer.dtype,
+                                        device=query_layer.device)
+                attention_mask = ~attention_mask
+                if attention_mask.dtype == torch.bool:
+                    attn_bias.masked_fill_(attention_mask.logical_not(), float("-inf"))
+                else:
+                    attn_bias += attention_mask
+            else:
+                attn_bias = None
+
+            if use_sdp(query_layer.shape[2], key_layer.shape[2],
+                       query_layer.shape[-1], query_layer):
+                import linear_q4_0
+                attn_output = linear_q4_0.sdp(query_layer, key_layer, value_layer, attn_bias)
                 context_layer = attn_output.view(query_layer.shape)
             else:
                 head_dim = query_layer.size(-1)
                 attn = torch.matmul(query_layer.to(key_layer.dtype),
                                     key_layer.transpose(2, 3)) / math.sqrt(head_dim)
-                if attention_mask is not None:
-                    attn_bias = torch.zeros(attention_mask.shape, dtype=query_layer.dtype,
-                                            device=query_layer.device)
-                    attention_mask = ~attention_mask
-                    if attention_mask.dtype == torch.bool:
-                        attn_bias.masked_fill_(attention_mask.logical_not(), float("-inf"))
-                    else:
-                        attn_bias += attention_mask
+                if attn_bias is not None:
                     attn += attn_bias
                 attn = F.softmax(attn, dim=-1,
                                  dtype=torch.float32).to(value_layer.dtype)
                 context_layer = torch.matmul(attn, value_layer)
         context_layer = context_layer.permute(2, 0, 1, 3)
         new_context_layer_shape = context_layer.size()[:-2] + (-1,)
         context_layer = context_layer.reshape(*new_context_layer_shape)
```

## ipex_llm/transformers/models/llama.py

```diff
@@ -129,14 +129,48 @@
         use_cache=use_cache,
         output_attentions=output_attentions,
         output_hidden_states=output_hidden_states,
         return_dict=return_dict,
     )
 
 
+def llama_model_forward_4_38(
+    self,
+    input_ids: torch.LongTensor = None,
+    attention_mask: Optional[torch.Tensor] = None,
+    position_ids: Optional[torch.LongTensor] = None,
+    past_key_values: Optional[List[torch.FloatTensor]] = None,
+    inputs_embeds: Optional[torch.FloatTensor] = None,
+    use_cache: Optional[bool] = None,
+    output_attentions: Optional[bool] = None,
+    output_hidden_states: Optional[bool] = None,
+    return_dict: Optional[bool] = None,
+    cache_position: Optional[torch.LongTensor] = None,
+) -> Union[Tuple, BaseModelOutputWithPast]:
+    from ipex_llm.transformers.kv import DynamicFp8Cache
+    use_cache = use_cache if use_cache is not None else self.config.use_cache
+    input = input_ids if input_ids is not None else inputs_embeds
+    if use_cache and use_quantize_kv_cache(self.layers[0].mlp.up_proj, input):
+        if not isinstance(past_key_values, DynamicFp8Cache):
+            past_key_values = DynamicFp8Cache.from_legacy_cache(past_key_values)
+    return llama_model_forward_4_38_internal(
+        self=self,
+        input_ids=input_ids,
+        attention_mask=attention_mask,
+        position_ids=position_ids,
+        past_key_values=past_key_values,
+        inputs_embeds=inputs_embeds,
+        use_cache=use_cache,
+        output_attentions=output_attentions,
+        output_hidden_states=output_hidden_states,
+        return_dict=return_dict,
+        cache_position=cache_position,
+    )
+
+
 def llama_rms_norm_forward(self, hidden_states):
     if hidden_states.device.type == "xpu" and not (self.training and hidden_states.requires_grad):
         import linear_q4_0
         x_2d = hidden_states.reshape(-1, hidden_states.size(-1)).contiguous()
         output = linear_q4_0.rms_norm(self.weight, x_2d, self.variance_epsilon)
         return output.reshape(hidden_states.shape)
 
@@ -851,19 +885,21 @@
                                                                            current_key_states,
                                                                            current_value_states)
                 updated_past_key_values.append((current_key_states, current_value_states))
 
                 current_key_states = repeat_kv(current_key_states, self.num_key_value_groups)
                 current_value_states = repeat_kv(current_value_states, self.num_key_value_groups)
 
+                cache_position = None
                 current_query_states = query_states[batch: batch + 1, :, :, :]
                 attn_output, attn_weights = native_sdp(current_query_states,
                                                        current_key_states,
                                                        current_value_states,
                                                        attention_mask[batch],
+                                                       cache_position,
                                                        1,
                                                        1,
                                                        current_kv_len,
                                                        self.head_dim,
                                                        self.num_heads,
                                                        output_attentions)
                 if attn_output.size() != (1, self.num_heads, 1, self.head_dim):
@@ -897,18 +933,20 @@
                                                                      dtype=attention_dtype)
     value_states = repeat_kv(value_states, self.num_key_value_groups).to(device,
                                                                          dtype=attention_dtype)
     # Can also happens for decoding fast path
     if isinstance(attention_mask, list):
         # For decoding fast path
         attention_mask = attention_mask[0]
+    cache_position = None
     attn_output, attn_weights = native_sdp(query_states,
                                            key_states,
                                            value_states,
                                            attention_mask,
+                                           cache_position,
                                            bsz,
                                            q_len,
                                            kv_seq_len,
                                            self.head_dim,
                                            self.num_heads,
                                            output_attentions)
 
@@ -1135,16 +1173,20 @@
             else:
                 # upcast attention to fp32
                 attn_weights = nn.functional.softmax(attn_weights, dim=-1,
                                                      dtype=torch.float32).to(query_states.dtype)
             attn_output = torch.matmul(attn_weights, value_states)
         else:
             import linear_q4_0
+            if cache_position is not None:
+                new_attn_mask = attention_mask[:, :, kv_seq_len-q_len:kv_seq_len, 0:kv_seq_len]
+            else:
+                new_attn_mask = attention_mask
             attn_output = linear_q4_0.sdp_fp8(query_states, key_states, value_states,
-                                              attention_mask)
+                                              new_attn_mask)
             attn_weights = None
 
     if attn_output.size() != (bsz, self.num_heads, q_len, self.head_dim):
         invalidInputError(
             False,
             f"`attn_output` should be of size {(bsz, self.num_heads, q_len, self.head_dim)},"
             f" but is {attn_output.size()}"
@@ -1441,15 +1483,15 @@
 
     return attn_output.to(original_dtype), attn_weights, past_key_value
 
 
 def native_sdp(query, key, value, attention_mask, cache_position,
                bsz, q_len, kv_seq_len, head_dim, num_heads, output_attentions):
     if should_split_qkv_tensor(query, bsz, num_heads, q_len, kv_seq_len, output_attentions):
-        return native_sdp_split_qkv_tensor(query, key, value, attention_mask,
+        return native_sdp_split_qkv_tensor(query, key, value, attention_mask, cache_position,
                                            bsz, q_len, kv_seq_len, head_dim, num_heads)
     else:
         attn_weights = torch.matmul(query.to(key.dtype),
                                     key.transpose(2, 3)) / math.sqrt(head_dim)
 
         attn_weights_size = (bsz, num_heads, q_len, kv_seq_len)
         if attn_weights.size() != attn_weights_size:
@@ -1498,22 +1540,22 @@
                               f"Splitted attention weights should be of size "
                               f"{attn_weights_split_size}, but is {attn_weights_split.size()}")
 
         if attention_mask is not None:
             if cache_position is not None:
                 # for transformers 4.38.0
                 causal_mask = attention_mask[:, :, cache_position, : kv_seq_len]
-                attn_weights = attn_weights + causal_mask
+                attn_weights_split = attn_weights_split + causal_mask
             else:
                 attn_mask_size = (bsz, 1, q_len, kv_seq_len)
                 if attention_mask.size() != attn_mask_size:
                     invalidInputError(False,
                                       f"Attention mask should be of size {attn_mask_size}, "
                                       f"but is {attention_mask.size()}")
-                attn_weights = attn_weights + attention_mask
+                attn_weights_split = attn_weights_split + attention_mask
         attn_weights_split = nn.functional.softmax(attn_weights_split, dim=-1)
         attn_outputs.append(torch.matmul(attn_weights_split, v))
     attn_output = torch.cat(attn_outputs, dim=1)
     return attn_output.to(key.dtype), None
 
 
 def llama_model_selective_batching_forward_4_31(
@@ -1763,16 +1805,17 @@
         value_states = torch.cat([past_key_value[1], value_states], dim=2)
 
     past_key_value = (key_states, value_states) if use_cache else None
 
     key_states = repeat_kv(key_states, self.num_key_value_groups)
     value_states = repeat_kv(value_states, self.num_key_value_groups)
 
+    cache_position = None
     attn_output, attn_weights = native_sdp(query_states, key_states, value_states,
-                                           attention_mask,
+                                           attention_mask, cache_position,
                                            bsz, q_len, kv_seq_len,
                                            self.head_dim, self.num_heads, output_attentions)
 
     attn_output_size = (bsz, self.num_heads, q_len, self.head_dim)
     if attn_output.size() != attn_output_size:
         invalidInputError(False,
                           f"`attn_output` should be of size {attn_output_size},"
@@ -1793,14 +1836,143 @@
 
     if not output_attentions:
         attn_weights = None
 
     return attn_output, attn_weights, past_key_value
 
 
+def llama_model_forward_4_38_internal(
+    self,
+    input_ids: torch.LongTensor = None,
+    attention_mask: Optional[torch.Tensor] = None,
+    position_ids: Optional[torch.LongTensor] = None,
+    past_key_values: Optional[List[torch.FloatTensor]] = None,
+    inputs_embeds: Optional[torch.FloatTensor] = None,
+    use_cache: Optional[bool] = None,
+    output_attentions: Optional[bool] = None,
+    output_hidden_states: Optional[bool] = None,
+    return_dict: Optional[bool] = None,
+    cache_position: Optional[torch.LongTensor] = None,
+) -> Union[Tuple, BaseModelOutputWithPast]:
+    output_attentions = output_attentions if output_attentions is not None else \
+        self.config.output_attentions
+    output_hidden_states = (
+        output_hidden_states if output_hidden_states is not None else
+        self.config.output_hidden_states
+    )
+    use_cache = use_cache if use_cache is not None else self.config.use_cache
+    return_dict = return_dict if return_dict is not None else self.config.use_return_dict
+
+    # retrieve input_ids and inputs_embeds
+    if (input_ids is None) ^ (inputs_embeds is not None):
+        invalidInputError(False,
+                          f"You cannot specify both input_ids and inputs_embeds at the same time,"
+                          f" and must specify either one")
+
+    if self.gradient_checkpointing and self.training and use_cache:
+        logger.warning_once(
+            "`use_cache=True` is incompatible with gradient checkpointing. "
+            "Setting `use_cache=False`."
+        )
+        use_cache = False
+
+    if inputs_embeds is None:
+        inputs_embeds = self.embed_tokens(input_ids)
+
+    past_seen_tokens = 0
+    if use_cache:  # kept for BC (cache positions)
+        if not isinstance(past_key_values, Cache):
+            past_key_values = DynamicCache.from_legacy_cache(past_key_values)
+        past_seen_tokens = past_key_values.get_seq_length()
+
+    if cache_position is None:
+        cache_position = torch.arange(
+            past_seen_tokens, past_seen_tokens + inputs_embeds.shape[1],
+            device=inputs_embeds.device
+        )
+
+    if position_ids is None:
+        position_ids = cache_position.unsqueeze(0)
+
+    causal_mask = self._update_causal_mask(attention_mask, inputs_embeds)
+
+    # embed positions
+    hidden_states = inputs_embeds
+
+    # decoder layers
+    all_hidden_states = () if output_hidden_states else None
+    all_self_attns = () if output_attentions else None
+    next_decoder_cache = None
+
+    for decoder_layer in self.layers:
+        if output_hidden_states:
+            all_hidden_states += (hidden_states,)
+
+        if self.gradient_checkpointing and self.training:
+            layer_outputs = self._gradient_checkpointing_func(
+                decoder_layer.__call__,
+                hidden_states,
+                causal_mask,
+                position_ids,
+                past_key_values,
+                output_attentions,
+                use_cache,
+                cache_position,
+            )
+        else:
+            # bigdl-llm changes:
+            curr_device = decoder_layer.input_layernorm.weight.device
+            if causal_mask is not None:
+                causal_mask = causal_mask.to(curr_device)
+            if position_ids is not None:
+                position_ids = position_ids.to(curr_device)
+            # bigdl-llm changes end
+            layer_outputs = decoder_layer(
+                hidden_states,
+                attention_mask=causal_mask,
+                position_ids=position_ids,
+                past_key_value=past_key_values,
+                output_attentions=output_attentions,
+                use_cache=use_cache,
+                cache_position=cache_position,
+            )
+
+        hidden_states = layer_outputs[0]
+
+        if use_cache:
+            next_decoder_cache = layer_outputs[2 if output_attentions else 1]
+
+        if output_attentions:
+            all_self_attns += (layer_outputs[1],)
+
+    hidden_states = self.norm(hidden_states)
+
+    # add hidden states from the last decoder layer
+    if output_hidden_states:
+        all_hidden_states += (hidden_states,)
+
+    next_cache = None
+    from ipex_llm.transformers.kv import DynamicFp8Cache
+    if use_cache:
+        next_cache = (
+            next_decoder_cache.to_legacy_cache()
+            if not isinstance(next_decoder_cache, DynamicFp8Cache)
+            else next_decoder_cache
+        )
+    if not return_dict:
+        return tuple(v for v in [hidden_states, next_cache, all_hidden_states,
+                                 all_self_attns] if v is not None)
+    return BaseModelOutputWithPast(
+        last_hidden_state=hidden_states,
+        past_key_values=next_cache,
+        hidden_states=all_hidden_states,
+        attentions=all_self_attns,
+    )
+
+
 def llama_model_forward_4_36_internal(
     self,
     input_ids: torch.LongTensor = None,
     attention_mask: Optional[torch.Tensor] = None,
     position_ids: Optional[torch.LongTensor] = None,
     past_key_values: Optional[List[torch.FloatTensor]] = None,
     inputs_embeds: Optional[torch.FloatTensor] = None,
```

## ipex_llm/transformers/models/phi3.py

```diff
@@ -34,19 +34,18 @@
 import math
 import torch
 import warnings
 from torch import nn
 
 from ipex_llm.transformers.models.utils import (
     rotate_half, should_use_fuse_rope,
-    apply_rotary_pos_emb_cache_freq_xpu
 )
 from ipex_llm.transformers.models.utils import mlp_fusion_check, SILU
-from ipex_llm.transformers.models.utils import use_sdp, use_sdp_causal, use_quantize_kv_cache
-from ipex_llm.transformers.models.utils import use_sdp_fp8, restore_fp8_kv_cache
+from ipex_llm.transformers.models.utils import use_sdp, use_sdp_causal
+from ipex_llm.transformers.models.utils import use_quantize_kv_cache, restore_fp8_kv_cache
 from ipex_llm.transformers.kv import DynamicNormalCache, DynamicFp8Cache
 
 from typing import Optional, Tuple, List
 from transformers.models.phi.modeling_phi import repeat_kv
 from transformers.cache_utils import Cache
 
 
@@ -54,54 +53,37 @@
     cos = cos.unsqueeze(unsqueeze_dim)
     sin = sin.unsqueeze(unsqueeze_dim)
     q_embed = (q * cos) + (rotate_half(q) * sin)
     k_embed = (k * cos) + (rotate_half(k) * sin)
     return q_embed, k_embed
 
 
-def su_scaled_rope_forward(self, x: torch.Tensor, position_ids: torch.Tensor, seq_len=None):
-    if self.inv_freq is None:
-        short_ext_factors = torch.tensor(self.short_factor, dtype=torch.float32, device=x.device)
-        inv_freq_shape = torch.arange(0, self.dim, 2,
-                                      dtype=torch.int64, device=x.device).float() / self.dim
-        self.inv_freq = 1.0 / (short_ext_factors * self.base**inv_freq_shape)
-
-        long_ext_factors = torch.tensor(self.long_factor, dtype=torch.float32, device=x.device)
-        self.register_buffer("long_inv_freq", None, persistent=False)
-        self.long_inv_freq = 1.0 / (long_ext_factors * self.base**inv_freq_shape)
-
-    seq_len = seq_len if seq_len is not None else torch.max(position_ids) + 1
-    if seq_len > self.original_max_position_embeddings:
-        inv_freq = self.long_inv_freq
-    else:
-        inv_freq = self.inv_freq
-
-    inv_freq_expanded = inv_freq[None, :, None].float().expand(position_ids.shape[0], -1, 1)
-    position_ids_expanded = position_ids[:, None, :].float()
+def pre_compute_inv_freq(module: torch.nn.Module):
+    if module.__class__.__name__ == "Phi3RotaryEmbedding":
+        module.inv_freq = 1.0 / (
+            module.base **
+            (torch.arange(0, module.dim, 2, dtype=torch.int64).float() / module.dim)
+        )
+    elif module.__class__.__name__ == "Phi3SuScaledRotaryEmbedding":
+        inv_freq_shape = torch.arange(0, module.dim, 2, dtype=torch.int64).float() / module.dim
+        short_ext_factors = torch.tensor(module.short_factor, dtype=torch.float32)
+        module.inv_freq = 1.0 / (short_ext_factors * module.base ** inv_freq_shape)
+
+        long_ext_factors = torch.tensor(module.long_factor, dtype=torch.float32)
+        module.register_buffer("long_inv_freq", None, persistent=False)
+        module.long_inv_freq = 1.0 / (long_ext_factors * module.base ** inv_freq_shape)
 
-    # Force float32 since bfloat16 loses precision on long contexts
-    # See https://github.com/huggingface/transformers/pull/29285
-    device_type = x.device.type
-    device_type = device_type if isinstance(device_type, str) and device_type != "mps" else "cpu"
-    with torch.autocast(device_type=device_type, enabled=False):
-        freqs = (inv_freq_expanded.float() @ position_ids_expanded.float()).transpose(1, 2)
-        emb = torch.cat((freqs, freqs), dim=-1)
-
-        scale = self.max_position_embeddings / self.original_max_position_embeddings
-        if scale <= 1.0:
-            scaling_factor = 1.0
+        if module.max_position_embeddings <= module.original_max_position_embeddings:
+            module.scaling_factor = 1.0
         else:
-            scaling_factor = math.sqrt(
-                1 + math.log(scale) / math.log(self.original_max_position_embeddings)
+            scale = module.max_position_embeddings / module.original_max_position_embeddings
+            module.scaling_factor = math.sqrt(
+                1 + math.log(scale) / math.log(module.original_max_position_embeddings)
             )
 
-        cos = emb.cos() * scaling_factor
-        sin = emb.sin() * scaling_factor
-    return cos.to(dtype=x.dtype), sin.to(dtype=x.dtype)
-
 
 def attention_forward(
     self,
     hidden_states: torch.Tensor,
     attention_mask: Optional[torch.Tensor] = None,
     position_ids: Optional[torch.LongTensor] = None,
     past_key_value: Optional[Cache] = None,
@@ -120,35 +102,47 @@
                                                         self.num_key_value_heads,
                                                         self.num_key_value_heads], dim=1)
 
     kv_seq_len = key_states.shape[-2]
     if past_key_value is not None:
         kv_seq_len += past_key_value.get_usable_length(kv_seq_len, self.layer_idx)
 
-    cos, sin = self.rotary_emb(value_states, position_ids, seq_len=kv_seq_len)
     # IPEX-LLM OPT: fuse rope
     if should_use_fuse_rope(hidden_states, position_ids, self.training):
-        query_states, key_states = apply_rotary_pos_emb_cache_freq_xpu(query_states, key_states,
-                                                                       sin, cos, "phi3")
+        import linear_q4_0
+        if self.rotary_emb.__class__.__name__ == "Phi3RotaryEmbedding":     # 4k
+            linear_q4_0.rotary_half_inplaced(self.rotary_emb.inv_freq, position_ids,
+                                             query_states, key_states)
+        else:   # 128k
+            if kv_seq_len > self.rotary_emb.original_max_position_embeddings:
+                linear_q4_0.rotary_half_inplaced(self.rotary_emb.long_inv_freq, position_ids,
+                                                 query_states, key_states)
+            else:
+                linear_q4_0.rotary_half_inplaced(self.rotary_emb.inv_freq, position_ids,
+                                                 query_states, key_states)
+            # todo: fuse scaling_factor
+            query_states *= self.rotary_emb.scaling_factor
+            key_states *= self.rotary_emb.scaling_factor
     else:
+        cos, sin = self.rotary_emb(value_states, position_ids, seq_len=kv_seq_len)
         query_states, key_states = apply_rotary_pos_emb(query_states, key_states,
                                                         cos, sin, position_ids)
 
     if past_key_value is not None:
         key_states, value_states = past_key_value.update(key_states, value_states,
                                                          self.layer_idx, None)
 
     if use_sdp(q_len, kv_seq_len, self.head_dim, query_states):
         import linear_q4_0
         if isinstance(past_key_value, DynamicFp8Cache):
             attn_output = linear_q4_0.sdp_fp8(query_states, key_states, value_states,
                                               attention_mask)
         else:
             attn_output = linear_q4_0.sdp(query_states, key_states, value_states, attention_mask)
-    elif use_sdp_causal(q_len, kv_seq_len, query_states, self.training):
+    elif use_sdp_causal(q_len, kv_seq_len, self.head_dim, query_states, self.training):
         import linear_q4_0
         if isinstance(past_key_value, DynamicFp8Cache):
             attn_output = linear_q4_0.sdp_fp8_causal(query_states, key_states, value_states)
         else:
             attn_output = linear_q4_0.sdp_causal(query_states, key_states, value_states)
     else:
         if isinstance(past_key_value, DynamicFp8Cache):
@@ -253,58 +247,14 @@
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
     return model_forward
 
 
-class Phi3RotaryEmbeddingCached(nn.Module):
-    def __init__(self, dim, max_position_embeddings=2048, base=10000, device=None):
-        super().__init__()
-
-        self.dim = dim
-        self.max_position_embeddings = max_position_embeddings
-        self.base = base
-        inv_freq = 1.0 / (self.base ** (torch.arange(0, self.dim, 2,
-                                                     dtype=torch.int64,
-                                                     device=device).float() / self.dim))
-        self.register_buffer("inv_freq", inv_freq, persistent=False)
-        # self.gen_seq_len = None
-
-        # Build here to make `torch.jit.trace` work.
-        self._set_cos_sin_cache(
-            seq_len=max_position_embeddings,
-            device=self.inv_freq.device, dtype=torch.get_default_dtype()
-        )
-
-    def _set_cos_sin_cache(self, seq_len, device, dtype):
-        self.max_seq_len_cached = seq_len
-        position_ids_expanded = torch.arange(self.max_seq_len_cached,
-                                             device=device,
-                                             dtype=self.inv_freq.dtype).reshape(1, 1, -1)
-        inv_freq_expanded = self.inv_freq[None, :, None].float().expand(1, -1, 1)
-        with torch.autocast(device_type=device.type, enabled=False):
-            freqs = (inv_freq_expanded.float() @ position_ids_expanded.float()).transpose(1, 2)
-            # Different from paper,
-            # but it uses a different permutation in order to obtain the same calculation
-            emb = torch.cat((freqs, freqs), dim=-1)
-            self.register_buffer("cos_cached", emb.cos().to(dtype), persistent=False)
-            self.register_buffer("sin_cached", emb.sin().to(dtype), persistent=False)
-
-    def forward(self, x, position_ids, seq_len=None):
-        # x: [bs, num_attention_heads, seq_len, head_size]
-        if seq_len > self.max_seq_len_cached:
-            self._set_cos_sin_cache(seq_len=seq_len, device=x.device, dtype=x.dtype)
-
-        return (
-            self.cos_cached[:, seq_len-position_ids.shape[-1]:seq_len, :].to(dtype=x.dtype),
-            self.sin_cached[:, seq_len-position_ids.shape[-1]:seq_len, :].to(dtype=x.dtype),
-        )
-
-
 def phi3_rms_norm_forward(self, hidden_states):
     if hidden_states.device.type == "xpu" and not (self.training and hidden_states.requires_grad):
         import linear_q4_0
         x_2d = hidden_states.reshape(-1, hidden_states.size(-1)).contiguous()
         output = linear_q4_0.rms_norm(self.weight, x_2d, self.variance_epsilon)
         return output.reshape(hidden_states.shape)
```

## ipex_llm/transformers/models/qwen2_moe.py

```diff
@@ -48,15 +48,15 @@
 from ipex_llm.transformers.models.qwen2 import should_use_fuse_rope
 from ipex_llm.transformers.models.utils import extend_kv_cache, append_kv_cache
 from ipex_llm.transformers.models.utils import apply_rotary_pos_emb_cache_freq_xpu
 from ipex_llm.transformers.models.utils import is_enough_kv_cache_room_4_36
 from transformers.models.qwen2.modeling_qwen2 import apply_rotary_pos_emb
 from ipex_llm.utils.common import invalidInputError
 from ipex_llm.transformers.models.utils import decoding_fast_path_qtype_check
-from ipex_llm.transformers.models.utils import use_flash_attention, use_esimd_sdp
+from ipex_llm.transformers.models.utils import use_flash_attention
 from transformers.models.qwen2_moe.modeling_qwen2_moe import Qwen2MoeModel, apply_rotary_pos_emb
 from ipex_llm.transformers.models.utils import use_quantize_kv_cache, restore_fp8_kv_cache
 from ipex_llm.transformers.kv import DynamicFp8Cache
 
 import os
 
 KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
```

## ipex_llm/transformers/models/utils.py

```diff
@@ -314,77 +314,14 @@
                 return False
             elif not attention_mask.equal(attention_mask[0].repeat(bsz, 1, 1, 1)):
                 # check whether mask of every batch is the same
                 return False
     return True
 
 
-def use_esimd_sdp(q_len, k_len, head_dim, query_states, attention_mask=None):
-    if head_dim != 128:
-        # esimd_sdp only support head_dim = 128 now
-        return False
-    elif q_len != 1:
-        # esimd_sdp only support rest token and q_len == 1 now
-        return False
-    elif k_len < 8:
-        # esimd_sdp will cause wrong output when k_len < 8
-        return False
-    elif query_states.device.type != "xpu":
-        # esimd_sdp only support GPU now
-        return False
-    elif query_states.dtype != torch.float16:
-        # esimd_sdp only has optimization for FP16 now
-        return False
-
-    device_name = torch.xpu.get_device_name(query_states.device.index)
-    if device_name.startswith("Intel(R) Arc(TM) A") or \
-       device_name.startswith("Intel(R) Data Center GPU Flex") or \
-       device_name.startswith("Intel(R) Data Center GPU Max"):
-        import linear_fp16_esimd
-        if not hasattr(linear_fp16_esimd, "sdp_forward"):
-            return False
-    else:
-        return False
-
-    if query_states.shape[0] > 1 and device_name.startswith("Intel(R) Data Center GPU Max"):
-        # esimd_sdp not support PVC GPU when batch size > 1 for now
-        return False
-    if query_states.shape[0] > 1 and device_name.startswith("Intel(R) Arc(TM) A") \
-            and is_deepspeed_available:
-        # esimd_sdp not support ARC GPU when batch size > 1 using DeepSpeed AutoTP for now
-        return False
-    if query_states.shape[0] > 1 and attention_mask is not None:
-        # for batched input, can't accept attention_mask
-        # TODO: this check needs some time
-        if not torch.all(attention_mask.eq(0)):
-            return False
-
-    return True
-
-
-def use_new_esimd_sdp_fp16(q_len, k_len, head_dim, query_states):
-    if query_states.device.type != "xpu":
-        # esimd_sdp only support GPU now
-        return False
-    elif query_states.dtype != torch.float16:
-        # esimd_sdp only has optimization for FP16 now
-        return False
-    elif head_dim not in [64, 96, 128]:
-        # esimd_sdp only support head_dim = 128 and 64 now
-        return False
-    elif q_len == k_len:
-        # new sdp_fp16 only support rest token now
-        return False
-    elif q_len > 32:
-        # Use new sdp_fp16 only when q_len <= 32
-        return False
-
-    return True
-
-
 def use_sdp(q_len, kv_len, head_dim, query_states):
     return (
         query_states.device.type == "xpu"
         and query_states.dtype in [torch.float, torch.half]     # fp32/fp16
         and head_dim in [64, 96, 128]
         and q_len != kv_len     # next token
         and q_len <= 32         # lookup
@@ -396,17 +333,18 @@
         query_states.device.type == "xpu"
         and query_states.dtype in [torch.float, torch.half]     # fp32/fp16
         and q_len != kv_len     # next token
         and q_len <= 32         # lookup
     )
 
 
-def use_sdp_causal(q_len, kv_len, query_states, training):
+def use_sdp_causal(q_len, kv_len, head_dim, query_states, training):
     return (
         q_len == kv_len     # first token
+        and head_dim in [64, 96, 128]           # for now
         and query_states.device.type == "xpu"   # GPU
         and query_states.dtype in [torch.float, torch.half]     # fp32/fp16
         and not query_states.requires_grad and not training     # not training
     )
 
 
 def mlp_fusion_check(x, qtype, training):
```

## Comparing `ipex_llm-2.1.0b20240515.data/scripts/llm-chat.ps1` & `ipex_llm-2.1.0b20240516.data/scripts/llm-chat.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240515.data/scripts/llm-cli.ps1` & `ipex_llm-2.1.0b20240516.data/scripts/llm-cli.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240515.dist-info/METADATA` & `ipex_llm-2.1.0b20240516.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipex-llm
-Version: 2.1.0b20240515
+Version: 2.1.0b20240516
 Summary: Large Language Model Develop Toolkit
 Home-page: https://github.com/intel-analytics/BigDL
 Author: BigDL Authors
 Author-email: bigdl-user-group@googlegroups.com
 License: Apache License, Version 2.0
 Platform: windows
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,23 +13,24 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Requires-Dist: py-cpuinfo ; extra == 'all'
 Requires-Dist: protobuf ; extra == 'all'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'all'
 Requires-Dist: numpy (==1.26.4) ; extra == 'all'
-Requires-Dist: torch ; extra == 'all'
 Requires-Dist: transformers (==4.31.0) ; extra == 'all'
 Requires-Dist: sentencepiece ; extra == 'all'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'all'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'all'
 Requires-Dist: tabulate ; extra == 'all'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'all'
+Requires-Dist: torch (==2.1.2+cpu) ; (platform_system == "Linux") and extra == 'all'
+Requires-Dist: torch (==2.1.2) ; (platform_system == "Windows") and extra == 'all'
 Provides-Extra: cpp
-Requires-Dist: bigdl-core-cpp (==2.5.0b20240515) ; extra == 'cpp'
+Requires-Dist: bigdl-core-cpp (==2.5.0b20240516) ; extra == 'cpp'
 Requires-Dist: dpcpp-cpp-rt (==2024.0.2) ; (platform_system == "Windows") and extra == 'cpp'
 Requires-Dist: mkl-dpcpp (==2024.0.0) ; (platform_system == "Windows") and extra == 'cpp'
 Requires-Dist: onednn (==2024.0.0) ; (platform_system == "Windows") and extra == 'cpp'
 Provides-Extra: llama-index
 Requires-Dist: py-cpuinfo ; extra == 'llama-index'
 Requires-Dist: protobuf ; extra == 'llama-index'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'llama-index'
@@ -54,31 +55,31 @@
 Requires-Dist: sentencepiece ; extra == 'xpu'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu'
 Requires-Dist: tabulate ; extra == 'xpu'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240515) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240515) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240516) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240516) ; extra == 'xpu'
 Provides-Extra: xpu-2-1
 Requires-Dist: py-cpuinfo ; extra == 'xpu-2-1'
 Requires-Dist: protobuf ; extra == 'xpu-2-1'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-1'
 Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-1'
 Requires-Dist: transformers (==4.31.0) ; extra == 'xpu-2-1'
 Requires-Dist: sentencepiece ; extra == 'xpu-2-1'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu-2-1'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-1'
 Requires-Dist: tabulate ; extra == 'xpu-2-1'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240515) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240515) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240516) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240516) ; extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-1'
 Requires-Dist: dpcpp-cpp-rt (==2024.0.2) ; (platform_system == "Windows") and extra == 'xpu-2-1'
 Requires-Dist: mkl-dpcpp (==2024.0.0) ; (platform_system == "Windows") and extra == 'xpu-2-1'
 Requires-Dist: onednn (==2024.0.0) ; (platform_system == "Windows") and extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu'
 Requires-Dist: dpcpp-cpp-rt (==2024.0.2) ; (platform_system == "Windows") and extra == 'xpu'
 Requires-Dist: mkl-dpcpp (==2024.0.0) ; (platform_system == "Windows") and extra == 'xpu'
```

## Comparing `ipex_llm-2.1.0b20240515.dist-info/RECORD` & `ipex_llm-2.1.0b20240516.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -38,58 +38,58 @@
 ipex_llm/langchain/embeddings/bigdlllm.py,sha256=auNueZ-S5RQrngss_huXlYdWImX2vPYfuEVOZsx35rk,13589
 ipex_llm/langchain/embeddings/transformersembeddings.py,sha256=hBtqBfGmGg_xjb4Us7hLNfyvbLMo5mJk9a0iooOWtPM,7225
 ipex_llm/langchain/llms/__init__.py,sha256=vBCl9JF45vnk9CWBG1k8lp8J6F8OCR9UY2E-idkkm5Y,1636
 ipex_llm/langchain/llms/bigdlllm.py,sha256=FAZG6cAIJhRgbxm16gMq-cyBwLe-u165zE7yyxD7r9E,24438
 ipex_llm/langchain/llms/transformersllm.py,sha256=7eaIkJi1CbTCSgNxBCoZTe-o_5FYjD1GTYPWpn0Ccr4,10576
 ipex_llm/langchain/llms/transformerspipelinellm.py,sha256=vm522YPPwWxxAPVvQBtxRfBinC4hIbXdKW6VjHDaFXY,7379
 ipex_llm/libs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ipex_llm/libs/bloom-api.dll,sha256=vD6jJYHUIXV_pi6XdH_jtdA7YC8lFfyLE1Uj2abqXRw,36352
-ipex_llm/libs/bloom.dll,sha256=_vSF8CAILTZyfsg0iegmWw2W89mylM15XY6KQysXIfI,473088
-ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=wyBxYJtbBtKVeMfPU_qZomQSBkdaz4vv9DIrIEzBF7I,854016
-ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=eSqlN1y44C07s3DRxNmS1NClc5fyqFTH5ZivWYXXzKU,856576
-ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=8bGBmISvxymBOu7HDDrPV24lPz88eTb-cwvnUFH2MJM,844288
-ipex_llm/libs/gptneox-api.dll,sha256=Qvp5exCrXItZSjwa7AvYxKYwVdYnx_ZQF6QwSRCUzKA,24576
-ipex_llm/libs/gptneox.dll,sha256=pmzy_PSUYxGyNn8DoeoUsguzVVajUBTkZXSPg_R5Gcs,532992
-ipex_llm/libs/libbloom_avx.dll,sha256=HafudzlIJZY4wGZ6cVBTTWkCZlNdjAYxt9ATbmqNRyY,499712
-ipex_llm/libs/libbloom_vnni.dll,sha256=k6PjDyAHsq9jqGBatXPjAo27kDPiIng-uBCZa8UuEWI,473600
-ipex_llm/libs/libgptneox_avx.dll,sha256=p8Odg5iBeXoHqfwnr4amjGovlsMHvuSnrTA-62aFjiE,559104
-ipex_llm/libs/libgptneox_vnni.dll,sha256=gTvd-hwAcx-4xwjousgioK3jCK9ILYatGYS5hA-8GZc,533504
-ipex_llm/libs/libllama_avx.dll,sha256=uf22b2bZpVw8Yaz8SrzC8_uhkAZ0LQ0ruD-xBMpRvys,553472
-ipex_llm/libs/libllama_vnni.dll,sha256=p3Exx1tJurRra3PF6XA-HayX7uwKOlN5my6eKQt5ifo,527872
-ipex_llm/libs/libstarcoder_avx.dll,sha256=EU6Sv2rxwB6XtXFEoaNvLNCARu4MH7ZAUt4zHgeivYg,590848
-ipex_llm/libs/libstarcoder_vnni.dll,sha256=n1qHD3khJ9GkZeZKeKf9fxvwB6BUxgHFIDFjj8WaDZY,564736
-ipex_llm/libs/llama-api.dll,sha256=xuKE9xR6YmjxfRIyNeyiNvY8OdRfAvxsMpt6cOZVBtE,25088
-ipex_llm/libs/llama.dll,sha256=2EAWV2pq2rL7pzqljy2Ce9HrP3jRGr09M5JaeoVhMjg,526848
-ipex_llm/libs/main-bloom.exe,sha256=kHuxvAiK0n3Om8wXMQUOyMgkLurLp3X9FxMreigKP18,103424
-ipex_llm/libs/main-chatglm_vnni.exe,sha256=rRQWswk8xPiIUmVRFTHkOP6sD3EF0S9MD9-bfQ9v640,726016
-ipex_llm/libs/main-gptneox.exe,sha256=SCkjJJ_69ouCMtu9Y3-pKxe8gZifxMWlPqkveeBBXbw,98816
-ipex_llm/libs/main-llama.exe,sha256=GoIGZvVmlnxqaSxJLu23t8woAFzW8V0iN15WYc1ywgY,99840
-ipex_llm/libs/main-starcoder.exe,sha256=nWzUc8lvkFN5oryLWeUm6eUIRfTZrsMlsK3HVUMRolA,157696
-ipex_llm/libs/quantize-bloom.exe,sha256=v-8bGue6MJ8YgvyiWwNj9gwUJo7hyvo9C1gs1gXPPQA,126464
-ipex_llm/libs/quantize-bloom_vnni.exe,sha256=lmKueF8--OPZ9tGb7Z6fXTVwrfpHnjYJeZa_Iciy2NQ,127488
-ipex_llm/libs/quantize-gptneox.exe,sha256=WlTe6zZUfDzh_HeRWrP_Xat0NkUh3E5AOHfKuHzWrRQ,103936
-ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=lRSs9vXyJFQrOaM_6z1At5JN13cY1RjCYWanb-2arWA,104448
-ipex_llm/libs/quantize-llama.exe,sha256=jceDivyFPx-1MfEEAExs_x_BouLTw5TtqtY89OncrRg,109056
-ipex_llm/libs/quantize-llama_vnni.exe,sha256=O66vQZkJsTIVAsQ2qEi87Uk1Vy27f6K93DFN_biYl8I,110080
-ipex_llm/libs/quantize-starcoder.exe,sha256=vZwjKWuDrf-SGPxBDqZD4-_kerBB9KZiW3i6K-B1-eQ,126976
-ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=-AJQW8yU5vj9Q-7C5ZIwHEeJstf-rHtso2JQ3ByrPqc,128512
-ipex_llm/libs/starcoder-api.dll,sha256=Pdfjww63PfNCTjfPxecNsOu_G3zX_nfNACiwUFL4VIs,21504
-ipex_llm/libs/starcoder.dll,sha256=n4KTQyDRN5uLLd7AKipmNtTZ2oCFEz7GAVMPW8oLGxM,564224
+ipex_llm/libs/bloom-api.dll,sha256=yfycsWaGUinYpeF4Qja9gsn__5BR9ouG3d39F88LjxA,36352
+ipex_llm/libs/bloom.dll,sha256=Tr2-k5BX5wmEBtRUj3dB_UcoWYeA6abX_BOrRFShu-g,473088
+ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=Fm6xW0TyFc_ou60slMknd2aASUQd0FzdmEibltQ2gd4,854016
+ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=ouAcVgzdqPvKLtdwIDgrjhqNUeSbFXMFlBWkLQI67Pg,856576
+ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=6UTEfiZwC1qxD1jjZP8c8XRUFjX5YD7oTd_tphofAE0,844288
+ipex_llm/libs/gptneox-api.dll,sha256=urIdrwkCZkBx6Lmmor3yc70xZCI3DYfO4MOcvwOsqp4,24576
+ipex_llm/libs/gptneox.dll,sha256=-Ni5bI4jmGeCs19zXQHdvMmRaU2rx20QKgmby0Qnl-0,532992
+ipex_llm/libs/libbloom_avx.dll,sha256=8p-HkbXzSOzyZaWuqLhZZHoWCuLBXooSzj3bzRYtN4Q,499712
+ipex_llm/libs/libbloom_vnni.dll,sha256=e15NbH8UkZ6Dil_fHx_YN0GRyn7YSKTxHk-6okLfjCk,473600
+ipex_llm/libs/libgptneox_avx.dll,sha256=3h6kEljKnM2ak0NMRq2lE9WDIRddd4s5_SN0w7KRpL0,559104
+ipex_llm/libs/libgptneox_vnni.dll,sha256=p_Pvo9rZh2GrNhYaabF10U_I7o2QNl8jdOn2bpSUXLU,533504
+ipex_llm/libs/libllama_avx.dll,sha256=0-W67AYXOJcmRtU_lRJ8tMlAGZ7WQM13ORzFDRBxIhI,553472
+ipex_llm/libs/libllama_vnni.dll,sha256=wxqFo73-jqaG8xChysvBpRRnxpg-L-l2R8zqT2t-km8,527872
+ipex_llm/libs/libstarcoder_avx.dll,sha256=Zi2Fhs53xOMiI5NNvvLDL-cLy7kYpLCNPWtVZyZacqk,590848
+ipex_llm/libs/libstarcoder_vnni.dll,sha256=gd_m77U-JP4qjr7VYoCTTgat5_y7QQ1FZAXpdOioItU,564736
+ipex_llm/libs/llama-api.dll,sha256=LiluZREjmgmkM2nGYt7KPVwFx8z4AfKevQs1OriHnIY,25088
+ipex_llm/libs/llama.dll,sha256=aTjamPd2RF5Yn3Ui_SlGfT0BFsBbAKBK2fDW0o3Otu8,526848
+ipex_llm/libs/main-bloom.exe,sha256=sSEsrMr_kiAmWfVKzKga-1DBvvBgFP1Y1fvQZK2GxUw,103424
+ipex_llm/libs/main-chatglm_vnni.exe,sha256=1h89dnsvybirPJhXfb40MSU9xLVd5jRrDufw3Y2Sf6U,726016
+ipex_llm/libs/main-gptneox.exe,sha256=5lq8I1iMJyrylNNksETwYXEXKw6SWP_o_XNeaDnU4RU,98816
+ipex_llm/libs/main-llama.exe,sha256=TtJHfvRp24K0Y7eOLZbHdnVurw_kJ5wZEgY46lb9jrE,99840
+ipex_llm/libs/main-starcoder.exe,sha256=cJzrkGisQxdNbkpnvM3m7-0xCMbBAZhNU2FURXy53hM,157696
+ipex_llm/libs/quantize-bloom.exe,sha256=rRgz9iSs3W7yGZylzOSY24SLYsz7a7qB-golhAAjIvI,126464
+ipex_llm/libs/quantize-bloom_vnni.exe,sha256=WsVBOHRSC6TZ4CBudNetDIWwfJzJsEWZANv_yb6L9GM,127488
+ipex_llm/libs/quantize-gptneox.exe,sha256=RrSgitK2LfxQS9c006a-R7wrgorLGh_VxYLXQuaZhXw,103936
+ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=XqCo9W-rL2_S_39QQ2Yr5p_yCYDNMRjrRA2Hu4AjYm8,104448
+ipex_llm/libs/quantize-llama.exe,sha256=rL5ryr5nuWNS2bOPYWf75tHjmdk3GkBPDpvcv4G9I6A,109056
+ipex_llm/libs/quantize-llama_vnni.exe,sha256=RRvnHCOTfPkIU5LUZqgGgbQQG2pKS1BKwKcxfIa_o50,110080
+ipex_llm/libs/quantize-starcoder.exe,sha256=9NsugfRvlLYfOkIxcgohHhpMzw6GlgVeOLv5TtBAa2o,126976
+ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=ZtMG68nMtVOGBe7glDHyd95Ncpw0kPYTCV8j7ydBXE8,128512
+ipex_llm/libs/starcoder-api.dll,sha256=Kgx9_5Q93ywMhbYLfdg0jaeJNA3n4MuflRxYQ9hOLws,21504
+ipex_llm/libs/starcoder.dll,sha256=ZCWEu9efFtS6d1diKY5cEDVNCsMdQap8eVET0A6Y-2o,564224
 ipex_llm/llamaindex/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/llamaindex/llms/__init__.py,sha256=KP1lEdGqDuxPoxL1ZSH25Pm2kKMPJBWUTLR0ckSLMIU,1139
 ipex_llm/llamaindex/llms/bigdlllm.py,sha256=FQBzq1KOjfc6uofTXAha3O7TqpJkNfOFepXQmOVlbnI,26314
 ipex_llm/serving/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/bigdl_llm_model.py,sha256=NXEN_3EPmcP3dDnvug4MokEXXE2zVUnENgBYxfubqic,10084
 ipex_llm/serving/fastchat/ipex_llm_worker.py,sha256=Jt3xvx7MJe8r5C5oAiJ5D3D_MbNGtcszrYiywuMIm5A,19585
 ipex_llm/serving/fastchat/model_worker.py,sha256=qJSLyWNkP6z70ysq4AV5SqHzXPJJiX2tz7AORB6jEvM,16649
 ipex_llm/serving/fastchat/vllm_worker.py,sha256=r_2yiI4v69w8teNzh8mZrKMsJ0l6NvWFl8TxEkvq0ug,10801
 ipex_llm/transformers/__init__.py,sha256=8zrY1AGBb2_AeKGDWHY4PCJyzelYA4KwahD54jPoiPg,1005
 ipex_llm/transformers/bmm.py,sha256=BlYrXqeJuw-m136Nf_ST9i6WtZrX6BiTG_psTe1M3Y0,1213
-ipex_llm/transformers/convert.py,sha256=NHRBzqecrMk2b3tCPybGqZwlHPlcY9ExQ1hnFPtX2HM,75714
+ipex_llm/transformers/convert.py,sha256=1fNtu3n-QDmtgROgB-NEphVUo-SmG9PhFh5LOOUhWhM,75529
 ipex_llm/transformers/convert_ipex.py,sha256=iKXo0n8fVFTOA2fNYYrByMFK0dovL-kLd2sVDk88AlQ,14334
 ipex_llm/transformers/embedding.py,sha256=f3crD31fEq0pT-d4FV_fS_9uLhgW64BofAxhHSO1QbE,4613
 ipex_llm/transformers/kv.py,sha256=PDdcXWElpiPvzVJQdkkx6Vez0mhROW4K59sngYaX0yY,4247
 ipex_llm/transformers/lisa.py,sha256=F5WxbtXQ7RdKulj83h_2DnEIgKiKGZf7zvOmg6QBl2s,3289
 ipex_llm/transformers/loader.py,sha256=0wMJ9NM0QKRB3AgVRGLmOKcSHYlQ40Rj6UXba513NG0,6812
 ipex_llm/transformers/lookup.py,sha256=OBFFNkuSHP9lK6ePTnNFieKs4_vRs83mECrJj0_XoCU,15562
 ipex_llm/transformers/low_bit_linear.py,sha256=iBMeQPIImmJLs6bc_AHis0RBOFRiY_kjl5PInTzRv-s,39846
@@ -128,44 +128,44 @@
 ipex_llm/transformers/gguf/models/model_implement/yuan2/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/transformers/gguf/models/model_implement/yuan2/configuration_yuan.py,sha256=PDCUoD7z5cR-61oBjMc5uBCzgtiLx7sbTZ6nTnDU49A,2192
 ipex_llm/transformers/gguf/models/model_implement/yuan2/yuan_hf_model.py,sha256=_AOGMV65XHxgTxIib7lgs49InopcecTzRwgtYR8NTUg,51084
 ipex_llm/transformers/layers/rope_embedding.py,sha256=aL36BVCsjrWSi9DyMWsPOgj5VUNDooYsaO2HDaWAEzs,2658
 ipex_llm/transformers/models/__init__.py,sha256=tp2DcVkKg1-QvdYk7DY7rZvQWCDQ4ZjU8NAQ7Fclrpg,584
 ipex_llm/transformers/models/aquila.py,sha256=xLMxa8EOtpXDdyT9fAc0If_DkuH8Knzmi0Logrv0Jdk,7415
 ipex_llm/transformers/models/baichuan.py,sha256=jwN4MWnT96UravTB87aA0Xri9OZMrLx1gX-4ziyz8H4,24239
-ipex_llm/transformers/models/baichuan2.py,sha256=ucI8BCE6_MWiuXv28vzEkIaFUea_7szT-a62YvDE2oQ,29489
+ipex_llm/transformers/models/baichuan2.py,sha256=yWKiIvIRQ1s_Cdu32cpS5ZnmI6324w6mu7y8EKJPrKw,29360
 ipex_llm/transformers/models/bert.py,sha256=bJNic2pt1kph0kBwdK5MRGyWupFfx2Ts0V3D1L-5kWo,6085
 ipex_llm/transformers/models/bloom.py,sha256=IfR1rEwQb157lY2yIBQmrsS185jsBpKhgPYXEeLDQVQ,8971
-ipex_llm/transformers/models/chatglm.py,sha256=crFSh7Df1xSpND27PPBtuDUOzT1aniNjW7xMHUiIcis,13743
-ipex_llm/transformers/models/chatglm2.py,sha256=LVpz3sFOtkeKGW7rahWid_-242TIPwj_r3SFTzzT2OY,31837
+ipex_llm/transformers/models/chatglm.py,sha256=WSkrLqEQ11uGaXOD6YjPilXaPCcj0kwbPT9Om7UVyMw,14638
+ipex_llm/transformers/models/chatglm2.py,sha256=InWivnCKv3UdhV1YVSoKXJxIz7VeV1AuGl4X_OOnoVc,31844
 ipex_llm/transformers/models/chatglm2_32k.py,sha256=ch9Mw7T4haXcXMgqqubIi-mIQvlsdZ8gw6RhSbaUrao,8697
 ipex_llm/transformers/models/cohere.py,sha256=k0o3drmOx_153hTn6Kd9x3SpM_gAj3HeliV_Ypb13a0,20978
 ipex_llm/transformers/models/decilm.py,sha256=oAKyfB2_9GWheuqi3SyQXCBcRd6ixr6jeuYhN1z_d6A,8654
 ipex_llm/transformers/models/falcon.py,sha256=f5BzMbv4E-R5Pete8zBscbgiueXGIaWGs-5RbcMlUo4,33549
 ipex_llm/transformers/models/gemma.py,sha256=ZMn_BizM1ekqZ3erJep8L_QNLSEDgJNrUm1hEJWsQLQ,12310
 ipex_llm/transformers/models/gptbigcode.py,sha256=93l2PRLk1aLEhCGpio_7Y93amALS4SPrD5VXWiRl6hs,4342
 ipex_llm/transformers/models/gptj.py,sha256=TTIx461X2nOcIkrAcZhEf7d7mjJ3yvEC9KLVc1-hrpc,17973
 ipex_llm/transformers/models/gptneox.py,sha256=MVVdTbxV2oGzpCCzBMUy6oysVlnMtohJkl7SiC0xMAA,6219
 ipex_llm/transformers/models/internlm.py,sha256=mHyKQswtAHpT8R44gVvH7N57jjbk_GNtxjZWJy7ioog,11647
-ipex_llm/transformers/models/llama.py,sha256=gI_oFNCw7zg24YP5fgDHCsq9Yy-pZy1i3kLFWcADEwc,101985
+ipex_llm/transformers/models/llama.py,sha256=RQsPJJIXXw_P7SRfa5BfjkEBHACpBV-Hb0JDcve3SRY,108673
 ipex_llm/transformers/models/mistral.py,sha256=wT9ojpt1AisVpAfENDbAVFhCsIqXKOo4CppdwWIb9r0,54855
 ipex_llm/transformers/models/mixtral.py,sha256=dcat_zQLYsQ04Akc1HfZ9AnuzyhjJccPdOR-UiuIcoU,27151
 ipex_llm/transformers/models/mpt.py,sha256=z02NwHogJZVh-Mk4sYoIzR90SFIKhoNN_-ifsD907TQ,9540
 ipex_llm/transformers/models/phi.py,sha256=7TG4NZrQY7L8ONeYv7Rav1-ogFtQl4vd_cl5GndUmcE,7668
-ipex_llm/transformers/models/phi3.py,sha256=NgqGGystj8aDLhdka4HZ7cBicW2Cl7hnrFIDGpaTSLs,14199
+ipex_llm/transformers/models/phi3.py,sha256=PVWI-xKZMWr3qFLs_FTnwvxay4qMcnU-7WK9dvc9450,11908
 ipex_llm/transformers/models/phixtral.py,sha256=4B_2iE26GlzTVdaemd6mwYQ8mp4Yo4Yq9DgSFkF0yvc,6268
 ipex_llm/transformers/models/qwen.py,sha256=VHaxAkCd2BxQwfKYbofPnrSgppcNeTbDLKT_K7pLrzQ,32210
 ipex_llm/transformers/models/qwen2.py,sha256=3QRW9-km30lfyzfNVFIWmy6Gqm6o-dis7wDdUCvGgqs,37312
-ipex_llm/transformers/models/qwen2_moe.py,sha256=xO4aGuwdu9QP4lmbPrH5VqFUx3atC__0URXNzbpWEiw,38484
+ipex_llm/transformers/models/qwen2_moe.py,sha256=QQjr5ZMsGg8CUg7hA_WT2ZSEhRRn-vcVLX_pr_foJQk,38469
 ipex_llm/transformers/models/qwen_vl.py,sha256=hU7AKxdlEuFgHFguVH_NmUjkchcQ2UxwDoQPjvuXo4o,11712
 ipex_llm/transformers/models/rwkv4.py,sha256=Kzu6QlEi0KDXiJrfoZ71TI_D2nju2-sOeaKSZqdJz8U,6135
 ipex_llm/transformers/models/rwkv5.py,sha256=nNtWQROVAUc82SClzHrbaYVsr6CALnlVos0I2TX0YUc,10722
 ipex_llm/transformers/models/stablelm.py,sha256=obstiFzu-QoSEux7Mqfvzv5rQBeHpEaqFMir5dw-hLc,20911
 ipex_llm/transformers/models/starcoder2.py,sha256=mGmsVfjOhezAiB2xmQRwUSb_uvI1ejvQBwTpMcNJRZ8,8805
-ipex_llm/transformers/models/utils.py,sha256=QPDRZozvcFh3SBln_XqZjtG5J7eKg87ADYvOjZ2xlI8,19638
+ipex_llm/transformers/models/utils.py,sha256=AZU3_sbaVLb6UP_lCyKsXi84o6dBVhaEcuuCyUt0rRg,17396
 ipex_llm/transformers/models/yuan.py,sha256=eRKyROYIPWpn8e9AmIK0V0XiiyWJpj8PekB_pihTfQU,20200
 ipex_llm/utils/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/utils/benchmark_util.py,sha256=cI04QCUOR7ZD71sUiuFdbOjaujMDd7rAdybunNcMesc,258647
 ipex_llm/utils/convert_chatglm.py,sha256=YLbpJIbqnQOd8aJSijG5q4xBudNi_QR5sYVjCtYoVkY,18074
 ipex_llm/utils/convert_util.py,sha256=X1eLTdF9crlca6jPEQKymEITRx_57i_87dhl1htPEhc,72612
 ipex_llm/utils/glibc_checker.py,sha256=bm6kN6gbpA7GKtnUgsCE6K16iZZyil-Ylp55SoRvHG8,2093
 ipex_llm/utils/ipex_importer.py,sha256=sZro19_QZGr7oKiTq4P_i0CMUrDFlQkc7Ple9mV38CA,2477
@@ -177,14 +177,14 @@
 ipex_llm/utils/common/log4Error.py,sha256=8UgIpEJYQasQO4gMOWO22nsOgr14w1emAJy4ts1VOb0,1763
 ipex_llm/vllm/__init__.py,sha256=zBSG6nzrVF5QnpR6_f7kPhBFeowTE9gaZ7D5m98E7_w,585
 ipex_llm/vllm/ipex_llm_gpu_executor.py,sha256=pY-8XxRRX1_9MTW0TUTidxHmjmXKGsvs1AIIVWU21yM,18514
 ipex_llm/vllm/model_convert.py,sha256=jbsUSUAeVHm24CokIiLdyv6ubd_HuCrN_pnF3cLhhWE,7208
 ipex_llm/vllm/engine/__init__.py,sha256=mzPVAyZdbvfzBQi-wxZh1sbme_NElPMmtrJ9C2zh8Us,747
 ipex_llm/vllm/engine/engine.py,sha256=mVuCyoTcCX7KnK819-8fL_rNAu05WF_gql6jEcZ9bn8,5941
 ipex_llm/vllm/entrypoints/openai/api_server.py,sha256=luEdC8lW0UZuFx_cWF13Yz7s1wUrvNhHnhAW_rHa1Ps,10564
-ipex_llm-2.1.0b20240515.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
-ipex_llm-2.1.0b20240515.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
-ipex_llm-2.1.0b20240515.dist-info/METADATA,sha256=X_a8QxkxZek9wlLy_K6308zC3uCK0zKb3LWd3rAoHlI,4835
-ipex_llm-2.1.0b20240515.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-ipex_llm-2.1.0b20240515.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
-ipex_llm-2.1.0b20240515.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
-ipex_llm-2.1.0b20240515.dist-info/RECORD,,
+ipex_llm-2.1.0b20240516.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
+ipex_llm-2.1.0b20240516.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
+ipex_llm-2.1.0b20240516.dist-info/METADATA,sha256=Gi-55bxgkZobtySIFshMvERMIJObCwQoMagP5TFER-8,4965
+ipex_llm-2.1.0b20240516.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+ipex_llm-2.1.0b20240516.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
+ipex_llm-2.1.0b20240516.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
+ipex_llm-2.1.0b20240516.dist-info/RECORD,,
```

