# Comparing `tmp/yaylib-0.1.2.tar.gz` & `tmp/yaylib-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaylib-0.1.2.tar", last modified: Sat Jun 10 05:31:49 2023, max compression
+gzip compressed data, was "yaylib-0.1.3.tar", last modified: Sun Jun 25 08:32:04 2023, max compression
```

## Comparing `yaylib-0.1.2.tar` & `yaylib-0.1.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 05:31:49.419185 yaylib-0.1.2/
--rw-rw-rw-   0        0        0     1088 2023-06-10 05:03:11.000000 yaylib-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     9580 2023-06-10 05:31:49.418185 yaylib-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     8723 2023-06-10 05:03:26.000000 yaylib-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-10 05:31:49.419185 yaylib-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1484 2023-06-10 05:03:11.000000 yaylib-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 05:31:49.372517 yaylib-0.1.2/tests/
--rw-rw-rw-   0        0        0      229 2023-06-10 05:03:11.000000 yaylib-0.1.2/tests/test_call.py
--rw-rw-rw-   0        0        0      829 2023-06-10 05:03:11.000000 yaylib-0.1.2/tests/test_cassandra.py
--rw-rw-rw-   0        0        0      229 2023-06-10 05:03:11.000000 yaylib-0.1.2/tests/test_chat.py
--rw-rw-rw-   0        0        0      231 2023-06-10 05:03:11.000000 yaylib-0.1.2/tests/test_group.py
--rw-rw-rw-   0        0        0      229 2023-06-10 05:03:11.000000 yaylib-0.1.2/tests/test_misc.py
--rw-rw-rw-   0        0        0     2552 2023-06-10 05:03:11.000000 yaylib-0.1.2/tests/test_post.py
--rw-rw-rw-   0        0        0      922 2023-06-10 05:03:11.000000 yaylib-0.1.2/tests/test_review.py
--rw-rw-rw-   0        0        0      233 2023-06-10 05:03:11.000000 yaylib-0.1.2/tests/test_thread.py
--rw-rw-rw-   0        0        0      229 2023-06-10 05:03:11.000000 yaylib-0.1.2/tests/test_user.py
-drwxrwxrwx   0        0        0        0 2023-06-10 05:31:49.381663 yaylib-0.1.2/yaylib/
--rw-rw-rw-   0        0        0      263 2023-06-05 07:27:36.000000 yaylib-0.1.2/yaylib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 05:31:49.415186 yaylib-0.1.2/yaylib/api/
--rw-rw-rw-   0        0        0      356 2023-06-03 14:25:16.000000 yaylib-0.1.2/yaylib/api/__init__.py
--rw-rw-rw-   0        0        0     5007 2023-06-10 05:03:11.000000 yaylib-0.1.2/yaylib/api/api.py
--rw-rw-rw-   0        0        0     7358 2023-06-10 05:03:11.000000 yaylib-0.1.2/yaylib/api/call.py
--rw-rw-rw-   0        0        0     1393 2023-06-10 05:03:11.000000 yaylib-0.1.2/yaylib/api/cassandra.py
--rw-rw-rw-   0        0        0    12641 2023-06-10 05:03:11.000000 yaylib-0.1.2/yaylib/api/chat.py
--rw-rw-rw-   0        0        0    19292 2023-06-10 05:03:11.000000 yaylib-0.1.2/yaylib/api/group.py
--rw-rw-rw-   0        0        0     4720 2023-06-10 05:03:26.000000 yaylib-0.1.2/yaylib/api/login.py
--rw-rw-rw-   0        0        0     5561 2023-06-10 05:03:11.000000 yaylib-0.1.2/yaylib/api/misc.py
--rw-rw-rw-   0        0        0    29245 2023-06-10 05:03:26.000000 yaylib-0.1.2/yaylib/api/post.py
--rw-rw-rw-   0        0        0     3036 2023-06-10 05:03:11.000000 yaylib-0.1.2/yaylib/api/review.py
--rw-rw-rw-   0        0        0     3968 2023-06-10 05:03:11.000000 yaylib-0.1.2/yaylib/api/thread.py
--rw-rw-rw-   0        0        0    22815 2023-06-10 05:03:26.000000 yaylib-0.1.2/yaylib/api/user.py
--rw-rw-rw-   0        0        0    76106 2023-06-10 05:03:26.000000 yaylib-0.1.2/yaylib/client.py
--rw-rw-rw-   0        0        0     5732 2023-06-10 05:31:25.000000 yaylib-0.1.2/yaylib/config.py
--rw-rw-rw-   0        0        0      373 2023-06-03 14:25:16.000000 yaylib-0.1.2/yaylib/errors.py
--rw-rw-rw-   0        0        0    50977 2023-06-10 05:03:11.000000 yaylib-0.1.2/yaylib/models.py
--rw-rw-rw-   0        0        0    30969 2023-06-10 05:03:26.000000 yaylib-0.1.2/yaylib/responses.py
--rw-rw-rw-   0        0        0     1079 2023-06-10 05:03:11.000000 yaylib-0.1.2/yaylib/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-10 05:31:49.395664 yaylib-0.1.2/yaylib.egg-info/
--rw-rw-rw-   0        0        0     9580 2023-06-10 05:31:49.000000 yaylib-0.1.2/yaylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      721 2023-06-10 05:31:49.000000 yaylib-0.1.2/yaylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 05:31:49.000000 yaylib-0.1.2/yaylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-10 05:31:49.000000 yaylib-0.1.2/yaylib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-10 05:31:49.000000 yaylib-0.1.2/yaylib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 08:32:04.006271 yaylib-0.1.3/
+-rw-rw-rw-   0        0        0     1088 2023-06-23 06:06:02.000000 yaylib-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     8215 2023-06-25 08:32:04.005228 yaylib-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7358 2023-06-23 12:05:23.000000 yaylib-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 08:32:04.006271 yaylib-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1506 2023-06-25 08:29:29.000000 yaylib-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 08:32:03.970299 yaylib-0.1.3/tests/
+-rw-rw-rw-   0        0        0      229 2023-06-23 06:06:02.000000 yaylib-0.1.3/tests/test_call.py
+-rw-rw-rw-   0        0        0      829 2023-06-23 06:06:02.000000 yaylib-0.1.3/tests/test_cassandra.py
+-rw-rw-rw-   0        0        0      229 2023-06-23 06:06:02.000000 yaylib-0.1.3/tests/test_chat.py
+-rw-rw-rw-   0        0        0      231 2023-06-23 06:06:02.000000 yaylib-0.1.3/tests/test_group.py
+-rw-rw-rw-   0        0        0      229 2023-06-23 06:06:02.000000 yaylib-0.1.3/tests/test_misc.py
+-rw-rw-rw-   0        0        0     2552 2023-06-23 06:06:02.000000 yaylib-0.1.3/tests/test_post.py
+-rw-rw-rw-   0        0        0      922 2023-06-23 06:06:02.000000 yaylib-0.1.3/tests/test_review.py
+-rw-rw-rw-   0        0        0      233 2023-06-23 06:06:02.000000 yaylib-0.1.3/tests/test_thread.py
+-rw-rw-rw-   0        0        0      229 2023-06-23 06:06:02.000000 yaylib-0.1.3/tests/test_user.py
+drwxrwxrwx   0        0        0        0 2023-06-25 08:32:03.977375 yaylib-0.1.3/yaylib/
+-rw-rw-rw-   0        0        0      263 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 08:32:04.004222 yaylib-0.1.3/yaylib/api/
+-rw-rw-rw-   0        0        0      356 2023-05-31 13:14:39.000000 yaylib-0.1.3/yaylib/api/__init__.py
+-rw-rw-rw-   0        0        0     6814 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/api/api.py
+-rw-rw-rw-   0        0        0     7402 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/api/call.py
+-rw-rw-rw-   0        0        0     1393 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/api/cassandra.py
+-rw-rw-rw-   0        0        0    12827 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/api/chat.py
+-rw-rw-rw-   0        0        0    19559 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/api/group.py
+-rw-rw-rw-   0        0        0     4772 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/api/login.py
+-rw-rw-rw-   0        0        0     5831 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/api/misc.py
+-rw-rw-rw-   0        0        0    29363 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/api/post.py
+-rw-rw-rw-   0        0        0     3492 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/api/review.py
+-rw-rw-rw-   0        0        0     4082 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/api/thread.py
+-rw-rw-rw-   0        0        0    21385 2023-06-23 12:05:23.000000 yaylib-0.1.3/yaylib/api/user.py
+-rw-rw-rw-   0        0        0    76772 2023-06-23 12:05:23.000000 yaylib-0.1.3/yaylib/client.py
+-rw-rw-rw-   0        0        0    17844 2023-06-25 08:32:00.000000 yaylib-0.1.3/yaylib/config.py
+-rw-rw-rw-   0        0        0      373 2023-05-23 09:12:41.000000 yaylib-0.1.3/yaylib/errors.py
+-rw-rw-rw-   0        0        0    50892 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/models.py
+-rw-rw-rw-   0        0        0    31265 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/responses.py
+-rw-rw-rw-   0        0        0     1079 2023-06-23 06:06:02.000000 yaylib-0.1.3/yaylib/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-25 08:32:03.990981 yaylib-0.1.3/yaylib.egg-info/
+-rw-rw-rw-   0        0        0     8215 2023-06-25 08:32:03.000000 yaylib-0.1.3/yaylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      721 2023-06-25 08:32:03.000000 yaylib-0.1.3/yaylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 08:32:03.000000 yaylib-0.1.3/yaylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-25 08:32:03.000000 yaylib-0.1.3/yaylib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-25 08:32:03.000000 yaylib-0.1.3/yaylib.egg-info/top_level.txt
```

### Comparing `yaylib-0.1.2/LICENSE` & `yaylib-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yaylib-0.1.2/PKG-INFO` & `yaylib-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 0.1.2
+Version: 0.1.3
 Summary: This Python package provides an easy-to-use interface for accessing data from Yay! (https://yay.space/). With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts.
 Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib
 Author: Qvco, Konn
 Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn
 Maintainer-email: nikola.desuga@gmail.com
@@ -13,31 +13,28 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div><a id="readme-top"></a></div>
-<p align="center">
-    <img src=https://img.shields.io/github/stars/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue />
-    <img src=https://img.shields.io/github/forks/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue />
-    <img src=https://img.shields.io/github/issues/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational />
-    <img src=https://img.shields.io/github/issues-pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational />
-</p>
+<div align="center">
+    <img src="https://img.shields.io/github/stars/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue" />
+    <img src="https://img.shields.io/github/forks/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue" />
+    <img src="https://img.shields.io/github/issues/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational" />
+    <img src="https://img.shields.io/github/issues-pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational" />
+</div>
 <br />
 <p align="center">
-    <a href="https://github.com/othneildrew/Best-README-Template">
+<!--     <a href="https://github.com/othneildrew/Best-README-Template">
         <img src="https://github.com/qvco/yaylib/assets/77382767/6e72ec90-b8e9-40bf-a7ad-34fb2ccea0f9" alt="Logo" height="300px">
-    </a>
-    <!-- <a href="https://github.com/othneildrew/Best-README-Template">
-        <img src="https://github.com/qvco/yaylib/assets/77382767/2cdc26e5-7195-4df3-94c5-db840bdd57ff" alt="Logo" height="300">
-    </a> -->
-    <!-- <a href="https://github.com/othneildrew/Best-README-Template">
-        <img src="https://github.com/qvco/yaylib/assets/77382767/ed3c51a3-1430-4371-b65d-61c161438ee1" alt="Logo" height="300">
     </a> -->
+    <a href="https://github.com/othneildrew/Best-README-Template">
+        <img src="https://github.com/qvco/yaylib/assets/77382767/5265b956-55b7-466c-8cdb-cf0f3abed946" alt="Logo" height="300px">
+    </a>
     <h3 align="center">yaylib</h3>
     <p align="center">
         「<strong>yaylib</strong>」は同世代でつながるチャットアプリ、Yay!（イェイ）の API クライアントです。<br />
         このライブラリを使用することで、あらゆる操作の自動化や、ボットの開発が可能です。
         <br />
         <br />
         <a href="https://github.com/qvco/yaylib/blob/main/docs/README.md">
@@ -50,54 +47,34 @@
         <a href="https://github.com/qvco/yaylib/issues">Request Feature</a>
         ·
         <a href="https://discord.gg/MEuBfNtqRN">Join the discord</a>
     </p>
 </p>
 
 <!-- TABLE OF CONTENTS -->
+
 <details>
   <summary>Table of Contents</summary>
   <ol>
-    <!-- <li><a href="#機能--特徴">機能 & 特徴</a></li> -->
     <li><a href="#buy-me-a-coffee">Buy me a coffee</a></li>
     <li><a href="#インストール">インストール</a></li>
     <li><a href="#使用例">使用例</a></li>
     <li><a href="#yaylib-で誕生したロボットたち">yaylib で誕生したロボットたち</a></li>
     <li><a href="#共同開発について">共同開発について</a></li>
     <li><a href="#免責事項">免責事項</a></li>
     <li><a href="#利用許諾">利用許諾</a></li>
   </ol>
 </details>
 
-<!-- 機能 & 特徴 -->
-
-<!-- ## 機能 & 特徴
-
-そこは将来何しろこんな参考者というのの時よりしでた。何だか結果に堕落児はよくそのらくたですまでで知っばいるにも影響突き抜けますですば、いっそにもしたましだっます。支を至るたものはなお生涯にちょうどありでする。
-
-Here's why:
-
-- しかるに岡田さんで準備本人これから把持に見るたごまかしこの英文いつか発展よりに従ってご意味でしょたでしょですて
-- 否さてお師範をありのしかこれから安泰と始めたて、その会にも申し上げうてという春にあるばいうた
-- そのため書物のうちそんな国家は私上に取り巻かんかと嘉納さんを罹りましん :smile:
-
-TODO:
-
-- 非同期処理に対応
-
-Use the `BLANK_README.md` to get started. -->
-
-<p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
-
 <!-- Buy me a coffee -->
 
 ## Buy me a coffee
 
-もしこのライブラリが気に入っていただけたら  
-私たちに ↓ コーヒー ↓ をお恵みくださいませ！！❤
+もしこのライブラリが気に入っていただけたら、<a href="https://github.com/qvco/yaylib/">ぜひスターをお願いします</a> ⭐️  
+また、Buy Me a Coffee からご支援いただけますと幸いです。
 
 <a href="https://www.buymeacoffee.com/qvco" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
 
 <!-- インストール -->
 
 ## インストール
 
@@ -117,14 +94,16 @@
 cd yaylib
 
 pip install -r requirements.txt
 
 pip install -e .
 ```
 
+「yaylib」の始め方については、[こちら](https://github.com/qvco/yaylib/blob/main/docs/TUTORIAL.md) を確認してください。
+
 <!-- 使用例 -->
 
 ## 使用例
 
 メールアドレスとパスワードを用いてログイン後、新しく投稿を作成するコードです。
 
 ```python
@@ -133,80 +112,72 @@
 api = yaylib.Client()
 
 api.login(email="メールアドレス", password="パスワード")
 
 api.create_post(text="初めての投稿！", color=2)
 ```
 
-より詳細な使用例については、[こちら](https://github.com/qvco/yaylib/blob/master/examples) を参照してください。
+より詳しい使用例については、[こちら](https://github.com/qvco/yaylib/blob/main/examples) を参照してください。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
 
 <!-- yaylib で誕生したボットの一覧 -->
 
 ## yaylib で誕生したロボットたち
 
 yaylib を用いて開発したロボットがある場合は、ぜひ教えてください！
 
 <table align="center">
     <thead>
         <tr>
-            <th>MindReader AI</th>
-            <th>Funktion (架空)</th>
-            <th>香ばしいボット (架空)</th>
+            <th><a href="https://yay.space/user/5855987">MindReader AI</a></th>
+            <th><a href="https://yay.space/user/0">Funktion</a></th>
+            <th><a href="https://yay.space/user/0">香ばしいボット</a></th>
         </tr>
     </thead>
     <tbody>
         <tr>
             <td align="center">
-                <a href="https://yay.space/user/5855987"><img src="https://github.com/qvco/yaylib/assets/77382767/472febe4-4c5f-490c-8417-de0d5dbbbc72" width="200px"></a>
+                <img src="https://github.com/qvco/yaylib/assets/77382767/472febe4-4c5f-490c-8417-de0d5dbbbc72" width="200px">
                 <br />
                 <p>開発者: <a href="https://yay.space/user/35152">毛の可能性</a></p>
             </td>
             <td align="center">
-                <a href="https://yay.space/user/0"><img src="https://github.com/qvco/yaylib/assets/77382767/ff207016-21bf-4e76-b0e0-f70ebc4a121f" width="200px"></a>
+                <img src="https://github.com/qvco/yaylib/assets/77382767/ff207016-21bf-4e76-b0e0-f70ebc4a121f" width="200px">
                 <br />
                 <p>開発者: <a href="https://yay.space/user/0">ぺゅー</a></p>
             </td>
             <td align="center">
-                <a href="https://yay.space/user/0"><img src="https://github.com/qvco/yaylib/assets/77382767/2324e518-b2c8-43cd-95e5-90ee2383aec1" width="200px"></a>
+                <img src="https://github.com/qvco/yaylib/assets/77382767/2324e518-b2c8-43cd-95e5-90ee2383aec1" width="200px">
                 <br />
                 <p>開発者: <a href="https://yay.space/user/0">めんぶれ天然水。</a></p>
             </td>
         </tr>
     </tbody>
 </table>
 
 <!-- 共同開発について -->
 
 ## 共同開発について
 
 私たちと一緒に開発することに興味を持っていただけているなら大歓迎です。
 
 - <a href="https://github.com/qvco/yaylib/pulls">プルリクエストを送信する</a>
-- nikola.desuga@gmail.com にメールを送信する
+- <a href="mailto:nikola.desuga@gmail.com">nikola.desuga@gmail.com</a> にメールを送信する
 - <a href="https://discord.gg/MEuBfNtqRN">Discord サーバーに参加する</a>
 
-のいずれかの方法でコンタクトしてください！
-
-<!-- サポート -->
-
-<!-- ## サポート
-
-Whether you use this project, have learned something from it, or just like it, please consider supporting it by buying me a coffee, so I can dedicate more time on open-source projects like this :)
-
-<a href="https://www.buymeacoffee.com/" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a> -->
+のいずれかの方法でコンタクトしてください。詳しくは[こちら](https://github.com/qvco/yaylib/blob/main/CONTRIBUTING.md)から！
 
 <!-- 免責事項 -->
 
 ## 免責事項
 
 yaylib は、API の公式なサポートやメンテナンスを提供するものではありません。このクライアントを使用する場合、利用者は**リスクや責任を自己負担**できるものとします。このクライアントによって提供される情報やデータの正確性、信頼性、完全性、適時性について、いかなる保証も行いません。また、このクライアントの使用によって生じた損害や不利益について、一切の責任を負いかねます。利用者は自己の責任において、このクライアントを使用し、API にアクセスするものとします。なお、この免責事項は予告なく変更される場合があります。
 
 <!-- 利用許諾 -->
 
 ## 利用許諾
 
-フルライセンスは [こちら](https://github.com/qvco/yaylib/blob/master/LICENSE) からご確認いただけます。  
+フルライセンスは [こちら](https://github.com/qvco/yaylib/blob/main/LICENSE) からご確認いただけます。  
 このプロジェクトは、 **【MIT ライセンス】** の条件の下でライセンスされています。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yaylib Version: 0.1.2 Summary: This Python package
+Metadata-Version: 2.1 Name: yaylib Version: 0.1.3 Summary: This Python package
 provides an easy-to-use interface for accessing data from Yay! (https://
 yay.space/). With this API Client, you can retrieve user profiles, posts,
 comments, and other content from Yay!, as well as perform common tasks like
 liking and commenting on posts. Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib Author: Qvco, Konn Author-email:
 nikola.desuga@gmail.com Maintainer: Qvco, Konn Maintainer-email:
 nikola.desuga@gmail.com License: MIT Keywords:
@@ -13,15 +13,15 @@
         [https://img.shields.io/github/stars/qvco/yaylib?style=for-the-
   badge&logo=appveyor&color=blue] [https://img.shields.io/github/forks/qvco/
  yaylib?style=for-the-badge&logo=appveyor&color=blue] [https://img.shields.io/
                    github/issues/qvco/yaylib?style=for-the-
 badge&logo=appveyor&color=informational] [https://img.shields.io/github/issues-
      pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational]
 
-                                   [Logo]
+                                     [Logo]
                                **** yaylib ****
 ãyaylibãã¯åä¸ä»£ã§ã¤ãªãããã£ããã¢ããªãYay!ï¼ã¤ã§ã¤ï¼ã®
                         API ã¯ã©ã¤ã¢ã³ãã§ãã
 ãã®ã©ã¤ãã©ãªãä½¿ç¨ãããã¨ã§ãããããæä½ã®èªååãããããã®éçºãå¯è½ã§ãã
 
 
           è©³ããæ©è½ã®è©³ç´°ãä½¿ãæ¹ã¯ãã¡ããã_Â»
@@ -31,46 +31,48 @@
    1. Buy_me_a_coffee
    2. ã¤ã³ã¹ãã¼ã«
    3. ä½¿ç¨ä¾
    4. yaylib_ã§èªçããã­ããããã¡
    5. å±åéçºã«ã¤ãã¦
    6. åè²¬äºé 
    7. å©ç¨è¨±è«¾
-
-                                                           (ãããã«æ»ã)
- ## Buy me a coffee
-ãããã®ã©ã¤ãã©ãªãæ°ã«å¥ã£ã¦ããã ããã ç§ãã¡ã«
-â ã³ã¼ãã¼ â ããæµã¿ãã ããã¾ãï¼ï¼â¤ [Buy_Me_A_Coffee]
-## ã¤ã³ã¹ãã¼ã« **â» Python 3.11
+  ## Buy me a coffee
+ãããã®ã©ã¤ãã©ãªãæ°ã«å¥ã£ã¦ããã ãããããã²ã¹ã¿ã¼ããé¡ããã¾ã
+â­ï¸ ã¾ããBuy Me a Coffee
+ãããæ¯æ´ããã ãã¾ãã¨å¹¸ãã§ãã [Buy_Me_A_Coffee]  ##
+ã¤ã³ã¹ãã¼ã« **â» Python 3.11
 ãããä»¥ä¸ã®ãã¼ã¸ã§ã³ãå¿è¦ã§ãã**
 ã©ã¤ãã©ãªãã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®ã³ãã³ããå®è¡ãã¾ã:
 ```bash pip install yaylib ```
 éçºãã¼ã¸ã§ã³ãã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®æé ãå®è¡ãã¾ã:
 ```bash git clone https://github.com/qvco/yaylib cd yaylib pip install -
-r requirements.txt pip install -e . ```  ## ä½¿ç¨ä¾
+r requirements.txt pip install -e . ```
+ãyaylibãã®å§ãæ¹ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
+yaylib/blob/main/docs/TUTORIAL.md) ãç¢ºèªãã¦ãã ããã  ## ä½¿ç¨ä¾
 ã¡ã¼ã«ã¢ãã¬ã¹ã¨ãã¹ã¯ã¼ããç¨ãã¦ã­ã°ã¤ã³å¾ãæ°ããæç¨¿ãä½æããã³ã¼ãã§ãã
 ```python import yaylib api = yaylib.Client() api.login
 (email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") api.create_post
 (text="åãã¦ã®æç¨¿ï¼", color=2) ```
