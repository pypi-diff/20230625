# Comparing `tmp/dronefly_core-0.3.6.dev5.tar.gz` & `tmp/dronefly_core-0.3.6.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dronefly_core-0.3.6.dev5.tar", max compression
+gzip compressed data, was "dronefly_core-0.3.6.dev6.tar", max compression
```

## Comparing `dronefly_core-0.3.6.dev5.tar` & `dronefly_core-0.3.6.dev6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    56815 2023-04-16 13:37:18.956988 dronefly_core-0.3.6.dev5/LICENSE
--rw-r--r--   0        0        0      702 2023-01-28 19:16:26.368426 dronefly_core-0.3.6.dev5/README.md
--rw-r--r--   0        0        0       53 2023-01-29 15:27:41.654095 dronefly_core-0.3.6.dev5/dronefly/core/__init__.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev5/dronefly/core/clients/__init__.py
--rw-r--r--   0        0        0     1028 2023-03-13 15:05:57.725989 dronefly_core-0.3.6.dev5/dronefly/core/clients/inat.py
--rw-r--r--   0        0        0     8043 2023-06-22 17:27:01.514036 dronefly_core-0.3.6.dev5/dronefly/core/commands/__init__.py
--rw-r--r--   0        0        0      635 2023-03-19 08:14:11.111276 dronefly_core-0.3.6.dev5/dronefly/core/constants.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev5/dronefly/core/formatters/__init__.py
--rw-r--r--   0        0        0      445 2023-04-16 10:53:39.829302 dronefly_core-0.3.6.dev5/dronefly/core/formatters/constants.py
--rw-r--r--   0        0        0    35801 2023-06-22 17:32:04.480260 dronefly_core-0.3.6.dev5/dronefly/core/formatters/generic.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.624333 dronefly_core-0.3.6.dev5/dronefly/core/models/__init__.py
--rw-r--r--   0        0        0     1753 2023-04-09 09:38:32.529718 dronefly_core-0.3.6.dev5/dronefly/core/models/controlled_terms.py
--rw-r--r--   0        0        0      188 2023-03-13 15:15:33.501579 dronefly_core-0.3.6.dev5/dronefly/core/models/user.py
--rw-r--r--   0        0        0       49 2023-01-29 15:28:49.919496 dronefly_core-0.3.6.dev5/dronefly/core/parsers/__init__.py
--rw-r--r--   0        0        0     3721 2023-06-14 15:48:19.092273 dronefly_core-0.3.6.dev5/dronefly/core/parsers/constants.py
--rw-r--r--   0        0        0     9291 2023-02-18 13:51:02.476816 dronefly_core-0.3.6.dev5/dronefly/core/parsers/natural.py
--rw-r--r--   0        0        0     6329 2023-03-19 08:21:31.268129 dronefly_core-0.3.6.dev5/dronefly/core/parsers/unixlike.py
--rw-r--r--   0        0        0     2346 2023-01-29 15:35:29.175688 dronefly_core-0.3.6.dev5/dronefly/core/parsers/url.py
--rw-r--r--   0        0        0       51 2023-01-29 15:27:27.497804 dronefly_core-0.3.6.dev5/dronefly/core/query/__init__.py
--rw-r--r--   0        0        0    21941 2023-06-18 15:05:34.396886 dronefly_core-0.3.6.dev5/dronefly/core/query/query.py
--rw-r--r--   0        0        0     1366 2023-06-18 14:57:16.774410 dronefly_core-0.3.6.dev5/dronefly/core/utils/__init__.py
--rw-r--r--   0        0        0      741 2023-06-22 17:38:46.644562 dronefly_core-0.3.6.dev5/pyproject.toml
--rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev5/setup.py
--rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev5/PKG-INFO
+-rw-r--r--   0        0        0    56815 2023-04-16 13:37:18.956988 dronefly_core-0.3.6.dev6/LICENSE
+-rw-r--r--   0        0        0      702 2023-01-28 19:16:26.368426 dronefly_core-0.3.6.dev6/README.md
+-rw-r--r--   0        0        0       53 2023-01-29 15:27:41.654095 dronefly_core-0.3.6.dev6/dronefly/core/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev6/dronefly/core/clients/__init__.py
+-rw-r--r--   0        0        0     1028 2023-03-13 15:05:57.725989 dronefly_core-0.3.6.dev6/dronefly/core/clients/inat.py
+-rw-r--r--   0        0        0     9888 2023-06-25 13:22:40.463140 dronefly_core-0.3.6.dev6/dronefly/core/commands/__init__.py
+-rw-r--r--   0        0        0      635 2023-03-19 08:14:11.111276 dronefly_core-0.3.6.dev6/dronefly/core/constants.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev6/dronefly/core/formatters/__init__.py
+-rw-r--r--   0        0        0      445 2023-04-16 10:53:39.829302 dronefly_core-0.3.6.dev6/dronefly/core/formatters/constants.py
+-rw-r--r--   0        0        0    37682 2023-06-25 13:22:17.490660 dronefly_core-0.3.6.dev6/dronefly/core/formatters/generic.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.624333 dronefly_core-0.3.6.dev6/dronefly/core/models/__init__.py
+-rw-r--r--   0        0        0     1753 2023-04-09 09:38:32.529718 dronefly_core-0.3.6.dev6/dronefly/core/models/controlled_terms.py
+-rw-r--r--   0        0        0      188 2023-03-13 15:15:33.501579 dronefly_core-0.3.6.dev6/dronefly/core/models/user.py
+-rw-r--r--   0        0        0       49 2023-01-29 15:28:49.919496 dronefly_core-0.3.6.dev6/dronefly/core/parsers/__init__.py
+-rw-r--r--   0        0        0     3721 2023-06-14 15:48:19.092273 dronefly_core-0.3.6.dev6/dronefly/core/parsers/constants.py
+-rw-r--r--   0        0        0     9291 2023-02-18 13:51:02.476816 dronefly_core-0.3.6.dev6/dronefly/core/parsers/natural.py
+-rw-r--r--   0        0        0     6329 2023-03-19 08:21:31.268129 dronefly_core-0.3.6.dev6/dronefly/core/parsers/unixlike.py
+-rw-r--r--   0        0        0     2346 2023-01-29 15:35:29.175688 dronefly_core-0.3.6.dev6/dronefly/core/parsers/url.py
+-rw-r--r--   0        0        0       51 2023-01-29 15:27:27.497804 dronefly_core-0.3.6.dev6/dronefly/core/query/__init__.py
+-rw-r--r--   0        0        0    21941 2023-06-18 15:05:34.396886 dronefly_core-0.3.6.dev6/dronefly/core/query/query.py
+-rw-r--r--   0        0        0     1366 2023-06-18 14:57:16.774410 dronefly_core-0.3.6.dev6/dronefly/core/utils/__init__.py
+-rw-r--r--   0        0        0      741 2023-06-25 13:23:17.247908 dronefly_core-0.3.6.dev6/pyproject.toml
+-rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev6/setup.py
+-rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev6/PKG-INFO
```

### Comparing `dronefly_core-0.3.6.dev5/LICENSE` & `dronefly_core-0.3.6.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev5/README.md` & `dronefly_core-0.3.6.dev6/README.md`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev5/dronefly/core/clients/inat.py` & `dronefly_core-0.3.6.dev6/dronefly/core/clients/inat.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev5/dronefly/core/commands/__init__.py` & `dronefly_core-0.3.6.dev6/dronefly/core/commands/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 from enum import Enum
 import re
+from typing import Union
 
 from attrs import define
 from rich.markdown import Markdown
 
 from ..clients.inat import iNatClient
 from ..constants import INAT_DEFAULTS, INAT_USER_DEFAULT_PARAMS, RANK_KEYWORDS
 
 from ..parsers import NaturalParser
-from ..formatters.generic import LifeListFormatter, ObservationFormatter, TaxonFormatter
+from ..formatters.generic import (
+    BaseFormatter,
+    LifeListFormatter,
+    ListFormatter,
+    ObservationFormatter,
+    TaxonFormatter,
+)
 from ..models.user import User
 from ..query.query import get_base_query_args, QueryResponse
 
 
 RICH_BQ_NEWLINE_PAT = re.compile(r"^(\> .*?)\n(?=\> )", re.MULTILINE)
 RICH_BQ_END_PAT = re.compile(r"^((\> .*?\n)+)(?!> )", re.MULTILINE)
 RICH_NO_BQ_NEWLINE_PAT = re.compile(r"^(?!\> )(.+?)(\n)(?!$|\> )", re.MULTILINE)
@@ -25,14 +32,24 @@
 
 
 @define
 class Context:
     """A Dronefly command context."""
 
     author: User = User()
+    # Optional page formatter and current page:
+    # - Provides support for next & prev commands to navigate through
+    #   paged command results.
+    # - Every command providing paged results must:
+    #   - Set page_formatter to the formatter for the new results.
+    #   - Set page to the initial page number (default: 0).
+    # - Therefore, only a single command providing paged results can
+    #   be active at a time.
+    page_formatter: Union[BaseFormatter, ListFormatter] = None
+    page: int = 0
 
     def get_inat_user_default(self, inat_param: str):
         """Return iNat API default for user param default, if any, otherwise global default."""
         if inat_param not in INAT_USER_DEFAULT_PARAMS:
             return None
         if self.author:
             default = getattr(self.author, inat_param, None) or INAT_DEFAULTS.get(
@@ -67,16 +84,19 @@
     inat_client: iNatClient = iNatClient()
     parser: NaturalParser = NaturalParser()
     format: Format = Format.discord_markdown
 
     def _parse(self, query_str):
         return self.parser.parse(query_str)
 
-    def _format_markdown(self, formatter):
-        markdown_text = formatter.format()
+    def _format_markdown(self, formatter, page: int = 0):
+        if getattr(formatter, "format_page", None):
+            markdown_text = formatter.format_page(page)
+        else:
+            markdown_text = formatter.format()
         if self.format == Format.rich:
             # Richify the markdown:
             # - In Discord markdown, all newlines are rendered as line breaks
             # - In Rich:
             #   - Before every newline, emit " \" to force a line break, except
             #     for these exceptions to handle blockquotes:
             #     - Don't do this for a line preceding a blockquote
@@ -131,18 +151,48 @@
             obs_args = query_response.obs_args()
             life_list = client.observations.life_list(**obs_args)
 
         if not life_list:
             return f"No life list {query_response.obs_query_description()}"
 
         formatter = LifeListFormatter(
-            life_list, per_rank, query_response, with_taxa=True, max_taxa=100
+            life_list, per_rank, query_response, with_taxa=True, per_page=20
         )
+        ctx.page_formatter = formatter
+        ctx.page = 0
         return self._format_markdown(formatter)
 
+    def next(self, ctx: Context):
+        if not ctx.page_formatter:
+            return "Type a command that has pages first"
+        ctx.page += 1
+        if ctx.page > ctx.page_formatter.last_page():
+            ctx.page = 0
+        return self._format_markdown(ctx.page_formatter, ctx.page)
+
+    def page(self, ctx: Context, page: int = 1):
+        if not ctx.page_formatter:
+            return "Type a command that has pages first"
+        last_page = ctx.page_formatter.last_page() + 1
+        if page > last_page or page < 1:
+            msg = "Specify page 1"
+            if last_page > 1:
+                msg += f" through {last_page}"
+            return msg
+        ctx.page = page - 1
+        return self._format_markdown(ctx.page_formatter, ctx.page)
+
+    def prev(self, ctx: Context):
+        if not ctx.page_formatter:
+            return "Type a command that has pages first"
+        ctx.page -= 1
+        if ctx.page < 0:
+            ctx.page = ctx.page_formatter.last_page()
+        return self._format_markdown(ctx.page_formatter, ctx.page)
+
     def taxon(self, ctx: Context, *args):
         query = self._parse(" ".join(args))
         # TODO: Handle all query clauses, not just main.terms
         # TODO: Doesn't do any ranking or filtering of results
         if not query.main or not query.main.terms:
             return "Not a taxon"
         main_query_str = " ".join(query.main.terms)
```

