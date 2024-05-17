# Comparing `tmp/pyriak-0.1.0.tar.gz` & `tmp/pyriak-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriak-0.1.0.tar", max compression
+gzip compressed data, was "pyriak-0.2.0.tar", max compression
```

## Comparing `pyriak-0.1.0.tar` & `pyriak-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1083 2024-05-04 21:26:50.483291 pyriak-0.1.0/LICENSE
--rw-r--r--   0        0        0      883 2024-05-05 21:03:13.370848 pyriak-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7554 2024-05-04 21:26:50.484289 pyriak-0.1.0/README.md
--rw-r--r--   0        0        0     4800 2024-05-05 20:55:56.655692 pyriak-0.1.0/src/pyriak/__init__.py
--rw-r--r--   0        0        0     3380 2024-05-04 21:26:50.486289 pyriak-0.1.0/src/pyriak/_importer.py
--rw-r--r--   0        0        0     4575 2024-05-04 21:26:50.487290 pyriak-0.1.0/src/pyriak/entity.py
--rw-r--r--   0        0        0     4685 2024-05-04 21:26:50.488290 pyriak-0.1.0/src/pyriak/eventkey.py
--rw-r--r--   0        0        0     4001 2024-05-04 21:26:50.488290 pyriak-0.1.0/src/pyriak/events.py
--rw-r--r--   0        0        0      188 2024-05-04 21:26:50.490288 pyriak-0.1.0/src/pyriak/managers/__init__.py
--rw-r--r--   0        0        0    10028 2024-05-05 20:57:27.520842 pyriak-0.1.0/src/pyriak/managers/entitymanager.py
--rw-r--r--   0        0        0     3408 2024-05-04 21:26:50.491287 pyriak-0.1.0/src/pyriak/managers/statemanager.py
--rw-r--r--   0        0        0    19548 2024-05-04 21:26:50.492287 pyriak-0.1.0/src/pyriak/managers/systemmanager.py
--rw-r--r--   0        0        0     6422 2024-05-04 21:26:50.493286 pyriak-0.1.0/src/pyriak/query.py
--rw-r--r--   0        0        0     3542 2024-05-04 21:26:50.493286 pyriak-0.1.0/src/pyriak/space.py
--rw-r--r--   0        0        0     6015 2024-05-04 21:26:50.494285 pyriak-0.1.0/src/pyriak/system.py
--rw-r--r--   0        0        0     7992 1970-01-01 00:00:00.000000 pyriak-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-05-04 21:26:50.483291 pyriak-0.2.0/LICENSE
+-rw-r--r--   0        0        0      948 2024-05-17 03:34:47.669779 pyriak-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4002 2024-05-17 01:56:40.828708 pyriak-0.2.0/README.md
+-rw-r--r--   0        0        0     4476 2024-05-17 01:03:05.389730 pyriak-0.2.0/src/pyriak/__init__.py
+-rw-r--r--   0        0        0     3364 2024-05-15 05:27:35.698514 pyriak-0.2.0/src/pyriak/_importer.py
+-rw-r--r--   0        0        0     5265 2024-05-17 01:36:17.343647 pyriak-0.2.0/src/pyriak/entity.py
+-rw-r--r--   0        0        0     4565 2024-05-17 01:11:40.294812 pyriak-0.2.0/src/pyriak/eventkey.py
+-rw-r--r--   0        0        0     4691 2024-05-17 03:18:22.514876 pyriak-0.2.0/src/pyriak/events.py
+-rw-r--r--   0        0        0      188 2024-05-04 21:26:50.490288 pyriak-0.2.0/src/pyriak/managers/__init__.py
+-rw-r--r--   0        0        0    10388 2024-05-15 05:27:35.702513 pyriak-0.2.0/src/pyriak/managers/entitymanager.py
+-rw-r--r--   0        0        0     4002 2024-05-17 01:36:29.474375 pyriak-0.2.0/src/pyriak/managers/statemanager.py
+-rw-r--r--   0        0        0    18739 2024-05-17 01:41:58.456283 pyriak-0.2.0/src/pyriak/managers/systemmanager.py
+-rw-r--r--   0        0        0        0 2024-05-15 05:27:35.705512 pyriak-0.2.0/src/pyriak/py.typed
+-rw-r--r--   0        0        0     6473 2024-05-17 03:15:01.879124 pyriak-0.2.0/src/pyriak/query.py
+-rw-r--r--   0        0        0     3260 2024-05-17 03:07:55.524384 pyriak-0.2.0/src/pyriak/space.py
+-rw-r--r--   0        0        0     6048 2024-05-17 03:05:14.375655 pyriak-0.2.0/src/pyriak/system.py
+-rw-r--r--   0        0        0     4543 1970-01-01 00:00:00.000000 pyriak-0.2.0/PKG-INFO
```

### Comparing `pyriak-0.1.0/LICENSE` & `pyriak-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriak-0.1.0/pyproject.toml` & `pyriak-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [tool.poetry]
 name = "pyriak"
-version = "0.1.0"
+version = "0.2.0"
 description = "A lightweight implementation of Entity Component System architecture"
 authors = ["aatle <168398276+aatle@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.urls]
 Repository = "https://github.com/aatle/pyriak.git"
 Issues = "https://github.com/aatle/pyriak/issues"
 
 
+[tool.poetry.group.dev.dependencies]
+ruff = "^0.4.4"
+mypy = "^1.10.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.ruff]
 target-version = "py311"
@@ -40,12 +44,12 @@
   "RSE",
   "RET",
   "SLOT",
   "PERF",
   "RUF",
   # "FURB",
 ]
-ignore = ["SIM105", "FBT003"]
+ignore = ["SIM105"]
 
 [tool.ruff.lint.isort]
 lines-after-imports = 2
 combine-as-imports = true
```

### Comparing `pyriak-0.1.0/src/pyriak/__init__.py` & `pyriak-0.2.0/src/pyriak/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,45 +4,42 @@
   'Space',
   'System',
   'bind',
   'Entity',
   'EntityId',
   'Query',
   'subclasses',
+  'strict_subclasses',
   'key_functions',
   'set_key',
-  'NoKey',
-  'NoKeyType',
   'tagclass',
-  'Callback',
-  'dead_weakref',
+  'first',
 ]
 
 from collections.abc import (
-  Callable as _Callable,
   Generator as _Generator,
   MutableSequence as _MutableSequence,
 )
+from enum import Enum as _Enum
 from typing import (
   Any as _Any,
+  Literal as _Literal,
   TypeAlias as _TypeAlias,
   TypeVar as _TypeVar,
   overload as _overload,
 )
 from weakref import ref as _weakref
 
-from pyriak.eventkey import NoKey, NoKeyType, key_functions, set_key
-
 
 _TypeT = _TypeVar('_TypeT', bound=type)
 _T = _TypeVar('_T')
 _D = _TypeVar('_D')
 
 
-EventQueue: _TypeAlias = _MutableSequence[_Any]
+EventQueue: _TypeAlias = _MutableSequence[object]
 
 
 dead_weakref: _weakref[_Any] = _weakref(set())
 
 
 _get_subclasses = type.__subclasses__
 
@@ -69,23 +66,24 @@
   while stack:
     subclass = pop()
     yield subclass
     stack += get_subclasses(subclass)
   return cls
 
 
