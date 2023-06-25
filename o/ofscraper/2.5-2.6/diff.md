# Comparing `tmp/ofscraper-2.5.tar.gz` & `tmp/ofscraper-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-2.5.tar", max compression
+gzip compressed data, was "ofscraper-2.6.tar", max compression
```

## Comparing `ofscraper-2.5.tar` & `ofscraper-2.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1067 2023-06-22 06:44:41.511715 ofscraper-2.5/LICENSE
--rw-r--r--   0        0        0     6001 2023-06-22 06:44:41.511715 ofscraper-2.5/README.md
--rw-r--r--   0        0        0      607 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/__init__.py
--rw-r--r--   0        0        0      999 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/__version__.py
--rw-r--r--   0        0        0        1 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     7709 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/archive.py
--rw-r--r--   0        0        0     4682 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1067 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/init.py
--rw-r--r--   0        0        0     2338 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/me.py
--rw-r--r--   0        0        0     8507 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/messages.py
--rw-r--r--   0        0        0     9163 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/paid.py
--rw-r--r--   0        0        0     5159 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/pinned.py
--rw-r--r--   0        0        0    11529 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/posts.py
--rw-r--r--   0        0        0     3593 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/profile.py
--rw-r--r--   0        0        0     3047 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     8254 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/api/timeline.py
--rw-r--r--   0        0        0    14116 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/commands/check.py
--rw-r--r--   0        0        0     5025 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/commands/manual.py
--rwxr-xr-x   0        0        0    13993 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0     6293 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/db/__init__.py
--rw-r--r--   0        0        0     8581 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3253 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     4768 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/interaction/like.py
--rw-r--r--   0        0        0      696 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0     6754 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0    27282 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0      744 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/start.py
--rw-r--r--   0        0        0        1 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0    10460 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/utils/args.py
--rw-r--r--   0        0        0     8893 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/utils/auth.py
--rw-r--r--   0        0        0     9023 2023-06-22 06:44:41.519716 ofscraper-2.5/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0    10680 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/config.py
--rw-r--r--   0        0        0      257 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/console.py
--rw-r--r--   0        0        0      993 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    20329 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2865 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     3022 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/filters.py
--rw-r--r--   0        0        0     6442 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/logger.py
--rw-r--r--   0        0        0     9870 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/of.py
--rw-r--r--   0        0        0     7934 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     3073 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      399 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/semaphoreDelayed.py
--rw-r--r--   0        0        0     1358 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/separate.py
--rw-r--r--   0        0        0      554 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/stdout.py
--rw-r--r--   0        0        0    28869 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/table.py
--rw-r--r--   0        0        0     6089 2023-06-22 06:44:41.523716 ofscraper-2.5/ofscraper/utils/userselector.py
--rw-r--r--   0        0        0     1624 2023-06-22 06:45:18.414684 ofscraper-2.5/pyproject.toml
--rw-r--r--   0        0        0     7503 1970-01-01 00:00:00.000000 ofscraper-2.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-25 19:47:48.618819 ofscraper-2.6/LICENSE
+-rw-r--r--   0        0        0     2862 2023-06-25 19:47:48.618819 ofscraper-2.6/README.md
+-rw-r--r--   0        0        0      607 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/__init__.py
+-rw-r--r--   0        0        0      999 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/__version__.py
+-rw-r--r--   0        0        0        1 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     8188 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/archive.py
+-rw-r--r--   0        0        0     4852 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1067 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/init.py
+-rw-r--r--   0        0        0     2859 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/me.py
+-rw-r--r--   0        0        0     9021 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     9689 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     5550 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0    11505 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/posts.py
+-rw-r--r--   0        0        0     3909 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     3047 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     8725 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0    14097 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/commands/check.py
+-rw-r--r--   0        0        0     4884 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/commands/manual.py
+-rwxr-xr-x   0        0        0    13452 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0     6312 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0     8581 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3253 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     4973 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0      696 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0     7683 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0    27766 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0     1139 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/start.py
+-rw-r--r--   0        0        0        1 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0    11211 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/args.py
+-rw-r--r--   0        0        0     8950 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0     8977 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0    10803 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      257 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      993 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    19529 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2865 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     3376 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0     6442 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0     9615 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/of.py
+-rw-r--r--   0        0        0    11732 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     4263 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      399 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/semaphoreDelayed.py
+-rw-r--r--   0        0        0     1358 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0      554 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/stdout.py
+-rw-r--r--   0        0        0    29248 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/table.py
+-rw-r--r--   0        0        0     6089 2023-06-25 19:47:48.626819 ofscraper-2.6/ofscraper/utils/userselector.py
+-rw-r--r--   0        0        0     1694 2023-06-25 19:48:22.475505 ofscraper-2.6/pyproject.toml
+-rw-r--r--   0        0        0     4364 1970-01-01 00:00:00.000000 ofscraper-2.6/PKG-INFO
```

### Comparing `ofscraper-2.5/LICENSE` & `ofscraper-2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-2.5/ofscraper/__init__.py` & `ofscraper-2.6/ofscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.5/ofscraper/__version__.py` & `ofscraper-2.6/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.5/ofscraper/api/archive.py` & `ofscraper-2.6/ofscraper/api/archive.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 import time
 import asyncio
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 import logging
 import contextvars
 import math
-import httpx
+import aiohttp
 from tenacity import retry,stop_after_attempt,wait_random
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
 )
@@ -35,15 +35,15 @@
 from diskcache import Cache
 cache = Cache(getcachepath())
 log=logging.getLogger(__package__)
 attempt = contextvars.ContextVar("attempt")
 
 sem = semaphoreDelayed(constants.AlT_SEM)
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
-async def scrape_archived_posts(headers, model_id,progress, timestamp=None,required_ids=None) -> list:
+async def scrape_archived_posts(c, model_id,progress, timestamp=None,required_ids=None) -> list:
     global tasks
     global sem
     posts=None
     attempt.set(attempt.get(0) + 1)
     if timestamp and   (float(timestamp)>(args_.getargs().before or arrow.now()).float_timestamp):
         return []
     if timestamp:
@@ -53,99 +53,100 @@
         url = ep.format(model_id, timestamp)
     else:
         ep=constants.archivedEP
         url=ep.format(model_id)
     log.debug(url)
     async with sem:
         task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Timestamp -> {arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}",visible=True)
-        async with httpx.AsyncClient(http2=True, headers=headers) as c:
-            auth.add_cookies(c)
-            c.headers.update(auth.create_sign(url, headers))
-            r = await c.get(url , timeout=None)
-    if not r.is_error:
-        progress.remove_task(task)
-        posts = r.json()['list']
-        log_id=f"timestamp:{arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}"
-        if not posts:
-            posts= []
-        if len(posts)==0:
-            log.debug(f" {log_id} -> number of post found 0")
-        elif len(posts)>0:
-            log.debug(f"{log_id} -> number of archived post found {len(posts)}")
-            log.debug(f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}")
-            log.debug(f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}")
-            log.debug(f"{log_id} -> first ID {posts[0]['id']}")
-            log.debug(f"{log_id} -> last ID {posts[-1]['id']}")        
-            if required_ids==None:
-                attempt.set(0)
-                tasks.append(asyncio.create_task(scrape_archived_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'])))
+        headers=auth.make_headers(auth.read_auth())
+        headers=auth.create_sign(url, headers)
+        async with c.request("get",url,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=headers) as r:       
+            if r.ok:
+                progress.remove_task(task)
+                posts =( await r.json())['list']
+                log_id=f"timestamp:{arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}"
+                if not posts:
+                    posts= []
+                if len(posts)==0:
+                    log.debug(f" {log_id} -> number of post found 0")
+                elif len(posts)>0:
+                    log.debug(f"{log_id} -> number of archived post found {len(posts)}")
+                    log.debug(f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}")
+                    log.debug(f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}")
+                    log.debug(f"{log_id} -> first ID {posts[0]['id']}")
+                    log.debug(f"{log_id} -> last ID {posts[-1]['id']}")        
+                    if required_ids==None:
+                        attempt.set(0)
+                        tasks.append(asyncio.create_task(scrape_archived_posts(c, model_id,progress,timestamp=posts[-1]['postedAtPrecise'])))
+                    else:
+                        [required_ids.discard(float(ele["postedAtPrecise"])) for ele in posts]
+
+
+                        #try once more to get id if only 1 left
+                        if len(required_ids)==1:
+                            attempt.set(0)
+                            tasks.append(asyncio.create_task(scrape_archived_posts(c, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=set())))
+
+                        elif len(required_ids)>0:
+                            attempt.set(0)
+                            tasks.append(asyncio.create_task(scrape_archived_posts(c, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=required_ids)))
             else:
-                [required_ids.discard(float(ele["postedAtPrecise"])) for ele in posts]
-
-
-                #try once more to get id if only 1 left
-                if len(required_ids)==1:
-                    attempt.set(0)
-                    tasks.append(asyncio.create_task(scrape_archived_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=set())))
-
-                elif len(required_ids)>0:
-                    attempt.set(0)
-                    tasks.append(asyncio.create_task(scrape_archived_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=required_ids)))
-    else:
-            log.debug(f"[bold]archived request status code:[/bold]{r.status_code}")
-            log.debug(f"[bold]archived response:[/bold] {r.content.decode()}")
-            log.debug(f"[bold]archived headers:[/bold] {r.headers}")
-            progress.remove_task(task)
-            r.raise_for_status()
+                    log.debug(f"[bold]archived request status code:[/bold]{r.status}")
+                    log.debug(f"[bold]archived response:[/bold] {await r.text()}")
+                    log.debug(f"[bold]archived headers:[/bold] {r.headers}")
+                    progress.remove_task(task)
+                    r.raise_for_status()
     return posts
 
-async def get_archived_post(headers,model_id): 
+async def get_archived_post(model_id): 
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting archived media...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
     global tasks
     tasks=[]
     min_posts=50
     responseArray=[]
     page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console): 
+        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=None, connect=None,
+                            sock_connect=None, sock_read=None)) as c: 
 
-        oldarchived=cache.get(f"archived_{model_id}",default=[])
-        oldtimeset=set(map(lambda x:x.get("id"),oldarchived))
-        log.debug(f"[bold]Archived Cache[/bold] {len(oldarchived)} found")
-        oldarchived=list(filter(lambda x:x.get("postedAtPrecise")!=None,oldarchived))
-        postedAtArray=sorted(list(map(lambda x:float(x["postedAtPrecise"]),oldarchived)))
-        filteredArray=list(filter(lambda x:x>=(args_.getargs().after or arrow.get(0)).float_timestamp,postedAtArray))
+            oldarchived=cache.get(f"archived_{model_id}",default=[])
+            oldtimeset=set(map(lambda x:x.get("id"),oldarchived))
+            log.debug(f"[bold]Archived Cache[/bold] {len(oldarchived)} found")
+            oldarchived=list(filter(lambda x:x.get("postedAtPrecise")!=None,oldarchived))
+            postedAtArray=sorted(list(map(lambda x:float(x["postedAtPrecise"]),oldarchived)))
+            filteredArray=list(filter(lambda x:x>=(args_.getargs().after or arrow.get(0)).float_timestamp,postedAtArray))
+            
         
-    
-       
-        if len(filteredArray)>min_posts:
-            splitArrays=[filteredArray[i:i+min_posts] for i in range(0, len(filteredArray), min_posts)]
-            #use the previous split for timesamp
-            tasks.append(asyncio.create_task(scrape_archived_posts(headers,model_id,job_progress,required_ids=set(splitArrays[0]),timestamp= splitArrays[0][0]-20000)))
-            [tasks.append(asyncio.create_task(scrape_archived_posts(headers,model_id,job_progress,required_ids=set(splitArrays[i]),timestamp=splitArrays[i-1][-1])))
-            for i in range(1,len(splitArrays)-1)]
-            # keeping grabbing until nothign left
-            tasks.append(asyncio.create_task(scrape_archived_posts(headers,model_id,job_progress,timestamp=splitArrays[-2][-1])))
-        else:
-            tasks.append(asyncio.create_task(scrape_archived_posts(headers,model_id,job_progress,timestamp=args_.getargs().after.float_timestamp if args_.getargs().after else None)))
-    
-
-        page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True)
-        while len(tasks)!=0:
-            for coro in asyncio.as_completed(tasks):
-                result=await coro or []
-                page_count=page_count+1
-                overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
-                responseArray.extend(result)
-            time.sleep(1)
-            tasks=list(filter(lambda x:x.done()==False,tasks))
-        overall_progress.remove_task(page_task)
+        
+            if len(filteredArray)>min_posts:
+                splitArrays=[filteredArray[i:i+min_posts] for i in range(0, len(filteredArray), min_posts)]
+                #use the previous split for timesamp
+                tasks.append(asyncio.create_task(scrape_archived_posts(c,model_id,job_progress,required_ids=set(splitArrays[0]),timestamp= splitArrays[0][0]-20000)))
+                [tasks.append(asyncio.create_task(scrape_archived_posts(c,model_id,job_progress,required_ids=set(splitArrays[i]),timestamp=splitArrays[i-1][-1])))
+                for i in range(1,len(splitArrays)-1)]
+                # keeping grabbing until nothign left
+                tasks.append(asyncio.create_task(scrape_archived_posts(c,model_id,job_progress,timestamp=splitArrays[-2][-1])))
+            else:
+                tasks.append(asyncio.create_task(scrape_archived_posts(c,model_id,job_progress,timestamp=args_.getargs().after.float_timestamp if args_.getargs().after else None)))
+        
+
+            page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True)
+            while len(tasks)!=0:
+                for coro in asyncio.as_completed(tasks):
+                    result=await coro or []
+                    page_count=page_count+1
+                    overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
+                    responseArray.extend(result)
+                time.sleep(1)
+                tasks=list(filter(lambda x:x.done()==False,tasks))
+            overall_progress.remove_task(page_task)
     unduped=[]
     dupeSet=set()
     log.debug(f"[bold]Archived Count with Dupes[/bold] {len(responseArray)} found")
     for post in responseArray:
         if post["id"] in dupeSet:
             continue
         dupeSet.add(post["id"])
```

### Comparing `ofscraper-2.5/ofscraper/api/highlights.py` & `ofscraper-2.6/ofscraper/api/highlights.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 import asyncio
 import logging
 import contextvars
-import httpx
+import aiohttp
 from tenacity import retry,stop_after_attempt,wait_random
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
 )
@@ -29,64 +29,64 @@
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 import ofscraper.utils.console as console
 
 log=logging.getLogger(__package__)
 sem = semaphoreDelayed(1)
 attempt = contextvars.ContextVar("attempt")
 
-async def get_highlight_post(headers,model_id):
+async def get_highlight_post(model_id):
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting highlight media...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
 
     output=[]
     page_count=0
     global tasks
     tasks=[]
     with Live(progress_group, refresh_per_second=5,console=console.shared_console):
-        tasks.append(asyncio.create_task(scrape_highlights(headers,model_id,job_progress)))
-        page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
-        while len(tasks)!=0:
-            for coro in asyncio.as_completed(tasks):
-                result=await coro or []
-                page_count=page_count+1
-                overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
-                output.extend(result)
-            tasks=list(filter(lambda x:x.done()==False,tasks))
-        overall_progress.remove_task(page_task)  
+        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=None, connect=None,
+                      sock_connect=None, sock_read=None)) as c: 
+            tasks.append(asyncio.create_task(scrape_highlights(c,model_id,job_progress)))
+            page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
+            while len(tasks)!=0:
+                for coro in asyncio.as_completed(tasks):
+                    result=await coro or []
+                    page_count=page_count+1
+                    overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
+                    output.extend(result)
+                tasks=list(filter(lambda x:x.done()==False,tasks))
+            overall_progress.remove_task(page_task)  
     return output
 
 
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
-async def scrape_highlights(headers, user_id,job_progress) -> list:
+async def scrape_highlights( c,user_id,job_progress) -> list:
     global sem
     global tasks
     attempt.set(attempt.get(0) + 1)
     highlights_=None; stories=None
     await sem.acquire()
     task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}",visible=True)
+    headers=auth.make_headers(auth.read_auth())
+  
 
-    async with httpx.AsyncClient(http2=True, headers=headers) as c:
-        url_stories = constants.highlightsWithStoriesEP.format(user_id)
-        url_story = constants.highlightsWithAStoryEP.format(user_id)
-        auth.add_cookies(c)
-        c.headers.update(auth.create_sign(url_stories, headers))
-        r_multiple = await c.get(url_stories, timeout=None)
-        c.headers.update(auth.create_sign(url_story, headers))
-        r_one = await c.get(url_story, timeout=None)
-      
-        # highlights_, stories
-        sem.release()
-    if not r_multiple.is_error and not r_one.is_error:
+    url_stories = constants.highlightsWithStoriesEP.format(user_id)
+    url_story = constants.highlightsWithAStoryEP.format(user_id)
+    r_one=await c.request("get",url_story ,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=auth.create_sign(url_story , headers))
+    r_multiple=await c.request("get",url_stories ,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=auth.create_sign(url_stories , headers))
+    
+    # highlights_, stories
+    sem.release()
+    if  r_multiple.ok and r_one.ok:
         attempt.set(0)
-        log.debug(f"[bold]Highlight Post Count without Dupes[/bold] {len(r_multiple.json())} found")
-        log.debug(f"[bold]Story Post Count without Dupes[/bold] {len(r_one.json())} found")
-        highlights_, stories =get_highlightList(r_multiple.json()),r_one.json()
+        log.debug(f"[bold]Highlight Post Count without Dupes[/bold] {len(await r_multiple.json())} found")
+        log.debug(f"[bold]Story Post Count without Dupes[/bold] {len(await r_one.json())} found")
+        highlights_, stories =get_highlightList(await r_multiple.json()),await r_one.json()
         job_progress.remove_task(task)
 
     else:
         job_progress.remove_task(task)
         r_multiple.raise_for_status()
         r_one.raise_for_status()
     return  highlights_, stories
```

### Comparing `ofscraper-2.5/ofscraper/api/init.py` & `ofscraper-2.6/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.5/ofscraper/api/me.py` & `ofscraper-2.6/ofscraper/api/me.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,40 +5,56 @@
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 import logging
+from functools import lru_cache
+import json
 import httpx
 from rich.console import Console
 from tenacity import retry,stop_after_attempt,wait_random
 import ofscraper.constants as constants
 import ofscraper.utils.auth as auth
 import ofscraper.utils.encoding as encoding
 import ofscraper.utils.stdout as stdout
-from ofscraper.utils.logger import updateSenstiveDict
+import ofscraper.utils.logger as logger
+import ofscraper.constants as constants
+import ofscraper.utils.paths as paths
 log=logging.getLogger(__package__)
 console=Console()
 
+from diskcache import Cache
+
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MAX, max=constants.OF_MAX),reraise=True,after=lambda retry_state:print(f"Trying to login attempt:{retry_state.attempt_number}/{constants.NUM_TRIES}")) 
 def scrape_user(headers):