-ããè©³ç´°ãªä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
-yaylib/blob/master/examples) ãåç§ãã¦ãã ããã
+ããè©³ããä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
+yaylib/blob/main/examples) ãåç§ãã¦ãã ããã
                                                            (ãããã«æ»ã)
  ## yaylib ã§èªçããã­ããããã¡ yaylib
 ãç¨ãã¦éçºããã­ããããããå ´åã¯ããã²æãã¦ãã ããï¼
-MindReader AI                                      Funktion (æ¶ç©º)                é¦ã°ããããã (æ¶ç©º)
+MindReader_AI                                      Funktion                               é¦ã°ããããã
  [https://github.com/qvco/yaylib/assets/77382767/     [https://github.com/qvco/yaylib/    [https://github.com/qvco/yaylib/assets/77382767/2324e518-b2c8-43cd-
       472febe4-4c5f-490c-8417-de0d5dbbbc72]         assets/77382767/ff207016-21bf-4e76-                           95e5-90ee2383aec1]
             éçºè: æ¯ã®å¯�         b0e0-f70ebc4a121f]                            éçºè: ããã¶ãå¤©ç¶æ°´ã
                                                             éçºè: ãºãã¼
  ## å±åéçºã«ã¤ãã¦
 ç§ãã¡ã¨ä¸ç·ã«éçºãããã¨ã«èå³ãæã£ã¦ããã ãã¦ãããªãå¤§æ­è¿ã§ãã
 - ãã«ãªã¯ã¨ã¹ããéä¿¡ãã - nikola.desuga@gmail.com
 ã«ã¡ã¼ã«ãéä¿¡ãã - Discord_ãµã¼ãã¼ã«åå ãã
-ã®ããããã®æ¹æ³ã§ã³ã³ã¿ã¯ããã¦ãã ããï¼    ##
-åè²¬äºé  yaylib ã¯ãAPI
+ã®ããããã®æ¹æ³ã§ã³ã³ã¿ã¯ããã¦ãã ãããè©³ããã¯
+[ãã¡ã](https://github.com/qvco/yaylib/blob/main/CONTRIBUTING.md)ããï¼
+## åè²¬äºé  yaylib ã¯ãAPI
 ã®å¬å¼ãªãµãã¼ããã¡ã³ããã³ã¹ãæä¾ãããã®ã§ã¯ããã¾ããããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããå ´åãå©ç¨èã¯**ãªã¹ã¯ãè²¬ä»»ãèªå·±è² æ**ã§ãããã®ã¨ãã¾ãããã®ã¯ã©ã¤ã¢ã³ãã«ãã£ã¦æä¾ãããæå ±ããã¼ã¿ã®æ­£ç¢ºæ§ãä¿¡é ¼æ§ãå®å¨æ§ãé©ææ§ã«ã¤ãã¦ããããªãä¿è¨¼ãè¡ãã¾ãããã¾ãããã®ã¯ã©ã¤ã¢ã³ãã®ä½¿ç¨ã«ãã£ã¦çããæå®³ãä¸å©çã«ã¤ãã¦ãä¸åã®è²¬ä»»ãè² ããã­ã¾ããå©ç¨èã¯èªå·±ã®è²¬ä»»ã«ããã¦ããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããAPI
 ã«ã¢ã¯ã»ã¹ãããã®ã¨ãã¾ãããªãããã®åè²¬äºé ã¯äºåãªãå¤æ´ãããå ´åãããã¾ãã
 ## å©ç¨è¨±è«¾ ãã«ã©ã¤ã»ã³ã¹ã¯ [ãã¡ã](https://github.com/qvco/
-yaylib/blob/master/LICENSE) ãããç¢ºèªããã ãã¾ãã
+yaylib/blob/main/LICENSE) ãããç¢ºèªããã ãã¾ãã
 ãã®ãã­ã¸ã§ã¯ãã¯ã **ãMIT ã©ã¤ã»ã³ã¹ã**
 ã®æ¡ä»¶ã®ä¸ã§ã©ã¤ã»ã³ã¹ããã¦ãã¾ãã
                                                            (ãããã«æ»ã)