-def mro(obj: object) -> tuple[type, ...]:
-  """Return the method resolution order (MRO) of the object as a tuple.
-
-  It is the value of the __mro__ attribute of the object's class.
-  Note that if a class object is passed in, the mro of the metaclass is returned.
-
-  (equivalent to `type(obj).__mro__)`)
-  """
-  return type(obj).__mro__
+def strict_subclasses(cls: _TypeT, /) -> _Generator[_TypeT, None, _TypeT]:
+  """Same as subclasses, but does not yield the original class."""
+  get_subclasses = _get_subclasses
+  stack = get_subclasses(cls)
+  pop = stack.pop
+  while stack:
+    subclass = pop()
+    yield subclass
+    stack += get_subclasses(subclass)
+  return cls
 
 
 @_overload
 def tagclass(cls: _TypeT, /) -> _TypeT: ...
 @_overload
 def tagclass(
   name: str, bases: tuple[type, ...] = (), namespace: dict[str, _Any] = ..., /
@@ -133,36 +131,31 @@
     namespace.update(args[2])
   else:
     raise TypeError('tag() takes at most 3 arguments')
   cls = type(first, bases, namespace)  # required variable so dunder methods know cls
   return cls  # noqa: RET504
 
 
-class Callback:
-  """Built-in callback."""
+def first(arg: _T, *args: _Any) -> _T:  # noqa: ARG001
+  return arg
+
+
+class _Sentinel(_Enum):
+  SENTINEL = 1
 
-  def __init__(self, callback: _Callable[..., _Any], /, *args, **kwargs):
-    self.callback = callback
-    self.args = args
-    self.kwargs = kwargs
-
-  def __call__(self, /, *args, **kwargs):
-    """Execute self's callback. Return the return value of the callback.
-
-    Args are passed first, then self's args, then kwargs, and lastly, self's kwargs.
-    """
-    return self.callback(*args, *self.args, **kwargs, **self.kwargs)
+_SENTINEL = _Sentinel.SENTINEL
 
 
 # circular imports
 from pyriak import _importer  # noqa: E402
 from pyriak.entity import Entity, EntityId  # noqa: E402
+from pyriak.eventkey import key_functions, set_key  # noqa: E402
 from pyriak.query import Query  # noqa: E402
 from pyriak.space import Space  # noqa: E402
 from pyriak.system import System, bind  # noqa: E402
 
 
 _importer.install()  # install meta path finder for system initialization
 
 
 # cleanup namespace
-del _MutableSequence, _TypeVar, _weakref
+del _MutableSequence, _Enum, _Literal, _TypeVar, _weakref
```

### Comparing `pyriak-0.1.0/src/pyriak/_importer.py` & `pyriak-0.2.0/src/pyriak/_importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     lock_names.add(fullname)
     try:
       spec = _find_spec(fullname)
       if spec is None:
         return None
       loader = getattr(spec, 'loader', None)
       if loader is not None:
-        spec.loader = self.wrapper(loader)  # type: ignore
+        spec.loader = self.wrapper(loader)
       return spec
     finally:
       lock_names.remove(fullname)
 
 
 def _install(cls, /):
   """Install a finder at the front of sys.meta_path.
```

### Comparing `pyriak-0.1.0/src/pyriak/entity.py` & `pyriak-0.2.0/src/pyriak/entity.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __all__ = ['Entity']
 
 from collections.abc import Iterable
-from typing import TYPE_CHECKING, Any, NewType, TypeVar
+from typing import TYPE_CHECKING, NewType, TypeVar, overload
 from uuid import uuid4
 
-from pyriak import dead_weakref, subclasses
+from pyriak import _SENTINEL, dead_weakref, strict_subclasses, subclasses
 from pyriak.events import ComponentAdded, ComponentRemoved
 
 
 if TYPE_CHECKING:
   from weakref import ref as weakref
 
   from pyriak.managers import EntityManager
@@ -20,44 +20,44 @@
 _T = TypeVar('_T')
 _D = TypeVar('_D')
 
 
 class Entity:
   __slots__ = 'id', '_components', '_manager', '__weakref__'
 
-  def __init__(self, components: Iterable[Any] = (), /):
+  def __init__(self, components: Iterable[object] = (), /):
     self.id: EntityId = self.new_id()
     self._manager: weakref[EntityManager] = dead_weakref
-    comp_dict = {}
+    comp_dict: dict[type, object] = {}
     for comp in components:
       comp_type = type(comp)
       if comp_type in comp_dict and (
           (other := comp_dict[comp_type]) is comp or other == comp):
         continue
       comp_dict[comp_type] = comp
-    self._components: dict[type, Any] = comp_dict
+    self._components: dict[type, object] = comp_dict
 
-  def add(self, *components: Any) -> None:
+  def add(self, *components: object) -> None:
     self_components = self._components
-    events = []
+    events: list[ComponentAdded | ComponentRemoved] = []
     append_event = events.append
     for component in components:
       component_type = type(component)
       if component_type in self_components:
         other_component = self_components[component_type]
         if other_component is component or other_component == component:
           continue
         append_event(ComponentRemoved(self, other_component))
       self_components[component_type] = component
       append_event(ComponentAdded(self, component))
     manager = self._manager()
     if manager is not None:
       manager._components_added(self.id, components, events)
 
-  def remove(self, *components: Any) -> None:
+  def remove(self, *components: object) -> None:
     self_components = self._components
     manager = self._manager()
     for i, component in enumerate(components):
       component_type = type(component)
       try:
         other_component = self_components[component_type]
       except KeyError:
@@ -71,47 +71,62 @@
       raise ValueError(component)
     if manager is not None:
       manager._components_removed(self, components)
 
   def __call__(self, *component_types: type[_T]) -> list[_T]:
     components = self._components
     return [
-      components[component_type]
+      components[component_type]  # type: ignore
       for component_type in {
         comp_type: None for cls in component_types for comp_type in subclasses(cls)
       }  # dict instead of set to guarantee stable ordering while still removing dupes
       if component_type in components
     ]
 
   def __getitem__(self, component_type: type[_T], /) -> _T:
-    components = self._components
-    for cls in subclasses(component_type):
-      if cls in components:
-        return components[cls]
-    raise KeyError(component_type)
+    try:
+      return self._components[component_type]  # type: ignore[return-value]
+    except KeyError:
+      components = self._components
+      for cls in strict_subclasses(component_type):
+        if cls in components:
+          return components[cls]  # type: ignore[return-value]
+      raise
 
   def __setitem__(self, component_type: type[_T], component: _T, /):
-    self.remove(*self(component_type))
+    self.pop(component_type, None)
     self.add(component)
 
   def __delitem__(self, component_type: type, /):
     self.remove(self[component_type])
 
-  def get(self, component_type: type[_T], default: _D = None, /) -> _T | _D:
+  @overload
+  def get(self, component_type: type[_T], /) -> _T | None: ...
+  @overload
+  def get(self, component_type: type[_T], default: _D, /) -> _T | _D: ...
+  def get(self, component_type, default=None, /):
+    try:
+      return self._components[component_type]
+    except KeyError:
+      pass
     components = self._components
-    for cls in subclasses(component_type):
+    for cls in strict_subclasses(component_type):
       if cls in components:
         return components[cls]
     return default
 
-  def pop(self, component_type: type[_T], default: _D = ..., /) -> _T | _D:
+  @overload
+  def pop(self, component_type: type[_T], /) -> _T: ...
+  @overload
+  def pop(self, component_type: type[_T], default: _D, /) -> _T | _D: ...
+  def pop(self, component_type, default=_SENTINEL, /):
     try:
       component = self[component_type]
     except KeyError:
-      if default is Ellipsis:
+      if default is _SENTINEL:
         raise
       return default
     self.remove(component)
     return component
 
   def types(self):
     return self._components.keys()
@@ -121,23 +136,25 @@
 
   def __reversed__(self):
     return reversed(self._components.values())
 
   def __len__(self):
     return len(self._components)
 
-  def __contains__(self, obj: Any, /):
+  def __contains__(self, obj: object, /):
+    if obj in self._components:
+      return True
     if isinstance(obj, type):
       components = self._components
-      for cls in subclasses(obj):
+      for cls in strict_subclasses(obj):
         if cls in components:
           return True
     return False
 
-  def __eq__(self, other: Any, /):
+  def __eq__(self, other: object, /):
     if self is other:
       return True
     if isinstance(other, Entity):
       return self._components == other._components
     return NotImplemented
 
   def clear(self):
```

### Comparing `pyriak-0.1.0/src/pyriak/eventkey.py` & `pyriak-0.2.0/src/pyriak/eventkey.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,25 @@
-__all__ = ['key_functions', 'set_key', 'NoKey', 'NoKeyType', 'KeyFunction']
+__all__ = ['key_functions', 'set_key', 'KeyFunction']
 
-from collections.abc import Callable, Hashable, Iterable, Mapping
-from typing import Any, TypeAlias, TypeVar
+from collections.abc import Callable, Hashable, Iterator, Mapping
+from typing import Any, TypeAlias, TypeVar, overload
 from weakref import WeakKeyDictionary
 
+from pyriak import _SENTINEL
+
 
 _T = TypeVar('_T')
 _D = TypeVar('_D')
 
 del TypeVar
 
 
-class NoKeyType:
-  __slots__ = ()
-
-  def __new__(cls, /):
-    return NoKey
-
-  def __repr__(self, /):
-    return 'NoKey'
-
-  def __init_subclass__(cls, /, **kwargs):
-    raise TypeError(f"cannot subclass type '{cls.__name__}'")
-
-
-NoKey = object.__new__(NoKeyType)
-
-
-# if return is NoKey, no key, else if return value is hashable and not generator,
-# return value is the key, else it is an iterable of keys
-KeyFunction: TypeAlias = Callable[[_T], Hashable | Iterable[Hashable] | NoKeyType]
+# if it is iterator (especially generator), it is multiple
+# hashable keys, else it is the key itself (must be hashable)
+KeyFunction: TypeAlias = Callable[[_T], Hashable | Iterator[Hashable]]
 
 
 class EventKeyFunctions:
   """A weakkey dict of event types to key functions or None."""
 
   __slots__ = ('_data',)
 
@@ -41,17 +27,19 @@
     self, dict: Mapping[type, KeyFunction[Any] | None] | None = None
   ):
     self._data: WeakKeyDictionary[type, KeyFunction[Any] | None]
     self._data = WeakKeyDictionary()
     if dict is not None:
       self.update(dict)
 
-  def __call__(
-    self, event_type: type[_T], default: _D = ...
-  ) -> KeyFunction[_T] | _D:
+  @overload
+  def __call__(self, event_type: type[_T]) -> KeyFunction[_T]: ...
+  @overload
+  def __call__(self, event_type: type[_T], default: _D) -> KeyFunction[_T] | _D: ...
+  def __call__(self, event_type, default=_SENTINEL):
     """Return the key function for event_type.
 
     A key function is used to extract a key from an event of type event_type.
 
     Each type in the event_type's method resolution order (__mro__) is checked until
     a specific key function is found and is not None,
     in which case the key function is returned.
@@ -60,15 +48,15 @@
     This is the only method that considers superclasses, other than the exists method.
     """
     get = self._data.get
     for cls in event_type.__mro__:
       key_function = get(cls)
       if key_function is not None:
         return key_function
-    if default is Ellipsis:
+    if default is _SENTINEL:
       raise KeyError(event_type)
     return default
 
   def exists(self, event_type: type) -> bool:
     """Return True if there is a key function for event_type that is not None."""
     return self(event_type, None) is not None
 
@@ -76,19 +64,21 @@
     """Return the specific key function for an event_type, ignoring superclasses."""
     return self._data[event_type]
 
   def __setitem__(self, event_type: type[_T], key: KeyFunction[_T] | None):
     data = self._data
     if event_type in data:
       raise KeyError(f'cannot reassign event type key: {event_type!r}')
-    if key is NoKey:
-      raise TypeError(f'do not use {NoKey} to denote no key function, use None instead')
     data[event_type] = key
 
-  def get(self, event_type: type[_T], default: _D = None) -> KeyFunction[_T] | None | _D:
+  @overload
+  def get(self, event_type: type[_T]) -> KeyFunction[_T] | None: ...
+  @overload
+  def get(self, event_type: type[_T], default: _D) -> KeyFunction[_T] | _D: ...
+  def get(self, event_type, default=None):
     try:
       return self._data[event_type]
     except KeyError:
       return default
 
   def setdefault(
     self, event_type: type[_T], default: KeyFunction[_T] | None = None
@@ -127,15 +117,15 @@
   def __ror__(self, other: Mapping[type, KeyFunction[Any] | None]):
     return other | self._data
 
   def __ior__(self, other: Mapping[type, KeyFunction[Any] | None]):
     self.update(other)
     return self
 
-  __copy__ = None
+  __copy__ = None  # type: ignore
 
   def copy(self):
     return self._data.copy()
 
   def keyrefs(self):
     return self._data.keyrefs()
```

### Comparing `pyriak-0.1.0/src/pyriak/events.py` & `pyriak-0.2.0/src/pyriak/events.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,36 +9,44 @@
   'SystemRemoved',
   'EventHandlerAdded',
   'EventHandlerRemoved',
   'StateAdded',
   'StateRemoved',
 ]
 
-from collections.abc import Hashable, Iterable
-from typing import TYPE_CHECKING, Any
+from collections.abc import Callable, Hashable, Iterator
+from typing import TYPE_CHECKING, Any, Generic, TypeVar
 
-from pyriak import (
-  Callback as _Callback,
-  NoKey as _NoKey,
-  mro as _mro,
-  set_key as _set_key,
-  subclasses as _subclasses,
-)
+from pyriak import subclasses as _subclasses
+from pyriak.eventkey import set_key as _set_key
 
 
 if TYPE_CHECKING:
-  from pyriak import Entity, System
+  from pyriak.entity import Entity
   from pyriak.managers.systemmanager import _EventHandler
+  from pyriak.space import Space
+  from pyriak.system import System, _Callback
 
 
-class SpaceCallback(_Callback):
+_T = TypeVar('_T')
+
+
+class SpaceCallback(Generic[_T]):
   """A SystemManager automatically calls a SpaceCallback Event when it processes one."""
 
+  # TODO: python 3.11 - callback: Callable[['Space', *_Ts], _T]
 
-#= system callback
+  def __init__(self, callback: Callable [..., _T], /, *args: Any, **kwargs: Any):
+    self.callback = callback
+    self.args = list(args)
+    self.kwargs = kwargs
+
+  def __call__(self, space: 'Space', /) -> _T:
+    """Execute self's callback with self's args and kwargs."""
+    return self.callback(space, *self.args, **self.kwargs)
 
 
 class SendEvent:
   """A special built-in Event type for sending Events to specific System(s).
 
   A SendEvent is basically a wrapper of another Event.
   When a SendEvent is triggered by a SystemManager, only the SendEvent's receivers
@@ -53,31 +61,31 @@
   The order in which the bound callbacks of the receivers are invoked
   is no different from normal Event triggering,
   where higher priority callbacks are called first.
 
   The actual SendEvent instance itself is never processed.
   """
 
-  def __init__(self, event: Any, *receivers: 'System'):
+  def __init__(self, event: object, *receivers: 'System'):
     self.event = event
     self.receivers = set(receivers)
 
 
-def _component_type_key(event: 'ComponentAdded | ComponentRemoved') -> Iterable[type]:
-  yield from _mro(event.component)
+def _component_type_key(event: 'ComponentAdded | ComponentRemoved') -> Iterator[type]:
+  yield from type(event.component).__mro__
 
 @_set_key(_component_type_key)
 class ComponentAdded:
-  def __init__(self, entity: 'Entity', component: Any):
+  def __init__(self, entity: 'Entity', component: object):
     self.entity = entity
     self.component = component
 
 @_set_key(_component_type_key)
 class ComponentRemoved:
-  def __init__(self, entity: 'Entity', component: Any):
+  def __init__(self, entity: 'Entity', component: object):
     self.entity = entity
     self.component = component
 
 
 class EntityAdded:
   def __init__(self, entity: 'Entity'):
     self.entity = entity
@@ -97,70 +105,71 @@
 
 @_set_key(_system_key)
 class SystemRemoved:
   def __init__(self, system: 'System'):
     self.system = system
 
 
-def _handler_key(event: '_EventHandlerEvent') -> Iterable[type]:
-  return _subclasses(event.event_type)
+def _handler_key(event: 'EventHandlerAdded | EventHandlerRemoved') -> Iterator[type]:
+  yield from _subclasses(event.event_type)
 
 @_set_key(_handler_key)
-class _EventHandlerEvent:
+class EventHandlerAdded:
   def __init__(
-    self, handler: '_EventHandler', event_type: type, keys: frozenset[Hashable]
+    self, _handler: '_EventHandler', _event_type: type, _keys: frozenset[Hashable]
   ):
-    self._handler = handler
-    self._event_type = event_type
-    self._keys = keys
+    self._handler = _handler
+    self.event_type = _event_type
+    self.keys = _keys
 
   @property
-  def event_type(self):
-    return self._event_type
+  def system(self):
+    return self._handler.system
 
   @property
   def callback(self):
     return self._handler.callback
 
   @property
-  def system(self):
-    return self._handler.system
+  def name(self):
+    return self._handler.name
 
   @property
   def priority(self):
     return self._handler.priority
 
   @property
-  def name(self):
-    return self._handler.name
+  def key(self):
+    [key] = self.keys
+    return key
 
-  @property
-  def keys(self):
-    return self._keys
+@_set_key(_handler_key)
+class EventHandlerRemoved:
+  def __init__(
+    self, _system: 'System', _callback: '_Callback', _name: str, _priority: Any,
+    _event_type: type, _keys: frozenset[Hashable]
+  ):
+    self.system = _system
+    self.callback = _callback
+    self.name = _name
+    self.priority = _priority
+    self.event_type = _event_type
+    self.keys = _keys
 
   @property
   def key(self):
-    keys = self.keys
-    if not keys:
-      return _NoKey
-    [key] = keys
+    [key] = self.keys
     return key
 
-class EventHandlerAdded(_EventHandlerEvent):
-  pass
-
-class EventHandlerRemoved(_EventHandlerEvent):
-  pass
-
 
-def _state_type_key(event: 'StateAdded | StateRemoved') -> Iterable[type]:
-  yield from _mro(event.state)
+def _state_type_key(event: 'StateAdded | StateRemoved') -> Iterator[type]:
+  yield from type(event.state).__mro__
 
 @_set_key(_state_type_key)
 class StateAdded:
-  def __init__(self, state: Any):
+  def __init__(self, state: object):
     self.state = state
 
 @_set_key(_state_type_key)
 class StateRemoved:
-  def __init__(self, state: Any):
+  def __init__(self, state: object):
     self.state = state
```

### Comparing `pyriak-0.1.0/src/pyriak/managers/entitymanager.py` & `pyriak-0.2.0/src/pyriak/managers/entitymanager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 __all__ = ['EntityManager']
 
 from collections.abc import Iterable, Iterator, KeysView
-from typing import Any, Callable, NoReturn, TypeVar, overload
+from typing import Callable, NoReturn, TypeVar, overload
 from weakref import ref as weakref
 
-from pyriak import EventQueue, dead_weakref, subclasses
+from pyriak import _SENTINEL, EventQueue, dead_weakref, subclasses
 from pyriak.entity import Entity, EntityId
 from pyriak.events import ComponentAdded, ComponentRemoved, EntityAdded, EntityRemoved
-from pyriak.query import ComponentQueryResult, EntityQueryResult, IdQueryResult, Query
+from pyriak.query import (
+  ComponentQueryResult,
+  EntityQueryResult,
+  IdQueryResult,
+  Query,
+  QueryResult,
+)
 
 
 _T = TypeVar('_T')
+_Q = TypeVar('_Q', bound=QueryResult)
 
 
 class _Components:
   """The components attribute of an EntityManager instance, exposes more functionality.
 
   If the EntityManager has been garbage collected, all methods
   raise TypeError.
@@ -38,26 +45,26 @@
     entities = manager._entities
     return (entities[entity_id][component_type]
             for entity_id in manager._component_types.get(component_type, ()))
 
   def types(self) -> KeysView[type]:
     return self._manager()._component_types.keys()
 
-  def __iter__(self) -> Iterator[Any]:
+  def __iter__(self) -> Iterator[object]:
     for entity in self._manager():
       yield from entity
 
-  def __reversed__(self) -> Iterator[Any]:
+  def __reversed__(self) -> Iterator[object]:
     for entity in reversed(self._manager()):
       yield from reversed(entity)
 
   def __len__(self):
     return sum(len(entity) for entity in self._manager()._entities.values())
 
-  def __contains__(self, obj: Any, /):
+  def __contains__(self, obj: object, /):
     types = self._manager()._component_types
     if isinstance(obj, type):
       for cls in subclasses(obj):
         if cls in types:
           return True
     return False
 
@@ -68,21 +75,21 @@
   def __init__(
     self, entities: Iterable[Entity] = (), /, event_queue: EventQueue | None = None
   ):
     self.event_queue = event_queue
     self.components = _Components()
     self.components._manager = weakref(self)  # type: ignore
     self._entities: dict[EntityId, Entity] = {}
-    self._component_types = {}
+    self._component_types: dict[type, set[EntityId]] = {}
     self.add(*entities)
 
   def add(self, *entities: Entity) -> None:
     component_types = self._component_types
     self_entities = self._entities
-    self_weakref: weakref[EntityManager] = weakref(self)  # type: ignore
+    self_weakref: weakref[EntityManager] = weakref(self)
     event_queue = self.event_queue
     for entity in entities:
       entity_id = entity.id
       if entity_id in self_entities:
         continue
       if entity._manager() is not None:
         raise RuntimeError(f'{entity!r} already added to another manager')
@@ -97,15 +104,15 @@
           component_types[component_type] = {entity_id}
       if event_queue is not None:
         event_queue.extend([
           EntityAdded(entity),
           *[ComponentAdded(entity, component) for component in entity]
         ])
 
-  def create(self, *components: Any) -> Entity:
+  def create(self, *components: object) -> Entity:
     """Create an Entity with the given components, add it to self, and return it.
 
     The returned Entity can, of course, be directly modified.
     """
     entity: Entity = Entity(components)
     self.add(entity)
     return entity
@@ -135,22 +142,30 @@
 
   def __getitem__(self, entity_id: EntityId, /) -> Entity:
     return self._entities[entity_id]
 
   def __delitem__(self, entity_id: EntityId, /):
     self.remove(self._entities[entity_id])
 
-  def get(self, entity_id: EntityId, default: _T = None, /) -> Entity | _T:
+  @overload
+  def get(self, entity_id: EntityId, /) -> Entity | None: ...
+  @overload
+  def get(self, entity_id: EntityId, default: _T, /) -> Entity | _T: ...
+  def get(self, entity_id, default=None, /):
     return self._entities.get(entity_id, default)
 
-  def pop(self, entity_id: EntityId, default: _T = ..., /) -> Entity | _T:
+  @overload
+  def pop(self, entity_id: EntityId, /) -> Entity: ...
+  @overload
+  def pop(self, entity_id: EntityId, default: _T, /) -> Entity | _T: ...
+  def pop(self, entity_id, default=_SENTINEL, /):
     try:
       entity = self._entities[entity_id]
     except KeyError:
-      if default is Ellipsis:
+      if default is _SENTINEL:
         raise
       return default
     self.remove(entity)
     return entity
 
   @overload
   def query(self, query: Query, /) -> ComponentQueryResult: ...
@@ -160,15 +175,15 @@
   ) -> NoReturn: ...
   @overload
   def query(
     self, /,
     *component_types: type,
     merge: Callable[..., set] = set.intersection,
   ) -> ComponentQueryResult: ...