### Comparing `dronefly_core-0.3.6.dev5/dronefly/core/constants.py` & `dronefly_core-0.3.6.dev6/dronefly/core/constants.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev5/dronefly/core/formatters/generic.py` & `dronefly_core-0.3.6.dev6/dronefly/core/formatters/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 Anything more complicated than plain text can be rendered in Markdown,
 which is then fairly easy to render to other formats as needed.
 """
 from __future__ import annotations
 import copy
 from datetime import datetime as dt
+from math import ceil
 import re
 from typing import TYPE_CHECKING, Union
 
 if TYPE_CHECKING:
     from dronefly.core.query.query import QueryResponse
 
 import html2markdown
@@ -528,111 +529,162 @@
 
 
 class BaseFormatter:
     def format():
         raise NotImplementedError
 
 
+class ListFormatter(BaseFormatter):
+    def format_page():
+        raise NotImplementedError
+
+    def last_page():
+        raise NotImplementedError
+
+
 class BaseCountFormatter(BaseFormatter):
     def count():
         raise NotImplementedError
 
     def description():
         raise NotImplementedError
 
 
-class LifeListFormatter(BaseFormatter):
+class LifeListFormatter(ListFormatter):
     def __init__(
         self,
         life_list: LifeList,
         per_rank: str,
         query_response: QueryResponse,
         with_url: bool = True,
         with_taxa: bool = False,
-        max_len: int = 0,
-        max_taxa: int = 20,
+        per_page: int = 20,
     ):
         """
         Parameters
         ----------