```

### Comparing `yaylib-0.1.2/README.md` & `yaylib-0.1.3/yaylib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,40 @@
+Metadata-Version: 2.1
+Name: yaylib
+Version: 0.1.3
+Summary: This Python package provides an easy-to-use interface for accessing data from Yay! (https://yay.space/). With this API Client, you can retrieve user profiles, posts, comments, and other content from Yay!, as well as perform common tasks like liking and commenting on posts.
+Home-page: https://github.com/qvco/yaylib
+Download-URL: https://github.com/qvco/yaylib
+Author: Qvco, Konn
+Author-email: nikola.desuga@gmail.com
+Maintainer: Qvco, Konn
+Maintainer-email: nikola.desuga@gmail.com
+License: MIT
+Keywords: yay,yaylib,api,bot,library,wrapper,ボット,ライブラリ
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div><a id="readme-top"></a></div>
-<p align="center">
-    <img src=https://img.shields.io/github/stars/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue />
-    <img src=https://img.shields.io/github/forks/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue />
-    <img src=https://img.shields.io/github/issues/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational />
-    <img src=https://img.shields.io/github/issues-pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational />
-</p>
+<div align="center">
+    <img src="https://img.shields.io/github/stars/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue" />
+    <img src="https://img.shields.io/github/forks/qvco/yaylib?style=for-the-badge&logo=appveyor&color=blue" />
+    <img src="https://img.shields.io/github/issues/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational" />
+    <img src="https://img.shields.io/github/issues-pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational" />
+</div>
 <br />
 <p align="center">
-    <a href="https://github.com/othneildrew/Best-README-Template">
+<!--     <a href="https://github.com/othneildrew/Best-README-Template">
         <img src="https://github.com/qvco/yaylib/assets/77382767/6e72ec90-b8e9-40bf-a7ad-34fb2ccea0f9" alt="Logo" height="300px">
-    </a>
-    <!-- <a href="https://github.com/othneildrew/Best-README-Template">
-        <img src="https://github.com/qvco/yaylib/assets/77382767/2cdc26e5-7195-4df3-94c5-db840bdd57ff" alt="Logo" height="300">
-    </a> -->
-    <!-- <a href="https://github.com/othneildrew/Best-README-Template">
-        <img src="https://github.com/qvco/yaylib/assets/77382767/ed3c51a3-1430-4371-b65d-61c161438ee1" alt="Logo" height="300">
     </a> -->
+    <a href="https://github.com/othneildrew/Best-README-Template">
+        <img src="https://github.com/qvco/yaylib/assets/77382767/5265b956-55b7-466c-8cdb-cf0f3abed946" alt="Logo" height="300px">
+    </a>
     <h3 align="center">yaylib</h3>
     <p align="center">
         「<strong>yaylib</strong>」は同世代でつながるチャットアプリ、Yay!（イェイ）の API クライアントです。<br />
         このライブラリを使用することで、あらゆる操作の自動化や、ボットの開発が可能です。
         <br />
         <br />
         <a href="https://github.com/qvco/yaylib/blob/main/docs/README.md">
@@ -32,54 +47,34 @@
         <a href="https://github.com/qvco/yaylib/issues">Request Feature</a>
         ·
         <a href="https://discord.gg/MEuBfNtqRN">Join the discord</a>
     </p>
 </p>
 
 <!-- TABLE OF CONTENTS -->
+
 <details>
   <summary>Table of Contents</summary>
   <ol>
-    <!-- <li><a href="#機能--特徴">機能 & 特徴</a></li> -->
     <li><a href="#buy-me-a-coffee">Buy me a coffee</a></li>
     <li><a href="#インストール">インストール</a></li>
     <li><a href="#使用例">使用例</a></li>
     <li><a href="#yaylib-で誕生したロボットたち">yaylib で誕生したロボットたち</a></li>
     <li><a href="#共同開発について">共同開発について</a></li>
     <li><a href="#免責事項">免責事項</a></li>
     <li><a href="#利用許諾">利用許諾</a></li>
   </ol>
 </details>
 
-<!-- 機能 & 特徴 -->
-
-<!-- ## 機能 & 特徴
-
-そこは将来何しろこんな参考者というのの時よりしでた。何だか結果に堕落児はよくそのらくたですまでで知っばいるにも影響突き抜けますですば、いっそにもしたましだっます。支を至るたものはなお生涯にちょうどありでする。
-
-Here's why:
-
-- しかるに岡田さんで準備本人これから把持に見るたごまかしこの英文いつか発展よりに従ってご意味でしょたでしょですて
-- 否さてお師範をありのしかこれから安泰と始めたて、その会にも申し上げうてという春にあるばいうた
-- そのため書物のうちそんな国家は私上に取り巻かんかと嘉納さんを罹りましん :smile:
-
-TODO:
-
-- 非同期処理に対応
-
-Use the `BLANK_README.md` to get started. -->
-
-<p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
-
 <!-- Buy me a coffee -->
 
 ## Buy me a coffee
 
-もしこのライブラリが気に入っていただけたら  
-私たちに ↓ コーヒー ↓ をお恵みくださいませ！！❤
+もしこのライブラリが気に入っていただけたら、<a href="https://github.com/qvco/yaylib/">ぜひスターをお願いします</a> ⭐️  
+また、Buy Me a Coffee からご支援いただけますと幸いです。
 
 <a href="https://www.buymeacoffee.com/qvco" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
 
 <!-- インストール -->
 
 ## インストール
 
@@ -99,14 +94,16 @@
 cd yaylib
 
 pip install -r requirements.txt
 
 pip install -e .
 ```
 
+「yaylib」の始め方については、[こちら](https://github.com/qvco/yaylib/blob/main/docs/TUTORIAL.md) を確認してください。
+
 <!-- 使用例 -->
 
 ## 使用例
 
 メールアドレスとパスワードを用いてログイン後、新しく投稿を作成するコードです。
 
 ```python
@@ -115,80 +112,72 @@
 api = yaylib.Client()
 
 api.login(email="メールアドレス", password="パスワード")
 
 api.create_post(text="初めての投稿！", color=2)
 ```
 
-より詳細な使用例については、[こちら](https://github.com/qvco/yaylib/blob/master/examples) を参照してください。
+より詳しい使用例については、[こちら](https://github.com/qvco/yaylib/blob/main/examples) を参照してください。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
 
 <!-- yaylib で誕生したボットの一覧 -->
 
 ## yaylib で誕生したロボットたち
 
 yaylib を用いて開発したロボットがある場合は、ぜひ教えてください！
 
 <table align="center">
     <thead>
         <tr>
-            <th>MindReader AI</th>
-            <th>Funktion (架空)</th>
-            <th>香ばしいボット (架空)</th>
+            <th><a href="https://yay.space/user/5855987">MindReader AI</a></th>
+            <th><a href="https://yay.space/user/0">Funktion</a></th>
+            <th><a href="https://yay.space/user/0">香ばしいボット</a></th>
         </tr>
     </thead>
     <tbody>
         <tr>
             <td align="center">
-                <a href="https://yay.space/user/5855987"><img src="https://github.com/qvco/yaylib/assets/77382767/472febe4-4c5f-490c-8417-de0d5dbbbc72" width="200px"></a>
+                <img src="https://github.com/qvco/yaylib/assets/77382767/472febe4-4c5f-490c-8417-de0d5dbbbc72" width="200px">
                 <br />
                 <p>開発者: <a href="https://yay.space/user/35152">毛の可能性</a></p>
             </td>
             <td align="center">
-                <a href="https://yay.space/user/0"><img src="https://github.com/qvco/yaylib/assets/77382767/ff207016-21bf-4e76-b0e0-f70ebc4a121f" width="200px"></a>
+                <img src="https://github.com/qvco/yaylib/assets/77382767/ff207016-21bf-4e76-b0e0-f70ebc4a121f" width="200px">
                 <br />
                 <p>開発者: <a href="https://yay.space/user/0">ぺゅー</a></p>
             </td>
             <td align="center">
-                <a href="https://yay.space/user/0"><img src="https://github.com/qvco/yaylib/assets/77382767/2324e518-b2c8-43cd-95e5-90ee2383aec1" width="200px"></a>
+                <img src="https://github.com/qvco/yaylib/assets/77382767/2324e518-b2c8-43cd-95e5-90ee2383aec1" width="200px">
                 <br />
                 <p>開発者: <a href="https://yay.space/user/0">めんぶれ天然水。</a></p>
             </td>
         </tr>
     </tbody>
 </table>
 
 <!-- 共同開発について -->
 
 ## 共同開発について
 
 私たちと一緒に開発することに興味を持っていただけているなら大歓迎です。
 
 - <a href="https://github.com/qvco/yaylib/pulls">プルリクエストを送信する</a>
-- nikola.desuga@gmail.com にメールを送信する
+- <a href="mailto:nikola.desuga@gmail.com">nikola.desuga@gmail.com</a> にメールを送信する
 - <a href="https://discord.gg/MEuBfNtqRN">Discord サーバーに参加する</a>
 
-のいずれかの方法でコンタクトしてください！
-
-<!-- サポート -->
-
-<!-- ## サポート
-
-Whether you use this project, have learned something from it, or just like it, please consider supporting it by buying me a coffee, so I can dedicate more time on open-source projects like this :)
-
-<a href="https://www.buymeacoffee.com/" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a> -->
+のいずれかの方法でコンタクトしてください。詳しくは[こちら](https://github.com/qvco/yaylib/blob/main/CONTRIBUTING.md)から！
 
 <!-- 免責事項 -->
 
 ## 免責事項
 
 yaylib は、API の公式なサポートやメンテナンスを提供するものではありません。このクライアントを使用する場合、利用者は**リスクや責任を自己負担**できるものとします。このクライアントによって提供される情報やデータの正確性、信頼性、完全性、適時性について、いかなる保証も行いません。また、このクライアントの使用によって生じた損害や不利益について、一切の責任を負いかねます。利用者は自己の責任において、このクライアントを使用し、API にアクセスするものとします。なお、この免責事項は予告なく変更される場合があります。
 
 <!-- 利用許諾 -->
 
 ## 利用許諾
 
-フルライセンスは [こちら](https://github.com/qvco/yaylib/blob/master/LICENSE) からご確認いただけます。  
+フルライセンスは [こちら](https://github.com/qvco/yaylib/blob/main/LICENSE) からご確認いただけます。  
 このプロジェクトは、 **【MIT ライセンス】** の条件の下でライセンスされています。
 
 <p align="right">(<a href="#readme-top">トップに戻る</a>)</p>
```

#### html2text {}

```diff
@@ -1,15 +1,27 @@
+Metadata-Version: 2.1 Name: yaylib Version: 0.1.3 Summary: This Python package
+provides an easy-to-use interface for accessing data from Yay! (https://
+yay.space/). With this API Client, you can retrieve user profiles, posts,
+comments, and other content from Yay!, as well as perform common tasks like
+liking and commenting on posts. Home-page: https://github.com/qvco/yaylib
+Download-URL: https://github.com/qvco/yaylib Author: Qvco, Konn Author-email:
+nikola.desuga@gmail.com Maintainer: Qvco, Konn Maintainer-email:
+nikola.desuga@gmail.com License: MIT Keywords:
+yay,yaylib,api,bot,library,wrapper,ããã,ã©ã¤ãã©ãª Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.11 Description-
+Content-Type: text/markdown License-File: LICENSE
         [https://img.shields.io/github/stars/qvco/yaylib?style=for-the-
   badge&logo=appveyor&color=blue] [https://img.shields.io/github/forks/qvco/
  yaylib?style=for-the-badge&logo=appveyor&color=blue] [https://img.shields.io/
                    github/issues/qvco/yaylib?style=for-the-
 badge&logo=appveyor&color=informational] [https://img.shields.io/github/issues-
      pr/qvco/yaylib?style=for-the-badge&logo=appveyor&color=informational]
 
-                                   [Logo]
+                                     [Logo]
                                **** yaylib ****
 ãyaylibãã¯åä¸ä»£ã§ã¤ãªãããã£ããã¢ããªãYay!ï¼ã¤ã§ã¤ï¼ã®
                         API ã¯ã©ã¤ã¢ã³ãã§ãã
 ãã®ã©ã¤ãã©ãªãä½¿ç¨ãããã¨ã§ãããããæä½ã®èªååãããããã®éçºãå¯è½ã§ãã
 
 
           è©³ããæ©è½ã®è©³ç´°ãä½¿ãæ¹ã¯ãã¡ããã_Â»
@@ -19,46 +31,48 @@
    1. Buy_me_a_coffee
    2. ã¤ã³ã¹ãã¼ã«
    3. ä½¿ç¨ä¾
    4. yaylib_ã§èªçããã­ããããã¡
    5. å±åéçºã«ã¤ãã¦
    6. åè²¬äºé 
    7. å©ç¨è¨±è«¾
-
-                                                           (ãããã«æ»ã)
- ## Buy me a coffee
-ãããã®ã©ã¤ãã©ãªãæ°ã«å¥ã£ã¦ããã ããã ç§ãã¡ã«
-â ã³ã¼ãã¼ â ããæµã¿ãã ããã¾ãï¼ï¼â¤ [Buy_Me_A_Coffee]
-## ã¤ã³ã¹ãã¼ã« **â» Python 3.11
+  ## Buy me a coffee
+ãããã®ã©ã¤ãã©ãªãæ°ã«å¥ã£ã¦ããã ãããããã²ã¹ã¿ã¼ããé¡ããã¾ã
+â­ï¸ ã¾ããBuy Me a Coffee
+ãããæ¯æ´ããã ãã¾ãã¨å¹¸ãã§ãã [Buy_Me_A_Coffee]  ##
+ã¤ã³ã¹ãã¼ã« **â» Python 3.11
 ãããä»¥ä¸ã®ãã¼ã¸ã§ã³ãå¿è¦ã§ãã**
 ã©ã¤ãã©ãªãã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®ã³ãã³ããå®è¡ãã¾ã:
 ```bash pip install yaylib ```
 éçºãã¼ã¸ã§ã³ãã¤ã³ã¹ãã¼ã«ããã«ã¯ãä»¥ä¸ã®æé ãå®è¡ãã¾ã:
 ```bash git clone https://github.com/qvco/yaylib cd yaylib pip install -
-r requirements.txt pip install -e . ```  ## ä½¿ç¨ä¾
+r requirements.txt pip install -e . ```
+ãyaylibãã®å§ãæ¹ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
+yaylib/blob/main/docs/TUTORIAL.md) ãç¢ºèªãã¦ãã ããã  ## ä½¿ç¨ä¾
 ã¡ã¼ã«ã¢ãã¬ã¹ã¨ãã¹ã¯ã¼ããç¨ãã¦ã­ã°ã¤ã³å¾ãæ°ããæç¨¿ãä½æããã³ã¼ãã§ãã
 ```python import yaylib api = yaylib.Client() api.login
 (email="ã¡ã¼ã«ã¢ãã¬ã¹", password="ãã¹ã¯ã¼ã") api.create_post
 (text="åãã¦ã®æç¨¿ï¼", color=2) ```
-ããè©³ç´°ãªä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
-yaylib/blob/master/examples) ãåç§ãã¦ãã ããã
+ããè©³ããä½¿ç¨ä¾ã«ã¤ãã¦ã¯ã[ãã¡ã](https://github.com/qvco/
+yaylib/blob/main/examples) ãåç§ãã¦ãã ããã
                                                            (ãããã«æ»ã)
  ## yaylib ã§èªçããã­ããããã¡ yaylib
 ãç¨ãã¦éçºããã­ããããããå ´åã¯ããã²æãã¦ãã ããï¼
-MindReader AI                                      Funktion (æ¶ç©º)                é¦ã°ããããã (æ¶ç©º)
+MindReader_AI                                      Funktion                               é¦ã°ããããã
  [https://github.com/qvco/yaylib/assets/77382767/     [https://github.com/qvco/yaylib/    [https://github.com/qvco/yaylib/assets/77382767/2324e518-b2c8-43cd-
       472febe4-4c5f-490c-8417-de0d5dbbbc72]         assets/77382767/ff207016-21bf-4e76-                           95e5-90ee2383aec1]
             éçºè: æ¯ã®å¯�         b0e0-f70ebc4a121f]                            éçºè: ããã¶ãå¤©ç¶æ°´ã
                                                             éçºè: ãºãã¼
  ## å±åéçºã«ã¤ãã¦
 ç§ãã¡ã¨ä¸ç·ã«éçºãããã¨ã«èå³ãæã£ã¦ããã ãã¦ãããªãå¤§æ­è¿ã§ãã
 - ãã«ãªã¯ã¨ã¹ããéä¿¡ãã - nikola.desuga@gmail.com
 ã«ã¡ã¼ã«ãéä¿¡ãã - Discord_ãµã¼ãã¼ã«åå ãã
-ã®ããããã®æ¹æ³ã§ã³ã³ã¿ã¯ããã¦ãã ããï¼    ##
-åè²¬äºé  yaylib ã¯ãAPI
+ã®ããããã®æ¹æ³ã§ã³ã³ã¿ã¯ããã¦ãã ãããè©³ããã¯
+[ãã¡ã](https://github.com/qvco/yaylib/blob/main/CONTRIBUTING.md)ããï¼
+## åè²¬äºé  yaylib ã¯ãAPI
 ã®å¬å¼ãªãµãã¼ããã¡ã³ããã³ã¹ãæä¾ãããã®ã§ã¯ããã¾ããããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããå ´åãå©ç¨èã¯**ãªã¹ã¯ãè²¬ä»»ãèªå·±è² æ**ã§ãããã®ã¨ãã¾ãããã®ã¯ã©ã¤ã¢ã³ãã«ãã£ã¦æä¾ãããæå ±ããã¼ã¿ã®æ­£ç¢ºæ§ãä¿¡é ¼æ§ãå®å¨æ§ãé©ææ§ã«ã¤ãã¦ããããªãä¿è¨¼ãè¡ãã¾ãããã¾ãããã®ã¯ã©ã¤ã¢ã³ãã®ä½¿ç¨ã«ãã£ã¦çããæå®³ãä¸å©çã«ã¤ãã¦ãä¸åã®è²¬ä»»ãè² ããã­ã¾ããå©ç¨èã¯èªå·±ã®è²¬ä»»ã«ããã¦ããã®ã¯ã©ã¤ã¢ã³ããä½¿ç¨ããAPI
 ã«ã¢ã¯ã»ã¹ãããã®ã¨ãã¾ãããªãããã®åè²¬äºé ã¯äºåãªãå¤æ´ãããå ´åãããã¾ãã
 ## å©ç¨è¨±è«¾ ãã«ã©ã¤ã»ã³ã¹ã¯ [ãã¡ã](https://github.com/qvco/
-yaylib/blob/master/LICENSE) ãããç¢ºèªããã ãã¾ãã
+yaylib/blob/main/LICENSE) ãããç¢ºèªããã ãã¾ãã
 ãã®ãã­ã¸ã§ã¯ãã¯ã **ãMIT ã©ã¤ã»ã³ã¹ã**
 ã®æ¡ä»¶ã®ä¸ã§ã©ã¤ã»ã³ã¹ããã¦ãã¾ãã
                                                            (ãããã«æ»ã)
```

### Comparing `yaylib-0.1.2/setup.py` & `yaylib-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,16 @@
     "library",
     "wrapper",
     "ボット",
     "ライブラリ"
 ]
 
 install_requires = [
-    "httpx>=0.17.1"
+    "httpx>=0.17.1",
+    "Pillow>=9.3.0"
 ]
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
 ]
```

### Comparing `yaylib-0.1.2/tests/test_cassandra.py` & `yaylib-0.1.3/tests/test_cassandra.py`

 * *Files identical despite different names*

### Comparing `yaylib-0.1.2/tests/test_post.py` & `yaylib-0.1.3/tests/test_post.py`

 * *Files identical despite different names*

### Comparing `yaylib-0.1.2/tests/test_review.py` & `yaylib-0.1.3/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `yaylib-0.1.2/yaylib/api/api.py` & `yaylib-0.1.3/yaylib/api/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import time
 import logging
 
 from json import JSONDecodeError
 from typing import Optional, Dict, Any
 
 import httpx
 
@@ -18,15 +19,18 @@
 class API:
 
     def __init__(
             self,
             access_token: str = None,
             refresh_token: str = None,
             proxy: str = None,
-            timeout=60,
+            max_retries=3,
+            backoff_factor=1.0,
+            timeout=30,
+            lang="ja",
             base_path=current_path,
             loglevel_stream=logging.INFO,
             host=Configs.YAY_PRODUCTION_HOST,
     ):
         self.yaylib_version = Configs.YAYLIB_VERSION
         self.api_version = Configs.YAY_API_VERSION
         self.api_key = Configs.YAY_API_KEY
@@ -36,15 +40,19 @@
             "refresh_token": refresh_token,
         })
 
         self.proxy = {}
         if proxy is not None:
             self.proxy["https"] = proxy
 
+        self.max_retries = max_retries
+        self.retry_statuses = [500, 502, 503, 504]
+        self.backoff_factor = backoff_factor
         self.timeout = timeout
+        self.lang = lang
         self.base_path = base_path
         self.host = "https://" + host
 
         self.generate_all_uuids()
         self.session = httpx.Client(proxies=self.proxy, timeout=self.timeout)
         self.session.headers.update(Configs.REQUEST_HEADERS)
         self.session.headers.update({"X-Device-Uuid": self.device_uuid})
@@ -76,39 +84,58 @@
     def request(self, method, endpoint, params=None, payload=None, user_auth=True, headers=None):
 
         if headers is None:
             headers = self.session.headers
         if not user_auth:
             headers["Authorization"] = None
 
-        self.logger.debug(
-            "Making API request:\n\n"
-            f"{method}: {endpoint}\n\n"
-            f"Parameters: {params}\n\n"
-            f"Headers: {headers}\n\n"
-            f"Body: {payload}\n"
-        )
-
-        response = self.session.request(
-            method, endpoint, params=params, json=payload, headers=headers
-        )
+        response = None
+        backoff_duration = 0
 
-        self.logger.debug(
-            "Received API response:\n\n"
-            f"Status Code: {response.status_code}\n\n"
-            f"Headers: {response.headers}\n\n"
-            f"Response: {response.text}\n"
-        )
-        self._handle_response(response)
+        for i in range(self.max_retries):
+            time.sleep(backoff_duration)
+            try:
+
+                self.logger.debug(
+                    "Making API request:\n\n"
+                    f"{method}: {endpoint}\n\n"
+                    f"Parameters: {params}\n\n"
+                    f"Headers: {headers}\n\n"
+                    f"Body: {payload}\n"
+                )
+                response = self.session.request(
+                    method, endpoint, params=params, json=payload, headers=headers
+                )
+                self.logger.debug(
+                    "Received API response:\n\n"
+                    f"Status Code: {response.status_code}\n\n"
+                    f"Headers: {response.headers}\n\n"
+                    f"Response: {response.text}\n"
+                )
+
+                if response.status_code not in self.retry_statuses:
+                    break
+
+            except httpx.HTTPError:
+                pass
+
+            if response is not None:
+                self.logger.error(
+                    f"Request failed with status code {response.status_code}. Retrying...")
+            else:
+                self.logger.error("Request failed. Retrying...")
+            backoff_duration = self.backoff_factor * (2 ** i)
 
         try:
-            return response.json()
+            json_response = response.json()
         except JSONDecodeError:
             return response.text
 
+        return self._handle_response(response, json_response)
+
     def _make_request(
             self, method: str, endpoint: str, params: dict = None,
             payload: dict = None, data_type=None, user_auth=True, headers=None
     ):
         response = self.request(
             method, endpoint, params, payload, user_auth, headers
         )
@@ -125,27 +152,43 @@
         return data
 
     def _check_authorization(self) -> None:
         if self.session.headers.get("Authorization") is None:
             raise AuthenticationError(
                 "Authorization is not present in the header.")
 
-    def _handle_response(self, response):
+    def _handle_response(self, response, json_response):
+        translated_response = self.translate_error_message(json_response)
         if response.status_code == 400:
-            raise BadRequestError(response.text)
+            raise BadRequestError(translated_response)
         if response.status_code == 401:
-            raise AuthenticationError(response.text)
+            raise AuthenticationError(translated_response)
         if response.status_code == 403:
-            raise ForbiddenError(response.text)
+            raise ForbiddenError(translated_response)
         if response.status_code == 404:
-            raise NotFoundError(response.text)
+            raise NotFoundError(translated_response)
         if response.status_code == 429:
-            raise RateLimitError(response.text)
+            raise RateLimitError(translated_response)
         if response.status_code == 500:
-            raise YayServerError(response.text)
+            raise YayServerError(translated_response)
         if response.status_code and not 200 <= response.status_code < 300:
-            raise HTTPError(response.text)
-        return response
+            raise HTTPError(translated_response)
+        return json_response
+
+    def translate_error_message(self, response):
+        if self.lang == "ja":
+            try:
+                error_code = response.get("error_code", None)
+                if error_code is not None:
+                    error_type = ErrorType(error_code)
+                    if error_type.name in ErrorMessage.__members__:
+                        error_message = ErrorMessage[error_type.name].value
+                        response["message"] = error_message
+                return response
+            except ValueError:
+                return response
+        else:
+            return response
 
     def generate_all_uuids(self):
         self.device_uuid = generate_uuid()[0]
         self.uuid, self.url_uuid = generate_uuid()
```

