# Comparing `tmp/shared_ndarray2-2.0.0.post0.tar.gz` & `tmp/shared_ndarray2-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shared_ndarray2-2.0.0.post0.tar", max compression
+gzip compressed data, was "shared_ndarray2-2.0.1.tar", max compression
```

## Comparing `shared_ndarray2-2.0.0.post0.tar` & `shared_ndarray2-2.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1097 2022-02-09 23:14:29.416983 shared_ndarray2-2.0.0.post0/LICENSE
--rw-r--r--   0        0        0     6169 2024-05-16 22:36:26.194629 shared_ndarray2-2.0.0.post0/README.md
--rw-r--r--   0        0        0     1004 2024-05-16 22:40:47.971162 shared_ndarray2-2.0.0.post0/pyproject.toml
--rw-r--r--   0        0        0      294 2024-05-15 23:09:58.643475 shared_ndarray2-2.0.0.post0/shared_ndarray2/__init__.py
--rw-r--r--   0        0        0       53 2023-01-12 21:23:59.165842 shared_ndarray2-2.0.0.post0/shared_ndarray2/py.typed
--rw-r--r--   0        0        0    10934 2024-05-15 23:11:24.167635 shared_ndarray2-2.0.0.post0/shared_ndarray2/shared_ndarray.py
--rw-r--r--   0        0        0      166 2024-05-15 23:13:49.007906 shared_ndarray2-2.0.0.post0/shared_ndarray2/version.py
--rw-r--r--   0        0        0     7081 1970-01-01 00:00:00.000000 shared_ndarray2-2.0.0.post0/setup.py
--rw-r--r--   0        0        0     7100 1970-01-01 00:00:00.000000 shared_ndarray2-2.0.0.post0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2022-02-09 23:14:29.416983 shared_ndarray2-2.0.1/LICENSE
+-rw-r--r--   0        0        0     6169 2024-05-16 22:36:26.194629 shared_ndarray2-2.0.1/README.md
+-rw-r--r--   0        0        0      998 2024-05-16 23:10:55.946877 shared_ndarray2-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      315 2024-05-16 23:09:31.790691 shared_ndarray2-2.0.1/shared_ndarray2/__init__.py
+-rw-r--r--   0        0        0       53 2023-01-12 21:23:59.165842 shared_ndarray2-2.0.1/shared_ndarray2/py.typed
+-rw-r--r--   0        0        0    10934 2024-05-15 23:11:24.167635 shared_ndarray2-2.0.1/shared_ndarray2/shared_ndarray.py
+-rw-r--r--   0        0        0      166 2024-05-15 23:13:49.007906 shared_ndarray2-2.0.1/shared_ndarray2/version.py
+-rw-r--r--   0        0        0     7075 1970-01-01 00:00:00.000000 shared_ndarray2-2.0.1/setup.py
+-rw-r--r--   0        0        0     7094 1970-01-01 00:00:00.000000 shared_ndarray2-2.0.1/PKG-INFO
```

### Comparing `shared_ndarray2-2.0.0.post0/LICENSE` & `shared_ndarray2-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shared_ndarray2-2.0.0.post0/README.md` & `shared_ndarray2-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `shared_ndarray2-2.0.0.post0/pyproject.toml` & `shared_ndarray2-2.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "shared-ndarray2"
-version = "2.0.0.post0"
+version = "2.0.1"
 description = "Interface for NumPy ndarray using multiprocessing SharedMemory"
 authors = ["Randall Pittman <randallpittman@outlook.com>"]
 license = "MIT"
 homepage = "https://gitlab.com/osu-nrsg/shared-ndarray2"
 repository = "https://gitlab.com/osu-nrsg/shared-ndarray2"
 keywords = ["numpy", "shared_memory", "ndarray"]
 classifiers = [
```

### Comparing `shared_ndarray2-2.0.0.post0/shared_ndarray2/shared_ndarray.py` & `shared_ndarray2-2.0.1/shared_ndarray2/shared_ndarray.py`

 * *Files identical despite different names*