-    with httpx.Client(http2=True, headers=headers) as c:
-        url = constants.meEP
+    return _scraper_user_helper(json.dumps(headers))
 
-        auth.add_cookies(c)
-        c.headers.update(auth.create_sign(url, headers))
-        r = c.get(url, timeout=None)
-        if not r.is_error:
-            updateSenstiveDict(r.json()["id"],"userid")
-            updateSenstiveDict(r.json()["username"],"username")
-            updateSenstiveDict(r.json()["name"],"name")
-            return r.json()
-        r.raise_for_status()
 
+@lru_cache(maxsize=None)
+def _scraper_user_helper(headers):
+    headers = json.loads(headers)
+    cache = Cache(paths.getcachepath())
+    data=cache.get(f"myinfo_{headers['user-id']}",None)
+    if not data:
+        with httpx.Client(http2=True, headers=headers) as c:
+            url = constants.meEP
+            auth.add_cookies(c)
+            c.headers.update(auth.create_sign(url, headers))
+            r = c.get(url, timeout=None)
+            if not r.is_error:
+                data=r.json()
+            r.raise_for_status()
+    cache.set(f"myinfo_{headers['user-id']}",data,constants.HOURLY_EXPIRY)
+    cache.close()
+    logger.updateSenstiveDict(data["id"],"userid")
+    logger.updateSenstiveDict(data["username"],"username")
+    logger.updateSenstiveDict(data["name"],"name")
+    return data
 
 def parse_user(profile):
     name = encoding.encode_utf_16(profile['name'])
     username = profile['username']
 
     return (name, username)
```

### Comparing `ofscraper-2.5/ofscraper/api/messages.py` & `ofscraper-2.6/ofscraper/api/messages.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,15 @@
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 import asyncio
-import time
-import httpx
+import aiohttp
 import logging
 import contextvars
 from tenacity import retry,stop_after_attempt,wait_random
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
@@ -39,15 +38,15 @@
 log=logging.getLogger(__package__)
 attempt = contextvars.ContextVar("attempt")
 
 sem = semaphoreDelayed(constants.MAX_SEMAPHORE)
 
 
 
-async def get_messages(headers, model_id):
+async def get_messages(model_id):
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue"),),TextColumn("Getting Messages...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
 
     global tasks
@@ -56,53 +55,55 @@
 
     tasks=[]
     responseArray=[]
     page_count=0
     #require a min num of posts to be returned
     min_posts=50
     with Live(progress_group, refresh_per_second=constants.refreshScreen,console=console.shared_console): 
-        oldmessages=cache.get(f"messages_{model_id}",default=[]) if not args_.getargs().no_cache else []
-        oldmsgset=set(map(lambda x:x.get("id"),oldmessages))
-        log.debug(f"[bold]Messages Cache[/bold] {len(oldmessages)} found")
-        oldmessages=list(filter(lambda x:(x.get("createdAt") or x.get("postedAt"))!=None,oldmessages))
-        startdex=0 if len(oldmessages)==0 else \
-        max(([i for i in range(len(oldmessages)) if arrow.get(oldmessages[i].get("createdAt") or oldmessages[i].get("postedAt")) <=(args_.getargs().before or arrow.now())] or [len(oldmessages)])[0]-1,0)
-        log.debug(f"Setting Start Index at {startdex}")
-        postedAtArray=list(map(lambda x:x["id"],sorted(oldmessages,key=lambda x:arrow.get(x.get("createdAt") or x.get("postedAt") ).float_timestamp,reverse=True)))
-        postedAtArray=postedAtArray[startdex:]
+        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=None, connect=None,
+                      sock_connect=None, sock_read=None)) as c: 
+            oldmessages=cache.get(f"messages_{model_id}",default=[]) if not args_.getargs().no_cache else []
+            oldmsgset=set(map(lambda x:x.get("id"),oldmessages))
+            log.debug(f"[bold]Messages Cache[/bold] {len(oldmessages)} found")
+            oldmessages=list(filter(lambda x:(x.get("createdAt") or x.get("postedAt"))!=None,oldmessages))
+            startdex=0 if len(oldmessages)==0 else \
+            max(([i for i in range(len(oldmessages)) if arrow.get(oldmessages[i].get("createdAt") or oldmessages[i].get("postedAt")) <=(args_.getargs().before or arrow.now())] or [len(oldmessages)])[0]-1,0)
+            log.debug(f"Setting Start Index at {startdex}")
+            postedAtArray=list(map(lambda x:x["id"],sorted(oldmessages,key=lambda x:arrow.get(x.get("createdAt") or x.get("postedAt") ).float_timestamp,reverse=True)))
+            postedAtArray=postedAtArray[startdex:]
 
-    
         
-     
-        if len(postedAtArray)>min_posts:
-            splitArrays=[postedAtArray[i:i+min_posts] for i in range(0, len(postedAtArray), min_posts)]
-            #use the previous split for message_id
-            tasks.append(asyncio.create_task(scrape_messages(headers,model_id,job_progress,message_id=None if startdex==0 else splitArrays[0][0] ,required_ids=set(splitArrays[0]))))
-            [tasks.append(asyncio.create_task(scrape_messages(headers,model_id,job_progress,required_ids=set(splitArrays[i]),message_id=splitArrays[i-1][-1])))
-            for i in range(1,len(splitArrays)-1)]
-            # keeping grabbing until nothing left
-            tasks.append(asyncio.create_task(scrape_messages(headers,model_id,job_progress,message_id=splitArrays[-2][-1])))
-        else:
-            tasks.append(asyncio.create_task(scrape_messages(headers,model_id,job_progress,message_id=None if startdex==0 else postedAtArray[0])))
-    
-    
+            
+        
+            if len(postedAtArray)>min_posts:
+                splitArrays=[postedAtArray[i:i+min_posts] for i in range(0, len(postedAtArray), min_posts)]
+                #use the previous split for message_id
+                tasks.append(asyncio.create_task(scrape_messages(c,model_id,job_progress,message_id=None if startdex==0 else splitArrays[0][0] ,required_ids=set(splitArrays[0]))))
+                [tasks.append(asyncio.create_task(scrape_messages(c,model_id,job_progress,required_ids=set(splitArrays[i]),message_id=splitArrays[i-1][-1])))
+                for i in range(1,len(splitArrays)-1)]
+                # keeping grabbing until nothing left
+                tasks.append(asyncio.create_task(scrape_messages(c,model_id,job_progress,message_id=splitArrays[-2][-1])))
+            else:
+                tasks.append(asyncio.create_task(scrape_messages(c,model_id,job_progress,message_id=None if startdex==0 else postedAtArray[0])))
         
         
+            
+            
 
-        page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True)
+            page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True)
 
 
-        while len(tasks)!=0:
-            for coro in asyncio.as_completed(tasks):
-                result=await coro or []
-                page_count=page_count+1
-                overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
-                responseArray.extend(result)
-            tasks=list(filter(lambda x:x.done()==False,tasks))
-        overall_progress.remove_task(page_task)  
+            while len(tasks)!=0:
+                for coro in asyncio.as_completed(tasks):
+                    result=await coro or []
+                    page_count=page_count+1
+                    overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
+                    responseArray.extend(result)
+                tasks=list(filter(lambda x:x.done()==False,tasks))
+            overall_progress.remove_task(page_task)  
     unduped=[]
     dupeSet=set()
     log.debug(f"[bold]Messages Count with Dupes[/bold] {len(responseArray)} found")
     for message in responseArray:
         if message["id"] in dupeSet:
             continue
         dupeSet.add(message["id"])
@@ -118,68 +119,69 @@
         cache.set(f"message_check_{model_id}",[],expire=constants.CHECK_EXPIRY)
         cache.close()
         log.debug("Some messages where not retrived resetting cache")
 
     return unduped    
 
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
-async def scrape_messages(headers, model_id, progress,message_id=None,required_ids=None) -> list:
+async def scrape_messages(c, model_id, progress,message_id=None,required_ids=None) -> list:
     global sem
     global tasks
     messages=None
     attempt.set(attempt.get(0) + 1)
     ep = constants.messagesNextEP if message_id else constants.messagesEP
     url = ep.format(model_id, message_id)
     log.debug(f"{message_id if message_id else 'init'}{url}")
 
 
     async with sem:
-        task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Message ID-> {message_id if message_id else 'initial'}")
-        async with httpx.AsyncClient(http2=True, headers=headers) as c:
-            auth.add_cookies(c)
-            c.headers.update(auth.create_sign(url, headers))
-            r = await c.get(url, timeout=None)
-    if not r.is_error:
-
-        messages = r.json()['list']
-        log_id=f"offset messageid:{message_id if message_id else 'init id'}"
-        if not messages:
-            messages=[]
-        if len(messages)==0:
-            log.debug(f"{log_id} -> number of messages found 0")
-        elif len(messages)>0:
-            log.debug(f"{log_id} -> number of messages found {len(messages)}")
-            log.debug(f"{log_id} -> first date {messages[-1].get('createdAt') or messages[0].get('postedAt')}")
-            log.debug(f"{log_id} -> first ID {messages[0]['id']}")
-            log.debug(f"{log_id} -> last date {messages[-1].get('createdAt') or messages[0].get('postedAt')}")
-            log.debug(f"{log_id} -> last ID {messages[-1]['id']}")    
-            if (arrow.get( messages[-1].get("createdAt") or messages[-1].get("postedAt")).float_timestamp<(args_.getargs().after or arrow.get(0)).float_timestamp):
-                attempt.set(0)
-            elif required_ids==None:
-                attempt.set(0)
-                tasks.append(asyncio.create_task(scrape_messages(headers, model_id,progress,message_id=messages[-1]['id'])))
+        headers=auth.make_headers(auth.read_auth())
+        headers=auth.create_sign(url, headers)
+        async with c.request("get",url,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=headers) as r:
+            task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Message ID-> {message_id if message_id else 'initial'}")
+            
+            if r.ok:
+
+                messages = (await r.json())['list']
+                log_id=f"offset messageid:{message_id if message_id else 'init id'}"
+                if not messages:
+                    messages=[]
+                if len(messages)==0:
+                    log.debug(f"{log_id} -> number of messages found 0")
+                elif len(messages)>0:
+                    log.debug(f"{log_id} -> number of messages found {len(messages)}")
+                    log.debug(f"{log_id} -> first date {messages[-1].get('createdAt') or messages[0].get('postedAt')}")
+                    log.debug(f"{log_id} -> first ID {messages[0]['id']}")
+                    log.debug(f"{log_id} -> last date {messages[-1].get('createdAt') or messages[0].get('postedAt')}")
+                    log.debug(f"{log_id} -> last ID {messages[-1]['id']}")    
+                    if (arrow.get( messages[-1].get("createdAt") or messages[-1].get("postedAt")).float_timestamp<(args_.getargs().after or arrow.get(0)).float_timestamp):
+                        attempt.set(0)
+                    elif required_ids==None:
+                        attempt.set(0)
+                        tasks.append(asyncio.create_task(scrape_messages(c, model_id,progress,message_id=messages[-1]['id'])))
+                    else:
+                        [required_ids.discard(ele["id"]) for ele in messages]
+                        #try once more to grab, else quit
+                        if len(required_ids)==1:
+                            attempt.set(0)
+                            tasks.append(asyncio.create_task(scrape_messages(c, model_id,progress,message_id=messages[-1]['id'],required_ids=set())))
+
+                        elif len(required_ids)>0:
+                            attempt.set(0)
+                            tasks.append(asyncio.create_task(scrape_messages(c, model_id,progress,message_id=messages[-1]['id'],required_ids=required_ids)))
+                progress.remove_task(task)
+
             else:
-                [required_ids.discard(ele["id"]) for ele in messages]
-                #try once more to grab, else quit
-                if len(required_ids)==1:
-                    attempt.set(0)
-                    tasks.append(asyncio.create_task(scrape_messages(headers, model_id,progress,message_id=messages[-1]['id'],required_ids=set())))
-
-                elif len(required_ids)>0:
-                    attempt.set(0)
-                    tasks.append(asyncio.create_task(scrape_messages(headers, model_id,progress,message_id=messages[-1]['id'],required_ids=required_ids)))
-    else:
-        log.debug(f"[bold]message request status code:[/bold]{r.status_code}")
-        log.debug(f"[bold]message response:[/bold] {r.content.decode()}")
-        log.debug(f"[bold]message headers:[/bold] {r.headers}")
+                log.debug(f"[bold]message request status code:[/bold]{r.status}")
+                log.debug(f"[bold]message response:[/bold] {await r.text()}")
+                log.debug(f"[bold]message headers:[/bold] {r.headers}")
 
-        progress.remove_task(task)
-        r.raise_for_status()
+                progress.remove_task(task)
+                r.raise_for_status()
 
-    progress.remove_task(task)
     return messages
 
 def get_individual_post(model_id,postid,client=None):
     headers = auth.make_headers(auth.read_auth())
     url=constants.messageSPECIFIC.format(model_id,postid)
 
     auth.add_cookies(client)
```

### Comparing `ofscraper-2.5/ofscraper/api/paid.py` & `ofscraper-2.6/ofscraper/api/paid.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 import asyncio
-import httpx
+import aiohttp
 import logging
 import contextvars
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
@@ -59,65 +59,68 @@
     Panel(Group(job_progress)))
 
     output=[]
     global tasks
     tasks=[]
     page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console):
-        tasks.append(asyncio.create_task(scrape_paid(username,job_progress)))
-        
-        page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
-        while len(tasks)!=0:
-            for coro in asyncio.as_completed(tasks):
-                result=await coro or []
-                page_count=page_count+1
-                overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
-                output.extend(result)
-            tasks=list(filter(lambda x:x.done()==False,tasks))
-        overall_progress.remove_task(page_task)  
+        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=None, connect=None,
+                      sock_connect=None, sock_read=None)) as c: 
+
+            tasks.append(asyncio.create_task(scrape_paid(c,username,job_progress)))
+
+            
+            page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
+            while len(tasks)!=0:
+                for coro in asyncio.as_completed(tasks):
+                    result=await coro or []
+                    page_count=page_count+1
+                    overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
+                    output.extend(result)
+                tasks=list(filter(lambda x:x.done()==False,tasks))
+            overall_progress.remove_task(page_task)  
     log.debug(f"[bold]Paid Post count without Dupes[/bold] {len(output)} found")
     # set purchash check values during scan
     cache.set(f"purchased_check_{model_id}",output,expire=constants.CHECK_EXPIRY)
+    cache.close()
     return output
 
 
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
-async def scrape_paid(username,job_progress,offset=0):
+async def scrape_paid(c,username,job_progress,offset=0):
     """Takes headers to access onlyfans as an argument and then checks the purchased content
     url to look for any purchased content. If it finds some it will return it as a list."""
     global sem
     global tasks
     media = None
-    headers = auth.make_headers(auth.read_auth())
     attempt.set(attempt.get(0) + 1)
-    
+    url = constants.purchased_contentEP.format(offset,username)
     await sem.acquire()
     task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}",visible=True)
-    async with httpx.AsyncClient(http2=True, headers=headers, follow_redirects=True) as c:
-        auth.add_cookies(c)
-        url = constants.purchased_contentEP.format(offset,username)
-        c.headers.update(auth.create_sign(url, headers))
-        r = await c.get(url, timeout=None)
+    headers=auth.make_headers(auth.read_auth())
+    headers=auth.create_sign(url, headers)
+    async with c.request("get",url,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=headers) as r:
         sem.release()
-    if not r.is_error:
-        attempt.set(0)
-        media=list(filter(lambda x:isinstance(x,list),r.json().values()))[0]
-        log.debug(f"offset:{offset} -> media found {len(media)}")
-        log.debug(f"offset:{offset} -> hasmore value in json {r.json().get('hasMore','undefined') }")
-        if  r.json().get("hasMore"):
-            offset += len(media)
-            tasks.append(asyncio.create_task(scrape_paid(username,job_progress,offset=offset)))
-        job_progress.remove_task(task)
-
-    else:
-        log.debug(f"[bold]paid request status code:[/bold]{r.status_code}")
-        log.debug(f"[bold]paid response:[/bold] {r.content.decode()}")
-        log.debug(f"[bold]paid headers:[/bold] {r.headers}")
-        job_progress.remove_task(task)
-        r.raise_for_status()
+        if r.ok:
+            data=await r.json()
+            attempt.set(0)
+            media=list(filter(lambda x:isinstance(x,list),data.values()))[0]
+            log.debug(f"offset:{offset} -> media found {len(media)}")
+            log.debug(f"offset:{offset} -> hasmore value in json {data.get('hasMore','undefined') }")
+            if  data.get("hasMore"):
+                offset += len(media)
+                tasks.append(asyncio.create_task(scrape_paid(username,job_progress,offset=offset)))
+            job_progress.remove_task(task)
+
+        else:
+            log.debug(f"[bold]paid request status code:[/bold]{r.status}")
+            log.debug(f"[bold]paid response:[/bold] {await r.text()}")
+            log.debug(f"[bold]paid headers:[/bold] {r.headers}")
+            job_progress.remove_task(task)
+            r.raise_for_status()
     return media
 
 
 
 
 
 async def get_all_paid_posts():
@@ -129,105 +132,103 @@
 
     output=[]
     min_posts=100
     global tasks
     tasks=[]
     page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console):
-        allpaid=cache.get(f"purchased_all",default=[]) if not args_.getargs().no_cache else []
-        log.debug(f"[bold]All Paid Cache[/bold] {len(allpaid)} found")
-        
-      
-        if len(allpaid)>min_posts:
-            splitArrays=[i for i in range(0, len(allpaid), min_posts)]
-            #use the previous split for timesamp
-            tasks.append(asyncio.create_task(scrape_all_paid(job_progress,offset=0,count=0,required=0)))
-            [ tasks.append(asyncio.create_task(scrape_all_paid(job_progress,count=0,required=0,offset=splitArrays[i])))
-            for i in range(1,len(splitArrays))]
-            # keeping grabbing until nothign left
-            tasks.append(asyncio.create_task(scrape_all_paid(job_progress,offset=len(allpaid))))
-        else:
-            tasks.append(asyncio.create_task(scrape_all_paid(job_progress)))
+        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=None, connect=None,
+                      sock_connect=None, sock_read=None)) as c: 
+            allpaid=cache.get(f"purchased_all",default=[]) if not args_.getargs().no_cache else []
+            log.debug(f"[bold]All Paid Cache[/bold] {len(allpaid)} found")
             
         
-        
-        page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
-        while len(tasks)!=0:
-            for coro in asyncio.as_completed(tasks):
-                result=await coro or []
-                page_count=page_count+1
-                overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
-                output.extend(result)
-            tasks=list(filter(lambda x:x.done()==False,tasks))
-        overall_progress.remove_task(page_task)  
+            if len(allpaid)>min_posts:
+                splitArrays=[i for i in range(0, len(allpaid), min_posts)]
+                #use the previous split for timesamp
+                tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress,offset=0,count=0,required=0)))
+                [ tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress,count=0,required=0,offset=splitArrays[i])))
+                for i in range(1,len(splitArrays))]
+                # keeping grabbing until nothign left
+                tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress,offset=len(allpaid))))
+            else:
+                tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress)))
+                
+            
+            
+            page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
+            while len(tasks)!=0:
+                for coro in asyncio.as_completed(tasks):
+                    result=await coro or []
+                    page_count=page_count+1
+                    overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
+                    output.extend(result)
+                tasks=list(filter(lambda x:x.done()==False,tasks))
+            overall_progress.remove_task(page_task)  
     unduped=[]
     dupeSet=set()
     log.debug(f"[bold]Paid Post count with Dupes[/bold] {len(output)} found")
     for post in output:
         if post["id"] in dupeSet:
             continue
         dupeSet.add(post["id"])
         unduped.append(post)
     log.debug(f"[bold]Paid Post count[/bold] {len(unduped)} found")
     cache.set(f"purchased_all",output,expire=constants.RESPONSE_EXPIRY)
