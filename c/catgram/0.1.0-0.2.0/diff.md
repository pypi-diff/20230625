# Comparing `tmp/catgram-0.1.0.tar.gz` & `tmp/catgram-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catgram-0.1.0.tar", max compression
+gzip compressed data, was "catgram-0.2.0.tar", max compression
```

## Comparing `catgram-0.1.0.tar` & `catgram-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-04-09 07:25:13.612244 catgram-0.1.0/LICENSE
--rw-r--r--   0        0        0     1351 2023-05-26 07:24:25.513582 catgram-0.1.0/README.md
--rw-r--r--   0        0        0      137 2023-05-26 06:09:48.351744 catgram-0.1.0/catgram/__init__.py
--rw-r--r--   0        0        0    15884 2023-05-26 06:27:32.233460 catgram-0.1.0/catgram/category_tree.py
--rw-r--r--   0        0        0     9260 2023-05-26 06:35:04.186455 catgram-0.1.0/catgram/term_graph.py
--rw-r--r--   0        0        0      714 2023-05-26 06:59:45.263749 catgram-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2155 1970-01-01 00:00:00.000000 catgram-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-06-01 01:00:07.993420 catgram-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7035 2023-06-25 00:47:42.218613 catgram-0.2.0/README.md
+-rw-r--r--   0        0        0      112 2023-06-24 22:12:32.374566 catgram-0.2.0/catgram/__init__.py
+-rw-r--r--   0        0        0    16815 2023-06-24 22:13:23.558176 catgram-0.2.0/catgram/category_tree.py
+-rw-r--r--   0        0        0        0 2023-06-24 22:06:40.002658 catgram-0.2.0/catgram/ccg/__init__.py
+-rw-r--r--   0        0        0    11310 2023-06-18 19:49:35.602078 catgram-0.2.0/catgram/ccg/candc_ignore.py
+-rw-r--r--   0        0        0    13739 2023-06-24 22:20:51.792620 catgram-0.2.0/catgram/ccg/dependencies.py
+-rw-r--r--   0        0        0    12542 2023-06-24 22:15:21.751929 catgram-0.2.0/catgram/ccg/heads.py
+-rw-r--r--   0        0        0        0 2023-06-24 22:08:43.796662 catgram-0.2.0/catgram/cli/__init__.py
+-rwxr-xr-x   0        0        0     5032 2023-06-24 22:54:36.321165 catgram-0.2.0/catgram/cli/ccg_depeval.py
+-rwxr-xr-x   0        0        0     1827 2023-06-24 22:11:28.844222 catgram-0.2.0/catgram/cli/ccg_roots.py
+-rw-r--r--   0        0        0     9155 2023-06-24 22:13:34.418234 catgram-0.2.0/catgram/term_graph.py
+-rw-r--r--   0        0        0      822 2023-06-24 22:32:39.838647 catgram-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7839 1970-01-01 00:00:00.000000 catgram-0.2.0/PKG-INFO
```

### Comparing `catgram-0.1.0/LICENSE` & `catgram-0.2.0/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -170,32 +170,7 @@
       on Your own behalf and on Your sole responsibility, not on behalf
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
```

### Comparing `catgram-0.1.0/catgram/category_tree.py` & `catgram-0.2.0/catgram/category_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-#!/usr/bin/env python3
-
 from dataclasses import dataclass
 from functools import cache, cached_property
 import logging
 import re
-from typing import ClassVar, overload
+from typing import ClassVar, overload, Optional
 
 try:
     from typing import Self  # Python 3.11+
 except ImportError:
-    from typing import TypeVar
+    from typing import TypeAlias
 
-    Self = TypeVar("Self", bound="CategoryTree")
+    Self: TypeAlias = "CategoryTree"
 
 
 @dataclass(frozen=True, repr=False)
 class CategoryTree:
     """A tree representation of a category."""
 
     atom_re: ClassVar[re.Pattern] = re.compile(r"^[^\s/\\()]+$")
     atom_delim: ClassVar[re.Pattern] = re.compile(r"([()\\/])")
 
     root: str
-    result: Self | None = None
-    argument: Self | None = None
+    result: Optional[Self] = None
+    argument: Optional[Self] = None
 
     def __post_init__(self: Self):
         # validate the fields' values
         if not isinstance(self.root, str):
             raise TypeError(f"root must be {str} instance; got {self.root!r}")
         if self.result is None:
             if self.argument is not None:
