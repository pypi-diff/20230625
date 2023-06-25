# Comparing `tmp/cozo_client-0.1.2.tar.gz` & `tmp/cozo_client-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cozo_client-0.1.2.tar", last modified: Thu Jun  8 17:46:32 2023, max compression
+gzip compressed data, was "cozo_client-0.1.4.tar", last modified: Sun Jun 25 11:49:49 2023, max compression
```

## Comparing `cozo_client-0.1.2.tar` & `cozo_client-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-06-08 17:46:32.233044 cozo_client-0.1.2/
--rw-r--r--   0 zh217      (501) staff       (20)     3098 2023-05-30 06:46:54.000000 cozo_client-0.1.2/.gitignore
--rw-r--r--   0 zh217      (501) staff       (20)      304 2023-06-08 17:46:32.232909 cozo_client-0.1.2/PKG-INFO
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-06-08 17:46:32.231938 cozo_client-0.1.2/cozo_client/
--rw-r--r--   0 zh217      (501) staff       (20)      464 2023-05-30 06:34:19.000000 cozo_client-0.1.2/cozo_client/__init__.py
--rw-r--r--   0 zh217      (501) staff       (20)     7424 2023-05-30 06:27:28.000000 cozo_client-0.1.2/cozo_client/_builder.py
--rw-r--r--   0 zh217      (501) staff       (20)    22686 2023-06-08 14:39:52.000000 cozo_client-0.1.2/cozo_client/_client.py
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-06-08 17:46:32.232748 cozo_client-0.1.2/cozo_client.egg-info/
--rw-r--r--   0 zh217      (501) staff       (20)      304 2023-06-08 17:46:32.000000 cozo_client-0.1.2/cozo_client.egg-info/PKG-INFO
--rw-r--r--   0 zh217      (501) staff       (20)      296 2023-06-08 17:46:32.000000 cozo_client-0.1.2/cozo_client.egg-info/SOURCES.txt
--rw-r--r--   0 zh217      (501) staff       (20)        1 2023-06-08 17:46:32.000000 cozo_client-0.1.2/cozo_client.egg-info/dependency_links.txt
--rw-r--r--   0 zh217      (501) staff       (20)       41 2023-06-08 17:46:32.000000 cozo_client-0.1.2/cozo_client.egg-info/requires.txt
--rw-r--r--   0 zh217      (501) staff       (20)       12 2023-06-08 17:46:32.000000 cozo_client-0.1.2/cozo_client.egg-info/top_level.txt
--rw-r--r--   0 zh217      (501) staff       (20)      535 2023-06-08 17:45:52.000000 cozo_client-0.1.2/pyproject.toml
--rw-r--r--   0 zh217      (501) staff       (20)       40 2023-05-31 08:07:55.000000 cozo_client-0.1.2/requirements.txt
--rw-r--r--   0 zh217      (501) staff       (20)       38 2023-06-08 17:46:32.233086 cozo_client-0.1.2/setup.cfg
--rw-r--r--   0 zh217      (501) staff       (20)       38 2023-05-20 12:04:30.000000 cozo_client-0.1.2/setup.py
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-06-25 11:49:49.871245 cozo_client-0.1.4/
+-rw-r--r--   0 zh217      (501) staff       (20)     3106 2023-06-19 09:16:44.000000 cozo_client-0.1.4/.gitignore
+-rw-r--r--   0 zh217      (501) staff       (20)      304 2023-06-25 11:49:49.871045 cozo_client-0.1.4/PKG-INFO
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-06-25 11:49:49.870120 cozo_client-0.1.4/cozo_client/
+-rw-r--r--   0 zh217      (501) staff       (20)      464 2023-05-30 06:34:19.000000 cozo_client-0.1.4/cozo_client/__init__.py
+-rw-r--r--   0 zh217      (501) staff       (20)     7424 2023-05-30 06:27:28.000000 cozo_client-0.1.4/cozo_client/_builder.py
+-rw-r--r--   0 zh217      (501) staff       (20)    29722 2023-06-25 10:45:58.000000 cozo_client-0.1.4/cozo_client/_client.py
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-06-25 11:49:49.870804 cozo_client-0.1.4/cozo_client.egg-info/
+-rw-r--r--   0 zh217      (501) staff       (20)      304 2023-06-25 11:49:49.000000 cozo_client-0.1.4/cozo_client.egg-info/PKG-INFO
+-rw-r--r--   0 zh217      (501) staff       (20)      296 2023-06-25 11:49:49.000000 cozo_client-0.1.4/cozo_client.egg-info/SOURCES.txt
+-rw-r--r--   0 zh217      (501) staff       (20)        1 2023-06-25 11:49:49.000000 cozo_client-0.1.4/cozo_client.egg-info/dependency_links.txt
+-rw-r--r--   0 zh217      (501) staff       (20)       38 2023-06-25 11:49:49.000000 cozo_client-0.1.4/cozo_client.egg-info/requires.txt
+-rw-r--r--   0 zh217      (501) staff       (20)       12 2023-06-25 11:49:49.000000 cozo_client-0.1.4/cozo_client.egg-info/top_level.txt
+-rw-r--r--   0 zh217      (501) staff       (20)      532 2023-06-25 10:48:08.000000 cozo_client-0.1.4/pyproject.toml
+-rw-r--r--   0 zh217      (501) staff       (20)       37 2023-06-13 21:28:10.000000 cozo_client-0.1.4/requirements.txt
+-rw-r--r--   0 zh217      (501) staff       (20)       38 2023-06-25 11:49:49.871301 cozo_client-0.1.4/setup.cfg
+-rw-r--r--   0 zh217      (501) staff       (20)       38 2023-05-20 12:04:30.000000 cozo_client-0.1.4/setup.py
```

### Comparing `cozo_client-0.1.2/.gitignore` & `cozo_client-0.1.4/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -156,7 +156,8 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/
 
