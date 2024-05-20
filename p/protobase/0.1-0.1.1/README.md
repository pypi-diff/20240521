# Comparing `tmp/protobase-0.1.tar.gz` & `tmp/protobase-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protobase-0.1.tar", max compression
+gzip compressed data, was "protobase-0.1.1.tar", max compression
```

## Comparing `protobase-0.1.tar` & `protobase-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2024-01-28 02:44:22.902768 protobase-0.1/LICENSE
--rw-r--r--   0        0        0     1237 2024-01-28 02:44:22.906768 protobase-0.1/README.md
--rw-r--r--   0        0        0      618 2024-01-28 02:44:37.534661 protobase-0.1/pyproject.toml
--rw-r--r--   0        0        0       74 2024-01-28 02:44:22.906768 protobase-0.1/src/protobase/__init__.py
--rw-r--r--   0        0        0        0 2024-01-28 02:44:22.906768 protobase-0.1/src/protobase/annotations.py
--rw-r--r--   0        0        0     6377 2024-01-28 02:44:22.906768 protobase-0.1/src/protobase/core.py
--rw-r--r--   0        0        0      632 2024-01-28 02:44:22.906768 protobase-0.1/src/protobase/settings.py
--rw-r--r--   0        0        0      193 2024-01-28 02:44:22.906768 protobase-0.1/src/protobase/trait/__init__.py
--rw-r--r--   0        0        0     1425 2024-01-28 02:44:22.906768 protobase-0.1/src/protobase/trait/cmp.py
--rw-r--r--   0        0        0     1646 2024-01-28 02:44:22.906768 protobase-0.1/src/protobase/trait/consed.py
--rw-r--r--   0        0        0      350 2024-01-28 02:44:22.906768 protobase-0.1/src/protobase/trait/dynamic_attrs.py
--rw-r--r--   0        0        0     1623 2024-01-28 02:44:22.906768 protobase-0.1/src/protobase/trait/eq.py
--rw-r--r--   0        0        0      803 2024-01-28 02:44:22.906768 protobase-0.1/src/protobase/trait/hash.py
--rw-r--r--   0        0        0     1112 2024-01-28 02:44:22.906768 protobase-0.1/src/protobase/trait/init.py
--rw-r--r--   0        0        0      735 2024-01-28 02:44:22.906768 protobase-0.1/src/protobase/trait/inmutable.py
--rw-r--r--   0        0        0     1559 2024-01-28 02:44:22.906768 protobase-0.1/src/protobase/trait/repr.py
--rw-r--r--   0        0        0      549 2024-01-28 02:44:22.906768 protobase-0.1/src/protobase/trait/weak.py
--rw-r--r--   0        0        0     3344 2024-01-28 02:44:22.906768 protobase-0.1/src/protobase/utils.py
--rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 protobase-0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-20 22:35:35.989027 protobase-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5284 2024-05-20 22:35:35.989027 protobase-0.1.1/README.md
+-rw-r--r--   0        0        0      943 2024-05-20 22:35:49.725020 protobase-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      109 2024-05-20 22:35:35.993028 protobase-0.1.1/src/protobase/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 22:35:35.993028 protobase-0.1.1/src/protobase/annotations.py
+-rw-r--r--   0        0        0     3979 2024-05-20 22:35:35.993028 protobase-0.1.1/src/protobase/attr.py
+-rw-r--r--   0        0        0     8142 2024-05-20 22:35:35.993028 protobase-0.1.1/src/protobase/core.py
+-rw-r--r--   0        0        0      632 2024-05-20 22:35:35.993028 protobase-0.1.1/src/protobase/settings.py
+-rw-r--r--   0        0        0      335 2024-05-20 22:35:35.993028 protobase-0.1.1/src/protobase/traits/__init__.py
+-rw-r--r--   0        0        0     2996 2024-05-20 22:35:35.993028 protobase-0.1.1/src/protobase/traits/cmp.py
+-rw-r--r--   0        0        0     1803 2024-05-20 22:35:35.993028 protobase-0.1.1/src/protobase/traits/consed.py
+-rw-r--r--   0        0        0      350 2024-05-20 22:35:35.993028 protobase-0.1.1/src/protobase/traits/dynamic_attrs.py
+-rw-r--r--   0        0        0     1700 2024-05-20 22:35:35.993028 protobase-0.1.1/src/protobase/traits/hash.py
+-rw-r--r--   0        0        0     1693 2024-05-20 22:35:35.993028 protobase-0.1.1/src/protobase/traits/init.py
+-rw-r--r--   0        0        0     4138 2024-05-20 22:35:35.993028 protobase-0.1.1/src/protobase/traits/inmutable.py
+-rw-r--r--   0        0        0     1538 2024-05-20 22:35:35.993028 protobase-0.1.1/src/protobase/traits/repr.py
+-rw-r--r--   0        0        0      403 2024-05-20 22:35:35.993028 protobase-0.1.1/src/protobase/traits/weak.py
+-rw-r--r--   0        0        0     3177 2024-05-20 22:35:35.993028 protobase-0.1.1/src/protobase/utils.py
+-rw-r--r--   0        0        0     5918 1970-01-01 00:00:00.000000 protobase-0.1.1/PKG-INFO
```

### Comparing `protobase-0.1/LICENSE` & `protobase-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `protobase-0.1/src/protobase/core.py` & `protobase-0.1.1/src/protobase/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,163 +1,219 @@
 # %%
 from __future__ import annotations
 
+from functools import cached_property
 from itertools import chain
+from threading import RLock
 from types import (
     GetSetDescriptorType,
     MappingProxyType,
     MemberDescriptorType,
     MethodType,
 )
 from typing import (
     Any,
     Callable,
     Generic,
+    NamedTuple,
+    Optional,
+    ParamSpec,
+    TypeVar,
     dataclass_transform,
     get_type_hints,
 )
 
+
 from protobase.utils import mro_of_bases
 
 
 @dataclass_transform()
-class Meta(type):
+class ObjectMeta(type):
     """
     Metaclass for protobase classes.
 
     This metaclass is responsible for:
     - Generating the __slots__ attribute of the class.
     - Generating the __kwdefaults__ attribute of the class.
 
     NOTE: The default object instantiation protocol is overriden in
     protobase classes. The __new__ function is responsible for
     calling the __init__ function. This behaviour is choosen
     to allow Consign objects to be pickleable.
     """
 
+    # __kwargs__: dict[str, Any] ## implementamos como un ChainMap según el mro?
+
     __kwdefaults__: dict[str, Any]
     __attr_cache__: MappingProxyType(dict[str, Any])
 
     def __new__(
         mcs, name: str, bases: tuple[type, ...], namespace: dict[str, Any], **kwargs
     ):
         bases = mro_of_bases(bases)
 
         kwdefaults = {}
         base_slots = set()
 
         for base in reversed(bases):
             if base is object or base is Generic:
                 continue
-            if not isinstance(base, Meta):
+            if not isinstance(base, ObjectMeta):
                 raise TypeError(
                     f"Invalid base class: '{base.__qualname__}'."
                     f" All base classes must be 'proto.Base' classes."
                 )
 
             base_slots.update(base.__slots__)
             kwdefaults.update(base.__kwdefaults__)
 
         fields = namespace.get("__annotations__", {}).keys()
 
+        # TODO: filter annotations values starts by ClassVar[ or Annotation[ClassVar[
+
         for field in chain(fields, base_slots):
             if field in namespace:
                 kwdefaults[field] = namespace.pop(field)
 
         # if "__slots__" in namespace:
         #     raise TypeError("You cannot define '__slots__' in a ProtoBase class.")
-        slots = namespace.get("__slots__", ())
-        slots = slots + tuple(field for field in fields if field not in base_slots)
+        user_defined_slots = namespace.get("__slots__", ())
+        field_slots = tuple(field for field in fields if field not in base_slots)
+
+        for nm, attr in namespace.items():
+            if isinstance(attr, cached_property):
+                from protobase.attr import slot_cached
+
+                namespace[nm] = slot_cached(attr.func)
+
+        # cached_property_slots = tuple(
+        #     attr.__set_name__(None, nm)
+        #     for nm, attr in namespace.items()
+        #     if isinstance(attr, cached_slot)
+        # )
 
-        namespace["__slots__"] = tuple(slots)
         namespace["__kwdefaults__"] = kwdefaults
+        namespace["__slots__"] = (
+            *user_defined_slots,
+            *field_slots,
+            # *cached_property_slots,
+        )
 
         return type.__new__(mcs, name, tuple(bases), namespace)
 
     def __call__(cls, *args, **kwargs):
-        return cls.__new__(cls, *args, **kwargs)
+        return cls.__class_call__(*args, **kwargs)
+
+    def __class_call__(cls, *args, **kwargs):
+        self = cls.__new__(cls, *args, **kwargs)
+        self.__init__(*args, **kwargs)
+        return self
 
 
 @dataclass_transform()
-class Trait(metaclass=Meta):
+class Trait(metaclass=ObjectMeta):  # TODO: Quitar trait de la metaclase
     """
     Base class for all traits.
     Traits are classes whose instances are meant to be used as
     mixins for other classes.
     """
 
-    def __new__(cls, *args, **kwargs):
-        if not issubclass(cls, Base):
-            raise TypeError(f"Cannot instantiate trait '{cls.__qualname__}'")
-
-        obj = object.__new__(cls)
-        obj.__init__(*args, **kwargs)
-        return obj
-
-    def __getnewargs_ex__(self):
-        return (), {nm: getattr(self, nm) for nm in fields_of(self)}
-
-    def __getstate__(self):
+    @classmethod
+    def __check_type_hints__(cls):
         pass
 
-    def __setstate__(self, state):
-        pass
+    def __new__(cls, *args, **kwargs):
+        if is_trait(cls):
+            raise TypeError(
+                f"Cannot instantiate a bare trait class '{cls.__qualname__}'"
+            )
+
+        return object.__new__(cls)
 
 
 @dataclass_transform()
-class Base(Trait, metaclass=Meta):
+class Object(Trait, metaclass=ObjectMeta):
     """
     Base class for all protobase classes.
     """
 
-    def __init_subclass__(cls) -> None:
-        super().__init_subclass__()
+    # def __init_subclass__(cls) -> None:
+    #     super().__init_subclass__()
 
-        # Copy proto method descriptors from base traits
-        for base in cls.__bases__:
-            if base is object:
-                # if issubclass(base, Base) or base is object:
-                continue
+    #     # Pop front on the mro  the class descriptors for slots, protomethods
+    #     for base in cls.__mro__:
+    #         if not issubclass(base, Trait):
+    #             continue
+
+    #         # for nm in base.__slots__:
+    #         #     if not nm in cls.__dict__:
+    #         #         setattr(cls, nm, base.__dict__[nm])
+
+    #         for nm, item in base.__dict__.items():
+    #             if not isinstance(
+    #                 item, (trait_method, MemberDescriptorType, GetSetDescriptorType)
+    #             ):
+    #                 continue
+
+    #             if nm in cls.__dict__:
+    #                 continue
+
+    #             # cls.__dict__[nm] = item
+    #             setattr(cls, nm, item)
+
+
+#
+def is_trait(cls: type[Object]) -> bool:
+    return issubclass(cls, Trait) and not issubclass(cls, Object)
 
-            for nm, item in base.__dict__.items():
-                if nm in cls.__dict__:
-                    continue
-
-                if isinstance(
-                    item, (protomethod, MemberDescriptorType, GetSetDescriptorType)
-                ):
-                    # cls.__dict__[nm] = item
-                    setattr(cls, nm, item)
 
+class AttrInfo(NamedTuple):
+    name: str
+    type: type
+    default: Any
+    annotations: dict[str, Any]
 
-def fields_of(cls_or_obj: Meta | Base) -> MappingProxyType[str, Any]:
+
+def fields_of(cls: type[Object]) -> MappingProxyType[str, Any]:
     """
     Get the fields of a protobase class or object.
+
     """
-    if not hasattr(cls_or_obj, "__attr_cache__"):
-        cls_or_obj.__attr_cache__ = get_type_hints(cls_or_obj)
+    assert issubclass(cls, Object)
+
+    if "__attr_cache__" not in cls.__dict__:
+        hints = get_type_hints(cls)
+        cls.__attr_cache__ = hints
+        cls.__check_type_hints__()
 
     return MappingProxyType(
         {
             nm: tp
-            for nm, tp in cls_or_obj.__attr_cache__.items()
-            if not nm.startswith("_")
+            for nm, tp in cls.__dict__["__attr_cache__"].items()
+            # if not nm.startswith("_")
         }
     )
 
 
-class protomethod[**Args, RType]:
+Args = ParamSpec("Args")
+RType = TypeVar("RType")
+
+
+class proto_method: ...
+
+
+class trait_method(Generic[Args, RType]):
     """
 
     Example:
     >>> class MyTrait(proto.Trait):
-    ...     @proto.method
+    ...     @trait_method
     ...     def my_meth(self, x: int) -> str:
     ...         ...
-    >>> @MyTrait.my_meth.impl()
+    >>> @MyTrait.my_meth.implementer()
     ... async def _my_meth_impl(cls: type[MyTrait]):
     ...     fields = attrs(cls).keys()
     ...     return compile_function(
     ...         'my_meth',
     ...         'def my_meth(self): return  "HelloWorld"'
     ...     )
 
@@ -167,61 +223,67 @@
 
     Methods:
         impl(self) -> Callable[[Callable[[type[Base]]], Callable[Args, RType]]]:
         Decorator for setting the implementation function.
 
     """
 
-    __slots__ = (
-        "_proto_fn",
-        "_impl_fn",
-        "_owner",
-    )
-    _proto_fn: Callable
-    _impl_fn: Callable
-    _owner: type[Base]
-
-    def __init__(self, proto_fn: Callable[Args, RType] = None) -> None:
-        if proto_fn is not None:
-            self(proto_fn)
-
-    def __call__(self, proto_fn: Callable[Args, RType]):
-        self._proto_fn = proto_fn
-        return self
+    _trait_fn: Callable
+    _implementer: Callable
+    _implementations: dict[type[Object], Callable]
+
+    def __init__(self, trait_fn: Callable[Args, RType] = None) -> None:
+        self._trait_fn = trait_fn
+        self._implementer = None
+        self._implementations = {}
+
+    def __repr__(self):
+        return f"<trait_method {self._trait_fn.__name__}>"
+
+    def implementer(
+        self, implementer_fn: Callable[[type[Object]], Callable[Args, RType]]
+    ) -> Callable:
+        assert self._implementer is None, "Cannot reassign the implementation function."
+        self._implementer = implementer_fn
+        return implementer_fn
 
     def __set_name__(self, owner, name):
-        if self._proto_fn.__name__ != name:
-            raise NameError(
-                f"Cannot define a protobase method '{name}' with a different name than '{self._proto_fn.__name__}'"
-            )
-        if not issubclass(owner, Trait) or issubclass(owner, Base):
+        if not is_trait(owner):
             raise TypeError(
                 f"Cannot define a protobase method '{name}' in a non-trait only class '{owner.__qualname__}'"
             )
-        self._owner = owner
+        if name != self._trait_fn.__name__:
+            raise NameError(
+                f"Cannot define a protomethod '{name}' with a different name than '{self._trait_fn.__name__}'"
+            )
+        # self._owner = owner
 
     def __get__(self, obj, objtype=None):
         if obj is None:
             return self
 
-        assert issubclass(objtype, Base)
+        fn = self._implementations.get(objtype, None)
 
-        fn = self._impl_fn(objtype)
-        fn.__name__ = self._proto_fn.__name__
-        fn.__module__ = self._proto_fn.__module__
-        fn.__doc__ = self._proto_fn.__doc__
+        if fn is None:
+            assert not is_trait(objtype)
 
-        setattr(objtype, self._proto_fn.__name__, fn)  # se sobreescribe el descriptor
+            if self._implementer is None:
+                raise TypeError(
+                    f"Cannot find an implementation function for '{self._trait_fn.__name__}'"
+                )
 
-        return MethodType(fn, obj)
+            fn = self._implementer(objtype)
+            fn.__name__ = self._trait_fn.__name__
+            fn.__module__ = self._trait_fn.__module__
+            fn.__doc__ = self._trait_fn.__doc__
 
+            self._implementations[objtype] = fn
 
-def impl(target: protomethod):
-    """
-    Decorator for setting the implementation function of a protobase method.
-    """
+        return MethodType(fn, obj)
 
-    def impl_decorator(impl_fn):
-        target._impl_fn = impl_fn
-        return impl_fn
 
-    return impl_decorator
+@dataclass_transform()
+def protobase():
+    def protobase_decorator(cls):
+        return cls
+
+    return protobase_decorator
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `protobase-0.1/src/protobase/settings.py` & `protobase-0.1.1/src/protobase/settings.py`

 * *Files identical despite different names*

### Comparing `protobase-0.1/src/protobase/trait/consed.py` & `protobase-0.1.1/src/protobase/traits/consed.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from weakref import WeakKeyDictionary, ref
 