@@ -78,16 +76,16 @@
                 that can be straightforwardly corrected.
 
         Returns:
             CategorTree: The CategoryTree representation of the input category.
         """
         if (key := (cat, lambek)) in INSTANCES:
             return INSTANCES[key]
-        cat = tuple(a for a in cls.atom_delim.split(cat) if a)
-        return cls._parse_str(cat, left_associative, lambek, strict)[0]
+        cat_ = tuple(a for a in cls.atom_delim.split(cat) if a)
+        return cls._parse_str(cat_, left_associative, lambek, strict)[0]
 
     @classmethod
     def _parse_str(
         cls,
         cat: tuple[str],
         l_assoc: bool,
         lambek: bool,
@@ -203,40 +201,40 @@
                 msg = f'nclosed parenthetical in "{"".join(cat)}" at index {i}'
                 if strict:
                     raise MalformedCategoryError(f"U{msg}")
                 logging.warning(f"Ignoring u{msg}")
         if root is None:
             raise MalformedCategoryError("Empty category")
 
-        cat = "".join(cat[idx:i])
+        cat_ = "".join(cat[idx:i])
         if isinstance(root, cls):
-            logging.warning(f'Stripping redundant parentheses in "{cat}"')
-            cat = cat[1:-1]
+            logging.warning(f'Stripping redundant parentheses in "{cat_}"')
+            cat_ = cat_[1:-1]
             # TODO: nix sanity check after adding some tests
-            assert root == INSTANCES[cat, lambek]
+            assert root == INSTANCES[cat_, lambek]
             return root, i
         if root in "/\\" and right is None:
             raise MalformedCategoryError(
-                f'Missing right node after "{root}" at index {i} in "{cat}"'
+                f'Missing right node after "{root}" at index {i} in "{cat_}"'
             )
 
-        key = cat, lambek
+        key = cat_, lambek
         if key in INSTANCES:
-            cat = INSTANCES[key]
+            cat_ = INSTANCES[key]
             # TODO: nix sanity check after adding some tests
             if lambek and root == "\\":
-                assert cat == cls(root, right, left)
+                assert cat_ == cls(root, right, left)
             else:
-                assert cat == cls(root, left, right)
+                assert cat_ == cls(root, left, right)
         elif lambek and root == "\\":
-            INSTANCES[key] = cat = cls(root, right, left)
+            INSTANCES[key] = cat_ = cls(root, right, left)
         else:
-            INSTANCES[key] = cat = cls(root, left, right)
+            INSTANCES[key] = cat_ = cls(root, left, right)
 
-        return cat, i
+        return cat_, i
 
     @cached_property
     def is_complex(self: Self) -> bool:
         """Whether this category is complex (i.e., not atomic)."""
         return not self.is_atomic
 
     @cached_property
@@ -340,19 +338,19 @@
         l_assoc: bool = False,
         lambek: bool = False,
     ) -> str | tuple[str, int]:
         """String representation of this category
 
         Args:
             pol_start: If not None, add an index to each atomic category
-              that indicates the position of that (polarized) primitive in the
-              lexical decomposition of the category. The integer value of this
-              parameter specifies the offset to use for the first index.
+                that indicates the position of that (polarized) primitive in
+                the lexical decomposition of the category. The integer value of
+                this parameter specifies the offset to use for the first index.
             positive: Whether the category has positive polarity. Has no effect
-              if `pol_start_idx` is None.
+                if `pol_start_idx` is None.
             l_assoc: Whether to use left-associative notation
             lambek: Whether to use Lambek notation
         Returns:
             If `pol_start_idx` is None, returns a string representation of this
             category according to the specified notation. If `pol_start_idx` is
             not None, returns a 2-tuple: the first element is the string
             representation of this category and the second element is the final
@@ -372,15 +370,18 @@
             seq[i] = f"{seq_[i]}_{pol_start + j}"
         return "".join(seq), pol_start + len(leaf_idxs)
 
     def __repr__(self: Self) -> str:
         # cls = self.__class__.__name__
         # if self.is_atomic:
         #    return f"{cls}({self.root})"
