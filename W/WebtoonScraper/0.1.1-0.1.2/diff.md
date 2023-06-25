# Comparing `tmp/WebtoonScraper-0.1.1.tar.gz` & `tmp/WebtoonScraper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebtoonScraper-0.1.1.tar", last modified: Wed Jun 21 12:03:58 2023, max compression
+gzip compressed data, was "WebtoonScraper-0.1.2.tar", last modified: Sun Jun 25 12:35:24 2023, max compression
```

## Comparing `WebtoonScraper-0.1.1.tar` & `WebtoonScraper-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 12:03:58.127315 WebtoonScraper-0.1.1/
--rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      140 2023-06-06 01:23:54.000000 WebtoonScraper-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0    10314 2023-06-21 12:03:58.126316 WebtoonScraper-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     9226 2023-06-21 11:54:52.000000 WebtoonScraper-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 12:03:58.108159 WebtoonScraper-0.1.1/WebtoonScraper/
--rw-rw-rw-   0        0        0      516 2023-06-06 00:42:00.000000 WebtoonScraper-0.1.1/WebtoonScraper/BestChallengeScraper.py
--rw-rw-rw-   0        0        0     6198 2023-06-21 11:41:23.000000 WebtoonScraper-0.1.1/WebtoonScraper/BufftoonScraper.py
--rw-rw-rw-   0        0        0     7405 2023-06-21 11:54:44.000000 WebtoonScraper-0.1.1/WebtoonScraper/NaverPostScraper.py
--rw-rw-rw-   0        0        0     3332 2023-06-07 11:43:11.000000 WebtoonScraper-0.1.1/WebtoonScraper/NaverWebtoonScraper.py
--rw-rw-rw-   0        0        0    16642 2023-06-21 08:37:42.000000 WebtoonScraper-0.1.1/WebtoonScraper/Scraper.py
--rw-rw-rw-   0        0        0     4665 2023-06-17 13:02:43.000000 WebtoonScraper-0.1.1/WebtoonScraper/TelescopeScraper.py
--rw-rw-rw-   0        0        0     4284 2023-06-21 12:03:29.000000 WebtoonScraper-0.1.1/WebtoonScraper/Webtoon.py
--rw-rw-rw-   0        0        0      501 2023-06-06 00:44:55.000000 WebtoonScraper-0.1.1/WebtoonScraper/WebtoonCanvasScraper.py
--rw-rw-rw-   0        0        0     4250 2023-06-17 07:29:55.000000 WebtoonScraper-0.1.1/WebtoonScraper/WebtoonOriginalsScraper.py
--rw-rw-rw-   0        0        0      630 2023-06-21 11:25:23.000000 WebtoonScraper-0.1.1/WebtoonScraper/__init__.py
--rw-rw-rw-   0        0        0     9473 2023-05-17 13:49:27.000000 WebtoonScraper-0.1.1/WebtoonScraper/foldermanagement.py
-drwxrwxrwx   0        0        0        0 2023-06-21 12:03:58.124313 WebtoonScraper-0.1.1/WebtoonScraper.egg-info/
--rw-rw-rw-   0        0        0    10314 2023-06-21 12:03:58.000000 WebtoonScraper-0.1.1/WebtoonScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      653 2023-06-21 12:03:58.000000 WebtoonScraper-0.1.1/WebtoonScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 12:03:58.000000 WebtoonScraper-0.1.1/WebtoonScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 14:16:38.000000 WebtoonScraper-0.1.1/WebtoonScraper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       39 2023-06-21 12:03:58.000000 WebtoonScraper-0.1.1/WebtoonScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-21 12:03:58.000000 WebtoonScraper-0.1.1/WebtoonScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 12:03:58.127315 WebtoonScraper-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1879 2023-06-21 11:51:34.000000 WebtoonScraper-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 12:03:58.125316 WebtoonScraper-0.1.1/test/
--rw-rw-rw-   0        0        0      308 2023-06-21 12:02:19.000000 WebtoonScraper-0.1.1/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-25 12:35:24.685039 WebtoonScraper-0.1.2/
+-rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      140 2023-06-06 01:23:54.000000 WebtoonScraper-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    11009 2023-06-25 12:35:24.684032 WebtoonScraper-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9930 2023-06-22 08:36:45.000000 WebtoonScraper-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 12:35:24.666243 WebtoonScraper-0.1.2/WebtoonScraper/
+-rw-rw-rw-   0        0        0      516 2023-06-06 00:42:00.000000 WebtoonScraper-0.1.2/WebtoonScraper/BestChallengeScraper.py
+-rw-rw-rw-   0        0        0     6198 2023-06-21 11:41:23.000000 WebtoonScraper-0.1.2/WebtoonScraper/BufftoonScraper.py
+-rw-rw-rw-   0        0        0     7405 2023-06-21 11:54:44.000000 WebtoonScraper-0.1.2/WebtoonScraper/NaverPostScraper.py
+-rw-rw-rw-   0        0        0     3332 2023-06-07 11:43:11.000000 WebtoonScraper-0.1.2/WebtoonScraper/NaverWebtoonScraper.py
+-rw-rw-rw-   0        0        0    16629 2023-06-25 12:32:48.000000 WebtoonScraper-0.1.2/WebtoonScraper/Scraper.py
+-rw-rw-rw-   0        0        0     4715 2023-06-25 12:26:12.000000 WebtoonScraper-0.1.2/WebtoonScraper/TelescopeScraper.py
+-rw-rw-rw-   0        0        0     4333 2023-06-22 08:34:53.000000 WebtoonScraper-0.1.2/WebtoonScraper/Webtoon.py
+-rw-rw-rw-   0        0        0      501 2023-06-06 00:44:55.000000 WebtoonScraper-0.1.2/WebtoonScraper/WebtoonCanvasScraper.py
+-rw-rw-rw-   0        0        0     4250 2023-06-17 07:29:55.000000 WebtoonScraper-0.1.2/WebtoonScraper/WebtoonOriginalsScraper.py
+-rw-rw-rw-   0        0        0      630 2023-06-21 11:25:23.000000 WebtoonScraper-0.1.2/WebtoonScraper/__init__.py
+-rw-rw-rw-   0        0        0     9473 2023-05-17 13:49:27.000000 WebtoonScraper-0.1.2/WebtoonScraper/foldermanagement.py
+drwxrwxrwx   0        0        0        0 2023-06-25 12:35:24.681869 WebtoonScraper-0.1.2/WebtoonScraper.egg-info/
+-rw-rw-rw-   0        0        0    11009 2023-06-25 12:35:24.000000 WebtoonScraper-0.1.2/WebtoonScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2023-06-25 12:35:24.000000 WebtoonScraper-0.1.2/WebtoonScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 12:35:24.000000 WebtoonScraper-0.1.2/WebtoonScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 14:16:38.000000 WebtoonScraper-0.1.2/WebtoonScraper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       48 2023-06-25 12:35:24.000000 WebtoonScraper-0.1.2/WebtoonScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-25 12:35:24.000000 WebtoonScraper-0.1.2/WebtoonScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 12:35:24.685039 WebtoonScraper-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1879 2023-06-25 12:34:38.000000 WebtoonScraper-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 12:35:24.682883 WebtoonScraper-0.1.2/test/
+-rw-rw-rw-   0        0        0      339 2023-06-25 12:33:54.000000 WebtoonScraper-0.1.2/test/test.py
```

### Comparing `WebtoonScraper-0.1.1/LICENSE` & `WebtoonScraper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.1/PKG-INFO` & `WebtoonScraper-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: WebtoonScraper
-Version: 0.1.1
+Version: 0.1.2
 Summary: Scraping webtoons and some utils for it
 Home-page: https://github.com/ilotoki0804/WebtoonScraper
 Author: ilotoki0804
 Author-email: ilotoki0804@gmail.com
 License: MIT