+    cache.close()
     return unduped
 
 
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
-async def scrape_all_paid(job_progress,offset=0,count=0,required=0):
+async def scrape_all_paid(c,job_progress,offset=0,count=0,required=0):
     """Takes headers to access onlyfans as an argument and then checks the purchased content
     url to look for any purchased content. If it finds some it will return it as a list."""
     global sem
     global tasks
     media = None
-    headers = auth.make_headers(auth.read_auth())
     attempt.set(attempt.get(0) + 1)
-    
     await sem.acquire()
+    url = constants.purchased_contentALL.format(offset)
     task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES} offset={offset}",visible=True)
-    async with httpx.AsyncClient(http2=True, headers=headers, follow_redirects=True) as c:
-        auth.add_cookies(c)
-        url = constants.purchased_contentALL.format(offset)
-        offset += 10
-        c.headers.update(auth.create_sign(url, headers))
-        r = await c.get(url, timeout=None)
+    headers=auth.make_headers(auth.read_auth())
+    headers=auth.create_sign(url, headers)
+    async with c.request("get",url,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=headers) as r:
         sem.release()
-    if not r.is_error:
-        attempt.set(0) 
-        log_id=offset or 0
-
-        
-        job_progress.remove_task(task)
-        media=list(filter(lambda x:isinstance(x,list),r.json().values()))[0]
-        if not r.json().get("hasMore"):
-            media=[]
-        if not media:
-            media=[]
-        if len(media)==0:
-            log.debug(f"offset:{log_id} -> number of post found 0")
-        elif len(media)>0:
-            log.debug(f"{log_id} -> number of post found {len(media)}")
-            log.debug(f"{log_id} -> first date {media[0].get('createdAt') or media[0].get('postedAt')}")
-            log.debug(f"{log_id} -> last date {media[-1].get('createdAt') or media[-1].get('postedAt')}")
-            log.debug(f"{log_id} -> first ID {media[0]['id']}")
-            log.debug(f"{log_id} -> last ID {media[-1]['id']}")
-            if required==0:
-                attempt.set(0)
-                tasks.append(asyncio.create_task(scrape_all_paid(job_progress,offset=offset+len(media))))
+        if r.ok:
+            attempt.set(0) 
+            log_id=f"offset {offset or 0}:"
+            data=await r.json()   
+            job_progress.remove_task(task)
+            media=list(filter(lambda x:isinstance(x,list),data.values()))[0]
+            if not data.get("hasMore"):
+                media=[]
+            if not media:
+                media=[]
+            if len(media)==0:
+                log.debug(f"{log_id} -> number of post found 0")
+            elif len(media)>0:
+                log.debug(f"{log_id} -> number of post found {len(media)}")
+                log.debug(f"{log_id} -> first date {media[0].get('createdAt') or media[0].get('postedAt')}")
+                log.debug(f"{log_id} -> last date {media[-1].get('createdAt') or media[-1].get('postedAt')}")
+                log.debug(f"{log_id} -> first ID {media[0]['id']}")
+                log.debug(f"{log_id} -> last ID {media[-1]['id']}")
+                if required==0:
+                    attempt.set(0)
+                    tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress,offset=offset+len(media))))
 
-            elif len(count)<len(required):
-                tasks.append(asyncio.create_task(scrape_all_paid(job_progress,offset=offset+len(media),required=required,count=count+len(media))))
+                elif len(count)<len(required):
+                    tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress,offset=offset+len(media),required=required,count=count+len(media))))
 
 
-        
+            
 
-    else:
-        log.debug(f"[bold]paid request status code:[/bold]{r.status_code}")
-        log.debug(f"[bold]paid response:[/bold] {r.content.decode()}")
-        log.debug(f"[bold]paid headers:[/bold] {r.headers}")
-        job_progress.remove_task(task)
-        r.raise_for_status()
+        else:
+            log.debug(f"[bold]paid request status code:[/bold]{r.status}")
+            log.debug(f"[bold]paid response:[/bold] {await r.text()}")
+            log.debug(f"[bold]paid headers:[/bold] {r.headers}")
+            job_progress.remove_task(task)
+            r.raise_for_status()
     return media
```

### Comparing `ofscraper-2.5/ofscraper/api/pinned.py` & `ofscraper-2.6/ofscraper/api/pinned.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 import time
 import asyncio
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 import logging
 import contextvars
 import math
-import httpx
+import aiohttp
 from tenacity import retry,stop_after_attempt,wait_random
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
 )
@@ -31,15 +31,15 @@
 import ofscraper.utils.args as args_
 
 log=logging.getLogger(__package__)
 attempt = contextvars.ContextVar("attempt")
 
 sem = semaphoreDelayed(constants.AlT_SEM)
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
-async def scrape_pinned_posts(headers, model_id,progress, timestamp=None,required_ids=None) -> list:
+async def scrape_pinned_posts(c, model_id,progress, timestamp=None,required_ids=None) -> list:
     global tasks
     global sem
     posts=None
     attempt.set(attempt.get(0) + 1)
     if timestamp and   (float(timestamp)>(args_.getargs().before or arrow.now()).float_timestamp):
         return []
     if timestamp:
@@ -49,71 +49,71 @@
         url = ep.format(model_id, timestamp)
     else:
         ep=constants.timelinePinnedEP
         url=ep.format(model_id)
     log.debug(url)
     async with sem:
         task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Timestamp -> {arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}",visible=True)
-        async with httpx.AsyncClient(http2=True, headers=headers) as c:
-            auth.add_cookies(c)
-            c.headers.update(auth.create_sign(url, headers))
-            r = await c.get(url , timeout=None)
-    if not r.is_error:
-        progress.remove_task(task)
-        posts = r.json()['list']
-        log_id=f"timestamp:{arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}"
-        if not posts:
-            posts= []
-        if len(posts)==0:
-            log.debug(f"{log_id} -> number of pinned post f found 0")
-        else:
-            log.debug(f"{log_id} -> number of pinned post found {len(posts)}")
-            log.debug(f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}")
-            log.debug(f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}")
-            log.debug(f"{log_id} -> first ID {posts[0]['id']}")
-            log.debug(f"{log_id} -> last ID {posts[-1]['id']}")
-        #post infinite loops            
-        # elif required_ids==None:
-        #     attempt.set(0)
-            # tasks.append(asyncio.create_task(scrape_pinned_posts(headers, model_id,progress,timestamp=posts[0]['postedAtPrecise'])))
-    else:
-            log.debug(f"[bold]pinned request status code:[/bold]{r.status_code}")
-            log.debug(f"[bold]pinned response:[/bold] {r.content.decode()}")
-            log.debug(f"[bold]pinned headers:[/bold] {r.headers}")
-            progress.remove_task(task)
-            r.raise_for_status()
+        headers=auth.make_headers(auth.read_auth())
+        headers=auth.create_sign(url, headers)
+        async with c.request("get",url,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=headers) as r:         
+            if r.ok:
+                progress.remove_task(task)
+                posts =( await r.json())['list']
+                log_id=f"timestamp:{arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}"
+                if not posts:
+                    posts= []
+                if len(posts)==0:
+                    log.debug(f"{log_id} -> number of pinned post f found 0")
+                else:
+                    log.debug(f"{log_id} -> number of pinned post found {len(posts)}")
+                    log.debug(f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}")
+                    log.debug(f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}")
+                    log.debug(f"{log_id} -> first ID {posts[0]['id']}")
+                    log.debug(f"{log_id} -> last ID {posts[-1]['id']}")
+                #post infinite loops            
+                # elif required_ids==None:
+                #     attempt.set(0)
+                    # tasks.append(asyncio.create_task(scrape_pinned_posts(headers, model_id,progress,timestamp=posts[0]['postedAtPrecise'])))
+            else:
+                    log.debug(f"[bold]pinned request status code:[/bold]{r.status}")
+                    log.debug(f"[bold]pinned response:[/bold] {await r.text()}")
+                    log.debug(f"[bold]pinned headers:[/bold] {r.headers}")
+                    progress.remove_task(task)
+                    r.raise_for_status()
     return posts
 
-async def get_pinned_post(headers,model_id): 
+async def get_pinned_post(model_id): 
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting pinned media...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
 
     global tasks
     tasks=[]
     min_posts=50
     responseArray=[]
     page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console): 
-
-        tasks.append(asyncio.create_task(scrape_pinned_posts(headers,model_id,job_progress,timestamp=args_.getargs().after.float_timestamp if args_.getargs().after else None)))
-    
-
-        page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True)
-        while len(tasks)!=0:
-            for coro in asyncio.as_completed(tasks):
-                result=await coro or []
-                page_count=page_count+1
-                overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
-                responseArray.extend(result)
-            time.sleep(1)
-            tasks=list(filter(lambda x:x.done()==False,tasks))
-        overall_progress.remove_task(page_task)
+        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=None, connect=None,
+                                    sock_connect=None, sock_read=None)) as c: 
+            tasks.append(asyncio.create_task(scrape_pinned_posts(c,model_id,job_progress,timestamp=args_.getargs().after.float_timestamp if args_.getargs().after else None)))
+        
+
+            page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True)
+            while len(tasks)!=0:
+                for coro in asyncio.as_completed(tasks):
+                    result=await coro or []
+                    page_count=page_count+1
+                    overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
+                    responseArray.extend(result)
+                time.sleep(1)
+                tasks=list(filter(lambda x:x.done()==False,tasks))
+            overall_progress.remove_task(page_task)
     unduped=[]
     dupeSet=set()
     log.debug(f"[bold]Pinned Count with Dupes[/bold] {len(responseArray)} found")
     for post in responseArray:
         if post["id"] in dupeSet:
             continue
         dupeSet.add(post["id"])
```

### Comparing `ofscraper-2.5/ofscraper/api/posts.py` & `ofscraper-2.6/ofscraper/api/posts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 import logging
-import httpx
+import aiohttp
 import arrow
 from ..constants import LICENCE_URL
 import ofscraper.utils.args as args_
 import ofscraper.utils.auth as auth
 from mpegdash.parser import MPEGDASHParser
 import ofscraper.utils.config as config
 
@@ -364,23 +364,23 @@
     @property
     def media(self):
         return self._media
     @property
     async def parse_mpd(self): 
         if not self.mpd:
             return
-        headers = auth.make_headers(auth.read_auth())
+      
         params={"Policy":self.policy,"Key-Pair-Id":self.keypair,"Signature":self.signature}
-        async with httpx.AsyncClient(http2=True, headers=headers,params=params) as c:
-            auth.add_cookies(c)
-            c.headers.update(auth.create_sign(self.mpd, headers))
-            r = await c.get(self.mpd, timeout=None)
-            if r.status_code!=200:
-                return None
-            return MPEGDASHParser.parse(r.content.decode())
+        async with aiohttp.ClientSession() as session:
+            headers=auth.make_headers(auth.read_auth())
+            headers=auth.create_sign(self.mpd, headers) 
+            async with session.request("get",self.mpd,headers=headers,params=params) as r:
+                if not r.ok:
+                    return None
+                return MPEGDASHParser.parse(await r.text())
     @property
     def license(self):
         if not self.mpd:
             return None
         responsetype=self.post.post["responseType"]
         if responsetype in ["timeline","archived","pinned"]:
             responsetype="post"
```

### Comparing `ofscraper-2.5/ofscraper/api/profile.py` & `ofscraper-2.6/ofscraper/api/profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import logging
 import contextvars
 
 from typing import Union
 import httpx
 from rich.console import Console
 from tenacity import retry,stop_after_attempt,wait_random
-from ..constants import profileEP,NUM_TRIES,DAILY_EXPIRY
+from ..constants import profileEP,NUM_TRIES,HOURLY_EXPIRY,DAILY_EXPIRY
 from ..utils import auth, encoding
 from xxhash import xxh128
 from diskcache import Cache
 from ..utils.paths import getcachepath
 import ofscraper.constants as constants
 cache = Cache(getcachepath())
 
@@ -27,26 +27,33 @@
 console=Console()
 attempt = contextvars.ContextVar("attempt")
 
 
 
 # can get profile from username or id
 @retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
-def scrape_profile(headers, username:Union[int, str]) -> dict:
+def scrape_profile(username:Union[int, str]) -> dict:
+    id=cache.get(f"username_{username}",None)
+    if id:
+        return id
+    headers = auth.make_headers(auth.read_auth())
+
     attempt.set(attempt.get(0) + 1)
     log.info(f"Attempt {attempt.get()}/{constants.NUM_TRIES} to get profile {username}")
     with httpx.Client(http2=True, headers=headers) as c:
         url = profileEP.format(username)
 
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
 
         r = c.get(profileEP.format(username), timeout=None)
         if not r.is_error:
             attempt.set(0)
+            cache.set(f"username_{username}",r.json(),int(HOURLY_EXPIRY*2))
+            cache.close()
             return r.json()
         elif r.status_code==404:
             return {"username":"modeldeleted"}
         r.raise_for_status()
 
 
 def parse_profile(profile: dict) -> tuple:
@@ -82,27 +89,28 @@
     header_fmt = 'Name: {} | Username: {} | ID: {} | Joined: {}\n'
     info_fmt = '- {} posts\n -- {} photos\n -- {} videos\n -- {} audios\n- {} archived posts'
     final_fmt = header_fmt + info_fmt
     log.info(final_fmt.format(*info))
 
 
 @retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
-def get_id(headers, username):
-    id=cache.get(f"model_id_{username}",None)
-    if id:
-        return id
+def get_id( username):
+    
+    headers = auth.make_headers(auth.read_auth())
     with httpx.Client(http2=True, headers=headers) as c:
         url = profileEP.format(username)
-
+        id=cache.get(f"model_id_{username}",None)
+        if id:
+            return id
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
-
         r = c.get(url, timeout=None)
         if not r.is_error:
             id=r.json()['id']
             cache.set(f"model_id_{username}",id,DAILY_EXPIRY)
+            cache.close()
             return id
         
         r.raise_for_status()
