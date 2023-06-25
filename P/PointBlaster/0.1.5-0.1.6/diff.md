# Comparing `tmp/PointBlaster-0.1.5.tar.gz` & `tmp/PointBlaster-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PointBlaster-0.1.5.tar", last modified: Sun Jun 25 07:11:06 2023, max compression
+gzip compressed data, was "PointBlaster-0.1.6.tar", last modified: Sun Jun 25 07:14:57 2023, max compression
```

## Comparing `PointBlaster-0.1.5.tar` & `PointBlaster-0.1.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:11:06.760446 PointBlaster-0.1.5/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 06:45:46.000000 PointBlaster-0.1.5/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       61 2023-06-25 06:30:58.000000 PointBlaster-0.1.5/MANIFEST.in
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-25 07:11:06.760327 PointBlaster-0.1.5/PKG-INFO
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:11:06.737680 PointBlaster-0.1.5/PointBlaster/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:10:09.000000 PointBlaster-0.1.5/PointBlaster/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    21412 2023-06-25 06:11:03.000000 PointBlaster-0.1.5/PointBlaster/PointBlaster.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      303 2023-06-25 07:10:20.000000 PointBlaster-0.1.5/PointBlaster/__init__.py
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:11:06.738508 PointBlaster-0.1.5/PointBlaster/db/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:06:04.000000 PointBlaster-0.1.5/PointBlaster/db/.DS_Store
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:11:06.738757 PointBlaster-0.1.5/PointBlaster/db/point_mutation/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    10244 2023-06-25 07:06:04.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/.DS_Store
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:11:06.747737 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:10:09.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2972 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/23S.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        4 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/RNA_genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)  4259822 2023-06-19 06:54:12.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     8705 2023-06-25 07:08:32.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     8657 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:54:12.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/campylobacter.length.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      149 2023-06-19 06:54:12.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/campylobacter.name
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4936 2023-06-19 06:54:12.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       14 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     5272 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2613 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2523 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1961 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      412 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/rpsL.fsa
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:11:06.755776 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1593 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/RNA_genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     3214 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/acrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2694 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/gyrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2469 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/gyrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2311 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/parC.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1940 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/parE.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     7137 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/phenotypes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      698 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/pmrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1106 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/pmrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     5030 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)  4318510 2023-06-19 06:54:12.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    16121 2023-06-25 07:08:53.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/salmonella.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    16025 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       72 2023-06-19 06:54:12.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/salmonella.length.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      296 2023-06-19 06:54:12.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/salmonella.name
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     7888 2023-06-19 06:54:12.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:11:06.738377 PointBlaster-0.1.5/PointBlaster.egg-info/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-25 07:11:06.000000 PointBlaster-0.1.5/PointBlaster.egg-info/PKG-INFO
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2422 2023-06-25 07:11:06.000000 PointBlaster-0.1.5/PointBlaster.egg-info/SOURCES.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2023-06-25 07:11:06.000000 PointBlaster-0.1.5/PointBlaster.egg-info/dependency_links.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       65 2023-06-25 07:11:06.000000 PointBlaster-0.1.5/PointBlaster.egg-info/entry_points.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       39 2023-06-25 07:11:06.000000 PointBlaster-0.1.5/PointBlaster.egg-info/requires.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       13 2023-06-25 07:11:06.000000 PointBlaster-0.1.5/PointBlaster.egg-info/top_level.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1611 2023-06-25 06:11:36.000000 PointBlaster-0.1.5/README.md
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:11:06.759516 PointBlaster-0.1.5/dist/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 06:45:51.000000 PointBlaster-0.1.5/dist/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)   248595 2023-06-25 06:46:08.000000 PointBlaster-0.1.5/dist/PointBlaster-0.1.4-py3-none-any.whl
--rw-r--r--   0 cuiqingpo   (501) staff       (20)   242824 2023-06-25 06:46:08.000000 PointBlaster-0.1.5/dist/PointBlaster-0.1.4.tar.gz
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       57 2023-06-25 05:58:37.000000 PointBlaster-0.1.5/requirements.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2023-06-25 07:11:06.760488 PointBlaster-0.1.5/setup.cfg
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2162 2023-06-25 06:43:25.000000 PointBlaster-0.1.5/setup.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:14:57.699455 PointBlaster-0.1.6/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:13:43.000000 PointBlaster-0.1.6/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       61 2023-06-25 06:30:58.000000 PointBlaster-0.1.6/MANIFEST.in
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-25 07:14:57.699328 PointBlaster-0.1.6/PKG-INFO
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:14:57.678265 PointBlaster-0.1.6/PointBlaster/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:10:09.000000 PointBlaster-0.1.6/PointBlaster/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    21412 2023-06-25 06:11:03.000000 PointBlaster-0.1.6/PointBlaster/PointBlaster.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      303 2023-06-25 07:13:53.000000 PointBlaster-0.1.6/PointBlaster/__init__.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:14:57.679004 PointBlaster-0.1.6/PointBlaster/db/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:06:04.000000 PointBlaster-0.1.6/PointBlaster/db/.DS_Store
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:14:57.679220 PointBlaster-0.1.6/PointBlaster/db/point_mutation/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    10244 2023-06-25 07:13:48.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/.DS_Store
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:14:57.687993 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:10:09.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2972 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/23S.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        4 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/RNA_genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)  4259822 2023-06-19 06:54:12.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     8705 2023-06-25 07:08:32.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     8657 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:54:12.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/campylobacter.length.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      149 2023-06-19 06:54:12.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/campylobacter.name
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4936 2023-06-19 06:54:12.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       14 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     5272 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2613 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2523 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1961 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      412 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/rpsL.fsa
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:14:57.694740 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1593 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/RNA_genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     3214 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/acrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2694 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/gyrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2469 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/gyrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2311 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/parC.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1940 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/parE.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     7137 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/phenotypes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      698 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/pmrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1106 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/pmrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     5026 2023-06-25 07:13:32.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)  4318510 2023-06-19 06:54:12.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    16121 2023-06-25 07:08:53.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/salmonella.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    16025 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       72 2023-06-19 06:54:12.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/salmonella.length.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      296 2023-06-19 06:54:12.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/salmonella.name
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     7888 2023-06-19 06:54:12.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:14:57.678899 PointBlaster-0.1.6/PointBlaster.egg-info/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-25 07:14:57.000000 PointBlaster-0.1.6/PointBlaster.egg-info/PKG-INFO
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2422 2023-06-25 07:14:57.000000 PointBlaster-0.1.6/PointBlaster.egg-info/SOURCES.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2023-06-25 07:14:57.000000 PointBlaster-0.1.6/PointBlaster.egg-info/dependency_links.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       65 2023-06-25 07:14:57.000000 PointBlaster-0.1.6/PointBlaster.egg-info/entry_points.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       39 2023-06-25 07:14:57.000000 PointBlaster-0.1.6/PointBlaster.egg-info/requires.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       13 2023-06-25 07:14:57.000000 PointBlaster-0.1.6/PointBlaster.egg-info/top_level.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1611 2023-06-25 06:11:36.000000 PointBlaster-0.1.6/README.md
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:14:57.698500 PointBlaster-0.1.6/dist/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 06:45:51.000000 PointBlaster-0.1.6/dist/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)   248595 2023-06-25 06:46:08.000000 PointBlaster-0.1.6/dist/PointBlaster-0.1.4-py3-none-any.whl
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)   242824 2023-06-25 06:46:08.000000 PointBlaster-0.1.6/dist/PointBlaster-0.1.4.tar.gz
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       57 2023-06-25 05:58:37.000000 PointBlaster-0.1.6/requirements.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2023-06-25 07:14:57.699495 PointBlaster-0.1.6/setup.cfg
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2162 2023-06-25 06:43:25.000000 PointBlaster-0.1.6/setup.py
```

### Comparing `PointBlaster-0.1.5/.DS_Store` & `PointBlaster-0.1.6/.DS_Store`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 00000610: 3030 d601 0203 0405 0607 0807 080b 085d  00.............]
 00000620: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
 00000630: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
 00000640: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
 00000650: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
 00000660: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
 00000670: 6465 6261 7208 0908 095f 1019 7b7b 3134  debar...._..{{14
-00000680: 3930 2c20 3637 347d 2c20 7b39 3230 2c20  90, 674}, {920, 
+00000680: 3930 2c20 3637 357d 2c20 7b39 3230 2c20  90, 675}, {920, 
 00000690: 3433 367d 7d09 0815 232f 3b52 5f6b 6c6d  436}}...#/;R_klm
 000006a0: 6e6f 8b00 0000 0000 0001 0100 0000 0000  no..............
 000006b0: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
 000006c0: 0000 8c00 0000 0c00 5000 6f00 6900 6e00  ........P.o.i.n.
 000006d0: 7400 4200 6c00 6100 7300 7400 6500 726c  t.B.l.a.s.t.e.rl
 000006e0: 6731 5363 6f6d 7000 0000 0000 0000 0000  g1Scomp.........
 000006f0: 0000 0c00 5000 6f00 6900 6e00 7400 4200  ....P.o.i.n.t.B.
```