-        taxon: Taxon
-            The taxon to format.
+        life_list: LifeList
+            Life list of all taxa matching the observations query in
+            query_response.
+
+        per_rank: str
+            Rank to include in list of taxa, or one of the special values:
+                - 'leaf' (default) = leaf taxa
+                - 'main' = any of the most commonly used ranks
+                - 'any' = every rank in the life list
+
+        query_response: QueryResponse
+            The query response contains all iNat objects in the query
+            except for the life_list itself (e.g. user, place, etc.)
 
         with_url: bool, optional
-            When True, link the name to taxon.url.
+            When True, link the title to the life list, provided the query
+            was for a single user.
+
+        with_taxa: bool, optional
+            When True, format() and format_page() format the specified
+            page of taxa on the life_list as a per_page sized page.
+
+            The first page links to the observations in the query
+            and the last page ends with a total per rank in the query.
+
+            When False, only page 0 can be formatted with the observations link
+            and per rank summary alone.
+
+        per_page: int, optional
+            The number of taxa to include in each page.
         """
         self.life_list = life_list
         self.per_rank = per_rank
         self.query_response = query_response
         self.with_url = with_url
         self.with_taxa = with_taxa
-        self.max_len = max_len
-        self.max_taxa = max_taxa
+        self.per_page = per_page
+        (taxa, self.ranks, self.rank_totals) = filter_life_list(
+            self.life_list, self.per_rank, self.query_response.taxon
+        )
+        self.taxa = list(taxa)
+        self.max_digits = len(
+            str(max([taxon.descendant_obs_count for taxon in self.taxa]))
+        )
 
-    def format(self, with_title: bool = True):
+    def format(self, with_title: bool = True, page: int = 0):
         """Format the life list as markdown."""
-        description = self.format_description()
+        description = self.format_page(page)
         if with_title:
             description = "\n\n".join([self.format_title(), description])
         return description
 
     def format_title(self):
         """Format life list title as Discord-like markdown.
 
         Returns
         -------
         str
             - Describe the life list in terms of the observations query
               parameters passed.