```

### Comparing `ofscraper-2.5/ofscraper/api/subscriptions.py` & `ofscraper-2.6/ofscraper/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.5/ofscraper/api/timeline.py` & `ofscraper-2.6/ofscraper/api/timeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
                  \/     \/           \/            \/         
 """
 import time
 import asyncio
 import logging
 import contextvars
 import math
-import httpx
+import aiohttp
 from tenacity import retry,stop_after_attempt,wait_random
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
 )
@@ -34,15 +34,15 @@
 from diskcache import Cache
 cache = Cache(getcachepath())
 log=logging.getLogger(__package__)
 attempt = contextvars.ContextVar("attempt")
 
 sem = semaphoreDelayed(constants.MAX_SEMAPHORE)
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
-async def scrape_timeline_posts(headers, model_id,progress, timestamp=None,required_ids=None) -> list:
+async def scrape_timeline_posts(c, model_id,progress, timestamp=None,required_ids=None) -> list:
     global tasks
     global sem
     posts=None
     attempt.set(attempt.get(0) + 1)
     if timestamp and   (float(timestamp)>(args_.getargs().before or arrow.now()).float_timestamp):
         return []
     if timestamp:
@@ -52,102 +52,104 @@
         url = ep.format(model_id, timestamp)
     else:
         ep=constants.timelineEP
         url=ep.format(model_id)
     log.debug(url)
     async with sem:
         task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Timestamp -> {arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}",visible=True)
-        async with httpx.AsyncClient(http2=True, headers=headers) as c:
-            auth.add_cookies(c)
-            c.headers.update(auth.create_sign(url, headers))
-            r = await c.get(url , timeout=None)
-    if not r.is_error:
-        progress.remove_task(task)
-        posts = r.json()['list']
-        log_id=f"timestamp:{arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}"
-        if not posts:
-            posts= []
-        if len(posts)==0:
-            log.debug(f"{log_id} -> number of post found 0")
-
-
-        elif len(posts)>0:
-            log.debug(f"{log_id} -> number of post found {len(posts)}")
-            log.debug(f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}")
-            log.debug(f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}")
-            log.debug(f"{log_id} -> first ID {posts[0]['id']}")
-            log.debug(f"{log_id} -> last ID {posts[-1]['id']}")
-
-            if required_ids==None:
-                attempt.set(0)
-                tasks.append(asyncio.create_task(scrape_timeline_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'])))
+        headers=auth.make_headers(auth.read_auth())
+        headers=auth.create_sign(url, headers)
+        async with c.request("get",url,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=headers) as r:
+            if r.ok:
+                progress.remove_task(task)
+                posts = (await r.json())['list']
+                log_id=f"timestamp:{arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}"
+                if not posts:
+                    posts= []
+                if len(posts)==0:
+                    log.debug(f"{log_id} -> number of post found 0")
+
+
+                elif len(posts)>0:
+                    log.debug(f"{log_id} -> number of post found {len(posts)}")
+                    log.debug(f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}")
+                    log.debug(f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}")
+                    log.debug(f"{log_id} -> first ID {posts[0]['id']}")
+                    log.debug(f"{log_id} -> last ID {posts[-1]['id']}")
+
+                    if required_ids==None:
+                        attempt.set(0)
+                        tasks.append(asyncio.create_task(scrape_timeline_posts(c, model_id,progress,timestamp=posts[-1]['postedAtPrecise'])))
+                    else:
+                        [required_ids.discard(float(ele["postedAtPrecise"])) for ele in posts]
+                        #try once more to get id if only 1 left
+                        if len(required_ids)==1:
+                            attempt.set(0)
+                            tasks.append(asyncio.create_task(scrape_timeline_posts(c, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=set())))
+
+                        elif len(required_ids)>0:
+                            attempt.set(0)
+                            tasks.append(asyncio.create_task(scrape_timeline_posts(c, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=required_ids)))
             else:
-                [required_ids.discard(float(ele["postedAtPrecise"])) for ele in posts]
-                #try once more to get id if only 1 left
-                if len(required_ids)==1:
-                    attempt.set(0)
-                    tasks.append(asyncio.create_task(scrape_timeline_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=set())))
-
-                elif len(required_ids)>0:
-                    attempt.set(0)
-                    tasks.append(asyncio.create_task(scrape_timeline_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=required_ids)))
-    else:
-            log.debug(f"[bold]timeline request status code:[/bold]{r.status_code}")
-            log.debug(f"[bold]timeline response:[/bold] {r.content.decode()}")
-            log.debug(f"[bold]timeline headers:[/bold] {r.headers}")
+                    log.debug(f"[bold]timeline request status code:[/bold]{r.status}")
+                    log.debug(f"[bold]timeline response:[/bold] {await r.text()}")
+                    log.debug(f"[bold]timeline headers:[/bold] {r.headers}")
 
-            progress.remove_task(task)
-            r.raise_for_status()
+                    progress.remove_task(task)
+                    r.raise_for_status()
     return posts
 
-async def get_timeline_post(headers,model_id): 
+async def get_timeline_post(model_id): 
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting timeline media...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
 
     global tasks
     tasks=[]
     min_posts=50
     responseArray=[]
     page_count=0
+    
     with Live(progress_group, refresh_per_second=5,console=console.shared_console): 
+        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=None, connect=None,
+                      sock_connect=None, sock_read=None)) as c: 
 
-        oldtimeline=cache.get(f"timeline_{model_id}",default=[]) if not args_.getargs().no_cache else []
-        oldtimeset=set(map(lambda x:x.get("id"),oldtimeline))
-        log.debug(f"[bold]Timeline Cache[/bold] {len(oldtimeline)} found")
-        oldtimeline=list(filter(lambda x:x.get("postedAtPrecise")!=None,oldtimeline))
-        postedAtArray=sorted(list(map(lambda x:float(x["postedAtPrecise"]),oldtimeline)))
-        filteredArray=list(filter(lambda x:x>=(args_.getargs().after or arrow.get(0)).float_timestamp,postedAtArray))
+            oldtimeline=cache.get(f"timeline_{model_id}",default=[]) if not args_.getargs().no_cache else []
+            oldtimeset=set(map(lambda x:x.get("id"),oldtimeline))
+            log.debug(f"[bold]Timeline Cache[/bold] {len(oldtimeline)} found")
+            oldtimeline=list(filter(lambda x:x.get("postedAtPrecise")!=None,oldtimeline))
+            postedAtArray=sorted(list(map(lambda x:float(x["postedAtPrecise"]),oldtimeline)))
+            filteredArray=list(filter(lambda x:x>=(args_.getargs().after or arrow.get(0)).float_timestamp,postedAtArray))
+            
+        
+        
+            if len(filteredArray)>min_posts:
+                splitArrays=[filteredArray[i:i+min_posts] for i in range(0, len(filteredArray), min_posts)]
+                #use the previous split for timesamp
+                tasks.append(asyncio.create_task(scrape_timeline_posts(c,model_id,job_progress,required_ids=set(splitArrays[0]),timestamp= splitArrays[0][0]-20000)))
+                [tasks.append(asyncio.create_task(scrape_timeline_posts(c,model_id,job_progress,required_ids=set(splitArrays[i]),timestamp=splitArrays[i-1][-1])))
+                for i in range(1,len(splitArrays)-1)]
+                # keeping grabbing until nothign left
+                tasks.append(asyncio.create_task(scrape_timeline_posts(c,model_id,job_progress,timestamp=splitArrays[-2][-1])))
+            else:
+                tasks.append(asyncio.create_task(scrape_timeline_posts(c,model_id,job_progress,timestamp=args_.getargs().after.float_timestamp if args_.getargs().after else None)))
         
-    
-       
-        if len(filteredArray)>min_posts:
-            splitArrays=[filteredArray[i:i+min_posts] for i in range(0, len(filteredArray), min_posts)]
-            #use the previous split for timesamp
-            tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,required_ids=set(splitArrays[0]),timestamp= splitArrays[0][0]-20000)))
-            [tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,required_ids=set(splitArrays[i]),timestamp=splitArrays[i-1][-1])))
-            for i in range(1,len(splitArrays)-1)]
-            # keeping grabbing until nothign left
-            tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,timestamp=splitArrays[-2][-1])))
-        else:
-            tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,timestamp=args_.getargs().after.float_timestamp if args_.getargs().after else None)))
-    
 
-        page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True)
-        while len(tasks)!=0:
-            for coro in asyncio.as_completed(tasks):
-                result=await coro or []
-                page_count=page_count+1
-                overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
-                responseArray.extend(result)
-            time.sleep(1)
-            tasks=list(filter(lambda x:x.done()==False,tasks))
-        overall_progress.remove_task(page_task)
+            page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True)
+            while len(tasks)!=0:
+                for coro in asyncio.as_completed(tasks):
+                    result=await coro or []
+                    page_count=page_count+1
+                    overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
+                    responseArray.extend(result)
+                time.sleep(1)
+                tasks=list(filter(lambda x:x.done()==False,tasks))
+            overall_progress.remove_task(page_task)
     unduped=[]
     dupeSet=set()
     log.debug(f"[bold]Timeline Count with Dupes[/bold] {len(responseArray)} found")
     for post in responseArray:
         if post["id"] in dupeSet:
             continue
         dupeSet.add(post["id"])
```

### Comparing `ofscraper-2.5/ofscraper/commands/check.py` & `ofscraper-2.6/ofscraper/commands/check.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,61 +93,62 @@
 
 
 
 
 
 
 def post_checker():
-    headers = auth.make_headers(auth.read_auth())
     user_dict = {}
-    client = httpx.Client(http2=True, headers=headers)
-    links = list(url_helper())
-    for ele in links:
-        name_match = re.search(f"onlyfans.com/({constants.USERNAME_REGEX}+$)", ele)
-        name_match2 = re.search(f"^{constants.USERNAME_REGEX}+$", ele)
-
-        if name_match:
-            user_name = name_match.group(1)
-            log.info(f"Getting Full Timeline for {user_name}")
-            model_id = profile.get_id(headers, user_name)
-        elif name_match2:
-            user_name = name_match2.group(0)
-            model_id = profile.get_id(headers, user_name)
-        else:
-            continue
-       
-        oldtimeline = cache.get(f"timeline_check_{model_id}", default=[])
-        if len(oldtimeline) > 0 and not args.force:
-            user_dict[user_name] = oldtimeline
-        elif not user_dict.get(user_name):
-            user_dict[user_name] = {}
-            user_dict[user_name] = user_dict[user_name] or []
-            user_dict[user_name].extend(asyncio.run(
-                timeline.get_timeline_post(headers, model_id)))
-            user_dict[user_name].extend(asyncio.run(
-                pinned.get_pinned_post(headers, model_id)))
-            user_dict[user_name].extend(asyncio.run(
-                archive.get_archived_post(headers, model_id)))
-            cache.set(
-                f"timeline_check_{model_id}", user_dict[user_name], expire=constants.CHECK_EXPIRY)
-
-    # individual links
-    for ele in list(filter(lambda x: re.search(f"onlyfans.com/{constants.NUMBER_REGEX}+/{constants.USERNAME_REGEX}+$", x), links)):
-        name_match = re.search(f"/({constants.USERNAME_REGEX}+$)", ele)
-        num_match = re.search(f"/({constants.NUMBER_REGEX}+)", ele)
-        if name_match and num_match:
-            user_name = name_match.group(1)
-            post_id=num_match.group(1)
-            model_id = profile.get_id(headers, user_name)
-            log.info(f"Getting Invidiual Link for {user_name}")
-            if not user_dict.get(user_name):
-                user_dict[name_match.group(1)] = {}
-            data = timeline.get_individual_post(post_id, client)
-            user_dict[user_name] = user_dict[user_name] or []
-            user_dict[user_name].append(data)
+    with httpx.Client(http2=True, headers=  auth.make_headers(auth.read_auth())) as c:
+        links = list(url_helper())
+        for ele in links:
+            name_match = re.search(f"onlyfans.com/({constants.USERNAME_REGEX}+$)", ele)
+            name_match2 = re.search(f"^{constants.USERNAME_REGEX}+$", ele)
+
+            if name_match:
+                user_name = name_match.group(1)
+                log.info(f"Getting Full Timeline for {user_name}")
+                model_id = profile.get_id( user_name)
+            elif name_match2:
+                user_name = name_match2.group(0)
+                model_id = profile.get_id( user_name)
+            else:
+                continue
+        
+            oldtimeline = cache.get(f"timeline_check_{model_id}", default=[])
+            if len(oldtimeline) > 0 and not args.force:
+                user_dict[user_name] = oldtimeline
+            elif not user_dict.get(user_name):
+                user_dict[user_name] = {}
+                user_dict[user_name] = user_dict[user_name] or []
+                user_dict[user_name].extend(asyncio.run(
+                    timeline.get_timeline_post( model_id)))
+                user_dict[user_name].extend(asyncio.run(
+                    pinned.get_pinned_post( model_id)))
+                user_dict[user_name].extend(asyncio.run(
+                    archive.get_archived_post( model_id)))
+                cache.set(
+                    f"timeline_check_{model_id}", user_dict[user_name], expire=constants.CHECK_EXPIRY)
+                cache.close()
+                
+
+        # individual links
+        for ele in list(filter(lambda x: re.search(f"onlyfans.com/{constants.NUMBER_REGEX}+/{constants.USERNAME_REGEX}+$", x), links)):
+            name_match = re.search(f"/({constants.USERNAME_REGEX}+$)", ele)
+            num_match = re.search(f"/({constants.NUMBER_REGEX}+)", ele)
+            if name_match and num_match:
+                user_name = name_match.group(1)
+                post_id=num_match.group(1)
+                model_id = profile.get_id( user_name)
+                log.info(f"Getting Invidiual Link for {user_name}")
+                if not user_dict.get(user_name):
+                    user_dict[name_match.group(1)] = {}
+                data = timeline.get_individual_post(post_id, c)
+                user_dict[user_name] = user_dict[user_name] or []
+                user_dict[user_name].append(data)
 
     ROWS=[]
     for user_name in user_dict.keys():
         downloaded = get_downloaded(user_name, model_id,True)
         media = get_all_found_media(user_name, user_dict[user_name])
         ROWS.extend(row_gather(media, downloaded, user_name))
     reset_url() 
@@ -179,18 +180,18 @@
     ROWS=[]
     for item in links:
         num_match = re.search(f"({constants.NUMBER_REGEX}+)", item) or re.search(f"^({constants.NUMBER_REGEX}+)$", item)
         name_match = re.search(f"^{constants.USERNAME_REGEX}+$", item)
         headers = auth.make_headers(auth.read_auth())
         if num_match:
             model_id = num_match.group(1)
-            user_name = profile.scrape_profile(headers, model_id)['username']
+            user_name = profile.scrape_profile( model_id)['username']
         elif name_match:
             user_name = name_match.group(0)
-            model_id = profile.get_id(headers, user_name) 
+            model_id = profile.get_id(user_name) 
         else:
             continue    
         log.info(f"Getting Messages/Paid content for {user_name}")
         # messages
         messages = None
         oldmessages = cache.get(f"message_check_{model_id}", default=[])
         log.debug(f"Number of messages in cache {len(oldmessages)}")
@@ -216,28 +217,29 @@
         id_set=set()
         for ele in media:
             if ele.id==None or ele.id not in id_set:
                 unduped.append(ele)
                 id_set.add(ele.id)
         downloaded = get_downloaded(user_name, model_id,True)
         ROWS.extend(row_gather(unduped, downloaded, user_name))
+    
     reset_url()
     set_count(ROWS)
     thread_starters(ROWS)
 
 
 
 def purchase_checker():
     user_dict = {}
     headers = auth.make_headers(auth.read_auth())
     ROWS = []
     for user_name in args.username:
-        user_name=profile.scrape_profile(headers,user_name)["username"]
+        user_name=profile.scrape_profile(user_name)["username"]
         user_dict[user_name] = user_dict.get(user_name, [])
-        model_id = profile.get_id(headers, user_name)
+        model_id = profile.get_id( user_name)
         oldpaid = cache.get(f"purchased_check_{model_id}", default=[])
         paid = None
         
         if len(oldpaid) > 0 and not args.force:
             paid = oldpaid
         else:
             paid = asyncio.run(paid_.get_paid_posts(user_name, model_id))
@@ -249,21 +251,20 @@
     reset_url()
     set_count(ROWS)
     thread_starters(ROWS)
 
 
 def stories_checker():
     user_dict = {}
-    headers = auth.make_headers(auth.read_auth())
     ROWS=[]
     for user_name in args.username:
-        user_name=profile.scrape_profile(headers,user_name)["username"]
+        user_name=profile.scrape_profile(user_name)["username"]
         user_dict[user_name] = user_dict.get(user_name, [])
-        model_id = profile.get_id(headers, user_name)    
-        highlights, stories = asyncio.run(highlights_.get_highlight_post(headers, model_id))
+        model_id = profile.get_id( user_name)    
+        highlights, stories = asyncio.run(highlights_.get_highlight_post( model_id))
         highlights=list(map(lambda x:posts_.Post(
         x, model_id, user_name,"highlights"), highlights))
         stories=list(map(lambda x:posts_.Post(
         x, model_id, user_name,"stories"), stories))
             
 
      
@@ -282,18 +283,17 @@
     out = []
     out.extend(args.file or [])
     out.extend(args.url or [])
     return map(lambda x: x.strip(), out)
 
 
 def get_all_found_media(user_name, posts):
-    headers = auth.make_headers(auth.read_auth())
 
     temp = []
-    model_id = profile.get_id(headers, user_name)
+    model_id = profile.get_id( user_name)
     posts_array=list(map(lambda x:posts_.Post(
         x, model_id, user_name), posts))
     [temp.extend(ele.all_media) for ele in posts_array]
     return temp
```

### Comparing `ofscraper-2.5/ofscraper/commands/manual.py` & `ofscraper-2.6/ofscraper/commands/manual.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,34 +34,33 @@
         model_id,
         value,
         )) 
     log.info(f"Finished")
 
 def get_media_from_urls(urls):
     args = args_.getargs()
-    headers = auth.make_headers(auth.read_auth())
     args.dupe=True
     args_.changeargs(args)
     user_name_dict={}
     id_dict={}
-    with httpx.Client(http2=True, headers=headers) as c:
+    with httpx.Client(http2=True) as c:
         for url in url_helper(urls):
             response=get_info(url)
             model=response[0]
             postid=response[1]
             type=response[2]
             if type=="post":
-                model_id=user_name_dict.get(model) or profile.get_id(headers, model)
+                model_id=user_name_dict.get(model) or profile.get_id( model)
                 user_name_dict[model]=model_id
                 id_dict[model_id]=id_dict.get(model_id,[])+[timeline.get_individual_post(postid,client=c)]
             elif type=="msg":
                 model_id=model
                 id_dict[model_id]=id_dict.get(model_id,[])+[messages_.get_individual_post(model_id,postid,client=c)]
             elif type=="msg2":
-                model_id=user_name_dict.get(model) or profile.get_id(headers, model)
+                model_id=user_name_dict.get(model) or profile.get_id( model)
                 id_dict[model_id]=id_dict.get(model_id,[])+[messages_.get_individual_post(model_id,postid,client=c)]
             elif type=="unknown":
                 data=unknown_type_helper(postid,c) or {}
                 model_id=data.get("author",{}).get("id")
                 id_dict[model_id]=id_dict.get(model_id,[])+[data]
             elif type=="highlights":
                 data=highlights_.get_individual_highlight(postid,c) or {}
@@ -87,19 +86,18 @@
     return timeline.get_individual_post(postid,client)
             
 
     
 
 def get_all_media(id_dict,inputtype=None):
     media_dict={}
-    headers = auth.make_headers(auth.read_auth())
 
     for model_id,value in  id_dict.items():
         temp = []
-        user_name = profile.scrape_profile(headers, model_id)['username']
+        user_name = profile.scrape_profile( model_id)['username']
         posts_array=list(map(lambda x:posts_.Post(
         x, model_id, user_name,responsetype=inputtype), value))
         [temp.extend(ele.media) for ele in posts_array]
         media_dict[model_id]=temp
    
    
     return media_dict
```

### Comparing `ofscraper-2.5/ofscraper/commands/scraper.py` & `ofscraper-2.6/ofscraper/commands/scraper.py`

 * *Files 10% similar despite different names*

```diff
@@ -83,28 +83,20 @@
 
             if result_profiles_prompt == 0:
                 # Change profiles
                 profiles.change_profile()
 
             elif result_profiles_prompt == 1:
                 # Edit a profile
-                profiles_ = profiles.get_profiles()
-
-                old_profile_name = prompts.edit_profiles_prompt(profiles_)
-                new_profile_name = prompts.new_name_edit_profiles_prompt(
-                    old_profile_name)
-
-                profiles.edit_profile_name(old_profile_name, new_profile_name)
+                profiles.edit_profile_name()
 
             elif result_profiles_prompt == 2:
                 # Create a new profile
-                profile_path = profiles.get_profile_path()
-                profile_name = prompts.create_profiles_prompt()
 
-                profiles.create_profile(profile_path, profile_name)
+                profiles.create_profile()
 
             elif result_profiles_prompt == 3:
                 # Delete a profile
                 profiles.delete_profile()
 
             elif result_profiles_prompt == 4:
                 # View profiles
@@ -136,18 +128,18 @@
             userdata=userselector.getselected_usernames()
             length=len(userdata)
             for count,ele in enumerate(userdata):
                 log.debug(f"getting content for {count+1}/{length} model")
                 if args.posts:
                     log.info(f"Getting {','.join(args.posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
                 try:
-                    model_id = profile.get_id(headers, ele["name"])
+                    model_id = profile.get_id( ele["name"])
                     operations.create_tables(model_id,ele['name'])
                     operations.write_profile_table(model_id,ele['name'])
-                    output.extend(OF.process_areas(headers, ele, model_id)) 
+                    output.extend(OF.process_areas( ele, model_id)) 
                 except Exception as e:
                     log.traceback(f"failed with exception: {e}")
                     log.traceback(traceback.format_exc())               
             if args.scrape_paid:
                 output.extend(OF.process_all_paid())
             user_dict={}
             [user_dict.update({ele.post.model_id:user_dict.get(ele.post.model_id,[])+[ele]}) for ele in output]
@@ -169,18 +161,18 @@
         userdata=userselector.getselected_usernames() if "None" not in args.posts else []
         length=len(userdata)
         for count,ele in enumerate(userdata):
             log.debug(f"Getting content+downloading {count+1}/{length} model")
             if args.posts:
                 log.info(f"Getting {','.join(args.posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
             try:
-                model_id = profile.get_id(headers, ele["name"])
+                model_id = profile.get_id( ele["name"])
                 operations.create_tables(model_id,ele['name'])
                 operations.write_profile_table(model_id,ele['name'])
-                combined_urls=OF.process_areas(headers, ele, model_id)
+                combined_urls=OF.process_areas( ele, model_id)
                 asyncio.run(download.process_dicts(
                 ele["name"],
                 model_id,
                 combined_urls,
                 ))
             except Exception as e:
                 log.traceback(f"failed with exception: {e}")
@@ -205,42 +197,43 @@
                 log.traceback(traceback.format_exc())     
             
 
 def process_like():
     with scrape_context_manager():
         profiles.print_current_profile()
         headers = auth.make_headers(auth.read_auth())
+        init.print_sign_status(headers)
         userdata=userselector.getselected_usernames()
         with stdout.lowstdout():
             for ele in list(filter(lambda x: x["active"],userdata)):
-                    model_id = profile.get_id(headers, ele["name"])
-                    posts = like.get_posts(headers, model_id)
+                    model_id = profile.get_id( ele["name"])
+                    posts = like.get_posts(model_id)
                     unfavorited_posts = like.filter_for_unfavorited(posts)  
                     unfavorited_posts=filters.timeline_array_filter(unfavorited_posts)   
                     log.debug(f"[bold]Number of unliked posts left after date filters[/bold] {len(unfavorited_posts)}")
                     post_ids = like.get_post_ids(unfavorited_posts)
                     log.debug(f"[bold]Final Number of open and likable post[/bold] {len(post_ids)}")
-                    like.like(headers, model_id, ele["name"], post_ids)
+                    like.like( model_id, ele["name"], post_ids)
 
 def process_unlike():
     with scrape_context_manager(): 
         profiles.print_current_profile()
         headers = auth.make_headers(auth.read_auth())
         init.print_sign_status(headers)
         userdata=userselector.getselected_usernames()
         with stdout.lowstdout():
             for ele in list(filter(lambda x: x["active"],userdata)):
-                    model_id = profile.get_id(headers, ele["name"])
-                    posts = like.get_posts(headers, model_id)
+                    model_id = profile.get_id( ele["name"])
+                    posts = like.get_posts( model_id)
                     favorited_posts = like.filter_for_favorited(posts)
                     favorited_posts=filters.timeline_array_filter(favorited_posts) 
                     log.debug(f"[bold]Number of liked posts left after date filters[/bold] {len(favorited_posts)}")
                     post_ids = like.get_post_ids(favorited_posts)
                     log.debug(f"[bold]Final Number of open and unlikable post[/bold] {len(post_ids)}")
-                    like.unlike(headers, model_id, ele["name"], post_ids)
+                    like.unlike( model_id, ele["name"], post_ids)
 #Adds a function to the job queue
 def set_schedule(*functs):
     [schedule.every(args.daemon).minutes.do(jobqueue.put,funct) for funct in functs]
     while True:
         schedule.run_pending()
         time.sleep(30)
 
@@ -355,18 +348,14 @@
                     log.traceback(traceback.format_exc())
                     sys.exit(0)
             except KeyboardInterrupt:
                 sys.exit(0)
 def scrapper():
     if platform.system == 'Windows':
         os.system('color')
-    # try:
-    #     webbrowser.open(donateEP)
-    # except:
-    #     pass
     global selectedusers
     selectedusers=None
     functs=[]
     if len(args.posts)==0 and not args.action and not args.scrape_paid:
         if args.daemon:
                     log.error("You need to pass at least one scraping method\n--action\n--posts\n--purchase\nAre all valid options. Skipping and going to menu")
         process_prompts()
```

### Comparing `ofscraper-2.5/ofscraper/constants.py` & `ofscraper-2.6/ofscraper/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
             "profile":"Profile",
             "pinned":"Posts"
         }
 NUM_TRIES=10
 RESPONSE_EXPIRY=5000000
 CHECK_EXPIRY=86400
 DAILY_EXPIRY=86400
+HOURLY_EXPIRY=3600
 DISCORDWAIT=5
 OF_MIN=15
 OF_MAX=50
 LICENCE_URL="https://onlyfans.com/api2/v2/users/media/{}/drm/{}/{}?type=widevine"
 logname="ofscraper"
 PATH_STR_MAX=200
 TABLE_STR_MAX=100
```

### Comparing `ofscraper-2.5/ofscraper/db/operations.py` & `ofscraper-2.6/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.5/ofscraper/db/queries.py` & `ofscraper-2.6/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.5/ofscraper/interaction/like.py` & `ofscraper-2.6/ofscraper/interaction/like.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 
 import random
 import time
 import logging
 from typing import Union
 import asyncio
-import httpx
+import aiohttp
 
 from tenacity import retry,stop_after_attempt,wait_random
 
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     MofNCompleteColumn,
@@ -38,28 +38,29 @@
 
 sem = semaphoreDelayed(1)
 log=logging.getLogger(__package__)
 import ofscraper.utils.args as args_
 
 
 
-def get_posts(headers, model_id):
+def get_posts( model_id):
     pinned_posts=[]
     timeline_posts=[]
     archived_posts=[]
     args=args_.getargs()
 
+
     args.posts = list(map(lambda x:x.capitalize(),(args.posts or prompts.like_areas_prompt())
     ))
     if ('Pinned' in args.posts or 'All' in args.posts):
-        pinned_posts = asyncio.run(pinned.get_pinned_post(headers, model_id))
+        pinned_posts = asyncio.run(pinned.get_pinned_post( model_id))
     if ('Timeline' in args.posts or 'All' in args.posts):
-        timeline_posts = asyncio.run(timeline.get_timeline_post(headers, model_id))
+        timeline_posts = asyncio.run(timeline.get_timeline_post( model_id))
     if ('Archived' in args.posts or 'All' in args.posts):
-        archived_posts = asyncio.run(archive.get_archived_post(headers, model_id))
+        archived_posts = asyncio.run(archive.get_archived_post( model_id))
     log.debug(f"[bold]Number of Post Found[/bold] {len(pinned_posts) + len(timeline_posts) + len(archived_posts)}")
     return pinned_posts + timeline_posts + archived_posts
 
 
 def filter_for_unfavorited(posts: list) -> list:
     output=list(filter(lambda x:x.get("isFavorite")==False,posts))
     log.debug(f"[bold]Number of unliked post[/bold] {len(output)}")
@@ -77,63 +78,63 @@
 
 def get_post_ids(posts: list) -> list:
     valid_post=list(filter(lambda x:x.get("isOpened")==True,posts))
     return list(map(lambda x:x.get("id"),valid_post))
    
 
 
-def like(headers, model_id, username, ids: list):
+def like( model_id, username, ids: list):
+    headers = auth.make_headers(auth.read_auth())
     asyncio.run(_like(headers, model_id, username, ids, True))
 
 
-def unlike(headers, model_id, username, ids: list):
+def unlike( model_id, username, ids: list):
+    headers = auth.make_headers(auth.read_auth())
     asyncio.run(_like(headers, model_id, username, ids, False))
 
 
 
 
 async def _like(headers, model_id, username, ids: list, like_action: bool):
     title = "Liking" if like_action else "Unliking"
     global sem
     sem.delay=3
     with Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}"),BarColumn(),MofNCompleteColumn(),console=console.shared_console) as overall_progress:
-        tasks=[]
-        task1=overall_progress.add_task(f"{title} posts...\n",total=len(ids))
-
-        [tasks.append(asyncio.create_task(_like_request(headers,id,model_id,username)))
-            for id in ids]
-        for count,coro in enumerate(asyncio.as_completed(tasks)):
-                id=await coro
-                log.debug(f"ID: {id} Performed {'like' if like_action==True else 'unlike'} action")
-                if count+1%60==0 and count+1%50==0:
-                    sem.delay=15
-                elif count+1%60==0:
-                    sem.delay=3
-                elif count+1%50==0:
-                    sem.delay=30  
-                 
-                overall_progress.update(task1,advance=1,refresh=True)
+        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=None, connect=None,
+                      sock_connect=None, sock_read=None)) as c: 
+            tasks=[]
+            task1=overall_progress.add_task(f"{title} posts...\n",total=len(ids))
+
+            [tasks.append(asyncio.create_task(_like_request(c,id,model_id)))
+                for id in ids]
+            for count,coro in enumerate(asyncio.as_completed(tasks)):
+                    id=await coro
+                    log.debug(f"ID: {id} Performed {'like' if like_action==True else 'unlike'} action")
+                    if count+1%60==0 and count+1%50==0:
+                        sem.delay=15
+                    elif count+1%60==0:
+                        sem.delay=3
+                    elif count+1%50==0:
+                        sem.delay=30  
+                    
+                    overall_progress.update(task1,advance=1,refresh=True)
 
         
         
 
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
-async def _like_request(headers,id,model_id,username):
+async def _like_request(c,id,model_id):
     async with sem:
-        with httpx.Client(http2=True, headers=headers) as c:
-            url = favoriteEP.format(id, model_id)
-            auth.add_cookies(c)
-            c.headers.update(auth.create_sign(url, headers))
-            r = c.post(url)
-    
-            if not r.is_error or r.status_code == 400:
-                return id
-                     
-            
-            log.debug(f"[bold]timeline request status code:[/bold]{r.status_code}")
-            log.debug(f"[bold]timeline response:[/bold] {r.content.decode()}")
+        url = favoriteEP.format(id, model_id)
+        headers=auth.make_headers(auth.read_auth())
+        headers=auth.create_sign(url, headers)
+        async with c.request("post",url,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=headers) as r:
+            if r.ok:
+                return id                  
+            log.debug(f"[bold]timeline request status code:[/bold]{r.status}")
+            log.debug(f"[bold]timeline response:[/bold] {await r.text()}")
             log.debug(f"[bold]timeline headers:[/bold] {r.headers}")
             r.raise_for_status()
```

### Comparing `ofscraper-2.5/ofscraper/prompts/prompt_strings.py` & `ofscraper-2.6/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.5/ofscraper/prompts/prompt_validators.py` & `ofscraper-2.6/ofscraper/prompts/prompt_validators.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import string
 from pathvalidate import  validate_filepath,validate_filename
 import platform
 import pathlib
 import arrow
 import textwrap
 import ofscraper.utils.paths as paths
-import ofscraper.utils.stdout as stdout
+import ofscraper.utils.profiles as profiles
 
 
 
 class MultiValidator(Validator):
     """:Runs Multiple Validators Since Inquirerpy does seem to support this functionality natively
 
     Args:
@@ -24,18 +24,48 @@
         self,
         *args):
         self.inputs=args
 
     def validate(self,document) -> None:
        for input in self.inputs:
             try:
-                input.validate(document)
+                if isinstance(input,Validator):
+                    input.validate(document)
+                else:
+                    if input(document.text)==False: 
+                        raise Exception()
             except Exception as E:
                 raise E
                 
+def currentProfilesValidator():
+    def callable(x):
+        x=profiles.profile_name_fixer(x)
+        return x not in set(profiles.get_profile_names())
+    return Validator.from_callable(
+    callable,
+    "You can not change name to a current profile name"
+    )
+
+def currentProfilesCreationValidator():
+    def callable(x):
+        x=profiles.profile_name_fixer(x)
+        return x not in set(profiles.get_profile_names())
+    return Validator.from_callable(
+    callable,
+    "This Profile already exists"
+    )
+def currentProfileDeleteValidator():
+    def callable(x):
+        return profiles.profile_name_fixer(x)!=profiles.get_active_profile()
+    
+    return Validator.from_callable(
+    callable,
+    "You can not delete the active profile"
+    )
+
 def emptyListValidator():
     def callable(x):
         return len(x)>0
     return Validator.from_callable(
     callable,
     "You must select at least one"
     )
```

### Comparing `ofscraper-2.5/ofscraper/prompts/prompts.py` & `ofscraper-2.6/ofscraper/prompts/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,35 +287,35 @@
     name = 'new_name'
 
     questions = [
         {
             'type': 'input',
             'name': name,
             'message': f'What would you like to rename {old_profile_name} to?',
-            'validator':EmptyInputValidator()
+            'validate':prompt_validators.MultiValidator(EmptyInputValidator(),prompt_validators.currentProfilesValidator())
         }
     ]
 
     answer = prompt(questions)
     return answer[name]
 
-
 def create_profiles_prompt() -> str:
     name = 'create'
 
     questions = [
         {
             'type': 'input',
             'name': name,
             'message': 
 """
 What would you like to name your new profile?
 only letters, numbers, and underscores are allowed
 """,
-            'validator':prompt_validators.namevalitator()
+            'validate':prompt_validators.MultiValidator(prompt_validators.namevalitator(),prompt_validators.currentProfilesCreationValidator()
+)
 
         }
     ]
 
     answer = prompt(questions)
     return answer[name]
 
@@ -325,15 +325,17 @@
 
     questions = [
         {
             'type': 'list',
             'name': name,
             'message': 'Select Profile',
             'choices':profiles
-            ,"validate":prompt_validators.emptyListValidator()
+            ,"validate":prompt_validators.MultiValidator(  prompt_validators.emptyListValidator(),prompt_validators.currentProfileDeleteValidator())
+            
+          
         }
     ]
     answer = prompt(questions)
     profile = answer[name]
     return profile
 
 
@@ -452,26 +454,24 @@
             'type': 'filepath',
             'name': 'mp4decrypt',
             "message":"mp4decrypt path: ",
              "validate":prompt_validators.MultiValidator(EmptyInputValidator(),prompt_validators.mp4decryptpathvalidator(),prompt_validators.mp4decryptexecutevalidator()),
             "default":config.get_mp4decrypt(config_),
             "long_instruction":             """
 Certain content requires decryption to process please provide the full path to mp4decrypt
-Linux version [mp4decrypt] and windows version [mp4decrypt.exe] are provided in the repo         
 """
         },
         {
                         'type': 'filepath',
             'name': 'ffmpeg',
             "message":"ffmpeg path: ",
              "validate":prompt_validators.MultiValidator(EmptyInputValidator(),prompt_validators.ffmpegpathvalidator(),prompt_validators.ffmpegexecutevalidator()),
              "long_instruction": 
              """
 Certain content requires decryption to process please provide the full path to ffmpeg
-Linux version [ffmpeg] and windows version [ffmpeg.exe] are provided in the repo         
 """,
 "default":config.get_ffmpeg(config_)
         
         },
 
         {
             'type': 'input',
@@ -895,7 +895,21 @@
             "instruction":"\nKeyBindings\nSubmit: esc+Enter or Home+Enter or pageDown +Enter",
         }
     ]
 
 
     answer = prompt(questions)
     return answer[0]
+
+def relative_config_path_prompt(curr,file) -> bool:
+    name = 'path'
+    questions = [
+        {
+            'type': 'list',
+            'name': name,
+            'message': "Where do you want to make the config folder",
+            'choices':[Choice(True,str(pathlib.Path(curr,file))),Choice(False,str(pathlib.Path(file)))]
+        }
+    ]
+
+    answer = prompt(questions)
+    return answer[name]
```

### Comparing `ofscraper-2.5/ofscraper/utils/args.py` & `ofscraper-2.6/ofscraper/utils/args.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,83 +4,79 @@
 import re
 import arrow
 import pathlib
 from ofscraper.__version__ import __version__ 
 
 args=None
 log=logging.getLogger(__package__)
-def getargs(input=None):
-    global args
-    if args and input==None:
-        return args
-    if "pytest" in sys.modules and input==None:
-        input=[]
-    elif input==None:
-        input=sys.argv[1:]
+def create_parser(input=None):
     parent_parser=argparse.ArgumentParser(add_help=False)
-    general=parent_parser.add_argument_group("General",description="General Args")  
+    general=parent_parser.add_argument_group("Program",description="Program Args")  
     general.add_argument('-v', '--version', action='version', version=__version__ ,default=__version__)
+    general.add_argument(
+        '-cg', '--config', help="Change location of config folder/file",default=None
+    )
+    general.add_argument(
+        '-r', '--profile', help="Change which profile you want to use\nIf not set then the config file is used\nProfiles are always within the config file parent directory",default=None,type=lambda x:f"{re.sub('_profile','', x)}_profile"
+    )
     output=parent_parser.add_argument_group("Logging",description="Arguments for output controls")  
 
     output.add_argument(
         '-l', '--log', help = 'set log file level', type=str.upper,default="OFF",choices=["OFF","STATS","LOW","NORMAL","DEBUG"]
     ),
     output.add_argument(
         '-dc', '--discord', help = 'set discord log level', type=str.upper,default="OFF",choices=["OFF","STATS","LOW","NORMAL","DEBUG"]
     )
 
     output.add_argument(
         '-p', '--output', help = 'set console output log level', type=str.upper,default="NORMAL",choices=["PROMPT","STATS","LOW","NORMAL","DEBUG"]
     )
-    output.add_argument(
-        '-cg', '--config', help="Change location of config folder/file",default=None
-    )
-    output.add_argument(
-        '-au', '--auth', help="Change location of auth file",default=None
-    )
+  
 
 
-    parser = argparse.ArgumentParser(add_help=False,parents=[parent_parser])  
+    parser = argparse.ArgumentParser(add_help=False,parents=[parent_parser],prog="OF-Scraper")  
     parser.add_argument( '-h', '--help', action='help')
     scraper=parser.add_argument_group("scraper",description="General Arguments for scraper")                                
     scraper.add_argument(
         '-u', '--username', help="select which username to process (name,name2)\nSet to ALL for all users",type=username_helper,action="extend"
     )
     scraper.add_argument(
         '-eu', '--excluded-username', help="select which usernames to exclude  (name,name2)\nThis has preference over --username",type=username_helper,action="extend"
     )
   
     scraper.add_argument(
         '-d', '--daemon', help='run script in the background\nSet value to minimum minutes between script runs\nOverdue runs will run as soon as previous run finishes', type=int,default=None
     )
 
     scraper.add_argument(
-        '-g', '--original', help = 'don\'t trunicate long paths', default=False,action="store_true"
+        '-g', '--original', help = 'don\'t truncate long paths', default=False,action="store_true"
     )
+    scraper.add_argument("-c","--letter-count",action="store_true",default=False,help="intrepret config 'textlength' as max length by letter")
+    scraper.add_argument("-a","--action",default=None,help="perform like or unlike action on each post",choices=["like","unlike"])
 
 
     post=parser.add_argument_group("Post",description="What type of post to scrape")                                      
 
     post.add_argument("-e","--dupe",action="store_true",default=False,help="Bypass the dupe check and redownload all files")
     post.add_argument(
         '-o', '--posts', help = 'Download content from a model',default=[],required=False,type = posttype_helper,action='extend'
     )
-    post.add_argument("-c","--letter-count",action="store_true",default=False,help="intrepret config 'textlength' as max length by letter")
 