### Comparing `yaylib-0.1.2/yaylib/api/call.py` & `yaylib-0.1.3/yaylib/api/call.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     params = {}
     if group_id:
         params["group_id"] = group_id
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.CALLS_V1}/{call_id}/bulk_invite",
         params=params
     )
-    self.logger.info("Invited to call bulk.")
+    self.logger.info("Invited your online followings to the call.")
     return response
 
 
 def invite_users_to_call(self, call_id: int, user_ids: List[int]):
     """
 
     Parameters
@@ -139,15 +139,15 @@
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.CALLS_V1}/conference_calls/{call_id}/invite",
         payload={
             "call_id": call_id,
             "user_ids[]": user_ids
         }
     )
-    self.logger.info("Invitation sent.")
+    self.logger.info("Invited users to call.")
     return response
 
 
 def invite_users_to_chat_call(
         self,
         chat_room_id: int,
         room_id: int,
@@ -157,15 +157,15 @@
         "POST", endpoint=f"{Endpoints.CALLS_V2}/invite",
         payload={
             "chat_room_id": chat_room_id,
             "room_id": room_id,
             "room_url": room_url
         }
     )
-    self.logger.info("Invitation of chat call sent.")
+    self.logger.info("Invited users to chat call.")
     return response
 
 
 def kick_and_ban_from_call(self, call_id: int, user_id: int):
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.CALLS_V1}/conference_calls/{call_id}/kick",
         payload={"user_id": user_id}
@@ -219,29 +219,29 @@
         "PUT", endpoint=f"{Endpoints.CALLS_V1}/{call_id}",
         payload={
             "joinable_by": joinable_by,
             "game_title": game_title,
             "category_id": category_id,
         }
     )
-    self.logger.info("Call set.")
+    self.logger.info("Started a call")
     return response
 
 
 def set_user_role(
         self,
         call_id: int,
         user_id: int,
         role: str
 ):
     response = self._make_request(
         "PUT", endpoint=f"{Endpoints.CALLS_V1}/{call_id}/users/{user_id}",
         payload={"role": role}
     )
-    self.logger.info("User has been given a role.")
+    self.logger.info(f"User '{user_id}' has been given a role.")
     return response
 
 
 def start_call(
         self,
         conference_id: int,
         call_sid: str
```

### Comparing `yaylib-0.1.2/yaylib/api/cassandra.py` & `yaylib-0.1.3/yaylib/api/cassandra.py`

 * *Files identical despite different names*

### Comparing `yaylib-0.1.2/yaylib/api/chat.py` & `yaylib-0.1.3/yaylib/api/chat.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def accept_chat_request(self, chat_room_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/accept_chat_request",
         payload={"chat_room_ids[]": chat_room_ids}
     )
-    self.logger.info("Chat request accepted.")
+    self.logger.info("Accepted chat requests")
     return response
 
 
 def check_unread_status(self, from_time: int) -> UnreadStatusResponse:
     self._check_authorization()
     return self._make_request(
         "GET", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/unread_status",
@@ -41,15 +41,15 @@
             "name": name,
             "with_user_ids[]": with_user_ids,
             "icon_filename": icon_filename,
             "background_filename": background_filename,
         },
         data_type=CreateChatRoomResponse
     )
-    self.logger.info(f"Group chat '{name}' created.")
+    self.logger.info(f"Group chat '{name}' has been created.")
     return response
 
 
 def create_private_chat(
         self,
         with_user_id: int,
         matching_id: int = None,
@@ -61,33 +61,33 @@
         payload={
             "with_user_id": with_user_id,
             "matching_id": matching_id,
             "hima_chat": hima_chat,
         },
         data_type=CreateChatRoomResponse
     )
-    self.logger.info(f"Private chatroom with '{with_user_id}' created.")
+    self.logger.info(f"Created a private chatroom with '{with_user_id}'.")
     return response
 
 
 def delete_background(self, room_id: int):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{room_id}/background",
     )
-    self.logger.info("Background deleted.")
+    self.logger.info("Background image of the chatroom has been deleted.")
     return response
 
 
 def delete_message(self, room_id: int, message_id: int):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{room_id}/messages/{message_id}/delete",
     )
-    self.logger.info("Message deleted.")
+    self.logger.info("Message has been deleted.")
     return response
 
 
 def edit_chat_room(
         self,
         chat_room_id: int,
         name: str,
@@ -99,15 +99,15 @@
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{chat_room_id}/edit",
         payload={
             "name": name,
             "icon_filename": icon_filename,
             "background_filename": background_filename,
         }
     )
-    self.logger.info("Chatroom updated.")
+    self.logger.info("Chatroom has been updated.")
     return response
 
 
 def get_chatable_users(
         self,
         # @Body @Nullable SearchUsersRequest searchUsersRequest
         from_follow_id: int = None,
@@ -220,25 +220,25 @@
 
 def hide_chat(self, chat_room_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.HIDDEN_V1}/chats",
         payload={"chat_room_id": chat_room_id},
     )
-    self.logger.info("Chatroom hidden.")
+    self.logger.info(f"Chatroom '{chat_room_id}' has been hidden.")
     return response
 
 
 def invite_to_chat(self, chat_room_id: int, user_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{chat_room_id}/invite",
         payload={"with_user_ids[]": user_ids},
     )
-    self.logger.info("Chatroom invitation sent.")
+    self.logger.info("Invited users to the chatroom.")
     return response
 
 
 def kick_users_from_chat(self, chat_room_id: int, user_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{chat_room_id}/kick",
@@ -249,15 +249,15 @@
 
 
 def pin_chat(self, room_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{room_id}/pinned"
     )
-    self.logger.info("Pinned chatroom.")
+    self.logger.info("Pinned the chatroom.")
     return response
 
 
 def read_attachment(
         self,
         room_id: int,
         attachment_msg_ids: List[int]
@@ -266,38 +266,38 @@
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{room_id}/attachments_read",
         payload={
             "attachment_msg_ids[]": attachment_msg_ids
         }
     )
-    self.logger.info("Attachment read.")
+    self.logger.info("Attachment has been read.")
     return response
 
 
 def read_message(self, chat_room_id: int, message_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V2}/{chat_room_id}/messages/{message_id}/read",
     )
-    self.logger.info("Message read.")
+    self.logger.info("Message has been read.")
     return response
 
 
 def read_video_message(
         self,
         room_id: int,
         video_msg_ids: List[int]
 ):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{room_id}/videos_read",
         payload={"video_msg_ids": video_msg_ids},
     )
-    self.logger.info("Video message read.")
+    self.logger.info("Video message has been read.")
     return response
 
 
 def refresh_chat_rooms(self, from_time: int = None) -> ChatRoomsResponse:
     self._check_authorization()
     params = {}
     if from_time:
@@ -310,15 +310,15 @@
 
 def remove_chat_rooms(self, chat_room_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V2}/mass_destroy",
         payload={"chat_room_ids[]": chat_room_ids},
     )
-    self.logger.info("Chat rooms removed.")
+    self.logger.info(f"Chatrooms have been removed.")
     return response
 
 
 def report_chat_room(
         self,
         chat_room_id: int,
         opponent_id: int,
@@ -339,24 +339,24 @@
             "reason": reason,
             "screenshot_filename": screenshot_filename,
             "screenshot_2_filename": screenshot_2_filename,
             "screenshot_3_filename": screenshot_3_filename,
             "screenshot_4_filename": screenshot_4_filename,
         },
     )
-    self.logger.info("Chat room reported.")
+    self.logger.info(f"Chatroom '{chat_room_id}' has been reported.")
     return response
 
 
 def send_media_screenshot_notification(self, room_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{room_id}/screen_captured"
     )
-    self.logger.info("Media screenshot notification sent.")
+    self.logger.info("Media screenshot notification has been sent.")
     return response
 
 
 def send_message(
         self,
         chat_room_id: int,
         message_type: str,
@@ -379,15 +379,15 @@
             "font_size": font_size,
             "gif_image_id": gif_image_id,
             "attachment_file_name": attachment_file_name,
             "sticker_pack_id": sticker_pack_id,
             "video_file_name": video_file_name,
         }, data_type=MessageResponse
     )
-    self.logger.info("Message sent.")
+    self.logger.info("Your message has been sent.")
     return response
 
 
 def set_notification_settings(
         self,
         chat_room_id: int,
         notification_chat: int
@@ -398,18 +398,18 @@
 
 def unhide_chat(self, chat_room_ids: int):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.HIDDEN_V1}/chats",
         params={"chat_room_ids[]": chat_room_ids},
     )
-    self.logger.info("Chatroom unhidden.")
+    self.logger.info("Unhid the chatrooms")
     return response
 
 
 def unpin_chat(self, chat_room_id: int):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.CHAT_ROOMS_V1}/{chat_room_id}/pinned"
     )
-    self.logger.info("Chatroom unpinned.")
+    self.logger.info("Unpinned the chatroom")
     return response
```

### Comparing `yaylib-0.1.2/yaylib/api/group.py` & `yaylib-0.1.3/yaylib/api/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,52 +9,52 @@
 
 
 def accept_moderator_offer(self, group_id: int):
     self._check_authorization()
     response = self._make_request(
         "PUT", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/deputize"
     )
-    self.logger.info("Moderator offer accepted.")
+    self.logger.info("Accepted the group moderator offer.")
     return response
 
 
 def accept_ownership_offer(self, group_id: int):
     self._check_authorization()
     response = self._make_request(
         "PUT", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/transfer"
     )
-    self.logger.info("Ownership offer accepted.")
+    self.logger.info("Accepted the group ownership offer.")
     return response
 
 
 def accept_group_join_request(self, group_id: int, user_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/accept/{user_id}"
     )
-    self.logger.info("Accepted group join request.")
+    self.logger.info("Accepted the group join request.")
     return response
 
 
 def add_related_groups(self, group_id: int, related_group_id: List[int]):
     self._check_authorization()
     response = self._make_request(
         "PUT", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/related",
         params={"related_group_id[]": related_group_id}
     )
-    self.logger.info("Group added to the related groups")
+    self.logger.info("Group has been added to the related groups")
     return response
 
 
 def ban_group_user(self, group_id: int, user_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/ban/{user_id}"
     )
-    self.logger.info("User has been banned from the group.")
+    self.logger.info(f"User '{user_id}' has been banned from the group.")
     return response
 
 
 def check_unread_status(self, from_time: int = None) -> UnreadStatusResponse:
     self._check_authorization()
     params = {}
     if from_time:
@@ -117,61 +117,61 @@
             "sub_category_id": sub_category_id,
             "hide_from_game_eight": hide_from_game_eight,
             "allow_members_to_post_image_and_video": allow_members_to_post_media,
             "allow_members_to_post_url": allow_members_to_post_url,
             "guidelines": guidelines,
         }, data_type=CreateGroupResponse
     )
-    self.logger.info("Group created.")
+    self.logger.info("Group has been created.")
     return response
 
 
 def create_pin_group(self, group_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.PINNED_V1}/groups",
         payload={"id": group_id}
     )
-    self.logger.info("Pinned post in the group.")
+    self.logger.info("Pinned the group.")
     return response
 
 
 def decline_moderator_offer(self, group_id: int):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/deputize"
     )
-    self.logger.info("Declined moderator offer.")
+    self.logger.info("Declined the moderator offer.")
     return response
 
 
 def decline_ownership_offer(self, group_id: int):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/transfer"
     )
-    self.logger.info("Declined ownership offer.")
+    self.logger.info("Declined the ownership offer.")
     return response
 
 
 def decline_group_join_request(self, group_id: int, user_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/decline/{user_id}"
     )
-    self.logger.info("Declined group join request")
+    self.logger.info("Declined the group join request.")
     return response
 
 
 def delete_pin_group(self, group_id: int):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.PINNED_V1}/groups/{group_id}"
     )
-    self.logger.info("Unpinned group post.")
+    self.logger.info("Unpinned the group.")
     return response
 
 
 def get_banned_group_members(self, group_id: int, page: int = None) -> UsersResponse:
     self._check_authorization()
     params = {}
     if page:
@@ -348,24 +348,24 @@
 
 def invite_users_to_group(self, group_id: int, user_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/invite",
         payload={"user_ids[]": user_ids}
     )
-    self.logger.info("Group invitation sent.")
+    self.logger.info("Invited users to the group.")
     return response
 
 
 def join_group(self, group_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/join",
     )
-    self.logger.info("Joined the group.")
+    self.logger.info("You are now one of the members of the group.")
     return response
 
 
 def leave_group(self, group_id: int):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/leave",
@@ -376,43 +376,43 @@
 
 def post_gruop_social_shared(self, group_id: int, sns_name: str):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V2}/{group_id}/social_shared",
         params={"sns_name": sns_name}
     )
-    self.logger.info("Group social shared posted.")
+    self.logger.info("Group social shared has been posted.")
     return response
 
 
 def remove_group_cover(self, group_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/remove_cover",
     )
-    self.logger.info("Group cover removed.")
+    self.logger.info("Group cover image has been removed.")
     return response
 
 
 def remove_moderator(self, group_id: int, user_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/fire/{user_id}",
     )
-    self.logger.info("Group moderator removed.")
+    self.logger.info(f"Group moderator '{user_id}' has been removed.")
     return response
 
 
 def remove_related_groups(self, group_id: int, related_group_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/related",
         params={"related_group_id[]": related_group_ids}
     )
-    self.logger.info("Related groups removed.")
+    self.logger.info("Related groups have been removed.")
     return response
 
 
 def report_group(
         self,
         group_id: int,
         category_id: int,
@@ -423,21 +423,24 @@
         screenshot_3_filename: str = None,
         screenshot_4_filename: str = None,
 ):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V3}/{group_id}/report",
         payload={
-            "category_id": category_id, "reason": reason,
-            "opponent_id": opponent_id, "screenshot_filename": screenshot_filename, "screenshot_2_filename": screenshot_2_filename,
+            "category_id": category_id,
+            "reason": reason,
+            "opponent_id": opponent_id,
+            "screenshot_filename": screenshot_filename,
+            "screenshot_2_filename": screenshot_2_filename,
             "screenshot_3_filename": screenshot_3_filename,
             "screenshot_4_filename": screenshot_4_filename
         }
     )
-    self.logger.info("Group reported.")
+    self.logger.info("Group has been reported.")
     return response
 
 
 def send_moderator_offers(self, group_id: int, user_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V3}/{group_id}/deputize/mass",
@@ -446,15 +449,15 @@
             "api_key": self.api_key, "timestamp": int(datetime.now().timestamp()),
             "signed_info": signed_info_calculating(
                 self.api_key, self.device_uuid,
                 int(datetime.now().timestamp())
             ),
         }
     )
-    self.logger.info("Group moderator offer sent.")
+    self.logger.info("Offered users to become a group moderator.")
     return response
 
 
 def send_ownership_offer(self, group_id: int, user_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V3}/{group_id}/transfer",
@@ -463,15 +466,15 @@
             "api_key": self.api_key, "timestamp": int(datetime.now().timestamp()),
             "signed_info": signed_info_calculating(
                 self.api_key, self.device_uuid,
                 int(datetime.now().timestamp())
             ),
         }
     )
-    self.logger.info("Group ownership offer sent.")
+    self.logger.info("Offered user to become a group owner.")
     return response
 
 
 def set_group_notification_settings(
         self,
         group_id: int,
         notification_group_post: int = None,
@@ -484,15 +487,15 @@
 
 def set_group_title(self, group_id: int, title: str):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/set_title",
         payload={"title": title}
     )
-    self.logger.info("Group title set.")
+    self.logger.info("Group tittle has been set.")
     return response
 
 
 def take_over_group_ownership(self, group_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/take_over",
@@ -502,15 +505,15 @@
 
 
 def unban_group_member(self, group_id: int, user_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/unban/{user_id}",
     )
-    self.logger.info("Group user has been unbanned.")
+    self.logger.info("User has been banned from the group.")
     return response
 
 
 def update_group(
         self,
         group_id: int,
         topic: str,
@@ -563,36 +566,36 @@
             ),
             "hide_from_game_eight": hide_from_game_eight,
             "allow_members_to_post_image_and_video": allow_members_to_post_media,
             "allow_members_to_post_url": allow_members_to_post_url,
             "guidelines": guidelines,
         }, data_type=GroupResponse
     )
-    self.logger.info("Group has been updated.")
+    self.logger.info("Group details have been updated.")
     return response
 
 
 def visit_group(self, group_id: int):
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/visit",
     )
-    self.logger.info("Group visited.")
+    self.logger.info("Visited the group.")
     return response
 
 
 def withdraw_moderator_offer(self, group_id: int, user_id: int):
     self._check_authorization()
     response = self._make_request(
         "PUT", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/deputize/{user_id}/withdraw",
     )
-    self.logger.info("Group moderator offer withdrawn")
+    self.logger.info("Group moderator offer has been withdrawn")
     return response
 
 
 def withdraw_ownership_offer(self, group_id: int, user_id: int):
     self._check_authorization()
     response = self._make_request(
         "PUT", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/transfer/withdraw",
         payload={"user_id": user_id}
     )
-    self.logger.info("Group ownershipt offer withdrawn")
+    self.logger.info("Group ownership offer has been withdrawn")
     return response
```

### Comparing `yaylib-0.1.2/yaylib/api/login.py` & `yaylib-0.1.3/yaylib/api/login.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         payload={
             "api_key": self.api_key,
             "email": email,
             "password": password,
             "email_grant_token": email_grant_token
         }, data_type=LoginUpdateResponse
     )
-    self.logger.info("Email has been changed.")
+    self.logger.info(self, fname="Your email has been changed.")
     return response
 
 
 def change_password(
         self,
         current_password: str,
         new_password: str
@@ -36,15 +36,15 @@
         "PUT", endpoint=f"{Endpoints.USERS_V1}/change_email",
         payload={
             "api_key": self.api_key,
             "current_password": current_password,
             "password": new_password
         }, data_type=LoginUpdateResponse
     )
-    self.logger.info("Password has been changed.")
+    self.logger.info(self, fname="Your password has been changed..")
     return response
 
 
 def connect_account_with_sns(self):
     pass
 
 
@@ -85,36 +85,36 @@
         raise ForbiddenError(message)
 
     self.login_data = response
     self.session.headers.setdefault(
         "Authorization", f"Bearer {self.login_data.access_token}"
     )
 
-    self.logger.info(f'Successfully logged in as [{self.login_data.user_id}]')
+    self.logger.info(f"Successfully logged in as '{self.login_data.user_id}'")
     return response
 
 
 def login_with_sns(self):
     pass
 
 
 def logout(self):
     try:
         self._check_authorization()
         response = self._make_request(
             "POST", endpoint=f"{Endpoints.USERS_V1}/logout",
             payload={"uuid": self.uuid}
         )
-        self.session.headers.pop('Authorization', None)
+        self.session.headers.pop("Authorization", None)
         self.login_data = None
-        self.logger.info('User has Logged out.')
+        self.logger.info("User has logged out.")
         return response
 
     except:
-        self.logger.error(f'User is not logged in.')
+        self.logger.error("User is not logged in.")
         return None
 
 
 def migrate_token(self):
     pass
 
 
@@ -138,23 +138,23 @@
             "uuid": self.uuid,
             "timestamp": timestamp,
             "signed_info": signed_info_calculating(
                 self.device_uuid, timestamp
             ),
         }
     )
-    self.logger.info("User restored.")
+    self.logger.info("User has been restored.")
     return response
 
 
 def revoke_tokens(self):
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.USERS_V1}/device_tokens"
     )
-    self.logger.info("Token revoked.")
+    self.logger.info("Token has been revoked.")
     return response
 
 
 def save_account_with_email(
         self,
         email: str,
         password: str = None,
```

### Comparing `yaylib-0.1.2/yaylib/api/misc.py` & `yaylib-0.1.3/yaylib/api/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,22 @@
         "GET", endpoint=f"{Endpoints.SNS_THUMBNAIL_V1}/generate",
         params=params
     )
     self.logger.info("SNS thumbnail generated.")
     return response
 
 
+def get_email_grant_token(self, code: int, email: str) -> EmailGrantTokenResponse:
+    return self._make_request(
+        "POST", endpoint=f"{Endpoints.GET_EMAIL_GRANT_TOKEN}",
+        payload={"code": code, "email": email},
+        data_type=EmailGrantTokenResponse
+    ).email_grant_token
+
+
 def get_email_verification_presigned_url(self, email: str, locale: str, intent: str = None) -> str:
     return self._make_request(
         "POST", endpoint=f"{Endpoints.EMAIL_VERIFICATION_URL_V1}",
         payload={
             "device_uuid": self.device_uuid,
             "email": email,
             "locale": locale,
@@ -132,25 +140,23 @@
         payload={
             "app_version": app_version,
             "device_uuid": device_uuid,
             "platform": platform,
             "verification_string": verification_string,
         }, data_type=VerifyDeviceResponse
     )
-    self.logger.info("Device verified.")
+    self.logger.info("Device has been verified.")
     return response
 
 
 def upload_image(self, image_type: str, image_path: str) -> str:
     """
 
     画像をアップロードしてattachment_filenameを返します。
 