-            - Only link to the life list when the query is for one user.
-              The website doesn't support life lists for any other kind of
-              query.
+            - When with_url is True, only link to the life list when the query
+              is for one user. The website doesn't support life lists for any
+              other kind of query.
         """
         title = f"Life list {self.query_response.obs_query_description()}"
         if self.with_url:
             if self.query_response.user:
                 url = lifelists_url_from_query_response(self.query_response)
                 title = format_link(title, url)
         return title
 
-    def format_description(self):
+    def format_page(self, page: int = 0):
         """Format the life list description."""
         description = []
-        (taxa, ranks, rank_totals) = filter_life_list(
-            self.life_list, self.per_rank, self.query_response.taxon
-        )
         query_response = self.query_response
-        obs_link = format_link(
-            "All Life List Observations",
-            obs_url_from_v1(query_response.obs_args()),
-        )
-        description.append(obs_link)
+        if page == 0:
+            obs_link = format_link(
+                "All Life List Observations",
+                obs_url_from_v1(query_response.obs_args()),
+            )
+            description.append(obs_link)
         # TODO: if more than max_taxa, support paged result
-        if self.with_taxa and len(taxa) <= self.max_taxa:
-            max_digits = len(str(max([taxon.descendant_obs_count for taxon in taxa])))
+        if self.taxa and self.with_taxa:
+            page_start = page * self.per_page
+            page_end = page_start + self.per_page
+            page_of_taxa = self.taxa[page_start:page_end]
             formatted_taxa = []
             obs_args = query_response.obs_args()
-            for taxon in taxa:
+            for taxon in page_of_taxa:
                 # Replace any taxa in the original query with just the one:
                 if "taxon_ids" in obs_args:
                     del obs_args["taxon_ids"]
                 taxon_obs_url = obs_url_from_v1(
                     {
                         **obs_args,
                         "taxon_id": taxon.id,
                     }
                 )
-                formatted_count = str(taxon.descendant_obs_count).rjust(max_digits)
+                formatted_count = str(taxon.descendant_obs_count).rjust(self.max_digits)
                 formatted_name = format_link(taxon.name, taxon_obs_url)
                 formatted_taxa.append(f"`{formatted_count}` {formatted_name}")
             description.append("\n".join(formatted_taxa))
-        life_list_summary = format_life_list_summary(taxa, ranks, rank_totals)
-        description.append(life_list_summary)
+        if page == self.last_page():
+            life_list_summary = format_life_list_summary(
+                self.taxa, self.ranks, self.rank_totals
+            )
+            description.append(life_list_summary)
         return "\n\n".join(description)
 
+    def format_all(self):
+        return [self.format_page(page) for page in range(0, self.last_page() + 1)]
+
+    def last_page(self):
+        return (
+            ceil(len(self.taxa) / self.per_page) - 1
+            if self.with_taxa and self.taxa
+            else 0
+        )
+
 
 class TaxonFormatter(BaseFormatter):
     def __init__(
         self,
         taxon: Taxon,
         lang: str = None,
         with_url: bool = True,
```

### Comparing `dronefly_core-0.3.6.dev5/dronefly/core/models/controlled_terms.py` & `dronefly_core-0.3.6.dev6/dronefly/core/models/controlled_terms.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev5/dronefly/core/parsers/constants.py` & `dronefly_core-0.3.6.dev6/dronefly/core/parsers/constants.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev5/dronefly/core/parsers/natural.py` & `dronefly_core-0.3.6.dev6/dronefly/core/parsers/natural.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev5/dronefly/core/parsers/unixlike.py` & `dronefly_core-0.3.6.dev6/dronefly/core/parsers/unixlike.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev5/dronefly/core/parsers/url.py` & `dronefly_core-0.3.6.dev6/dronefly/core/parsers/url.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev5/dronefly/core/query/query.py` & `dronefly_core-0.3.6.dev6/dronefly/core/query/query.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev5/dronefly/core/utils/__init__.py` & `dronefly_core-0.3.6.dev6/dronefly/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev5/pyproject.toml` & `dronefly_core-0.3.6.dev6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 exclude_dirs = ["tests"]
 
 [tool.flake8]
 max-line-length = 100
 
 [tool.poetry]
 name = "dronefly-core"
-version = "0.3.6.dev5"
+version = "0.3.6.dev6"
 description = "Core dronefly components"
 authors = ["Ben Armstrong <synrg@debian.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 packages = [
 	{ include = "dronefly/core" },
 ]
```

### Comparing `dronefly_core-0.3.6.dev5/setup.py` & `dronefly_core-0.3.6.dev6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'html2markdown>=0.1.7,<0.2.0',
  'inflect>=5.3.0,<6.0.0',
  'pyinaturalist>=0.19.0.dev2,<0.20',
  'rich>=10.9,<14']
 
 setup_kwargs = {
     'name': 'dronefly-core',
-    'version': '0.3.6.dev5',
+    'version': '0.3.6.dev6',
     'description': 'Core dronefly components',
     'long_description': "# Dronefly core\n\nThis is an incomplete rewrite of [Dronefly](https://dronefly.readthedocs.io)\nDiscord bot's core components. We're not yet making version guarantees until\nit is more usable.\n\n# Related packages\n\n## Dronefly command-line client\n\nThe [dronefly-cli](https://github.com/dronefly-garden/dronefly-cli) command-line\nclient will provide a standalone text user interface that can perform a usable\nsubset of Dronefly Discord bot's capabilities, built solely with Dronefly core.\n\n## Dronefly Discord bot\n\nDronefly Discord bot brings [iNaturalist](https://www.inaturalist.org) taxa,\nobservations, and other data from the site into conversations on the\n[Discord](https://discord.com) chat platform.\n",
     'author': 'Ben Armstrong',
     'author_email': 'synrg@debian.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dronefly_core-0.3.6.dev5/PKG-INFO` & `dronefly_core-0.3.6.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dronefly-core
-Version: 0.3.6.dev5
+Version: 0.3.6.dev6
 Summary: Core dronefly components
 License: AGPL-3.0-or-later
 Author: Ben Armstrong
 Author-email: synrg@debian.org
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

