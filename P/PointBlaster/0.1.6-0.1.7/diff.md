# Comparing `tmp/PointBlaster-0.1.6.tar.gz` & `tmp/PointBlaster-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PointBlaster-0.1.6.tar", last modified: Sun Jun 25 07:14:57 2023, max compression
+gzip compressed data, was "PointBlaster-0.1.7.tar", last modified: Sun Jun 25 07:26:57 2023, max compression
```

## Comparing `PointBlaster-0.1.6.tar` & `PointBlaster-0.1.7.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:14:57.699455 PointBlaster-0.1.6/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:13:43.000000 PointBlaster-0.1.6/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       61 2023-06-25 06:30:58.000000 PointBlaster-0.1.6/MANIFEST.in
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-25 07:14:57.699328 PointBlaster-0.1.6/PKG-INFO
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:14:57.678265 PointBlaster-0.1.6/PointBlaster/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:10:09.000000 PointBlaster-0.1.6/PointBlaster/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    21412 2023-06-25 06:11:03.000000 PointBlaster-0.1.6/PointBlaster/PointBlaster.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      303 2023-06-25 07:13:53.000000 PointBlaster-0.1.6/PointBlaster/__init__.py
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:14:57.679004 PointBlaster-0.1.6/PointBlaster/db/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:06:04.000000 PointBlaster-0.1.6/PointBlaster/db/.DS_Store
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:14:57.679220 PointBlaster-0.1.6/PointBlaster/db/point_mutation/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    10244 2023-06-25 07:13:48.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/.DS_Store
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:14:57.687993 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:10:09.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2972 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/23S.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        4 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/RNA_genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)  4259822 2023-06-19 06:54:12.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     8705 2023-06-25 07:08:32.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     8657 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:54:12.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/campylobacter.length.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      149 2023-06-19 06:54:12.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/campylobacter.name
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4936 2023-06-19 06:54:12.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       14 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     5272 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2613 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2523 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1961 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      412 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/rpsL.fsa
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:14:57.694740 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1593 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/RNA_genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     3214 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/acrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2694 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/gyrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2469 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/gyrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2311 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/parC.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1940 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/parE.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     7137 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/phenotypes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      698 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/pmrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1106 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/pmrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     5026 2023-06-25 07:13:32.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)  4318510 2023-06-19 06:54:12.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    16121 2023-06-25 07:08:53.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/salmonella.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    16025 2023-06-19 06:40:55.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       72 2023-06-19 06:54:12.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/salmonella.length.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      296 2023-06-19 06:54:12.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/salmonella.name
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     7888 2023-06-19 06:54:12.000000 PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:14:57.678899 PointBlaster-0.1.6/PointBlaster.egg-info/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-25 07:14:57.000000 PointBlaster-0.1.6/PointBlaster.egg-info/PKG-INFO
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2422 2023-06-25 07:14:57.000000 PointBlaster-0.1.6/PointBlaster.egg-info/SOURCES.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2023-06-25 07:14:57.000000 PointBlaster-0.1.6/PointBlaster.egg-info/dependency_links.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       65 2023-06-25 07:14:57.000000 PointBlaster-0.1.6/PointBlaster.egg-info/entry_points.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       39 2023-06-25 07:14:57.000000 PointBlaster-0.1.6/PointBlaster.egg-info/requires.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       13 2023-06-25 07:14:57.000000 PointBlaster-0.1.6/PointBlaster.egg-info/top_level.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1611 2023-06-25 06:11:36.000000 PointBlaster-0.1.6/README.md
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:14:57.698500 PointBlaster-0.1.6/dist/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 06:45:51.000000 PointBlaster-0.1.6/dist/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)   248595 2023-06-25 06:46:08.000000 PointBlaster-0.1.6/dist/PointBlaster-0.1.4-py3-none-any.whl
--rw-r--r--   0 cuiqingpo   (501) staff       (20)   242824 2023-06-25 06:46:08.000000 PointBlaster-0.1.6/dist/PointBlaster-0.1.4.tar.gz
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       57 2023-06-25 05:58:37.000000 PointBlaster-0.1.6/requirements.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2023-06-25 07:14:57.699495 PointBlaster-0.1.6/setup.cfg
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2162 2023-06-25 06:43:25.000000 PointBlaster-0.1.6/setup.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:26:57.485663 PointBlaster-0.1.7/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:13:43.000000 PointBlaster-0.1.7/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       61 2023-06-25 06:30:58.000000 PointBlaster-0.1.7/MANIFEST.in
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-25 07:26:57.485514 PointBlaster-0.1.7/PKG-INFO
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:26:57.463519 PointBlaster-0.1.7/PointBlaster/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:10:09.000000 PointBlaster-0.1.7/PointBlaster/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    21434 2023-06-25 07:26:38.000000 PointBlaster-0.1.7/PointBlaster/PointBlaster.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      303 2023-06-25 07:16:59.000000 PointBlaster-0.1.7/PointBlaster/__init__.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:26:57.464296 PointBlaster-0.1.7/PointBlaster/db/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:06:04.000000 PointBlaster-0.1.7/PointBlaster/db/.DS_Store
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:26:57.464549 PointBlaster-0.1.7/PointBlaster/db/point_mutation/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    10244 2023-06-25 07:13:48.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/.DS_Store
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:26:57.473434 PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:10:09.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2972 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/23S.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        4 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/RNA_genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)  4259822 2023-06-19 06:54:12.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     8705 2023-06-25 07:08:32.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     8657 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:54:12.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/campylobacter.length.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      149 2023-06-19 06:54:12.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/campylobacter.name
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4936 2023-06-19 06:54:12.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       14 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     5272 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2613 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2523 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1961 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      412 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/rpsL.fsa
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:26:57.480656 PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1593 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/RNA_genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     3214 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/acrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2694 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/gyrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2469 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/gyrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2311 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/parC.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1940 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/parE.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     7137 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/phenotypes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      698 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/pmrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1106 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/pmrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     5026 2023-06-25 07:13:32.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)  4318510 2023-06-19 06:54:12.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    16121 2023-06-25 07:08:53.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/salmonella.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    16025 2023-06-19 06:40:55.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       72 2023-06-19 06:54:12.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/salmonella.length.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      296 2023-06-19 06:54:12.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/salmonella.name
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     7888 2023-06-19 06:54:12.000000 PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:26:57.464188 PointBlaster-0.1.7/PointBlaster.egg-info/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-25 07:26:57.000000 PointBlaster-0.1.7/PointBlaster.egg-info/PKG-INFO
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2422 2023-06-25 07:26:57.000000 PointBlaster-0.1.7/PointBlaster.egg-info/SOURCES.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2023-06-25 07:26:57.000000 PointBlaster-0.1.7/PointBlaster.egg-info/dependency_links.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       65 2023-06-25 07:26:57.000000 PointBlaster-0.1.7/PointBlaster.egg-info/entry_points.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       39 2023-06-25 07:26:57.000000 PointBlaster-0.1.7/PointBlaster.egg-info/requires.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       13 2023-06-25 07:26:57.000000 PointBlaster-0.1.7/PointBlaster.egg-info/top_level.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1611 2023-06-25 06:11:36.000000 PointBlaster-0.1.7/README.md
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:26:57.484633 PointBlaster-0.1.7/dist/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 06:45:51.000000 PointBlaster-0.1.7/dist/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)   248595 2023-06-25 06:46:08.000000 PointBlaster-0.1.7/dist/PointBlaster-0.1.4-py3-none-any.whl
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)   242824 2023-06-25 06:46:08.000000 PointBlaster-0.1.7/dist/PointBlaster-0.1.4.tar.gz
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       57 2023-06-25 05:58:37.000000 PointBlaster-0.1.7/requirements.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2023-06-25 07:26:57.485722 PointBlaster-0.1.7/setup.cfg
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2162 2023-06-25 06:43:25.000000 PointBlaster-0.1.7/setup.py
```

### Comparing `PointBlaster-0.1.6/.DS_Store` & `PointBlaster-0.1.7/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PKG-INFO` & `PointBlaster-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PointBlaster
-Version: 0.1.6
+Version: 0.1.7
 Summary: find point mutation in assembled genomes
 Home-page: https://github.com/hbucqp/PointBlaster
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,wgs,blastn,pointmutation
 Platform: any