-    ※ 対応形式: jpeg, png, gif
-
     Parameteres
     -----------
         - image_type: str - (required): "post", "user_avatar" のどちらか
         - image_path: str - (required): "画像のパス
 
     """
     valid_types = ["post", "user_avatar"]
```

### Comparing `yaylib-0.1.2/yaylib/api/post.py` & `yaylib-0.1.3/yaylib/api/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 
 def add_bookmark(self, user_id: int, post_id: int) -> BookmarkPostResponse:
     self._check_authorization()
     response = self._make_request(
         "PUT", endpoint=f"{Endpoints.USERS_V1}/{user_id}/bookmarks/{post_id}",
         data_type=BookmarkPostResponse
     )
-    self.logger.info("Added to bookmarks.")
+    self.logger.info("Post has been added to the bookmarks.")
     return response
 
 
 def add_group_highlight_post(self, group_id: int, post_id: int):
     self._check_authorization()
     response = self._make_request(
         "PUT", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/highlights/{post_id}",
     )
-    self.logger.info("Added to group highlight.")
+    self.logger.info("Post has been added to the group highlight.")
     return response
 
 
 def create_call_post(
         self,
         text: str = None,
         font_size: int = None,
@@ -82,35 +82,35 @@
             "attachment_5_filename": attachment_5_filename,
             "attachment_6_filename": attachment_6_filename,
             "attachment_7_filename": attachment_7_filename,
             "attachment_8_filename": attachment_8_filename,
             "attachment_9_filename": attachment_9_filename,
         }, data_type=CreatePostResponse
     ).conference_call
-    self.logger.info("Call post created.")
+    self.logger.info("Call post has been created.")
     return response
 
 
 def create_group_pin_post(self, post_id: int, group_id: int):
     self._check_authorization()
     response = self._make_request(
         "PUT", endpoint=f"{Endpoints.POSTS_V2}/group_pinned_post",
         payload={"post_id": post_id, "group_id": group_id}
     )
-    self.logger.info("Pinned post in a group.")
+    self.logger.info("Pinned the post in the group.")
     return response
 
 
 def create_pin_post(self, post_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.PINNED_V1}/posts",
         payload={"id": post_id}
     )
-    self.logger.info("Pinned post")
+    self.logger.info("Pinned post.")
     return response
 
 
 def mention(self, user_id: int) -> str:
     if not (isinstance(user_id, int) or str(user_id).isdigit()):
         raise ValueError(
             "The value of 'user_id' must be an integer or a string containing only digits.")
@@ -222,27 +222,26 @@
             "attachment_6_filename": attachment_6_filename,
             "attachment_7_filename": attachment_7_filename,
             "attachment_8_filename": attachment_8_filename,
             "attachment_9_filename": attachment_9_filename,
             "video_file_name": video_file_name,
         }, data_type=Post, headers=headers
     )
-    self.logger.info("Post created.")
+    self.logger.info("Post has been created.")
     return response
 
 
 def create_repost(
         self,
         post_id: int,
         text: str = None,
         font_size: int = None,
         color: int = None,
         in_reply_to: int = None,
         group_id: int = None,
-        post_type: str = None,
         mention_ids: List[int] = None,
         choices: List[str] = None,
         shared_url: Dict[str, Union[str, int]] = None,
         message_tags: str = "[]",
         attachment_filename: str = None,
         attachment_2_filename: str = None,
         attachment_3_filename: str = None,
@@ -293,15 +292,15 @@
             "attachment_6_filename": attachment_6_filename,
             "attachment_7_filename": attachment_7_filename,
             "attachment_8_filename": attachment_8_filename,
             "attachment_9_filename": attachment_9_filename,
             "video_file_name": video_file_name,
         }, data_type=CreatePostResponse, headers=headers
     ).post
-    self.logger.info("Repost created.")
+    self.logger.info("Repost has been created.")
     return response
 
 
 def create_share_post(
         self,
         shareable_type: str,
         shareable_id: int,
@@ -325,27 +324,26 @@
             "api_key": self.api_key,
             "timestamp": timestamp,
             "signed_info": signed_info_calculating(
                 self.device_uuid, timestamp
             ),
         }, data_type=Post
     )
-    self.logger.info("Share post created.")
+    self.logger.info("Share post has been created.")
     return response
 
 
 def create_thread_post(
         self,
         post_id: int,
         text: str = None,
         font_size: int = None,
         color: int = None,
         in_reply_to: int = None,
         group_id: int = None,
-        post_type: str = None,
         mention_ids: List[int] = None,
         choices: List[str] = None,
         shared_url: Dict[str, Union[str, int]] = None,
         message_tags: str = "[]",
         attachment_filename: str = None,
         attachment_2_filename: str = None,
         attachment_3_filename: str = None,
@@ -396,37 +394,37 @@
             "attachment_6_filename": attachment_6_filename,
             "attachment_7_filename": attachment_7_filename,
             "attachment_8_filename": attachment_8_filename,
             "attachment_9_filename": attachment_9_filename,
             "video_file_name": video_file_name,
         }, data_type=Post, headers=headers
     )
-    self.logger.info("Thread post created.")
+    self.logger.info("Thread post has been created.")
     return response
 
 
 def delete_all_post(self):
     self._check_authorization()
     try:
         response = self._make_request(
             "POST", endpoint=f"{Endpoints.POSTS_V1}/delete_all_post",
         )
-        self.logger.info("Post deletion requested.")
+        self.logger.info("Post deletion request has been sent.")
         return response
     except NotFoundError:
-        self.logger.info("Post not found.")
+        self.logger.info("Post not found. Skipping...")
 
 
 def delete_group_pin_post(self, group_id: int):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.POSTS_V2}/group_pinned_post",
         payload={"group_id": group_id}
     )
-    self.logger.info("Unpinned post in a group.")
+    self.logger.info("Unpinned post in the group.")
     return response
 
 
 def delete_pin_post(self, post_id: int):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.PINNED_V1}/posts/{post_id}"
@@ -780,26 +778,26 @@
     )
 
 
 def like_posts(self, post_ids: List[int]) -> LikePostsResponse:
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.POSTS_V2}/like",
-        payload={"post_ids[]": post_ids}, data_type=LikePostsResponse
+        payload={"post_ids": post_ids}, data_type=LikePostsResponse
     )
-    self.logger.info("Posts liked.")
+    self.logger.info("Posts have been liked.")
     return response
 
 
 def remove_bookmark(self, user_id: int, post_id: int):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.USERS_V1}/{user_id}/bookmarks/{post_id}",
     )
-    self.logger.info("Bookmark removed.")
+    self.logger.info("Bookmark has been removed.")
     return response
 
 
 def remove_group_highlight_post(self, group_id: int, post_id: int):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.GROUPS_V1}/{group_id}/highlights/{post_id}",
@@ -810,15 +808,15 @@
 
 def remove_posts(self, post_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.POSTS_V2}/mass_destroy",
         payload={"posts_ids": post_ids}
     )
-    self.logger.info("Posts removed.")
+    self.logger.info("Posts have been removed.")
     return response
 
 
 def report_post(
         self,
         post_id: int,
         opponent_id: int,
@@ -838,24 +836,24 @@
             "reason": reason,
             "screenshot_filename": screenshot_filename,
             "screenshot_2_filename": screenshot_2_filename,
             "screenshot_3_filename": screenshot_3_filename,
             "screenshot_4_filename": screenshot_4_filename,
         }
     )
-    self.logger.info("Post reported.")
+    self.logger.info("Post has been reported.")
     return response
 
 
 def unlike_post(self, post_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.POSTS_V1}/{post_id}/unlike",
     )
-    self.logger.info("Post unliked.")
+    self.logger.info("Post has been unliked.")
     return response
 
 
 def update_post(
         self,
         post_id: int,
         text: str = None,
@@ -880,15 +878,15 @@
             "api_key": self.api_key,
             "timestamp": timestamp,
             "signed_info": signed_info_calculating(
                 self.device_uuid, timestamp
             ),
         }
     )
-    self.logger.info("Post updated.")
+    self.logger.info("Post has been updated.")
     return response
 
 
 def update_recommendation_feedback(
         self, post_id: int, feedback_result: str, *,
         experiment_num: int, variant_num: int,
 ):
@@ -897,39 +895,39 @@
         "POST", endpoint=f"{Endpoints.POSTS_V2}/{post_id}/recommendation_feedback",
         payload={
             "feedback_result": feedback_result,
             "experiment_num": experiment_num,
             "variant_num": variant_num
         }
     )
-    self.logger.info("Recommendation feedback updated.")
+    self.logger.info("Recommendation feedback has been updated.")
     return response
 
 
 def validate_post(self, text: str, *, group_id: int = None, thread_id: int = None) -> ValidationPostResponse:
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.POSTS_V1}/validate",
         payload={
             "text": text, "group_id": group_id, "thread_id": thread_id
         }, data_type=ValidationPostResponse
     )
-    self.logger.info("Post validated.")
+    self.logger.info("Post has been validated.")
     return response
 
 
 def view_video(self, video_id: int):
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.POSTS_V1}/videos/{video_id}/view"
     )
-    self.logger.info("Viewed a video")
+    self.logger.info("Viewed the video.")
     return response
 
 
 def vote_survey(self, survey_id: int, choice_id: int) -> Survey:
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.SURVEYS_V2}/{survey_id}/vote",
         payload={"choice_id": choice_id}, data_type=ValidationPostResponse
     ).survey
-    self.logger.info("Survey voted.")
+    self.logger.info("Voted.")
     return response
```

### Comparing `yaylib-0.1.2/yaylib/api/review.py` & `yaylib-0.1.3/yaylib/api/review.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,30 +4,41 @@
 from ..config import *
 from ..errors import *
 from ..models import *
 from ..responses import *
 from ..utils import *
 
 
+# def create_review(self, user_id: int, comment: str):
+#     # TODO: check the update of v3.18
+#     self._check_authorization()
+#     timestamp = int(datetime.now().timestamp())
+#     response = self._make_request(
+#         "POST", endpoint=f"{Endpoints.USERS_V2}/reviews/{user_id}",
+#         payload={
+#             "comment": comment,
+#             "uuid": self.uuid,
+#             "api_key": self.api_key,
+#             "timestamp": timestamp,
+#             "signed_info": signed_info_calculating(
+#                 self.uuid, timestamp, shared_key=True
+#             ),
+#         },
+#     )
+#     self.logger.info("Review has been sent to {user_id}.")
+#     return response
+
+
 def create_review(self, user_id: int, comment: str):
     self._check_authorization()
-    timestamp = int(datetime.now().timestamp())
     response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V2}/reviews/{user_id}",
-        payload={
-            "comment": comment,
-            "uuid": self.uuid,
-            "api_key": self.api_key,
-            "timestamp": timestamp,
-            "signed_info": signed_info_calculating(
-                self.uuid, timestamp, shared_key=True
-            ),
-        },
+        "POST", endpoint=f"{Endpoints.USERS_V1}/reviews/{user_id}",
+        payload={"comment": comment}
     )
-    self.logger.info("Review created.")
+    self.logger.info(f"Review has been sent to {user_id}.")
     return response
 
 
 def create_reviews(self, user_ids: List[int], comment: str):
     self._check_authorization()
     timestamp = int(datetime.now().timestamp())
     response = self._make_request(
@@ -39,25 +50,25 @@
             "api_key": self.api_key,
             "timestamp": timestamp,
             "signed_info": signed_info_calculating(
                 self.uuid, timestamp, shared_key=True
             ),
         },
     )
-    self.logger.info("Reviews created.")
+    self.logger.info("Reviews have been sent to multiple users.")
     return response
 
 
 def delete_reviews(self, review_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.USERS_V1}/reviews",
         params={"review_ids[]": review_ids}
     )
-    self.logger.info("Reviews deleted.")
+    self.logger.info("Reviews have been deleted.")
     return response
 
 
 def get_my_reviews(self, **params) -> ReviewsResponse:
     """
 
     Parameters
@@ -102,9 +113,9 @@
 
 
 def unpin_review(self, review_id: int):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.PINNED_V1}/reviews{review_id}"
     )
-    self.logger.info("Review unpinned.")
+    self.logger.info("Unpinned the review.")
     return response
```

### Comparing `yaylib-0.1.2/yaylib/api/thread.py` & `yaylib-0.1.3/yaylib/api/thread.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def add_post_to_thread(self, post_id: int, thread_id: int) -> ThreadInfo:
     self._check_authorization()
     response = self._make_request(
         "PUT", endpoint=f"{Endpoints.POSTS_V3}/{post_id}/move_to_thread/{thread_id}",
         data_type=ThreadInfo
     )