-  def query(self, /, *types, merge=...):
+  def query(self, /, *types, merge=None):
     """"""
     return self._query(ComponentQueryResult, types, merge)
 
   @overload
   def entity_query(self, query: Query, /) -> EntityQueryResult: ...
   @overload
   def entity_query(
@@ -176,15 +191,15 @@
   ) -> NoReturn: ...
   @overload
   def entity_query(
     self, /,
     *component_types: type,
     merge: Callable[..., set] = set.intersection,
   ) -> EntityQueryResult: ...
-  def entity_query(self, /, *types, merge=...):
+  def entity_query(self, /, *types, merge=None):
     """"""
     return self._query(EntityQueryResult, types, merge)
 
   @overload
   def id_query(self, query: Query, /) -> IdQueryResult: ...
   @overload
   def id_query(
@@ -192,32 +207,32 @@
   ) -> NoReturn: ...
   @overload
   def id_query(
     self, /,
     *component_types: type,
     merge: Callable[..., set] = set.intersection,
   ) -> IdQueryResult: ...
-  def id_query(self, /, *types, merge=...):
+  def id_query(self, /, *types, merge=None):
     """"""
     return self._query(IdQueryResult, types, merge)
 
-  def _query(self, query_cls: type[_T], types, merge=..., /) -> _T:
+  def _query(self, result_cls: type[_Q], types, merge=None, /) -> _Q:
     """"""
     if len(types) == 1 and isinstance((query := types[0]), Query):