-Keywords: Webtoon,Webtoon Scraper,Naver Webtoon,Webtoon Downloader,Download Webtoon,demjson3
+Keywords: Webtoon,Webtoon Scraper,Naver Webtoon,Webtoon Downloader,Download Webtoon
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 이 설명은 최신 버전이 아닐 수 있습니다. 만약 최신 버전을 확인하고 싶으시다면 [여기](https://github.com/ilotoki0804/WebtoonScraper)를 참고하세요.
 # WebtoonScraper
 
 웹툰을 다운로드하는 프로젝트입니다. 그 외에도 웹툰 모아서 보기 등 몇 가지 편의 기능을 지원합니다.
 
+네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 버프툰, 네이버 포스트를 지원합니다.
 # 시작하기
 
 1. 파이썬을 설치합니다.
 2. cmd 창을 열어 다음과 같은 명령어를 칩니다.
 
    ```
    pip install -U WebtoonScraper
@@ -92,42 +93,52 @@
 4. 내려서 Cookie: 라고 되어 있는 모든 내용을 복사합니다.
 5. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
    ```python
    from WebtoonScraper import Webtoon as wt
 
    wt.get_webtoon(1007888, wt.BU) # 첫 번째로 복사했던 숫자를 여기에다 붙여넣으세요.
    ```
+   혹은 다음과 같이 cookie를 코드 내에 포함할 수도 있습니다.
+   ```python
+   from WebtoonScraper import Webtoon as wt
+   cookie = '두 번째로 복사했던 문자를 여기에다 붙여넣으세요.'
+   wt.get_webtoon(1007888, wt.BU, cookie=cookie) # 첫 번째로 복사했던 숫자를 여기에다 붙여넣으세요.
+   ```
 6. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to preceed without cookie)'라는 문구와 함께 입력란이 나오면 두 번째로 복사했던 일련의 문자열을 붙여넣기합니다.
 4. 로그인하면 볼 수 있는 모든 에피소드가 다운로드됩니다.
+
+## 주의사항
+* 버프툰은 titleid를 자동으로 알아내지 않습니다. 하지만 cookie를 입력하면 자동으로 버프툰으로 인식합니다.
+
 # 네이버 포스트 다운로드하기
 
 1. 웹툰이 있는 페이지로 가서 seriesNo와 memberNo를 복사하세요. 예시에서는 각각 597061과 19803452입니다.
    ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/naver_post.png)
-<!-- 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_post(597061, 19803452) # seriesNo와 memberNo를 차례대로 입력해주세요.
-   ``` -->
-2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+   wt.get_webtoon(597061, wt.M) # 우선 seriesNo만 여기에 입력해주세요.
+   ```
+   혹은 memberNo를 코드 내에 포함할 수 있습니다. 
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(597061, wt.M) # 우선 seriesNo만 여기에 입력해주세요.
+   wt.get_webtoon(597061, wt.M, member_no='19803452')
    ```
 3. 'Enter memberNo of 597061(해당 웹툰의 seriesNo)'라는 말과 함께 입력란이 나오면 거기에 아까 복사해 놓은 memberNo를 붙여넣습니다.
+   만약 앞에서 이미 member_no를 사용했다면 이 단계는 건너뛰어집니다.
    ```
-   Enter memberNo 19803452
+   Enter memberNo  of 597061: 19803452
    ...진행됨...
    ```
 4. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
 ## 주의사항
-* get_webtoon이 **아닌** get_post 함수를 사용한다는 점을 주의하세요.
-* 웹툰 태그(Webtoon.P)를 작성할 필요가 없으며 작성하면 오류가 난다는 점을 주의하세요.
-* 가끔씩 이유 없는 오류가 발생할 수 있습니다. 
+* 가끔씩 이유 없는 오류가 발생할 수 있습니다. 그럴 때는 조금 시간이 지난 후에 다시 시도해 보세요.
+* 네이버 포스트는 titleid를 자동으로 알아내지 않습니다. 하지만 member_no를 입력하면 자동으로 포스트로 인식합니다.
 # 여러 회차 하나로 묶기
 
 1. 웹툰을 상기한 대로 다운로드받습니다.
 2. 다음과 같이 코드를 짭니다.
    ```python
    from WebtoonScraper import *
```

### Comparing `WebtoonScraper-0.1.1/README.md` & `WebtoonScraper-0.1.2/WebtoonScraper.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,30 @@
+Metadata-Version: 2.1
+Name: WebtoonScraper
+Version: 0.1.2
+Summary: Scraping webtoons and some utils for it
+Home-page: https://github.com/ilotoki0804/WebtoonScraper
+Author: ilotoki0804
+Author-email: ilotoki0804@gmail.com
+License: MIT
+Keywords: Webtoon,Webtoon Scraper,Naver Webtoon,Webtoon Downloader,Download Webtoon
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+이 설명은 최신 버전이 아닐 수 있습니다. 만약 최신 버전을 확인하고 싶으시다면 [여기](https://github.com/ilotoki0804/WebtoonScraper)를 참고하세요.
 # WebtoonScraper
 
 웹툰을 다운로드하는 프로젝트입니다. 그 외에도 웹툰 모아서 보기 등 몇 가지 편의 기능을 지원합니다.
 
+네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 버프툰, 네이버 포스트를 지원합니다.
 # 시작하기
 
 1. 파이썬을 설치합니다.
 2. cmd 창을 열어 다음과 같은 명령어를 칩니다.
 
    ```
    pip install -U WebtoonScraper
@@ -16,19 +35,19 @@
    ```
    pip3 install -U WebtoonScraper
    ```
 
 # 네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경 다운로드하기
 버프툰과 네이버 포스트는 아래로 가서 확인하세요.
 1. 원하는 웹툰으로 가서 titleid 또는 title_no를 복사하세요.
-   ![img](naver_webtoon.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/naver_webtoon.png)
    국내의 경우 여기에서,
-   ![img](webtoons_original.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/webtoons_original.png)
    해외의 경우는 여기에서,
-   ![img](manhwakyung.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/manhwakyung.png)
    만화경의 경우는 여기에서 확인할 수 있습니다.
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요. 웹툰은 정식 연재와 베스트 도전, Webtoons 오리지널과 캔버스, 만화경 모두 가능합니다.
 
    ```python
    from WebtoonScraper import Webtoon as wt
 
    # 네이버 웹툰
@@ -74,42 +93,52 @@
 4. 내려서 Cookie: 라고 되어 있는 모든 내용을 복사합니다.
 5. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
    ```python
    from WebtoonScraper import Webtoon as wt
 
    wt.get_webtoon(1007888, wt.BU) # 첫 번째로 복사했던 숫자를 여기에다 붙여넣으세요.
    ```
+   혹은 다음과 같이 cookie를 코드 내에 포함할 수도 있습니다.
+   ```python
+   from WebtoonScraper import Webtoon as wt
+   cookie = '두 번째로 복사했던 문자를 여기에다 붙여넣으세요.'
+   wt.get_webtoon(1007888, wt.BU, cookie=cookie) # 첫 번째로 복사했던 숫자를 여기에다 붙여넣으세요.
+   ```
 6. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to preceed without cookie)'라는 문구와 함께 입력란이 나오면 두 번째로 복사했던 일련의 문자열을 붙여넣기합니다.
 4. 로그인하면 볼 수 있는 모든 에피소드가 다운로드됩니다.
+
+## 주의사항
+* 버프툰은 titleid를 자동으로 알아내지 않습니다. 하지만 cookie를 입력하면 자동으로 버프툰으로 인식합니다.
+
 # 네이버 포스트 다운로드하기
 
 1. 웹툰이 있는 페이지로 가서 seriesNo와 memberNo를 복사하세요. 예시에서는 각각 597061과 19803452입니다.
-   ![img](naver_post.png)
-<!-- 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/naver_post.png)
+2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_post(597061, 19803452) # seriesNo와 memberNo를 차례대로 입력해주세요.
-   ``` -->
-2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+   wt.get_webtoon(597061, wt.M) # 우선 seriesNo만 여기에 입력해주세요.
+   ```
+   혹은 memberNo를 코드 내에 포함할 수 있습니다. 
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(597061, wt.M) # 우선 seriesNo만 여기에 입력해주세요.
+   wt.get_webtoon(597061, wt.M, member_no='19803452')
    ```
 3. 'Enter memberNo of 597061(해당 웹툰의 seriesNo)'라는 말과 함께 입력란이 나오면 거기에 아까 복사해 놓은 memberNo를 붙여넣습니다.
+   만약 앞에서 이미 member_no를 사용했다면 이 단계는 건너뛰어집니다.
    ```