-    self.logger.info("Post added to the thread.")
+    self.logger.info(f"Post '{post_id}' added to the thread '{thread_id}'.")
     return response
 
 
 def convert_post_to_thread(
         self,
         post_id: int,
         title: str = None,
@@ -28,15 +28,15 @@
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.POSTS_V3}/{post_id}/move_to_thread",
         payload={
             "title": title,
             "thread_icon_filename": thread_icon_filename
         }, data_type=ThreadInfo
     )
-    self.logger.info("Post converted to a thread.")
+    self.logger.info("Post has been converted to a thread.")
     return response
 
 
 def create_thread(
         self,
         group_id: int,
         title: str,
@@ -47,15 +47,15 @@
         "POST", endpoint=f"{Endpoints.THREADS_V1}",
         payload={
             "group_id": group_id,
             "title": title,
             "thread_icon_filename": thread_icon_filename,
         }, data_type=ThreadInfo
     )
-    self.logger.info("Thread created.")
+    self.logger.info("A new thread has been created.")
     return response
 
 
 def get_group_thread_list(self, group_id: int, from_str: str = None, **params) -> GroupThreadListResponse:
     """
 
     Parameters:
@@ -103,15 +103,15 @@
 
 
 def join_thread(self, thread_id: int, user_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.THREADS_V1}/{thread_id}/members/{user_id}",
     )
-    self.logger.info("Joined the thread.")
+    self.logger.info(f"Joined the thread '{thread_id}'.")
     return response
 
 
 def leave_thread(self, thread_id: int, user_id: int):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.THREADS_V1}/{thread_id}/members/{user_id}",
@@ -121,24 +121,24 @@
 
 
 def remove_thread(self, thread_id: int):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.THREADS_V1}/{thread_id}",
     )
-    self.logger.info("Thread removed.")
+    self.logger.info(f"Thread '{thread_id}' has been removed.")
     return response
 
 
 def update_thread(
         self,
         thread_id: int,
         title: str,
         thread_icon_filename: str
 ):
     self._check_authorization()
     response = self._make_request(
         "PUT", endpoint=f"{Endpoints.THREADS_V1}/{thread_id}",
         payload={"title": title, "thread_icon_filename": thread_icon_filename}
     )
-    self.logger.info("Thread updated.")
+    self.logger.info(f"Thread '{thread_id}' has been updated.")
     return response
```

### Comparing `yaylib-0.1.2/yaylib/api/user.py` & `yaylib-0.1.3/yaylib/api/user.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,77 +4,29 @@
 from ..config import *
 from ..errors import *
 from ..models import *
 from ..responses import *
 from ..utils import *
 
 
-def create_user(
-        self,
-        nickname: str,
-        birth_date: str,
-        gender: int = -1,
-        country_code: str = "JP",
-        biography: str = None,
-        prefecture: str = None,
-        profile_icon_filename: str = None,
-        cover_image_filename: str = None,
-        # @Nullable @Part("sns_info") SignUpSnsInfoRequest signUpSnsInfoRequest,
-        email: str = None,
-        password: str = None,
-        email_grant_token: str = None,
-        en: int = None,
-        vn: int = None
-) -> CreateUserResponse:
-    timestamp = int(datetime.now().timestamp())
-    response = self._make_request(
-        "POST", endpoint=f"{Endpoints.USERS_V3}/edit",
-        payload={
-            "app_version": self.api_version,
-            "timestamp": timestamp,
-            "api_key": self.api_key,
-            "signed_version": signed_version_calculating(),
-            "signed_info": signed_info_calculating(
-                self.device_uuid, timestamp
-            ),
-            "uuid": self.uuid,
-            "nickname": nickname,
-            "birth_date": birth_date,
-            "gender": gender,
-            "country_code": country_code,
-            "biography": biography,
-            "prefecture": prefecture,
-            "profile_icon_filename": profile_icon_filename,
-            "cover_image_filename": cover_image_filename,
-            "email": email,
-            "password": password,
-            "email_grant_token": email_grant_token,
-            "en": en,
-            "vn": vn,
-        }
-    )
-    self.logger.info("Account created.")
-    return response
-
-
 def delete_contact_friends(self):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.USERS_V1}/contact_friends"
     )
-    self.logger.info("Contact friends deleted.")
+    self.logger.info("Contact friends have been deleted.")
     return response
 
 
 def delete_footprint(self, user_id: int, footprint_id: int):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.USERS_V2}/{user_id}/footprints/{footprint_id}"
     )
-    self.logger.info("Footprint deleted.")
+    self.logger.info("Footprint has been deleted.")
     return response
 
 
 def destroy_user(self):
     self._check_authorization()
     answer = input("Are you sure you want to delete your account? Y/N")
     if answer.lower() != "y":
@@ -96,25 +48,25 @@
 
 
 def follow_user(self, user_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/{user_id}/follow"
     )
-    self.logger.info(f"User '{user_id}' followed.")
+    self.logger.info("Followed the user '{user_id}'.")
     return response
 
 
 def follow_users(self, user_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/follow",
         params={"user_ids[]": user_ids}
     )
-    self.logger.info("Users followed.")
+    self.logger.info("Followed multiple users.")
     return response
 
 
 def get_active_followings(self, **params) -> ActiveFollowingsResponse:
     """
 
     Parameters:
@@ -416,15 +368,15 @@
 
 
 def post_social_shared(self, sns_name: str):
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/social_shared",
         params={"sns_name": sns_name}
     )
-    self.logger.info("Social shared posted.")
+    self.logger.info("Posted social shared post.")
     return response
 
 
 def record_app_review_status(self):
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V1}/{self.url_uuid}/app_review_status",
         params={"uuid": self.uuid}
@@ -444,40 +396,40 @@
             "timestamp": timestamp,
             "signed_info": signed_info_calculating(
                 self.device_uuid, timestamp
             ),
             "signed_version": signed_version_calculating()
         }, data_type=CreatePostResponse
     )
-    self.logger.info("Penalty reduced.")
+    self.logger.info("Penalty has been reduced.")
     return response
 
 
 def refresh_counter(self, counter: str):
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V1}/reset_counters",
         payload={"counter": counter}
     )
-    self.logger.info("Counter refreshed.")
+    self.logger.info("Requested counter refresh.")
     return response
 
 
 def remove_user_avatar(self):
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/remove_profile_photo"
     )
-    self.logger.info("User avatar removed.")
+    self.logger.info("Profile image has been removed.")
     return response
 
 
 def remove_user_cover(self):
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/remove_cover_image"
     )
-    self.logger.info("User cover removed.")
+    self.logger.info("Profile cover image has been removed.")
     return response
 
 
 def report_user(
         self,
         user_id: int,
         category_id: int,
@@ -495,28 +447,28 @@
             "reason": reason,
             "screenshot_filename": screenshot_filename,
             "screenshot_2_filename": screenshot_2_filename,
             "screenshot_3_filename": screenshot_3_filename,
             "screenshot_4_filename": screenshot_4_filename,
         }
     )
-    self.logger.info("User reported.")
+    self.logger.info(f"Reported the user '{user_id}'")
     return response
 
 
 def reset_password(self, email: str, email_grant_token: str, password: str):
     response = self._make_request(
         "PUT", endpoint=f"{Endpoints.USERS_V1}/reset_password",
         payload={
             "email": email,
             "email_grant_token": email_grant_token,
             "password": password,
         }
     )
-    self.logger.info("Password has been reset.")
+    self.logger.info("Reset the password.")
     return response
 
 
 def search_lobi_users(self, **params) -> UsersResponse:
     """
 
     Parameters:
@@ -558,15 +510,15 @@
 
 
 def set_additional_setting_enabled(self, mode: str, on: int = None):
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V1}/additonal_notification_setting",
         payload={"mode": mode, "on": on}
     )
-    self.logger.info("Additional setting enabled.")
+    self.logger.info("Additional settings have been enabled.")
     return response
 
 
 def set_follow_permission_enabled(self, nickname: str, is_private: bool = None):
     timestamp = int(datetime.now().timestamp())
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/edit",
@@ -578,25 +530,25 @@
             "timestamp": timestamp,
             "signed_info": signed_info_calculating(
                 self.device_uuid, timestamp
             ),
             "signed_version": signed_version_calculating()
         }
     )
-    self.logger.info("Follow permission enabled.")
+    self.logger.info("Follow permission has been enabled.")
     return response
 
 
 def set_setting_follow_recommendation_enabled(self, on: bool):
     response = self._make_request(
         "POST",
         endpoint=f"{Endpoints.USERS_V1}/visible_on_sns_friend_recommendation_setting",
         params={"on": on}
     )
-    self.logger.info("Follow recommendation enabled.")
+    self.logger.info("Follow recommendation has been enabled.")
     return response
 
 
 def take_action_follow_request(self, target_id: int, action: str):
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/{target_id}/follow_request",
         payload={"action": action}
@@ -606,24 +558,24 @@
 
 
 def turn_on_hima(self):
     self._check_authorization()
     response = self._make_request(
         "GET", endpoint=f"{Endpoints.USERS_V1}/hima",
     )
-    self.logger.info("Turned on hima now.")
+    self.logger.info("Turned on 'hima now'.")
     return response
 
 
 def unfollow_user(self, user_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/{user_id}/unfollow",
     )
-    self.logger.info("User unfollowed.")
+    self.logger.info(f"Unfollowed the user '{user_id}'")
     return response
 
 
 def update_invite_contact_status(self, mobile_number: str):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V1}/invite_contact",
@@ -642,15 +594,15 @@
             "api_key": self.api_key,
             "timestamp": timestamp,
             "signed_info": signed_info_calculating(
                 self.device_uuid, timestamp),
             "language": language,
         }
     )
-    self.logger.info("Language updated.")
+    self.logger.info("Language has been updated.")
     return response
 
 
 def update_user(
         self,
         nickname: str,
         biography: str = None,
@@ -678,15 +630,15 @@
             "api_key": self.api_key,
             "timestamp": timestamp,
             "signed_info": signed_info_calculating(
                 self.device_uuid, timestamp
             ),
         }
     )
-    self.logger.info("User profile updated.")
+    self.logger.info("User profile has been updated.")
     return response
 
 
 def update_user_interests(
         self,
         # @Body @NotNull CommonIdsRequest commonIdsRequest,
         # @NotNull Continuation<? super Unit> continuation
@@ -703,27 +655,27 @@
 
 def upload_twitter_friend_ids(self, twitter_friend_ids: List[str]):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V1}/twitter_friends",
         payload={"twitter_friend_ids[]": twitter_friend_ids}
     )
-    self.logger.info("Twitter friend ids updated.")
+    self.logger.info("Uploaded Twitter friend ids.")
     return response
 
 
 # BlockApi
 
 
 def block_user(self, user_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V1}/{user_id}/block",
     )
-    self.logger.info("User blocked.")
+    self.logger.info(f"Blocked the user '{user_id}'")
     return response
 
 
 def get_blocked_user_ids(self) -> BlockedUserIdsResponse:
     self._check_authorization()
     return self._make_request(
         "GET", endpoint=f"{Endpoints.USERS_V1}/block_ids",
@@ -744,15 +696,15 @@
 
 
 def unblock_user(self, user_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.USERS_V2}/{user_id}/unblock"
     )
-    self.logger.info("User unblocked.")
+    self.logger.info(f"Unblocked the user '{user_id}'")
     return response
 
 
 # HiddenApi
 
 
 def get_hidden_users_list(self, **params: Union[str, int]) -> HiddenResponse:
@@ -774,19 +726,19 @@
 
 def hide_user(self, user_id: int):
     self._check_authorization()
     response = self._make_request(
         "POST", endpoint=f"{Endpoints.HIDDEN_V1}/users",
         payload={"user_id": user_id}
     )
-    self.logger.info("user hidden.")
+    self.logger.info(f"User '{user_id}' is hidden")
     return response
 
 
 def unhide_users(self, user_ids: List[int]):
     self._check_authorization()
     response = self._make_request(
         "DELETE", endpoint=f"{Endpoints.HIDDEN_V1}/users",
         params={"user_ids[]": user_ids}
     )
-    self.logger.info("User unhidden.")
+    self.logger.info("Unhid users")
     return response
```

### Comparing `yaylib-0.1.2/yaylib/client.py` & `yaylib-0.1.3/yaylib/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,24 +38,27 @@
         >>> timeline = api.get_timeline(number=30)
 
     #### Parameters
 
         - access_token: str - (optional)
         - refresh_token: str - (optional)
         - proxy: str - (optional)
+        - max_retries: int - (optional)
+        - backoff_factor: float - (optional)
         - timeout: int - (optional)
+        - lang: str - (optional)
         - base_path: str - (optional)
         - loglevel_stream: int - (optional)
         - host: str - (optional)
 
     <https://github.com/qvco/yaylib>
 
     ---
 
-    ### Yay! API v3 Client
+    ### Yay! (nanameue, Inc.) API Client
 
     Copyright (c) 2023 Qvco, Konn
 
     """
 
     # -CALL
 
@@ -141,17 +144,19 @@
             - group_category_id: int - (optional)
             - from_timestamp: int - (optional)
             - scope: str - (optional)
 
         """
         return get_group_calls(self, **params)
 
-    def invite_to_call_bulk(self, call_id: int, group_id: int = None) -> dict:
+    def invite_online_followings_to_call(self, call_id: int, group_id: int = None) -> dict:
         """
 