-from protobase.core import Trait
-from protobase.trait.eq import Eq
-from protobase.trait.hash import Hash
-from protobase.trait.init import Init
-from protobase.trait.inmutable import Inmutable
-from protobase.trait.weak import Weak
+from protobase.core import Object, Trait
 
+from .cmp import Eq
+from .hash import Hash
+from .init import Init
+from .inmutable import Inmutable
+from .weak import Weak
 
-class Consed(Eq, Hash, Inmutable, Init, Weak, Trait):
+
+class Consed(Hash, Eq, Inmutable, Init, Weak, Trait):
     """
     Trait for a class that is a hash-consed object.
     Conses objects are objects that are unique for each set of field values.
     They have a fixed identity and can be compared with 'is'.
 
     Example:
         >>> class Foo(Base, Consed):
@@ -24,24 +25,31 @@
         >>> a is b
         True
         >>> c = Foo(1, 2, 4)
         >>> a is c
         False
     """
 
+    __slots__ = ("__hash_cache__",)
+
     def __init_subclass__(cls) -> None:
         super().__init_subclass__()
-        cls.__consing__ = WeakKeyDictionary()
+        if issubclass(cls, Object):
+            cls.__consing__ = WeakKeyDictionary()
 
     def __new__(cls, *args, **kwargs):