-   Enter memberNo 19803452
+   Enter memberNo  of 597061: 19803452
    ...진행됨...
    ```
 4. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
 ## 주의사항
-* get_webtoon이 **아닌** get_post 함수를 사용한다는 점을 주의하세요.
-* 웹툰 태그(Webtoon.P)를 작성할 필요가 없으며 작성하면 오류가 난다는 점을 주의하세요.
-* 가끔씩 이유 없는 오류가 발생할 수 있습니다. 
+* 가끔씩 이유 없는 오류가 발생할 수 있습니다. 그럴 때는 조금 시간이 지난 후에 다시 시도해 보세요.
+* 네이버 포스트는 titleid를 자동으로 알아내지 않습니다. 하지만 member_no를 입력하면 자동으로 포스트로 인식합니다.
 # 여러 회차 하나로 묶기
 
 1. 웹툰을 상기한 대로 다운로드받습니다.
 2. 다음과 같이 코드를 짭니다.
    ```python
    from WebtoonScraper import *
```

### Comparing `WebtoonScraper-0.1.1/WebtoonScraper/BestChallengeScraper.py` & `WebtoonScraper-0.1.2/WebtoonScraper/BestChallengeScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.1/WebtoonScraper/BufftoonScraper.py` & `WebtoonScraper-0.1.2/WebtoonScraper/BufftoonScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.1/WebtoonScraper/NaverPostScraper.py` & `WebtoonScraper-0.1.2/WebtoonScraper/NaverPostScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.1/WebtoonScraper/NaverWebtoonScraper.py` & `WebtoonScraper-0.1.2/WebtoonScraper/NaverWebtoonScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.1/WebtoonScraper/Scraper.py` & `WebtoonScraper-0.1.2/WebtoonScraper/Scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
                                      22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 34, 42, 58, 60, 62, 63, 124):
                     strict_checked_string += ' '
                 else:
                     strict_checked_string += chractor
             return strict_checked_string
         return processed
     
