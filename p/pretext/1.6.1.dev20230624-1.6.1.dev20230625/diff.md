# Comparing `tmp/pretext-1.6.1.dev20230624.tar.gz` & `tmp/pretext-1.6.1.dev20230625.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.6.1.dev20230624.tar", max compression
+gzip compressed data, was "pretext-1.6.1.dev20230625.tar", max compression
```

## Comparing `pretext-1.6.1.dev20230624.tar` & `pretext-1.6.1.dev20230625.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35148 2023-06-24 06:20:20.721768 pretext-1.6.1.dev20230624/LICENSE
--rw-r--r--   0        0        0     9757 2023-06-24 06:20:20.721768 pretext-1.6.1.dev20230624/README.md
--rw-r--r--   0        0        0     1909 2023-06-24 06:21:01.642387 pretext-1.6.1.dev20230624/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-06-24 06:20:20.725768 pretext-1.6.1.dev20230624/pretext/__main__.py
--rw-r--r--   0        0        0     8531 2023-06-24 06:20:20.725768 pretext-1.6.1.dev20230624/pretext/build.py
--rw-r--r--   0        0        0    25561 2023-06-24 06:20:20.725768 pretext-1.6.1.dev20230624/pretext/cli.py
--rw-r--r--   0        0        0     5856 2023-06-24 06:20:20.725768 pretext-1.6.1.dev20230624/pretext/codechat.py
--rw-r--r--   0        0        0     5943 2023-06-24 06:20:20.725768 pretext-1.6.1.dev20230624/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-06-24 06:20:20.725768 pretext-1.6.1.dev20230624/pretext/core/__init__.py
--rw-r--r--   0        0        0   172432 2023-06-24 06:21:06.398458 pretext-1.6.1.dev20230624/pretext/core/pretext.py
--rw-r--r--   0        0        0     1484 2023-06-24 06:20:20.725768 pretext-1.6.1.dev20230624/pretext/core/resources.py
--rw-r--r--   0        0        0  1035425 2023-06-24 06:21:06.398458 pretext-1.6.1.dev20230624/pretext/core/resources.zip
--rw-r--r--   0        0        0    16741 2023-06-24 06:20:20.725768 pretext-1.6.1.dev20230624/pretext/generate.py
--rw-r--r--   0        0        0    31778 2023-06-24 06:20:20.725768 pretext-1.6.1.dev20230624/pretext/project.py
--rw-r--r--   0        0        0      739 2023-06-24 06:20:20.725768 pretext-1.6.1.dev20230624/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-06-24 06:21:06.466459 pretext-1.6.1.dev20230624/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-06-24 06:21:06.466459 pretext-1.6.1.dev20230624/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160110 2023-06-24 06:21:06.442459 pretext-1.6.1.dev20230624/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     7616 2023-06-24 06:21:06.446459 pretext-1.6.1.dev20230624/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173309 2023-06-24 06:21:06.466459 pretext-1.6.1.dev20230624/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     2192 2023-06-24 06:21:06.466459 pretext-1.6.1.dev20230624/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     4657 2023-06-24 06:21:06.454459 pretext-1.6.1.dev20230624/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0     1710 2023-06-24 06:21:06.466459 pretext-1.6.1.dev20230624/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-06-24 06:21:06.466459 pretext-1.6.1.dev20230624/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8392 2023-06-24 06:21:06.450459 pretext-1.6.1.dev20230624/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    19529 2023-06-24 06:20:20.725768 pretext-1.6.1.dev20230624/pretext/utils.py
--rw-r--r--   0        0        0     3333 2023-06-24 06:21:01.642387 pretext-1.6.1.dev20230624/pyproject.toml
--rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230624/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-25 06:20:11.550752 pretext-1.6.1.dev20230625/LICENSE
+-rw-r--r--   0        0        0     9757 2023-06-25 06:20:11.550752 pretext-1.6.1.dev20230625/README.md
+-rw-r--r--   0        0        0     1909 2023-06-25 06:20:48.727156 pretext-1.6.1.dev20230625/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-25 06:20:11.550752 pretext-1.6.1.dev20230625/pretext/__main__.py
+-rw-r--r--   0        0        0     8531 2023-06-25 06:20:11.550752 pretext-1.6.1.dev20230625/pretext/build.py
+-rw-r--r--   0        0        0    25561 2023-06-25 06:20:11.550752 pretext-1.6.1.dev20230625/pretext/cli.py
+-rw-r--r--   0        0        0     5856 2023-06-25 06:20:11.550752 pretext-1.6.1.dev20230625/pretext/codechat.py
+-rw-r--r--   0        0        0     5943 2023-06-25 06:20:11.550752 pretext-1.6.1.dev20230625/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-06-25 06:20:11.550752 pretext-1.6.1.dev20230625/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172432 2023-06-25 06:20:54.051200 pretext-1.6.1.dev20230625/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1484 2023-06-25 06:20:11.550752 pretext-1.6.1.dev20230625/pretext/core/resources.py
+-rw-r--r--   0        0        0  1035425 2023-06-25 06:20:54.051200 pretext-1.6.1.dev20230625/pretext/core/resources.zip
+-rw-r--r--   0        0        0    16741 2023-06-25 06:20:11.554751 pretext-1.6.1.dev20230625/pretext/generate.py
+-rw-r--r--   0        0        0    31778 2023-06-25 06:20:11.554751 pretext-1.6.1.dev20230625/pretext/project.py
+-rw-r--r--   0        0        0      739 2023-06-25 06:20:11.554751 pretext-1.6.1.dev20230625/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-06-25 06:20:54.143201 pretext-1.6.1.dev20230625/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-25 06:20:54.143201 pretext-1.6.1.dev20230625/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160110 2023-06-25 06:20:54.111200 pretext-1.6.1.dev20230625/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7616 2023-06-25 06:20:54.115201 pretext-1.6.1.dev20230625/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173309 2023-06-25 06:20:54.139201 pretext-1.6.1.dev20230625/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     2192 2023-06-25 06:20:54.143201 pretext-1.6.1.dev20230625/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4657 2023-06-25 06:20:54.123201 pretext-1.6.1.dev20230625/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0     1710 2023-06-25 06:20:54.139201 pretext-1.6.1.dev20230625/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-06-25 06:20:54.139201 pretext-1.6.1.dev20230625/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8392 2023-06-25 06:20:54.119201 pretext-1.6.1.dev20230625/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    19529 2023-06-25 06:20:11.554751 pretext-1.6.1.dev20230625/pretext/utils.py
+-rw-r--r--   0        0        0     3333 2023-06-25 06:20:48.731156 pretext-1.6.1.dev20230625/pyproject.toml
+-rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230625/PKG-INFO
```

### Comparing `pretext-1.6.1.dev20230624/LICENSE` & `pretext-1.6.1.dev20230625/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230624/README.md` & `pretext-1.6.1.dev20230625/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230624/pretext/__init__.py` & `pretext-1.6.1.dev20230625/pretext/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230624/pretext/build.py` & `pretext-1.6.1.dev20230625/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230624/pretext/cli.py` & `pretext-1.6.1.dev20230625/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230624/pretext/codechat.py` & `pretext-1.6.1.dev20230625/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230624/pretext/config/xml_overlay.py` & `pretext-1.6.1.dev20230625/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230624/pretext/core/pretext.py` & `pretext-1.6.1.dev20230625/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230624/pretext/core/resources.py` & `pretext-1.6.1.dev20230625/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230624/pretext/core/resources.zip` & `pretext-1.6.1.dev20230625/pretext/core/resources.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,143 +1,143 @@
 Zip file size: 1035425 bytes, number of entries: 141
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:21 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:21 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:21 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:21 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:21 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:21 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-Jun-24 06:21 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-Jun-24 06:21 script/mbx
--rw-r--r--  2.0 unx      481 b- defN 23-Jun-24 06:21 script/mjsre/README.md
--rw-r--r--  2.0 unx      116 b- defN 23-Jun-24 06:21 script/mjsre/package.json
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-24 06:21 script/mjsre/update-sre
--rw-r--r--  2.0 unx     9251 b- defN 23-Jun-24 06:21 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-24 06:21 pretext/__init__.py
--rw-r--r--  2.0 unx    30908 b- defN 23-Jun-24 06:21 pretext/pretext
--rw-r--r--  2.0 unx     1367 b- defN 23-Jun-24 06:21 pretext/README.md
--rw-r--r--  2.0 unx     2566 b- defN 23-Jun-24 06:21 pretext/pretext.cfg
--rw-r--r--  2.0 unx   172432 b- defN 23-Jun-24 06:21 pretext/pretext.py
--rw-r--r--  2.0 unx     1955 b- defN 23-Jun-24 06:21 pretext/module-test.py
--rw-r--r--  2.0 unx    35449 b- defN 23-Jun-24 06:21 pretext/braille_format.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:21 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:21 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:21 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:21 xsl/utilities/
--rw-r--r--  2.0 unx     2248 b- defN 23-Jun-24 06:21 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx   612399 b- defN 23-Jun-24 06:21 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx    12084 b- defN 23-Jun-24 06:21 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx   231248 b- defN 23-Jun-24 06:21 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-Jun-24 06:21 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-Jun-24 06:21 xsl/README.md
--rw-r--r--  2.0 unx    39918 b- defN 23-Jun-24 06:21 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-Jun-24 06:21 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx   546938 b- defN 23-Jun-24 06:21 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-Jun-24 06:21 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-Jun-24 06:21 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx   109017 b- defN 23-Jun-24 06:21 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-Jun-24 06:21 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-Jun-24 06:21 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-Jun-24 06:21 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-Jun-24 06:21 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-Jun-24 06:21 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx   544229 b- defN 23-Jun-24 06:21 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-Jun-24 06:21 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-Jun-24 06:21 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-Jun-24 06:21 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx   112450 b- defN 23-Jun-24 06:21 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-Jun-24 06:21 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-Jun-24 06:21 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-Jun-24 06:21 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-Jun-24 06:21 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-Jun-24 06:21 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-Jun-24 06:21 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-Jun-24 06:21 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-Jun-24 06:21 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-Jun-24 06:21 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-Jun-24 06:21 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-Jun-24 06:21 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx    89128 b- defN 23-Jun-24 06:21 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx   139486 b- defN 23-Jun-24 06:21 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-Jun-24 06:21 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-Jun-24 06:21 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-Jun-24 06:21 xsl/entities.ent
--rw-r--r--  2.0 unx     6066 b- defN 23-Jun-24 06:21 xsl/pretext-json-manifest.xsl
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:21 xsl/support/play-button/
--rw-r--r--  2.0 unx      504 b- defN 23-Jun-24 06:21 xsl/support/README.md
--rw-r--r--  2.0 unx     5065 b- defN 23-Jun-24 06:21 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx    10306 b- defN 23-Jun-24 06:21 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5800 b- defN 23-Jun-24 06:21 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-Jun-24 06:21 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx      486 b- defN 23-Jun-24 06:21 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5879 b- defN 23-Jun-24 06:21 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx     2657 b- defN 23-Jun-24 06:21 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx      722 b- defN 23-Jun-24 06:21 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     6621 b- defN 23-Jun-24 06:21 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx    14482 b- defN 23-Jun-24 06:21 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-Jun-24 06:21 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-Jun-24 06:21 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-Jun-24 06:21 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-Jun-24 06:21 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx    17040 b- defN 23-Jun-24 06:21 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx     2227 b- defN 23-Jun-24 06:21 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    16518 b- defN 23-Jun-24 06:21 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx     4708 b- defN 23-Jun-24 06:21 xsl/localizations/README.md
--rw-r--r--  2.0 unx    17215 b- defN 23-Jun-24 06:21 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    16821 b- defN 23-Jun-24 06:21 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    16333 b- defN 23-Jun-24 06:21 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    16484 b- defN 23-Jun-24 06:21 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17065 b- defN 23-Jun-24 06:21 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    17285 b- defN 23-Jun-24 06:21 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx    19169 b- defN 23-Jun-24 06:21 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    15566 b- defN 23-Jun-24 06:21 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    15938 b- defN 23-Jun-24 06:21 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16236 b- defN 23-Jun-24 06:21 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    16296 b- defN 23-Jun-24 06:21 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx    19049 b- defN 23-Jun-24 06:21 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    16069 b- defN 23-Jun-24 06:21 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx      787 b- defN 23-Jun-24 06:21 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx     1810 b- defN 23-Jun-24 06:21 xsl/utilities/README.md
--rw-r--r--  2.0 unx      513 b- defN 23-Jun-24 06:21 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4926 b- defN 23-Jun-24 06:21 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx    30257 b- defN 23-Jun-24 06:21 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4299 b- defN 23-Jun-24 06:21 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx    34210 b- defN 23-Jun-24 06:21 schema/pretext-dev.rng
--rw-r--r--  2.0 unx    17587 b- defN 23-Jun-24 06:21 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx     1180 b- defN 23-Jun-24 06:21 schema/README.md
--rw-r--r--  2.0 unx    18421 b- defN 23-Jun-24 06:21 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx   101829 b- defN 23-Jun-24 06:21 schema/pretext.rng
--rw-r--r--  2.0 unx   134043 b- defN 23-Jun-24 06:21 schema/pretext.xml
--rw-r--r--  2.0 unx    58086 b- defN 23-Jun-24 06:21 schema/pretext.rnc
--rw-r--r--  2.0 unx     3135 b- defN 23-Jun-24 06:21 schema/build.sh
--rw-r--r--  2.0 unx      326 b- defN 23-Jun-24 06:21 schema/xml.xsd
--rw-r--r--  2.0 unx    25870 b- defN 23-Jun-24 06:21 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx   125135 b- defN 23-Jun-24 06:21 schema/pretext.xsd
--rw-r--r--  2.0 unx     2446 b- defN 23-Jun-24 06:21 css/colors_martiansands.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jun-24 06:21 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     1276 b- defN 23-Jun-24 06:21 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx     4021 b- defN 23-Jun-24 06:21 css/update_css
--rw-r--r--  2.0 unx     1865 b- defN 23-Jun-24 06:21 css/README.md
--rw-r--r--  2.0 unx      691 b- defN 23-Jun-24 06:21 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx    12567 b- defN 23-Jun-24 06:21 css/style_oscarlevin.css
--rw-r--r--  2.0 unx   146685 b- defN 23-Jun-24 06:21 css/mathbook-content.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-24 06:21 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2608 b- defN 23-Jun-24 06:21 css/colors_default.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-24 06:21 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     2438 b- defN 23-Jun-24 06:21 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     1338 b- defN 23-Jun-24 06:21 css/colors_red_blue.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-24 06:21 css/colors_orange_navy.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-24 06:21 css/colors_green_blue.css
--rw-r--r--  2.0 unx     1362 b- defN 23-Jun-24 06:21 css/epub.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-24 06:21 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx    22438 b- defN 23-Jun-24 06:21 css/pretext.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-24 06:21 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-24 06:21 css/colors_green_plum.css
--rw-r--r--  2.0 unx     2441 b- defN 23-Jun-24 06:21 css/kindle.css
--rw-r--r--  2.0 unx     7761 b- defN 23-Jun-24 06:21 css/style_default.css
--rw-r--r--  2.0 unx    71198 b- defN 23-Jun-24 06:21 css/pretext_add_on.css
--rw-r--r--  2.0 unx    14069 b- defN 23-Jun-24 06:21 css/setcolors.css
--rw-r--r--  2.0 unx     3473 b- defN 23-Jun-24 06:21 css/style_soundwriting.css
--rw-r--r--  2.0 unx     4308 b- defN 23-Jun-24 06:21 css/colors_blue_green.css
--rw-r--r--  2.0 unx     1280 b- defN 23-Jun-24 06:21 css/colors_brown_gold.css
--rw-r--r--  2.0 unx   435680 b- defN 23-Jun-24 06:21 css/mathbook-3.css
--rw-r--r--  2.0 unx    63664 b- defN 23-Jun-24 06:21 css/mathbook-add-on.css
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-Jun-25 06:20 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-Jun-25 06:20 script/mbx
+-rw-r--r--  2.0 unx      481 b- defN 23-Jun-25 06:20 script/mjsre/README.md
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-25 06:20 script/mjsre/package.json
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-25 06:20 script/mjsre/update-sre
+-rw-r--r--  2.0 unx     9251 b- defN 23-Jun-25 06:20 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-25 06:20 pretext/__init__.py
+-rw-r--r--  2.0 unx    30908 b- defN 23-Jun-25 06:20 pretext/pretext
+-rw-r--r--  2.0 unx     1367 b- defN 23-Jun-25 06:20 pretext/README.md
+-rw-r--r--  2.0 unx     2566 b- defN 23-Jun-25 06:20 pretext/pretext.cfg
+-rw-r--r--  2.0 unx   172432 b- defN 23-Jun-25 06:20 pretext/pretext.py
+-rw-r--r--  2.0 unx     1955 b- defN 23-Jun-25 06:20 pretext/module-test.py
+-rw-r--r--  2.0 unx    35449 b- defN 23-Jun-25 06:20 pretext/braille_format.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 xsl/utilities/
+-rw-r--r--  2.0 unx     2248 b- defN 23-Jun-25 06:20 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx   612399 b- defN 23-Jun-25 06:20 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx    12084 b- defN 23-Jun-25 06:20 xsl/xml-to-json.xsl
+-rw-r--r--  2.0 unx   231248 b- defN 23-Jun-25 06:20 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-Jun-25 06:20 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-Jun-25 06:20 xsl/README.md
+-rw-r--r--  2.0 unx    39918 b- defN 23-Jun-25 06:20 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-Jun-25 06:20 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx   546938 b- defN 23-Jun-25 06:20 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-Jun-25 06:20 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-Jun-25 06:20 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx   109017 b- defN 23-Jun-25 06:20 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-Jun-25 06:20 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx    13186 b- defN 23-Jun-25 06:20 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-Jun-25 06:20 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-Jun-25 06:20 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-Jun-25 06:20 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx   544229 b- defN 23-Jun-25 06:20 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-Jun-25 06:20 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-Jun-25 06:20 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-Jun-25 06:20 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx   112450 b- defN 23-Jun-25 06:20 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-Jun-25 06:20 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-Jun-25 06:20 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-Jun-25 06:20 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-Jun-25 06:20 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-Jun-25 06:20 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-Jun-25 06:20 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 23-Jun-25 06:20 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-Jun-25 06:20 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-Jun-25 06:20 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-Jun-25 06:20 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-Jun-25 06:20 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx    89128 b- defN 23-Jun-25 06:20 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx   139486 b- defN 23-Jun-25 06:20 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-Jun-25 06:20 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-Jun-25 06:20 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-Jun-25 06:20 xsl/entities.ent
+-rw-r--r--  2.0 unx     6066 b- defN 23-Jun-25 06:20 xsl/pretext-json-manifest.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 xsl/support/play-button/
+-rw-r--r--  2.0 unx      504 b- defN 23-Jun-25 06:20 xsl/support/README.md
+-rw-r--r--  2.0 unx     5065 b- defN 23-Jun-25 06:20 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx    10306 b- defN 23-Jun-25 06:20 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5800 b- defN 23-Jun-25 06:20 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-Jun-25 06:20 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx      486 b- defN 23-Jun-25 06:20 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5879 b- defN 23-Jun-25 06:20 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx     2657 b- defN 23-Jun-25 06:20 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx      722 b- defN 23-Jun-25 06:20 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     6621 b- defN 23-Jun-25 06:20 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx    14482 b- defN 23-Jun-25 06:20 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-Jun-25 06:20 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-Jun-25 06:20 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-Jun-25 06:20 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-Jun-25 06:20 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx    17040 b- defN 23-Jun-25 06:20 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx     2227 b- defN 23-Jun-25 06:20 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    16518 b- defN 23-Jun-25 06:20 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx     4708 b- defN 23-Jun-25 06:20 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    17215 b- defN 23-Jun-25 06:20 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    16821 b- defN 23-Jun-25 06:20 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    16333 b- defN 23-Jun-25 06:20 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    16484 b- defN 23-Jun-25 06:20 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    17065 b- defN 23-Jun-25 06:20 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    17285 b- defN 23-Jun-25 06:20 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    19169 b- defN 23-Jun-25 06:20 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    15566 b- defN 23-Jun-25 06:20 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    15938 b- defN 23-Jun-25 06:20 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16236 b- defN 23-Jun-25 06:20 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    16296 b- defN 23-Jun-25 06:20 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx    19049 b- defN 23-Jun-25 06:20 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    16069 b- defN 23-Jun-25 06:20 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx      787 b- defN 23-Jun-25 06:20 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx     1810 b- defN 23-Jun-25 06:20 xsl/utilities/README.md
+-rw-r--r--  2.0 unx      513 b- defN 23-Jun-25 06:20 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4926 b- defN 23-Jun-25 06:20 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx    30257 b- defN 23-Jun-25 06:20 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4299 b- defN 23-Jun-25 06:20 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx    34210 b- defN 23-Jun-25 06:20 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx    17587 b- defN 23-Jun-25 06:20 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx     1180 b- defN 23-Jun-25 06:20 schema/README.md
+-rw-r--r--  2.0 unx    18421 b- defN 23-Jun-25 06:20 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx   101829 b- defN 23-Jun-25 06:20 schema/pretext.rng
+-rw-r--r--  2.0 unx   134043 b- defN 23-Jun-25 06:20 schema/pretext.xml
+-rw-r--r--  2.0 unx    58086 b- defN 23-Jun-25 06:20 schema/pretext.rnc
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jun-25 06:20 schema/build.sh
+-rw-r--r--  2.0 unx      326 b- defN 23-Jun-25 06:20 schema/xml.xsd
+-rw-r--r--  2.0 unx    25870 b- defN 23-Jun-25 06:20 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx   125135 b- defN 23-Jun-25 06:20 schema/pretext.xsd
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-25 06:20 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-25 06:20 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     1276 b- defN 23-Jun-25 06:20 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-Jun-25 06:20 css/update_css
+-rw-r--r--  2.0 unx     1865 b- defN 23-Jun-25 06:20 css/README.md
+-rw-r--r--  2.0 unx      691 b- defN 23-Jun-25 06:20 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-Jun-25 06:20 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-Jun-25 06:20 css/mathbook-content.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-25 06:20 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-Jun-25 06:20 css/colors_default.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-25 06:20 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-Jun-25 06:20 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-Jun-25 06:20 css/colors_red_blue.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-25 06:20 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-25 06:20 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-Jun-25 06:20 css/epub.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-25 06:20 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-Jun-25 06:20 css/pretext.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-25 06:20 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-25 06:20 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-Jun-25 06:20 css/kindle.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-Jun-25 06:20 css/style_default.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-Jun-25 06:20 css/pretext_add_on.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-Jun-25 06:20 css/setcolors.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-Jun-25 06:20 css/style_soundwriting.css
+-rw-r--r--  2.0 unx     4308 b- defN 23-Jun-25 06:20 css/colors_blue_green.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-Jun-25 06:20 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-Jun-25 06:20 css/mathbook-3.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-Jun-25 06:20 css/mathbook-add-on.css
 141 files, 4814466 bytes uncompressed, 1017983 bytes compressed:  78.9%