### Comparing `PointBlaster-0.1.5/PKG-INFO` & `PointBlaster-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PointBlaster
-Version: 0.1.5
+Version: 0.1.6
 Summary: find point mutation in assembled genomes
 Home-page: https://github.com/hbucqp/PointBlaster
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,wgs,blastn,pointmutation
 Platform: any
```

### Comparing `PointBlaster-0.1.5/PointBlaster/.DS_Store` & `PointBlaster-0.1.6/PointBlaster/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/PointBlaster.py` & `PointBlaster-0.1.6/PointBlaster/PointBlaster.py`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/.DS_Store` & `PointBlaster-0.1.6/PointBlaster/db/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/.DS_Store` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/.DS_Store`

 * *Files 14% similar despite different names*

```diff
@@ -284,109 +284,109 @@
 000011b0: 7b31 3439 302c 2036 3735 7d2c 207b 3932  {1490, 675}, {92
 000011c0: 302c 2034 3336 7d7d 0908 1523 2f3b 525f  0, 436}}...#/;R_
 000011d0: 6b6c 6d6e 6f8b 0000 0000 0000 0101 0000  klmno...........
 000011e0: 0000 0000 000d 0000 0000 0000 0000 0000  ................
 000011f0: 0000 0000 008c 0000 000a 0073 0061 006c  ...........s.a.l
 00001200: 006d 006f 006e 0065 006c 006c 0061 6c73  .m.o.n.e.l.l.als
 00001210: 7643 626c 6f62 0000 033e 6270 6c69 7374  vCblob...>bplist