+        オンラインの友達をまとめて通話に招待します
+
         Parameters
         ----------
             - call_id: int - (required)
             - group_id: int - (optional)
 
         """
         return invite_to_call_bulk(self, call_id, group_id)
@@ -356,15 +361,14 @@
         グループチャットを作成します
 
         Parameters
         ----------
 
             - name: str - (required)
             - with_user_ids: List[int] - (required)
-            - chat_room_ids: List[int] - (required)
             - icon_filename: str - (optional)
             - background_filename: str - (optional)
 
         """
         return create_group_chat(
             self,
             name,
@@ -382,15 +386,15 @@
         """
 
         個人チャットを作成します
 
         Parameters
         ----------
 
-            - with_user_ids: List[int] - (required)
+            - with_user_id: int - (required)
             - matching_id: str - (optional)
             - hima_chat: bool - (optional)
 
         """
         return create_private_chat(
             self,
             with_user_id,
@@ -564,46 +568,46 @@
         """
 
         チャットルームをピン止めします
 
         """
         return pin_chat(self, room_id)
 
-    def read_attachment(
-            self,
-            room_id: int,
-            attachment_msg_ids: List[int]
-    ) -> dict:
-        """
-
-        アタッチメントを既読にします
-
-        """
-        # TODO: check if this works
-        return read_attachment(self, room_id, attachment_msg_ids)
+    # def read_attachment(
+    #         self,
+    #         room_id: int,
+    #         attachment_msg_ids: List[int]
+    # ) -> dict:
+    #     """
+
+    #     アタッチメントを既読にします
+
+    #     """
+    #     # TODO: check if this works
+    #     return read_attachment(self, room_id, attachment_msg_ids)
 
     def read_message(self, chat_room_id: int, message_id: int) -> dict:
         """
 
         メッセージを既読にします
 
         """
         return read_message(self, chat_room_id, message_id)
 
-    def read_video_message(
-            self,
-            room_id: int,
-            video_msg_ids: List[int]
-    ) -> dict:
-        """
+    # def read_video_message(
+    #         self,
+    #         room_id: int,
+    #         video_msg_ids: List[int]
+    # ) -> dict:
+    #     """
 
-        動画のメッセージを既読にします
+    #     動画のメッセージを既読にします
 
-        """
-        return read_video_message(self, room_id, video_msg_ids)
+    #     """
+    #     return read_video_message(self, room_id, video_msg_ids)
 
     def refresh_chat_rooms(self, from_time: int = None) -> ChatRoomsResponse:
         """
 
         チャットルームを更新します
 
         """
@@ -707,55 +711,55 @@
         return unpin_chat(self, chat_room_id)
 
     # -GROUP
 
     def accept_moderator_offer(self, group_id: int) -> dict:
         """
 
-        グループ副管理人の権限オファーを引き受けます
+        サークル副管理人の権限オファーを引き受けます
 
         """
         return accept_moderator_offer(self, group_id)
 
     def accept_ownership_offer(self, group_id: int) -> dict:
         """
 
-        グループ管理人の権限オファーを引き受けます
+        サークル管理人の権限オファーを引き受けます
 
         """
         return accept_ownership_offer(self, group_id)
 
     def accept_group_join_request(self, group_id: int, user_id: int) -> dict:
         """
 
-        グループ参加リクエストを承認します
+        サークル参加リクエストを承認します
 
         """
         return accept_group_join_request(self, group_id, user_id)
 
     def add_related_groups(self, group_id: int, related_group_id: List[int]) -> dict:
         """
 
-        関連グループを追加します
+        関連サークルを追加します
 
         """
         return add_related_groups(self, group_id, related_group_id)
 
     def ban_group_user(self, group_id: int, user_id: int) -> dict:
         """
 
-        グループからユーザーを追放します
+        サークルからユーザーを追放します
 
         """
         return ban_group_user(self, group_id, user_id)
 
     def check_unread_status(self, from_time: int = None) -> UnreadStatusResponse:
         """
 
-        グループの未読ステータスを取得します
+        サークルの未読ステータスを取得します
 
         """
         return check_unread_status(self, from_time)
 
     def create_group(
             self,
             topic: str,
@@ -777,15 +781,15 @@
             hide_from_game_eight: bool = None,
             allow_members_to_post_media: bool = None,
             allow_members_to_post_url: bool = None,
             guidelines: str = None,
     ) -> CreateGroupResponse:
         """
 
-        グループを作成します
+        サークルを作成します
 
         """
         return create_group(
             self,
             topic,
             description,
             secret,
@@ -806,96 +810,96 @@
             allow_members_to_post_url,
             guidelines
         )
 
     def create_pin_group(self, group_id: int) -> dict:
         """
 
-        グループの投稿をピンします
+        サークルの投稿をピンします
 
         """
         return create_pin_group(self, group_id)
 
     def decline_moderator_offer(self, group_id: int) -> dict:
         """
 
-        グループ副管理人の権限オファーを断ります
+        サークル副管理人の権限オファーを断ります
 
         """
         return decline_moderator_offer(self, group_id)
 
     def decline_ownership_offer(self, group_id: int) -> dict:
         """
 
-        グループ管理人の権限オファーを断ります
+        サークル管理人の権限オファーを断ります
 
         """
         return decline_ownership_offer(self, group_id)
 
     def decline_group_join_request(self, group_id: int, user_id: int) -> dict:
         """
 
-        グループ参加リクエストを断ります
+        サークル参加リクエストを断ります
 
         """
         return decline_ownership_offer(self, group_id, user_id)
 
     def delete_pin_group(self, group_id: int) -> dict:
         """
 
-        グループのピン投稿を解除します
+        サークルのピン投稿を解除します
 
         """
         return delete_pin_group(self, group_id)
 
     def get_banned_group_members(self, group_id: int, page: int = None) -> UsersResponse:
         """
 
-        追放されたグループメンバーを取得します
+        追放されたサークルメンバーを取得します
 
         """
         return get_banned_group_members(self, group_id, page)
 
     def get_group_categories(self, **params) -> GroupCategoriesResponse:
         """
 
-        グループのカテゴリーを取得します
+        サークルのカテゴリーを取得します
 
         Parameters
         ----------
 
             - page: int - (optional)
             - number: int - (optional)
 
         """
         return get_group_categories(self, **params)
 
     def get_create_group_quota(self) -> CreateGroupQuota:
         """
 
-        グループ作成可能な割当量を取得します
+        サークル作成可能な割当量を取得します
 
         """
         return get_create_group_quota(self)
 
     def get_group(self, group_id: int) -> GroupResponse:
         """
 
-        グループの詳細を取得します
+        サークルの詳細を取得します
 
         """
         return get_group(self, group_id)
 
     # def get_group_notification_settings(self, group_id: int) -> GroupNotificationSettingsResponse:
     #     return get_group_notification_settings(self, group_id)
 
     def get_groups(self, **params) -> GroupsResponse:
         """
 
-        複数のグループの詳細を取得します
+        複数のサークルの詳細を取得します
 
         Parameters
         ----------
 
             - group_category_id: int = None
             - keyword: str = None
             - from_timestamp: int = None
@@ -903,15 +907,15 @@
 
         """
         return get_groups(self, **params)
 
     def get_invitable_users(self, group_id: int, **params) -> UsersByTimestampResponse:
         """
 
-        グループに招待可能なユーザーを取得します
+        サークルに招待可能なユーザーを取得します
 
         Parameters
         ----------
 
             - from_timestamp: int - (optional)
             - user[nickname]: str - (optional)
 
@@ -920,23 +924,23 @@
 
     def get_joined_statuses(self, ids: List[int]) -> dict:
         return get_joined_statuses(self, ids)
 
     def get_group_member(self, group_id: int, user_id: int) -> GroupUserResponse:
         """
 
-        特定のグループメンバーの情報を取得します
+        特定のサークルメンバーの情報を取得します
 
         """
         return get_group_member(self, group_id, user_id)
 
     def get_group_members(self, group_id: int, **params) -> GroupUsersResponse:
         """
 
-        グループメンバーを取得します
+        サークルメンバーを取得します
 
         Parameters
         ----------
 
             - id: int - (required)
             - mode: str - (optional)
             - keyword: str - (optional)
@@ -947,110 +951,115 @@
 
         """
         return get_group_members(self, group_id, **params)
 
     def get_my_groups(self, from_timestamp: None) -> GroupsResponse:
         """
 
-        自分のグループを取得します
+        自分のサークルを取得します
 
         """
         return get_my_groups(self, from_timestamp)
 
     def get_relatable_groups(self, group_id: int, **params) -> GroupsRelatedResponse:
         """
 
-        関連がある可能性があるグループを取得します
+        関連がある可能性があるサークルを取得します
 
         Parameters
         ----------
 
             - group_id: int - (required)
             - keyword: str - (optional)
             - from: str - (optional)
 
         """
         return get_relatable_groups(self, group_id, **params)
 
     def get_related_groups(self, group_id: int, **params) -> GroupsRelatedResponse:
         """
 
-        関連があるグループを取得します
+        関連があるサークルを取得します
 
         Parameters
         ----------
 
             - group_id: int - (required)
             - keyword: str - (optional)
             - from: str - (optional)
 
         """
         return get_related_groups(self, group_id, **params)
 
     def get_user_groups(self, **params) -> GroupsResponse:
         """
 
-        特定のユーザーが参加しているグループを取得します
+        特定のユーザーが参加しているサークルを取得します
 
         Parameters
         ----------
 
             - user_id: int - (required)
             - page: int - (optional)
 
         """
         return get_user_groups(self, **params)
 
     def invite_users_to_group(self, group_id: int, user_ids: List[int]) -> dict:
         """
 
-        グループにユーザーを招待します
+        サークルにユーザーを招待します
 
         """
         return invite_users_to_group(self, group_id, user_ids)
 
     def join_group(self, group_id: int) -> dict:
         """
 
-        グループに参加します
+        サークルに参加します
 
         """
         return join_group(self, group_id)
 
     def leave_group(self, group_id: int) -> dict:
         """
 
-        グループから脱退します
+        サークルから脱退します
 
         """
         return leave_group(self, group_id)
 
     def post_gruop_social_shared(self, group_id: int, sns_name: str) -> dict:
+        """
+
+        サークルのソーシャルシェアを投稿します
+
+        """
         return post_gruop_social_shared(self, group_id, sns_name)
 
     def remove_group_cover(self, group_id: int) -> dict:
         """
 
-        グループのカバー画像を削除します
+        サークルのカバー画像を削除します
 
         """
         return remove_group_cover(self, group_id)
 
     def remove_moderator(self, group_id: int, user_id: int) -> dict:
         """
 
-        グループの副管理人を削除します
+        サークルの副管理人を削除します
 
         """
         return remove_moderator(self, group_id, user_id)
 
     def remove_related_groups(self, group_id: int, related_group_ids: List[int]) -> dict:
         """
 
-        関連のあるグループを削除します
+        関連のあるサークルを削除します
 
         """
         return remove_related_groups(self, group_id, related_group_ids)
 
     def report_group(
             self,
             group_id: int,
@@ -1060,15 +1069,15 @@
             screenshot_filename: str = None,
             screenshot_2_filename: str = None,
             screenshot_3_filename: str = None,
             screenshot_4_filename: str = None,
     ) -> dict:
         """
 
-        グループを通報します
+        サークルを通報します
 
         """
         return report_group(
             self,
             group_id,
             category_id,
             reason,
@@ -1078,23 +1087,23 @@
             screenshot_3_filename,
             screenshot_4_filename
         )
 
     def send_moderator_offers(self, group_id: int, user_ids: List[int]) -> dict:
         """
 
-        複数人に副管理人のオファーを送信します
+        複数人にサークル副管理人のオファーを送信します
 
         """
         return send_moderator_offers(self, group_id, user_ids)
 
     def send_ownership_offer(self, group_id: int, user_id: int) -> dict:
         """
 
-        グループ管理人権限のオファーを送信します
+        サークル管理人権限のオファーを送信します
 
         """
         return send_ownership_offer(self, group_id, user_id)
 
     # def set_group_notification_settings(
     #         self,
     #         group_id: int,
@@ -1104,31 +1113,31 @@
     #         notification_group_message_tag_all: int = None,
     # ) -> AdditionalSettingsResponse:
     #     return set_group_notification_settings(self)
 
     def set_group_title(self, group_id: int, title: str) -> dict:
         """
 
-        グループのタイトルを設定します
+        サークルのタイトルを設定します
 
         """
         return set_group_title(self, group_id, title)
 
     def take_over_group_ownership(self, group_id: int) -> dict:
         """
 
-        グループ管理人の権限を引き継ぎます
+        サークル管理人の権限を引き継ぎます
 
         """
         return take_over_group_ownership(self, group_id)
 
     def unban_group_member(self, group_id: int, user_id: int) -> dict:
         """
 
-        特定のグループメンバーの追放を解除します
+        特定のサークルメンバーの追放を解除します
 
         """
         return unban_group_member(self, group_id, user_id)
 
     def update_group(
             self,
             group_id: int,
@@ -1151,15 +1160,15 @@
             hide_from_game_eight: bool = None,
             allow_members_to_post_media: bool = None,
             allow_members_to_post_url: bool = None,
             guidelines: str = None,
     ) -> GroupResponse:
         """
 
-        グループを編集します
+        サークルを編集します
 
         """
         return update_group(
             group_id,
             topic,
             description,
             secret,
@@ -1181,31 +1190,31 @@
             allow_members_to_post_url,
             guidelines,
         )
 
     def visit_group(self, group_id: int) -> dict:
         """
 
-        グループを訪問します
+        サークルを訪問します
 
         """
         return visit_group(self, group_id)
 
     def withdraw_moderator_offer(self, group_id: int, user_id: int) -> dict:
         """
 
-        グループ副管理人のオファーを取り消します
+        サークル副管理人のオファーを取り消します
 
         """
         return withdraw_moderator_offer(self, group_id, user_id)
 
     def withdraw_ownership_offer(self, group_id: int, user_id: int) -> dict:
         """
 
-        グループ管理人のオファーを取り消します
+        サークル管理人のオファーを取り消します
 
         """
         return withdraw_ownership_offer(self, group_id, user_id)
 
     # -LOGIN
 
     def change_email(
@@ -1244,15 +1253,15 @@
             grant_type: str,
             refresh_token: str = None,
             email: str = None,
             password: str = None
     ) -> TokenResponse:
         """
 
-        トークンを再取得します
+        アクセストークンを再発行します
 
         """
         return get_token(
             self,
             grant_type,
             refresh_token,
             email,
@@ -1281,17 +1290,27 @@
     # def migrate_token(self) -> dict:
     #     return migrate_token(self)
 
     # def register_device_token(self) -> dict:
     #     return register_device_token(self)
 
     def resend_confirm_email(self) -> dict:
+        """
+
+        確認メールを再送信します
+
+        """
         return resend_confirm_email(self)
 
     def restore_user(self, user_id: int) -> LoginUserResponse:
+        """
+
+        ユーザーを復元します
+
+        """
         return restore_user(self, user_id)
 
     def revoke_tokens(self) -> dict:
         """
 
         トークンを無効化します
 
@@ -1316,28 +1335,36 @@
             password,
             current_password,
             email_grant_token,
         )
 
     # -MISC
 
-    def accept_policy_agreement(self, type: str) -> dict:
-        return accept_policy_agreement(self, type)
+    # def accept_policy_agreement(self, type: str) -> dict:
+    #     return accept_policy_agreement(self, type)
 
-    def generate_sns_thumbnail(self, **params) -> dict:
-        """
+    # def generate_sns_thumbnail(self, **params) -> dict:
+    #     """
 
-        Parameters
-        ----------
+    #     Parameters
+    #     ----------
+
+    #         - resource_type: str - (Required)
+    #         - resource_id: int - (Required)
+
+    #     """
+    #     return generate_sns_thumbnail(self, **params)
 
-            - resource_type: str - (Required)
-            - resource_id: int - (Required)
+    def get_email_grant_token(self, code: int, email: str) -> str:
+        """
+
+        email_grant_token を取得します
 
         """
-        return generate_sns_thumbnail(self, **params)
+        return get_email_grant_token(self, code, email)
 
     def get_email_verification_presigned_url(self, email: str, locale: str, intent: str = None) -> str:
         """
 
         メールアドレス確認用の署名付きURLを取得します
 
         """
@@ -1358,75 +1385,73 @@
     #         **params
     # ) -> str:
     #     return get_id_checker_presigned_url(self, model, action, **params)
 
     def get_old_file_upload_presigned_url(self, video_file_name: str) -> str:
         """
 
-        ファイルアップロード用の署名付きURLを取得します
+        動画ファイルアップロード用の署名付きURLを取得します
 
         """
         return get_old_file_upload_presigned_url(self, video_file_name)
 
     def get_policy_agreements(self) -> PolicyAgreementsResponse:
         return get_policy_agreements(self)
 
-    def get_promotions(self, **params) -> List[Promotion]:
-        """
+    # def get_promotions(self, **params) -> List[Promotion]:
+    #     """
 
-        プロモーションを取得します
+    #     プロモーションを取得します
 
-        Parameters
-        ----------
+    #     Parameters
+    #     ----------
 
-            - page: int - (Optional)
-            - number: int - (Optional)
+    #         - page: int - (Optional)
+    #         - number: int - (Optional)
 
-        """
-        return get_promotions(self, **params)
+    #     """
+    #     return get_promotions(self, **params)
 
-    def get_vip_game_reward_url(self, device_type: str) -> str:
-        return get_vip_game_reward_url(self, device_type)
+    # def get_vip_game_reward_url(self, device_type: str) -> str:
+    #     return get_vip_game_reward_url(self, device_type)
 
     def get_web_socket_token(self) -> str:
         """
 
         Web Socket Token を取得します
 
         """
         return get_web_socket_token(self)
 
-    def verify_device(
-            self,
-            app_version: str,
-            device_uuid: str,
-            platform: str,
-            verification_string: str
-    ) -> VerifyDeviceResponse:
-        """
-
-        デバイスを検証します
-
-        """
-        # TODO: check platform, verification_string
-        return verify_device(
-            self,
-            app_version,
-            device_uuid,
-            platform,
-            verification_string
-        )
+    # def verify_device(
+    #         self,
+    #         app_version: str,
+    #         device_uuid: str,
+    #         platform: str,
+    #         verification_string: str
+    # ) -> VerifyDeviceResponse:
+    #     """
+
+    #     デバイスを検証します
+
+    #     """
+    #     # TODO: check platform, verification_string
+    #     return verify_device(
+    #         self,
+    #         app_version,
+    #         device_uuid,
+    #         platform,
+    #         verification_string
+    #     )
 
     def upload_image(self, image_type: str, image_path: str) -> str:
         """
 
         画像をアップロードしてattachment_filenameを返します。
 
-        ※ 対応形式: jpeg, png, gif
-
         Parameteres
         -----------
             - image_type: str - (required): "post", "user_avatar" のどちらか
             - image_path: str - (required): "画像のパス
 
         """
         return upload_image(self, image_type, image_path)
@@ -1438,14 +1463,19 @@
 
         ブックマークに追加します
 
         """
         return add_bookmark(self, user_id, post_id)
 
     def add_group_highlight_post(self, group_id: int, post_id: int) -> dict:
+        """
+
+        投稿をグループハイライトに追加します
+
+        """
         return add_group_highlight_post(self, group_id, post_id)
 
     def create_call_post(
             self,
             text: str = None,
             font_size: int = None,
             color: int = None,
@@ -1488,23 +1518,23 @@
             attachment_5_filename,
             attachment_6_filename,
             attachment_7_filename,
             attachment_8_filename,
             attachment_9_filename
         )
 
-    def create_group_pin_post(self, post_id: int, group_id: int) -> dict:
+    def pin_group_post(self, post_id: int, group_id: int) -> dict:
         """
 
         グループの投稿をピンします
 
         """
         return create_group_pin_post(self, post_id, group_id)
 
-    def create_pin_post(self, post_id: int) -> dict:
+    def pin_post(self, post_id: int) -> dict:
         """
 
         投稿をピンします
 
         """
         return create_pin_post(self, post_id)
 
@@ -1521,15 +1551,15 @@
             text: str = None,
             font_size: int = 0,
             color: int = 0,
             in_reply_to: int = None,
             group_id: int = None,
             mention_ids: List[int] = None,
             choices: List[str] = None,
-            shared_url: Dict[str, str | int] = None,
+            shared_url: str = None,
             message_tags: str = "[]",
             attachment_filename: str = None,
             attachment_2_filename: str = None,
             attachment_3_filename: str = None,
             attachment_4_filename: str = None,
             attachment_5_filename: str = None,
             attachment_6_filename: str = None,
@@ -1570,15 +1600,14 @@
             self,
             post_id: int,
             text: str = None,
             font_size: int = None,
             color: int = None,
             in_reply_to: int = None,
             group_id: int = None,
-            post_type: str = None,
             mention_ids: List[int] = None,
             choices: List[str] = None,
             shared_url: Dict[str, Union[str, int]] = None,
             message_tags: str = "[]",
             attachment_filename: str = None,
             attachment_2_filename: str = None,
             attachment_3_filename: str = None,
@@ -1599,15 +1628,14 @@
             self,
             post_id,
             text,
             font_size,
             color,
             in_reply_to,
             group_id,
-            post_type,
             mention_ids,
             choices,
             shared_url,
             message_tags,
             attachment_filename,
             attachment_2_filename,
             attachment_3_filename,
@@ -1625,14 +1653,19 @@
             shareable_type: str,
             shareable_id: int,
             text: str = None,
             font_size: int = None,
             color: int = None,
             group_id: int = None,
     ) -> Post:
+        """
+
+        シェア投稿を作成します
+
+        """
         return create_share_post(
             self,
             shareable_type,
             shareable_id,
             text,
             font_size,
             color,
@@ -1643,15 +1676,14 @@
             self,
             post_id: int,
             text: str = None,
             font_size: int = None,
             color: int = None,
             in_reply_to: int = None,
             group_id: int = None,
-            post_type: str = None,
             mention_ids: List[int] = None,
             choices: List[str] = None,
             shared_url: Dict[str, Union[str, int]] = None,
             message_tags: str = "[]",
             attachment_filename: str = None,
             attachment_2_filename: str = None,
             attachment_3_filename: str = None,
@@ -1672,15 +1704,14 @@
             self,
             post_id,
             text,
             font_size,
             color,
             in_reply_to,
             group_id,
-            post_type,
             mention_ids,
             choices,
             shared_url,
             message_tags,
             attachment_filename,
             attachment_2_filename,
             attachment_3_filename,
@@ -1697,23 +1728,23 @@
         """
 
         すべての投稿を削除します
 
         """
         return delete_all_post(self)
 
-    def delete_group_pin_post(self, group_id: int) -> dict:
+    def unpin_group_post(self, group_id: int) -> dict:
         """
 
-        グループのピン投稿を削除します
+        グループのピン投稿を解除します
 
         """
         return delete_group_pin_post(self, group_id)
 
-    def delete_pin_post(self, post_id: int) -> dict:
+    def unpin_post(self, post_id: int) -> dict:
         """
 
         ピン投稿を削除します
 
         """
         return delete_pin_post(self, post_id)
 
@@ -1808,14 +1839,16 @@
 
         """
         return get_following_timeline(self, **params)
 
     def get_group_highlight_posts(self, group_id: int, **params) -> PostsResponse:
         """
 
+        グループのハイライト投稿を取得します
+
         Parameters
         ----------
 
             - group_id: int
             - from_post: int = None
             - number: int = None
 
@@ -1905,15 +1938,15 @@
 
             - from_id: int - (optional)
             - number: int - (optional)
 
         """
         return get_post_likers(self, post_id, **params)
 
-    def get_post_reposts(self, post_id: int, **params: int) -> PostsResponse:
+    def get_reposts(self, post_id: int, **params: int) -> PostsResponse:
         """
 
         投稿の(´∀｀∩)↑age↑を取得します
 
         Parameters
         ----------
 
@@ -1931,14 +1964,19 @@
 
         """
         return get_posts(self, post_ids)
 
     def get_recommended_post_tags(
         self, tag: str = None, save_recent_search: bool = False
     ) -> PostTagsResponse:
+        """
+
+        おすすめのタグ候補を取得します
+
+        """
         return get_recommended_post_tags(self, tag, save_recent_search)
 
     def get_recommended_posts(self, **params) -> PostsResponse:
         """
 
         おすすめの投稿を取得します
 
@@ -1963,15 +2001,15 @@
             - keyword: str
             - from_post_id: int
             - number: int
 
         """
         return get_timeline_by_keyword(self, keyword, **params)
 
-    def get_timeline(self, **params: int | str | bool) -> PostsResponse:
+    def get_timeline(self, **params) -> PostsResponse:
         # - from: str - (optional)
         """
 
         タイムラインを取得します
 
         Parameters
         ----------
@@ -1988,14 +2026,19 @@
             - reduce_selfie: bool - (optional)
             - custom_generation_range: bool - (optional)
 
         """
         return get_timeline(self, **params)
 
     def get_url_metadata(self, url: str) -> SharedUrl:
+        """
+
+        URLのメタデータを取得します
+
+        """
         return get_url_metadata(self, url)
 
     def get_user_timeline(self, user_id: int, **params) -> PostsResponse:
         """
 
         ユーザーのタイムラインを取得します
 
@@ -2022,14 +2065,19 @@
 
         ブックマークを削除します
 
         """
         return remove_bookmark(self, user_id, post_id)
 
     def remove_group_highlight_post(self, group_id: int, post_id: int) -> dict:
+        """
+
+        サークルのハイライト投稿を解除します
+
+        """
         return remove_group_highlight_post(self, group_id, post_id)
 
     def remove_posts(self, post_ids: List[int]) -> dict:
         """
 
         複数の投稿を削除します
 
@@ -2085,23 +2133,33 @@
         投稿を編集します
 
         """
         return update_post(
             self, post_id, text, font_size, color, message_tags
         )
 
-    def update_recommendation_feedback(
-        self, post_id: int, feedback_result: str, *,
-        experiment_num: int, variant_num: int,
-    ) -> dict:
-        return update_recommendation_feedback(
-            self, post_id, feedback_result, experiment_num, variant_num
-        )
+    # def update_recommendation_feedback(
+    #     self, post_id: int, feedback_result: str,
+    #     experiment_num: int, variant_num: int,
+    # ) -> dict:
+    #     """
+
+    #     おすすめのフィードバックを更新します
+
+    #     """
+    #     return update_recommendation_feedback(
+    #         self, post_id, feedback_result, experiment_num, variant_num
+    #     )
 
     def validate_post(self, text: str, *, group_id: int = None, thread_id: int = None) -> ValidationPostResponse:
+        """
+
+        与えられたテキストが有効な投稿であるかどうかを検証します
+
+        """
         return validate_post(self, text, group_id, thread_id)
 
     def view_video(self, video_id: int) -> dict:
         """
 
         動画を視聴します
 
@@ -2311,61 +2369,21 @@
             thread_id,
             title,
             thread_icon_filename
         )
 
     # -USER
 
-    def create_user(
-            self,
-            nickname: str,
-            birth_date: str,
-            gender: int = -1,
-            country_code: str = "JP",
-            biography: str = None,
-            prefecture: str = None,
-            profile_icon_filename: str = None,
-            cover_image_filename: str = None,
-            # @Nullable @Part("sns_info") SignUpSnsInfoRequest signUpSnsInfoRequest,
-            email: str = None,
-            password: str = None,
-            email_grant_token: str = None,
-            en: int = None,
-            vn: int = None
-    ) -> CreateUserResponse:
-        """
+    # def delete_contact_friends(self) -> dict:
+    #     """
 
-        アカウントを作成します
+    #     連絡先の友人を削除します
 
-        birth_date: 2000-01-01の形式
-        """
-        return create_user(
-            self,
-            nickname,
-            birth_date,
-            gender,
-            country_code,
-            biography,
-            prefecture,
-            profile_icon_filename,
-            cover_image_filename,
-            email,
-            password,
-            email_grant_token,
-            en,
-            vn
-        )
-
-    def delete_contact_friends(self) -> dict:
-        """
-
-        連絡先の友人を削除します
-
-        """
-        return delete_contact_friends(self)
+    #     """
+    #     return delete_contact_friends(self)
 
     def delete_footprint(self, user_id: int, footprint_id: int) -> dict:
         """
 
         足跡を削除します
 
         """
@@ -2394,31 +2412,33 @@
 
         """
         return follow_users(self, user_ids)
 
     def get_active_followings(self, **params) -> ActiveFollowingsResponse:
         """
 
+        アクティブなフォロー中のユーザーを取得します
+
         Parameters
         ----------
 
             - only_online: bool
             - from_loggedin_at: int = None
 
         """
         return get_active_followings(self, **params)
 
     # def get_additional_settings(self) -> Settings:
     #     return get_additional_settings(self)
 
-    def get_app_review_status(self) -> AppReviewStatusResponse:
-        return get_app_review_status(self)
+    # def get_app_review_status(self) -> AppReviewStatusResponse:
+    #     return get_app_review_status(self)
 
-    def get_contact_status(self, mobile_numbers: List[str]) -> ContactStatusResponse:
-        return get_contact_status(self, mobile_numbers)
+    # def get_contact_status(self, mobile_numbers: List[str]) -> ContactStatusResponse:
+    #     return get_contact_status(self, mobile_numbers)
 
     # def get_default_settings(self) -> TimelineSettings:
     #     return get_default_settings(self)
 
     def get_follow_recommendations(self, **params) -> FollowRecommendationsResponse:
         """
 
@@ -2447,14 +2467,19 @@
 
         フォローリクエストの数を取得します
 
         """
         return get_follow_request_count(self)
 
     def get_following_users_born(self, birthdate: int = None) -> UsersResponse:
+        """
+
+        フォロー中のユーザーの誕生日を取得します
+
+        """
         return get_following_users_born(self, birthdate)
 
     def get_footprints(self, **params) -> List[Footprint]:
         """
 
         足跡を取得します
 
@@ -2481,35 +2506,40 @@
 
             - from_hima_id: int = None
             - number: int = None
 
         """
         return get_hima_users(self, **params)
 
-    def get_initial_recommended_users_to_follow(self, **params) -> UsersResponse:
-        return get_initial_recommended_users_to_follow(self, **params)
+    # def get_initial_recommended_users_to_follow(self, **params) -> UsersResponse:
+    #     return get_initial_recommended_users_to_follow(self, **params)
 
-    def get_recommended_users_to_follow_for_profile(
-            self, user_id: int, **params
-    ) -> UsersResponse:
-        """
+    # def get_recommended_users_to_follow_for_profile(
+    #         self, user_id: int, **params
+    # ) -> UsersResponse:
+    #     """
+
+    #     Parameters
+    #     ----------
+
+    #         - user_id: int - (Required)
+    #         - number: int - (Optional)
+    #         - page: int - (Optional)
+
+    #     """
+    #     return get_recommended_users_to_follow_for_profile(
+    #         self, user_id, **params
+    #     )
 
-        Parameters
-        ----------
+    def get_refresh_counter_requests(self) -> RefreshCounterRequestsResponse:
+        """
 
-            - user_id: int - (Required)
-            - number: int - (Optional)
-            - page: int - (Optional)
+        カウンター更新のリクエストを取得します
 
         """
-        return get_recommended_users_to_follow_for_profile(
-            self, user_id, **params
-        )
-
-    def get_refresh_counter_requests(self) -> RefreshCounterRequestsResponse:
         return get_refresh_counter_requests(self)
 
     def get_social_shared_users(self, **params) -> SocialShareUsersResponse:
         """
 
         Parameters
         ----------
@@ -2533,16 +2563,16 @@
         """
 
         ユーザーの情報を取得します
 
         """
         return get_user(self, user_id)
 
-    def get_user_custom_definitions(self) -> UserCustomDefinitionsResponse:
-        return get_user_custom_definitions(self)
+    # def get_user_custom_definitions(self) -> UserCustomDefinitionsResponse:
+    #     return get_user_custom_definitions(self)
 
     def get_user_email(self, user_id: int) -> str:
         """
 
         ユーザーのメールアドレスを取得します
 
         """
@@ -2600,37 +2630,42 @@
         """
 
         複数のユーザーの情報を取得します
 
         """
         return get_users(self, user_ids)
 
-    def get_users_from_uuid(self, uuid: str) -> UsersResponse:
-        """
+    # def get_users_from_uuid(self, uuid: str) -> UsersResponse:
+    #     """
 
-        UUIDからユーザーを取得します
+    #     UUIDからユーザーを取得します
 
-        """
-        return get_users_from_uuid(self, uuid)
+    #     """
+    #     return get_users_from_uuid(self, uuid)
 
     def post_social_shared(self, sns_name: str) -> dict:
         return post_social_shared(self, sns_name)
 
-    def record_app_review_status(self) -> dict:
-        return record_app_review_status(self)
+    # def record_app_review_status(self) -> dict:
+    #     return record_app_review_status(self)
 
     def reduce_kenta_penalty(self, user_id: int) -> dict:
         """
 
         ペナルティーを緩和します
 
         """
         return reduce_kenta_penalty(self, user_id)
 
     def refresh_counter(self, counter: str) -> dict:
+        """
+
+        カウンターを更新します
+
+        """
         return refresh_counter(self, counter)
 
     def remove_user_avatar(self) -> dict:
         """
 
         ユーザーのアイコンを削除します
 
@@ -2712,24 +2747,24 @@
             - recently_created: bool = None
             - same_prefecture: bool = None
             - save_recent_search: bool = None
 
         """
         return search_users(self, **params)
 
-    def set_additional_setting_enabled(self, mode: str, on: int = None) -> dict:
-        return set_additional_setting_enabled(self, mode, on)
+    # def set_additional_setting_enabled(self, mode: str, on: int = None) -> dict:
+    #     return set_additional_setting_enabled(self, mode, on)
 
     def set_follow_permission_enabled(
             self, nickname: str, is_private: bool = None
     ) -> dict:
         return set_follow_permission_enabled(self, nickname, is_private)
 
-    def set_setting_follow_recommendation_enabled(self, on: bool) -> dict:
-        return set_setting_follow_recommendation_enabled(self, on)
+    # def set_setting_follow_recommendation_enabled(self, on: bool) -> dict:
+    #     return set_setting_follow_recommendation_enabled(self, on)
 
     def take_action_follow_request(self, target_id: int, action: str) -> dict:
         return take_action_follow_request(self, target_id, action)
 
     def turn_on_hima(self) -> dict:
         """
 
@@ -2742,16 +2777,16 @@
         """
 
         ユーザーをアンフォローします
 
         """
         return unfollow_user(self, user_id)
 
-    def update_invite_contact_status(self, mobile_number: str) -> dict:
-        return update_invite_contact_status(self, mobile_number)
+    # def update_invite_contact_status(self, mobile_number: str) -> dict:
+    #     return update_invite_contact_status(self, mobile_number)
 
     def update_language(self, language: str) -> dict:
         """
 
         言語を更新します
 
         """
@@ -2780,16 +2815,21 @@
 
     # def update_user_interests(self) -> dict:
     #     return update_user_interests(self)
 
     # def upload_contacts_friends(self) -> dict:
     #     return upload_contacts_friends(self)
 
-    def upload_twitter_friend_ids(self, twitter_friend_ids: List[str]) -> dict:
-        return upload_twitter_friend_ids(self, twitter_friend_ids)
+    # def upload_twitter_friend_ids(self, twitter_friend_ids: List[str]) -> dict:
+    #     """
+
+    #     TwitterのフレンドのIDをアップロードします
+
+    #     """
+    #     return upload_twitter_friend_ids(self, twitter_friend_ids)
 
     def block_user(self, user_id: int) -> dict:
         """
 
         ユーザーをブロックします
 
         """
```

### Comparing `yaylib-0.1.2/yaylib/models.py` & `yaylib-0.1.3/yaylib/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from .utils import parse_datetime
 
 
 class Activity:
 
     __slots__ = (
         "data", "id", "created_at", "created_at_parsed", "type", "user", "from_post",
-        "to_post", "group", "followers", "from_post_ids", "vip_reward", "metadata",
+        "to_post", "group", "followers", "from_post_ids", "vip_reward",
+        "is_bulk_invitation",
     )
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.created_at = data.get("created_at")
         self.created_at_parsed = parse_datetime(data.get("created_at"))
@@ -34,20 +35,16 @@
         self.followers = data.get("followers")
         if self.followers is not None:
             self.followers = [
                 User(follower) for follower in self.followers
             ]
 
         self.from_post_ids = data.get("from_post_ids")
-
         self.vip_reward = data.get("vip_reward")
-
-        self.metadata = data.get("metadata")
-        # if self.metadata is not None:
-        #     self.metadata = Metadata(self.metadata)
+        self.is_bulk_invitation = data.get("is_bulk_invitation")
 
     def __repr__(self):
         return f"Activity(data={self.data})"
 
 
 class BanWord:
 
@@ -184,19 +181,19 @@
 
     def __repr__(self):
         return f"CoinAmount(data={self.data})"
 
 
 class CoinExpiration:
 
-    __slots__ = ("data", "expired_at_seconds", "amount")
+    __slots__ = ("data", "expired_at", "amount")
 
     def __init__(self, data):
         self.data = data
-        self.expired_at_seconds = data.get("expired_at_seconds")
+        self.expired_at = data.get("expired_at")
         self.amount = data.get("amount")
 
     def __repr__(self):
         return f"CoinExpiration(data={self.data})"
 
 
 class CoinProduct:
```

### Comparing `yaylib-0.1.2/yaylib/responses.py` & `yaylib-0.1.3/yaylib/responses.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,14 +290,26 @@
         self.refresh_token = data.get("refresh_token")
         self.expires_in = data.get("expires_in")
 
     def __repr__(self):
         return f"CreateUserResponse(data={self.data})"
 
 
+class EmailGrantTokenResponse:
+
+    __slots__ = ("data", "email_grant_token")
+
+    def __init__(self, data):
+        self.data = data
+        self.email_grant_token = data.get("email_grant_token")
+
+    def __repr__(self):
+        return f"EmailGrantTokenResponse(data={self.data})"
+
+
 class EmailVerificationPresignedUrlResponse:
 
     __slots__ = ("data", "url")
 
     def __init__(self, data):
         self.data = data
         self.url = data.get("url")
```

### Comparing `yaylib-0.1.2/yaylib/utils.py` & `yaylib-0.1.3/yaylib/utils.py`

 * *Files identical despite different names*

### Comparing `yaylib-0.1.2/yaylib.egg-info/SOURCES.txt` & `yaylib-0.1.3/yaylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