+/*.ipynb
```

### Comparing `cozo_client-0.1.2/cozo_client/_builder.py` & `cozo_client-0.1.4/cozo_client/_builder.py`

 * *Files identical despite different names*

### Comparing `cozo_client-0.1.2/cozo_client/_client.py` & `cozo_client-0.1.4/cozo_client/_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 from enum import Enum
 import logging
 import html
 import json
 from typing import Any, Generator, Union, Callable
 
-import requests
+import httpx
 import cozo_embedded
 from pydantic import BaseModel
 
 from ._builder import InputProgram, ConstantRule, RuleHead, InlineRule, Param, RuleApply, StoredRuleNamedApply, \
     StoreOp, InputRelation
 
 logger = logging.getLogger(__name__)
@@ -33,14 +33,26 @@
     remote = 'remote'
 
 
 class CozoResponse(BaseModel):
     headers: list[str]
     rows: list[list[Any]]
     max_display_rows: int = 50
+    next: Any
+
+    def multi(self) -> list:
+        cur = self.next
+        self.next = None
+        resp = [self]
+        while cur:
+            nxt = CozoResponse(**cur)
+            cur = cur.get('next')
+            nxt.next = None
+            resp.append(nxt)
+        return resp
 
     def _repr_html_(self):
         html_str = ["<table>", "<thead>", "<tr>", "<th></th>"]
 
         for header in self.headers:
             html_str.append(f"<th style='font-size: 80%; text-align: center;'>{html.escape(header)}</th>")
 
@@ -261,14 +273,34 @@
         bold_font = Font(bold=True)
         for cell in ws["1:1"]:
             cell.font = bold_font
 
         wb.save(filename)
 
 
+def _get_ident(d):
+    match d:
+        case str(d):
+            return d
+        case tuple(d):
+            return d[0]
+        case _:
+            raise ValueError(f'Invalid column definition: {d}')
+
+
+def _get_type(d):
+    match d:
+        case str(_):
+            return 'Any?'
+        case tuple(d):
+            return d[1]
+        case _:
+            raise ValueError(f'Invalid column definition: {d}')
+
+
 class CozoRow(BaseModel):
     headers: list[str]
     row: list[Any]
 
     def _repr_html_(self):
         html_str = ["<table>", "<tbody>"]
         for i, header in enumerate(self.headers):
@@ -338,19 +370,22 @@
         if engine == StorageEngine.remote:
             if remote_host.endswith('/'):
                 remote_host = remote_host[:len(remote_host) - 1]
             self.host = remote_host
             self.embedded = None
             self._remote_sse = {}
             self._remote_cb_id = 0
-            self._session = requests.Session()
+            self._session = httpx.Client(timeout=600)
+            self._asession = httpx.AsyncClient(timeout=600)
             if remote_token:
                 self._session.headers.update({'Authorization': f'Bearer {remote_token}'})
+                self._asession.headers.update({'Authorization': f'Bearer {remote_token}'})
             elif remote_auth:
                 self._session.headers.update({'x-cozo-auth': remote_auth})
+                self._asession.headers.update({'x-cozo-auth': remote_auth})
         else:
             self.embedded = cozo_embedded.CozoDbPy(engine, path or '', '{}')
 
     def ensure_index(self, name: str, idx_name: str, cols: list[str]):
         try:
             existing_cols = self.run(f'::columns {name}:{idx_name}')
             for i, row in enumerate(existing_cols):
@@ -359,55 +394,75 @@
         except QueryException as e:
             if e.code == 'query::relation_not_found':
                 prog = f'''::index create {name}:{idx_name} {{ {', '.join(cols)} }}'''
                 self.run(prog)
             else:
                 raise
 
+    async def a_ensure_index(self, name: str, idx_name: str, cols: list[str]):
+        try:
+            existing_cols = await self.a_run(f'::columns {name}:{idx_name}')
+            for i, row in enumerate(existing_cols):
+                assert row['column'] == cols[i], f'Column {i} is {row["column"]} not {cols[i]}'
+
+        except QueryException as e:
+            if e.code == 'query::relation_not_found':
+                prog = f'''::index create {name}:{idx_name} {{ {', '.join(cols)} }}'''
+                await self.a_run(prog)
+            else:
+                raise
+
     def ensure_relation(self,
                         name: str,
                         keys: list[str | tuple[str, str] | tuple[str, str, str]],
                         vals: list[str | tuple[str, str] | tuple[str, str, str]]):
-        def get_ident(d):
-            match d:
-                case str(d):
-                    return d
-                case tuple(d):
-                    return d[0]
-                case _:
-                    raise ValueError(f'Invalid column definition: {d}')
-
-        def get_type(d):
-            match d:
-                case str(_):
-                    return 'Any?'
-                case tuple(d):
-                    return d[1]
-                case _:
-                    raise ValueError(f'Invalid column definition: {d}')
-
         try:
             existing_cols = self.run(f'::columns {name}')
             assert len([row for row in existing_cols if row['is_key']]) == len(keys)
             assert len([row for row in existing_cols if not row['is_key']]) == len(vals)
             for i, col in enumerate(keys):
-                assert get_ident(col) == existing_cols[i]['column']
-                assert get_type(col) == existing_cols[i]['type']
+                assert _get_ident(col) == existing_cols[i]['column']
+                assert _get_type(col) == existing_cols[i]['type']
             col_map = {row['column']: row for row in existing_cols if not row['is_key']}
             for col in vals:
-                assert get_ident(col) in col_map
-                assert get_type(col) == col_map[get_ident(col)]['type']
+                assert _get_ident(col) in col_map, f'Column {col} not found'
+                assert _get_type(col).replace(' ', '') == col_map[_get_ident(col)]['type'].replace(' ', ''), \
+                    f'Column {col} has type {col_map[_get_ident(col)]["type"]} not {_get_type(col)}'
         except QueryException as e:
             if e.code == 'query::relation_not_found':
                 prog = InputProgram(
                     store_relation=(StoreOp.CREATE, InputRelation(name=name, keys=keys, values=vals)))
                 self.run(prog)
             else:
                 raise
 
+    async def a_ensure_relation(self,
+                                name: str,
+                                keys: list[str | tuple[str, str] | tuple[str, str, str]],
+                                vals: list[str | tuple[str, str] | tuple[str, str, str]]):
+        try:
+            existing_cols = await self.a_run(f'::columns {name}')
+            assert len([row for row in existing_cols if row['is_key']]) == len(keys)
+            assert len([row for row in existing_cols if not row['is_key']]) == len(vals)
+            for i, col in enumerate(keys):
+                assert _get_ident(col) == existing_cols[i]['column']
+                assert _get_type(col) == existing_cols[i]['type']
+            col_map = {row['column']: row for row in existing_cols if not row['is_key']}
+            for col in vals:
+                assert _get_ident(col) in col_map, f'Column {col} not found'
+                assert _get_type(col).replace(' ', '') == col_map[_get_ident(col)]['type'].replace(' ', ''), \
+                    f'Column {col} has type {col_map[_get_ident(col)]["type"]} not {_get_type(col)}'
+        except QueryException as e:
+            if e.code == 'query::relation_not_found':
+                prog = InputProgram(
+                    store_relation=(StoreOp.CREATE, InputRelation(name=name, keys=keys, values=vals)))
+                await self.a_run(prog)
+            else:
+                raise
+
     def ensure_lsh(self,
                    rel_name: str,
                    idx_name: str,
                    extractor: str,
                    filter: str | None,
                    n_perm: int = 200,
                    n_gram: int = 7,
@@ -424,14 +479,38 @@
                     target_threshold: {target_threshold},
                     n_gram: {n_gram},
                 }}'''
                 self.run(query)
             else:
                 raise
 
+    async def a_ensure_lsh(self,
+                           rel_name: str,
+                           idx_name: str,
+                           extractor: str,
+                           filter: str | None,
+                           n_perm: int = 200,
+                           n_gram: int = 7,
+                           target_threshold: float = 0.5):
+        try:
+            await self.a_run(f'''::columns {rel_name}:{idx_name}''')
+        except QueryException as e:
+            if e.code == 'query::relation_not_found':
+                query = f'''::lsh create {rel_name}:{idx_name} {{
+                    extractor: {extractor},
+                    {'filter: ' + filter + ',' if filter else ''}
+                    tokenizer: NGram,
+                    n_perm: {n_perm},
+                    target_threshold: {target_threshold},
+                    n_gram: {n_gram},
+                }}'''
+                await self.a_run(query)
+            else:
+                raise
+
     def ensure_vec_index(self, rel_name: str, idx_name: str, dim: int, m: int, ef: int):
         try:
             self.run(f'::columns {rel_name}:{idx_name}')
         except QueryException as e:
             if e.code == 'query::relation_not_found':
                 self.run(f'''::hnsw create {rel_name}:{idx_name} {{
                     dim: $dim,
@@ -440,14 +519,30 @@
                     fields: vec,
                     distance: Cosine,
                     ef: $ef,
                 }}''', {'dim': dim, 'm': m, 'ef': ef})
             else:
                 raise
 
+    async def a_ensure_vec_index(self, rel_name: str, idx_name: str, dim: int, m: int, ef: int):
+        try:
+            await self.a_run(f'::columns {rel_name}:{idx_name}')
+        except QueryException as e:
+            if e.code == 'query::relation_not_found':
+                await self.a_run(f'''::hnsw create {rel_name}:{idx_name} {{
+                    dim: $dim,
+                    m: $m,
+                    dtype: F32,
+                    fields: vec,
+                    distance: Cosine,
+                    ef: $ef,
+                }}''', {'dim': dim, 'm': m, 'ef': ef})
+            else:
+                raise
+
     def __eq__(self, other):
         if isinstance(other, CozoClient):
             if self.is_remote and other.is_remote:
                 return self.host == other.host
             elif not self.is_remote and not other.is_remote:
                 return self.embedded == other.embedded
         return False
@@ -463,23 +558,31 @@
         return self.embedded is None
 
     def close(self):
         if self.embedded:
             self.embedded.close()
 
     def _client_request(self, script, params=None, immutable=False):
-
         r = self._session.post(f'{self.host}/text-query', json={
             'script': script,
             'params': params or {},
             'immutable': immutable
         })
         res = r.json()
         return self._format_return(res)
 
+    async def _async_client_request(self, script, params=None, immutable=False):
+        r = await self._asession.post(f'{self.host}/text-query', json={
+            'script': script,
+            'params': params or {},
+            'immutable': immutable
+        })
+        res = r.json()
+        return self._format_return(res)
+
     @staticmethod
     def _format_return(res):
         if not res['ok']:
             raise QueryException(res)
 
         return CozoResponse(**res)
 
@@ -495,45 +598,58 @@
             params: dict[str, Any] | None = None,
             replace: dict[str, str] | None = None,
             immutable=False
             ) -> CozoResponse:
         script = str(script)
         if replace:
             for k, v in replace.items():
-                r = r'\$\$' + k + r'\$\$'
+                r = r'<<' + k + r'>>'
                 script = re.sub(r, v, script)
         if self.is_remote:
             return self._client_request(script, params, immutable)
         else:
             return self._embedded_request(script, params, immutable)
 
+    async def a_run(self,
+                    script: str | InputProgram,
+                    params: dict[str, Any] | None = None,
+                    replace: dict[str, str] | None = None,
+                    immutable=False
+                    ) -> CozoResponse:
+        assert self.is_remote
+        script = str(script)
+        if replace:
+            for k, v in replace.items():
+                r = r'<<' + k + r'>>'
+                script = re.sub(r, v, script)
+        return await self._async_client_request(script, params, immutable)
+
     def export_relations(self, relations) -> dict[str, CozoResponse]:
         if not self.is_remote:
             return {k: CozoResponse(**v) for k, v in self.embedded.export_relations(relations).items()}
         else:
             import urllib.parse
 
             rels = ','.join(map(lambda s: urllib.parse.quote_plus(s), relations))
             url = f'{self.host}/export/{rels}'
 
-            r = requests.get(url)
+            r = self._session.get(url)
             res = r.json()
             if res['ok']:
                 return {k: CozoResponse(**v) for k, v in res['data'].items()}
             else:
                 raise RuntimeError(res['message'])
 
     def import_relations(self, data):
         if self.embedded:
             self.embedded.import_relations(data)
         else:
-            import requests
             url = f'{self.host}/import'
 
-            r = requests.put(url, json=data)
+            r = self._session.put(url, json=data)
             res = r.json()
             if not res['ok']:
                 raise RuntimeError(res['message'])
 
     def backup(self, path):
         if self.embedded:
             self.embedded.backup(path)
@@ -581,29 +697,52 @@
         cols, processed_data = self._process_mutate_data(data)
         cols_str = ', '.join(cols)
         q = f'?[{cols_str}] <- $data :{op} {relation} {{ {cols_str} }}'
         if returning:
             q += ' :returning'
         return self.run(q, {'data': processed_data})
 
+    async def _a_mutate(self, relation, data, op, returning):
+        cols, processed_data = self._process_mutate_data(data)
+        cols_str = ', '.join(cols)
+        q = f'?[{cols_str}] <- $data :{op} {relation} {{ {cols_str} }}'
+        if returning:
+            q += ' :returning'
+        return await self.a_run(q, {'data': processed_data})
+
     def insert(self, relation: str, data: dict[str, Any] | list[dict[str, Any]], returning: bool = False):
         return self._mutate(relation, data, 'insert', returning)
 
+    async def a_insert(self, relation: str, data: dict[str, Any] | list[dict[str, Any]], returning: bool = False):
+        return await self._a_mutate(relation, data, 'insert', returning)
+
     def put(self, relation: str, data: dict[str, Any] | list[dict[str, Any]], returning: bool = False):
         return self._mutate(relation, data, 'put', returning)
 
+    async def a_put(self, relation: str, data: dict[str, Any] | list[dict[str, Any]], returning: bool = False):
+        return await self._a_mutate(relation, data, 'put', returning)
+
     def update(self, relation: str, data: dict[str, Any] | list[dict[str, Any]], returning: bool = False):
         return self._mutate(relation, data, 'update', returning)
 
+    async def a_update(self, relation: str, data: dict[str, Any] | list[dict[str, Any]], returning: bool = False):
+        return await self._a_mutate(relation, data, 'update', returning)
+
     def rm(self, relation: str, data: dict[str, Any] | list[dict[str, Any]], returning: bool = False):
         return self._mutate(relation, data, 'rm', returning)
 
+    async def a_rm(self, relation: str, data: dict[str, Any] | list[dict[str, Any]], returning: bool = False):
+        return await self._a_mutate(relation, data, 'rm', returning)
+
     def delete(self, relation: str, data: dict[str, Any] | list[dict[str, Any]], returning: bool = False):
         return self._mutate(relation, data, 'delete', returning)
 
+    async def a_delete(self, relation: str, data: dict[str, Any] | list[dict[str, Any]], returning: bool = False):
+        return await self._a_mutate(relation, data, 'delete', returning)
+
     def get(self, relation: str, data: dict[str, Any] | list[dict[str, Any]], out: list[str] | None = None):
         if out is None:
             out = [row['column'] for row in self.run(f'::columns {relation}')]
 
         cols, processed_data = self._process_mutate_data(data)
         prog = InputProgram(
             rules=[
@@ -611,14 +750,29 @@
                 InlineRule(head=RuleHead(name='?', args=out),
                            atoms=[RuleApply(name='data', args=cols),
                                   StoredRuleNamedApply(name=relation, args={k: k for k in out})]),
             ],
         )
         return self.run(prog, {'data': processed_data})
 
+    async def a_get(self, relation: str, data: dict[str, Any] | list[dict[str, Any]], out: list[str] | None = None):
+        if out is None:
+            out = [row['column'] for row in await self.a_run(f'::columns {relation}')]
+
+        cols, processed_data = self._process_mutate_data(data)
+        prog = InputProgram(
+            rules=[
+                ConstantRule(head=RuleHead(name='data', args=cols), body=Param(name='data')),
+                InlineRule(head=RuleHead(name='?', args=out),
+                           atoms=[RuleApply(name='data', args=cols),
+                                  StoredRuleNamedApply(name=relation, args={k: k for k in out})]),
+            ],
+        )
+        return await self.a_run(prog, {'data': processed_data})
+
 
 class QueryException(Exception):
     def __init__(self, resp):
         super().__init__()
         self.resp = resp
 
     def __str__(self):
```

### Comparing `cozo_client-0.1.2/pyproject.toml` & `cozo_client-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 keywords = ["client"]
 license = { text = "MIT" }
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "cozo-embedded",
-    "requests",
+    "httpx",
     "pydantic",
     "openpyxl"
 ]
-version = "0.1.2"
+version = "0.1.4"
```