-00001220: 3030 da01 0203 0405 0607 0809 0a0b 0b0d  00..............
-00001230: 1856 5758 595a 5b5f 1010 7573 6552 656c  .VWXYZ[_..useRel
-00001240: 6174 6976 6544 6174 6573 5f10 0f73 686f  ativeDates_..sho
-00001250: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
-00001260: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
-00001270: 416c 6c53 697a 6573 5f10 0f73 6372 6f6c  AllSizes_..scrol
-00001280: 6c50 6f73 6974 696f 6e59 5874 6578 7453  lPositionYXtextS
-00001290: 697a 655f 100f 7363 726f 6c6c 506f 7369  ize_..scrollPosi
-000012a0: 7469 6f6e 585a 736f 7274 436f 6c75 6d6e  tionXZsortColumn
-000012b0: 5869 636f 6e53 697a 655f 1012 7669 6577  XiconSize_..view
-000012c0: 4f70 7469 6f6e 7356 6572 7369 6f6e 0909  OptionsVersion..
-000012d0: ae0e 171c 2125 2a2f 3439 3e43 484c 50d4  ....!%*/49>CHLP.
-000012e0: 0f10 1112 1314 0b0b 5a69 6465 6e74 6966  ........Zidentif
-000012f0: 6965 7255 7769 6474 6859 6173 6365 6e64  ierUwidthYascend
-00001300: 696e 6757 7669 7369 626c 6554 6e61 6d65  ingWvisibleTname
-00001310: 1101 5509 09d4 1210 110f 1819 181b 0810  ..U.............
-00001320: 2308 5875 6269 7175 6974 79d4 1210 110f  #.Xubiquity.....
-00001330: 0b1e 1820 0910 b508 5c64 6174 654d 6f64  ... ....\dateMod
-00001340: 6966 6965 64d4 1210 110f 181e 1824 0808  ified........$..
-00001350: 5b64 6174 6543 7265 6174 6564 d412 1011  [dateCreated....
-00001360: 0f0b 2718 2909 1061 0854 7369 7a65 d412  ..'.)..a.Tsize..
-00001370: 1011 0f0b 2c0b 2e09 1073 0954 6b69 6e64  ....,....s.Tkind
-00001380: d412 1011 0f18 310b 3308 1064 0955 6c61  ......1.3..d.Ula
-00001390: 6265 6cd4 1210 110f 1836 0b38 0810 4b09  bel......6.8..K.
-000013a0: 5776 6572 7369 6f6e d412 1011 0f18 3b0b  Wversion......;.
-000013b0: 3d08 1101 2c09 5863 6f6d 6d65 6e74 73d4  =...,.Xcomments.
-000013c0: 1210 110f 1840 1842 0810 c408 5e64 6174  .....@.B....^dat
-000013d0: 654c 6173 744f 7065 6e65 64d4 1210 110f  eLastOpened.....
-000013e0: 1845 1847 0810 c808 5a73 6861 7265 4f77  .E.G....ZshareOw
-000013f0: 6e65 72d4 1210 110f 1845 184b 0808 5f10  ner......E.K.._.
-00001400: 0f73 6861 7265 4c61 7374 4564 6974 6f72  .shareLastEditor
-00001410: d412 1011 0f18 1e18 4f08 0859 6461 7465  ........O..Ydate
-00001420: 4164 6465 64d4 0f10 1112 5152 1818 5f10  Added.....QR.._.
-00001430: 1069 6e76 6974 6174 696f 6e53 7461 7475  .invitationStatu
-00001440: 7310 d208 0808 2340 3b00 0000 0000 0023  s.....#@;......#
-00001450: 402a 0000 0000 0000 2300 0000 0000 0000  @*......#.......
-00001460: 0054 6b69 6e64 2340 3000 0000 0000 0014  .Tkind#@0.......
-00001470: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-00001480: 0008 001d 0030 0042 004a 005e 0070 0079  .....0.B.J.^.p.y
-00001490: 008b 0096 009f 00b4 00b5 00b6 00c5 00ce  ................
-000014a0: 00d9 00df 00e9 00f1 00f6 00f9 00fa 00fb  ................
-000014b0: 0104 0105 0107 0108 0111 011a 011b 011d  ................
-000014c0: 011e 012b 0134 0135 0136 0142 014b 014c  ...+.4.5.6.B.K.L
-000014d0: 014e 014f 0154 015d 015e 0160 0161 0166  .N.O.T.].^.`.a.f
-000014e0: 016f 0170 0172 0173 0179 0182 0183 0185  .o.p.r.s.y......
-000014f0: 0186 018e 0197 0198 019b 019c 01a5 01ae  ................
-00001500: 01af 01b1 01b2 01c1 01ca 01cb 01cd 01ce  ................
-00001510: 01d9 01e2 01e3 01e4 01f6 01ff 0200 0201  ................
-00001520: 020b 0214 0227 0229 022a 022b 022c 0235  .....'.).*.+.,.5
-00001530: 023e 0247 024c 0255 0000 0000 0000 0201  .>.G.L.U........
+00001220: 3030 da01 0203 0405 0607 0809 0a0b 0c0d  00..............
+00001230: 1856 5758 595a 0c5f 1012 7669 6577 4f70  .VWXYZ._..viewOp
+00001240: 7469 6f6e 7356 6572 7369 6f6e 5f10 0f73  tionsVersion_..s
+00001250: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
+00001260: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
+00001270: 7465 416c 6c53 697a 6573 5f10 0f73 6372  teAllSizes_..scr
+00001280: 6f6c 6c50 6f73 6974 696f 6e59 5874 6578  ollPositionYXtex
+00001290: 7453 697a 655f 100f 7363 726f 6c6c 506f  tSize_..scrollPo
+000012a0: 7369 7469 6f6e 585a 736f 7274 436f 6c75  sitionXZsortColu
+000012b0: 6d6e 5869 636f 6e53 697a 655f 1010 7573  mnXiconSize_..us
+000012c0: 6552 656c 6174 6976 6544 6174 6573 1400  eRelativeDates..
+000012d0: 0000 0000 0000 0000 0000 0000 0000 0109  ................
+000012e0: ae0e 171c 2125 2a2f 3439 3e43 484c 50d4  ....!%*/49>CHLP.
+000012f0: 0f10 1112 1314 0c0c 5a69 6465 6e74 6966  ........Zidentif
+00001300: 6965 7255 7769 6474 6859 6173 6365 6e64  ierUwidthYascend
+00001310: 696e 6757 7669 7369 626c 6554 6e61 6d65  ingWvisibleTname
+00001320: 1101 5509 09d4 1210 110f 1819 181b 0810  ..U.............
+00001330: 2308 5875 6269 7175 6974 79d4 1210 110f  #.Xubiquity.....
+00001340: 0c1e 1820 0910 b508 5c64 6174 654d 6f64  ... ....\dateMod
+00001350: 6966 6965 64d4 1210 110f 181e 1824 0808  ified........$..
+00001360: 5b64 6174 6543 7265 6174 6564 d412 1011  [dateCreated....
+00001370: 0f0c 2718 2909 1061 0854 7369 7a65 d412  ..'.)..a.Tsize..
+00001380: 1011 0f0c 2c0c 2e09 1073 0954 6b69 6e64  ....,....s.Tkind
+00001390: d412 1011 0f18 310c 3308 1064 0955 6c61  ......1.3..d.Ula
+000013a0: 6265 6cd4 1210 110f 1836 0c38 0810 4b09  bel......6.8..K.
+000013b0: 5776 6572 7369 6f6e d412 1011 0f18 3b0c  Wversion......;.
+000013c0: 3d08 1101 2c09 5863 6f6d 6d65 6e74 73d4  =...,.Xcomments.
+000013d0: 1210 110f 1840 1842 0810 c408 5e64 6174  .....@.B....^dat
+000013e0: 654c 6173 744f 7065 6e65 64d4 1210 110f  eLastOpened.....
+000013f0: 1845 1847 0810 c808 5a73 6861 7265 4f77  .E.G....ZshareOw
+00001400: 6e65 72d4 1210 110f 1845 184b 0808 5f10  ner......E.K.._.
+00001410: 0f73 6861 7265 4c61 7374 4564 6974 6f72  .shareLastEditor
+00001420: d412 1011 0f18 1e18 4f08 0859 6461 7465  ........O..Ydate
+00001430: 4164 6465 64d4 0f10 1112 5152 1818 5f10  Added.....QR.._.
+00001440: 1069 6e76 6974 6174 696f 6e53 7461 7475  .invitationStatu
+00001450: 7310 d208 0808 2340 4780 0000 0000 0023  s.....#@G......#
+00001460: 402a 0000 0000 0000 2300 0000 0000 0000  @*......#.......
+00001470: 0054 6b69 6e64 2340 3000 0000 0000 0009  .Tkind#@0.......
+00001480: 0008 001d 0032 0044 004c 0060 0072 007b  .....2.D.L.`.r.{
+00001490: 008d 0098 00a1 00b4 00c5 00c6 00d5 00de  ................
+000014a0: 00e9 00ef 00f9 0101 0106 0109 010a 010b  ................
+000014b0: 0114 0115 0117 0118 0121 012a 012b 012d  .........!.*.+.-
+000014c0: 012e 013b 0144 0145 0146 0152 015b 015c  ...;.D.E.F.R.[.\
+000014d0: 015e 015f 0164 016d 016e 0170 0171 0176  .^._.d.m.n.p.q.v
+000014e0: 017f 0180 0182 0183 0189 0192 0193 0195  ................
+000014f0: 0196 019e 01a7 01a8 01ab 01ac 01b5 01be  ................
+00001500: 01bf 01c1 01c2 01d1 01da 01db 01dd 01de  ................
+00001510: 01e9 01f2 01f3 01f4 0206 020f 0210 0211  ................
+00001520: 021b 0224 0237 0239 023a 023b 023c 0245  ...$.7.9.:.;.<.E
+00001530: 024e 0257 025c 0265 0000 0000 0000 0201  .N.W.\.e........
 00001540: 0000 0000 0000 005c 0000 0000 0000 0000  .......\........
 00001550: 0000 0000 0000 0266 0000 000a 0073 0061  .......f.....s.a
 00001560: 006c 006d 006f 006e 0065 006c 006c 0061  .l.m.o.n.e.l.l.a
 00001570: 6c73 7670 626c 6f62 0000 02b3 6270 6c69  lsvpblob....bpli
 00001580: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
-00001590: 0b0d 1f48 494a 4b4c 4d5f 1010 7573 6552  ...HIJKLM_..useR
-000015a0: 656c 6174 6976 6544 6174 6573 5f10 0f73  elativeDates_..s
-000015b0: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
-000015c0: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
-000015d0: 7465 416c 6c53 697a 6573 5f10 0f73 6372  teAllSizes_..scr
-000015e0: 6f6c 6c50 6f73 6974 696f 6e59 5874 6578  ollPositionYXtex
-000015f0: 7453 697a 655f 100f 7363 726f 6c6c 506f  tSize_..scrollPo
-00001600: 7369 7469 6f6e 585a 736f 7274 436f 6c75  sitionXZsortColu
-00001610: 6d6e 5869 636f 6e53 697a 655f 1012 7669  mnXiconSize_..vi
-00001620: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
-00001630: 0909 d90e 0f10 1112 1314 1516 1720 252a  ............. %*
-00001640: 2f34 383d 4258 636f 6d6d 656e 7473 556c  /48=BXcommentsUl
-00001650: 6162 656c 5776 6572 7369 6f6e 5b64 6174  abelWversion[dat
-00001660: 6543 7265 6174 6564 5473 697a 655c 6461  eCreatedTsize\da
-00001670: 7465 4d6f 6469 6669 6564 546b 696e 6454  teModifiedTkindT
-00001680: 6e61 6d65 5e64 6174 654c 6173 744f 7065  name^dateLastOpe
-00001690: 6e65 64d4 1819 1a1b 1c1d 0b1f 5569 6e64  ned.........Uind
-000016a0: 6578 5577 6964 7468 5961 7363 656e 6469  exUwidthYascendi
-000016b0: 6e67 5776 6973 6962 6c65 1007 1101 2c09  ngWvisible....,.
-000016c0: 08d4 1819 1a1b 2122 0b1f 1005 1064 0908  ......!".....d..
-000016d0: d418 191a 1b26 270b 1f10 0610 4b09 08d4  .....&'.....K...
-000016e0: 1819 1a1b 2b2c 1f1f 1002 10b5 0808 d418  ....+,..........
-000016f0: 191a 1b30 311f 0b10 0310 6108 09d4 1819  ...01.....a.....
-00001700: 1a1b 352c 1f0b 1001 0809 d418 191a 1b39  ..5,...........9
-00001710: 3a0b 0b10 0410 7309 09d4 1b19 1a18 0b3f  :.....s........?
-00001720: 0b41 0911 0155 0910 00d4 1819 1a1b 4344  .A...U........CD
-00001730: 1f1f 1008 10c4 0808 0823 403b 0000 0000  .........#@;....
-00001740: 0000 2340 2a00 0000 0000 0023 0000 0000  ..#@*......#....
-00001750: 0000 0000 546b 696e 6423 4030 0000 0000  ....Tkind#@0....
-00001760: 0000 1400 0000 0000 0000 0000 0000 0000  ................
-00001770: 0000 0100 0800 1d00 3000 4200 4a00 5e00  ........0.B.J.^.
-00001780: 7000 7900 8b00 9600 9f00 b400 b500 b600  p.y.............
-00001790: c900 d200 d800 e000 ec00 f100 fe01 0301  ................
-000017a0: 0801 1701 2001 2601 2c01 3601 3e01 4001  .... .&.,.6.>.@.
-000017b0: 4301 4401 4501 4e01 5001 5201 5301 5401  C.D.E.N.P.R.S.T.
-000017c0: 5d01 5f01 6101 6201 6301 6c01 6e01 7001  ]._.a.b.c.l.n.p.
-000017d0: 7101 7201 7b01 7d01 7f01 8001 8101 8a01  q.r.{.}.........
-000017e0: 8c01 8d01 8e01 9701 9901 9b01 9c01 9d01  ................
-000017f0: a601 a701 aa01 ab01 ad01 b601 b801 ba01  ................
-00001800: bb01 bc01 bd01 c601 cf01 d801 dd01 e600  ................
+00001590: 0c0d 1f48 494a 4b4c 0c5f 1012 7669 6577  ...HIJKL._..view
+000015a0: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
+000015b0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+000015c0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+000015d0: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
+000015e0: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
+000015f0: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
+00001600: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
+00001610: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
+00001620: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+00001630: 1400 0000 0000 0000 0000 0000 0000 0000  ................
+00001640: 0109 d90e 0f10 1112 1314 1516 1720 252a  ............. %*
+00001650: 2f34 383d 4258 636f 6d6d 656e 7473 556c  /48=BXcommentsUl
+00001660: 6162 656c 5776 6572 7369 6f6e 5b64 6174  abelWversion[dat
+00001670: 6543 7265 6174 6564 5473 697a 655c 6461  eCreatedTsize\da
+00001680: 7465 4d6f 6469 6669 6564 546b 696e 6454  teModifiedTkindT
+00001690: 6e61 6d65 5e64 6174 654c 6173 744f 7065  name^dateLastOpe
+000016a0: 6e65 64d4 1819 1a1b 1c1d 0c1f 5569 6e64  ned.........Uind
+000016b0: 6578 5577 6964 7468 5961 7363 656e 6469  exUwidthYascendi
+000016c0: 6e67 5776 6973 6962 6c65 1007 1101 2c09  ngWvisible....,.
+000016d0: 08d4 1819 1a1b 2122 0c1f 1005 1064 0908  ......!".....d..
+000016e0: d418 191a 1b26 270c 1f10 0610 4b09 08d4  .....&'.....K...
+000016f0: 1819 1a1b 2b2c 1f1f 1002 10b5 0808 d418  ....+,..........
+00001700: 191a 1b30 311f 0c10 0310 6108 09d4 1819  ...01.....a.....
+00001710: 1a1b 352c 1f0c 1001 0809 d418 191a 1b39  ..5,...........9
+00001720: 3a0c 0c10 0410 7309 09d4 1b19 1a18 0c3f  :.....s........?
+00001730: 0c41 0911 0155 0910 00d4 1819 1a1b 4344  .A...U........CD
+00001740: 1f1f 1008 10c4 0808 0823 4047 8000 0000  .........#@G....
+00001750: 0000 2340 2a00 0000 0000 0023 0000 0000  ..#@*......#....
+00001760: 0000 0000 546b 696e 6423 4030 0000 0000  ....Tkind#@0....
+00001770: 0000 0900 0800 1d00 3200 4400 4c00 6000  ........2.D.L.`.
+00001780: 7200 7b00 8d00 9800 a100 b400 c500 c600  r.{.............
+00001790: d900 e200 e800 f000 fc01 0101 0e01 1301  ................
+000017a0: 1801 2701 3001 3601 3c01 4601 4e01 5001  ..'.0.6.<.F.N.P.
+000017b0: 5301 5401 5501 5e01 6001 6201 6301 6401  S.T.U.^.`.b.c.d.
+000017c0: 6d01 6f01 7101 7201 7301 7c01 7e01 8001  m.o.q.r.s.|.~...
+000017d0: 8101 8201 8b01 8d01 8f01 9001 9101 9a01  ................
+000017e0: 9c01 9d01 9e01 a701 a901 ab01 ac01 ad01  ................
+000017f0: b601 b701 ba01 bb01 bd01 c601 c801 ca01  ................
+00001800: cb01 cc01 cd01 d601 df01 e801 ed01 f600  ................
 00001810: 0000 0000 0002 0100 0000 0000 0000 4e00  ..............N.
 00001820: 0000 0000 0000 0000 0000 0000 0001 f700  ................
 00001830: 0000 0a00 7300 6100 6c00 6d00 6f00 6e00  ....s.a.l.m.o.n.
 00001840: 6500 6c00 6c00 6176 5372 6e6c 6f6e 6700  e.l.l.avSrnlong.
 00001850: 0000 0100 0000 0000 0000 0000 0000 0000  ................
 00001860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -586,56 +586,56 @@
 00002490: 0100 0200 0000 0000 0100 0400 0000 0000  ................
 000024a0: 0100 0800 0000 0000 0100 1000 0000 0000  ................
 000024b0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
 000024c0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
 000024d0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
 000024e0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
 000024f0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
-00002500: 00af 01b1 01b2 01c1 01ca 01cb 01cd 01ce  ................
-00002510: 01d9 01e2 01e3 01e4 01f6 01ff 0200 0201  ................
-00002520: 020b 0214 0227 0229 022a 022b 022c 0235  .....'.).*.+.,.5
-00002530: 023e 0247 024c 0255 0000 0000 0000 0201  .>.G.L.U........
+00002500: 00bf 01c1 01c2 01d1 01da 01db 01dd 01de  ................
+00002510: 01e9 01f2 01f3 01f4 0206 020f 0210 0211  ................
+00002520: 021b 0224 0237 0239 023a 023b 023c 0245  ...$.7.9.:.;.<.E
+00002530: 024e 0257 025c 0265 0000 0000 0000 0201  .N.W.\.e........
 00002540: 0000 0000 0000 005c 0000 0000 0000 0000  .......\........
 00002550: 0000 0000 0000 0266 0000 000a 0073 0061  .......f.....s.a
 00002560: 006c 006d 006f 006e 0065 006c 006c 0061  .l.m.o.n.e.l.l.a
 00002570: 6c73 7670 626c 6f62 0000 02b3 6270 6c69  lsvpblob....bpli
 00002580: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
-00002590: 0b0d 1f48 494a 4b4c 4d5f 1010 7573 6552  ...HIJKLM_..useR
-000025a0: 656c 6174 6976 6544 6174 6573 5f10 0f73  elativeDates_..s
-000025b0: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
-000025c0: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
-000025d0: 7465 416c 6c53 697a 6573 5f10 0f73 6372  teAllSizes_..scr
-000025e0: 6f6c 6c50 6f73 6974 696f 6e59 5874 6578  ollPositionYXtex
-000025f0: 7453 697a 655f 100f 7363 726f 6c6c 506f  tSize_..scrollPo
-00002600: 7369 7469 6f6e 585a 736f 7274 436f 6c75  sitionXZsortColu
-00002610: 6d6e 5869 636f 6e53 697a 655f 1012 7669  mnXiconSize_..vi
-00002620: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
-00002630: 0909 d90e 0f10 1112 1314 1516 1720 252a  ............. %*
-00002640: 2f34 383d 4258 636f 6d6d 656e 7473 556c  /48=BXcommentsUl
-00002650: 6162 656c 5776 6572 7369 6f6e 5b64 6174  abelWversion[dat
-00002660: 6543 7265 6174 6564 5473 697a 655c 6461  eCreatedTsize\da
-00002670: 7465 4d6f 6469 6669 6564 546b 696e 6454  teModifiedTkindT
-00002680: 6e61 6d65 5e64 6174 654c 6173 744f 7065  name^dateLastOpe
-00002690: 6e65 64d4 1819 1a1b 1c1d 0b1f 5569 6e64  ned.........Uind
-000026a0: 6578 5577 6964 7468 5961 7363 656e 6469  exUwidthYascendi
-000026b0: 6e67 5776 6973 6962 6c65 1007 1101 2c09  ngWvisible....,.
-000026c0: 08d4 1819 1a1b 2122 0b1f 1005 1064 0908  ......!".....d..
-000026d0: d418 191a 1b26 270b 1f10 0610 4b09 08d4  .....&'.....K...
-000026e0: 1819 1a1b 2b2c 1f1f 1002 10b5 0808 d418  ....+,..........
-000026f0: 191a 1b30 311f 0b10 0310 6108 09d4 1819  ...01.....a.....
-00002700: 1a1b 352c 1f0b 1001 0809 d418 191a 1b39  ..5,...........9
-00002710: 3a0b 0b10 0410 7309 09d4 1b19 1a18 0b3f  :.....s........?
-00002720: 0b41 0911 0155 0910 00d4 1819 1a1b 4344  .A...U........CD
-00002730: 1f1f 1008 10c4 0808 0823 403b 0000 0000  .........#@;....
-00002740: 0000 2340 2a00 0000 0000 0023 0000 0000  ..#@*......#....
-00002750: 0000 0000 546b 696e 6423 4030 0000 0000  ....Tkind#@0....
-00002760: 0000 1400 0000 0000 0000 0000 0000 0000  ................
-00002770: 0000 0100 0800 1d00 3000 4200 4a00 5e00  ........0.B.J.^.
-00002780: 7000 7900 8b00 9600 9f00 b400 b500 b600  p.y.............
-00002790: c900 d200 d800 e000 ec00 f100 fe01 0301  ................
-000027a0: 0801 1701 2001 2601 2c01 3601 3e01 4001  .... .&.,.6.>.@.
-000027b0: 4301 4401 4501 4e01 5001 5201 5301 5401  C.D.E.N.P.R.S.T.
-000027c0: 5d01 5f01 6101 6201 6301 6c01 6e01 7001  ]._.a.b.c.l.n.p.
-000027d0: 7101 7201 7b01 7d01 7f01 8001 8101 8a01  q.r.{.}.........
-000027e0: 8c01 8d01 8e01 9701 9901 9b01 9c01 9d01  ................
-000027f0: a601 a701 aa01 ab01 ad01 b601 b801 ba01  ................
-00002800: bb01 bc01                                ....
+00002590: 0c0d 1f48 494a 4b4c 0c5f 1012 7669 6577  ...HIJKL._..view
+000025a0: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
+000025b0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+000025c0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+000025d0: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
+000025e0: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
+000025f0: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
+00002600: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
+00002610: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
+00002620: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+00002630: 1400 0000 0000 0000 0000 0000 0000 0000  ................
+00002640: 0109 d90e 0f10 1112 1314 1516 1720 252a  ............. %*
+00002650: 2f34 383d 4258 636f 6d6d 656e 7473 556c  /48=BXcommentsUl
+00002660: 6162 656c 5776 6572 7369 6f6e 5b64 6174  abelWversion[dat
+00002670: 6543 7265 6174 6564 5473 697a 655c 6461  eCreatedTsize\da
+00002680: 7465 4d6f 6469 6669 6564 546b 696e 6454  teModifiedTkindT
+00002690: 6e61 6d65 5e64 6174 654c 6173 744f 7065  name^dateLastOpe
+000026a0: 6e65 64d4 1819 1a1b 1c1d 0c1f 5569 6e64  ned.........Uind
+000026b0: 6578 5577 6964 7468 5961 7363 656e 6469  exUwidthYascendi
+000026c0: 6e67 5776 6973 6962 6c65 1007 1101 2c09  ngWvisible....,.
+000026d0: 08d4 1819 1a1b 2122 0c1f 1005 1064 0908  ......!".....d..
+000026e0: d418 191a 1b26 270c 1f10 0610 4b09 08d4  .....&'.....K...
+000026f0: 1819 1a1b 2b2c 1f1f 1002 10b5 0808 d418  ....+,..........
+00002700: 191a 1b30 311f 0c10 0310 6108 09d4 1819  ...01.....a.....
+00002710: 1a1b 352c 1f0c 1001 0809 d418 191a 1b39  ..5,...........9
+00002720: 3a0c 0c10 0410 7309 09d4 1b19 1a18 0c3f  :.....s........?
+00002730: 0c41 0911 0155 0910 00d4 1819 1a1b 4344  .A...U........CD
+00002740: 1f1f 1008 10c4 0808 0823 4047 8000 0000  .........#@G....
+00002750: 0000 2340 2a00 0000 0000 0023 0000 0000  ..#@*......#....
+00002760: 0000 0000 546b 696e 6423 4030 0000 0000  ....Tkind#@0....
+00002770: 0000 0900 0800 1d00 3200 4400 4c00 6000  ........2.D.L.`.
+00002780: 7200 7b00 8d00 9800 a100 b400 c500 c600  r.{.............
+00002790: d900 e200 e800 f000 fc01 0101 0e01 1301  ................
+000027a0: 1801 2701 3001 3601 3c01 4601 4e01 5001  ..'.0.6.<.F.N.P.
+000027b0: 5301 5401 5501 5e01 6001 6201 6301 6401  S.T.U.^.`.b.c.d.
+000027c0: 6d01 6f01 7101 7201 7301 7c01 7e01 8001  m.o.q.r.s.|.~...
+000027d0: 8101 8201 8b01 8d01 8f01 9001 9101 9a01  ................
+000027e0: 9c01 9d01 9e01 a701 a901 ab01 ac01 ad01  ................
+000027f0: b601 b701 ba01 bb01 bd01 c601 c801 ca01  ................
+00002800: cb01 cc01                                ....
```

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/.DS_Store` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/23S.fsa` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/23S.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/acrB.fsa` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/acrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/gyrA.fsa` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/gyrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/gyrB.fsa` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/gyrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/parC.fsa` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/parC.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/parE.fsa` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/parE.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/phenotypes.txt` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/phenotypes.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/pmrA.fsa` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/pmrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/pmrB.fsa` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/pmrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt`

 * *Files 2% similar despite different names*

```diff
@@ -50,9 +50,9 @@
 parE	parE	454	GAA	E	G	Nalidixic acid,Ciprofloxacin	15388468	Target modification		gyrA_S83Y.F.A;gyrA_D87N.G.Y.K
 parE	parE	458	TCG	S	P	Nalidixic acid,Ciprofloxacin	14576119	Target modification		gyrA_S83Y.F.A;gyrA_D87N.G.Y.K
 parE	parE	462	CAT	H	Y	Nalidixic acid,Ciprofloxacin	19104017	Target modification		gyrA_S83Y.F.A;gyrA_D87N.G.Y.K
 parE	parE	462	CAT	H	Y	Nalidixic acid,Ciprofloxacin	15388468	Target modification		gyrA_S83Y.F.A;gyrA_D87N.G.Y.K
 parE	parE	499	GCT	A	T	Nalidixic acid,Ciprofloxacin	15388468	Target modification		gyrA_S83Y.F.A;gyrA_D87N.G.Y.K
 parE	parE	514	GTG	V	G	Nalidixic acid,Ciprofloxacin	15388468	Target modification		gyrA_S83Y.F.A;gyrA_D87N.G.Y.K
 acrB	acrB	717	CGG	R	Q,L	Azithromycin	 31730615	Target modification		
-16S_rrsD	16S	1065	C	C	T	Spectinomycin	12402084	Target modification		
-16S_rrsD	16S	1192	C	C	T	Spectinomycin	12402084	Target modification		
+16S-rrsD	16S	1065	C	C	T	Spectinomycin	12402084	Target modification
+16S-rrsD	16S	1192	C	C	T	Spectinomycin	12402084	Target modification
```

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/salmonella.fsa` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/salmonella.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b` & `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/PointBlaster.egg-info/PKG-INFO` & `PointBlaster-0.1.6/PointBlaster.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PointBlaster
-Version: 0.1.5
+Version: 0.1.6
 Summary: find point mutation in assembled genomes
 Home-page: https://github.com/hbucqp/PointBlaster
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,wgs,blastn,pointmutation
 Platform: any
```

### Comparing `PointBlaster-0.1.5/PointBlaster.egg-info/SOURCES.txt` & `PointBlaster-0.1.6/PointBlaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/README.md` & `PointBlaster-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/dist/.DS_Store` & `PointBlaster-0.1.6/dist/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/dist/PointBlaster-0.1.4-py3-none-any.whl` & `PointBlaster-0.1.6/dist/PointBlaster-0.1.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/dist/PointBlaster-0.1.4.tar.gz` & `PointBlaster-0.1.6/dist/PointBlaster-0.1.4.tar.gz`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.5/setup.py` & `PointBlaster-0.1.6/setup.py`

 * *Files identical despite different names*

