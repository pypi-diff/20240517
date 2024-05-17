# Comparing `tmp/globalcache-0.2.0.tar.gz` & `tmp/globalcache-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globalcache-0.2.0.tar", last modified: Fri Feb 23 07:48:42 2024, max compression
+gzip compressed data, was "globalcache-0.2.1.tar", last modified: Fri May 17 04:52:14 2024, max compression
```

## Comparing `globalcache-0.2.0.tar` & `globalcache-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-02-23 07:48:42.437792 globalcache-0.2.0/
--rw-rw-rw-   0        0        0     1086 2024-01-06 07:57:35.000000 globalcache-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0     4017 2024-02-23 07:48:42.436790 globalcache-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3485 2024-02-23 07:33:00.000000 globalcache-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-02-23 07:48:42.414631 globalcache-0.2.0/globalcache/
--rw-rw-rw-   0        0        0     2052 2024-02-22 08:22:03.000000 globalcache-0.2.0/globalcache/__init__.py
--rw-rw-rw-   0        0        0    28260 2024-02-23 07:43:37.000000 globalcache-0.2.0/globalcache/cache.py
-drwxrwxrwx   0        0        0        0 2024-02-23 07:48:42.436790 globalcache-0.2.0/globalcache.egg-info/
--rw-rw-rw-   0        0        0     4017 2024-02-23 07:48:42.000000 globalcache-0.2.0/globalcache.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2024-02-23 07:48:42.000000 globalcache-0.2.0/globalcache.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-23 07:48:42.000000 globalcache-0.2.0/globalcache.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-01-14 05:47:30.000000 globalcache-0.2.0/globalcache.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-02-23 07:48:42.000000 globalcache-0.2.0/globalcache.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      606 2024-02-23 07:47:17.000000 globalcache-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-23 07:48:42.437792 globalcache-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      582 2024-02-23 07:46:52.000000 globalcache-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-23 07:48:42.435790 globalcache-0.2.0/tests/
--rw-rw-rw-   0        0        0    12253 2024-02-23 07:24:42.000000 globalcache-0.2.0/tests/test.py
--rw-rw-rw-   0        0        0      315 2024-02-23 07:08:22.000000 globalcache-0.2.0/tests/test2.py
--rw-rw-rw-   0        0        0      329 2024-02-23 05:41:37.000000 globalcache-0.2.0/tests/test_import.py
--rw-rw-rw-   0        0        0      332 2024-02-23 05:42:21.000000 globalcache-0.2.0/tests/test_import2.py
+drwxrwxrwx   0        0        0        0 2024-05-17 04:52:14.817644 globalcache-0.2.1/
+-rw-rw-rw-   0        0        0     1086 2024-01-06 07:57:35.000000 globalcache-0.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     4074 2024-05-17 04:52:14.816638 globalcache-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3542 2024-03-10 09:09:17.000000 globalcache-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 04:52:14.806134 globalcache-0.2.1/globalcache/
+-rw-rw-rw-   0        0        0     2083 2024-04-04 06:07:34.000000 globalcache-0.2.1/globalcache/__init__.py
+-rw-rw-rw-   0        0        0    31059 2024-04-04 06:06:05.000000 globalcache-0.2.1/globalcache/cache.py
+drwxrwxrwx   0        0        0        0 2024-05-17 04:52:14.816133 globalcache-0.2.1/globalcache.egg-info/
+-rw-rw-rw-   0        0        0     4074 2024-05-17 04:52:14.000000 globalcache-0.2.1/globalcache.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2024-05-17 04:52:14.000000 globalcache-0.2.1/globalcache.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 04:52:14.000000 globalcache-0.2.1/globalcache.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-01-14 05:47:30.000000 globalcache-0.2.1/globalcache.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-05-17 04:52:14.000000 globalcache-0.2.1/globalcache.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      606 2024-05-17 04:48:43.000000 globalcache-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 04:52:14.817644 globalcache-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      634 2024-04-09 04:43:33.000000 globalcache-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 04:52:14.815133 globalcache-0.2.1/tests/
+-rw-rw-rw-   0        0        0    12934 2024-04-04 05:26:20.000000 globalcache-0.2.1/tests/test.py
+-rw-rw-rw-   0        0        0      296 2024-03-10 10:02:45.000000 globalcache-0.2.1/tests/test2.py
+-rw-rw-rw-   0        0        0      321 2024-03-10 10:10:02.000000 globalcache-0.2.1/tests/test_import.py
+-rw-rw-rw-   0        0        0      327 2024-03-10 10:14:47.000000 globalcache-0.2.1/tests/test_import2.py
```

### Comparing `globalcache-0.2.0/LICENSE.txt` & `globalcache-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `globalcache-0.2.0/PKG-INFO` & `globalcache-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalcache
-Version: 0.2.0
+Version: 0.2.1
 Summary: Global caching for iPython and Spyder
 Author-email: John Huang <johnzilla76@gmail.com>
 Project-URL: Homepage, https://github.com/johnh865/globalcache
 Project-URL: Issues, https://github.com/johnh865/globalcache/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -65,15 +65,15 @@
     >>> @gcache.decorate(reset=True)
     >>> def func1(*args, **kwargs):
     >>>    ....
 
 Clear out cache from globals():
 
     >>> gcache.reset()
-	
+
 
 Set limitations on how many results we can store at a time:
 
     >>> @gcache.decorate(size_limit=5)
     >>> def func2(*args, **kwargs):
     >>>     ...
 
@@ -93,51 +93,51 @@
 
     >>> gcache.delete_shelve()
     
 
 
 By default, results are saved in the current working directory in a folder
 called `.globalcache/`. The default can be changed using:
-	
-	>>> gcache.init(globals(), save_dir='/p/folder1/path_to_new_directory')
-	
-
+    
+    >>> gcache.init(globals(), save_dir='/p/folder1/path_to_new_directory')
+    
+    
 Caching an if-block
 --------------------
 
 globalcache can cache a variable and skip an expensive block of code. 
 	
 Store a parameter with an if block:
     
     >>> var1 = gcache.var('my-param')
     >>> if var1.not_cached:
     >>>     out = expensive_function()
     >>>     var1.set(out)
     >>> out = var1.get()
-	
-Results can be cached dependent on the change of other variables:
 
-	>>> var2 = gcache.var('param2', args=(args1, args2),
-	>>>                   kwargs=dict2, save=False, size_limit=None)
-	>>> if var2.not_cached:
-	>>> 	out = expensive_function()
-	>>>		var2.set(out)
-	>>> out = var2.get()
-	
+Results can be cached dependent on the change of other variables:
+    
+    >>> var2 = gcache.var('param2', args=(args1, args2),
+    >>>                   kwargs=dict2, save=False, size_limit=None)
+    >>> if var2.not_cached:
+    >>>     out = expensive_function()
+    >>>     var2.set(out)
+    >>> out = var2.get()
+    
 
 Disabling the globalcache
 -------------------------
 
 Force disable the globalcache:
 
-	>>> import globalcache
-	>>> globalcache.Settings.disable = True
-	
-	
-	
+    >>> import globalcache
+    >>> globalcache.Settings.disable = True
+    
+    
+    
 Dealing with Unhashable Arguments
 ---------------------------------
 If your function relies on unhashable arguments, there are various
 strategies. For example, you can associate unhashable
 arguments with hashable parameters. For example:
 
     >>> dict1 = {'a': [1,2,3],
```