-    def set_folders(self, base_dir: str='Python/files/webtoon') -> None:
+    def set_folders(self, base_dir: str='webtoon') -> None:
         """Set base folder."""
         self.BASE_DIR = Path(base_dir)
 
 ################################## MAIN ACTION ##################################
 
     def download_one_webtoon(self, titleid: int, value_range: tuple|int|None=None) -> None:
         """async를 사용하지 않는 일반 상태일 경우 사용하는 함수이다. 사용법은 download_one_webtoon_async와 동일하다."""
```

### Comparing `WebtoonScraper-0.1.1/WebtoonScraper/TelescopeScraper.py` & `WebtoonScraper-0.1.2/WebtoonScraper/TelescopeScraper.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,20 +8,20 @@
     '''Scrape webtoons from Manhwakyung.'''
     def __init__(self, pbar_independent=False, short_connection=False):
         super().__init__(pbar_independent, short_connection)
         self.BASE_URL = 'https://www.manhwakyung.com'
         self.IS_STABLE_CONNECTION = False
         self.TIMEOUT = 3
 
-    def download_one_webtoon_async(self, titleid, episode_no_range: tuple|int|None=None):
-        self.title, self.list_thumbnail_url, self.grid_thumbnail_url, self.episode_infomation = self._get_episode_infomation(titleid)
+    async def download_one_webtoon_async(self, titleid, episode_no_range: tuple|int|None=None):
+        self.title, self.list_thumbnail_url, self.grid_thumbnail_url, self.episode_infomation = await self._get_episode_infomation(titleid)
         # return await super().download_one_webtoon_async(titleid, episode_no_range)