-    post.add_argument("-a","--action",default=None,help="perform like or unlike action on each post",choices=["like","unlike"])
-    post.add_argument("-sk","--skip-timed",default=None,help="skip promotional or tempory post",action="store_true")
+    post.add_argument("-sk","--skip-timed",default=None,help="skip promotional or temporary post",action="store_true")
     post.add_argument(
         '-ft', '--filter', help = 'Filter post by provide regex\nNote if you include any uppercase characters the search will be case-sensitive',default=".*",required=False,type = str
     )
     post.add_argument(
         '-sp', '--scrape-paid', help = 'scrape the entire paid page for content. This can take a very long time',default=False,required=False,action="store_true"
     )
+
     post.add_argument(
-        '-nc', '--no-cache', help = 'disable cache',default=False,required=False,action="store_true"
+        '-dt', '--download-type', help = 'Filter to what type of download you want None==Both, protected=Files that need mp4decrpyt',default=None,required=False,type=str.lower,choices=["protected","normal"]
     )
+   
 
      #Filters for accounts
     filters=parser.add_argument_group("filters",description="Filters out usernames based on selected parameters")
     
     filters.add_argument(
         '-at', '--account-type', help = 'Filter Free or paid accounts\npaid and free correspond to your original price, and not the renewal price',default=None,required=False,type = str.lower,choices=["paid","free"]
     )
@@ -103,94 +99,110 @@
     sort.add_argument(
         '-ds', '--desc', help = 'Sort the model list in descending order',action="store_true",default=False) 
     
     advanced=parser.add_argument_group("Advanced",description="Advanced Args")  
     advanced.add_argument(
         '-uf', '--users-first', help = 'Scrape all users first rather then one at a time. This only effects downloading posts',default=False,required=False,action="store_true"
     )
+    advanced.add_argument(
+        '-nc', '--no-cache', help = 'disable cache',default=False,required=False,action="store_true"
+    )
 
     subparser=parser.add_subparsers(help="commands",dest="command")
-    post_check=subparser.add_parser("post_check",help="Check if data from a post\nCache lasts for 24 hours",parents=[parent_parser])
+    post_check=subparser.add_parser("post_check",help="Display a generated table of data with information about models post(s)\nCache lasts for 24 hours",parents=[parent_parser])
 
 
     post_check.add_argument("-u","--url",
-    help = 'Check if media is in library via url',default=None,required=False,type = check_strhelper,action='extend'
+    help = 'Scan posts via url',default=None,required=False,type = check_strhelper,action='extend'
     )
 
 
     post_check.add_argument("-f","--file",
-    help = 'Check if media is in library via file',default=None,required=False,type = check_filehelper
+    help = 'Scan posts via file\nWith line seperated URL(s)',default=None,required=False,type = check_filehelper
     )
     
     post_check.add_argument(
-        '-fo', '--force', help = 'force retrival of new posts info from API', default=False,action="store_true"
+        '-fo', '--force', help = 'force retrieval of new posts info from API', default=False,action="store_true"
     )
 
-    message_check=subparser.add_parser("msg_check",help="Parse a user's messages and view status of missing media\nCache lasts for 24 hours",parents=[parent_parser])
+    message_check=subparser.add_parser("msg_check",help="Display a generated table of data with information about models messages\nCache lasts for 24 hours",parents=[parent_parser])
     message_check.add_argument(
-        '-fo', '--force', help = 'force retrival of new posts info from API', default=False,action="store_true"
+        '-fo', '--force', help = 'force retrieval of new messages info from API', default=False,action="store_true"
     )
     message_check.add_argument("-f","--file",
-    help = 'Check if media is in library via file',default=None,required=False,type = check_filehelper
+    help = 'Scan messages via file\nWith line seperated URL(s)',default=None,required=False,type = check_filehelper
     )
     
 
     message_check.add_argument("-u","--url",
-    help = 'link to conversation',type = check_strhelper,action="extend")
-    message_check.add_argument("-un","--username",
-    help = 'link to conversation',type = check_strhelper,action="extend")
+    help = 'scan messages via file',type = check_strhelper,action="extend")
+ 
 
-    paid_check=subparser.add_parser("paid_check",help="Parse Purchases sent from a user\nCache last for 24 hours",parents=[parent_parser])
+    paid_check=subparser.add_parser("paid_check",help="Display a generated table of data with information purchashes from model\nCache last for 24 hours",parents=[parent_parser])
     paid_check.add_argument(
-        '-fo', '--force', help = 'force retrival of new posts info from API', default=False,action="store_true"
+        '-fo', '--force', help = 'force retrieval of new purchases info from API', default=False,action="store_true"
     )
     paid_check.add_argument("-f","--file",
-    help = 'Check if media is in library via file',default=None,required=False,type = check_filehelper
+    help = 'Scan purchases via file\nWith line seperated usernames(s)',default=None,required=False,type = check_filehelper
     )
     
 
-    paid_check.add_argument("-us","--username",
-    help = 'link to conversation',type = check_strhelper,action="extend")
+    paid_check.add_argument("-u","--username",
+    help = 'Scan purchases via usernames',type = check_strhelper,action="extend")
 
 
 
 
     story_check=subparser.add_parser("story_check",help="Parse Stories/Highlights sent from a user\nCache last for 24 hours",parents=[parent_parser])
     story_check.add_argument(
-        '-fo', '--force', help = 'force retrival of new posts info from API', default=False,action="store_true"
+        '-fo', '--force', help = 'force retrieval of new posts info from API', default=False,action="store_true"
     )
     story_check.add_argument("-f","--file",
-    help = 'Check if media is in library via file',default=None,required=False,type = check_filehelper
+    help = 'Scan mevia file',default=None,required=False,type = check_filehelper
     )
     
 
-    story_check.add_argument("-us","--username",
+    story_check.add_argument("-u","--username",
     help = 'link to conversation',type = check_strhelper,action="extend")
 
     manual=subparser.add_parser("manual",help="Manually download content via url or ID",parents=[parent_parser])
     manual.add_argument("-f","--file",
     help = 'Pass links/IDs to download via file',default=None,required=False,type = check_filehelper
     )
-    manual.add_argument("-us","--url",
+    manual.add_argument("-u","--url",
     help = 'pass links to download via url',type = check_strhelper,action="extend")
 
+    return parser
+  
+    
 
+def getargs(input=None):
+    global args
+    if args and input==None:
+        return args
+    if "pytest" in sys.modules and input==None:
+        input=[]
+    elif input==None:
+        input=sys.argv[1:]
+    parser=create_parser(input)
     args=parser.parse_args(input)
     #deduplicate posts
     args.posts=list(set(args.posts or []))
     args.username=set(args.username or [])
     args.excluded_username=set( args.excluded_username or [])
 
-    if args.command=="post_check" and not (args.url or args.file):
+    if args.command in set(["post_check","msg_check"])and not (args.url or args.file):
         raise argparse.ArgumentTypeError("error: argument missing --url or --file must be specified )")
-
+    if args.command in set(["story_check","paid_check"])and not (args.username or args.file):
+        raise argparse.ArgumentTypeError("error: argument missing --username or --file must be specified )")
     return args
 
 
 
+
 def check_strhelper(x):
     temp=None
     if isinstance(x,list):
         temp=x
     elif isinstance(x,str):
         temp=x.split(",")
     return temp
@@ -199,15 +211,15 @@
     if isinstance(x,str) and pathlib.Path(x).exists():
         with open(x,"r") as _:
            return _.readlines()
 
    
     
 def posttype_helper(x):
-    choices=set(["Highlights","All","Archived","Messages","Timeline","Pinned","Stories","Purchased","Profile","None"])
+    choices=set(["Highlights","All","Archived","Messages","Timeline","Pinned","Stories","Purchased","Profile","Skip"])
     if isinstance(x,str):
         x=x.split(',')
         x=list(map(lambda x:x.capitalize() ,x))
     if len(list(filter(lambda y: y not in choices,x)))>0:
         raise argparse.ArgumentTypeError("error: argument -o/--posts: invalid choice: (choose from 'highlights', 'all', 'archived', 'messages', 'timeline', 'pinned', 'stories', 'purchased','profile')")
     return x
```

### Comparing `ofscraper-2.5/ofscraper/utils/auth.py` & `ofscraper-2.6/ofscraper/utils/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 import hashlib
 import json
-import pathlib
 import time
+import logging
 from urllib.parse import urlparse
 import requests
 from rich.console import Console
 import httpx
 import browser_cookie3
-from .profiles import get_current_profile
+from .profiles import get_active_profile
 from ..prompts.prompts import *
 from ..constants import configPath, DYNAMIC, requestAuth
 import ofscraper.utils.paths as paths
 
-console=Console()
-
 
+console=Console()
+log=logging.getLogger(__package__)
 
 def read_auth():
     make_request_auth()
 
     authFile=paths.get_auth_file()
    
     while True:
@@ -52,26 +52,27 @@
             with open( authFile, 'w') as f:
                 f.write(manual_auth_prompt(authText))
     return auth
 
 
 def edit_auth():
     authFile=paths.get_auth_file()
+    log.info(f"Auth Path {authFile}" )
     try:
         with open(authFile, 'r') as f:
             authText=f.read()
             auth = json.loads(authText)
         print("Hint: Select 'Enter Each Field Manually' to edit your current config\n")
         make_auth(auth)
 
         console.print('Your `auth.json` file has been edited.')
     except FileNotFoundError:
         
         if ask_make_auth_prompt():
-            make_auth(auth)
+            make_auth()
     except json.JSONDecodeError as e:
             while True:
                 try:
                     print("You auth.json has a syntax error")
                     print(f"{e}\n\n")
                     with open(authFile, 'w') as f:
                         f.write(manual_auth_prompt(authText))
@@ -223,17 +224,18 @@
             'time': time2
         }
     )
     return headers
 
 
 def read_request_auth() -> dict:
-    profile = get_current_profile()
+    profile = get_active_profile()
+    
 
-    p = paths.get_config_path().parent/profile/ requestAuth
+    p = paths.get_config_home()/profile/ requestAuth
     with open(p, 'r') as f:
         content = json.load(f)
     return content
 
 
 def make_request_auth():
     request_auth = {
@@ -246,17 +248,17 @@
     # *values, = get_request_auth()
     result = get_request_auth()
     if result:
         *values, = result
 
         request_auth.update(zip(request_auth.keys(), values))
 
-        profile = get_current_profile()
+        profile = get_active_profile()
 
-        p = paths.get_config_path().parent/profile
+        p = paths.get_config_home()/profile
         if not p.is_dir():
             p.mkdir(parents=True, exist_ok=True)
 
         with open(p / requestAuth, 'w') as f:
             f.write(json.dumps(request_auth, indent=4))
```

### Comparing `ofscraper-2.5/ofscraper/utils/binaries.py` & `ofscraper-2.6/ofscraper/utils/binaries.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                     with open(pathlib.Path(zip_path),"wb") as f:
                         num_bytes_downloaded = r.num_bytes_downloaded
                         for chunk in r.iter_bytes(chunk_size=1024):
                             f.write(chunk)
                             download.update(task1, advance=r.num_bytes_downloaded - num_bytes_downloaded)
                             num_bytes_downloaded = r.num_bytes_downloaded
             download.remove_task(task1)
-        bin_path=paths_.get_config_path().parent / "bin"/"mp4decrypt.exe"
+        bin_path=paths_.get_config_home()/ "bin"/"mp4decrypt.exe"
         bin_path.parent.mkdir(exist_ok=True,parents=True)
         with ZipFile(zip_path) as zObject:
              zObject.extractall(path=t)
         shutil.move(list(pathlib.Path(t).glob("**/mp4decrypt.exe"))[0],bin_path)
         st = os.stat(bin_path)
         os.chmod(bin_path, st.st_mode | stat.S_IEXEC)
         return str(bin_path)
@@ -68,15 +68,15 @@
                     with open(pathlib.Path(zip_path),"wb") as f:
                         num_bytes_downloaded = r.num_bytes_downloaded
                         for chunk in r.iter_bytes(chunk_size=1024):
                             f.write(chunk)
                             download.update(task1, advance=r.num_bytes_downloaded - num_bytes_downloaded)
                             num_bytes_downloaded = r.num_bytes_downloaded
             download.remove_task(task1)
-        bin_path=paths_.get_config_path().parent / "bin"/"mp4decrypt"
+        bin_path=paths_.get_config_home() / "bin"/"mp4decrypt"
         bin_path.parent.mkdir(exist_ok=True,parents=True)
         with ZipFile(zip_path) as zObject:
              zObject.extractall(path=t)
         shutil.move(list(pathlib.Path(t).glob("**/mp4decrypt"))[0],bin_path)
         st = os.stat(bin_path)
         os.chmod(bin_path, st.st_mode | stat.S_IEXEC)
         return str(bin_path)
@@ -94,15 +94,15 @@
                     with open(pathlib.Path(zip_path),"wb") as f:
                         num_bytes_downloaded = r.num_bytes_downloaded
                         for chunk in r.iter_bytes(chunk_size=1024):
                             f.write(chunk)
                             download.update(task1, advance=r.num_bytes_downloaded - num_bytes_downloaded)
                             num_bytes_downloaded = r.num_bytes_downloaded
             download.remove_task(task1)
-        bin_path=paths_.get_config_path().parent / "bin"/"mp4decrypt"
+        bin_path=paths_.get_config_home() / "bin"/"mp4decrypt"
         bin_path.parent.mkdir(exist_ok=True,parents=True)
         with ZipFile(zip_path) as zObject:
              zObject.extractall(path=t)
         shutil.move(list(pathlib.Path(t).glob("**/mp4decrypt"))[0],bin_path)
         st = os.stat(bin_path)
         os.chmod(bin_path, st.st_mode | stat.S_IEXEC)
         return str(bin_path)
@@ -119,15 +119,15 @@
                     num_bytes_downloaded = r.num_bytes_downloaded
                     with open(pathlib.Path(zip_path),"wb") as f:
                         for chunk in r.iter_bytes(chunk_size=1024):
                             f.write(chunk)
                             download.update(task1, advance=r.num_bytes_downloaded - num_bytes_downloaded)
                             num_bytes_downloaded = r.num_bytes_downloaded
             download.remove_task(task1)
-        bin_path=paths_.get_config_path().parent / "bin"/"ffmpeg.exe"
+        bin_path=paths_.get_config_home()/ "bin"/"ffmpeg.exe"
         bin_path.parent.mkdir(exist_ok=True,parents=True)
         with ZipFile(zip_path) as zObject:
              zObject.extractall(path=t)
         pathlib.Path(bin_path).unlink(missing_ok=True)
         shutil.move(list(pathlib.Path(t).glob("**/ffmpeg.exe"))[0],bin_path)
         st = os.stat(bin_path)
         os.chmod(bin_path, st.st_mode | stat.S_IEXEC)
@@ -145,15 +145,15 @@
                     num_bytes_downloaded = r.num_bytes_downloaded
                     with open(pathlib.Path(zip_path),"wb") as f:
                         for chunk in r.iter_bytes(chunk_size=1024):
                             f.write(chunk)
                             download.update(task1, advance=r.num_bytes_downloaded - num_bytes_downloaded)
                             num_bytes_downloaded = r.num_bytes_downloaded
             download.remove_task(task1)
-        bin_path=paths_.get_config_path().parent / "bin"/"ffmpeg"
+        bin_path=paths_.get_config_home()/ "bin"/"ffmpeg"
         bin_path.parent.mkdir(exist_ok=True,parents=True)
         with TarFile.open(zip_path,mode="r:xz") as zObject:
              zObject.extractall(path=t)
         pathlib.Path(bin_path).unlink(missing_ok=True)
         shutil.move(list(pathlib.Path(t).glob("**/ffmpeg"))[0],bin_path)
         st = os.stat(bin_path)
         os.chmod(bin_path, st.st_mode | stat.S_IEXEC)
@@ -172,15 +172,15 @@
                     num_bytes_downloaded = r.num_bytes_downloaded
                     with open(pathlib.Path(zip_path),"wb") as f:
                         for chunk in r.iter_bytes(chunk_size=1024):
                             f.write(chunk)
                             download.update(task1, advance=r.num_bytes_downloaded - num_bytes_downloaded)
                             num_bytes_downloaded = r.num_bytes_downloaded
             download.remove_task(task1)
-        bin_path=paths_.get_config_path().parent / "bin"/"ffmpeg"
+        bin_path=paths_.get_config_home()/ "bin"/"ffmpeg"
         bin_path.parent.mkdir(exist_ok=True,parents=True)
         with ZipFile(zip_path) as zObject:
              zObject.extractall(path=t)
         pathlib.Path(bin_path).unlink(missing_ok=True)
         shutil.move(list(pathlib.Path(t).glob("**/ffmpeg"))[0],bin_path)
         st = os.stat(bin_path)
         os.chmod(bin_path, st.st_mode | stat.S_IEXEC)
```

### Comparing `ofscraper-2.5/ofscraper/utils/config.py` & `ofscraper-2.6/ofscraper/utils/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,21 +10,25 @@
 
 import json
 import pathlib
 import logging
 import ofscraper.constants as constants
 import ofscraper.prompts.prompts as prompts 
 import ofscraper.utils.binaries as binaries
-import ofscraper.utils.args as args_
 import ofscraper.utils.paths as paths_
 import ofscraper.utils.console as console_
 
 console=console_.shared_console
 log=logging.getLogger(__package__)
 
+def get_config_folder():
+    out=paths_.get_config_path().parent
+    out.mkdir(exist_ok=True,parents=True)
+    return out
+
 def read_config():
     p = pathlib.Path(paths_.get_config_path())
     if not p.parent.is_dir():
         p.parent.mkdir(parents=True, exist_ok=True)
 
     config = {}
     while True:
@@ -126,15 +130,16 @@
         f.write(json.dumps(new_config, indent=4))
 
     return new_config
 
 
 def edit_config():
     try:
-        p = paths_.get_config_path() 
+        p = paths_.get_config_path()
+        log.info(f"config path: {p}")
         with open(p, 'r') as f:
             configText=f.read()
             config = json.loads(configText)
 
         updated_config = {
             'config': prompts.config_prompt(config['config'])
         }
```

### Comparing `ofscraper-2.5/ofscraper/utils/dates.py` & `ofscraper-2.6/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.5/ofscraper/utils/download.py` & `ofscraper-2.6/ofscraper/utils/download.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from random import randint
 import platform
 import shutil
 import traceback
 import re
 import logging
 import aiohttp
-import httpx
 import contextvars
 import json
 import subprocess
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TimeElapsedColumn,
@@ -55,15 +54,15 @@
 import ofscraper.utils.logger as logger
 import ofscraper.utils.console as console
 import ofscraper.utils.stdout as stdout
 import ofscraper.utils.config as config_
 import ofscraper.utils.args as args_
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 from diskcache import Cache
-
+import ofscraper.api.me as me
 cache = Cache(paths.getcachepath())
 attempt = contextvars.ContextVar("attempt")
 log=logging.getLogger(__package__)
 
 
 async def process_dicts(username, model_id, medialist):
     with stdout.lowstdout():
@@ -73,14 +72,15 @@
         TaskProgressColumn(),TimeRemainingColumn(),TransferSpeedColumn(),DownloadColumn())
         progress_group = Group(
         overall_progress
         , Panel(Group(job_progress,fit=True)))
         # This need to be here: https://stackoverflow.com/questions/73599594/asyncio-works-in-python-3-10-but-not-in-python-3-8
         global sem
         sem = semaphoreDelayed(config_.get_threads(config_.read_config()))