-        obj = super().__new__(cls, *args, **kwargs)
-        if obj in cls.__consing__:
-            return cls.__consing__[obj]()
-        cls.__consing__[obj] = ref(obj)
-        return obj
+        self = super().__new__(cls, *args, **kwargs)
+        try:
+            if self in cls.__consing__:
+                return cls.__consing__[self]()
+        except TypeError as exc:
+            raise ValueError(f"Cannot hash-consed mutable object: {self}") from exc
+
+        cls.__consing__[self] = ref(self)
+        return self
 
 
 def consed_count(cls: type[Consed]) -> int:
     """
     Returns the number of instances of `Consed` class.
 
     Args:
```

### Comparing `protobase-0.1/src/protobase/trait/eq.py` & `protobase-0.1.1/src/protobase/traits/init.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,64 @@
-from typing import Self
-from protobase.core import Trait, fields_of, impl, protomethod
+from typing import Any
+from protobase import attr
+from protobase.core import Trait, Object, fields_of, trait_method
 from protobase.utils import compile_function
 
 
-class Eq(Trait):
+class Init(Trait):
     """
-    A trait that enables equality operators (__eq__, __ne__) based on
-    the fields of a proto object.
+    Trait for initializing fields on a class.
+    This trait automatically generates an __init__ method for the class, with
+    keyword-only arguments for each field.
 
     Example:
-
-        >>> from protobase.core import Base
-        >>> from protobase.trait import Eq
-        >>>
-        >>> class Point(Base, Eq):
-        ...     x: int
-        ...     y: int
-        ...
-        >>> p1 = Point(x=1, y=2)
-        >>> p2 = Point(x=2, y=1)
-        >>> p3 = Point(x=1, y=2)
-        >>> p1 == p2
-        False
-        >>> p1 == p3
-        True
-        >>> p1 != p2
-        True
-        >>> p1 != p3
-        False
+        >>> class Foo(Base, Init):
+        ...     x: int = 1
+        ...     y: int = 2
+        >>> foo = Foo(x=3)
+        >>> foo.x
+        3
+        >>> foo.y
+        2
     """
 
-    @protomethod()
-    def __eq__(self, other: Self) -> bool:
-        ...
-
-    @protomethod()
-    def __ne__(self, other: Self) -> bool:
-        ...
-
-
-@impl(Eq.__eq__)
-def _impl_eq(cls: type[Eq]):
-    fields = fields_of(cls).keys()
+    @trait_method
+    def __init__(self, *args, **kwargs):
+        raise NotImplementedError()
+
+    @trait_method
+    def __getstate__(self) -> dict[str, Any]: ...
+
+    def __setstate__(self, state: dict[str, Any]) -> None:
+        self.__init__(**state)
+
+
+@Init.__init__.implementer
+def _impl_init(cls: type[Object]):
+    fields = fields_of(cls)
+
+    if len(fields) == 0:
+        return compile_function(
+            "def __init__(self):",
+            "    pass",
+        )
 
     return compile_function(
-        "__eq__",
-        "def __eq__(self, other):",
-        "    if self is other: return True",
-        "    if type(self) != type(other): return NotImplemented",
-        f"    return ({' and '.join(f'self.{field} == other.{field}' for field in fields)})",
+        f"def __init__(self, *, {", ".join(fields)}):",
+        *[f"    global {field}_setter" for field in fields],
+        *[f"    {field}_setter(self, {field})" for field in fields],
+        globals={f"{field}_setter": attr.setter(cls, field) for field in fields},
+        __kwdefaults__=cls.__kwdefaults__,
+        # __defaults__=cls.__defaults__,
     )
 
 
-@impl(Eq.__ne__)
-def _impl_ne(cls: type[Eq]):
-    fields = fields_of(cls).keys()
+@Init.__getstate__.implementer
+def _impl_getstate(cls: type[Object]):
+    fields = fields_of(cls)
+
+    params = ", ".join(f"{field}=self.{field}" for field in fields)
 
     return compile_function(
-        "__ne__",
-        "def __ne__(self, other):",
-        "    if self is other: return False",
-        "    if type(self) != type(other): return NotImplemented",
-        f"    return ({' or '.join(f'self.{field} != other.{field}' for field in fields)})",
+        "def __getstate__(self):",
+        f"    return dict({params})",
     )
```

### Comparing `protobase-0.1/src/protobase/utils.py` & `protobase-0.1.1/src/protobase/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 from itertools import chain
+
+import re
+from types import ModuleType
 from typing import Any, Callable, Sequence
 
 
 def _mro(cls):
     if cls is object:
         return [object]
     return [cls] + _mro_merge([_mro(base) for base in cls.__bases__])
@@ -20,75 +23,68 @@
         raise TypeError("No legal mro")
 
 
 def mro_of_bases(bases: Sequence[type]):
     return _mro_merge([_mro(base) for base in bases])
 
 
-def attr_lookup(cls: type, nm: str):
-    """
-    Look up a attribute by name in the class hierarchy without
-    triggering the __getattribute__ mechanism.
-
-    Args:
-        cls (type): The class to search in.
-        nm (str): The name of the descriptor to look up.
-
-    Returns:
-        object: The descriptor object.
-
-    Raises:
-        AttributeError: If the descriptor cannot be found in the class hierarchy.
-
-    """
-    for base in cls.__mro__:
-        if nm in base.__dict__:
-            return base.__dict__[nm]
-    raise AttributeError(f"Cannot find '{nm}' in '{cls.__qualname__}'")
+FN_NAME_RE = re.compile("^def\s(\w+)")
 
 
 def compile_function(
-    name: str,
     *source,
     locals: dict[str, Any] | None = None,
     globals: dict[str, Any] | None = None,
     **kwargs,
 ) -> Callable:
     """
     Compile a function from source code.
 
     Args:
         name (str): The name of the function.