```

### Comparing `pretext-1.6.1.dev20230624/pretext/generate.py` & `pretext-1.6.1.dev20230625/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230624/pretext/project.py` & `pretext-1.6.1.dev20230625/pretext/project.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230624/pretext/templates/__init__.py` & `pretext-1.6.1.dev20230625/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230624/pretext/templates/resources/.gitignore` & `pretext-1.6.1.dev20230625/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230624/pretext/templates/resources/article.zip` & `pretext-1.6.1.dev20230625/pretext/templates/resources/article.zip`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
 Zip file size: 160110 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:21 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:20 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:20 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:20 source/
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-24 06:21 project.ptx
--rw-r--r--  2.0 unx       86 b- defN 23-Jun-24 06:20 README.md
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-24 06:21 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-24 06:21 codechat_config.yaml
--rw-r--r--  2.0 unx     2192 b- defN 23-Jun-24 06:21 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx   154806 b- defN 23-Jun-24 06:20 assets/frog.jpg
--rw-r--r--  2.0 unx      449 b- defN 23-Jun-24 06:20 source/section-1.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-Jun-24 06:20 source/section-2.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-Jun-24 06:20 source/main.ptx
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-24 06:20 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 source/
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-25 06:20 project.ptx
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-25 06:20 README.md
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-25 06:20 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-25 06:20 codechat_config.yaml
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-25 06:20 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jun-25 06:20 assets/frog.jpg
+-rw-r--r--  2.0 unx      449 b- defN 23-Jun-25 06:20 source/section-1.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-Jun-25 06:20 source/section-2.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-Jun-25 06:20 source/main.ptx
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-25 06:20 publication/publication.ptx
 14 files, 164841 bytes uncompressed, 158588 bytes compressed:  3.8%
```

