# Comparing `tmp/pidgeotto-0.0.4.tar.gz` & `tmp/pidgeotto-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pidgeotto-0.0.4.tar", last modified: Sat May  8 10:22:00 2021, max compression
+gzip compressed data, was "pidgeotto-0.0.5.tar", last modified: Sun Jun 25 14:28:41 2023, max compression
```

## Comparing `pidgeotto-0.0.4.tar` & `pidgeotto-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nihar     (1000) users      (985)        0 2021-05-08 10:22:00.670044 pidgeotto-0.0.4/
--rw-r--r--   0 nihar     (1000) users      (985)     1073 2021-04-24 02:02:55.000000 pidgeotto-0.0.4/LICENSE
--rw-r--r--   0 nihar     (1000) users      (985)     4008 2021-05-08 10:22:00.670044 pidgeotto-0.0.4/PKG-INFO
--rwxr-xr-x   0 nihar     (1000) users      (985)     2609 2021-05-08 10:11:16.000000 pidgeotto-0.0.4/README.md
-drwxr-xr-x   0 nihar     (1000) users      (985)        0 2021-05-08 10:22:00.660044 pidgeotto-0.0.4/pidgeotto.egg-info/
--rw-r--r--   0 nihar     (1000) users      (985)     4008 2021-05-08 10:22:00.000000 pidgeotto-0.0.4/pidgeotto.egg-info/PKG-INFO
--rw-r--r--   0 nihar     (1000) users      (985)      315 2021-05-08 10:22:00.000000 pidgeotto-0.0.4/pidgeotto.egg-info/SOURCES.txt
--rw-r--r--   0 nihar     (1000) users      (985)        1 2021-05-08 10:22:00.000000 pidgeotto-0.0.4/pidgeotto.egg-info/dependency_links.txt
--rw-r--r--   0 nihar     (1000) users      (985)       47 2021-05-08 10:22:00.000000 pidgeotto-0.0.4/pidgeotto.egg-info/entry_points.txt
--rw-r--r--   0 nihar     (1000) users      (985)       24 2021-05-08 10:22:00.000000 pidgeotto-0.0.4/pidgeotto.egg-info/requires.txt
--rw-r--r--   0 nihar     (1000) users      (985)        7 2021-05-08 10:22:00.000000 pidgeotto-0.0.4/pidgeotto.egg-info/top_level.txt
-drwxr-xr-x   0 nihar     (1000) users      (985)        0 2021-05-08 10:22:00.660044 pidgeotto-0.0.4/pidgey/
--rwxr-xr-x   0 nihar     (1000) users      (985)       20 2021-05-08 09:05:07.000000 pidgeotto-0.0.4/pidgey/__init__.py
--rwxr-xr-x   0 nihar     (1000) users      (985)     5083 2021-05-08 09:54:21.000000 pidgeotto-0.0.4/pidgey/builder.py
--rwxr-xr-x   0 nihar     (1000) users      (985)     9170 2021-05-08 09:50:29.000000 pidgeotto-0.0.4/pidgey/creator.py
--rwxr-xr-x   0 nihar     (1000) users      (985)     2071 2021-05-08 09:35:52.000000 pidgeotto-0.0.4/pidgey/pidgey.py
--rwxr-xr-x   0 nihar     (1000) users      (985)     1699 2021-05-08 09:54:18.000000 pidgeotto-0.0.4/pidgey/server.py
--rw-r--r--   0 nihar     (1000) users      (985)       38 2021-05-08 10:22:00.670044 pidgeotto-0.0.4/setup.cfg
--rw-r--r--   0 nihar     (1000) users      (985)     1130 2021-05-08 09:29:58.000000 pidgeotto-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 14:28:41.846704 pidgeotto-0.0.5/
+-rw-rw-rw-   0        0        0     1094 2023-06-25 12:13:36.000000 pidgeotto-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3612 2023-06-25 14:28:41.845704 pidgeotto-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2766 2023-06-25 14:28:12.000000 pidgeotto-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 14:28:41.821719 pidgeotto-0.0.5/pidgeotto.egg-info/
+-rw-rw-rw-   0        0        0     3612 2023-06-25 14:28:41.000000 pidgeotto-0.0.5/pidgeotto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-06-25 14:28:41.000000 pidgeotto-0.0.5/pidgeotto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 14:28:41.000000 pidgeotto-0.0.5/pidgeotto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-25 14:28:41.000000 pidgeotto-0.0.5/pidgeotto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2023-06-25 14:28:41.000000 pidgeotto-0.0.5/pidgeotto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-25 14:28:41.000000 pidgeotto-0.0.5/pidgeotto.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 14:28:41.844700 pidgeotto-0.0.5/pidgey/
+-rw-rw-rw-   0        0        0       21 2023-06-25 12:13:36.000000 pidgeotto-0.0.5/pidgey/__init__.py
+-rw-rw-rw-   0        0        0     5354 2023-06-25 14:25:30.000000 pidgeotto-0.0.5/pidgey/builder.py
+-rw-rw-rw-   0        0        0     9028 2023-06-25 14:26:03.000000 pidgeotto-0.0.5/pidgey/creator.py
+-rw-rw-rw-   0        0        0     2104 2023-06-25 14:26:19.000000 pidgeotto-0.0.5/pidgey/pidgey.py
+-rw-rw-rw-   0        0        0     1731 2023-06-25 14:26:34.000000 pidgeotto-0.0.5/pidgey/server.py
+-rw-rw-rw-   0        0        0       42 2023-06-25 14:28:41.846704 pidgeotto-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1165 2023-06-25 12:13:36.000000 pidgeotto-0.0.5/setup.py
```

### Comparing `pidgeotto-0.0.4/LICENSE` & `pidgeotto-0.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Nihar Samantaray
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 Nihar Samantaray
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pidgeotto-0.0.4/README.md` & `pidgeotto-0.0.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,99 +1,107 @@
-# pidgeotto
-
-## Description
-Yet another static website generator. 
-
-Why choose pidgeotto?
-1. Free of javascript.
-2. Extensible, flexible, forkable.
-3. Minimal and fast.
-4. Free under MIT License.
-
-## Installation
-``` pip install pidgeotto ```
-
-$ pip install git+https://github.com/niharokz/pidgeotto
-
-## Prerequisites
-By default, pidgeotto will install the below packages from PyPI pip
-``` pyyaml, jinja2, markdown2 ```
-* PyYAML:	To consume the config file and header of blog posts.
-* jinja2:	Templating engine
-* markdown2:	To convert markdown to HTML
-
-## Usage:
-```console
-$ pidgey init project
-```
-To initiate pidgeotto with name "project"
-
-```console
-$ pidgey new pageName
-```
-To create new page/post/note with name "pageName"
-
-```console
-$ pidgey build pageName
-```
-To build static pages and keep those in the "public" directory.
-
-## Extra Functionalaties
-1. showInHome tag is present in each note markdown.
-        ``` showInHome: True ``` 
-        will create page which are blog/note post.
-        
-        ``` showInHome: False ``` 
-        will create page which are pages.
-
-2. config.yml is extensible. 
-        For example, if you want to add favicon.ico. Keep favicon in the resource folder.
-        ``` favicon: resource/favicon.ico ``` 
-        in config.yml
-        In template, add {{ config.get('favicon') }}.
-
-3. Extra metadata per page.
-        If you want to add some metadata to your page, it can be done using the below command on the markdown page.
-        ``` meta : '<link rel="stylesheet" type="text/css" href="/extra.css" /> ```
-
-
-## Structure
-
-    pidgeotto_project
-    ├── public
-    ├── config.yml
-    ├── content
-    │   ├── header.md
-    │   ├── footer.md
-    │   ├── home.md
-    │   ├── archive.md
-    │   └── note
-    │       └── other_pages.md
-    ├── resource
-    └── templates
-        ├── home_template.html
-        ├── note_template.html
-        └── rss_template.xml
-
-* config.yml:	To configure the title, name, CSS file, js file, and other configurations.
-* resource:	Location to store all CSS, js, image data and other static content.
-* content:	All markdown files are stored here.
-* template:	Layouts for different HTML pages are kept here.
-* public: All generated static files. It can be changed in config.yml
-
-## Example
-
-Below are examples of sites running via pidgeotto.
-1. [nihar.page](https://nihar.page)
-
-
-## TODO
-
-* (A) 08-05-2021 Clean up some clutter coding
-
-## Update
-
-### 0.0.3
-
-* Server Functionality added
-* Automatic .md extension
-* Error/Exception handled
+# pidgeotto
+
+## Description
+Yet another static website generator. 
+
+Why choose pidgeotto?
+1. Free of javascript.
+2. Extensible, flexible, forkable.
+3. Minimal and fast.
+4. Free under MIT License.
+
+## Installation
+``` pip install pidgeotto ```
+
+$ pip install git+https://github.com/niharokz/pidgeotto
+
+## Prerequisites
+By default, pidgeotto will install the below packages from PyPI pip
+``` pyyaml, jinja2, markdown2 ```
+* PyYAML:	To consume the config file and header of blog posts.
+* jinja2:	Templating engine
+* markdown2:	To convert markdown to HTML
+
+## Usage:
+```console
+$ pidgey init project
+```
+To initiate pidgeotto with name "project"
+
+```console
+$ pidgey new pageName
+```
+To create new page/post/note with name "pageName"
+
+```console
+$ pidgey build pageName
+```
+To build static pages and keep those in the "public" directory.
+
+## Extra Functionalaties
+1. showInHome tag is present in each note markdown.
+        ``` showInHome: True ``` 
+        will create page which are blog/note post.
+        
+        ``` showInHome: False ``` 
+        will create page which are pages.
+
+2. config.yml is extensible. 
+        For example, if you want to add favicon.ico. Keep favicon in the resource folder.
+        ``` favicon: resource/favicon.ico ``` 
+        in config.yml
+        In template, add {{ config.get('favicon') }}.
+
+3. Extra metadata per page.
+        If you want to add some metadata to your page, it can be done using the below command on the markdown page.
+        ``` meta : '<link rel="stylesheet" type="text/css" href="/extra.css" /> ```
+
+
+## Structure
+
+    pidgeotto_project
+    ├── public
+    ├── config.yml
+    ├── content
+    │   ├── header.md
+    │   ├── footer.md
+    │   ├── home.md
+    │   ├── archive.md
+    │   └── note
+    │       └── other_pages.md
+    ├── resource
+    └── templates
+        ├── home_template.html
+        ├── note_template.html
+        └── rss_template.xml
+
+* config.yml:	To configure the title, name, CSS file, js file, and other configurations.
+* resource:	Location to store all CSS, js, image data and other static content.
+* content:	All markdown files are stored here.
+* template:	Layouts for different HTML pages are kept here.
+* public: All generated static files. It can be changed in config.yml
+
+## Example
+
+Below are examples of sites running via pidgeotto.
+1. [nih.ar](https://nih.ar)
+
+
+## TODO
+
+* (A) 08-05-2021 Clean up some clutter coding
+
+## Update
+
+### 0.0.3
+
+* Server Functionality added
+* Automatic .md extension
+* Error/Exception handled
+
+### 0.0.4
+
+* Cleanup
+
+### 0.0.5
+
+* Windows support added
```

### Comparing `pidgeotto-0.0.4/pidgey/builder.py` & `pidgeotto-0.0.5/pidgey/builder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,125 +1,124 @@
-#!/bin/python
-
-#   
-#       ███╗   ██╗██╗██╗  ██╗ █████╗ ██████╗ ███████╗
-#       ████╗  ██║██║██║  ██║██╔══██╗██╔══██╗██╔════╝
-#       ██╔██╗ ██║██║███████║███████║██████╔╝███████╗
-#       ██║╚██╗██║██║██╔══██║██╔══██║██╔══██╗╚════██║
-#       ██║ ╚████║██║██║  ██║██║  ██║██║  ██║███████║
-#       ╚═╝  ╚═══╝╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚══════╝
-#       DRAFTED BY [https://nihar.page] ON 10-04-2021.
-#       SOURCE [builder.py] LAST MODIFIED ON 08-05-2021.
-#
-
-# External imports
-from shutil import copytree, rmtree, copy
-from os import path, makedirs
-from glob import glob
-from yaml import safe_load
-from jinja2 import Environment, FileSystemLoader
-from markdown2 import markdown
-
-def buildPidgey():
-    # Create Page
-    def create_page(template,post_detail,md,filename):
-        post_template = Environment(loader=FileSystemLoader(searchpath='./')).get_template(template)
-        post_title = title
-        post_date = post_data = posts_list = last_date = nextpage = post_meta = post_subtitle = ""
-        post_path =  home_path
-        if filename=="index.html":
-            post_file = filename
-            posts_list = posts
-        elif filename.endswith(".xml") :
-            post_file = filename
-            posts_list = posts
-            last_date = posts_list[0].get('date')
-        elif post_detail == None :
-            post_file = filename.replace('.md','.html')
-        else:
-            post_title = post_detail.get("title")
-            post_subtitle = post_detail.get("subtitle")
-            post_date = post_detail.get("date")
-            post_meta = post_detail.get("meta")
-            post_data = filename.split('/')
-            post_path = path.join(home_path)
-            post_file = post_data[2].replace('.md','.html')
-            post_data = post_data[1]
-
-            makedirs(post_path,exist_ok=True)
-
-        with open(path.join(post_path,post_file),'w') as output_file:
-            output_file.write(
-                post_template.render(
-                    title = title,
-                    post_title = post_title,
-                    post_subtitle = post_subtitle,
-                    date = post_date,
-                    metad = post_meta,
-                    url = path.join(url,post_file),
-                    article = markdown(md),
-                    posts = posts_list,
-                    home = home_md,
-                    header = markdown(readmd(header_md)),
-                    footer = markdown(readmd(footer_md)),
-                    nextpage = nextpage,
-                    last_date = last_date,
-                    config=config
-                )
-            )
-        output_file.close()
-        return post_file
-    
-    
-    # Markdown file to string
-    def readmd(md):
-        with open(md,'r') as data:
-            return data.read()
-
-
-    # PROGRAM STARTS HERE
-    try:
-        with open('config.yml') as conf:
-            config = safe_load(conf.read())
-            for key,val in config.items():
-                globals()[key] = val
-
-        # Recreated home path with resource
-        if path.exists(home_path):
-            rmtree(home_path)
-        copytree(resource_path, home_path)
-        
-        #Create all pages from content/note
-        posts = []
-        for note in glob(path.join(content_path,"note","*.md")):
-            yaml_lines, ym, md = [],'',''
-            with open(note) as infile:
-                for s in infile:
-                    if s.startswith('---'):
-                        for s in infile:
-                            if s.startswith('---'):
-                                break;
-                            else:
-                                yaml_lines.append(s)
-                        ym = ''.join(yaml_lines)
-                        md = ''.join(infile)
-                        break;
-            post_detail=safe_load(ym)
-            if (post_detail is not None):
-                post_url = create_page(note_template,post_detail,md,note)
-                ymd = post_detail
-                ymd.update({'url' : '/'+post_url})
-                ymd.update({'note' : markdown(md)})
-                posts += [ymd]
-        
-        #Sort posts based on date in descending order
-        posts= sorted(posts, key=lambda post :  post['date'], reverse=True)
-        
-        # Other pages are created here
-        create_page(home_template,None,readmd(home_md),"index.html")
-        create_page(feed_template,None,readmd(home_md),"rss.xml")
-
-    except:
-        print("while building pidgey, some issue occured.")
-        print("This can be due to \n\t1. Not a pidgey directory. \n\t2. Unknown file structure")
-
-
+#!/bin/python
+
+#   
+#       ███╗   ██╗██╗██╗  ██╗ █████╗ ██████╗ ███████╗
+#       ████╗  ██║██║██║  ██║██╔══██╗██╔══██╗██╔════╝
+#       ██╔██╗ ██║██║███████║███████║██████╔╝███████╗
+#       ██║╚██╗██║██║██╔══██║██╔══██║██╔══██╗╚════██║
+#       ██║ ╚████║██║██║  ██║██║  ██║██║  ██║███████║
+#       ╚═╝  ╚═══╝╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚══════╝
+#       DRAFTED BY [https://nih.ar] ON 10-04-2021.
+#       SOURCE [builder.py] LAST MODIFIED ON 25-06-2023.
+#
+
+# External imports
+from shutil import copytree, rmtree, copy
+from os import path, makedirs, sep
+from glob import glob
+from yaml import safe_load
+from jinja2 import Environment, FileSystemLoader
+from markdown2 import markdown
+
+def buildPidgey():
+    # Create Page
+    def create_page(template,post_detail,md,filename):
+        post_template = Environment(loader=FileSystemLoader(searchpath='./')).get_template(template)
+        post_title = title
+        post_date = post_data = posts_list = last_date = nextpage = post_meta = post_subtitle = ""
+        post_path =  home_path
+        if filename=="index.html":
+            post_file = filename
+            posts_list = posts
+        elif filename.endswith(".xml") :
+            post_file = filename
+            posts_list = posts
+            last_date = posts_list[0].get('date')
+        elif post_detail == None :
+            post_file = filename.replace('.md','.html')
+        else:
+            post_title = post_detail.get("title")
+            post_subtitle = post_detail.get("subtitle")
+            post_date = post_detail.get("date")
+            post_meta = post_detail.get("meta")
+            post_data = filename.split(sep)
+            post_path = path.join(home_path)
+            post_file = post_data[2].replace('.md','.html')
+            post_data = post_data[1]
+            makedirs(post_path,exist_ok=True)
+
+        with open(path.join(post_path,post_file),'w',encoding='utf8', errors='ignore') as output_file:
+            output_file.write(
+                post_template.render(
+                    title = title,
+                    post_title = post_title,
+                    post_subtitle = post_subtitle,
+                    date = post_date,
+                    metad = post_meta,
+                    url = path.join(url,post_file),
+                    article = markdown(md),
+                    posts = posts_list,
+                    home = home_md,
+                    header = markdown(readmd(header_md)),
+                    footer = markdown(readmd(footer_md)),
+                    nextpage = nextpage,
+                    last_date = last_date,
+                    config=config
+                )
+            )
+        output_file.close()
+        return post_file
+    
+    
+    # Markdown file to string
+    def readmd(md):
+        with open(md,'r',encoding='utf8', errors='ignore') as data:
+            return data.read()
+
+
+    # PROGRAM STARTS HERE
+    try:
+        with open('config.yml',encoding='utf8', errors='ignore') as conf:
+            config = safe_load(conf.read())
+            for key,val in config.items():
+                globals()[key] = val
+
+        # Recreated home path with resource
+        if path.exists(home_path):
+            rmtree(home_path)
+        copytree(resource_path, home_path)
+        
+        #Create all pages from content/note
+        posts = []
+        for note in glob(path.join(content_path,"note","*.md")):
+            yaml_lines, ym, md = [],'',''
+            with open(note,encoding='utf8', errors='ignore') as infile:
+                for s in infile:
+                    if s.startswith('---'):
+                        for s in infile:
+                            if s.startswith('---'):
+                                break;
+                            else:
+                                yaml_lines.append(s)
+                        ym = ''.join(yaml_lines)
+                        md = ''.join(infile)
+                        break;
+            post_detail=safe_load(ym)
+            if (post_detail is not None):
+                post_url = create_page(note_template,post_detail,md,note)
+                ymd = post_detail
+                ymd.update({'url' : '/'+post_url})
+                ymd.update({'note' : markdown(md)})
+                posts += [ymd]
+        
+        #Sort posts based on date in descending order
+        posts= sorted(posts, key=lambda post :  post['date'], reverse=True)
+        
+        # Other pages are created here
+        create_page(home_template,None,readmd(home_md),"index.html")
+        create_page(feed_template,None,readmd(home_md),"rss.xml")
+
+    except Exception as e:
+        print("while building pidgey, some issue occured.")
+        print("This can be due to \n\t1. Not a pidgey directory. \n\t2. Unknown file structure")
+
+
```

### Comparing `pidgeotto-0.0.4/pidgey/creator.py` & `pidgeotto-0.0.5/pidgey/creator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,574 +1,565 @@
-00000000: 2321 2f62 696e 2f70 7974 686f 6e33 0a0a  #!/bin/python3..
-00000010: 230a 2320 2020 2020 2020 e296 88e2 9688  #.#       ......
-00000020: e296 88e2 9597 2020 20e2 9688 e296 88e2  ......   .......
-00000030: 9597 e296 88e2 9688 e295 97e2 9688 e296  ................
-00000040: 88e2 9597 2020 e296 88e2 9688 e295 9720  ....  ......... 
-00000050: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
-00000060: 9597 20e2 9688 e296 88e2 9688 e296 88e2  .. .............
-00000070: 9688 e296 88e2 9597 20e2 9688 e296 88e2  ........ .......
-00000080: 9688 e296 88e2 9688 e296 88e2 9688 e295  ................
-00000090: 970a 2320 2020 2020 2020 e296 88e2 9688  ..#       ......
-000000a0: e296 88e2 9688 e295 9720 20e2 9688 e296  .........  .....
-000000b0: 88e2 9591 e296 88e2 9688 e295 91e2 9688  ................
-000000c0: e296 88e2 9591 2020 e296 88e2 9688 e295  ......  ........
-000000d0: 91e2 9688 e296 88e2 9594 e295 90e2 9590  ................
-000000e0: e296 88e2 9688 e295 97e2 9688 e296 88e2  ................
-000000f0: 9594 e295 90e2 9590 e296 88e2 9688 e295  ................
-00000100: 97e2 9688 e296 88e2 9594 e295 90e2 9590  ................
-00000110: e295 90e2 9590 e295 9d0a 2320 2020 2020  ..........#     
-00000120: 2020 e296 88e2 9688 e295 94e2 9688 e296    ..............
-00000130: 88e2 9597 20e2 9688 e296 88e2 9591 e296  .... ...........
-00000140: 88e2 9688 e295 91e2 9688 e296 88e2 9688  ................
-00000150: e296 88e2 9688 e296 88e2 9688 e295 91e2  ................
-00000160: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
-00000170: 88e2 9688 e295 91e2 9688 e296 88e2 9688  ................
-00000180: e296 88e2 9688 e296 88e2 9594 e295 9de2  ................
-00000190: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
-000001a0: 88e2 9688 e295 970a 2320 2020 2020 2020  ........#       
-000001b0: e296 88e2 9688 e295 91e2 959a e296 88e2  ................
-000001c0: 9688 e295 97e2 9688 e296 88e2 9591 e296  ................
-000001d0: 88e2 9688 e295 91e2 9688 e296 88e2 9594  ................
-000001e0: e295 90e2 9590 e296 88e2 9688 e295 91e2  ................
-000001f0: 9688 e296 88e2 9594 e295 90e2 9590 e296  ................
-00000200: 88e2 9688 e295 91e2 9688 e296 88e2 9594  ................
-00000210: e295 90e2 9590 e296 88e2 9688 e295 97e2  ................
-00000220: 959a e295 90e2 9590 e295 90e2 9590 e296  ................
-00000230: 88e2 9688 e295 910a 2320 2020 2020 2020  ........#       
-00000240: e296 88e2 9688 e295 9120 e295 9ae2 9688  ......... ......
-00000250: e296 88e2 9688 e296 88e2 9591 e296 88e2  ................
-00000260: 9688 e295 91e2 9688 e296 88e2 9591 2020  ..............  
-00000270: e296 88e2 9688 e295 91e2 9688 e296 88e2  ................
-00000280: 9591 2020 e296 88e2 9688 e295 91e2 9688  ..  ............
-00000290: e296 88e2 9591 2020 e296 88e2 9688 e295  ......  ........
-000002a0: 91e2 9688 e296 88e2 9688 e296 88e2 9688  ................
-000002b0: e296 88e2 9688 e295 910a 2320 2020 2020  ..........#     
-000002c0: 2020 e295 9ae2 9590 e295 9d20 20e2 959a    .........  ...
-000002d0: e295 90e2 9590 e295 90e2 959d e295 9ae2  ................
-000002e0: 9590 e295 9de2 959a e295 90e2 959d 2020  ..............  
-000002f0: e295 9ae2 9590 e295 9de2 959a e295 90e2  ................
-00000300: 959d 2020 e295 9ae2 9590 e295 9de2 959a  ..  ............
-00000310: e295 90e2 959d 2020 e295 9ae2 9590 e295  ......  ........
-00000320: 9de2 959a e295 90e2 9590 e295 90e2 9590  ................
-00000330: e295 90e2 9590 e295 9d0a 2320 2020 2020  ..........#     
-00000340: 2020 4452 4146 5445 4420 4259 205b 6874    DRAFTED BY [ht
-00000350: 7470 733a 2f2f 6e69 6861 722e 7061 6765  tps://nihar.page
-00000360: 5d20 4f4e 2031 382d 3034 2d32 3032 312e  ] ON 18-04-2021.
-00000370: 0a23 2020 2020 2020 2053 4f55 5243 4520  .#       SOURCE 
-00000380: 5b63 7265 6174 6f72 2e70 795d 204c 4153  [creator.py] LAS
-00000390: 5420 4d4f 4449 4649 4544 204f 4e20 3038  T MODIFIED ON 08
-000003a0: 2d30 352d 3230 3231 2e0a 230a 0a0a 6672  -05-2021..#...fr
-000003b0: 6f6d 206f 7320 696d 706f 7274 206d 6b64  om os import mkd
-000003c0: 6972 2c20 7061 7468 0a66 726f 6d20 6461  ir, path.from da
-000003d0: 7465 7469 6d65 2069 6d70 6f72 7420 6461  tetime import da
-000003e0: 7465 7469 6d65 0a0a 0a64 6566 2063 7265  tetime...def cre
-000003f0: 6174 6543 6f6e 6669 6728 7069 6467 6579  ateConfig(pidgey
-00000400: 4e61 6d65 293a 0a20 2020 2077 6974 6820  Name):.    with 
-00000410: 6f70 656e 2870 6174 682e 6a6f 696e 2870  open(path.join(p
-00000420: 6964 6765 794e 616d 652c 2763 6f6e 6669  idgeyName,'confi
-00000430: 672e 796d 6c27 292c 2777 2729 2061 7320  g.yml'),'w') as 
-00000440: 663a 0a20 2020 2020 2020 2063 6f6e 665f  f:.        conf_
-00000450: 6461 7461 203d 2028 0a20 2020 2020 2020  data = (.       
-00000460: 2020 2020 2022 2222 2320 4d61 6e64 6174       """# Mandat
-00000470: 6f72 7920 436f 6e66 6967 7572 6174 696f  ory Configuratio
-00000480: 6e0a 7469 746c 6520 3a20 4465 6d6f 2070  n.title : Demo p
-00000490: 6964 6765 6f74 746f 2077 6562 7369 7465  idgeotto website
-000004a0: 0a75 726c 203a 2079 6f75 7264 6f6d 6169  .url : yourdomai
-000004b0: 6e2e 746c 640a 6e6f 7465 5f74 656d 706c  n.tld.note_templ
-000004c0: 6174 6520 3a20 7465 6d70 6c61 7465 2f6e  ate : template/n
-000004d0: 6f74 655f 7465 6d70 6c61 7465 2e68 746d  ote_template.htm
-000004e0: 6c20 2020 2320 5465 6d70 6c61 7465 206f  l   # Template o
-000004f0: 6620 6e6f 7465 2070 6167 650a 686f 6d65  f note page.home
-00000500: 5f74 656d 706c 6174 6520 3a20 7465 6d70  _template : temp
-00000510: 6c61 7465 2f68 6f6d 655f 7465 6d70 6c61  late/home_templa
-00000520: 7465 2e68 746d 6c20 2020 2320 5465 6d70  te.html   # Temp
-00000530: 6c61 7465 206f 6620 686f 6d65 2070 6167  late of home pag
-00000540: 650a 6665 6564 5f74 656d 706c 6174 6520  e.feed_template 
-00000550: 3a20 7465 6d70 6c61 7465 2f66 6565 645f  : template/feed_
-00000560: 7465 6d70 6c61 7465 2e78 6d6c 2020 2023  template.xml   #
-00000570: 2054 656d 706c 6174 6520 6f66 2066 6565   Template of fee
-00000580: 642f 7273 7320 7061 6765 0a68 6f6d 655f  d/rss page.home_
-00000590: 7061 7468 203a 2070 7562 6c69 6320 2023  path : public  #
-000005a0: 2041 6674 6572 2062 7569 6c74 2c20 7374   After built, st
-000005b0: 6174 6963 2066 696c 6573 2077 696c 6c20  atic files will 
-000005c0: 6265 2067 656e 6572 6174 6564 2068 6572  be generated her
-000005d0: 650a 636f 6e74 656e 745f 7061 7468 203a  e.content_path :
-000005e0: 2063 6f6e 7465 6e74 2023 2041 6c6c 2070   content # All p
-000005f0: 6f73 7420 6e6f 7465 7320 6d61 726b 646f  ost notes markdo
-00000600: 776e 206c 6f63 6174 696f 6e0a 7265 736f  wn location.reso
-00000610: 7572 6365 5f70 6174 6820 3a20 7374 6174  urce_path : stat
-00000620: 6963 2023 2041 6c6c 2063 7373 2c20 6a73  ic # All css, js
-00000630: 2c20 696d 6167 6520 6c6f 6361 7469 6f6e  , image location
-00000640: 0a68 6f6d 655f 6d64 203a 2063 6f6e 7465  .home_md : conte
-00000650: 6e74 2f68 6f6d 652e 6d64 2023 2048 6f6d  nt/home.md # Hom
-00000660: 6570 6167 6520 636f 6e74 656e 740a 6865  epage content.he
-00000670: 6164 6572 5f6d 6420 3a20 636f 6e74 656e  ader_md : conten
-00000680: 742f 6865 6164 6572 2e6d 6420 2320 4865  t/header.md # He
-00000690: 6164 6572 2063 6f6e 7465 6e74 0a66 6f6f  ader content.foo
-000006a0: 7465 725f 6d64 203a 2063 6f6e 7465 6e74  ter_md : content
-000006b0: 2f66 6f6f 7465 722e 6d64 2023 2046 6f6f  /footer.md # Foo
-000006c0: 7465 7220 636f 6e74 656e 740a 0a23 204f  ter content..# O
-000006d0: 7074 696f 6e61 6c20 436f 6e66 6967 7572  ptional Configur
-000006e0: 6174 696f 6e2c 2041 6464 2079 6f75 7220  ation, Add your 
-000006f0: 6f77 6e20 636f 6e66 6967 7320 6865 7265  own configs here
-00000700: 0a73 6974 652d 7469 746c 6520 3a20 4465  .site-title : De
-00000710: 6d6f 2050 6964 6765 6f74 746f 0a63 7373  mo Pidgeotto.css
-00000720: 203a 2064 656d 6f2e 6373 730a 6465 7363   : demo.css.desc
-00000730: 203a 2057 7269 7465 2061 6e79 7468 696e   : Write anythin
-00000740: 6720 7468 6174 2068 756d 616e 2061 6e64  g that human and
-00000750: 206d 6163 6869 6e65 2063 616e 2075 6e64   machine can und
-00000760: 6572 7374 616e 642e 0a6d 6169 6c20 3a20  erstand..mail : 
-00000770: 736f 6d65 406d 6169 6c2e 636f 6d0a 2020  some@mail.com.  
-00000780: 2020 2020 2020 2020 2020 2222 2229 0a20            """). 
-00000790: 2020 2020 2020 2066 2e77 7269 7465 2863         f.write(c
-000007a0: 6f6e 665f 6461 7461 290a 2020 2020 2020  onf_data).      
-000007b0: 2020 7072 696e 7428 2763 6f6e 6669 672e    print('config.
-000007c0: 796d 6c20 6372 6561 7465 642e 2729 0a0a  yml created.')..
-000007d0: 0a64 6566 2063 7265 6174 6554 656d 706c  .def createTempl
-000007e0: 6174 6573 2870 6964 6765 794e 616d 6529  ates(pidgeyName)
-000007f0: 3a0a 2020 2020 7769 7468 206f 7065 6e28  :.    with open(
-00000800: 7061 7468 2e6a 6f69 6e28 7069 6467 6579  path.join(pidgey
-00000810: 4e61 6d65 2c27 7465 6d70 6c61 7465 272c  Name,'template',
-00000820: 2768 6f6d 655f 7465 6d70 6c61 7465 2e68  'home_template.h
-00000830: 746d 6c27 292c 2777 2729 2061 7320 663a  tml'),'w') as f:
-00000840: 0a20 2020 2020 2020 2063 6f6e 665f 6461  .        conf_da
-00000850: 7461 203d 2028 0a20 2020 2020 2020 2022  ta = (.        "
-00000860: 2222 3c21 444f 4354 5950 4520 6874 6d6c  ""<!DOCTYPE html
-00000870: 3e0a 3c68 746d 6c20 6c61 6e67 3d22 656e  >.<html lang="en
-00000880: 2d49 4e22 2064 6174 612d 7468 656d 653d  -IN" data-theme=
-00000890: 2264 6172 6b22 3e0a 0a3c 6865 6164 3e0a  "dark">..<head>.
-000008a0: 3c6d 6574 6120 6368 6172 7365 743d 2275  <meta charset="u
-000008b0: 7466 2d38 223e 0a3c 6d65 7461 2068 7474  tf-8">.<meta htt
-000008c0: 702d 6571 7569 763d 2258 2d55 412d 436f  p-equiv="X-UA-Co
-000008d0: 6d70 6174 6962 6c65 2220 636f 6e74 656e  mpatible" conten
-000008e0: 743d 2249 453d 6564 6765 223e 0a3c 6d65  t="IE=edge">.<me
-000008f0: 7461 206e 616d 653d 2276 6965 7770 6f72  ta name="viewpor
-00000900: 7422 2063 6f6e 7465 6e74 3d22 7769 6474  t" content="widt
-00000910: 683d 6465 7669 6365 2d77 6964 7468 2c20  h=device-width, 
-00000920: 696e 6974 6961 6c2d 7363 616c 653d 3122  initial-scale=1"
-00000930: 3e0a 3c6d 6574 6120 6e61 6d65 3d22 6465  >.<meta name="de
-00000940: 7363 7269 7074 696f 6e22 2063 6f6e 7465  scription" conte
-00000950: 6e74 3d22 207b 7b20 636f 6e66 6967 2e67  nt=" {{ config.g
-00000960: 6574 2827 6465 7363 2729 207d 7d22 3e0a  et('desc') }}">.
-00000970: 3c74 6974 6c65 3e7b 7b20 636f 6e66 6967  <title>{{ config
-00000980: 2e67 6574 2827 7369 7465 2d74 6974 6c65  .get('site-title
-00000990: 2729 207d 7d3c 2f74 6974 6c65 3e0a 3c6c  ') }}</title>.<l
-000009a0: 696e 6b20 7265 6c3d 2273 7479 6c65 7368  ink rel="stylesh
-000009b0: 6565 7422 2074 7970 653d 2274 6578 742f  eet" type="text/
-000009c0: 6373 7322 206d 6564 6961 3d22 7363 7265  css" media="scre
-000009d0: 656e 2220 6872 6566 3d22 7b7b 2063 6f6e  en" href="{{ con
-000009e0: 6669 672e 6765 7428 2763 7373 2729 207d  fig.get('css') }
-000009f0: 7d22 202f 3e0a 3c6c 696e 6b20 7265 6c3d  }" />.<link rel=
-00000a00: 2261 6c74 6572 6e61 7465 2220 7479 7065  "alternate" type
-00000a10: 3d22 6170 706c 6963 6174 696f 6e2f 6174  ="application/at
-00000a20: 6f6d 2b78 6d6c 2220 7469 746c 653d 2252  om+xml" title="R
-00000a30: 6563 656e 7420 626c 6f67 2070 6f73 7473  ecent blog posts
-00000a40: 2220 6872 6566 3d22 2f72 7373 2e78 6d6c  " href="/rss.xml
-00000a50: 223e 0a3c 2f68 6561 643e 0a0a 3c62 6f64  ">.</head>..<bod
-00000a60: 793e 0a3c 6865 6164 6572 3e0a 3c68 313e  y>.<header>.<h1>
-00000a70: 3c61 2068 7265 663d 222f 223e 7b25 2066  <a href="/">{% f
-00000a80: 696c 7465 7220 6c6f 7765 7220 257d 207b  ilter lower %} {
-00000a90: 7b20 7469 746c 6520 7d7d 207b 2520 656e  { title }} {% en
-00000aa0: 6466 696c 7465 7220 257d 3c2f 613e 3c2f  dfilter %}</a></
-00000ab0: 6831 3e0a 7b7b 2068 6561 6465 7220 7d7d  h1>.{{ header }}
-00000ac0: 0a3c 2f68 6561 6465 723e 0a3c 7365 6374  .</header>.<sect
-00000ad0: 696f 6e3e 0a7b 7b61 7274 6963 6c65 7d7d  ion>.{{article}}
-00000ae0: 0a3c 756c 3e0a 7b25 2066 6f72 2070 6f73  .<ul>.{% for pos
-00000af0: 7420 696e 2070 6f73 7473 2025 7d7b 2520  t in posts %}{% 
-00000b00: 6966 2028 706f 7374 2e73 686f 7749 6e48  if (post.showInH
-00000b10: 6f6d 6520 6973 2075 6e64 6566 696e 6564  ome is undefined
-00000b20: 2920 6f72 2070 6f73 742e 7368 6f77 496e  ) or post.showIn
-00000b30: 486f 6d65 2025 7d0a 3c6c 693e 7b7b 2070  Home %}.<li>{{ p
-00000b40: 6f73 742e 6461 7465 2e73 7472 6674 696d  ost.date.strftim
-00000b50: 6528 2725 6420 256d 2025 5927 2920 7d7d  e('%d %m %Y') }}
-00000b60: 203b 203c 6120 6872 6566 3d22 7b7b 2070   ; <a href="{{ p
-00000b70: 6f73 742e 7572 6c20 7d7d 223e 7b25 2066  ost.url }}">{% f
-00000b80: 696c 7465 7220 6c6f 7765 7220 257d 207b  ilter lower %} {
-00000b90: 7b20 706f 7374 2e74 6974 6c65 207d 7d20  { post.title }} 
-00000ba0: 7b25 2065 6e64 6669 6c74 6572 2025 7d3c  {% endfilter %}<
-00000bb0: 2f61 3e3c 2f6c 693e 0a7b 2520 656e 6469  /a></li>.{% endi
-00000bc0: 6620 257d 7b25 2065 6e64 666f 7220 257d  f %}{% endfor %}
-00000bd0: 0a7b 2520 6966 206e 6578 7470 6167 6520  .{% if nextpage 
-00000be0: 257d 203c 6120 6872 6566 3d22 7b7b 206e  %} <a href="{{ n
-00000bf0: 6578 7470 6167 6520 7d7d 223e 4f6c 6465  extpage }}">Olde
-00000c00: 7220 4e6f 7465 7320 3e3e 203c 2f61 3e20  r Notes >> </a> 
-00000c10: 7b25 2065 6e64 6966 2025 7d0a 3c2f 756c  {% endif %}.</ul
-00000c20: 3e0a 3c2f 7365 6374 696f 6e3e 0a3c 666f  >.</section>.<fo
-00000c30: 6f74 6572 3e0a 7b7b 2066 6f6f 7465 7220  oter>.{{ footer 
-00000c40: 7d7d 0a3c 2f66 6f6f 7465 723e 0a3c 2f62  }}.</footer>.</b
-00000c50: 6f64 793e 0a3c 2f68 746d 6c3e 0a20 2020  ody>.</html>.   
-00000c60: 2020 2020 2020 2020 2022 2222 290a 2020           """).  
-00000c70: 2020 2020 2020 662e 7772 6974 6528 636f        f.write(co
-00000c80: 6e66 5f64 6174 6129 0a20 2020 2020 2020  nf_data).       
-00000c90: 2070 7269 6e74 2827 686f 6d65 5f74 656d   print('home_tem
-00000ca0: 706c 6174 6520 6372 6561 7465 642e 2729  plate created.')
-00000cb0: 0a0a 2020 2020 7769 7468 206f 7065 6e28  ..    with open(
-00000cc0: 7061 7468 2e6a 6f69 6e28 7069 6467 6579  path.join(pidgey
-00000cd0: 4e61 6d65 2c27 7465 6d70 6c61 7465 272c  Name,'template',
-00000ce0: 276e 6f74 655f 7465 6d70 6c61 7465 2e68  'note_template.h
-00000cf0: 746d 6c27 292c 2777 2729 2061 7320 663a  tml'),'w') as f:
-00000d00: 0a20 2020 2020 2020 2063 6f6e 665f 6461  .        conf_da
-00000d10: 7461 203d 2028 0a20 2020 2020 2020 2020  ta = (.         
-00000d20: 2020 2022 2222 3c21 444f 4354 5950 4520     """<!DOCTYPE 
-00000d30: 6874 6d6c 3e0a 3c68 746d 6c20 6c61 6e67  html>.<html lang
-00000d40: 3d22 656e 2220 6461 7461 2d74 6865 6d65  ="en" data-theme
-00000d50: 3d22 6461 726b 223e 0a3c 6865 6164 3e0a  ="dark">.<head>.
-00000d60: 3c6d 6574 6120 6368 6172 7365 743d 2275  <meta charset="u
-00000d70: 7466 2d38 223e 0a0a 3c74 6974 6c65 3e7b  tf-8">..<title>{
-00000d80: 7b20 706f 7374 5f74 6974 6c65 207d 7d3c  { post_title }}<
-00000d90: 2f74 6974 6c65 3e0a 0a3c 6d65 7461 2068  /title>..<meta h
-00000da0: 7474 702d 6571 7569 763d 2258 2d55 412d  ttp-equiv="X-UA-
-00000db0: 436f 6d70 6174 6962 6c65 2220 636f 6e74  Compatible" cont
-00000dc0: 656e 743d 2249 453d 6564 6765 223e 0a3c  ent="IE=edge">.<
-00000dd0: 6d65 7461 206e 616d 653d 2276 6965 7770  meta name="viewp
-00000de0: 6f72 7422 2063 6f6e 7465 6e74 3d22 7769  ort" content="wi
-00000df0: 6474 683d 6465 7669 6365 2d77 6964 7468  dth=device-width
-00000e00: 2c20 696e 6974 6961 6c2d 7363 616c 653d  , initial-scale=
-00000e10: 3122 3e0a 3c6d 6574 6120 6e61 6d65 3d22  1">.<meta name="
-00000e20: 6465 7363 7269 7074 696f 6e22 2063 6f6e  description" con
-00000e30: 7465 6e74 3d22 207b 7b20 706f 7374 5f73  tent=" {{ post_s
-00000e40: 7562 7469 746c 6520 7d7d 223e 0a0a 3c6c  ubtitle }}">..<l
-00000e50: 696e 6b20 7265 6c3d 2273 7479 6c65 7368  ink rel="stylesh
-00000e60: 6565 7422 2074 7970 653d 2274 6578 742f  eet" type="text/
-00000e70: 6373 7322 206d 6564 6961 3d22 7363 7265  css" media="scre
-00000e80: 656e 2220 6872 6566 3d22 7b7b 2063 6f6e  en" href="{{ con
-00000e90: 6669 672e 6765 7428 2763 7373 2729 207d  fig.get('css') }
-00000ea0: 7d22 202f 3e0a 3c6c 696e 6b20 7265 6c3d  }" />.<link rel=
-00000eb0: 2261 6c74 6572 6e61 7465 2220 7479 7065  "alternate" type
-00000ec0: 3d22 6170 706c 6963 6174 696f 6e2f 6174  ="application/at
-00000ed0: 6f6d 2b78 6d6c 2220 7469 746c 653d 2252  om+xml" title="R
-00000ee0: 6563 656e 7420 626c 6f67 2070 6f73 7473  ecent blog posts
-00000ef0: 2220 6872 6566 3d22 2f72 7373 2e78 6d6c  " href="/rss.xml
-00000f00: 223e 0a7b 2520 6966 206d 6574 6164 2025  ">.{% if metad %
-00000f10: 7d20 207b 7b20 6d65 7461 6420 7d7d 207b  }  {{ metad }} {
-00000f20: 2520 656e 6469 6620 257d 0a3c 2f68 6561  % endif %}.</hea
-00000f30: 643e 0a0a 3c62 6f64 793e 0a3c 6865 6164  d>..<body>.<head
-00000f40: 6572 3e0a 3c68 313e 7b7b 2070 6f73 745f  er>.<h1>{{ post_
-00000f50: 7469 746c 6520 7d7d 203c 2f68 313e 2020  title }} </h1>  
-00000f60: 0a3c 2f68 6561 6465 723e 0a3c 6172 7469  .</header>.<arti
-00000f70: 636c 653e 0a7b 7b20 6172 7469 636c 6520  cle>.{{ article 
-00000f80: 7d7d 0a7b 2520 6966 2064 6174 6520 257d  }}.{% if date %}
-00000f90: 200a 3c70 3e23 204c 6173 7420 7570 6461   .<p># Last upda
-00000fa0: 7465 6420 6f6e 203c 7469 6d65 3e7b 7b20  ted on <time>{{ 
-00000fb0: 6461 7465 2e73 7472 6674 696d 6528 2725  date.strftime('%
-00000fc0: 6420 2562 2025 5927 2920 7d7d 2e3c 2f74  d %b %Y') }}.</t
-00000fd0: 696d 653e 3c2f 703e 0a7b 2520 656e 6469  ime></p>.{% endi
-00000fe0: 6620 257d 0a3c 2f61 7274 6963 6c65 3e0a  f %}.</article>.
-00000ff0: 3c66 6f6f 7465 723e 0a7b 7b20 666f 6f74  <footer>.{{ foot
-00001000: 6572 207d 7d0a 3c2f 666f 6f74 6572 3e0a  er }}.</footer>.
-00001010: 3c2f 626f 6479 3e0a 3c2f 6874 6d6c 3e0a  </body>.</html>.
-00001020: 2020 2020 2020 2020 2020 2020 2222 2229              """)
-00001030: 0a20 2020 2020 2020 2066 2e77 7269 7465  .        f.write
-00001040: 2863 6f6e 665f 6461 7461 290a 2020 2020  (conf_data).    
-00001050: 2020 2020 7072 696e 7428 276e 6f74 6520      print('note 
-00001060: 7465 6d70 6c61 7465 2063 7265 6174 6564  template created
-00001070: 2e27 290a 0a20 2020 2077 6974 6820 6f70  .')..    with op
-00001080: 656e 2870 6174 682e 6a6f 696e 2870 6964  en(path.join(pid
-00001090: 6765 794e 616d 652c 2774 656d 706c 6174  geyName,'templat
-000010a0: 6527 2c27 6665 6564 5f74 656d 706c 6174  e','feed_templat
-000010b0: 652e 786d 6c27 292c 2777 2729 2061 7320  e.xml'),'w') as 
-000010c0: 663a 0a20 2020 2020 2020 2063 6f6e 665f  f:.        conf_
-000010d0: 6461 7461 203d 2028 0a20 2020 2020 2020  data = (.       
-000010e0: 2020 2020 2022 2222 3c3f 786d 6c20 7665       """<?xml ve
-000010f0: 7273 696f 6e3d 2231 2e30 2220 656e 636f  rsion="1.0" enco
-00001100: 6469 6e67 3d22 5554 462d 3822 3f3e 0a3c  ding="UTF-8"?>.<
-00001110: 7273 7320 7665 7273 696f 6e3d 2232 2e30  rss version="2.0
-00001120: 220a 0978 6d6c 6e73 3a63 6f6e 7465 6e74  "..xmlns:content
-00001130: 3d22 6874 7470 3a2f 2f70 7572 6c2e 6f72  ="http://purl.or
-00001140: 672f 7273 732f 312e 302f 6d6f 6475 6c65  g/rss/1.0/module
-00001150: 732f 636f 6e74 656e 742f 220a 0978 6d6c  s/content/"..xml
-00001160: 6e73 3a77 6677 3d22 6874 7470 3a2f 2f77  ns:wfw="http://w
-00001170: 656c 6c66 6f72 6d65 6477 6562 2e6f 7267  ellformedweb.org
-00001180: 2f43 6f6d 6d65 6e74 4150 492f 220a 0978  /CommentAPI/"..x
-00001190: 6d6c 6e73 3a64 633d 2268 7474 703a 2f2f  mlns:dc="http://
-000011a0: 7075 726c 2e6f 7267 2f64 632f 656c 656d  purl.org/dc/elem
-000011b0: 656e 7473 2f31 2e31 2f22 0a09 786d 6c6e  ents/1.1/"..xmln
-000011c0: 733a 6174 6f6d 3d22 6874 7470 3a2f 2f77  s:atom="http://w
-000011d0: 7777 2e77 332e 6f72 672f 3230 3035 2f41  ww.w3.org/2005/A
-000011e0: 746f 6d22 0a09 786d 6c6e 733a 7379 3d22  tom"..xmlns:sy="
-000011f0: 6874 7470 3a2f 2f70 7572 6c2e 6f72 672f  http://purl.org/
-00001200: 7273 732f 312e 302f 6d6f 6475 6c65 732f  rss/1.0/modules/
-00001210: 7379 6e64 6963 6174 696f 6e2f 220a 2078  syndication/". x
-00001220: 6d6c 6e73 3a73 6c61 7368 3d22 6874 7470  mlns:slash="http
-00001230: 3a2f 2f70 7572 6c2e 6f72 672f 7273 732f  ://purl.org/rss/
-00001240: 312e 302f 6d6f 6475 6c65 732f 736c 6173  1.0/modules/slas
-00001250: 682f 223e 0a0a 203c 6368 616e 6e65 6c3e  h/">.. <channel>
-00001260: 0a20 203c 7469 746c 653e 7b7b 7469 746c  .  <title>{{titl
-00001270: 657d 7d3c 2f74 6974 6c65 3e0a 2020 3c61  e}}</title>.  <a
-00001280: 746f 6d3a 6c69 6e6b 2068 7265 663d 227b  tom:link href="{
-00001290: 7b20 7572 6c20 7d7d 2220 7265 6c3d 2273  { url }}" rel="s
-000012a0: 656c 6622 2074 7970 653d 2261 7070 6c69  elf" type="appli
-000012b0: 6361 7469 6f6e 2f72 7373 2b78 6d6c 2220  cation/rss+xml" 
-000012c0: 2f3e 0a20 203c 6c69 6e6b 3e7b 7b20 7572  />.  <link>{{ ur
-000012d0: 6c20 7d7d 3c2f 6c69 6e6b 3e0a 2020 3c64  l }}</link>.  <d
-000012e0: 6573 6372 6970 7469 6f6e 3e7b 7b20 7375  escription>{{ su
-000012f0: 6274 6974 6c65 207d 7d3c 2f64 6573 6372  btitle }}</descr
-00001300: 6970 7469 6f6e 3e0a 2020 3c6c 6173 7442  iption>.  <lastB
-00001310: 7569 6c64 4461 7465 3e7b 7b20 6c61 7374  uildDate>{{ last
-00001320: 5f64 6174 652e 7374 7266 7469 6d65 2827  _date.strftime('
-00001330: 2561 2c20 2564 2025 6220 2559 2025 483a  %a, %d %b %Y %H:
-00001340: 254d 3a25 5320 474d 5427 2920 7d7d 3c2f  %M:%S GMT') }}</
-00001350: 6c61 7374 4275 696c 6444 6174 653e 0a0a  lastBuildDate>..
-00001360: 2020 3c6c 616e 6775 6167 653e 656e 2d49    <language>en-I
-00001370: 4e3c 2f6c 616e 6775 6167 653e 0a20 203c  N</language>.  <
-00001380: 7379 3a75 7064 6174 6550 6572 696f 643e  sy:updatePeriod>
-00001390: 7765 656b 6c79 3c2f 7379 3a75 7064 6174  weekly</sy:updat
-000013a0: 6550 6572 696f 643e 0a20 203c 7379 3a75  ePeriod>.  <sy:u
-000013b0: 7064 6174 6546 7265 7175 656e 6379 3e31  pdateFrequency>1
-000013c0: 3c2f 7379 3a75 7064 6174 6546 7265 7175  </sy:updateFrequ
-000013d0: 656e 6379 3e0a 0a20 203c 696d 6167 653e  ency>..  <image>
-000013e0: 0a20 2020 3c75 726c 3e7b 7b20 636f 6e66  .   <url>{{ conf
-000013f0: 6967 2e67 6574 2827 7572 6c27 2920 7d7d  ig.get('url') }}
-00001400: 2f7b 7b20 636f 6e66 6967 2e67 6574 2827  /{{ config.get('
-00001410: 7068 7427 2920 7d7d 3c2f 7572 6c3e 0a20  pht') }}</url>. 
-00001420: 2020 3c74 6974 6c65 3e7b 7b20 7469 746c    <title>{{ titl
-00001430: 6520 7d7d 3c2f 7469 746c 653e 0a20 2020  e }}</title>.   
-00001440: 3c6c 696e 6b3e 7b7b 2075 726c 207d 7d3c  <link>{{ url }}<
-00001450: 2f6c 696e 6b3e 0a20 2020 3c77 6964 7468  /link>.   <width
-00001460: 3e33 323c 2f77 6964 7468 3e0a 2020 203c  >32</width>.   <
-00001470: 6865 6967 6874 3e33 323c 2f68 6569 6768  height>32</heigh
-00001480: 743e 0a20 203c 2f69 6d61 6765 3e0a 0a20  t>.  </image>.. 
-00001490: 207b 2520 666f 7220 706f 7374 2069 6e20   {% for post in 
-000014a0: 706f 7374 7320 257d 7b25 2069 6620 2870  posts %}{% if (p
-000014b0: 6f73 742e 7368 6f77 496e 486f 6d65 2069  ost.showInHome i
-000014c0: 7320 756e 6465 6669 6e65 6429 206f 7220  s undefined) or 
-000014d0: 706f 7374 2e73 686f 7749 6e48 6f6d 6520  post.showInHome 
-000014e0: 257d 0a20 203c 6974 656d 3e0a 2020 203c  %}.  <item>.   <
-000014f0: 7469 746c 653e 7b7b 2070 6f73 742e 7469  title>{{ post.ti
-00001500: 746c 6520 7d7d 3c2f 7469 746c 653e 0a20  tle }}</title>. 
-00001510: 2020 3c6c 696e 6b3e 7b7b 2063 6f6e 6669    <link>{{ confi
-00001520: 672e 6765 7428 2775 726c 2729 207d 7d7b  g.get('url') }}{
-00001530: 7b20 706f 7374 2e75 726c 207d 7d3c 2f6c  { post.url }}</l
-00001540: 696e 6b3e 0a20 2020 3c70 7562 4461 7465  ink>.   <pubDate
-00001550: 3e7b 7b20 706f 7374 2e64 6174 652e 7374  >{{ post.date.st
-00001560: 7266 7469 6d65 2827 2561 2c20 2564 2025  rftime('%a, %d %
-00001570: 6220 2559 2025 483a 254d 3a25 5320 255a  b %Y %H:%M:%S %Z
-00001580: 2047 4d54 2729 207d 7d3c 2f70 7562 4461   GMT') }}</pubDa
-00001590: 7465 3e0a 2020 203c 6775 6964 2069 7350  te>.   <guid isP
-000015a0: 6572 6d61 4c69 6e6b 3d22 6661 6c73 6522  ermaLink="false"
-000015b0: 3e7b 7b20 636f 6e66 6967 2e67 6574 2827  >{{ config.get('
-000015c0: 7572 6c27 2920 7d7d 7b7b 2070 6f73 742e  url') }}{{ post.
-000015d0: 7572 6c20 7d7d 3c2f 6775 6964 3e0a 0909  url }}</guid>...
-000015e0: 093c 6465 7363 7269 7074 696f 6e3e 3c21  .<description><!
-000015f0: 5b43 4441 5441 5b7b 7b20 706f 7374 2e73  [CDATA[{{ post.s
-00001600: 7562 7469 746c 6520 7d7d 202d 207b 7b20  ubtitle }} - {{ 
-00001610: 706f 7374 2e6e 6f74 6520 7d7d 205d 5d3e  post.note }} ]]>
-00001620: 3c2f 6465 7363 7269 7074 696f 6e3e 0a20  </description>. 
-00001630: 203c 2f69 7465 6d3e 0a20 207b 2520 656e   </item>.  {% en
-00001640: 6469 6620 257d 7b25 2065 6e64 666f 7220  dif %}{% endfor 
-00001650: 257d 0a20 3c2f 6368 616e 6e65 6c3e 0a20  %}. </channel>. 
-00001660: 2020 2020 2020 2020 2020 2022 2222 290a             """).
-00001670: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-00001680: 636f 6e66 5f64 6174 6129 0a20 2020 2020  conf_data).     
-00001690: 2020 2070 7269 6e74 2827 7273 7320 7465     print('rss te
-000016a0: 6d70 6c61 7465 2063 7265 6174 6564 2e27  mplate created.'
-000016b0: 290a 2020 2020 2020 2020 662e 636c 6f73  ).        f.clos
-000016c0: 6528 290a 0a0a 6465 6620 6372 6561 7465  e()...def create
-000016d0: 436f 6e74 656e 7428 7069 6467 6579 4e61  Content(pidgeyNa
-000016e0: 6d65 293a 0a20 2020 2077 6974 6820 6f70  me):.    with op
-000016f0: 656e 2870 6174 682e 6a6f 696e 2870 6964  en(path.join(pid
-00001700: 6765 794e 616d 652c 2763 6f6e 7465 6e74  geyName,'content
-00001710: 272c 2768 6561 6465 722e 6d64 2729 2c27  ','header.md'),'
-00001720: 7727 2920 6173 2066 3a0a 2020 2020 2020  w') as f:.      
-00001730: 2020 636f 6e66 5f64 6174 6120 3d20 280a    conf_data = (.
-00001740: 2020 2020 2020 2020 2020 2020 2222 222a              """*
-00001750: 2020 205b 486f 6d65 5d28 2f29 0a2a 2020     [Home](/).*  
-00001760: 205b 4f74 6865 7220 4c69 6e6b 735d 282f   [Other Links](/
-00001770: 290a 2a20 2020 5b45 6469 7420 636f 6e74  ).*   [Edit cont
-00001780: 656e 742f 6865 6164 6572 2e6d 645d 282f  ent/header.md](/
-00001790: 290a 2020 2020 2020 2020 2020 2020 2222  ).            ""
-000017a0: 2229 0a20 2020 2020 2020 2066 2e77 7269  ").        f.wri
-000017b0: 7465 2863 6f6e 665f 6461 7461 290a 2020  te(conf_data).  
-000017c0: 2020 2020 2020 7072 696e 7428 2768 6561        print('hea
-000017d0: 6465 7220 6372 6561 7465 642e 2729 0a0a  der created.')..
-000017e0: 2020 2020 7769 7468 206f 7065 6e28 7061      with open(pa
-000017f0: 7468 2e6a 6f69 6e28 7069 6467 6579 4e61  th.join(pidgeyNa
-00001800: 6d65 2c27 636f 6e74 656e 7427 2c27 666f  me,'content','fo
-00001810: 6f74 6572 2e6d 6427 292c 2777 2729 2061  oter.md'),'w') a
-00001820: 7320 663a 0a20 2020 2020 2020 2063 6f6e  s f:.        con
-00001830: 665f 6461 7461 203d 2028 0a20 2020 2020  f_data = (.     
-00001840: 2020 2020 2020 2022 2222 2a20 2020 5b48         """*   [H
-00001850: 6f6d 655d 282f 290a 2a20 2020 5b52 5353  ome](/).*   [RSS
-00001860: 5d28 2f29 0a2a 2020 205b 4564 6974 2063  ](/).*   [Edit c
-00001870: 6f6e 7465 6e74 2f66 6f6f 7465 722e 6d64  ontent/footer.md
-00001880: 5d28 2f29 0a2a 2020 2070 6f77 6572 6564  ](/).*   powered
-00001890: 2062 7920 5b50 6964 6765 6f74 746f 5d28   by [Pidgeotto](
-000018a0: 2f29 0a20 2020 2020 2020 2020 2020 2022  /).            "
-000018b0: 2222 290a 2020 2020 2020 2020 662e 7772  "").        f.wr
-000018c0: 6974 6528 636f 6e66 5f64 6174 6129 0a20  ite(conf_data). 
-000018d0: 2020 2020 2020 2070 7269 6e74 2827 666f         print('fo
-000018e0: 6f74 6572 2063 7265 6174 6564 2e27 290a  oter created.').
-000018f0: 0a20 2020 2077 6974 6820 6f70 656e 2870  .    with open(p
-00001900: 6174 682e 6a6f 696e 2870 6964 6765 794e  ath.join(pidgeyN
-00001910: 616d 652c 2763 6f6e 7465 6e74 272c 2768  ame,'content','h
-00001920: 6f6d 652e 6d64 2729 2c27 7727 2920 6173  ome.md'),'w') as
-00001930: 2066 3a0a 2020 2020 2020 2020 636f 6e66   f:.        conf
-00001940: 5f64 6174 6120 3d20 280a 2020 2020 2020  _data = (.      
-00001950: 2020 2020 2020 2222 2257 656c 636f 6d65        """Welcome
-00001960: 2074 6f20 5069 6467 656f 7474 6f2e 0a3c   to Pidgeotto..<
-00001970: 6272 3e20 5468 6973 2069 7320 6120 7361  br> This is a sa
-00001980: 6d70 6c65 2068 6f6d 6570 6167 6520 7768  mple homepage wh
-00001990: 6963 6820 6361 6e20 6265 2065 6469 7465  ich can be edite
-000019a0: 6420 6174 202f 636f 6e74 656e 742f 686f  d at /content/ho
-000019b0: 6d65 2e6d 640a 0a2a 2a20 5069 6467 656f  me.md..** Pidgeo
-000019c0: 7474 6f20 6c69 6e6b 733a 202a 2a0a 2a20  tto links: **.* 
-000019d0: 2020 5b44 6f63 756d 656e 7461 7469 6f6e    [Documentation
-000019e0: 5d28 2f29 2e0a 2a20 2020 5b47 6974 6875  ](/)..*   [Githu
-000019f0: 6220 536f 7572 6365 5d28 2f29 2e0a 2020  b Source](/)..  
-00001a00: 2020 2020 2020 2222 2229 0a20 2020 2020        """).     
-00001a10: 2020 2066 2e77 7269 7465 2863 6f6e 665f     f.write(conf_
-00001a20: 6461 7461 290a 2020 2020 2020 2020 7072  data).        pr
-00001a30: 696e 7428 2766 6f6f 7465 7220 6372 6561  int('footer crea
-00001a40: 7465 642e 2729 0a20 2020 200a 2020 2020  ted.').    .    
-00001a50: 7769 7468 206f 7065 6e28 7061 7468 2e6a  with open(path.j
-00001a60: 6f69 6e28 7069 6467 6579 4e61 6d65 2c27  oin(pidgeyName,'
-00001a70: 636f 6e74 656e 7427 2c27 6e6f 7465 272c  content','note',
-00001a80: 2762 6c6f 6731 2e6d 6427 292c 2777 2729  'blog1.md'),'w')
-00001a90: 2061 7320 663a 0a20 2020 2020 2020 2063   as f:.        c
-00001aa0: 6f6e 665f 6461 7461 203d 2028 0a20 2020  onf_data = (.   
-00001ab0: 2020 2020 2020 2020 2022 2222 2d2d 2d0a           """---.
-00001ac0: 7469 746c 6520 3a20 2253 616d 706c 6520  title : "Sample 
-00001ad0: 426c 6f67 2e22 0a73 7562 7469 746c 6520  Blog.".subtitle 
-00001ae0: 3a20 2253 616d 706c 6520 7375 6274 6974  : "Sample subtit
-00001af0: 6c65 220a 6461 7465 203a 207b 747d 0a2d  le".date : {t}.-
-00001b00: 2d2d 0a0a 2320 5468 6973 2069 7320 6120  --..# This is a 
-00001b10: 7361 6d70 6c65 206e 6f74 6520 7061 6765  sample note page
-00001b20: 2077 6869 6368 2063 616e 2062 6520 6564   which can be ed
-00001b30: 6974 6564 2f72 656e 616d 6564 2061 7420  ited/renamed at 
-00001b40: 2f63 6f6e 7465 6e74 2f6e 6f74 652f 626c  /content/note/bl
-00001b50: 6f67 312e 6d64 0a23 2054 6869 7320 6973  og1.md.# This is
-00001b60: 2068 6561 6469 6e67 2031 0a0a 2323 2054   heading 1..## T
-00001b70: 6869 7320 6973 2068 6561 6469 6e67 2032  his is heading 2
-00001b80: 0a0a 2323 2320 5468 6973 2069 7320 6865  ..### This is he
-00001b90: 6164 696e 6720 330a 0a23 2323 2320 5468  ading 3..#### Th
-00001ba0: 6973 2069 7320 6865 6164 696e 6720 340a  is is heading 4.
-00001bb0: 0a23 2323 2323 2054 6869 7320 6973 2068  .##### This is h
-00001bc0: 6561 6469 6e67 2035 0a0a 2323 2323 2323  eading 5..######
-00001bd0: 2054 6869 7320 6973 2068 6561 6469 6e67   This is heading
-00001be0: 2036 0a0a 2a2a 426f 6c64 2a2a 0a0a 2a69   6..**Bold**..*i
-00001bf0: 7461 6c69 632a 0a0a 2a20 6c69 7374 0a2a  talic*..* list.*
-00001c00: 206c 6973 740a 0a31 2e20 6f72 6465 7265   list..1. ordere
-00001c10: 6420 6c69 7374 0a32 2e20 6f72 6465 7265  d list.2. ordere
-00001c20: 6420 6c69 7374 0a0a 5b6c 696e 6b5d 282f  d list..[link](/
-00001c30: 290a 0a53 616d 706c 6520 7061 7261 6772  )..Sample paragr
-00001c40: 6170 6820 6973 2077 7269 7474 656e 206c  aph is written l
-00001c50: 696b 6520 7468 6973 2077 6974 6820 6c6f  ike this with lo
-00001c60: 7265 6d20 6970 7375 6d2e 204c 6f72 656d  rem ipsum. Lorem
-00001c70: 2069 7073 756d 2064 6f6c 6f72 2073 6974   ipsum dolor sit
-00001c80: 2061 6d65 742c 2063 6f6e 7365 6374 6574   amet, consectet
-00001c90: 7572 2061 6469 7069 7363 696e 6720 656c  ur adipiscing el
-00001ca0: 6974 2c20 7365 6420 646f 2065 6975 736d  it, sed do eiusm
-00001cb0: 6f64 2074 656d 706f 7220 696e 6369 6469  od tempor incidi
-00001cc0: 6475 6e74 2075 7420 6c61 626f 7265 2065  dunt ut labore e
-00001cd0: 7420 646f 6c6f 7265 206d 6167 6e61 2061  t dolore magna a
-00001ce0: 6c69 7175 612e 2055 7420 656e 696d 2061  liqua. Ut enim a
-00001cf0: 6420 6d69 6e69 6d20 7665 6e69 616d 2c20  d minim veniam, 
-00001d00: 7175 6973 206e 6f73 7472 7564 2065 7865  quis nostrud exe
-00001d10: 7263 6974 6174 696f 6e20 756c 6c61 6d63  rcitation ullamc
-00001d20: 6f20 6c61 626f 7269 7320 6e69 7369 2075  o laboris nisi u
-00001d30: 7420 616c 6971 7569 7020 6578 2065 6120  t aliquip ex ea 
-00001d40: 636f 6d6d 6f64 6f20 636f 6e73 6571 7561  commodo consequa
-00001d50: 742e 2044 7569 7320 6175 7465 2069 7275  t. Duis aute iru
-00001d60: 7265 2064 6f6c 6f72 2069 6e20 7265 7072  re dolor in repr
-00001d70: 6568 656e 6465 7269 7420 696e 2076 6f6c  ehenderit in vol
-00001d80: 7570 7461 7465 2076 656c 6974 2065 7373  uptate velit ess
-00001d90: 6520 6369 6c6c 756d 2064 6f6c 6f72 6520  e cillum dolore 
-00001da0: 6575 2066 7567 6961 7420 6e75 6c6c 6120  eu fugiat nulla 
-00001db0: 7061 7269 6174 7572 2e20 4578 6365 7074  pariatur. Except
-00001dc0: 6575 7220 7369 6e74 206f 6363 6165 6361  eur sint occaeca
-00001dd0: 7420 6375 7069 6461 7461 7420 6e6f 6e20  t cupidatat non 
-00001de0: 7072 6f69 6465 6e74 2c20 7375 6e74 2069  proident, sunt i
-00001df0: 6e20 6375 6c70 6120 7175 6920 6f66 6669  n culpa qui offi
-00001e00: 6369 6120 6465 7365 7275 6e74 206d 6f6c  cia deserunt mol
-00001e10: 6c69 7420 616e 696d 2069 6420 6573 7420  lit anim id est 
-00001e20: 6c61 626f 7275 6d2e 0a20 2020 2020 2020  laborum..       
-00001e30: 2022 2222 292e 666f 726d 6174 2874 3d64   """).format(t=d
-00001e40: 6174 6574 696d 652e 6e6f 7728 292e 7374  atetime.now().st
-00001e50: 7266 7469 6d65 2822 2559 2d25 6d2d 2564  rftime("%Y-%m-%d
-00001e60: 2229 290a 2020 2020 2020 2020 662e 7772  ")).        f.wr
-00001e70: 6974 6528 636f 6e66 5f64 6174 6129 0a20  ite(conf_data). 
-00001e80: 2020 2020 2020 2070 7269 6e74 2827 7361         print('sa
-00001e90: 6d70 6c65 2062 6c6f 6720 6372 6561 7465  mple blog create
-00001ea0: 642e 2729 0a0a 0a64 6566 2063 7265 6174  d.')...def creat
-00001eb0: 6550 6964 6765 7928 7069 6467 6579 4e61  ePidgey(pidgeyNa
-00001ec0: 6d65 293a 0a20 2020 2074 7279 3a0a 2020  me):.    try:.  
-00001ed0: 2020 2020 2020 6d6b 6469 7228 7069 6467        mkdir(pidg
-00001ee0: 6579 4e61 6d65 290a 2020 2020 2020 2020  eyName).        
-00001ef0: 7072 696e 7428 2270 6964 6765 7920 2220  print("pidgey " 
-00001f00: 2b20 7069 6467 6579 4e61 6d65 202b 2022  + pidgeyName + "
-00001f10: 2063 7265 6174 6564 2e22 290a 2020 2020   created.").    
-00001f20: 2020 2020 6d6b 6469 7228 7061 7468 2e6a      mkdir(path.j
-00001f30: 6f69 6e28 7069 6467 6579 4e61 6d65 2c27  oin(pidgeyName,'
-00001f40: 7465 6d70 6c61 7465 2729 290a 2020 2020  template')).    
-00001f50: 2020 2020 6d6b 6469 7228 7061 7468 2e6a      mkdir(path.j
-00001f60: 6f69 6e28 7069 6467 6579 4e61 6d65 2c27  oin(pidgeyName,'
-00001f70: 7374 6174 6963 2729 290a 2020 2020 2020  static')).      
-00001f80: 2020 6d6b 6469 7228 7061 7468 2e6a 6f69    mkdir(path.joi
-00001f90: 6e28 7069 6467 6579 4e61 6d65 2c27 636f  n(pidgeyName,'co
-00001fa0: 6e74 656e 7427 2929 0a20 2020 2020 2020  ntent')).       
-00001fb0: 206d 6b64 6972 2870 6174 682e 6a6f 696e   mkdir(path.join
-00001fc0: 2870 6964 6765 794e 616d 652c 2763 6f6e  (pidgeyName,'con
-00001fd0: 7465 6e74 272c 276e 6f74 6527 2929 0a20  tent','note')). 
-00001fe0: 2020 2020 2020 2063 7265 6174 6543 6f6e         createCon
-00001ff0: 6669 6728 7069 6467 6579 4e61 6d65 290a  fig(pidgeyName).
-00002000: 2020 2020 2020 2020 6372 6561 7465 5465          createTe
-00002010: 6d70 6c61 7465 7328 7069 6467 6579 4e61  mplates(pidgeyNa
-00002020: 6d65 290a 2020 2020 2020 2020 6372 6561  me).        crea
-00002030: 7465 436f 6e74 656e 7428 7069 6467 6579  teContent(pidgey
-00002040: 4e61 6d65 290a 2020 2020 6578 6365 7074  Name).    except
-00002050: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
-00002060: 2277 6869 6c65 2067 656e 6572 6174 696e  "while generatin
-00002070: 6720 7069 6467 6579 2022 2b20 7069 6467  g pidgey "+ pidg
-00002080: 6579 4e61 6d65 202b 2022 2c20 736f 6d65  eyName + ", some
-00002090: 2069 7373 7565 206f 6363 7572 6564 2e22   issue occured."
-000020a0: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
-000020b0: 2254 6869 7320 6361 6e20 6265 2064 7565  "This can be due
-000020c0: 2074 6f20 5c6e 5c74 312e 2050 6964 6765   to \n\t1. Pidge
-000020d0: 7920 616c 7265 6164 7920 6578 6973 7473  y already exists
-000020e0: 2e5c 6e5c 7432 2e20 4d65 6d6f 7279 2069  .\n\t2. Memory i
-000020f0: 7373 7565 2e5c 6e5c 7433 2e20 496e 7661  ssue.\n\t3. Inva
-00002100: 6c69 6420 696e 7075 742e 5c6e 5c74 342e  lid input.\n\t4.
-00002110: 2049 6620 6e6f 6e65 206f 6620 7468 6573   If none of thes
-00002120: 652c 2072 6570 6f72 7420 746f 2064 6576  e, report to dev
-00002130: 656c 6f70 6572 2e22 290a 0a64 6566 2063  eloper.")..def c
-00002140: 7265 6174 654e 6f74 6528 6e6f 7465 4e61  reateNote(noteNa
-00002150: 6d65 2c20 7368 6f77 496e 486f 6d65 3d54  me, showInHome=T
-00002160: 7275 6529 3a0a 2020 2020 7472 793a 0a20  rue):.    try:. 
-00002170: 2020 2020 2020 2069 6620 6e6f 7420 6e6f         if not no
-00002180: 7465 4e61 6d65 2e6c 6f77 6572 2829 2e65  teName.lower().e
-00002190: 6e64 7377 6974 6828 272e 6d64 2729 3a0a  ndswith('.md'):.
-000021a0: 2020 2020 2020 2020 2020 2020 6e6f 7465              note
-000021b0: 4e61 6d65 2b3d 272e 6d64 270a 2020 2020  Name+='.md'.    
-000021c0: 2020 2020 7769 7468 206f 7065 6e28 7061      with open(pa
-000021d0: 7468 2e6a 6f69 6e28 2763 6f6e 7465 6e74  th.join('content
-000021e0: 272c 276e 6f74 6527 2c6e 6f74 654e 616d  ','note',noteNam
-000021f0: 6529 2c27 7727 2920 6173 2066 3a0a 2020  e),'w') as f:.  
-00002200: 2020 2020 2020 2020 2020 636f 6e66 5f64            conf_d
-00002210: 6174 6120 3d20 280a 2020 2020 2020 2020  ata = (.        
-00002220: 2020 2020 2222 222d 2d2d 0a74 6974 6c65      """---.title
-00002230: 203a 2022 5469 746c 6522 0a73 7562 7469   : "Title".subti
-00002240: 746c 6520 3a20 2253 7562 7469 746c 6522  tle : "Subtitle"
-00002250: 0a73 686f 7749 6e48 6f6d 6520 3a20 7b73  .showInHome : {s
-00002260: 7d0a 6461 7465 203a 207b 747d 0a2d 2d2d  }.date : {t}.---
-00002270: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
-00002280: 292e 666f 726d 6174 2874 3d64 6174 6574  ).format(t=datet
-00002290: 696d 652e 6e6f 7728 292e 7374 7266 7469  ime.now().strfti
-000022a0: 6d65 2822 2559 2d25 6d2d 2564 2229 2c20  me("%Y-%m-%d"), 
-000022b0: 733d 7368 6f77 496e 486f 6d65 290a 2020  s=showInHome).  
-000022c0: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
-000022d0: 6528 636f 6e66 5f64 6174 6129 0a20 2020  e(conf_data).   
-000022e0: 2020 2020 2020 2020 2070 7269 6e74 286e           print(n
-000022f0: 6f74 654e 616d 652b 2220 6973 2063 7265  oteName+" is cre
-00002300: 6174 6564 2061 7420 636f 6e74 656e 742f  ated at content/
-00002310: 6e6f 7465 2f22 2b6e 6f74 654e 616d 6520  note/"+noteName 
-00002320: 290a 2020 2020 6578 6365 7074 3a0a 2020  ).    except:.  
-00002330: 2020 2020 2020 7072 696e 7428 2277 6869        print("whi
-00002340: 6c65 2067 656e 6572 6174 696e 6720 7061  le generating pa
-00002350: 6765 2022 2b6e 6f74 654e 616d 652b 222c  ge "+noteName+",
-00002360: 2073 6f6d 6520 6973 7375 6520 6f63 6375   some issue occu
-00002370: 7265 642e 2229 0a20 2020 2020 2020 2070  red.").        p
-00002380: 7269 6e74 2822 5468 6973 2063 616e 2062  rint("This can b
-00002390: 6520 6475 6520 746f 205c 6e5c 7431 2e20  e due to \n\t1. 
-000023a0: 4e6f 7420 6120 7069 6467 6579 2064 6972  Not a pidgey dir
-000023b0: 6563 746f 7279 2e20 5c6e 5c74 322e 2049  ectory. \n\t2. I
-000023c0: 6e76 616c 6964 2066 696c 656e 616d 6522  nvalid filename"
-000023d0: 290a                                     ).
+00000000: 2321 2f62 696e 2f70 7974 686f 6e33 0d0a  #!/bin/python3..
+00000010: 0d0a 230d 0a23 2020 2020 2020 20e2 9688  ..#..#       ...
+00000020: e296 88e2 9688 e295 9720 2020 e296 88e2  .........   ....
+00000030: 9688 e295 97e2 9688 e296 88e2 9597 e296  ................
+00000040: 88e2 9688 e295 9720 20e2 9688 e296 88e2  .......  .......
+00000050: 9597 20e2 9688 e296 88e2 9688 e296 88e2  .. .............
+00000060: 9688 e295 9720 e296 88e2 9688 e296 88e2  ..... ..........
+00000070: 9688 e296 88e2 9688 e295 9720 e296 88e2  ........... ....
+00000080: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
+00000090: 88e2 9597 0d0a 2320 2020 2020 2020 e296  ......#       ..
+000000a0: 88e2 9688 e296 88e2 9688 e295 9720 20e2  .............  .
+000000b0: 9688 e296 88e2 9591 e296 88e2 9688 e295  ................
+000000c0: 91e2 9688 e296 88e2 9591 2020 e296 88e2  ..........  ....
+000000d0: 9688 e295 91e2 9688 e296 88e2 9594 e295  ................
+000000e0: 90e2 9590 e296 88e2 9688 e295 97e2 9688  ................
+000000f0: e296 88e2 9594 e295 90e2 9590 e296 88e2  ................
+00000100: 9688 e295 97e2 9688 e296 88e2 9594 e295  ................
+00000110: 90e2 9590 e295 90e2 9590 e295 9d0d 0a23  ...............#
+00000120: 2020 2020 2020 20e2 9688 e296 88e2 9594         .........
+00000130: e296 88e2 9688 e295 9720 e296 88e2 9688  ......... ......
+00000140: e295 91e2 9688 e296 88e2 9591 e296 88e2  ................
+00000150: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
+00000160: 88e2 9591 e296 88e2 9688 e296 88e2 9688  ................
+00000170: e296 88e2 9688 e296 88e2 9591 e296 88e2  ................
+00000180: 9688 e296 88e2 9688 e296 88e2 9688 e295  ................
+00000190: 94e2 959d e296 88e2 9688 e296 88e2 9688  ................
+000001a0: e296 88e2 9688 e296 88e2 9597 0d0a 2320  ..............# 
+000001b0: 2020 2020 2020 e296 88e2 9688 e295 91e2        ..........
+000001c0: 959a e296 88e2 9688 e295 97e2 9688 e296  ................
+000001d0: 88e2 9591 e296 88e2 9688 e295 91e2 9688  ................
+000001e0: e296 88e2 9594 e295 90e2 9590 e296 88e2  ................
+000001f0: 9688 e295 91e2 9688 e296 88e2 9594 e295  ................
+00000200: 90e2 9590 e296 88e2 9688 e295 91e2 9688  ................
+00000210: e296 88e2 9594 e295 90e2 9590 e296 88e2  ................
+00000220: 9688 e295 97e2 959a e295 90e2 9590 e295  ................
+00000230: 90e2 9590 e296 88e2 9688 e295 910d 0a23  ...............#
+00000240: 2020 2020 2020 20e2 9688 e296 88e2 9591         .........
+00000250: 20e2 959a e296 88e2 9688 e296 88e2 9688   ...............
+00000260: e295 91e2 9688 e296 88e2 9591 e296 88e2  ................
+00000270: 9688 e295 9120 20e2 9688 e296 88e2 9591  .....  .........
+00000280: e296 88e2 9688 e295 9120 20e2 9688 e296  .........  .....
+00000290: 88e2 9591 e296 88e2 9688 e295 9120 20e2  .............  .
+000002a0: 9688 e296 88e2 9591 e296 88e2 9688 e296  ................
+000002b0: 88e2 9688 e296 88e2 9688 e296 88e2 9591  ................
+000002c0: 0d0a 2320 2020 2020 2020 e295 9ae2 9590  ..#       ......
+000002d0: e295 9d20 20e2 959a e295 90e2 9590 e295  ...  ...........
+000002e0: 90e2 959d e295 9ae2 9590 e295 9de2 959a  ................
+000002f0: e295 90e2 959d 2020 e295 9ae2 9590 e295  ......  ........
+00000300: 9de2 959a e295 90e2 959d 2020 e295 9ae2  ..........  ....
+00000310: 9590 e295 9de2 959a e295 90e2 959d 2020  ..............  
+00000320: e295 9ae2 9590 e295 9de2 959a e295 90e2  ................
+00000330: 9590 e295 90e2 9590 e295 90e2 9590 e295  ................
+00000340: 9d0d 0a23 2020 2020 2020 2044 5241 4654  ...#       DRAFT
+00000350: 4544 2042 5920 5b68 7474 7073 3a2f 2f6e  ED BY [https://n
+00000360: 6968 2e61 725d 204f 4e20 3138 2d30 342d  ih.ar] ON 18-04-
+00000370: 3230 3231 2e0d 0a23 2020 2020 2020 2053  2021...#       S
+00000380: 4f55 5243 4520 5b63 7265 6174 6f72 2e70  OURCE [creator.p
+00000390: 795d 204c 4153 5420 4d4f 4449 4649 4544  y] LAST MODIFIED
+000003a0: 204f 4e20 3235 2d30 362d 3230 3233 2e0d   ON 25-06-2023..
+000003b0: 0a23 0d0a 0d0a 0d0a 6672 6f6d 206f 7320  .#......from os 
+000003c0: 696d 706f 7274 206d 6b64 6972 2c20 7061  import mkdir, pa
+000003d0: 7468 0d0a 6672 6f6d 2064 6174 6574 696d  th..from datetim
+000003e0: 6520 696d 706f 7274 2064 6174 6574 696d  e import datetim
+000003f0: 650d 0a0d 0a0d 0a64 6566 2063 7265 6174  e......def creat
+00000400: 6543 6f6e 6669 6728 7069 6467 6579 4e61  eConfig(pidgeyNa
+00000410: 6d65 293a 0d0a 2020 2020 7769 7468 206f  me):..    with o
+00000420: 7065 6e28 7061 7468 2e6a 6f69 6e28 7069  pen(path.join(pi
+00000430: 6467 6579 4e61 6d65 2c27 636f 6e66 6967  dgeyName,'config
+00000440: 2e79 6d6c 2729 2c27 7727 2920 6173 2066  .yml'),'w') as f
+00000450: 3a0d 0a20 2020 2020 2020 2063 6f6e 665f  :..        conf_
+00000460: 6461 7461 203d 2028 0d0a 2020 2020 2020  data = (..      
+00000470: 2020 2020 2020 2222 2223 204d 616e 6461        """# Manda
+00000480: 746f 7279 2043 6f6e 6669 6775 7261 7469  tory Configurati
+00000490: 6f6e 0d0a 7469 746c 6520 3a20 4465 6d6f  on..title : Demo
+000004a0: 2070 6964 6765 6f74 746f 2077 6562 7369   pidgeotto websi
+000004b0: 7465 0d0a 7572 6c20 3a20 796f 7572 646f  te..url : yourdo
+000004c0: 6d61 696e 2e74 6c64 0d0a 6e6f 7465 5f74  main.tld..note_t
+000004d0: 656d 706c 6174 6520 3a20 7465 6d70 6c61  emplate : templa
+000004e0: 7465 2f6e 6f74 655f 7465 6d70 6c61 7465  te/note_template
+000004f0: 2e68 746d 6c20 2020 2320 5465 6d70 6c61  .html   # Templa
+00000500: 7465 206f 6620 6e6f 7465 2070 6167 650d  te of note page.
+00000510: 0a68 6f6d 655f 7465 6d70 6c61 7465 203a  .home_template :
+00000520: 2074 656d 706c 6174 652f 686f 6d65 5f74   template/home_t
+00000530: 656d 706c 6174 652e 6874 6d6c 2020 2023  emplate.html   #
+00000540: 2054 656d 706c 6174 6520 6f66 2068 6f6d   Template of hom
+00000550: 6520 7061 6765 0d0a 6665 6564 5f74 656d  e page..feed_tem
+00000560: 706c 6174 6520 3a20 7465 6d70 6c61 7465  plate : template
+00000570: 2f66 6565 645f 7465 6d70 6c61 7465 2e78  /feed_template.x
+00000580: 6d6c 2020 2023 2054 656d 706c 6174 6520  ml   # Template 
+00000590: 6f66 2066 6565 642f 7273 7320 7061 6765  of feed/rss page
+000005a0: 0d0a 686f 6d65 5f70 6174 6820 3a20 7075  ..home_path : pu
+000005b0: 626c 6963 2020 2320 4166 7465 7220 6275  blic  # After bu
+000005c0: 696c 742c 2073 7461 7469 6320 6669 6c65  ilt, static file
+000005d0: 7320 7769 6c6c 2062 6520 6765 6e65 7261  s will be genera
+000005e0: 7465 6420 6865 7265 0d0a 636f 6e74 656e  ted here..conten
+000005f0: 745f 7061 7468 203a 2063 6f6e 7465 6e74  t_path : content
+00000600: 2023 2041 6c6c 2070 6f73 7420 6e6f 7465   # All post note
+00000610: 7320 6d61 726b 646f 776e 206c 6f63 6174  s markdown locat
+00000620: 696f 6e0d 0a72 6573 6f75 7263 655f 7061  ion..resource_pa
+00000630: 7468 203a 2073 7461 7469 6320 2320 416c  th : static # Al
+00000640: 6c20 6373 732c 206a 732c 2069 6d61 6765  l css, js, image
+00000650: 206c 6f63 6174 696f 6e0d 0a68 6f6d 655f   location..home_
+00000660: 6d64 203a 2063 6f6e 7465 6e74 2f68 6f6d  md : content/hom
+00000670: 652e 6d64 2023 2048 6f6d 6570 6167 6520  e.md # Homepage 
+00000680: 636f 6e74 656e 740d 0a68 6561 6465 725f  content..header_
+00000690: 6d64 203a 2063 6f6e 7465 6e74 2f68 6561  md : content/hea
+000006a0: 6465 722e 6d64 2023 2048 6561 6465 7220  der.md # Header 
+000006b0: 636f 6e74 656e 740d 0a66 6f6f 7465 725f  content..footer_
+000006c0: 6d64 203a 2063 6f6e 7465 6e74 2f66 6f6f  md : content/foo
+000006d0: 7465 722e 6d64 2023 2046 6f6f 7465 7220  ter.md # Footer 
+000006e0: 636f 6e74 656e 740d 0a0d 0a23 204f 7074  content....# Opt
+000006f0: 696f 6e61 6c20 436f 6e66 6967 7572 6174  ional Configurat
+00000700: 696f 6e2c 2041 6464 2079 6f75 7220 6f77  ion, Add your ow
+00000710: 6e20 636f 6e66 6967 7320 6865 7265 0d0a  n configs here..
+00000720: 7369 7465 2d74 6974 6c65 203a 2044 656d  site-title : Dem
+00000730: 6f20 5069 6467 656f 7474 6f0d 0a63 7373  o Pidgeotto..css
+00000740: 203a 2064 656d 6f2e 6373 730d 0a64 6573   : demo.css..des
+00000750: 6320 3a20 5772 6974 6520 616e 7974 6869  c : Write anythi
+00000760: 6e67 2074 6861 7420 6875 6d61 6e20 616e  ng that human an
+00000770: 6420 6d61 6368 696e 6520 6361 6e20 756e  d machine can un
+00000780: 6465 7273 7461 6e64 2e0d 0a6d 6169 6c20  derstand...mail 
+00000790: 3a20 736f 6d65 406d 6169 6c2e 636f 6d0d  : some@mail.com.
+000007a0: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
+000007b0: 290d 0a20 2020 2020 2020 2066 2e77 7269  )..        f.wri
+000007c0: 7465 2863 6f6e 665f 6461 7461 290d 0a20  te(conf_data).. 
+000007d0: 2020 2020 2020 2070 7269 6e74 2827 636f         print('co
+000007e0: 6e66 6967 2e79 6d6c 2063 7265 6174 6564  nfig.yml created
+000007f0: 2e27 290d 0a0d 0a0d 0a64 6566 2063 7265  .')......def cre
+00000800: 6174 6554 656d 706c 6174 6573 2870 6964  ateTemplates(pid
+00000810: 6765 794e 616d 6529 3a0d 0a20 2020 2077  geyName):..    w
+00000820: 6974 6820 6f70 656e 2870 6174 682e 6a6f  ith open(path.jo
+00000830: 696e 2870 6964 6765 794e 616d 652c 2774  in(pidgeyName,'t
+00000840: 656d 706c 6174 6527 2c27 686f 6d65 5f74  emplate','home_t
+00000850: 656d 706c 6174 652e 6874 6d6c 2729 2c27  emplate.html'),'
+00000860: 7727 2920 6173 2066 3a0d 0a20 2020 2020  w') as f:..     
+00000870: 2020 2063 6f6e 665f 6461 7461 203d 2028     conf_data = (
+00000880: 0d0a 2020 2020 2020 2020 2222 223c 2144  ..        """<!D
+00000890: 4f43 5459 5045 2068 746d 6c3e 0d0a 3c68  OCTYPE html>..<h
+000008a0: 746d 6c20 6c61 6e67 3d22 656e 2d49 4e22  tml lang="en-IN"
+000008b0: 2064 6174 612d 7468 656d 653d 2264 6172   data-theme="dar
+000008c0: 6b22 3e0d 0a0d 0a3c 6865 6164 3e0d 0a3c  k">....<head>..<
+000008d0: 6d65 7461 2063 6861 7273 6574 3d22 7574  meta charset="ut
+000008e0: 662d 3822 3e0d 0a3c 6d65 7461 2068 7474  f-8">..<meta htt
+000008f0: 702d 6571 7569 763d 2258 2d55 412d 436f  p-equiv="X-UA-Co
+00000900: 6d70 6174 6962 6c65 2220 636f 6e74 656e  mpatible" conten
+00000910: 743d 2249 453d 6564 6765 223e 0d0a 3c6d  t="IE=edge">..<m
+00000920: 6574 6120 6e61 6d65 3d22 7669 6577 706f  eta name="viewpo
+00000930: 7274 2220 636f 6e74 656e 743d 2277 6964  rt" content="wid
+00000940: 7468 3d64 6576 6963 652d 7769 6474 682c  th=device-width,
+00000950: 2069 6e69 7469 616c 2d73 6361 6c65 3d31   initial-scale=1
+00000960: 223e 0d0a 3c6d 6574 6120 6e61 6d65 3d22  ">..<meta name="
+00000970: 6465 7363 7269 7074 696f 6e22 2063 6f6e  description" con
+00000980: 7465 6e74 3d22 207b 7b20 636f 6e66 6967  tent=" {{ config
+00000990: 2e67 6574 2827 6465 7363 2729 207d 7d22  .get('desc') }}"
+000009a0: 3e0d 0a3c 7469 746c 653e 7b7b 2063 6f6e  >..<title>{{ con
+000009b0: 6669 672e 6765 7428 2773 6974 652d 7469  fig.get('site-ti
+000009c0: 746c 6527 2920 7d7d 3c2f 7469 746c 653e  tle') }}</title>
+000009d0: 0d0a 3c6c 696e 6b20 7265 6c3d 2273 7479  ..<link rel="sty
+000009e0: 6c65 7368 6565 7422 2074 7970 653d 2274  lesheet" type="t
+000009f0: 6578 742f 6373 7322 206d 6564 6961 3d22  ext/css" media="
+00000a00: 7363 7265 656e 2220 6872 6566 3d22 7b7b  screen" href="{{
+00000a10: 2063 6f6e 6669 672e 6765 7428 2763 7373   config.get('css
+00000a20: 2729 207d 7d22 202f 3e0d 0a3c 6c69 6e6b  ') }}" />..<link
+00000a30: 2072 656c 3d22 616c 7465 726e 6174 6522   rel="alternate"
+00000a40: 2074 7970 653d 2261 7070 6c69 6361 7469   type="applicati
+00000a50: 6f6e 2f61 746f 6d2b 786d 6c22 2074 6974  on/atom+xml" tit
+00000a60: 6c65 3d22 5265 6365 6e74 2062 6c6f 6720  le="Recent blog 
+00000a70: 706f 7374 7322 2068 7265 663d 222f 7273  posts" href="/rs
+00000a80: 732e 786d 6c22 3e0d 0a3c 2f68 6561 643e  s.xml">..</head>
+00000a90: 0d0a 0d0a 3c62 6f64 793e 0d0a 3c68 6561  ....<body>..<hea
+00000aa0: 6465 723e 0d0a 3c68 313e 3c61 2068 7265  der>..<h1><a hre
+00000ab0: 663d 222f 223e 7b25 2066 696c 7465 7220  f="/">{% filter 
+00000ac0: 6c6f 7765 7220 257d 207b 7b20 7469 746c  lower %} {{ titl
+00000ad0: 6520 7d7d 207b 2520 656e 6466 696c 7465  e }} {% endfilte
+00000ae0: 7220 257d 3c2f 613e 3c2f 6831 3e0d 0a7b  r %}</a></h1>..{
+00000af0: 7b20 6865 6164 6572 207d 7d0d 0a3c 2f68  { header }}..</h
+00000b00: 6561 6465 723e 0d0a 3c73 6563 7469 6f6e  eader>..<section
+00000b10: 3e0d 0a7b 7b61 7274 6963 6c65 7d7d 0d0a  >..{{article}}..
+00000b20: 3c75 6c3e 0d0a 7b25 2066 6f72 2070 6f73  <ul>..{% for pos
+00000b30: 7420 696e 2070 6f73 7473 2025 7d7b 2520  t in posts %}{% 
+00000b40: 6966 2028 706f 7374 2e73 686f 7749 6e48  if (post.showInH
+00000b50: 6f6d 6520 6973 2075 6e64 6566 696e 6564  ome is undefined
+00000b60: 2920 6f72 2070 6f73 742e 7368 6f77 496e  ) or post.showIn
+00000b70: 486f 6d65 2025 7d0d 0a3c 6c69 3e7b 7b20  Home %}..<li>{{ 
+00000b80: 706f 7374 2e64 6174 652e 7374 7266 7469  post.date.strfti
+00000b90: 6d65 2827 2564 2025 6d20 2559 2729 207d  me('%d %m %Y') }
+00000ba0: 7d20 3b20 3c61 2068 7265 663d 227b 7b20  } ; <a href="{{ 
+00000bb0: 706f 7374 2e75 726c 207d 7d22 3e7b 2520  post.url }}">{% 
+00000bc0: 6669 6c74 6572 206c 6f77 6572 2025 7d20  filter lower %} 
+00000bd0: 7b7b 2070 6f73 742e 7469 746c 6520 7d7d  {{ post.title }}
+00000be0: 207b 2520 656e 6466 696c 7465 7220 257d   {% endfilter %}
+00000bf0: 3c2f 613e 3c2f 6c69 3e0d 0a7b 2520 656e  </a></li>..{% en
+00000c00: 6469 6620 257d 7b25 2065 6e64 666f 7220  dif %}{% endfor 
+00000c10: 257d 0d0a 7b25 2069 6620 6e65 7874 7061  %}..{% if nextpa
+00000c20: 6765 2025 7d20 3c61 2068 7265 663d 227b  ge %} <a href="{
+00000c30: 7b20 6e65 7874 7061 6765 207d 7d22 3e4f  { nextpage }}">O
+00000c40: 6c64 6572 204e 6f74 6573 203e 3e20 3c2f  lder Notes >> </
+00000c50: 613e 207b 2520 656e 6469 6620 257d 0d0a  a> {% endif %}..
+00000c60: 3c2f 756c 3e0d 0a3c 2f73 6563 7469 6f6e  </ul>..</section
+00000c70: 3e0d 0a3c 666f 6f74 6572 3e0d 0a7b 7b20  >..<footer>..{{ 
+00000c80: 666f 6f74 6572 207d 7d0d 0a3c 2f66 6f6f  footer }}..</foo
+00000c90: 7465 723e 0d0a 3c2f 626f 6479 3e0d 0a3c  ter>..</body>..<
+00000ca0: 2f68 746d 6c3e 0d0a 2020 2020 2020 2020  /html>..        
+00000cb0: 2020 2020 2222 2229 0d0a 2020 2020 2020      """)..      
+00000cc0: 2020 662e 7772 6974 6528 636f 6e66 5f64    f.write(conf_d
+00000cd0: 6174 6129 0d0a 2020 2020 2020 2020 7072  ata)..        pr
+00000ce0: 696e 7428 2768 6f6d 655f 7465 6d70 6c61  int('home_templa
+00000cf0: 7465 2063 7265 6174 6564 2e27 290d 0a0d  te created.')...
+00000d00: 0a20 2020 2077 6974 6820 6f70 656e 2870  .    with open(p
+00000d10: 6174 682e 6a6f 696e 2870 6964 6765 794e  ath.join(pidgeyN
+00000d20: 616d 652c 2774 656d 706c 6174 6527 2c27  ame,'template','
+00000d30: 6e6f 7465 5f74 656d 706c 6174 652e 6874  note_template.ht
+00000d40: 6d6c 2729 2c27 7727 2920 6173 2066 3a0d  ml'),'w') as f:.
+00000d50: 0a20 2020 2020 2020 2063 6f6e 665f 6461  .        conf_da
+00000d60: 7461 203d 2028 0d0a 2020 2020 2020 2020  ta = (..        
+00000d70: 2020 2020 2222 223c 2144 4f43 5459 5045      """<!DOCTYPE
+00000d80: 2068 746d 6c3e 0d0a 3c68 746d 6c20 6c61   html>..<html la
+00000d90: 6e67 3d22 656e 2220 6461 7461 2d74 6865  ng="en" data-the
+00000da0: 6d65 3d22 6461 726b 223e 0d0a 3c68 6561  me="dark">..<hea
+00000db0: 643e 0d0a 3c6d 6574 6120 6368 6172 7365  d>..<meta charse
+00000dc0: 743d 2275 7466 2d38 223e 0d0a 0d0a 3c74  t="utf-8">....<t
+00000dd0: 6974 6c65 3e7b 7b20 706f 7374 5f74 6974  itle>{{ post_tit
+00000de0: 6c65 207d 7d3c 2f74 6974 6c65 3e0d 0a0d  le }}</title>...
+00000df0: 0a3c 6d65 7461 2068 7474 702d 6571 7569  .<meta http-equi
+00000e00: 763d 2258 2d55 412d 436f 6d70 6174 6962  v="X-UA-Compatib
+00000e10: 6c65 2220 636f 6e74 656e 743d 2249 453d  le" content="IE=
+00000e20: 6564 6765 223e 0d0a 3c6d 6574 6120 6e61  edge">..<meta na
+00000e30: 6d65 3d22 7669 6577 706f 7274 2220 636f  me="viewport" co
+00000e40: 6e74 656e 743d 2277 6964 7468 3d64 6576  ntent="width=dev
+00000e50: 6963 652d 7769 6474 682c 2069 6e69 7469  ice-width, initi
+00000e60: 616c 2d73 6361 6c65 3d31 223e 0d0a 3c6d  al-scale=1">..<m
+00000e70: 6574 6120 6e61 6d65 3d22 6465 7363 7269  eta name="descri
+00000e80: 7074 696f 6e22 2063 6f6e 7465 6e74 3d22  ption" content="
+00000e90: 207b 7b20 706f 7374 5f73 7562 7469 746c   {{ post_subtitl
+00000ea0: 6520 7d7d 223e 0d0a 0d0a 3c6c 696e 6b20  e }}">....<link 
+00000eb0: 7265 6c3d 2273 7479 6c65 7368 6565 7422  rel="stylesheet"
+00000ec0: 2074 7970 653d 2274 6578 742f 6373 7322   type="text/css"
+00000ed0: 206d 6564 6961 3d22 7363 7265 656e 2220   media="screen" 
+00000ee0: 6872 6566 3d22 7b7b 2063 6f6e 6669 672e  href="{{ config.
+00000ef0: 6765 7428 2763 7373 2729 207d 7d22 202f  get('css') }}" /
+00000f00: 3e0d 0a3c 6c69 6e6b 2072 656c 3d22 616c  >..<link rel="al
+00000f10: 7465 726e 6174 6522 2074 7970 653d 2261  ternate" type="a
+00000f20: 7070 6c69 6361 7469 6f6e 2f61 746f 6d2b  pplication/atom+
+00000f30: 786d 6c22 2074 6974 6c65 3d22 5265 6365  xml" title="Rece
+00000f40: 6e74 2062 6c6f 6720 706f 7374 7322 2068  nt blog posts" h
+00000f50: 7265 663d 222f 7273 732e 786d 6c22 3e0d  ref="/rss.xml">.
+00000f60: 0a7b 2520 6966 206d 6574 6164 2025 7d20  .{% if metad %} 
+00000f70: 207b 7b20 6d65 7461 6420 7d7d 207b 2520   {{ metad }} {% 
+00000f80: 656e 6469 6620 257d 0d0a 3c2f 6865 6164  endif %}..</head
+00000f90: 3e0d 0a0d 0a3c 626f 6479 3e0d 0a3c 6865  >....<body>..<he
+00000fa0: 6164 6572 3e0d 0a3c 6831 3e7b 7b20 706f  ader>..<h1>{{ po
+00000fb0: 7374 5f74 6974 6c65 207d 7d20 3c2f 6831  st_title }} </h1
+00000fc0: 3e20 200d 0a3c 2f68 6561 6465 723e 0d0a  >  ..</header>..
+00000fd0: 3c61 7274 6963 6c65 3e0d 0a7b 7b20 6172  <article>..{{ ar
+00000fe0: 7469 636c 6520 7d7d 0d0a 7b25 2069 6620  ticle }}..{% if 
+00000ff0: 6461 7465 2025 7d20 0d0a 3c70 3e23 204c  date %} ..<p># L
+00001000: 6173 7420 7570 6461 7465 6420 6f6e 203c  ast updated on <
+00001010: 7469 6d65 3e7b 7b20 6461 7465 2e73 7472  time>{{ date.str
+00001020: 6674 696d 6528 2725 6420 2562 2025 5927  ftime('%d %b %Y'
+00001030: 2920 7d7d 2e3c 2f74 696d 653e 3c2f 703e  ) }}.</time></p>
+00001040: 0d0a 7b25 2065 6e64 6966 2025 7d0d 0a3c  ..{% endif %}..<
+00001050: 2f61 7274 6963 6c65 3e0d 0a3c 666f 6f74  /article>..<foot
+00001060: 6572 3e0d 0a7b 7b20 666f 6f74 6572 207d  er>..{{ footer }
+00001070: 7d0d 0a3c 2f66 6f6f 7465 723e 0d0a 3c2f  }..</footer>..</
+00001080: 626f 6479 3e0d 0a3c 2f68 746d 6c3e 0d0a  body>..</html>..
+00001090: 2020 2020 2020 2020 2020 2020 2222 2229              """)
+000010a0: 0d0a 2020 2020 2020 2020 662e 7772 6974  ..        f.writ
+000010b0: 6528 636f 6e66 5f64 6174 6129 0d0a 2020  e(conf_data)..  
+000010c0: 2020 2020 2020 7072 696e 7428 276e 6f74        print('not
+000010d0: 6520 7465 6d70 6c61 7465 2063 7265 6174  e template creat
+000010e0: 6564 2e27 290d 0a0d 0a20 2020 2077 6974  ed.')....    wit
+000010f0: 6820 6f70 656e 2870 6174 682e 6a6f 696e  h open(path.join
+00001100: 2870 6964 6765 794e 616d 652c 2774 656d  (pidgeyName,'tem
+00001110: 706c 6174 6527 2c27 6665 6564 5f74 656d  plate','feed_tem
+00001120: 706c 6174 652e 786d 6c27 292c 2777 2729  plate.xml'),'w')
+00001130: 2061 7320 663a 0d0a 2020 2020 2020 2020   as f:..        
+00001140: 636f 6e66 5f64 6174 6120 3d20 280d 0a20  conf_data = (.. 
+00001150: 2020 2020 2020 2020 2020 2022 2222 3c3f             """<?
+00001160: 786d 6c20 7665 7273 696f 6e3d 2231 2e30  xml version="1.0
+00001170: 2220 656e 636f 6469 6e67 3d22 5554 462d  " encoding="UTF-
+00001180: 3822 3f3e 0d0a 3c72 7373 2076 6572 7369  8"?>..<rss versi
+00001190: 6f6e 3d22 322e 3022 3e0d 0a0d 0a20 3c63  on="2.0">.... <c
+000011a0: 6861 6e6e 656c 3e0d 0a20 203c 7469 746c  hannel>..  <titl
+000011b0: 653e 7b7b 7469 746c 657d 7d3c 2f74 6974  e>{{title}}</tit
+000011c0: 6c65 3e0d 0a20 203c 6174 6f6d 3a6c 696e  le>..  <atom:lin
+000011d0: 6b20 6872 6566 3d22 7b7b 2075 726c 207d  k href="{{ url }
+000011e0: 7d22 2072 656c 3d22 7365 6c66 2220 7479  }" rel="self" ty
+000011f0: 7065 3d22 6170 706c 6963 6174 696f 6e2f  pe="application/
+00001200: 7273 732b 786d 6c22 202f 3e0d 0a20 203c  rss+xml" />..  <
+00001210: 6c69 6e6b 3e7b 7b20 7572 6c20 7d7d 3c2f  link>{{ url }}</
+00001220: 6c69 6e6b 3e0d 0a20 203c 6465 7363 7269  link>..  <descri
+00001230: 7074 696f 6e3e 7b7b 2073 7562 7469 746c  ption>{{ subtitl
+00001240: 6520 7d7d 3c2f 6465 7363 7269 7074 696f  e }}</descriptio
+00001250: 6e3e 0d0a 2020 3c6c 6173 7442 7569 6c64  n>..  <lastBuild
+00001260: 4461 7465 3e7b 7b20 6c61 7374 5f64 6174  Date>{{ last_dat
+00001270: 652e 7374 7266 7469 6d65 2827 2561 2c20  e.strftime('%a, 
+00001280: 2564 2025 6220 2559 2025 483a 254d 3a25  %d %b %Y %H:%M:%
+00001290: 5320 474d 5427 2920 7d7d 3c2f 6c61 7374  S GMT') }}</last
+000012a0: 4275 696c 6444 6174 653e 0d0a 2020 3c6c  BuildDate>..  <l
+000012b0: 616e 6775 6167 653e 656e 2d49 4e3c 2f6c  anguage>en-IN</l
+000012c0: 616e 6775 6167 653e 0d0a 0d0a 2020 3c69  anguage>....  <i
+000012d0: 6d61 6765 3e0d 0a20 2020 3c75 726c 3e7b  mage>..   <url>{
+000012e0: 7b20 636f 6e66 6967 2e67 6574 2827 7572  { config.get('ur
+000012f0: 6c27 2920 7d7d 2f7b 7b20 636f 6e66 6967  l') }}/{{ config
+00001300: 2e67 6574 2827 7068 7427 2920 7d7d 3c2f  .get('pht') }}</
+00001310: 7572 6c3e 0d0a 2020 203c 7469 746c 653e  url>..   <title>
+00001320: 7b7b 2074 6974 6c65 207d 7d3c 2f74 6974  {{ title }}</tit
+00001330: 6c65 3e0d 0a20 2020 3c6c 696e 6b3e 7b7b  le>..   <link>{{
+00001340: 2075 726c 207d 7d3c 2f6c 696e 6b3e 0d0a   url }}</link>..
+00001350: 2020 203c 7769 6474 683e 3332 3c2f 7769     <width>32</wi
+00001360: 6474 683e 0d0a 2020 203c 6865 6967 6874  dth>..   <height
+00001370: 3e33 323c 2f68 6569 6768 743e 0d0a 2020  >32</height>..  
+00001380: 3c2f 696d 6167 653e 0d0a 0d0a 2020 7b25  </image>....  {%
+00001390: 2066 6f72 2070 6f73 7420 696e 2070 6f73   for post in pos
+000013a0: 7473 2025 7d7b 2520 6966 2028 706f 7374  ts %}{% if (post
+000013b0: 2e73 686f 7749 6e48 6f6d 6520 6973 2075  .showInHome is u
+000013c0: 6e64 6566 696e 6564 2920 6f72 2070 6f73  ndefined) or pos
+000013d0: 742e 7368 6f77 496e 486f 6d65 2025 7d0d  t.showInHome %}.
+000013e0: 0a20 203c 6974 656d 3e0d 0a20 2020 3c74  .  <item>..   <t
+000013f0: 6974 6c65 3e7b 7b20 706f 7374 2e74 6974  itle>{{ post.tit
+00001400: 6c65 207d 7d3c 2f74 6974 6c65 3e0d 0a20  le }}</title>.. 
+00001410: 2020 3c6c 696e 6b3e 7b7b 2063 6f6e 6669    <link>{{ confi
+00001420: 672e 6765 7428 2775 726c 2729 207d 7d7b  g.get('url') }}{
+00001430: 7b20 706f 7374 2e75 726c 207d 7d3c 2f6c  { post.url }}</l
+00001440: 696e 6b3e 0d0a 2020 203c 7075 6244 6174  ink>..   <pubDat
+00001450: 653e 7b7b 2070 6f73 742e 6461 7465 2e73  e>{{ post.date.s
+00001460: 7472 6674 696d 6528 2725 612c 2025 6420  trftime('%a, %d 
+00001470: 2562 2025 5920 2548 3a25 4d3a 2553 2047  %b %Y %H:%M:%S G
+00001480: 4d54 2729 207d 7d3c 2f70 7562 4461 7465  MT') }}</pubDate
+00001490: 3e0d 0a20 2020 3c67 7569 6420 6973 5065  >..   <guid isPe
+000014a0: 726d 614c 696e 6b3d 2266 616c 7365 223e  rmaLink="false">
+000014b0: 7b7b 2063 6f6e 6669 672e 6765 7428 2775  {{ config.get('u
+000014c0: 726c 2729 207d 7d7b 7b20 706f 7374 2e75  rl') }}{{ post.u
+000014d0: 726c 207d 7d3c 2f67 7569 643e 0d0a 0909  rl }}</guid>....
+000014e0: 093c 6465 7363 7269 7074 696f 6e3e 3c21  .<description><!
+000014f0: 5b43 4441 5441 5b7b 7b20 706f 7374 2e73  [CDATA[{{ post.s
+00001500: 7562 7469 746c 6520 7d7d 202d 207b 7b20  ubtitle }} - {{ 
+00001510: 706f 7374 2e6e 6f74 6520 7d7d 205d 5d3e  post.note }} ]]>
+00001520: 3c2f 6465 7363 7269 7074 696f 6e3e 0d0a  </description>..
+00001530: 2020 3c2f 6974 656d 3e0d 0a20 207b 2520    </item>..  {% 
+00001540: 656e 6469 6620 257d 7b25 2065 6e64 666f  endif %}{% endfo
+00001550: 7220 257d 0d0a 203c 2f63 6861 6e6e 656c  r %}.. </channel
+00001560: 3e0d 0a20 2020 2020 2020 2020 2020 2022  >..            "
+00001570: 2222 290d 0a20 2020 2020 2020 2066 2e77  "")..        f.w
+00001580: 7269 7465 2863 6f6e 665f 6461 7461 290d  rite(conf_data).
+00001590: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
+000015a0: 7273 7320 7465 6d70 6c61 7465 2063 7265  rss template cre
+000015b0: 6174 6564 2e27 290d 0a20 2020 2020 2020  ated.')..       
+000015c0: 2066 2e63 6c6f 7365 2829 0d0a 0d0a 0d0a   f.close()......
+000015d0: 6465 6620 6372 6561 7465 436f 6e74 656e  def createConten
+000015e0: 7428 7069 6467 6579 4e61 6d65 293a 0d0a  t(pidgeyName):..
+000015f0: 2020 2020 7769 7468 206f 7065 6e28 7061      with open(pa
+00001600: 7468 2e6a 6f69 6e28 7069 6467 6579 4e61  th.join(pidgeyNa
+00001610: 6d65 2c27 636f 6e74 656e 7427 2c27 6865  me,'content','he
+00001620: 6164 6572 2e6d 6427 292c 2777 2729 2061  ader.md'),'w') a
+00001630: 7320 663a 0d0a 2020 2020 2020 2020 636f  s f:..        co
+00001640: 6e66 5f64 6174 6120 3d20 280d 0a20 2020  nf_data = (..   
+00001650: 2020 2020 2020 2020 2022 2222 2a20 2020           """*   
+00001660: 5b48 6f6d 655d 282f 290d 0a2a 2020 205b  [Home](/)..*   [
+00001670: 4f74 6865 7220 4c69 6e6b 735d 282f 290d  Other Links](/).
+00001680: 0a2a 2020 205b 4564 6974 2063 6f6e 7465  .*   [Edit conte
+00001690: 6e74 2f68 6561 6465 722e 6d64 5d28 2f29  nt/header.md](/)
+000016a0: 0d0a 2020 2020 2020 2020 2020 2020 2222  ..            ""
+000016b0: 2229 0d0a 2020 2020 2020 2020 662e 7772  ")..        f.wr
+000016c0: 6974 6528 636f 6e66 5f64 6174 6129 0d0a  ite(conf_data)..
+000016d0: 2020 2020 2020 2020 7072 696e 7428 2768          print('h
+000016e0: 6561 6465 7220 6372 6561 7465 642e 2729  eader created.')
+000016f0: 0d0a 0d0a 2020 2020 7769 7468 206f 7065  ....    with ope
+00001700: 6e28 7061 7468 2e6a 6f69 6e28 7069 6467  n(path.join(pidg
+00001710: 6579 4e61 6d65 2c27 636f 6e74 656e 7427  eyName,'content'
+00001720: 2c27 666f 6f74 6572 2e6d 6427 292c 2777  ,'footer.md'),'w
+00001730: 2729 2061 7320 663a 0d0a 2020 2020 2020  ') as f:..      
+00001740: 2020 636f 6e66 5f64 6174 6120 3d20 280d    conf_data = (.
+00001750: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
+00001760: 2a20 2020 5b48 6f6d 655d 282f 290d 0a2a  *   [Home](/)..*
+00001770: 2020 205b 5253 535d 282f 290d 0a2a 2020     [RSS](/)..*  
+00001780: 205b 4564 6974 2063 6f6e 7465 6e74 2f66   [Edit content/f
+00001790: 6f6f 7465 722e 6d64 5d28 2f29 0d0a 2a20  ooter.md](/)..* 
+000017a0: 2020 706f 7765 7265 6420 6279 205b 5069    powered by [Pi
+000017b0: 6467 656f 7474 6f5d 282f 290d 0a20 2020  dgeotto](/)..   
+000017c0: 2020 2020 2020 2020 2022 2222 290d 0a20           """).. 
+000017d0: 2020 2020 2020 2066 2e77 7269 7465 2863         f.write(c
+000017e0: 6f6e 665f 6461 7461 290d 0a20 2020 2020  onf_data)..     
+000017f0: 2020 2070 7269 6e74 2827 666f 6f74 6572     print('footer
+00001800: 2063 7265 6174 6564 2e27 290d 0a0d 0a20   created.').... 
+00001810: 2020 2077 6974 6820 6f70 656e 2870 6174     with open(pat
+00001820: 682e 6a6f 696e 2870 6964 6765 794e 616d  h.join(pidgeyNam
+00001830: 652c 2763 6f6e 7465 6e74 272c 2768 6f6d  e,'content','hom
+00001840: 652e 6d64 2729 2c27 7727 2920 6173 2066  e.md'),'w') as f
+00001850: 3a0d 0a20 2020 2020 2020 2063 6f6e 665f  :..        conf_
+00001860: 6461 7461 203d 2028 0d0a 2020 2020 2020  data = (..      
+00001870: 2020 2020 2020 2222 2257 656c 636f 6d65        """Welcome
+00001880: 2074 6f20 5069 6467 656f 7474 6f2e 0d0a   to Pidgeotto...
+00001890: 3c62 723e 2054 6869 7320 6973 2061 2073  <br> This is a s
+000018a0: 616d 706c 6520 686f 6d65 7061 6765 2077  ample homepage w
+000018b0: 6869 6368 2063 616e 2062 6520 6564 6974  hich can be edit
+000018c0: 6564 2061 7420 2f63 6f6e 7465 6e74 2f68  ed at /content/h
+000018d0: 6f6d 652e 6d64 0d0a 0d0a 2a2a 2050 6964  ome.md....** Pid
+000018e0: 6765 6f74 746f 206c 696e 6b73 3a20 2a2a  geotto links: **
+000018f0: 0d0a 2a20 2020 5b44 6f63 756d 656e 7461  ..*   [Documenta
+00001900: 7469 6f6e 5d28 2f29 2e0d 0a2a 2020 205b  tion](/)...*   [
+00001910: 4769 7468 7562 2053 6f75 7263 655d 282f  Github Source](/
+00001920: 292e 0d0a 2020 2020 2020 2020 2222 2229  )...        """)
+00001930: 0d0a 2020 2020 2020 2020 662e 7772 6974  ..        f.writ
+00001940: 6528 636f 6e66 5f64 6174 6129 0d0a 2020  e(conf_data)..  
+00001950: 2020 2020 2020 7072 696e 7428 2766 6f6f        print('foo
+00001960: 7465 7220 6372 6561 7465 642e 2729 0d0a  ter created.')..
+00001970: 2020 2020 0d0a 2020 2020 7769 7468 206f      ..    with o
+00001980: 7065 6e28 7061 7468 2e6a 6f69 6e28 7069  pen(path.join(pi
+00001990: 6467 6579 4e61 6d65 2c27 636f 6e74 656e  dgeyName,'conten
+000019a0: 7427 2c27 6e6f 7465 272c 2762 6c6f 6731  t','note','blog1
+000019b0: 2e6d 6427 292c 2777 2729 2061 7320 663a  .md'),'w') as f:
+000019c0: 0d0a 2020 2020 2020 2020 636f 6e66 5f64  ..        conf_d
+000019d0: 6174 6120 3d20 280d 0a20 2020 2020 2020  ata = (..       
+000019e0: 2020 2020 2022 2222 2d2d 2d0d 0a74 6974       """---..tit
+000019f0: 6c65 203a 2022 5361 6d70 6c65 2042 6c6f  le : "Sample Blo
+00001a00: 672e 220d 0a73 7562 7469 746c 6520 3a20  g."..subtitle : 
+00001a10: 2253 616d 706c 6520 7375 6274 6974 6c65  "Sample subtitle
+00001a20: 220d 0a64 6174 6520 3a20 7b74 7d0d 0a2d  "..date : {t}..-
+00001a30: 2d2d 0d0a 0d0a 2320 5468 6973 2069 7320  --....# This is 
+00001a40: 6120 7361 6d70 6c65 206e 6f74 6520 7061  a sample note pa
+00001a50: 6765 2077 6869 6368 2063 616e 2062 6520  ge which can be 
+00001a60: 6564 6974 6564 2f72 656e 616d 6564 2061  edited/renamed a
+00001a70: 7420 2f63 6f6e 7465 6e74 2f6e 6f74 652f  t /content/note/
+00001a80: 626c 6f67 312e 6d64 0d0a 2320 5468 6973  blog1.md..# This
+00001a90: 2069 7320 6865 6164 696e 6720 310d 0a0d   is heading 1...
+00001aa0: 0a23 2320 5468 6973 2069 7320 6865 6164  .## This is head
+00001ab0: 696e 6720 320d 0a0d 0a23 2323 2054 6869  ing 2....### Thi
+00001ac0: 7320 6973 2068 6561 6469 6e67 2033 0d0a  s is heading 3..
+00001ad0: 0d0a 2323 2323 2054 6869 7320 6973 2068  ..#### This is h
+00001ae0: 6561 6469 6e67 2034 0d0a 0d0a 2323 2323  eading 4....####
+00001af0: 2320 5468 6973 2069 7320 6865 6164 696e  # This is headin
+00001b00: 6720 350d 0a0d 0a23 2323 2323 2320 5468  g 5....###### Th
+00001b10: 6973 2069 7320 6865 6164 696e 6720 360d  is is heading 6.
+00001b20: 0a0d 0a2a 2a42 6f6c 642a 2a0d 0a0d 0a2a  ...**Bold**....*
+00001b30: 6974 616c 6963 2a0d 0a0d 0a2a 206c 6973  italic*....* lis
+00001b40: 740d 0a2a 206c 6973 740d 0a0d 0a31 2e20  t..* list....1. 
+00001b50: 6f72 6465 7265 6420 6c69 7374 0d0a 322e  ordered list..2.
+00001b60: 206f 7264 6572 6564 206c 6973 740d 0a0d   ordered list...
+00001b70: 0a5b 6c69 6e6b 5d28 2f29 0d0a 0d0a 5361  .[link](/)....Sa
+00001b80: 6d70 6c65 2070 6172 6167 7261 7068 2069  mple paragraph i
+00001b90: 7320 7772 6974 7465 6e20 6c69 6b65 2074  s written like t
+00001ba0: 6869 7320 7769 7468 206c 6f72 656d 2069  his with lorem i
+00001bb0: 7073 756d 2e20 4c6f 7265 6d20 6970 7375  psum. Lorem ipsu
+00001bc0: 6d20 646f 6c6f 7220 7369 7420 616d 6574  m dolor sit amet
+00001bd0: 2c20 636f 6e73 6563 7465 7475 7220 6164  , consectetur ad
+00001be0: 6970 6973 6369 6e67 2065 6c69 742c 2073  ipiscing elit, s
+00001bf0: 6564 2064 6f20 6569 7573 6d6f 6420 7465  ed do eiusmod te
+00001c00: 6d70 6f72 2069 6e63 6964 6964 756e 7420  mpor incididunt 
+00001c10: 7574 206c 6162 6f72 6520 6574 2064 6f6c  ut labore et dol
+00001c20: 6f72 6520 6d61 676e 6120 616c 6971 7561  ore magna aliqua
+00001c30: 2e20 5574 2065 6e69 6d20 6164 206d 696e  . Ut enim ad min
+00001c40: 696d 2076 656e 6961 6d2c 2071 7569 7320  im veniam, quis 
+00001c50: 6e6f 7374 7275 6420 6578 6572 6369 7461  nostrud exercita
+00001c60: 7469 6f6e 2075 6c6c 616d 636f 206c 6162  tion ullamco lab
+00001c70: 6f72 6973 206e 6973 6920 7574 2061 6c69  oris nisi ut ali
+00001c80: 7175 6970 2065 7820 6561 2063 6f6d 6d6f  quip ex ea commo
+00001c90: 646f 2063 6f6e 7365 7175 6174 2e20 4475  do consequat. Du
+00001ca0: 6973 2061 7574 6520 6972 7572 6520 646f  is aute irure do
+00001cb0: 6c6f 7220 696e 2072 6570 7265 6865 6e64  lor in reprehend
+00001cc0: 6572 6974 2069 6e20 766f 6c75 7074 6174  erit in voluptat
+00001cd0: 6520 7665 6c69 7420 6573 7365 2063 696c  e velit esse cil
+00001ce0: 6c75 6d20 646f 6c6f 7265 2065 7520 6675  lum dolore eu fu
+00001cf0: 6769 6174 206e 756c 6c61 2070 6172 6961  giat nulla paria
+00001d00: 7475 722e 2045 7863 6570 7465 7572 2073  tur. Excepteur s
+00001d10: 696e 7420 6f63 6361 6563 6174 2063 7570  int occaecat cup
+00001d20: 6964 6174 6174 206e 6f6e 2070 726f 6964  idatat non proid
+00001d30: 656e 742c 2073 756e 7420 696e 2063 756c  ent, sunt in cul
+00001d40: 7061 2071 7569 206f 6666 6963 6961 2064  pa qui officia d
+00001d50: 6573 6572 756e 7420 6d6f 6c6c 6974 2061  eserunt mollit a
+00001d60: 6e69 6d20 6964 2065 7374 206c 6162 6f72  nim id est labor
+00001d70: 756d 2e0d 0a20 2020 2020 2020 2022 2222  um...        """
+00001d80: 292e 666f 726d 6174 2874 3d64 6174 6574  ).format(t=datet
+00001d90: 696d 652e 6e6f 7728 292e 7374 7266 7469  ime.now().strfti
+00001da0: 6d65 2822 2559 2d25 6d2d 2564 2229 290d  me("%Y-%m-%d")).
+00001db0: 0a20 2020 2020 2020 2066 2e77 7269 7465  .        f.write
+00001dc0: 2863 6f6e 665f 6461 7461 290d 0a20 2020  (conf_data)..   
+00001dd0: 2020 2020 2070 7269 6e74 2827 7361 6d70       print('samp
+00001de0: 6c65 2062 6c6f 6720 6372 6561 7465 642e  le blog created.
+00001df0: 2729 0d0a 0d0a 0d0a 6465 6620 6372 6561  ')......def crea
+00001e00: 7465 5069 6467 6579 2870 6964 6765 794e  tePidgey(pidgeyN
+00001e10: 616d 6529 3a0d 0a20 2020 2074 7279 3a0d  ame):..    try:.
+00001e20: 0a20 2020 2020 2020 206d 6b64 6972 2870  .        mkdir(p
+00001e30: 6964 6765 794e 616d 6529 0d0a 2020 2020  idgeyName)..    
+00001e40: 2020 2020 7072 696e 7428 2270 6964 6765      print("pidge
+00001e50: 7920 2220 2b20 7069 6467 6579 4e61 6d65  y " + pidgeyName
+00001e60: 202b 2022 2063 7265 6174 6564 2e22 290d   + " created.").
+00001e70: 0a20 2020 2020 2020 206d 6b64 6972 2870  .        mkdir(p
+00001e80: 6174 682e 6a6f 696e 2870 6964 6765 794e  ath.join(pidgeyN
+00001e90: 616d 652c 2774 656d 706c 6174 6527 2929  ame,'template'))
+00001ea0: 0d0a 2020 2020 2020 2020 6d6b 6469 7228  ..        mkdir(
+00001eb0: 7061 7468 2e6a 6f69 6e28 7069 6467 6579  path.join(pidgey
+00001ec0: 4e61 6d65 2c27 7374 6174 6963 2729 290d  Name,'static')).
+00001ed0: 0a20 2020 2020 2020 206d 6b64 6972 2870  .        mkdir(p
+00001ee0: 6174 682e 6a6f 696e 2870 6964 6765 794e  ath.join(pidgeyN
+00001ef0: 616d 652c 2763 6f6e 7465 6e74 2729 290d  ame,'content')).
+00001f00: 0a20 2020 2020 2020 206d 6b64 6972 2870  .        mkdir(p
+00001f10: 6174 682e 6a6f 696e 2870 6964 6765 794e  ath.join(pidgeyN
+00001f20: 616d 652c 2763 6f6e 7465 6e74 272c 276e  ame,'content','n
+00001f30: 6f74 6527 2929 0d0a 2020 2020 2020 2020  ote'))..        
+00001f40: 6372 6561 7465 436f 6e66 6967 2870 6964  createConfig(pid
+00001f50: 6765 794e 616d 6529 0d0a 2020 2020 2020  geyName)..      
+00001f60: 2020 6372 6561 7465 5465 6d70 6c61 7465    createTemplate
+00001f70: 7328 7069 6467 6579 4e61 6d65 290d 0a20  s(pidgeyName).. 
+00001f80: 2020 2020 2020 2063 7265 6174 6543 6f6e         createCon
+00001f90: 7465 6e74 2870 6964 6765 794e 616d 6529  tent(pidgeyName)
+00001fa0: 0d0a 2020 2020 6578 6365 7074 3a0d 0a20  ..    except:.. 
+00001fb0: 2020 2020 2020 2070 7269 6e74 2822 7768         print("wh
+00001fc0: 696c 6520 6765 6e65 7261 7469 6e67 2070  ile generating p
+00001fd0: 6964 6765 7920 222b 2070 6964 6765 794e  idgey "+ pidgeyN
+00001fe0: 616d 6520 2b20 222c 2073 6f6d 6520 6973  ame + ", some is
+00001ff0: 7375 6520 6f63 6375 7265 642e 2229 0d0a  sue occured.")..
+00002000: 2020 2020 2020 2020 7072 696e 7428 2254          print("T
+00002010: 6869 7320 6361 6e20 6265 2064 7565 2074  his can be due t
+00002020: 6f20 5c6e 5c74 312e 2050 6964 6765 7920  o \n\t1. Pidgey 
+00002030: 616c 7265 6164 7920 6578 6973 7473 2e5c  already exists.\
+00002040: 6e5c 7432 2e20 4d65 6d6f 7279 2069 7373  n\t2. Memory iss
+00002050: 7565 2e5c 6e5c 7433 2e20 496e 7661 6c69  ue.\n\t3. Invali
+00002060: 6420 696e 7075 742e 5c6e 5c74 342e 2049  d input.\n\t4. I
+00002070: 6620 6e6f 6e65 206f 6620 7468 6573 652c  f none of these,
+00002080: 2072 6570 6f72 7420 746f 2064 6576 656c   report to devel
+00002090: 6f70 6572 2e22 290d 0a0d 0a64 6566 2063  oper.")....def c
+000020a0: 7265 6174 654e 6f74 6528 6e6f 7465 4e61  reateNote(noteNa
+000020b0: 6d65 2c20 7368 6f77 496e 486f 6d65 3d54  me, showInHome=T
+000020c0: 7275 6529 3a0d 0a20 2020 2074 7279 3a0d  rue):..    try:.
+000020d0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000020e0: 6e6f 7465 4e61 6d65 2e6c 6f77 6572 2829  noteName.lower()
+000020f0: 2e65 6e64 7377 6974 6828 272e 6d64 2729  .endswith('.md')
+00002100: 3a0d 0a20 2020 2020 2020 2020 2020 206e  :..            n
+00002110: 6f74 654e 616d 652b 3d27 2e6d 6427 0d0a  oteName+='.md'..
+00002120: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
+00002130: 6e28 7061 7468 2e6a 6f69 6e28 2763 6f6e  n(path.join('con
+00002140: 7465 6e74 272c 276e 6f74 6527 2c6e 6f74  tent','note',not
+00002150: 654e 616d 6529 2c27 7727 2920 6173 2066  eName),'w') as f
+00002160: 3a0d 0a20 2020 2020 2020 2020 2020 2063  :..            c
+00002170: 6f6e 665f 6461 7461 203d 2028 0d0a 2020  onf_data = (..  
+00002180: 2020 2020 2020 2020 2020 2222 222d 2d2d            """---
+00002190: 0d0a 7469 746c 6520 3a20 2254 6974 6c65  ..title : "Title
+000021a0: 220d 0a73 7562 7469 746c 6520 3a20 2253  "..subtitle : "S
+000021b0: 7562 7469 746c 6522 0d0a 7368 6f77 496e  ubtitle"..showIn
+000021c0: 486f 6d65 203a 207b 737d 0d0a 6461 7465  Home : {s}..date
+000021d0: 203a 207b 747d 0d0a 2d2d 2d0d 0a20 2020   : {t}..---..   
+000021e0: 2020 2020 2020 2020 2022 2222 292e 666f           """).fo
+000021f0: 726d 6174 2874 3d64 6174 6574 696d 652e  rmat(t=datetime.
+00002200: 6e6f 7728 292e 7374 7266 7469 6d65 2822  now().strftime("
+00002210: 2559 2d25 6d2d 2564 2229 2c20 733d 7368  %Y-%m-%d"), s=sh
+00002220: 6f77 496e 486f 6d65 290d 0a20 2020 2020  owInHome)..     
+00002230: 2020 2020 2020 2066 2e77 7269 7465 2863         f.write(c
+00002240: 6f6e 665f 6461 7461 290d 0a20 2020 2020  onf_data)..     
+00002250: 2020 2020 2020 2070 7269 6e74 286e 6f74         print(not
+00002260: 654e 616d 652b 2220 6973 2063 7265 6174  eName+" is creat
+00002270: 6564 2061 7420 636f 6e74 656e 742f 6e6f  ed at content/no
+00002280: 7465 2f22 2b6e 6f74 654e 616d 6520 290d  te/"+noteName ).
+00002290: 0a20 2020 2065 7863 6570 743a 0d0a 2020  .    except:..  
+000022a0: 2020 2020 2020 7072 696e 7428 2277 6869        print("whi
+000022b0: 6c65 2067 656e 6572 6174 696e 6720 7061  le generating pa
+000022c0: 6765 2022 2b6e 6f74 654e 616d 652b 222c  ge "+noteName+",
+000022d0: 2073 6f6d 6520 6973 7375 6520 6f63 6375   some issue occu
+000022e0: 7265 642e 2229 0d0a 2020 2020 2020 2020  red.")..        
+000022f0: 7072 696e 7428 2254 6869 7320 6361 6e20  print("This can 
+00002300: 6265 2064 7565 2074 6f20 5c6e 5c74 312e  be due to \n\t1.
+00002310: 204e 6f74 2061 2070 6964 6765 7920 6469   Not a pidgey di
+00002320: 7265 6374 6f72 792e 205c 6e5c 7432 2e20  rectory. \n\t2. 
+00002330: 496e 7661 6c69 6420 6669 6c65 6e61 6d65  Invalid filename
+00002340: 2229 0d0a                                ")..
```

### Comparing `pidgeotto-0.0.4/pidgey/pidgey.py` & `pidgeotto-0.0.5/pidgey/pidgey.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-#!/bin/python
-
-#   
-#       ███╗   ██╗██╗██╗  ██╗ █████╗ ██████╗ ███████╗
-#       ████╗  ██║██║██║  ██║██╔══██╗██╔══██╗██╔════╝
-#       ██╔██╗ ██║██║███████║███████║██████╔╝███████╗
-#       ██║╚██╗██║██║██╔══██║██╔══██║██╔══██╗╚════██║
-#       ██║ ╚████║██║██║  ██║██║  ██║██║  ██║███████║
-#       ╚═╝  ╚═══╝╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚══════╝
-#       DRAFTED BY [https://nihar.page] ON 10-04-2021.
-#       SOURCE [pidgey.py] LAST MODIFIED ON 20-04-2021.
-#
-
-# External imports
-from pidgey import creator,builder,server,__version__
-from argparse import ArgumentParser
-
-    
-def main():
-    parser = ArgumentParser(prog='pidgey', description='Yet another simple static site generator.')
-    parser.add_argument("-v", "--version", action="version", version="{version}".format(version=__version__) )
-    subparsers = parser.add_subparsers(dest='type', help='command help', required=True)
-    parser_init = subparsers.add_parser('init', help='start new pidgeotto').add_argument("name")
-    parser_new = subparsers.add_parser('new', help='create new note/post/page').add_argument("name")
-    parser_build = subparsers.add_parser('build', help='build the pidgeotto')
-    parser_serve = subparsers.add_parser('serve', help='serve the pidgeotto')
-    args = parser.parse_args()
-    if args.type == "init" and args.name:
-        creator.createPidgey(args.name)
-    elif args.type == "new" and args.name:
-        creator.createNote(args.name)
-    elif args.type == 'build':
-        builder.buildPidgey()
-    elif args.type == 'serve':
-        server.server()
-    else: 
-        parser.print_help()
+#!/bin/python
+
+#   
+#       ███╗   ██╗██╗██╗  ██╗ █████╗ ██████╗ ███████╗
+#       ████╗  ██║██║██║  ██║██╔══██╗██╔══██╗██╔════╝
+#       ██╔██╗ ██║██║███████║███████║██████╔╝███████╗
+#       ██║╚██╗██║██║██╔══██║██╔══██║██╔══██╗╚════██║
+#       ██║ ╚████║██║██║  ██║██║  ██║██║  ██║███████║
+#       ╚═╝  ╚═══╝╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚══════╝
+#       DRAFTED BY [https://nih.ar] ON 10-04-2021.
+#       SOURCE [pidgey.py] LAST MODIFIED ON 20-06-2023.
+#
+
+# External imports
+from pidgey import creator,builder,server,__version__
+from argparse import ArgumentParser
+
+    
+def main():
+    parser = ArgumentParser(prog='pidgey', description='Yet another simple static site generator.')
+    parser.add_argument("-v", "--version", action="version", version="{version}".format(version=__version__) )
+    subparsers = parser.add_subparsers(dest='type', help='command help', required=True)
+    parser_init = subparsers.add_parser('init', help='start new pidgeotto').add_argument("name")
+    parser_new = subparsers.add_parser('new', help='create new note/post/page').add_argument("name")
+    parser_build = subparsers.add_parser('build', help='build the pidgeotto')
+    parser_serve = subparsers.add_parser('serve', help='serve the pidgeotto')
+    args = parser.parse_args()
+    if args.type == "init" and args.name:
+        creator.createPidgey(args.name)
+    elif args.type == "new" and args.name:
+        creator.createNote(args.name)
+    elif args.type == 'build':
+        builder.buildPidgey()
+    elif args.type == 'serve':
+        server.server()
+    else: 
+        parser.print_help()
```

### Comparing `pidgeotto-0.0.4/pidgey/server.py` & `pidgeotto-0.0.5/pidgey/server.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-#!/bin/python3
-
-#
-#       ███╗   ██╗██╗██╗  ██╗ █████╗ ██████╗ ███████╗
-#       ████╗  ██║██║██║  ██║██╔══██╗██╔══██╗██╔════╝
-#       ██╔██╗ ██║██║███████║███████║██████╔╝███████╗
-#       ██║╚██╗██║██║██╔══██║██╔══██║██╔══██╗╚════██║
-#       ██║ ╚████║██║██║  ██║██║  ██║██║  ██║███████║
-#       ╚═╝  ╚═══╝╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚══════╝
-#       DRAFTED BY [https://nihar.page] ON 08-05-2021.
-#       SOURCE [serve.py] LAST MODIFIED ON 08-05-2021.
-#
-
-from http.server import SimpleHTTPRequestHandler
-from socketserver import TCPServer
-from os import path, chdir
-from yaml import safe_load
-
-
-def server():
-    try:
-        with open('config.yml') as conf:
-            config = safe_load(conf.read())
-            for key,val in config.items():
-                globals()[key] = val
-        PORT = 5555
-        chdir(path.join(home_path))
-        httpd = TCPServer(("", PORT), SimpleHTTPRequestHandler)
-        print("serving at port", PORT)
-        httpd.serve_forever()
-    except KeyboardInterrupt: 
-        pass; 
-        httpd.server_close() 
-    except:
-        print("while serving pidgey, some issue occured.")
-        print("This can be due to \n\t1. Not a pidgey directory. \n\t2. Pidgey not built yet.")
+#!/bin/python3
+
+#
+#       ███╗   ██╗██╗██╗  ██╗ █████╗ ██████╗ ███████╗
+#       ████╗  ██║██║██║  ██║██╔══██╗██╔══██╗██╔════╝
+#       ██╔██╗ ██║██║███████║███████║██████╔╝███████╗
+#       ██║╚██╗██║██║██╔══██║██╔══██║██╔══██╗╚════██║
+#       ██║ ╚████║██║██║  ██║██║  ██║██║  ██║███████║
+#       ╚═╝  ╚═══╝╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚══════╝
+#       DRAFTED BY [https://nih.ar] ON 08-05-2021.
+#       SOURCE [serve.py] LAST MODIFIED ON 08-06-2023.
+#
+
+from http.server import SimpleHTTPRequestHandler
+from socketserver import TCPServer
+from os import path, chdir
+from yaml import safe_load
+
+
+def server():
+    try:
+        with open('config.yml') as conf:
+            config = safe_load(conf.read())
+            for key,val in config.items():
+                globals()[key] = val
+        PORT = 5555
+        chdir(path.join(home_path))
+        httpd = TCPServer(("", PORT), SimpleHTTPRequestHandler)
+        print("serving at port", PORT)
+        httpd.serve_forever()
+    except KeyboardInterrupt: 
+        pass; 
+        httpd.server_close() 
+    except:
+        print("while serving pidgey, some issue occured.")
+        print("This can be due to \n\t1. Not a pidgey directory. \n\t2. Pidgey not built yet.")
```