-        return super().download_one_webtoon_async(titleid, episode_no_range)
+        await super().download_one_webtoon_async(titleid, episode_no_range)
 
-    def _get_episode_infomation(self, titleid):
+    async def _get_episode_infomation(self, titleid):
         XHR_HEADER = {
             "authority": 'api.manhwakyung.com',
             "method": 'GET',
             "path": '/episodes?titleId=180',
             "scheme": 'https',
             "accept": 'application/json, text/plain, */*',
             "accept-encoding": 'gzip, deflate, br',
@@ -36,15 +36,16 @@
             "sec-fetch-dest": 'empty',
             "sec-fetch-mode": 'cors',
             "sec-fetch-site": 'same-site',
             "sec-gpc": '1',
             "user-agent": 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 Edg/113.0.1774.57',
             "version": '3'
         }
-        seasons = self.get_internet('requests', f'https://api.manhwakyung.com/episodes?titleId={titleid}', headers=XHR_HEADER).json()
+        seasons = await self.get_internet('requests', f'https://api.manhwakyung.com/episodes?titleId={titleid}', headers=XHR_HEADER)
+        seasons = seasons.json()
         episodes = []
         for season in seasons['seasons']:
             episodes += season['episodes']
 
         # about webtoon
         title = episodes[0]['title']['name']
         list_thumbnail_url = episodes[0]['title']['listThumbnailImageUrl']
```

### Comparing `WebtoonScraper-0.1.1/WebtoonScraper/Webtoon.py` & `WebtoonScraper-0.1.2/WebtoonScraper/Webtoon.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,22 +65,22 @@
         raise ValueError('webtoon_type should be among naver_webtoon, best_challenge, originals, canvas, and telescope.')
     return webtoonscraper
 
 async def get_webtoon_async(webtoon_id:int, webtoon_type:str=None, *, merge:None|int=None, cookie: None|str=None, member_no: None|int=None) -> None:
     if webtoon_type is None:
         webtoon_type = await auto_webtoon_type(webtoon_id)
     webtoonscraper = await get_webtoon_type(webtoon_type)