-        *source: The source code of the function.
+        source: The source code of the function.
         locals (dict[str, Any] | None, optional): Local variables to be used during execution. Defaults to None.
         globals (dict[str, Any] | None, optional): Global variables to be used during execution. Defaults to None.
-        **kwargs: Additional keyword arguments to be set as attributes of the compiled function.
+        kwargs: Additional keyword arguments to be set as attributes of the compiled function.
 
     Returns:
         Callable: The compiled function.
+
     Example:
         >>> fn = compile_function(
-        ...     "foo",
         ...     "def foo(x: int, y: int) -> int:",
         ...     "    return x + y",
         ... )
         >>> fn(1, 2)
         3
         >>> fn.__source__
-        'def foo(x: int, y: int) -> int:\n    return x + y\n    \n    \n'
+        def foo(x: int, y: int) -> int:\n    return x + y\n    \n    \n
+
     """
     if locals is None:
         locals = {}
 
     source = "\n".join(source)
-    exec(source, globals, locals)
-    fn = locals[name]
+
+    try:
+        fn_name = FN_NAME_RE.match(source).group(1)
+    except:
+        raise ValueError("Cannot find function name in source code.")
+
+    try:
+        exec(source, globals, locals)
+    except SyntaxError as e:
+        raise SyntaxError(f"{e.msg} in source code:\n{source}")
+
+    fn = locals[fn_name]
     fn.__source__ = source
+
     for nm, val in kwargs.items():
         setattr(fn, nm, val)
+
     return fn
 
 
 def slots_of(cls: type):
     """
     Returns a tuple of all the slots defined in the class and its base classes.
 
@@ -117,7 +113,14 @@
 
 def can_import(module: str) -> bool:
     try:
         __import__(module)
         return True
     except ImportError:
         return False
+
+
+def try_import(module: str) -> ModuleType:
+    try:
+        return __import__(module)
+    except ImportError:
+        return None
```