### Comparing `pretext-1.6.1.dev20230624/pretext/templates/resources/book.zip` & `pretext-1.6.1.dev20230625/pretext/templates/resources/book.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 7616 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:21 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:20 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:20 source/
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-24 06:21 project.ptx
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-24 06:20 README.md
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-24 06:21 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-24 06:21 codechat_config.yaml
--rw-r--r--  2.0 unx     2192 b- defN 23-Jun-24 06:21 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     1767 b- defN 23-Jun-24 06:20 source/main.ptx
--rw-r--r--  2.0 unx     6114 b- defN 23-Jun-24 06:20 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 source/
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-25 06:20 project.ptx
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-25 06:20 README.md
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-25 06:20 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-25 06:20 codechat_config.yaml
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-25 06:20 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     1767 b- defN 23-Jun-25 06:20 source/main.ptx
+-rw-r--r--  2.0 unx     6114 b- defN 23-Jun-25 06:20 publication/publication.ptx
 10 files, 15809 bytes uncompressed, 6522 bytes compressed:  58.7%
```

### Comparing `pretext-1.6.1.dev20230624/pretext/templates/resources/demo.zip` & `pretext-1.6.1.dev20230625/pretext/templates/resources/demo.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,36 +1,36 @@
 Zip file size: 173309 bytes, number of entries: 34
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:21 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:20 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:20 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:20 source/
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-24 06:21 project.ptx
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-24 06:20 README.md
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-24 06:21 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-24 06:21 codechat_config.yaml
--rw-r--r--  2.0 unx     2192 b- defN 23-Jun-24 06:21 .devcontainer/devcontainer.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:20 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-Jun-24 06:20 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-Jun-24 06:20 assets/jsxgraph/infinity.js
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:20 source/images/
--rw-r--r--  2.0 unx     1515 b- defN 23-Jun-24 06:20 source/ex-first.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-Jun-24 06:20 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-Jun-24 06:20 source/ch-empty.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-Jun-24 06:20 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-Jun-24 06:20 source/frontmatter.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-Jun-24 06:20 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-Jun-24 06:20 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-Jun-24 06:20 source/sec-features.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-Jun-24 06:20 source/fig-tikz.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-Jun-24 06:20 source/ch-generate.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-Jun-24 06:20 source/ch-features.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-Jun-24 06:20 source/docinfo.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-Jun-24 06:20 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-Jun-24 06:20 source/main.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-Jun-24 06:20 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-Jun-24 06:20 source/backmatter.ptx
--rw-r--r--  2.0 unx      835 b- defN 23-Jun-24 06:20 source/images/cflag.asy
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-24 06:20 source/images/sageplot2d.sage
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-24 06:20 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx      357 b- defN 23-Jun-24 06:20 source/images/tikz.tex
--rw-r--r--  2.0 unx     6092 b- defN 23-Jun-24 06:20 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 source/
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-25 06:20 project.ptx
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-25 06:20 README.md
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-25 06:20 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-25 06:20 codechat_config.yaml
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-25 06:20 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jun-25 06:20 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-Jun-25 06:20 assets/jsxgraph/infinity.js
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 source/images/
+-rw-r--r--  2.0 unx     1515 b- defN 23-Jun-25 06:20 source/ex-first.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-Jun-25 06:20 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-Jun-25 06:20 source/ch-empty.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-Jun-25 06:20 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-Jun-25 06:20 source/frontmatter.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-Jun-25 06:20 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-Jun-25 06:20 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-Jun-25 06:20 source/sec-features.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-Jun-25 06:20 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jun-25 06:20 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      339 b- defN 23-Jun-25 06:20 source/ch-features.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-Jun-25 06:20 source/docinfo.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-Jun-25 06:20 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jun-25 06:20 source/main.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-Jun-25 06:20 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-Jun-25 06:20 source/backmatter.ptx
+-rw-r--r--  2.0 unx      835 b- defN 23-Jun-25 06:20 source/images/cflag.asy
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-25 06:20 source/images/sageplot2d.sage
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-25 06:20 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx      357 b- defN 23-Jun-25 06:20 source/images/tikz.tex
+-rw-r--r--  2.0 unx     6092 b- defN 23-Jun-25 06:20 publication/publication.ptx
 34 files, 190104 bytes uncompressed, 169353 bytes compressed:  10.9%