-    if webtoon_type.lower() == BUFFTOON:
+    if webtoon_type.lower() == BUFFTOON or cookie is not None:
         if cookie is None:
             webtoonscraper.COOKIE = cookie
         else:
             webtoonscraper.COOKIE = input(f'Enter cookie of {webtoon_id} (Enter nothing to preceed without cookie)')
-    if webtoon_type.lower() == NAVER_POST:
+    if webtoon_type.lower() == NAVER_POST or member_no is not None:
         if not member_no:
-            member_no = int(input(f'Enter memberNo of {webtoon_id}'))
+            member_no = int(input(f'Enter memberNo of {webtoon_id}: '))
         await webtoonscraper.download_one_webtoon_async(titleid=webtoon_id, member_no=member_no)
     else:
         await webtoonscraper.download_one_webtoon_async(titleid=webtoon_id)
     if merge:
         fd = WebtoonFolderManagement('webtoon_merge')
         fd.divide_all_webtoons(merge)
```

### Comparing `WebtoonScraper-0.1.1/WebtoonScraper/WebtoonOriginalsScraper.py` & `WebtoonScraper-0.1.2/WebtoonScraper/WebtoonOriginalsScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.1/WebtoonScraper/__init__.py` & `WebtoonScraper-0.1.2/WebtoonScraper/__init__.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.1/WebtoonScraper/foldermanagement.py` & `WebtoonScraper-0.1.2/WebtoonScraper/foldermanagement.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.1/WebtoonScraper.egg-info/PKG-INFO` & `WebtoonScraper-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,12 @@
-Metadata-Version: 2.1
-Name: WebtoonScraper
-Version: 0.1.1
-Summary: Scraping webtoons and some utils for it
-Home-page: https://github.com/ilotoki0804/WebtoonScraper
-Author: ilotoki0804
-Author-email: ilotoki0804@gmail.com
-License: MIT
-Keywords: Webtoon,Webtoon Scraper,Naver Webtoon,Webtoon Downloader,Download Webtoon,demjson3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-이 설명은 최신 버전이 아닐 수 있습니다. 만약 최신 버전을 확인하고 싶으시다면 [여기](https://github.com/ilotoki0804/WebtoonScraper)를 참고하세요.
 # WebtoonScraper
 
 웹툰을 다운로드하는 프로젝트입니다. 그 외에도 웹툰 모아서 보기 등 몇 가지 편의 기능을 지원합니다.
 
+네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 버프툰, 네이버 포스트를 지원합니다.
 # 시작하기
 
 1. 파이썬을 설치합니다.
 2. cmd 창을 열어 다음과 같은 명령어를 칩니다.
 
    ```
    pip install -U WebtoonScraper
@@ -34,19 +17,19 @@
    ```
    pip3 install -U WebtoonScraper
    ```
 
 # 네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경 다운로드하기
 버프툰과 네이버 포스트는 아래로 가서 확인하세요.
 1. 원하는 웹툰으로 가서 titleid 또는 title_no를 복사하세요.
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/naver_webtoon.png)
+   ![img](naver_webtoon.png)
    국내의 경우 여기에서,
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/webtoons_original.png)
+   ![img](webtoons_original.png)
    해외의 경우는 여기에서,
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/manhwakyung.png)
+   ![img](manhwakyung.png)
    만화경의 경우는 여기에서 확인할 수 있습니다.
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요. 웹툰은 정식 연재와 베스트 도전, Webtoons 오리지널과 캔버스, 만화경 모두 가능합니다.
 
    ```python
    from WebtoonScraper import Webtoon as wt
 
    # 네이버 웹툰
@@ -92,42 +75,52 @@
 4. 내려서 Cookie: 라고 되어 있는 모든 내용을 복사합니다.
 5. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
    ```python
    from WebtoonScraper import Webtoon as wt
 
    wt.get_webtoon(1007888, wt.BU) # 첫 번째로 복사했던 숫자를 여기에다 붙여넣으세요.
    ```
+   혹은 다음과 같이 cookie를 코드 내에 포함할 수도 있습니다.
+   ```python
+   from WebtoonScraper import Webtoon as wt
+   cookie = '두 번째로 복사했던 문자를 여기에다 붙여넣으세요.'
+   wt.get_webtoon(1007888, wt.BU, cookie=cookie) # 첫 번째로 복사했던 숫자를 여기에다 붙여넣으세요.
+   ```
 6. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to preceed without cookie)'라는 문구와 함께 입력란이 나오면 두 번째로 복사했던 일련의 문자열을 붙여넣기합니다.
 4. 로그인하면 볼 수 있는 모든 에피소드가 다운로드됩니다.