-        # return f"{cls}(result={self.result!r}, root={self.root}, argument={self.argument!r})"
+        # return (
+        #     f"{cls}(result={self.result!r}, root={self.root}, "
+        #     f"argument={self.argument!r})"
+        # )
         # The above can get pretty long for larger categories, so just use the
         # string representation wrapped in the class name.
         return f"{self.__class__.__name__}({self.to_str()})"
 
     @cache
     def _inorder(
         self: Self, l_assoc: bool, lambek: bool, positive: bool
@@ -401,13 +402,38 @@
             offset = len(result_idxs)
             argument_idxs = tuple(i + offset for i in argument_idxs)
 
         if lambek and self.root == "\\":
             return argument + (self.root,) + result, argument_idxs + result_idxs
         return result + (self.root,) + argument, result_idxs + argument_idxs
 
+    @cached_property
+    def func_seq(self: Self) -> tuple[str, ...]:
+        """
+        The functorial sequence that this category decomposes into, as defined
+        by Bhargava and Penn (ACL 2023).
+        """
+        if self.is_atomic:
+            return (self.root,)
+        argument_str = self.argument.to_str()
+        if self.argument.is_atomic:
+            argument_str = f"{self.root}{argument_str}"
+        else:
+            argument_str = f"{self.root}({argument_str})"
+        return self.result.func_seq + (argument_str,)
+
+    @cache
+    def get_arg(self: Self, slot: int) -> Self:
+        if slot > self.arity:
+            raise ValueError(
+                f"invalid slot {slot!r} for category {self} with arity {self.arity}"
+            )
+        if slot == self.arity:
+            return self.argument if slot else self
+        return self.result.get_arg(slot)
+
 
 class MalformedCategoryError(Exception):
     pass
 
 
 INSTANCES: dict[tuple[str, bool], CategoryTree] = {}
```

### Comparing `catgram-0.1.0/catgram/term_graph.py` & `catgram-0.2.0/catgram/term_graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-#!/usr/bin/env python3
-
 from collections.abc import Mapping, Sequence
 from functools import cache
 import re
 from typing import NamedTuple
 
 try:
     from typing import Self  # Python 3.11+
 except ImportError:
-    from typing import TypeVar
+    from typing import TypeAlias
 
-    Self = TypeVar("Self", bound="LexicalDecomposition")
+    Self: TypeAlias = "LexicalDecomposition"
 
 from lambda_calculus import terms
 
 from catgram import CategoryTree
 
 
 class ProofFrameNode(NamedTuple):
@@ -49,15 +47,15 @@
       order indicated by the decomposition rules.
     * The `edges` field is a tuple of integer 2-tuples, indicating the source
       and destination indices of the nodes (as in the `nodes` tuple) for each
       edge (regular or Lambek) as constructed by the lexical decomposition.
     * The `target` field is the index of the node in the `nodes` tuple
       corresponding to the "target" atom of the lexical category. The target
       node is the root node of the lexical decomposition. In constructing
-      semantic terms in term graphs, word labels are assigned to target atoms.
+      semantic terms in term graphs, token labels are assigned to target atoms.
     """
 
     nodes: tuple[ProofFrameNode, ...]
     edges: tuple[tuple[int, int], ...]
     target: int
 
     @classmethod
@@ -106,17 +104,15 @@
                 nodes = list(result.nodes)
                 nodes[result.target] = nodes[result.target]._replace(
                     children=(edge[1] - edge[0],) + target.children
                 )
                 right = result._replace(nodes=tuple(nodes))
                 # left, right = argument, result
             case _:
-                raise ValueError(
-                    f"Invalid polarized category: ({category}){'+' if positive else '-'}"
-                )
+                raise ValueError(f"invalid category: {category}")
 
         nodes = left.nodes + right.nodes
         edges = [
             edge,
             *left.edges,
             *[(src + shift, dst + shift) for src, dst in right.edges],
         ]
@@ -140,15 +136,15 @@
         *,
         sentential: int | None = 0,
         linkage: Mapping[int, int] | None = None,
         words: Sequence | None = None,
     ):
         """
         Construct a term graph for the given sequent and linkage with optional
-        word labels.
+        token labels.
 
         Args:
             categories: A `Sequence` of any combination of `CategoryTree`s,
                 `str`s, and `None`s. Strings are converted to `CategoryTree`s
                 and `None` categories can be useful for representing words with
                 no lexical category, a convention sometimes used for some
                 punctuation (e.g., in LCGbank).
@@ -209,21 +205,21 @@
         ):
             if decomp is None:
                 continue
             self.labels[clen + decomp.target] = word
 
     def get_term(self, idx: int = 0) -> terms.Term:
         """
-        Get the semantic term for the word at the given index.
+        Get the semantic term for the token at the given index.
 
         Args:
-            idx (int): The index for the word.
+            idx (int): The index for the token.
 
         Returns:
-            Term: the semantic term for the word as situated in the term graph.
+            Term: the semantic term for the token as situated in the term graph.
                 If the index provided is that of the sentential category and
                 `self` is a valid term graph, this will return the semantic
                 term for the entire sentence.
         """
         return self._get_term(self.clens[idx] + self.decomps[idx].target)
 
     def _get_term(self, idx: int) -> terms.Term:
```

### Comparing `catgram-0.1.0/pyproject.toml` & `catgram-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "catgram"
-version = "0.1.0"
+version = "0.2.0"
 description = "Basic tools for working with categorial grammars"
 license = "Apache-2.0"
 authors = ["Aditya Bhargava <aditya@cs.toronto.edu>"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
@@ -13,14 +13,17 @@
 readme = "README.md"
 repository = "https://github.com/rightaditya/catgram"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 lambda-calculus = "^3.0.0"
 
-
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 
+[tool.poetry.scripts]
+ccg_depeval = 'catgram.cli.ccg_depeval:main'
+ccg_roots = 'catgram.cli.ccg_roots:main'
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