### Comparing `globalcache-0.2.0/README.md` & `globalcache-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     >>> @gcache.decorate(reset=True)
     >>> def func1(*args, **kwargs):
     >>>    ....
 
 Clear out cache from globals():
 
     >>> gcache.reset()
-	
+
 
 Set limitations on how many results we can store at a time:
 
     >>> @gcache.decorate(size_limit=5)
     >>> def func2(*args, **kwargs):
     >>>     ...
 
@@ -79,51 +79,51 @@
 
     >>> gcache.delete_shelve()
     
 
 
 By default, results are saved in the current working directory in a folder
 called `.globalcache/`. The default can be changed using:
-	
-	>>> gcache.init(globals(), save_dir='/p/folder1/path_to_new_directory')
-	
-
+    
+    >>> gcache.init(globals(), save_dir='/p/folder1/path_to_new_directory')
+    
+    
 Caching an if-block
 --------------------
 
 globalcache can cache a variable and skip an expensive block of code. 
 	
 Store a parameter with an if block:
     
     >>> var1 = gcache.var('my-param')
     >>> if var1.not_cached:
     >>>     out = expensive_function()
     >>>     var1.set(out)
     >>> out = var1.get()
-	
-Results can be cached dependent on the change of other variables:
 
-	>>> var2 = gcache.var('param2', args=(args1, args2),
-	>>>                   kwargs=dict2, save=False, size_limit=None)
-	>>> if var2.not_cached:
-	>>> 	out = expensive_function()
-	>>>		var2.set(out)
-	>>> out = var2.get()
-	
+Results can be cached dependent on the change of other variables:
+    
+    >>> var2 = gcache.var('param2', args=(args1, args2),
+    >>>                   kwargs=dict2, save=False, size_limit=None)
+    >>> if var2.not_cached:
+    >>>     out = expensive_function()
+    >>>     var2.set(out)
+    >>> out = var2.get()
+    
 
 Disabling the globalcache
 -------------------------
 
 Force disable the globalcache:
 