+     
 
         with Live(progress_group, refresh_per_second=constants.refreshScreen,console=console.shared_console):    
                 if not args_.getargs().dupe:
                     media_ids = set(operations.get_media_ids(model_id,username))
                     medialist = seperate.separate_by_id(medialist, media_ids)
                     medialist=seperate.seperate_avatars(medialist)
                     log.info(f"Skipping previously downloaded\nMedia left for download {len(medialist)}")
@@ -93,20 +93,20 @@
                 video_count = 0
                 audio_count=0
                 skipped = 0
                 total_bytes_downloaded = 0
                 data = 0
                 desc = 'Progress: ({p_count} photos, {v_count} videos, {a_count} audios,  {skipped} skipped || {sumcount}/{mediacount}||{data})'    
 
-                
-
-                async with aiohttp.ClientSession(cookies=auth.add_cookies_aio()) as c: 
+              
+                async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=None, connect=None,
+                      sock_connect=None, sock_read=None)) as c: 
+                    i=0
                     for ele in medialist:
-                        with paths.set_directory(paths.getmediadir(ele,username,model_id)):
-                            aws.append(asyncio.create_task(download(c,ele,pathlib.Path(".").absolute() ,model_id, username,file_size_limit,job_progress)))
+                        aws.append(asyncio.create_task(download(c,ele ,model_id, username,file_size_limit,job_progress)))
                     task1 = overall_progress.add_task(desc.format(p_count=photo_count, v_count=video_count,a_count=audio_count, skipped=skipped,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped,data=data), total=len(aws),visible=True)
                     # progress_group.renderables[1].height=max(15,console.shared_console.size[1]-2)
                     for coro in asyncio.as_completed(aws):
                             try:
                                 media_type, num_bytes_downloaded = await coro
                             except Exception as e:
                                 log.traceback(e)
@@ -130,45 +130,45 @@
         overall_progress.remove_task(task1)
     log.error(f'[bold]{username}[/bold] ({photo_count} photos, {video_count} videos, {audio_count} audios,  {skipped} skipped)' )
     return photo_count+video_count+audio_count,skipped
 def retry_required(value):
     return value == ('skipped', 1)
 
 @retry(retry=retry_if_result(retry_required),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True) 
-async def download(c,ele,path,model_id,username,file_size_limit,progress):
-    attempt.set(attempt.get(0) + 1)
-    
+async def download(c,ele,model_id,username,file_size_limit,progress):
+    attempt.set(attempt.get(0) + 1)  
     try:
-        if ele.url:
-           return await main_download_helper(c,ele,path,file_size_limit,username,model_id,progress)
-        elif ele.mpd:
-            return await alt_download_helper(ele,path,file_size_limit,username,model_id,progress)
-        else:
-            return None
+            with paths.set_directory(paths.getmediadir(ele,username,model_id)):
+                if ele.url:
+                    return await main_download_helper(c,ele,pathlib.Path(".").absolute(),file_size_limit,username,model_id,progress)
+                elif ele.mpd:
+                    return await alt_download_helper(c,ele,pathlib.Path(".").absolute(),file_size_limit,username,model_id,progress)
+                else:
+                    return None
     except Exception as e:
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] exception {e}")   
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] exception {traceback.format_exc()}")   
         return 'skipped', 1
 async def main_download_helper(c,ele,path,file_size_limit,username,model_id,progress):
     url=ele.url
     path_to_file=None
     async with sem:
             log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {ele.filename_} with {url}")
             log.debug(f"Media:{ele.id} Post:{ele.postid} Downloading with normal downloader")
-            async with c.get(url) as r:
+            async with c.request("get",url,allow_redirects=True,verify_ssl=False,cookies=None) as r:
                 if r.ok:
                     rheaders=r.headers
                     total = int(rheaders['Content-Length'])
                     if file_size_limit>0 and total > int(file_size_limit): 
                             return 'skipped', 1       
                     content_type = rheaders.get("content-type").split('/')[-1]
-                    filename=createfilename(ele,username,model_id,content_type)
-                    path_to_file = paths.trunicate(pathlib.Path(path,f"{filename}"))                 
+                    filename=paths.createfilename(ele,username,model_id,content_type)
+                    path_to_file = paths.truncate(pathlib.Path(path,f"{filename}"))                 
                     pathstr=str(path_to_file)
-                    temp=paths.trunicate(f"{path_to_file}.part")
+                    temp=paths.truncate(f"{path_to_file}.part")
                     pathlib.Path(temp).unlink(missing_ok=True)
                     task1 = progress.add_task(f"{(pathstr[:constants.PATH_STR_MAX] + '....') if len(pathstr) > constants.PATH_STR_MAX else pathstr}\n", total=total,visible=True)
                     with open(temp, 'wb') as f:                           
                         progress.update(task1,visible=True )
                         async for chunk in r.content.iter_chunked(1024):
                             f.write(chunk)
                             progress.update(task1, advance=len(chunk))
@@ -193,24 +193,24 @@
             log.debug(f"Media:{ele.id} Post:{ele.postid} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}")  
 
         if ele.id:
             operations.write_media_table(ele,path_to_file,model_id,username)
         set_cache_helper(ele)
         return ele.mediatype,total
 
-async def alt_download_helper(ele,path,file_size_limit,username,model_id,progress):
+async def alt_download_helper(c,ele,path,file_size_limit,username,model_id,progress):
     async with sem:
         log.debug(f"Media:{ele.id} Post:{ele.postid} Downloading with protected media downloader")      
         log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {ele.filename_} with {ele.mpd}")
         video = None
         audio = None
         base_url=re.sub("[0-9a-z]*\.mpd$","",ele.mpd,re.IGNORECASE)
         mpd=await ele.parse_mpd
-        path_to_file = paths.trunicate(pathlib.Path(path,f'{createfilename(ele,username,model_id,"mp4")}'))
-        temp_path=paths.trunicate(pathlib.Path(path,f"temp_{ele.id or ele.filename_}_{randint(100,999)}.mp4"))
+        path_to_file = paths.truncate(pathlib.Path(path,f'{paths.createfilename(ele,username,model_id,"mp4")}'))
+        temp_path=paths.truncate(pathlib.Path(path,f"temp_{ele.id or ele.filename_}_{randint(100,999)}.mp4"))
         for period in mpd.periods:
             for adapt_set in filter(lambda x:x.mime_type=="video/mp4",period.adaptation_sets):             
                 kId=None
                 for prot in adapt_set.content_protections:
                     if prot.value==None:
                         kId = prot.pssh[0].pssh 
                         break
@@ -232,47 +232,46 @@
                     name=f"{repr.base_urls[0].base_url_value}_{randint(100,999)}"
                     audio={"origname":repr.base_urls[0].base_url_value,"pssh":kId,"type":"audio","name":name}
                     break
             for item in [audio,video]:
                 url=f"{base_url}{item['origname']}"
                 log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {item['origname']} with {url}")
                 params={"Policy":ele.policy,"Key-Pair-Id":ele.keypair,"Signature":ele.signature}   
-                async with aiohttp.ClientSession(cookies=auth.add_cookies_aio(),headers=auth.make_headers(auth.read_auth())) as c: 
-                    async with c.get(url,params=params) as r:
-                        if r.ok:
-                            rheaders=r.headers
-                            total = int(rheaders['Content-Length'])
-                            item["total"]=total
-                            if file_size_limit>0 and total > int(file_size_limit): 
-                                    return 'skipped', 1       
-                            temp= paths.trunicate(pathlib.Path(path,f"{item['name']}.part"))
-                            temp.unlink(missing_ok=True)
-                            item["path"]=temp
-                            pathstr=str(temp)
-                            task1 = progress.add_task(f"{(pathstr[:constants.PATH_STR_MAX] + '....') if len(pathstr) > constants.PATH_STR_MAX else pathstr}\n", total=total,visible=True)
-                            with open(temp, 'wb') as f:                           
-                                progress.update(task1,visible=True )
-                                async for chunk in r.content.iter_chunked(1024):
-                                    f.write(chunk)
-                                    progress.update(task1, advance=len(chunk))
-                                progress.remove_task(task1) 
-                        else:
-                            r.raise_for_status()
+                async with c.request("get",url,params=params,allow_redirects=True,verify_ssl=False,cookies=auth.add_cookies_aio(),headers=auth.make_headers(auth.read_auth())) as r:
+                    if r.ok:
+                        rheaders=r.headers
+                        total = int(rheaders['Content-Length'])
+                        item["total"]=total
+                        if file_size_limit>0 and total > int(file_size_limit): 
+                                return 'skipped', 1       
+                        temp= paths.truncate(pathlib.Path(path,f"{item['name']}.part"))
+                        temp.unlink(missing_ok=True)
+                        item["path"]=temp
+                        pathstr=str(temp)
+                        task1 = progress.add_task(f"{(pathstr[:constants.PATH_STR_MAX] + '....') if len(pathstr) > constants.PATH_STR_MAX else pathstr}\n", total=total,visible=True)
+                        with open(temp, 'wb') as f:                           
+                            progress.update(task1,visible=True )
+                            async for chunk in r.content.iter_chunked(1024):
+                                f.write(chunk)
+                                progress.update(task1, advance=len(chunk))
+                            progress.remove_task(task1) 
+                    else:
+                        r.raise_for_status()
     log.debug(f"Media:{ele.id} Post:{ele.postid} video name:{video['name']}")
     log.debug(f"Media:{ele.id} Post:{ele.postid} audio name:{audio['name']}")
     for item in [audio,video]:
         if not pathlib.Path(item["path"]).exists():
                 log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {item['path']} was not created") 
                 return "skipped",1
         elif abs(item["total"]-pathlib.Path(item['path']).absolute().stat().st_size)>500:
             log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {item['name']} size mixmatch target: {total} vs actual: {pathlib.Path(item['path']).absolute().stat().st_size}")   
             return "skipped",1 
                 
     for item in [audio,video]:
-        key=await key_helper(item["pssh"],ele.license,ele.id)
+        key=await key_helper(c,item["pssh"],ele.license,ele.id)
         if key==None:
             log.debug(f"Media:{ele.id} Post:{ele.postid} Could not get key")
             return "skipped",1 
         log.debug(f"Media:{ele.id} Post:{ele.postid} got key")
         newpath=pathlib.Path(re.sub("\.part$","",str(item["path"]),re.IGNORECASE))
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] renaming {pathlib.Path(item['path']).absolute()} -> {newpath}")   
         r=subprocess.run([config_.get_mp4decrypt(config_.read_config()),"--key",key,str(item["path"]),str(newpath)],stdout=subprocess.PIPE,stderr=subprocess.PIPE)
@@ -303,37 +302,38 @@
         set_time(path_to_file,newDate )
         log.debug(f"Media:{ele.id} Post:{ele.postid} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}")  
     if ele.id:
         operations.write_media_table(ele,path_to_file,model_id,username)
     set_cache_helper(ele)
     return ele.mediatype,total
 
-async def key_helper(pssh,licence_url,id):
+async def key_helper(c,pssh,licence_url,id):
     out=cache.get(licence_url)
     log.debug(f"ID:{id} pssh: {pssh!=None}")
     log.debug(f"ID:{id} licence: {licence_url}")
     if not out:
         headers=auth.make_headers(auth.read_auth())
         headers["cookie"]=auth.get_cookies()
         auth.create_sign(licence_url,headers)
         json_data = {
-            'license': str(httpx.URL(licence_url)),
+            'license': licence_url,
             'headers': json.dumps(headers),
             'pssh': pssh,
             'buildInfo': '',
             'proxy': '',
             'cache': True,
         }
 
 
-        
-        async with httpx.AsyncClient(http2=True, follow_redirects=True, timeout=None) as c: 
-            r=await c.post('https://cdrm-project.com/wv',json=json_data)
-            log.debug(f"ID:{id} key_response: {r.content.decode()}")
-            soup = BeautifulSoup(r.content, 'html.parser')
+                 
+
+        async with c.request("post",'https://cdrm-project.com/wv',json=json_data,verify_ssl=False,allow_redirects=True,cookies=None) as r:
+            httpcontent=await r.text()
+            log.debug(f"ID:{id} key_response: {httpcontent}")
+            soup = BeautifulSoup(httpcontent, 'html.parser')
             out=soup.find("li").contents[0]
             cache.set(licence_url,out, expire=2592000)
             cache.close()
     return out
         
 
 
@@ -356,36 +356,15 @@
 
 def get_error_message(content):
     error_content = content.get('error', 'No error message available')
     try:
         return error_content.get('message', 'No error message available')
     except AttributeError:
         return error_content
-def createfilename(ele,username,model_id,ext):
-    filename=ele.filename_
-    sitename="Onlyfans"
-    site_name="Onlyfans"
-    post_id=ele.postid_
-    media_id=ele.id
-    first_letter=username[0]
-    mediatype=ele.mediatype
-    value=ele.value
-    text=ele.text_
-    date=arrow.get(ele.postdate).format(config_.get_date(config_.read_config()))
-    model_username=username
-    responsetype=ele.responsetype
-
-    if ele.responsetype_ =="profile":
-        return f"{filename}.{ext}"
-    elif config_.get_allow_code_execution(config_.read_config()):
-        return eval("f'{}'".format(config_.get_fileformat(config_.read_config())))
-    else:
-        return config_.get_fileformat(config_.read_config()).format(filename=filename,sitename=sitename,site_name=sitename,post_id=post_id,media_id=media_id,first_letter=first_letter,mediatype=mediatype,value=value,text=text,date=date,ext=ext,model_username=username,model_id=model_id,responsetype=responsetype) 
 
-    
 
 def set_cache_helper(ele):
     if  ele.postid and ele.responsetype_=="profile":
         cache.set(ele.postid ,True)
         cache.close()
     elif  ele.filename_ and ele.responsetype_=="highlights":
         cache.set(ele.filename_,True)
```

### Comparing `ofscraper-2.5/ofscraper/utils/encoding.py` & `ofscraper-2.6/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.5/ofscraper/utils/exit.py` & `ofscraper-2.6/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.5/ofscraper/utils/filters.py` & `ofscraper-2.6/ofscraper/utils/filters.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 def filterMedia(media):
     media=dupefilter(media)
     media=post_datesorter(media)
     media=posts_type_filter(media)
     media=posts_date_filter(media)
     media=post_timed_filter(media)
     media=post_user_filter(media)
+    media=download_type_filter(media)
     media=sort_media(media)
     return media
 
 def sort_media(media):
     return sorted(media,key=lambda x:x.date)
 
 def post_manual_filter():
@@ -80,8 +81,16 @@
         return list(filter(lambda x:not x.expires,media))
     return media
 def post_user_filter(media):
     userfilter=args.filter
     if not userfilter.islower():
         return list(filter(lambda x:re.search(userfilter,x.text or "")!=None,media))
     else:
-        return list(filter(lambda x:re.search(userfilter,x.text or "",re.IGNORECASE)!=None,media))
+        return list(filter(lambda x:re.search(userfilter,x.text or "",re.IGNORECASE)!=None,media))
+
+def download_type_filter(media):
+    if args_.getargs().download_type==None:
+        return media
+    elif args_.getargs().download_type=="protected":
+        return list(filter(lambda x:x.mpd!=None,media))  
+    elif args_.getargs().download_type=="normal":
+        return list(filter(lambda x:x.url!=None,media))
```

### Comparing `ofscraper-2.5/ofscraper/utils/logger.py` & `ofscraper-2.6/ofscraper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.5/ofscraper/utils/of.py` & `ofscraper-2.6/ofscraper/utils/of.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,28 +17,27 @@
 import ofscraper.db.operations as operations
 import ofscraper.api.posts as posts_
 import ofscraper.utils.args as args_
 import ofscraper.api.paid as paid
 import ofscraper.api.highlights as highlights
 import ofscraper.api.timeline as timeline
 import ofscraper.api.profile as profile
-import ofscraper.utils.auth as auth
 import ofscraper.utils.args as args_
 import ofscraper.utils.filters as filters
 import ofscraper.utils.stdout as stdout
 import ofscraper.api.archive as archive
 import ofscraper.api.pinned as pinned
 
 log=logging.getLogger(__package__)
 args=args_.getargs()
 log.debug(args)
 
-def process_messages(headers, model_id,username):
+def process_messages(model_id,username):
     with stdout.lowstdout():
-        messages_ =asyncio.run(messages.get_messages(headers,  model_id)) 
+        messages_ =asyncio.run(messages.get_messages(  model_id)) 
         messages_=list(map(lambda x:posts_.Post(x,model_id,username),messages_))
         log.debug(f"[bold]Messages Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),messages_))}")
         log.debug("Removing locked messages media")
         for message in messages_:
             operations.write_messages_table(message)
         output=[]
         [ output.extend(message.media) for message in messages_]
@@ -54,17 +53,17 @@
             operations.write_post_table(post,model_id,username)
         output=[]
         [output.extend(post.media) for post in paid_content]
         return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
          
 
-def process_highlights(headers, model_id,username):
+def process_highlights( model_id,username):
     with stdout.lowstdout():
-        highlights_, stories = asyncio.run(highlights.get_highlight_post(headers, model_id))
+        highlights_, stories = asyncio.run(highlights.get_highlight_post( model_id))
         highlights_, stories=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="highlights"),highlights_)),\
         list(map(lambda x:posts_.Post(x,model_id,username,responsetype="stories"),stories))
         log.debug(f"[bold]Combined Story and Highlight Media count[/bold] {sum(map(lambda x:len(x.post_media), highlights_))+sum(map(lambda x:len(x.post_media), stories))}")
         for post in highlights_:
             operations.write_stories_table(post,model_id,username)
         for post in stories:
             operations.write_stories_table(post,model_id,username)   
@@ -77,57 +76,57 @@
         
 
 
 
 
 
 
-def process_timeline_posts(headers, model_id,username):
+def process_timeline_posts(model_id,username):
     with stdout.lowstdout():
-        timeline_posts = asyncio.run(timeline.get_timeline_post(headers, model_id))
+        timeline_posts = asyncio.run(timeline.get_timeline_post( model_id))
         timeline_posts  =list(map(lambda x:posts_.Post(x,model_id,username,"timeline"), timeline_posts ))
         log.debug(f"[bold]Timeline Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),timeline_posts))}")
         log.debug("Removing locked timeline media")
         for post in timeline_posts:
             operations.write_post_table(post,model_id,username)
         output=[]
         [output.extend(post.media) for post in  timeline_posts ]
         return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