```

### Comparing `pretext-1.6.1.dev20230624/pretext/templates/resources/devcontainer.json` & `pretext-1.6.1.dev20230625/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230624/pretext/templates/resources/hello.zip` & `pretext-1.6.1.dev20230625/pretext/templates/resources/hello.zip`

 * *Files 16% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 4657 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:21 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:20 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:20 source/
--rw-r--r--  2.0 unx     1217 b- defN 23-Jun-24 06:20 project.ptx
--rw-r--r--  2.0 unx       69 b- defN 23-Jun-24 06:20 README.md
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-24 06:21 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-24 06:21 codechat_config.yaml
--rw-r--r--  2.0 unx     2192 b- defN 23-Jun-24 06:21 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      156 b- defN 23-Jun-24 06:20 source/main.ptx
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-24 06:20 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 source/
+-rw-r--r--  2.0 unx     1217 b- defN 23-Jun-25 06:20 project.ptx
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-25 06:20 README.md
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-25 06:20 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-25 06:20 codechat_config.yaml
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-25 06:20 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-25 06:20 source/main.ptx
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-25 06:20 publication/publication.ptx
 10 files, 7820 bytes uncompressed, 3563 bytes compressed:  54.4%
```

### Comparing `pretext-1.6.1.dev20230624/pretext/templates/resources/project.ptx` & `pretext-1.6.1.dev20230625/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230624/pretext/templates/resources/slideshow.zip` & `pretext-1.6.1.dev20230625/pretext/templates/resources/slideshow.zip`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 8392 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:21 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:20 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:20 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-24 06:20 xsl/
--rw-r--r--  2.0 unx      784 b- defN 23-Jun-24 06:20 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-24 06:21 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-24 06:21 codechat_config.yaml
--rw-r--r--  2.0 unx     2192 b- defN 23-Jun-24 06:21 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      190 b- defN 23-Jun-24 06:20 xsl/slides.xsl
--rw-r--r--  2.0 unx    11200 b- defN 23-Jun-24 06:20 source/main.ptx
--rw-r--r--  2.0 unx     2097 b- defN 23-Jun-24 06:20 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-25 06:20 xsl/
+-rw-r--r--  2.0 unx      784 b- defN 23-Jun-25 06:20 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-25 06:20 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-25 06:20 codechat_config.yaml
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-25 06:20 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-25 06:20 xsl/slides.xsl
+-rw-r--r--  2.0 unx    11200 b- defN 23-Jun-25 06:20 source/main.ptx
+-rw-r--r--  2.0 unx     2097 b- defN 23-Jun-25 06:20 publication/publication.ptx
 11 files, 20407 bytes uncompressed, 7204 bytes compressed:  64.7%
```

### Comparing `pretext-1.6.1.dev20230624/pretext/utils.py` & `pretext-1.6.1.dev20230625/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230624/pyproject.toml` & `pretext-1.6.1.dev20230625/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # See https://python-poetry.org/docs/dependency-specification/ to get an understanding of
 # how poetry specifies dependencies.
 #
 # Project metadata
 # ----------------
 [tool.poetry]
 name = "pretext"
-version = "1.6.1.dev20230624"
+version = "1.6.1.dev20230625"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.6.1.dev20230624/PKG-INFO` & `pretext-1.6.1.dev20230625/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.6.1.dev20230624
+Version: 1.6.1.dev20230625
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