-	>>> import globalcache
-	>>> globalcache.Settings.disable = True
-	
-	
-	
+    >>> import globalcache
+    >>> globalcache.Settings.disable = True
+    
+    
+    
 Dealing with Unhashable Arguments
 ---------------------------------
 If your function relies on unhashable arguments, there are various
 strategies. For example, you can associate unhashable
 arguments with hashable parameters. For example:
 
     >>> dict1 = {'a': [1,2,3],
```

### Comparing `globalcache-0.2.0/globalcache/__init__.py` & `globalcache-0.2.1/globalcache/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,8 +87,9 @@
     
 """
 
 
 
 
 
-from globalcache.cache import Cache, Settings, CacheError, gcache
+from globalcache.cache import (
+    Cache, Settings, CacheError, gcache, reset, delete_shelves)
```

### Comparing `globalcache-0.2.0/globalcache/cache.py` & `globalcache-0.2.1/globalcache/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         Maximum size of cache for each cached variable. Set SIZE_LIMIT <= 0
         for unlimited length. 
         Set None for default length.
     save_dir : str
         Directory path of shelve cache on disc.
         
     """
-    global_cache_name = ''
+    global_cache_name = DEFAULT_GLOBAL_CACHE_NAME
     disable = DEFAULT_DISABLE
     size_limit = None
     save_dir = ''
 
 
 # class Environ:
 #     """Read any environmental variables."""
@@ -117,15 +117,21 @@
 
 class CacheError(Exception):
     pass
 
 
 
 class LimitDict(OrderedDict):
-    """Dictionary with limited size."""
+    """Dictionary with limited size.
+    
+    Attributes
+    ----------
+    size_limit : int
+        Max length of dict. You can re-set this on the fly.
+    """
     def __init__(self, *args, _size_limit: int=None, **kwargs):
         self.size_limit = _size_limit
         super().__init__(*args, **kwargs)
         self._check_size_limit()
     
     
     def __setitem__(self, key, value):
@@ -138,14 +144,90 @@
             while len(self) > self.size_limit:
                 self.popitem(last=False)
                 
 CacheValue = TypeVar('CacheValue')
 CacheDict = TypeVar('CacheDict', bound=dict[str, LimitDict[str, CacheValue] ])
 
 
+class _GlobalSingleton:
+    """A global object stored in globals() to coordinate the cache.
+    
+    Attributes
+    ----------
+    caches : dict[Cache]
+        Repository of all Caches initialized so far. 
+    global_dict : CacheDict
+        Dictionary of 
+    """
+    def __init__(self, gdict: dict, name: str=''):
+        self.caches = {}
+        self.global_dict = {}
+        if name == '':
+            name = Settings.global_cache_name
+        
+        gdict[name] = self
+        
+
+        self.update(gdict, name)
+    
+    
+    def update(self, gdict: dict, name: str=''):
+        
+        if name == '':
+            name = Settings.global_cache_name
+        
+        if name in gdict:
+            logger.debug('GlobalCache %r found in globals().', name)
+            self.myself = gdict[name]    
+            self.caches = self.myself.caches
+            global_dict1 = self.myself.global_dict
+            self.global_dict.update(global_dict1)
+            
+        else:
+            logger.debug('GlobalCache %r not found', name )
+            if gdict['__name__'] == '__main__':
+                logger.debug('__main__ found.')
+                gdict[name] = self
+
+        return self
+    
+    
+    def reset(self):
+        cache : Cache
+        for name, cache in self.caches.items():
+            cache.reset()
+            
+    def delete_shelve(self):
+        cache : Cache
+        for name, cache in self.caches.items():
+            cache.delete_shelve()
+            
+    def set_size_limit(self, size_limit: int):
+        cache: Cache
+        for cache in self.caches.values():
+            cache.set_size_limit(size_limit)
+            
+            
+    
+    
+    
+            
+            
+# Initialize the singleton.
+global_singleton = _GlobalSingleton(globals())
+
+def reset():
+    global_singleton.reset()
+    
+def delete_shelves():
+    global_singleton.delete_shelve()
+    
+def set_global_size_limit(size_limit: int):
+    global_singleton.set_size_limit(size_limit)
+
 
 class Cache:
     """Global cache to cache values in ipython session.
     
     Parameters
     ----------
     g : dict
@@ -154,34 +236,36 @@
         Name of dictionary stored in globals(). 
         Defaults to `DEFAULT_GLOBAL_CACHE_NAME`.
     reset : bool, optional
         Force reset of globalcache. The default is False.
         
     """    
     
-    cache : CacheDict
     _global_vars : set[str]
     size_limit : int
 
     def __init__(self,
                  g: dict, 
-                 name: str=None, 
+                 name: str='', 
                  reset: bool=False,
                  size_limit: int=None,
                  save_dir='',
                  ):
         self._globals = g
         self.name = name
         logger.debug('Creating cache %s', self)
         
-        if name is None:
-            name = DEFAULT_GLOBAL_CACHE_NAME        
-        
+        # if name is None:
+        #     name = DEFAULT_GLOBAL_CACHE_NAME    
+            
+        # self.cdict = {}
         self.size_limit = size_limit
         self.save_dir = save_dir
+        self.is_main = False
+        self._is_main_found = False
         self._function_caches = set()
         self.set_globals(g, name, size_limit, save_dir)
         
         if reset:
             self.reset()
             
             
@@ -193,92 +277,67 @@
             gname = '...'
         out = f"Cache('{gname}','{self.name}')"
         return out
     
             
     def init(self,
             g: dict,
-            name: Union[str, None] = None, 
+            name: str = '', 
             size_limit: Union[int, None] = None,
             save_dir: str='',
             ):
+        """Call this to initialize gcache for each script it is imported into.
+        
+        >>> from globalcache import gcache
+        >>> gcache.init(globals())
+        
+        Parameters
+        ----------
+        g : dict
+            Input globals() here.
+        name : Union[str, None], optional
+            Name of cache's dictionary key in globals().
+            The default is None and will take the name '__GLOBAL_CACHE__'.
+        size_limit : Union[int, None], optional
+            Default max number of items to store in cache dictionary. The default is None.
+        save_dir : str, optional
+            Directory path to save data. By default this path is '.globalcache'.
+
+        Returns
+        -------
+        None.
+
+        """
         self.set_globals(
             g=g, name=name,
             size_limit=size_limit, save_dir=save_dir)
-    
+        
     
     def set_globals(
             self, 
             g: dict,
-            name: Union[str, None] = None, 
+            name: str = '', 
             # reset: bool = False,
             size_limit: Union[int, None] = None,
             save_dir: str='',
             ):
         """Use this method to re-set the globals() dict for the cache.
-        This is needed to enable the cache from another script. 
-        
-        Example
-        -------
-        module1.py
-        
-        >>> from globalcache import Cache
-        >>> cache = Cache(globals())
-        
-        main.py
-        
-        >>> from module1 import cache
-        >>> cache.set_globals(globals())
         
+        Initialization are probably a random mix of outside of __main__ and not. 
         """
         
-        if name is None:
-            name = self.name
-        self.name = name
+        self.global_singleton = global_singleton.update(g, name=name)
+        module_name = g['__name__']
+        self.global_singleton.caches[module_name] = self
+        
         self.size_limit = size_limit
         self.save_dir = save_dir
-        
-        # if size_limit is None:
-        #     size_limit = Settings.SIZE_LIMIT
-        # if save_dir == '':
-        #     save_dir = Settings.SAVE_DIR
-        
-        logger.debug('Set globals for %r', self)
-        
-        if name in g:
-            logger.debug('Cache dict %s found in globals()', name)
-            cache : Cache
-            cache = g[name]
-            self.cdict = cache.cdict
-            # breakpoint()
-            # self._function_caches.update(cache._function_caches)
-            
-        else:
-            logger.debug('No cache dict %s found in globals()', name)
-            self.cdict = {}
-            # self._function_caches = set()      
-            
-            
-        
-
-            
-            
+                    
         self._function_cache_names  = {}
-            
-        # Make sure to set self into globals()
-        g[name] = self        
-        
-
-
-        self._globals = g
-        try:
-            self.is_main = g['__name__'] == '__main__'
-        except KeyError:
-            self.is_main = False
-            
+                        
         return
     
     
     def var(self,
             name: str, 
             args: tuple=(),
             kwargs: dict={}, 
@@ -401,15 +460,16 @@
             
         return func
     
 
     def reset(self):
         """Reset the global cache dict."""
         logger.debug('Resetting cache %s', self)
-        self.cdict.clear()
+        self.global_singleton.global_dict.clear()
+        # self.cdict.clear()
         for fun_cache in self._function_caches:
             fun_cache.reset()
         
         
     def delete_shelve(self):
         """Delete persistent shelve file data."""
         dir1  = self.save_dir
@@ -423,15 +483,16 @@
             fn_cache._is_first_run = True
         
         
         
     @property
     def module_names(self) -> list[str]:
         """Names of all cached modules."""
-        return list(self.cdict.keys())
+        cdict = self.global_singleton.global_dict
+        return list(cdict.keys())
     
     def module_names_short(self) -> list[str]:
         names = [splitext(basename(path))[0] for path in self.module_names]
         out = rename_duplicates(names)
         return out
     
     
@@ -440,14 +501,33 @@
         d = dict(zip(self.module_names, self.module_names_short()))
         return d[name]
     
     @property
     def function_caches(self) -> list['FunctionCache']:
         return list(self._function_caches)
     
+    
+    def print_status(self):
+        print('globals() is initialized in main scope:', self.is_main)
+        print('')
+        print('Cached functions list:')
+        for fcache in self.function_caches:
+            print(fcache)
+            print('Module = ', fcache.module)
+            print('Cached entries = ', len(fcache.fcache))
+            print('')
+        print('')       
+        
+        
+    def set_size_limit(self, size_limit: int):
+        self.size_limit = size_limit
+        for fn_cache in self.function_caches:
+            fn_cache.fcache.size_limit = size_limit
+            
+    
         
 def get_name(fn : Callable) -> str:
     """Create a name for a callable function."""
     # name = fn.__name__
     name = fn.__qualname__
     while True:
         try:
@@ -509,34 +589,35 @@
         Raised if you attempt to define a cache for a function multiple times.
 
     Attributes
     ----------
     
     shelve_name : str
         Name of file corresponding to shelve file storage.
-    fcache : dict
+    fcache : LimitDict
         Cache dictionary for function.
         
 
     """
-
+    fcache: LimitDict
     def __init__(self, cache: Cache,
                  fn : Callable,
                  size_limit: int,
                  save: bool,
                  name: str = '',
                  module: str = '',
                  ):
 
         # Initialize deafault settings
         if module == '':
             module = inspect.getsourcefile(fn)
         if name == '':
             name = get_name(fn)       
         size_limit = get_size_limit(size_limit)
+        
         self.size_limit = size_limit
         self.name = name
         self.save = save
         self.module = module        
         self._cache = cache
         self.fn = fn
         self._is_first_run = True
@@ -563,17 +644,20 @@
         return hash(self.module + '-' + self.name)
         
             
     def reinit_dicts(self):
         """Reinitialize dictionaries to make sure they are in the right
         globals() dict."""
         cache = self._cache
+        global_dict = cache.global_singleton.global_dict
         
         # Get module-level dictionary
-        self.module_dict = cache.cdict.setdefault(self.module, {})
+        # self.module_dict = cache.m
+        self.module_dict = global_dict.setdefault(self.module, {})
+        # self.module_dict = cache.cdict.setdefault(self.module, {})
         
         # Get argument-value dictionary
         self.fcache = self.module_dict.setdefault(
             self.name,
             LimitDict(_size_limit=self.size_limit)
             )
         
@@ -630,18 +714,18 @@
         self.reinit_dicts()
         
         if get_disable():
             logger.debug('Disable flag detected. Disabling cache.')
             return self.fn(*args, **kwargs)
         
         # globalcache will not work if globals() are not from __main__ script
-        if not self._cache.is_main:
-            warnings.warn('gcache has not yet been initialized with globals(). Cache is disabled')
-            logger.debug('globals() not set. Disabling cache.')
-            return self.fn(*args, **kwargs)
+        # if not self._cache.is_main:
+        #     logger.info('gcache has not yet been initialized with globals(). Cache is disabled')
+        #     logger.debug('globals() not set. Disabling cache.')
+        #     return self.fn(*args, **kwargs)
             
         
         # Initialize file persistence
         if self._is_first_run:
             self._is_first_run = False
             if self.save:
                 logger.debug('Initializing shelve for %s', name)
@@ -987,8 +1071,8 @@
         
         return self.is_cached
         
     
 # %% Create a cache here 
 
 
-gcache = Cache({})
+gcache = Cache(globals())
```

### Comparing `globalcache-0.2.0/globalcache.egg-info/PKG-INFO` & `globalcache-0.2.1/globalcache.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalcache
-Version: 0.2.0
+Version: 0.2.1
 Summary: Global caching for iPython and Spyder
 Author-email: John Huang <johnzilla76@gmail.com>
 Project-URL: Homepage, https://github.com/johnh865/globalcache
 Project-URL: Issues, https://github.com/johnh865/globalcache/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -65,15 +65,15 @@
     >>> @gcache.decorate(reset=True)
     >>> def func1(*args, **kwargs):
     >>>    ....
 
 Clear out cache from globals():
 
     >>> gcache.reset()
-	
+
 
 Set limitations on how many results we can store at a time:
 
     >>> @gcache.decorate(size_limit=5)
     >>> def func2(*args, **kwargs):
     >>>     ...
 
@@ -93,51 +93,51 @@
 
     >>> gcache.delete_shelve()
     
 
 
 By default, results are saved in the current working directory in a folder
 called `.globalcache/`. The default can be changed using:
-	
-	>>> gcache.init(globals(), save_dir='/p/folder1/path_to_new_directory')
-	
-
+    
+    >>> gcache.init(globals(), save_dir='/p/folder1/path_to_new_directory')
+    
+    
 Caching an if-block
 --------------------
 
 globalcache can cache a variable and skip an expensive block of code. 
 	
 Store a parameter with an if block:
     
     >>> var1 = gcache.var('my-param')
     >>> if var1.not_cached:
     >>>     out = expensive_function()
     >>>     var1.set(out)
     >>> out = var1.get()
-	
-Results can be cached dependent on the change of other variables:
 
-	>>> var2 = gcache.var('param2', args=(args1, args2),
-	>>>                   kwargs=dict2, save=False, size_limit=None)
-	>>> if var2.not_cached:
-	>>> 	out = expensive_function()
-	>>>		var2.set(out)
-	>>> out = var2.get()
-	
+Results can be cached dependent on the change of other variables:
+    
+    >>> var2 = gcache.var('param2', args=(args1, args2),
+    >>>                   kwargs=dict2, save=False, size_limit=None)
+    >>> if var2.not_cached:
+    >>>     out = expensive_function()
+    >>>     var2.set(out)
+    >>> out = var2.get()
+    
 
 Disabling the globalcache
 -------------------------
 
 Force disable the globalcache:
 
-	>>> import globalcache
-	>>> globalcache.Settings.disable = True
-	
-	
-	
+    >>> import globalcache
+    >>> globalcache.Settings.disable = True
+    
+    
+    
 Dealing with Unhashable Arguments
 ---------------------------------
 If your function relies on unhashable arguments, there are various
 strategies. For example, you can associate unhashable
 arguments with hashable parameters. For example:
 
     >>> dict1 = {'a': [1,2,3],
```

### Comparing `globalcache-0.2.0/pyproject.toml` & `globalcache-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "globalcache"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="John Huang", email="johnzilla76@gmail.com" },
 ]
 description = "Global caching for iPython and Spyder"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `globalcache-0.2.0/setup.py` & `globalcache-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,13 +8,14 @@
       name='globalcache',
       # version='0.1',   # May 14, 2021 update
        # version='0.1.1',   # Jan 7, 2024  update
        # version='0.1.2',   # Jan 8, 2024  update
        # version='0.1.4',   # Jan 13, 2024  update
        # version='0.1.5',   # Jan 13, 2024  update
         # version='0.1.6',   # Feb 15, 2024  update
-        version='0.2.0',   # Feb 22, 2024  update
+        # version='0.2.0',   # Feb 22, 2024  update
+        version='0.2.1',   # Apr 8, 2024  update
       packages=find_packages(
           include=["globalcache*"]
           ),
       zip_safe=False,
       )
```

### Comparing `globalcache-0.2.0/tests/test.py` & `globalcache-0.2.1/tests/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -472,25 +472,43 @@
     folder = os.path.dirname(__file__)
     path = os.path.join(folder, fname)
     
     with Capturing() as output1:
         runfile(filename=path, current_namespace=False)
     
     hello_count = sum(1 for line in output1 if line == 'hello')
+    
     assert hello_count == 3
     
     
     with Capturing() as output2:
         
         runfile(filename=path, current_namespace=True)
-        
+    
     for line in output2:
         assert line != 'hello'
     
         
+def test_importing():
+    """Test importing of  module and mixing of order when gcache is initialized."""
+    import spydercustomize
+    from spydercustomize import runfile
+    
+    fname = 'test_import2.py'
+    folder = os.path.dirname(__file__)
+    path = os.path.join(folder, fname)
+    with Capturing() as output1:
+        runfile(filename=path, current_namespace=False)
+    count = sum(1 for line in output1 if line == 'testfun1')
+    assert count == 2
+    
+    with Capturing() as output2:
+        runfile(filename=path, current_namespace=True)
+    count = sum(1 for line in output2 if line == 'testfun1')
+    assert count == 0
     
     
 # %% main
 if __name__ == '__main__':
     
     logging.basicConfig(level=logging.DEBUG)
     logger = logging.getLogger()
@@ -515,9 +533,11 @@
     
     test_unhashable()
     test_name()
 
     test_wraps()
     
     test_run_in_spyder()
+    test_importing()
+
```