```

### Comparing `PointBlaster-0.1.6/PointBlaster/.DS_Store` & `PointBlaster-0.1.7/PointBlaster/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/PointBlaster.py` & `PointBlaster-0.1.7/PointBlaster/PointBlaster.py`

 * *Files 1% similar despite different names*

```diff
@@ -549,19 +549,19 @@
                         df, result_dict = Blaster(file_path, blastdb,
                                                   output_path, threads, minid, mincov).biopython_blast()
                         db_mutations = get_db_mutations(db_mutations_path)
                         genes, RNA_genes = get_gene_list(args.s)
 
                         gene_list_result = get_align_seq(result_dict)
 
-                        test = find_mutations(
+                        mutation_result = find_mutations(
                             gene_list_result, genes)
                         # print(test)
                         # print(gene_list_result)
-                        f.write(filter_result(test, db_mutations, genes))
+                        f.write(filter_result(mutation_result, db_mutations, genes))
 
                         print(
                             f"Finishing process {file}: writing results to " + str(outfile))
             f.close()
 
 
 if __name__ == '__main__':
```

### Comparing `PointBlaster-0.1.6/PointBlaster/db/.DS_Store` & `PointBlaster-0.1.7/PointBlaster/db/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/.DS_Store` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/.DS_Store` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/23S.fsa` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/23S.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/acrB.fsa` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/acrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/gyrA.fsa` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/gyrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/gyrB.fsa` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/gyrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/parC.fsa` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/parC.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/parE.fsa` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/parE.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/phenotypes.txt` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/phenotypes.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/pmrA.fsa` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/pmrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/pmrB.fsa` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/pmrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/salmonella.fsa` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/salmonella.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b` & `PointBlaster-0.1.7/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/PointBlaster.egg-info/PKG-INFO` & `PointBlaster-0.1.7/PointBlaster.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PointBlaster
-Version: 0.1.6
+Version: 0.1.7
 Summary: find point mutation in assembled genomes
 Home-page: https://github.com/hbucqp/PointBlaster
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,wgs,blastn,pointmutation
 Platform: any
```

### Comparing `PointBlaster-0.1.6/PointBlaster.egg-info/SOURCES.txt` & `PointBlaster-0.1.7/PointBlaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/README.md` & `PointBlaster-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/dist/.DS_Store` & `PointBlaster-0.1.7/dist/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/dist/PointBlaster-0.1.4-py3-none-any.whl` & `PointBlaster-0.1.7/dist/PointBlaster-0.1.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/dist/PointBlaster-0.1.4.tar.gz` & `PointBlaster-0.1.7/dist/PointBlaster-0.1.4.tar.gz`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.6/setup.py` & `PointBlaster-0.1.7/setup.py`

 * *Files identical despite different names*