### Comparing `shared_ndarray2-2.0.0.post0/setup.py` & `shared_ndarray2-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.21.1,<2.0.0', 'single-version>=1.5.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'shared-ndarray2',
-    'version': '2.0.0.post0',
+    'version': '2.0.1',
     'description': 'Interface for NumPy ndarray using multiprocessing SharedMemory',
     'long_description': '# shared-ndarray2  <!-- omit in toc -->\n\n`SharedNDArray` encapsulates a NumPy `ndarray` interface for using shared memory in\nmultiprocessing, using `multiprocessing.shared_memory` in Python 3.8+.\n\n- [Quick Start](#quick-start)\n- [Requirements](#requirements)\n- [Similar Projects](#similar-projects)\n- [Usage](#usage)\n  - [Creation](#creation)\n    - [`SharedNDArray()`](#sharedndarray)\n    - [`SharedNDArray.from_shape()` or `shared_ndarray.from_shape()`](#sharedndarrayfrom_shape-or-shared_ndarrayfrom_shape)\n    - [`SharedNDArray.from_array()` or `shared_ndarray.from_array()`](#sharedndarrayfrom_array-or-shared_ndarrayfrom_array)\n  - [Using like `np.ndarray`](#using-like-npndarray)\n  - [Releasing Shared Memory](#releasing-shared-memory)\n  - [`.lock` attribute](#lock-attribute)\n  - [Typed SharedNDArray](#typed-sharedndarray)\n\n## Quick Start\n\n```python\nimport multiprocessing\nfrom multiprocessing.managers import SharedMemoryManager\n\nimport numpy as np\n\nfrom shared_ndarray2 import SharedNDArray\n\n\ndef process_data(arr: SharedNDArray):\n    # Work with data\n    arr[:] += 1\n\n\nwith SharedMemoryManager() as mem_mgr:\n    arr = SharedNDArray.from_array(mem_mgr, np.arange(1024))\n    p = multiprocessing.Process(target=process_data, args=(arr,))\n    p.start()\n    p.join()\n    assert np.all(arr[:] == np.arange(1, 1025))\n```\n\n## Requirements\n\n- Python 3.8+\n- NumPy 1.21+\n\n## Similar Projects\n\n- [SharedArray](https://pypi.org/project/SharedArray/) - POSIX-only. Quite a different\n  paradigm, uses pre-Python 3.8 memory-sharing constructs, requires building a C module\n  with `gcc`.\n- [shared-ndarray](https://pypi.org/project/shared-ndarray/) - POSIX-only. Similar (uses\n  NumPy ndarray `buffer` arg), uses pre-Python 3.8 memory-sharing constructs (requires\n  `posix_ipc`).\n\n## Usage\n\n### Creation\n\nThere are three methods for constructing a `SharedNDArray`.\n\n#### `SharedNDArray()`\n\nTo create a `SharedNDArray` object from existing shared memory that represents a NumPy\narray, use the regular constructor providing _shape_ and _dtype_, either with an existing\n`multiprocessing.SharedMemory` object or the name of one:\n\n```python\nshm = SharedMemory(create=True, size=1024)\narr = SharedNDArray(shm, (1024,), np.uint8)\n# -or-\narr = SharedNDArray(shm.name, (1024,), np.uint8)\n```\n\n#### `SharedNDArray.from_shape()` or `shared_ndarray.from_shape()`\n\nThis method allocates shared memory managed by a SharedMemoryManager to represent a NumPy\n`ndarray` with some _shape_ and _dtype_.\n\n```python\nwith SharedMemoryManager as mem_mgr:\n    arr = SharedNDArray.from_shape(mem_mgr, (3, 1024, 1024), dtype=np.uint16)\n    # ... Use arr with e.g. multiprocessing.Pool or multiprocess.Process\n    # ... Be sure process instances join/terminate before exiting SharedMemoryManager context manager\n```\n\n<div style="font-size: small; margin-left: 4em">\n\nNote: _`shared_ndarray.from_shape()` is a standlone function and correctly types the\n`SharedNDArray`, whereas the classmethod might (in mypy) or might not (in pyright)_\n\n</div>\n\n#### `SharedNDArray.from_array()` or `shared_ndarray.from_array()`\n\nThis method allocates shared memory managed by a SharedMemoryManager to represent a some\nprovided NumPy `ndarray` and copies that ndarray into the shared memory\n\n```python\nx = np.arange(100.0).reshape(2, 2, 25)\nwith SharedMemoryManager as mem_mgr:\n    arr = SharedNDArray.from_array(mem_mgr, x)\n    assert np.all(arr[:] == x[:])\n    # ... Use arr as above...\n```\n\n<div style="font-size: small; margin-left: 4em">\n\nNote: _`shared_ndarray.from_array()` is a standlone function and correctly types the\n`SharedNDArray`, whereas the classmethod might (in mypy) or might not (in pyright)_\n\n</div>\n\n### Using like `np.ndarray`\n\nThe point of `SharedNDArray` is to remove the boilerplate of creating shared memory,\npassing around shapes and dtypes and reconstructing `np.ndarray` objects. `SharedNDArray`\ndoes this last step with its `.get()` method, which creates a `np.ndarray` on-the-fly\nusing the shared memory buffer. The `__getitem__()` and `__setitem__()` methods use the\n`.get()` method to get the np.ndarray to access the data, so multi-dimensional indexing\nand slicing work the same as with an `ndarray`. Other `np.ndarray` methods are not\ndirectly implemented but may be accessed by first calling `.get()`, e.g.\n`arr.get().mean()`.\n\n### Releasing Shared Memory\n\n`SharedNDArray` implements a `__del__()` method that calls the\n[`.close()`](https://docs.python.org/3/library/multiprocessing.shared_memory.html#multiprocessing.shared_memory.SharedMemory.close)\nmethod on the `SharedMemory` when the instance is destroyed (i.e. at process exit). When\nthe shared memory is unlinked in the parent process (either manually with\n[`shm.unlink()`](https://docs.python.org/3/library/multiprocessing.shared_memory.html#multiprocessing.shared_memory.SharedMemory.unlink)\nor by exiting a `SharedMemoryManager` context manager) the shared_memory is properly\nreleased. However if a sub-process is not joined or terminated before the shared memory is\nunlinked a warning will be emitted about "`leaked shared_memory objects to clean up at\nshutdown`".\n\n### `.lock` attribute\n\nThe `__init__()`, `from_shape()`, and `from_array()` methods may be given a `lock=True`\nargument that will also create a `multiprocessing.Lock` object and include it in the\n`SharedNDArray`, accesible as the `.lock` attribute. It should be noted, however, that it\ndoesn\'t work well to pass a `multiprocessing.Lock` as an argument to a\n`multiprocessing.Pool` function, for reasons described\n[here](https://stackoverflow.com/questions/25557686/python-sharing-a-lock-between-processes#comment72803059_25558333).\nThus by default `.lock` is set to `None`.\n\n### Typed SharedNDArray\n\n`SharedNDArray` is able to be typed with NumPy types. When using the `from_array()`\nconstructor, it is also able to inherit the type of the `ndarray` if it is typed using\n`numpy.typing.NDArray` (new in NumPy 1.21). Typing information does not pass through with\nslicing (`__getitem__`), however.\n\n```python\nx: npt.NDArray[np.int_] = np.arange(1024)\narr = SharedNDArray(mem_mgr, x)  # type of x is SharedNDArray[int_]\narr2 = arr[:]  # arr2 is typing.Any\n```\n',
     'author': 'Randall Pittman',
     'author_email': 'randallpittman@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/osu-nrsg/shared-ndarray2',
```

### Comparing `shared_ndarray2-2.0.0.post0/PKG-INFO` & `shared_ndarray2-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shared-ndarray2
-Version: 2.0.0.post0
+Version: 2.0.1
 Summary: Interface for NumPy ndarray using multiprocessing SharedMemory
 Home-page: https://gitlab.com/osu-nrsg/shared-ndarray2
 License: MIT
 Keywords: numpy,shared_memory,ndarray
 Author: Randall Pittman
 Author-email: randallpittman@outlook.com
 Requires-Python: >=3.8,<4.0
```