-def process_archived_posts(headers, model_id,username):
+def process_archived_posts( model_id,username):
     with stdout.lowstdout():
-        archived_posts = asyncio.run(archive.get_archived_post(headers, model_id))
+        archived_posts = asyncio.run(archive.get_archived_post(model_id))
         archived_posts =list(map(lambda x:posts_.Post(x,model_id,username),archived_posts ))
         log.debug(f"[bold]Archived Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),archived_posts))}")
         log.debug("Removing locked archived media")
 
         for post in archived_posts:
             operations.write_post_table(post,model_id,username)
         output=[]
         [ output.extend(post.media) for post in archived_posts ]
         return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
 
 
 
-def process_pinned_posts(headers, model_id,username):
+def process_pinned_posts( model_id,username):
     with stdout.lowstdout():
-        pinned_posts = asyncio.run(pinned.get_pinned_post(headers, model_id))
+        pinned_posts = asyncio.run(pinned.get_pinned_post( model_id))
         pinned_posts =list(map(lambda x:posts_.Post(x,model_id,username,"pinned"),pinned_posts ))
         log.debug(f"[bold]Pinned Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),pinned_posts))}")
         log.debug("Removing locked pinned media")
         for post in  pinned_posts:
             operations.write_post_table(post,model_id,username)
         output=[]
         [ output.extend(post.media) for post in pinned_posts ]
         return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
-def process_profile(headers, username) -> list:
+def process_profile( username) -> list:
     with stdout.lowstdout():
-        user_profile = profile.scrape_profile(headers, username)
+        user_profile = profile.scrape_profile( username)
         urls, info = profile.parse_profile(user_profile)
         profile.print_profile_info(info)       
         output=[]
         for ele in enumerate(urls):
             count=ele[0]
             data=ele[1]
             output.append(posts_.Media({"url":data["url"],"type":data["mediatype"]},count,posts_.Post(data,info[2],username,responsetype="profile")))
@@ -137,19 +136,18 @@
         return output
 
 def process_all_paid():
     with stdout.lowstdout():
         paid_content=asyncio.run(paid.get_all_paid_posts())
         user_dict={}
         post_array=[]
-        headers = auth.make_headers(auth.read_auth())
         [user_dict.update({(ele.get("fromUser",None) or ele.get("author",None) or {} ).get("id"):user_dict.get((ele.get("fromUser",None) or ele.get("author",None) or {} ).get("id"),[])+[ele]}) for ele in paid_content]
 
         for model_id,value in user_dict.items():
-            username=profile.scrape_profile(headers,model_id).get("username")
+            username=profile.scrape_profile(model_id).get("username")
             if username=="modeldeleted":
                 username=operations.get_profile_info(model_id,username) or username
             log.info(f"Processing {username}_{model_id}")
             operations.create_tables(model_id,username)
             log.debug(f"Created table for {username}")
             new_posts=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="paid"),value))
             post_array.extend(new_posts)
@@ -167,45 +165,45 @@
     if not args.scrape_paid and len( args.posts or [])==0:
           args.scrape_paid=prompts.scrape_paid_prompt()
     args.posts = list(map(lambda x:x.capitalize(),(args.posts or prompts.areas_prompt())
 ))
 
     args_.changeargs(args)
      
-def process_areas(headers, ele, model_id) -> list:
+def process_areas(ele, model_id) -> list:
     select_areas()
     timeline_posts_dicts  = []
     pinned_post_dict=[]
     archived_posts_dicts  = []
     highlights_dicts  = []
     messages_dicts  = []
     stories_dicts=[]
     purchased_dict=[]
     pinned_post_dict=[]
     profile_dicts=[]
 
 
     username=ele['name']
-    if "NONE" in args.posts:
+    if "Skip" in args.posts:
         return []
   
     if ('Profile' in args.posts or 'All' in args.posts):
-        profile_dicts  = process_profile(headers,username)
+        profile_dicts  = process_profile(username)
     if ('Pinned' in args.posts or 'All' in args.posts):
-            pinned_post_dict = process_pinned_posts(headers, model_id,username)
+            pinned_post_dict = process_pinned_posts(model_id,username)
     if ('Timeline' in args.posts or 'All' in args.posts):
-            timeline_posts_dicts = process_timeline_posts(headers, model_id,username)
+            timeline_posts_dicts = process_timeline_posts( model_id,username)
     if ('Archived' in args.posts or 'All' in args.posts):
-            archived_posts_dicts = process_archived_posts(headers, model_id,username)
+            archived_posts_dicts = process_archived_posts( model_id,username)
     if 'Messages' in args.posts or 'All' in args.posts:
-            messages_dicts = process_messages(headers, model_id,username)
+            messages_dicts = process_messages( model_id,username)
     if "Purchased" in args.posts or "All" in args.posts:
             purchased_dict=process_paid_post(model_id,username)
     if ('Highlights'  in args.posts or 'Stories'  in args.posts or 'All' in args.posts):
-            highlights_tuple = process_highlights(headers, model_id,username)  
+            highlights_tuple = process_highlights( model_id,username)  
             if 'Highlights'  in args.posts:
                 highlights_dicts=highlights_tuple[0]
             if 'Stories'  in args.posts:
                 stories_dicts=highlights_tuple[1]   
             if 'All' in args.posts:
                 highlights_dicts=highlights_tuple[0]
                 stories_dicts=highlights_tuple[1]
```

### Comparing `ofscraper-2.5/ofscraper/utils/paths.py` & `ofscraper-2.6/ofscraper/utils/paths.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,22 +11,26 @@
 import arrow
 from InquirerPy.utils import patched_print
 import ofscraper.constants as constants
 import ofscraper.utils.profiles as profiles
 import ofscraper.utils.config as config_
 import ofscraper.utils.args as args_
 import ofscraper.utils.console as console_
-from .profiles import get_current_profile
+from .profiles import get_current_config_profile
+import ofscraper.api.me as me
+
 
 
 console=console_.shared_console
 homeDir=pathlib.Path.home()
 log=logging.getLogger(__package__)
 
 
+
+
 @contextmanager
 def set_directory(path: Path):
     """Sets the cwd within the context
 
         Args:``
             path (``Path): The path to the cwd
 
@@ -45,37 +49,41 @@
 def createDir(path):
     try:
         path.mkdir(exist_ok=True,parents=True)
     except:
         log.info("Error creating directory, check the directory and make sure correct permissions have been issued.")
         sys.exit()
 def databasePathHelper(model_id,username):
-    configpath= get_config_path().parent
-    profile=profiles.get_current_profile()
+    configpath= get_config_home()
+    profile=profiles.get_active_profile()
     model_username=username
     username=username
     modelusername=username
-    modelusername=username
     model_id=model_id
     sitename="Onlyfans"
     site_name="Onlyfans"
     first_letter=username[0]
+
     save_location=config_.get_save_location(config_.read_config())
+    my_profile = profiles.get_my_info()
+    my_id, my_username =me.parse_user(my_profile)
     if config_.get_allow_code_execution(config_.read_config()):
         formatStr=eval("f'{}'".format(config_.get_metadata(config_.read_config())))
     else:
         formatStr=config_.get_metadata(config_.read_config()).format(
                          profile=profile,
                          model_username=username,
                          username=username,
                          model_id=model_id,
                          sitename=site_name,
                          site_name=site_name,
                          first_letter=first_letter,
-                         save_location=save_location,
+                        save_location=save_location,
+                                        my_id=my_id, 
+                        my_username=my_username,
                          configpath=configpath)
 
 
     formatStr
     return pathlib.Path(formatStr,"user_data.db")
 
 def getmediadir(ele,username,model_id):
@@ -86,14 +94,17 @@
     first_letter=username[0].capitalize()
     mediatype=ele.mediatype.capitalize()
     value=ele.value.capitalize()
     date=arrow.get(ele.postdate).format(config_.get_date(config_.read_config()))
     model_username=username
     responsetype=ele.responsetype
     root= pathlib.Path((config_.get_save_location(config_.read_config())))
+    profile=profiles.get_active_profile()
+    my_profile = profiles.get_my_info()
+    my_id, my_username =me.parse_user(my_profile)
     if config_.get_allow_code_execution(config_.read_config()):
         downloadDir=eval("f'{}'".format(config_.get_dirformat(config_.read_config())))
     else:
         downloadDir=config_.get_dirformat(config_.read_config())\
         .format(post_id=post_id,
                 sitename=site_name,
                 site_name=site_name,
@@ -101,46 +112,95 @@
                 modeluesrname=model_username,
                 first_letter=first_letter,
                 model_id=model_id,
                 model_username=username,
                 responsetype=responsetype,
                 mediatype=mediatype,
                 date=date,
+                      my_id=my_id, 
+                        my_username=my_username,
+                profile=profile,
                 value=value)
         
     return root /downloadDir  
 
 
 
+def createfilename(ele,username,model_id,ext):
+    filename=ele.filename_
+    sitename="Onlyfans"
+    site_name="Onlyfans"
+    user=me
+    post_id=ele.postid_
+    media_id=ele.id
+    first_letter=username[0]
+    mediatype=ele.mediatype
+    value=ele.value
+    text=ele.text_
+    date=arrow.get(ele.postdate).format(config_.get_date(config_.read_config()))
+    model_username=username
+    responsetype=ele.responsetype
+    profile=profiles.get_active_profile()
+    my_profile = profiles.get_my_info()
+    my_id, my_username =me.parse_user(my_profile)
+   
+
+    if ele.responsetype_ =="profile":
+        return f"{filename}.{ext}"
+    elif config_.get_allow_code_execution(config_.read_config()):
+        return eval("f'{}'".format(config_.get_fileformat(config_.read_config())))
+    else:
+        return config_.get_fileformat(config_.read_config()).format(filename=filename,
+                                                                    sitename=sitename,
+                                                                    site_name=sitename,post_id=post_id,
+                                                                    media_id=media_id,
+                                                                    first_letter=first_letter,
+                                                                    mediatype=mediatype,
+                                                                    value=value,
+                                                                    text=text,
+                                                                    date=date,
+                                                                    ext=ext,
+                                                                    model_username=username,
+                                                                    model_id=model_id,
+                                                                    responsetype=responsetype,
+                                                                          my_id=my_id, 
+                                                                my_username=my_username,
+                                                                    profile=profile) 
+
+
 
 
 
 
 def cleanup():
     log.info("Cleaning up temp files\n\n")
     root= pathlib.Path((config_.get_save_location(config_.read_config())))
     for file in list(filter(lambda x:re.search("\.part$|^temp_",str(x))!=None,root.glob("**/*"))):
         file.unlink(missing_ok=True)
 
 
 def getcachepath():
-    profile = profiles.get_current_profile()
-    path= get_config_path().parent/ profile/"cache"
+    profile = get_profile_path()
+    path= profile/"cache"
     createDir(path.parent)
     return path
-def trunicate(path):
+def truncate(path):
     if args_.getargs().original:
         return path
-    if platform.system() == 'Windows' and len(str(path))>256:
-        return _windows_trunicateHelper(path)
+    if platform.system() == 'Windows':
+        return _windows_truncateHelper(path)
     elif platform.system() == 'Linux':
-        return _linux_trunicateHelper(path)
+        return _linux_truncateHelper(path)
+    elif platform.system() == 'Darwin':
+        return _mac_truncateHelper(path)
     else:
         return pathlib.Path(path)
-def _windows_trunicateHelper(path):
+def _windows_truncateHelper(path):
+    if len(str(path))<=256:
+        return path
     path=pathlib.Path(path)
     dir=path.parent
     file=path.name
     match=re.search("_[0-9]+\.[a-z]*$",path.name,re.IGNORECASE) or re.search("\.[a-z]*$",path.name,re.IGNORECASE)
     if match:
         ext=match.group(0)
     else:
@@ -148,15 +208,28 @@
     #-1 is for / between parentdirs and file
     fileLength=256-len(ext)-len(str(dir))-1
     newFile=f"{re.sub(ext,'',file)[fileLength]}{ext}"
     final=pathlib.Path(dir,newFile)
     log.debug(f"path: {final} path size: {len(str(final))}")
     return pathlib.Path(dir,newFile)
 
-def _linux_trunicateHelper(path):
+def _mac_truncateHelper(path):
+    path=pathlib.Path(path)
+    dir=path.parent
+    match=re.search("_[0-9]+\.[a-z]*$",path.name,re.IGNORECASE) or re.search("\.[a-z]*$",path.name,re.IGNORECASE)
+    ext= match.group(0) if match else ""
+    file=re.sub(ext,"",path.name)
+    maxlength=255-len(ext)
+    newFile=f"{file[:maxlength]}{ext}"
+    final=pathlib.Path(dir,newFile)
+    log.debug(f"path: {final} path size: {len(str(final))}")
+    log.debug(f"path: {final} filename size: {len(str(final.name))}")
+    return pathlib.Path(dir,newFile)
+
+def _linux_truncateHelper(path):
     path=pathlib.Path(path)
     dir=path.parent
     match=re.search("_[0-9]+\.[a-z]*$",path.name,re.IGNORECASE) or re.search("\.[a-z]*$",path.name,re.IGNORECASE)
     ext= match.group(0) if match else ""
     file=re.sub(ext,"",path.name)
     maxbytes=254-len(ext.encode('utf8'))
     small=0
@@ -222,28 +295,48 @@
         patched_print("issue executing path as ffmpeg")
     except Exception as E:
         patched_print(E)
         patched_print(traceback.format_exc())
         return False  
    
 def getlogpath():
-    path= get_config_path().parent / "logging"/f'ofscraper_{config_.get_main_profile()}_{arrow.now().format("YYYY-MM-DD")}.log'
+    path= get_config_home() / "logging"/f'ofscraper_{config_.get_main_profile()}_{arrow.now().format("YYYY-MM-DD")}.log'
     createDir(path.parent)
     return path
 
 def get_config_path():
-    t=pathlib.Path(args_.getargs().config or pathlib.Path.home() / constants.configPath)        
-    if t.is_file():
-         return t
-    elif t.parent.is_dir():
-        t/constants.configFile
-    return t/constants.configFile
+    configPath=args_.getargs().config
+    defaultPath=pathlib.Path.home() / constants.configPath/constants.configFile
+    ofscraperHome=pathlib.Path.home() / constants.configPath
+
+    if configPath==None or configPath=="":
+        return defaultPath
+    configPath=pathlib.Path(configPath)
+    # check if path exists
+    if  configPath.is_file():
+         return configPath
+    elif configPath.is_dir():
+        return configPath/constants.configFile
+    #enforce that configpath needs some extension
+    elif configPath.suffix=="":
+        return configPath/constants.configFile
+    
+    elif str(configPath.parent)==".":
+        return ofscraperHome/configPath
+    return configPath
+
+def get_profile_path(name=None):
+    if name:
+        return get_config_home()/name
+    elif not args_.getargs().profile:
+        return get_config_home()/get_current_config_profile()
+    return get_config_home()/args_.getargs().profile
+
+def get_config_home():
+    return get_config_path().parent
+
 
 def get_auth_file():
-    profile = get_current_profile()
-    auth= get_config_path().parent/profile /constants.authFile if not args_.getargs().auth else args_.getargs().auth
-    if auth.is_dir():
-        raise Exception("Auth File must be a file")
-    return auth
+    return get_profile_path() /constants.authFile
```

### Comparing `ofscraper-2.5/ofscraper/utils/separate.py` & `ofscraper-2.6/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.5/ofscraper/utils/stdout.py` & `ofscraper-2.6/ofscraper/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.5/ofscraper/utils/table.py` & `ofscraper-2.6/ofscraper/utils/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,15 +168,14 @@
                 if text != ".":
                     int(text)
             except ValueError:
                 pass
             else:
                 super().insert_text_at_cursor(text)
 
-
 class TimeField(Horizontal):
     def __init__(self, name: str) -> None:
         super().__init__(id=name)
         self.filter_name = name
         self.timeconversions = [60*60, 60, 1]
 
     def compose(self):
@@ -441,14 +440,25 @@
         added= self.get_current_added_rows()
         self.sort_helper(event.label.plain)
         self.restore_added_rows(added)
       
         # set reverse
         # use native python sorting until textual has key support
 
+    def on_data_table_cell_selected(self, event):
+        table = self.query_one(DataTable) 
+        cursor_coordinate = table.cursor_coordinate
+        if cursor_coordinate[1]==self.row_names.index("Download_Cart"):
+            self.change_download_cart(event.coordinate)
+        
+
+      
+        # set reverse
+        # use native python sorting until textual has key support
+
 
 
    
     def on_button_pressed(self, event: Button.Pressed) -> None:
         if event.button.id == "submit":
             added=self.get_current_added_rows()
             self.set_filtered_rows()
@@ -561,15 +571,15 @@
 
     def add_to_row_queue(self):
         table=self.query_one(DataTable)
         keys=[str(ele[0]) for ele in self._filtered_rows]
         index=self.row_names.index("Download_Cart")
         filter_keys=list(filter(lambda x:table.get_row(x)[index].plain=="[added]",keys))
         self.update_downloadcart_cell(filter_keys,"[downloading]")
-        log.info(f"Number of Downloads Set to queue {len(filter_keys)}")
+        log.info(f"Number of Downloads sent to queue {len(filter_keys)}")
         [self.row_queue.put(ele) for ele in map(lambda x:(table.get_row(x),x),filter_keys)]
     def get_current_added_rows(self):
         table=self.query_one(DataTable)
         keys=[str(ele[0]) for ele in self._filtered_rows]
         index=self.row_names.index("Download_Cart")
         filter_keys=list(filter(lambda x:table.get_row(x)[index].plain=="[added]",keys))
         return filter_keys
```

### Comparing `ofscraper-2.5/ofscraper/utils/userselector.py` & `ofscraper-2.6/ofscraper/utils/userselector.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def getselected_usernames():
     #username list will be retrived once per daemon run
     # manual prompt will need to recertify options every call
     global selectedusers
     scraper_bool=len(args.posts)>0 or args.action
     #always return with correct args
-    if "None" in args.posts:
+    if "Skip" in args.posts:
         return []
     if selectedusers and scraper_bool:
             return selectedusers
     if scraper_bool:
         selectedusers=selectuserhelper()
     #create in these situations
     #set at least once
```

### Comparing `ofscraper-2.5/pyproject.toml` & `ofscraper-2.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "2.5"
+version = "2.6"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
 httpx = {extras = ["http2"], version = "^0.23.3"}
@@ -42,14 +42,21 @@
 pytest-check = { version = "2.1.4", python = ">3.7" }
 coverage = "^7.2.3"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 random-unicode-emoji = "^2.8"
 random-emoji = "^1.0.15"
 
+
+
+
+
+[tool.poetry.group.docs.dependencies]
+sphinx-argparse = "^0.4.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry.scripts]
 ofscraper = "ofscraper.start:main"
```