+
+## 주의사항
+* 버프툰은 titleid를 자동으로 알아내지 않습니다. 하지만 cookie를 입력하면 자동으로 버프툰으로 인식합니다.
+
 # 네이버 포스트 다운로드하기
 
 1. 웹툰이 있는 페이지로 가서 seriesNo와 memberNo를 복사하세요. 예시에서는 각각 597061과 19803452입니다.
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/naver_post.png)
-<!-- 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+   ![img](naver_post.png)
+2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_post(597061, 19803452) # seriesNo와 memberNo를 차례대로 입력해주세요.
-   ``` -->
-2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+   wt.get_webtoon(597061, wt.M) # 우선 seriesNo만 여기에 입력해주세요.
+   ```
+   혹은 memberNo를 코드 내에 포함할 수 있습니다. 
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon(597061, wt.M) # 우선 seriesNo만 여기에 입력해주세요.
+   wt.get_webtoon(597061, wt.M, member_no='19803452')
    ```
 3. 'Enter memberNo of 597061(해당 웹툰의 seriesNo)'라는 말과 함께 입력란이 나오면 거기에 아까 복사해 놓은 memberNo를 붙여넣습니다.
+   만약 앞에서 이미 member_no를 사용했다면 이 단계는 건너뛰어집니다.
    ```
-   Enter memberNo 19803452
+   Enter memberNo  of 597061: 19803452
    ...진행됨...
    ```
 4. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
 ## 주의사항
-* get_webtoon이 **아닌** get_post 함수를 사용한다는 점을 주의하세요.
-* 웹툰 태그(Webtoon.P)를 작성할 필요가 없으며 작성하면 오류가 난다는 점을 주의하세요.
-* 가끔씩 이유 없는 오류가 발생할 수 있습니다. 
+* 가끔씩 이유 없는 오류가 발생할 수 있습니다. 그럴 때는 조금 시간이 지난 후에 다시 시도해 보세요.
+* 네이버 포스트는 titleid를 자동으로 알아내지 않습니다. 하지만 member_no를 입력하면 자동으로 포스트로 인식합니다.
 # 여러 회차 하나로 묶기
 
 1. 웹툰을 상기한 대로 다운로드받습니다.
 2. 다음과 같이 코드를 짭니다.
    ```python
    from WebtoonScraper import *
```

### Comparing `WebtoonScraper-0.1.1/WebtoonScraper.egg-info/SOURCES.txt` & `WebtoonScraper-0.1.2/WebtoonScraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.1/setup.py` & `WebtoonScraper-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,25 +6,25 @@
     long_description = long_description.replace('naver_webtoon.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/naver_webtoon.png')
     long_description = long_description.replace('webtoons_original.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/webtoons_original.png')
     long_description = long_description.replace('manhwakyung.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/manhwakyung.png')
     long_description = long_description.replace('naver_post.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/naver_post.png')
 
 setup(
     name='WebtoonScraper',
-    version='0.1.1',
+    version='0.1.2',
     description='Scraping webtoons and some utils for it',
     author='ilotoki0804',
     author_email='ilotoki0804@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/ilotoki0804/WebtoonScraper',
-    install_requires=['tqdm', 'bs4', 'requests', 'better_abc', 'async_lru'],
+    install_requires=['tqdm', 'bs4', 'requests', 'better_abc', 'async_lru', 'demjson3'],
     packages=find_packages(exclude=[]),
-    keywords=['Webtoon', 'Webtoon Scraper', 'Naver Webtoon', 'Webtoon Downloader', 'Download Webtoon', 'demjson3'],
+    keywords=['Webtoon', 'Webtoon Scraper', 'Naver Webtoon', 'Webtoon Downloader', 'Download Webtoon'],
     python_requires='>=3.10',
     package_data={},
     zip_safe=False,
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         'Programming Language :: Python :: 3.10',
```