-      if merge is not Ellipsis:
+      if merge is not None:
         raise TypeError('unexpected keyword argument: merge')
       types = query.types
       merge = query.merge
-    elif merge is Ellipsis:
+    elif merge is None:
       merge = set.intersection
     if not types:
       raise ValueError('expected at least one type in component types')
     self_entities = self._entities
     self_component_types = self._component_types
-    return query_cls(
+    return result_cls(
       {
         id: self_entities[id]
         for id in merge(*[
           self_component_types[typ]  # noqa: SIM401
           if typ in self_component_types else set()
           for typ in types
         ])
@@ -233,15 +248,15 @@
       entities[entity_id] for entity_id in self._component_types.get(component_type, ())
     )
 
   @overload
   def ids(self, /) -> KeysView[EntityId]: ...
   @overload
   def ids(self, component_type: type, /) -> set[EntityId]: ...
-  def ids(self, component_type=None, /):  # type: ignore
+  def ids(self, component_type=None, /):
     """Return a set of all entity ids that contain the given component type.
 
     If no component type is given, then
     return a set-like view of all entity ids in self instead.
     """
     if component_type is None:
       return self._entities.keys()
@@ -259,39 +274,39 @@
 
   def __reversed__(self):
     return reversed(self._entities.values())
 
   def __len__(self):
     return len(self._entities)
 
-  def __contains__(self, obj: Any, /):
+  def __contains__(self, obj: object, /):
     if isinstance(obj, Entity):
       return obj.id in self._entities
     return obj in self._entities
 
   def clear(self):
     self.remove(*self)
 
   def _components_added(
-    self, entity_id: EntityId, components: Iterable[Any], events: Iterable[Any], /
+    self, entity_id: EntityId, components: Iterable[object], events: Iterable[object], /
   ) -> None:
     component_types = self._component_types
     for component_type in {
       component_type
       for component in components
       for component_type in type(component).__mro__
     }:
       try:
         component_types[component_type].add(entity_id)
       except KeyError:
         component_types[component_type] = {entity_id}
     if (queue := self.event_queue) is not None:
       queue.extend(events)
 
-  def _components_removed(self, entity: Entity, components: Iterable[Any], /) -> None:
+  def _components_removed(self, entity: Entity, components: Iterable[object], /) -> None:
     component_types = self._component_types
     entity_id = entity.id
     for component_type in {
       component_type
       for component in components
       for component_type in type(component).__mro__
       if component_type not in entity
```

### Comparing `pyriak-0.1.0/src/pyriak/managers/statemanager.py` & `pyriak-0.2.0/src/pyriak/managers/statemanager.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 __all__ = ['StateManager']
 
 from collections.abc import Iterable
-from typing import Any, TypeVar
+from typing import TypeVar, overload
 
-from pyriak import EventQueue, subclasses
+from pyriak import _SENTINEL, EventQueue, strict_subclasses, subclasses
 from pyriak.events import StateAdded, StateRemoved
 
 
 _T = TypeVar('_T')
 _D = TypeVar('_D')
 
 
@@ -16,36 +16,36 @@
 
   StateManager structure is very similar to an Entity.
   """
 
   __slots__ = '_states', 'event_queue', '__weakref__'
 
   def __init__(
-    self, states: Iterable[Any] = (), /, event_queue: EventQueue | None = None
+    self, states: Iterable[object] = (), /, event_queue: EventQueue | None = None
   ):
     self.event_queue = event_queue
-    self._states: dict[type, Any] = {}
+    self._states: dict[type, object] = {}
     self.add(*states)
 
-  def add(self, *states: Any) -> None:
+  def add(self, *states: object) -> None:
     self_states = self._states
     event_queue = self.event_queue
     for state in states:
       state_type = type(state)
       if state_type in self_states:
         other_state = self_states[state_type]
         if other_state is state or other_state == state:
           continue
         if event_queue is not None:
           event_queue.append(StateRemoved(other_state))
       self_states[state_type] = state
       if event_queue is not None:
         event_queue.append(StateAdded(state))
 
-  def remove(self, *states: Any) -> None:
+  def remove(self, *states: object) -> None:
     self_states = self._states
     event_queue = self.event_queue
     for state in states:
       state_type = type(state)
       try:
         other_state = self_states[state_type]
       except KeyError:
@@ -57,47 +57,62 @@
             event_queue.append(StateRemoved(state))
           continue
       raise ValueError(state)
 
   def __call__(self, *state_types: type[_T]) -> list[_T]:
     states = self._states
     return [
-      states[state_type]
+      states[state_type]  # type: ignore
       for state_type in {
         state_type: None for cls in state_types for state_type in subclasses(cls)
       }  # dict instead of set to guarantee stable ordering while still removing dupes
       if state_type in states
     ]
 
   def __getitem__(self, state_type: type[_T], /) -> _T:
-    states = self._states
-    for cls in subclasses(state_type):
-      if cls in states:
-        return states[cls]
-    raise KeyError(state_type)
+    try:
+      return self._states[state_type]  # type: ignore[return-value]
+    except KeyError:
+      states = self._states
+      for cls in strict_subclasses(state_type):
+        if cls in states:
+          return states[cls]  # type: ignore[return-value]
+      raise
 
   def __setitem__(self, state_type: type[_T], state: _T, /):
-    self.remove(*self(state_type))
+    self.pop(state_type, None)
     self.add(state)
 
   def __delitem__(self, state_type: type, /):
     self.remove(self[state_type])
 
-  def get(self, state_type: type[_T], default: _D = None, /) -> _T | _D:
+  @overload
+  def get(self, state_type: type[_T], /) -> _T | None: ...
+  @overload
+  def get(self, state_type: type[_T], default: _D, /) -> _T | _D: ...
+  def get(self, state_type, default=None, /):
+    try:
+      return self._states[state_type]
+    except KeyError:
+      pass
     states = self._states
-    for cls in subclasses(state_type):
+    for cls in strict_subclasses(state_type):
       if cls in states:
         return states[cls]
     return default
 
-  def pop(self, state_type: type[_T], default: _D = ..., /) -> _T | _D:
+  @overload
+  def pop(self, state_type: type[_T], /) -> _T: ...
+  @overload
+  def pop(self, state_type: type[_T], default: _D, /) -> _T | _D: ...
+  def pop(self, state_type, default=_SENTINEL, /):
     try:
       state = self[state_type]
     except KeyError:
-      if default is Ellipsis:
+      if default is _SENTINEL:
         raise
       return default
     self.remove(state)
     return state
 
   def types(self):
     return self._states.keys()
@@ -107,17 +122,19 @@
 
   def __reversed__(self):
     return reversed(self._states.values())
 
   def __len__(self):
     return len(self._states)
 
-  def __contains__(self, obj: Any, /):
+  def __contains__(self, obj: object, /):
+    if obj in self._states:
+      return True
     if isinstance(obj, type):
       states = self._states
-      for cls in subclasses(obj):
+      for cls in strict_subclasses(obj):
         if cls in states:
           return True
     return False
 
   def clear(self):
     self.remove(*self)
```

### Comparing `pyriak-0.1.0/src/pyriak/managers/systemmanager.py` & `pyriak-0.2.0/src/pyriak/managers/systemmanager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 __all__ = ['SystemManager']
 
-from collections.abc import Generator, Hashable, Iterable
+from collections.abc import Hashable, Iterable, Iterator, Mapping
 from typing import TYPE_CHECKING, Any, NamedTuple
 from weakref import ref as weakref
 
-from pyriak import EventQueue, NoKey, NoKeyType, dead_weakref, key_functions, subclasses
+from pyriak import EventQueue, dead_weakref, strict_subclasses, subclasses
+from pyriak.eventkey import key_functions
 from pyriak.events import (
   EventHandlerAdded,
   EventHandlerRemoved,
   SendEvent,
   SpaceCallback,
   SystemAdded,
   SystemRemoved,
 )
 from pyriak.system import System, _Callback
 
 
 if TYPE_CHECKING:
-  from pyriak import Space
-
-
-# event subhandler dict type alias
+  from pyriak.space import Space
 
 
 class _EventHandler(NamedTuple):
   """Object that holds the info for a single event handler callback in a SystemManager.
 
   A function on a system can be bound to event types. If a function is bound
   to at least one event type (most common is just one), then it is an event handler
@@ -47,47 +45,50 @@
   callback: _Callback
   name: str
   priority: Any
 
   def __call__(self, /, *args, **kwargs):
     return self.callback(*args, **kwargs)
 
-  def __eq__(self, other: Any):
+  def __eq__(self, other: object):
     if self is other:
       return True
     if isinstance(other, _EventHandler):
       return self.name == other.name and self.system == other.system
     return NotImplemented
 
   def __hash__(self):
     return hash((self.name,self.system))
 
 del NamedTuple
 
 
 class SystemManager:
-  __slots__ = '_space', '_systems', '_handlers', '_event_queue', '__weakref__'
+  __slots__ = (
+    '_space', '_systems', '_handlers', '_key_handlers', 'event_queue', '__weakref__'
+  )
+
+  event_queue: EventQueue | None
 
   def __init__(
     self,
     systems: Iterable[System] = (),
     /,
     space: 'Space | None' = None,
     event_queue: EventQueue | None = None
   ):
     self.space = space
-    self._event_queue = event_queue
+    self.event_queue = event_queue
     # values aren't used: dict is for insertion order
     self._systems: dict[System, None] = {}
-    self._handlers: dict[
-      type, list[_EventHandler] | dict[Hashable | NoKeyType, list[_EventHandler]]
-    ] = {}
+    self._handlers: dict[type, list[_EventHandler]] = {}
+    self._key_handlers: dict[type, dict[Hashable, list[_EventHandler]]] = {}
     self.add(*systems)
 
-  def process(self, event: Any, space: 'Space | None' = None) -> bool:
+  def process(self, event: object, space: 'Space | None' = None) -> bool:
     """Handle an event. Callbacks of the event are passed space and event.
 
     If the Event type has no binds, do nothing.
     If event is an instance of SpaceCallback or SendEvent, it is handled differently.
     If a callback returns a truthy value, the
     rest of the callbacks are skipped and True is returned, else False.
     """
@@ -187,57 +188,37 @@
 
   def __reversed__(self):
     return reversed(self._systems)
 
   def __len__(self):
     return len(self._systems)
 
-  def __contains__(self, obj: Any, /):
+  def __contains__(self, obj: object, /):
     """Return whether obj is a system added to self (ignoring subclasses)."""
     return obj in self._systems
 
   def clear(self):
     """Remove all systems and event handlers from self.
 
     Does not trigger any events.
     Does not invoke System._removed_ method.
     Does not change self's space or event_queue.
     """
     self._handlers.clear()
+    self._key_handlers.clear()
     self._systems.clear()
 
   @property
   def space(self) -> 'Space | None':
     return self._space()
 
   @space.setter
   def space(self, value: 'Space | None'):
     self._space = dead_weakref if value is None else weakref(value)
 
-  @space.deleter
-  def space(self):
-    self._space = dead_weakref
-
-  @property
-  def event_queue(self) -> EventQueue | None:
-    event_queue = self._event_queue
-    if event_queue is None:
-      space = self.space
-      if space is not None:
-        return space.event_queue
-    return event_queue
-
-  @event_queue.setter
-  def event_queue(self, value: EventQueue | None):
-    self._event_queue = value
-
-  @event_queue.deleter
-  def event_queue(self):
-    del self._event_queue
-
   @staticmethod
   def _insert_handler(list: list[_EventHandler], handler: _EventHandler, /) -> None:
     """Inserts a handler into a list of other handlers.
 
     Sorts by: highest priority, then oldest handler.
     """
     priority = handler.priority
@@ -277,245 +258,242 @@
       for n in system._handlers_:
         if other_name == n:
           return False
         if name == n:
           return True
       raise ValueError
 
-  def _sorted_handlers(
+  def _sort_handlers(
     self, handlers: Iterable[_EventHandler], /
   ) -> list[_EventHandler]:
     SortKey = self._SortKey
     systems = self._systems
-    return sorted(handlers, key=lambda h: SortKey(h, systems))
+    # Uses dict to remove duplicates while preserving some order
+    return sorted(dict.fromkeys(handlers), key=lambda h: SortKey(h, systems))
 
-  def _get_handlers(self, event: Any, /) -> list[_EventHandler]:
+  def _get_handlers(self, event: object, /) -> list[_EventHandler]:
     event_type = type(event)
     try:
       handlers = self._handlers[event_type]
     except KeyError:
       handlers = self._lazy_bind(event_type)
-    try:
-      key_function = key_functions(event_type)
-    except KeyError:
-      return handlers  # type: ignore
-    key = key_function(event)
-    if not isinstance(key, Generator):
+      if not key_functions.exists(event_type):
+        return handlers
+      key_handlers = self._lazy_key_bind(event_type)
+    else:
+      if event_type not in self._key_handlers:
+        return handlers
+      key_handlers = self._key_handlers[event_type]
+    key = key_functions(event_type)(event)
+    if not isinstance(key, Iterator):
       try:
-        return handlers[key]  # type: ignore
+        return key_handlers[key]
       except KeyError:
-        return handlers[NoKey]  # type: ignore
-      except TypeError:
-        pass
-    keys = {k for k in key if k in handlers}  # type: ignore
-    if not keys:
-      return handlers[NoKey]  # type: ignore
-    if len(keys) == 1:
-      return handlers[keys.pop()]
-    return self._sorted_handlers({
-      handler: None for key in keys for handler in handlers[key]
-    })  # preserving order slightly by using a dict instead of set
+        return handlers
+    keys = {k for k in key if k in key_handlers}
+    if len(keys) > 1:
+      return self._sort_handlers(handler for key in keys for handler in key_handlers[key])
+    if keys:
+      return key_handlers[keys.pop()]
+    return handlers
 
   def _bind(self, system: System, /) -> list[EventHandlerAdded]:
     """Bind a system's handlers so that they can process events.
 
     If a specified event type does not exist, _lazy_bind is called to find
     bindings for it based on existing superclasses.
 
     Bindings of an event type are sorted by highest priority,
     then oldest system, then first one bound in system.
     """
-    try:
-      if not system._bindings_:
-        return []
-    except AttributeError:
-      if isinstance(system, System):
-        raise
-      raise TypeError(f'{system!r} is not a System') from None
-    events: list[EventHandlerAdded] = []
+    if not isinstance(system, System):
+      raise TypeError(f'{system!r} is not a System')
+    if not system._bindings_:
+      return []
+    handler_events: list[EventHandlerAdded] = []
     all_handlers = self._handlers
+    all_key_handlers = self._key_handlers
     insert_handler = self._insert_handler
+    fromkeys = dict.fromkeys
     for name, bindings in system._bindings_.items():
       callback = getattr(system, name)
       if len(bindings) == 1:
         # the common case of only one event type for a handler (single @bind())
         [(event_type, binding)] = bindings.items()
         handler = _EventHandler(system, callback, name, binding.priority)
         event_handlers = {
-          cls: handler for cls in subclasses(event_type) if cls in all_handlers
-        }  #= only strict
+          cls: handler for cls in strict_subclasses(event_type) if cls in all_handlers
+        }
+        key_event_types = event_handlers.keys() & all_key_handlers
         event_handlers[event_type] = handler
-        keys = binding.keys
-        events.append(EventHandlerAdded(handler, event_type, keys))
-        if not keys:
-          handler_keys = {}
-        else:
-          keys = dict.fromkeys(keys, handler)
-          handler_keys = {
-            cls: keys for cls in event_handlers if key_functions.exists(cls)
-          }
+        if key_functions.exists(event_type):
+          key_event_types.add(event_type)
+        binding_keys = binding.keys
+        handler_keys: dict[type, Mapping[Hashable, _EventHandler]] = (
+          fromkeys(key_event_types, fromkeys(binding_keys, handler))
+          if binding_keys else {}
+        )
+        handler_events.append(EventHandlerAdded(handler, event_type, binding_keys))
       else:
         event_handlers = {}
-        base_handler_keys = {}
+        base_handler_keys: dict[type, Mapping[Hashable, _EventHandler]] = {}
+        cached_handlers: dict[int, _EventHandler] = {}
         for event_type, binding in bindings.items():
-          keys = binding.keys
           priority = binding.priority
-          for other_handler in event_handlers.values():
-            if priority is other_handler.priority:
-              # saves memory: duplicate handler for different event types that have same
-              # priority, is likely because multibinding is usually for similar classes
-              event_handlers[event_type] = handler = other_handler
-              break
+          priority_id = id(priority)
+          if priority_id in cached_handlers:
+            handler = cached_handlers[priority_id]
           else:
-            event_handlers[event_type] = handler = _EventHandler(
+            handler = cached_handlers[priority_id] = _EventHandler(
               system, callback, name, priority
             )
-          if keys:
-            base_handler_keys[event_type] = dict.fromkeys(keys, handler)
-          events.append(EventHandlerAdded(handler, event_type, keys))
-        handler_keys = {}
+          event_handlers[event_type] = handler
+          binding_keys = binding.keys
+          if binding_keys:
+            base_handler_keys[event_type] = fromkeys(binding_keys, handler)
+          handler_events.append(EventHandlerAdded(handler, event_type, binding_keys))
+        del cached_handlers
+        # Subclasses of bound event types may also trigger the event handler,
+        # and will inherit their binding (keys and priority).
+        # In the rare case that a class is the subclass of multiple bound
+        # event types, the subclass will try to inherit the bindings of all,
+        # but the first bound type in its MRO will take precedence
+        # for shared keys (or when the subclass is keyless).
+        # A bound event type may be the subclass of other bound event types.
         for cls in {
           cls
           for event_type in bindings
-          for cls in subclasses(event_type)
-          if cls in all_handlers or cls in bindings
+          for cls in strict_subclasses(event_type)
+          if cls in all_handlers
         }:
-          # The subclasses of a bound event type shall have their keys extended by
-          # the bound event type's direct keys, if there exists a key function for it.
-          key_function_exists = key_functions.exists(cls)
           for base in cls.__mro__:
-            # check each 'base' event type to see if its keys are needed
-            if base not in bindings:
-              continue
-            if cls not in event_handlers:
-              # copy the event handler for the subclass if it's not already there
+            if base in bindings:
               event_handlers[cls] = event_handlers[base]
-            if not (key_function_exists and base in handler_keys):
-              continue
-            if cls not in handler_keys:
-              # copy the keys for the subclass if it's not already there
-              handler_keys[cls] = dict(base_handler_keys[base])
-              continue
-            keys = handler_keys[cls]
-            for k, v in base_handler_keys[base].items():
-              # keys of the highest in mro will take priority over lower
-              if k not in keys:
-                # different keys may have different handler priorities because of
-                # different event types, so there may be different event handlers
-                keys[k] = v
+              break
+          else:
+            raise RuntimeError
+        handler_keys = {}
+        key_event_types = event_handlers.keys() & all_key_handlers
+        key_event_types |= {ev_t for ev_t in bindings if key_functions.exists(ev_t)}
+        for cls in key_event_types:
+          inherit_handler_keys: dict[Hashable, _EventHandler] = {}
+          total_len = 0
+          for base in reversed(cls.__mro__):
+            if base in base_handler_keys:
+              inherit_base_keys = base_handler_keys[base]
+              inherit_handler_keys.update(inherit_base_keys)
+              total_len += len(inherit_base_keys)
+          if total_len != len(inherit_handler_keys):
+            # When inheriting multiple of the same key,
+            # the key object of the first type in the MRO is kept
+            inherit_handler_keys = {
+              key: inherit_handler_keys[key]
+              for base in cls.__mro__ for key in base_handler_keys.get(base, ())
+            }
+          handler_keys[cls] = inherit_handler_keys
 
       for event_type, handler in event_handlers.items():
-        try:
-          handlers = all_handlers[event_type]
-        except KeyError:
-          if event_type not in bindings:
-            continue
-          handlers = self._lazy_bind(event_type)
-        if not key_functions.exists(event_type):
-          insert_handler(handlers, handler)  # type: ignore
+        handlers = (
+          all_handlers[event_type] if event_type in all_handlers
+          else self._lazy_bind(event_type)
+        )
+        if event_type not in key_event_types:
+          insert_handler(handlers, handler)
           continue
-        keys = handler_keys.get(event_type, ())
+        key_handlers = (
+          all_key_handlers[event_type] if event_type in all_key_handlers
+          else self._lazy_key_bind(event_type)
+        )
+        keys = handler_keys.get(event_type, {})
         if not keys:
-          for subhandlers in handlers.values():  # type: ignore
-            insert_handler(subhandlers, handler)
+          insert_handler(handlers, handler)
+          for handlers in key_handlers.values():
+            insert_handler(handlers, handler)
           continue
-        for key, subhandler in keys.items():
-          if key in handlers:
-            insert_handler(handlers[key], subhandler)  # type: ignore
-          else:
-            subhandlers = list(handlers[NoKey])  # type: ignore
-            handlers[key] = subhandlers  # type: ignore
-            insert_handler(subhandlers, subhandler)
-    return events
+        for key, handler in keys.items():
+          if key not in key_handlers:
+            key_handlers[key] = handlers[:]
+          insert_handler(key_handlers[key], handler)
+    return handler_events
 
-  def _lazy_bind(
-    self, event_type: type, /
-  ) -> list[_EventHandler] | dict[Hashable | NoKeyType, list[_EventHandler]]:
+  def _lazy_bind(self, event_type: type, /) -> list[_EventHandler]:
     """Find bindings for event_type and bind them and return the handlers.
 
     Subclass instances of an event_type can be processed by superclass handlers.
     These subclasses are only bound when a subclass is processed. Hence, lazy binding.
     """
     all_handlers = self._handlers
-    inherit_handlers = {
-      ev_t: all_handlers[ev_t] for ev_t in event_type.__mro__ if ev_t in all_handlers
-    }
-    if not inherit_handlers:
-      event_handlers = (
-        [] if not key_functions.exists(event_type) else {NoKey: []}
-      )  # type: ignore
-      all_handlers[event_type] = event_handlers
-      return event_handlers
-    # dicts with ignored values are used (instead of lists or sets)
-    # to remove duplicate handlers and somewhat preserve ordering,
-    # before converting back into sorted list
-    if not key_functions.exists(event_type):
-      event_handlers = {}
-      for ev_t, handlers in inherit_handlers.items():
-        if key_functions.exists(ev_t):
-          handlers = handlers[NoKey]  # type: ignore
-        event_handlers.update(dict.fromkeys(handlers))  # type: ignore
-      event_handlers = self._sorted_handlers(event_handlers)  # type: ignore
-    else:
-      event_handlers: dict[
-        Hashable | NoKeyType, list[_EventHandler]
-      ] = {NoKey: {}}  # type: ignore
-      nokey_handlers_list = []
-      for ev_t, handlers in inherit_handlers.items():
-        if not key_functions.exists(ev_t):
-          nokey_handlers_list.append(dict.fromkeys(handlers))
-          continue
-        for key, subhandlers in handlers.items():  # type: ignore
-          if key is NoKey:
-            nokey_handlers_list.append(subhandlers)
-            continue
-          if key in event_handlers:
-            event_handlers[key].update(dict.fromkeys(subhandlers))  # type: ignore
-          else:
-            event_handlers[key] = dict.fromkeys(subhandlers)  # type: ignore
-      inherit_nokey_handlers = {
-        h: None for nokey_handlers in nokey_handlers_list for h in nokey_handlers
-      }
-      for subhandlers in event_handlers.values():
-        subhandlers.update(inherit_nokey_handlers)  # type: ignore
-      sorted_handlers = self._sorted_handlers
-      event_handlers = {k: sorted_handlers(v) for k, v in event_handlers.items()}
+    event_handlers = [
+      handler
+      for ev_t in event_type.__mro__
+      if ev_t in all_handlers
+      for handler in all_handlers[ev_t]
+    ]
+    if event_handlers:
+      event_handlers = self._sort_handlers(event_handlers)
     all_handlers[event_type] = event_handlers
     return event_handlers
 
+  def _lazy_key_bind(
+    self, event_type: type, /
+  ) -> dict[Hashable, list[_EventHandler]]:
+    all_key_handlers = self._key_handlers
+    inherit_key_handlers = [
+      item
+      for ev_t in event_type.__mro__
+      if ev_t in all_key_handlers
+      for item in all_key_handlers[ev_t].items()
+    ]
+    if inherit_key_handlers:
+      unsorted_handlers: dict[Hashable, list[list[_EventHandler]]] = {}
+      base_handlers = self._handlers[event_type]
+      for key, handlers in inherit_key_handlers:
+        if key in unsorted_handlers:
+          unsorted_handlers[key].append(handlers)
+        else:
+          unsorted_handlers[key] = [base_handlers, handlers]
+      sort_handlers = self._sort_handlers
+      key_handlers: dict[Hashable, list[_EventHandler]] = {
+        key: sort_handlers(handler for handlers in handlers_list for handler in handlers)
+        for key, handlers_list in unsorted_handlers.items()
+      }
+    else:
+      key_handlers = {}
+    all_key_handlers[event_type] = key_handlers
+    return key_handlers
+
   def _unbind(self, system: System, /) -> list[EventHandlerRemoved]:
     """Remove all handlers that belong to system from self.
 
     If an event type no longer has any handlers, it is removed.
-    This also applies to keys with subhandlers.
+    This also applies to keys with handlers.
     """
     events: list[EventHandlerRemoved] = []
     all_handlers = self._handlers
-    for event_types in system._bindings_.values():
+    all_key_handlers = self._key_handlers
+    for name, event_types in system._bindings_.items():
       for cls, binding in event_types.items():
         for event_type in subclasses(cls):
           try:
             handlers = all_handlers[event_type]
           except KeyError:
             continue
-          if not key_functions.exists(event_type):
-            for handler in handlers[:]:  # type: ignore
-              if handler.system is system:
-                handlers.remove(handler)  # type: ignore
-            if not handlers:
-              del all_handlers[event_type]
-            continue
-          remove_event_type = True
-          for key, subhandlers in handlers.items():  # type: ignore
-            for handler in subhandlers[:]:
-              if handler.system is system:
-                subhandlers.remove(handler)
-            if subhandlers:
-              remove_event_type = False
-            elif key is not NoKey:
-              del handlers[key]  # type: ignore
-          if remove_event_type:
+          handlers[:] = [
+            handler for handler in handlers if handler.system is not system
+          ]
+          if not handlers:
             del all_handlers[event_type]
-        # a given bound event type for a handler
-        # will always have identical EventHandler objects
-        events.append(EventHandlerRemoved(handler, cls, binding.keys))  # type: ignore
+          if event_type not in all_key_handlers:
+            continue
+          key_handlers = all_key_handlers[event_type]
+          for key, handlers in key_handlers.items():
+            handlers[:] = [
+              handler for handler in handlers if handler.system is not system
+            ]
+            if not handlers:
+              del key_handlers[key]
+          if not key_handlers:
+            del all_key_handlers[event_type]
+        events.append(EventHandlerRemoved(
+          system, getattr(system, name), name, binding.priority, cls, binding.keys
+        ))
     return events
```

### Comparing `pyriak-0.1.0/src/pyriak/query.py` & `pyriak-0.2.0/src/pyriak/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,21 +50,22 @@
 
   def __iter__(self):
     return iter(self._types)
 
   def __len__(self):
     return len(self._types)
 
-  def __contains__(self, obj: Any, /):
+  def __contains__(self, obj: object, /):
     return obj in self._types
 
-  def __eq__(self, other: Any, /):
+  def __eq__(self, other: object, /):
     if not isinstance(other, Query):
       return NotImplemented
-    return self._types == other._types and self._merge == other._merge
+    # TODO: investigate unusual problem with type narrowing
+    return self._types == other._types and self._merge == other._merge  # type: ignore
 
   def __hash__(self):
     return hash((self._types,self._merge))
 
   def __repr__(self):
     return (
       f'{type(self).__name__}'
@@ -100,15 +101,15 @@
     """Return a new Query object that describes self."""
     return Query(*self.types, merge=self.merge)
 
   @overload
   def __call__(self) -> Iterator[Any]: ...
   @overload
   def __call__(self, *component_types: type[_T]) -> Iterator[_T]: ...
-  def __call__(self, *component_types):  # type: ignore
+  def __call__(self, *component_types):
     if not component_types:
       component_types = self.types
     return (comp for ent in self.entities for comp in ent(*component_types))
 
   # group method
 
   @overload
@@ -121,15 +122,15 @@
   ) -> tuple[Iterator[Any], ...]: ...
   @overload
   @abstractmethod
   def __getitem__(
     self, component_type: type[_T], /
   ) -> Iterator[_T] | tuple[Iterator[Any], Iterator[_T]]: ...
   @abstractmethod
-  def __getitem__(self, key, /):  # type: ignore
+  def __getitem__(self, key, /):
     ...
 
   #= get method?
 
   @abstractmethod
   def zip(self, *component_types: type) -> Iterator[tuple[Any, ...]]:
     ...
```

### Comparing `pyriak-0.1.0/src/pyriak/space.py` & `pyriak-0.2.0/src/pyriak/space.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,109 +1,95 @@
 __all__ = ['Space']
 
 from collections import deque
 from collections.abc import Callable
-from typing import Any, NoReturn, overload
+from typing import NoReturn, overload
 
 from pyriak import EventQueue, managers
 from pyriak.query import ComponentQueryResult, EntityQueryResult, IdQueryResult, Query
 
 
 class Space:
-  __slots__ = 'systems', 'entities', 'states', '_event_queue', '__weakref__'
+  __slots__ = 'systems', 'entities', 'states', 'event_queue', '__weakref__'
 
   def __init__(
     self, *,
-    systems: managers.SystemManager = ...,
-    entities: managers.EntityManager = ...,
-    states: managers.StateManager = ...,
-    event_queue: EventQueue = ...
+    systems: managers.SystemManager | None = None,
+    entities: managers.EntityManager | None = None,
+    states: managers.StateManager | None = None,
+    event_queue: EventQueue | None = None
   ):
     """A new Space instance, which glues together the managers and the event queue.
 
     By default, creates the EntityManager, StateManager, and SystemManager.
     """
-    if systems is Ellipsis:
+    if systems is None:
       systems = managers.SystemManager()
-      systems.space = self
-    self.systems = systems
-    if entities is Ellipsis:
+    if entities is None:
       entities = managers.EntityManager()
-    self.entities = entities
-    if states is Ellipsis:
+    if states is None:
       states = managers.StateManager()
-    self.states = states
-    if event_queue is Ellipsis:
+    if event_queue is None:
       event_queue = deque()
+    self.systems = systems
+    systems.space = self
+    self.entities = entities
+    self.states = states
     self.event_queue = event_queue
-
-  @property
-  def event_queue(self) -> EventQueue:
-    return self._event_queue
-
-  @event_queue.setter
-  def event_queue(self, value: EventQueue):
-    self._event_queue = value
-    for manager in (self.entities,self.states):
-      if manager is not None:
-        manager.event_queue = value
-
-  @event_queue.deleter
-  def event_queue(self):
-    del self._event_queue
+    systems.event_queue = entities.event_queue = states.event_queue = event_queue
 
   @overload
   def query(self, query: Query, /) -> ComponentQueryResult: ...
   @overload
   def query(
     self, /, *, merge: Callable[..., set] = set.intersection,
   ) -> NoReturn: ...
   @overload
   def query(
     self, /,
     *component_types: type,
     merge: Callable[..., set] = set.intersection,
   ) -> ComponentQueryResult: ...
-  def query(self, /, *types, merge=...):
+  def query(self, /, *types, merge=None):
     return self.entities.query(*types, merge=merge)
 
   @overload
   def entity_query(self, query: Query, /) -> EntityQueryResult: ...
   @overload
   def entity_query(
     self, /, *, merge: Callable[..., set] = set.intersection,
   ) -> NoReturn: ...
   @overload
   def entity_query(
     self, /,
     *component_types: type,
     merge: Callable[..., set] = set.intersection,
   ) -> EntityQueryResult: ...
-  def entity_query(self, /, *types, merge=...):
+  def entity_query(self, /, *types, merge=None):
     return self.entities.entity_query(*types, merge=merge)
 
   @overload
   def id_query(self, query: Query, /) -> IdQueryResult: ...
   @overload
   def id_query(
     self, /, *, merge: Callable[..., set] = set.intersection,
   ) -> NoReturn: ...
   @overload
   def id_query(
     self, /,
     *component_types: type,
     merge: Callable[..., set] = set.intersection,
   ) -> IdQueryResult: ...
-  def id_query(self, /, *types, merge=...):
+  def id_query(self, /, *types, merge=None):
     return self.entities.id_query(*types, merge=merge)
 
-  def process(self, event: Any):
+  def process(self, event: object):
     return self.systems.process(event, space=self)
 
-  def post(self, *events: Any) -> None:
+  def post(self, *events: object) -> None:
     self.event_queue.extend(events)
 
   def pump(self, events: int | None = None) -> int:
     process_event = self.process
     queue = self.event_queue
     if isinstance(queue, deque):
       pop = queue.popleft
```

### Comparing `pyriak-0.1.0/src/pyriak/system.py` & `pyriak-0.2.0/src/pyriak/system.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 __all__ = ['bind', 'System']
 
 from collections.abc import Callable, Hashable, Iterable
 from types import MappingProxyType, ModuleType
 from typing import TYPE_CHECKING, Any, TypeAlias, TypeVar, overload
 
-from pyriak import NoKey, NoKeyType, key_functions
+from pyriak import _SENTINEL
+from pyriak.eventkey import key_functions
 
 
 if TYPE_CHECKING:
-  from pyriak import Space
+  from pyriak.space import Space
 
 
 _T = TypeVar('_T')
+_R = TypeVar('_R')
 
-_Callback: TypeAlias = Callable[['Space', _T], Any]
+_Callback: TypeAlias = Callable[['Space', _T], _R]
 
 
 class _Binding:  #= public when expose event handlers
   __slots__ = 'priority', 'keys'
 
   def __init__(self, priority: Any, keys: frozenset[Hashable], /):
     self.priority = priority
@@ -40,56 +42,55 @@
 
   def __getattr__(self, name, /):
     return getattr(self._callback_, name)
 
 
 @overload
 def bind(
-  event_type: type[_T], priority: Any, /, *, key: Hashable | NoKeyType = NoKey
-) -> Callable[[_Callback[_T]], _Callback[_T]]: ...
+  event_type: type[_T], priority: Any, /
+) -> Callable[[_Callback[_T, _R]], _Callback[_T, _R]]: ...
 @overload
 def bind(
-  event_type: type[_T], priority: Any, /, *, keys: Iterable[Hashable] = ()
-) -> Callable[[_Callback[_T]], _Callback[_T]]: ...
+  event_type: type[_T], priority: Any, /, *, key: Hashable
+) -> Callable[[_Callback[_T, _R]], _Callback[_T, _R]]: ...
+@overload
 def bind(
-  event_type: type[_T], priority: Any, /, *, key: Hashable | NoKeyType = NoKey, keys=()
-) -> Callable[[_Callback[_T]], _Callback[_T]]:
+  event_type: type[_T], priority: Any, /, *, keys: Iterable[Hashable]
+) -> Callable[[_Callback[_T, _R]], _Callback[_T, _R]]: ...
+def bind(event_type, priority, /, *, key=_SENTINEL, keys=_SENTINEL):
   """Bind a callback to an event type.
 
 
   """
   if not isinstance(event_type, type):
     raise TypeError(f'{event_type!r} is not a type')
   try:
     hash(event_type)
   except TypeError:
     raise TypeError(f'{event_type!r} is not hashable') from None
-  if key is not NoKey:
-    if keys != ():
+  if key is not _SENTINEL:
+    if keys is not _SENTINEL:
       raise TypeError("bind() cannot be passed both 'key' and 'keys' kwargs")
     keys = frozenset([key])
   else:
-    keys = frozenset(keys)
-  if keys:
-    if not key_functions.exists(event_type):
-      raise ValueError(
-        f'bind(): keys were provided but no key function exists for {event_type!r}'
-      )
-    if NoKey in keys:
-      raise ValueError('NoKey cannot be a key')
-  def decorator(callback: _Callback[_T], /) -> _Callback[_T]:
+    keys = frozenset(keys) if keys is not _SENTINEL else frozenset()
+  if keys and not key_functions.exists(event_type):
+    raise ValueError(
+      f'bind(): keys were provided but no key function exists for {event_type!r}'
+    )
+  def decorator(callback: _Callback[_T, _R], /) -> _Callback[_T, _R]:
     if not isinstance(callback, _BindingWrapper):
-      return _BindingWrapper(callback, {event_type: _Binding(priority, keys)})  # type: ignore
+      return _BindingWrapper(callback, {event_type: _Binding(priority, keys)})
     bindings = callback._bindings_
     if event_type in bindings:
       raise ValueError(
         f'{event_type!r} is already bound to system event handler {callback._callback_!r}'
       )
     bindings[event_type] = _Binding(priority, keys)
-    return callback  # type: ignore
+    return callback
   return decorator
 
 
 class _SystemInfo:
   """Transitory object for initializing a system.
 
   Currently, this holds no configuration in the System constructor.
```

