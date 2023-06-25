# Comparing `tmp/PointBlaster-0.1.4.tar.gz` & `tmp/PointBlaster-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PointBlaster-0.1.4.tar", last modified: Sun Jun 25 06:46:08 2023, max compression
+gzip compressed data, was "PointBlaster-0.1.5.tar", last modified: Sun Jun 25 07:11:06 2023, max compression
```

## Comparing `PointBlaster-0.1.4.tar` & `PointBlaster-0.1.5.tar`

### file list

```diff
@@ -1,55 +1,62 @@
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:46:08.429609 PointBlaster-0.1.4/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 06:45:46.000000 PointBlaster-0.1.4/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       61 2023-06-25 06:30:58.000000 PointBlaster-0.1.4/MANIFEST.in
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-25 06:46:08.429479 PointBlaster-0.1.4/PKG-INFO
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:46:08.410458 PointBlaster-0.1.4/PointBlaster/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 06:38:55.000000 PointBlaster-0.1.4/PointBlaster/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    21412 2023-06-25 06:11:03.000000 PointBlaster-0.1.4/PointBlaster/PointBlaster.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      303 2023-06-25 06:43:10.000000 PointBlaster-0.1.4/PointBlaster/__init__.py
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:46:08.411278 PointBlaster-0.1.4/PointBlaster/db/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 06:42:07.000000 PointBlaster-0.1.4/PointBlaster/db/.DS_Store
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:46:08.411390 PointBlaster-0.1.4/PointBlaster/db/point_mutation/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     8196 2023-06-25 05:56:06.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/.DS_Store
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:46:08.419010 PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2972 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/23S.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        4 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/RNA_genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)  4259822 2023-06-19 06:54:12.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     8657 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:54:12.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/campylobacter.length.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      149 2023-06-19 06:54:12.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/campylobacter.name
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4936 2023-06-19 06:54:12.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       14 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     5272 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2613 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2523 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1961 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      412 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/rpsL.fsa
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:46:08.427863 PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1593 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/RNA_genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     3214 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/acrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2694 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/gyrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2469 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/gyrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2311 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/parC.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1940 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/parE.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     7137 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/phenotypes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      698 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/pmrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1106 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/pmrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     5030 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)  4318510 2023-06-19 06:54:12.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    16025 2023-06-19 06:40:55.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/salmonella.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       72 2023-06-19 06:54:12.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/salmonella.length.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      296 2023-06-19 06:54:12.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/salmonella.name
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     7888 2023-06-19 06:54:12.000000 PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:46:08.411152 PointBlaster-0.1.4/PointBlaster.egg-info/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-25 06:46:08.000000 PointBlaster-0.1.4/PointBlaster.egg-info/PKG-INFO
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2142 2023-06-25 06:46:08.000000 PointBlaster-0.1.4/PointBlaster.egg-info/SOURCES.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2023-06-25 06:46:08.000000 PointBlaster-0.1.4/PointBlaster.egg-info/dependency_links.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       65 2023-06-25 06:46:08.000000 PointBlaster-0.1.4/PointBlaster.egg-info/entry_points.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       39 2023-06-25 06:46:08.000000 PointBlaster-0.1.4/PointBlaster.egg-info/requires.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       13 2023-06-25 06:46:08.000000 PointBlaster-0.1.4/PointBlaster.egg-info/top_level.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1611 2023-06-25 06:11:36.000000 PointBlaster-0.1.4/README.md
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       57 2023-06-25 05:58:37.000000 PointBlaster-0.1.4/requirements.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2023-06-25 06:46:08.429655 PointBlaster-0.1.4/setup.cfg
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2162 2023-06-25 06:43:25.000000 PointBlaster-0.1.4/setup.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:11:06.760446 PointBlaster-0.1.5/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 06:45:46.000000 PointBlaster-0.1.5/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       61 2023-06-25 06:30:58.000000 PointBlaster-0.1.5/MANIFEST.in
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-25 07:11:06.760327 PointBlaster-0.1.5/PKG-INFO
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:11:06.737680 PointBlaster-0.1.5/PointBlaster/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:10:09.000000 PointBlaster-0.1.5/PointBlaster/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    21412 2023-06-25 06:11:03.000000 PointBlaster-0.1.5/PointBlaster/PointBlaster.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      303 2023-06-25 07:10:20.000000 PointBlaster-0.1.5/PointBlaster/__init__.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:11:06.738508 PointBlaster-0.1.5/PointBlaster/db/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:06:04.000000 PointBlaster-0.1.5/PointBlaster/db/.DS_Store
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:11:06.738757 PointBlaster-0.1.5/PointBlaster/db/point_mutation/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    10244 2023-06-25 07:06:04.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/.DS_Store
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:11:06.747737 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 07:10:09.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2972 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/23S.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        4 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/RNA_genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)  4259822 2023-06-19 06:54:12.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     8705 2023-06-25 07:08:32.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     8657 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:54:12.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/campylobacter.length.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      149 2023-06-19 06:54:12.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/campylobacter.name
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4936 2023-06-19 06:54:12.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       14 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     5272 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2613 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2523 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1961 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      412 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/rpsL.fsa
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:11:06.755776 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1593 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/RNA_genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     3214 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/acrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2694 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/gyrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2469 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/gyrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2311 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/parC.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1940 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/parE.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     7137 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/phenotypes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      698 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/pmrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1106 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/pmrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     5030 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)  4318510 2023-06-19 06:54:12.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    16121 2023-06-25 07:08:53.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/salmonella.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    16025 2023-06-19 06:40:55.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       72 2023-06-19 06:54:12.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/salmonella.length.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      296 2023-06-19 06:54:12.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/salmonella.name
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     7888 2023-06-19 06:54:12.000000 PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:11:06.738377 PointBlaster-0.1.5/PointBlaster.egg-info/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-25 07:11:06.000000 PointBlaster-0.1.5/PointBlaster.egg-info/PKG-INFO
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2422 2023-06-25 07:11:06.000000 PointBlaster-0.1.5/PointBlaster.egg-info/SOURCES.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2023-06-25 07:11:06.000000 PointBlaster-0.1.5/PointBlaster.egg-info/dependency_links.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       65 2023-06-25 07:11:06.000000 PointBlaster-0.1.5/PointBlaster.egg-info/entry_points.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       39 2023-06-25 07:11:06.000000 PointBlaster-0.1.5/PointBlaster.egg-info/requires.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       13 2023-06-25 07:11:06.000000 PointBlaster-0.1.5/PointBlaster.egg-info/top_level.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1611 2023-06-25 06:11:36.000000 PointBlaster-0.1.5/README.md
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 07:11:06.759516 PointBlaster-0.1.5/dist/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 06:45:51.000000 PointBlaster-0.1.5/dist/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)   248595 2023-06-25 06:46:08.000000 PointBlaster-0.1.5/dist/PointBlaster-0.1.4-py3-none-any.whl
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)   242824 2023-06-25 06:46:08.000000 PointBlaster-0.1.5/dist/PointBlaster-0.1.4.tar.gz
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       57 2023-06-25 05:58:37.000000 PointBlaster-0.1.5/requirements.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2023-06-25 07:11:06.760488 PointBlaster-0.1.5/setup.cfg
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2162 2023-06-25 06:43:25.000000 PointBlaster-0.1.5/setup.py
```

### Comparing `PointBlaster-0.1.4/.DS_Store` & `PointBlaster-0.1.5/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PKG-INFO` & `PointBlaster-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PointBlaster
-Version: 0.1.4
+Version: 0.1.5
 Summary: find point mutation in assembled genomes
 Home-page: https://github.com/hbucqp/PointBlaster
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,wgs,blastn,pointmutation
 Platform: any
```

### Comparing `PointBlaster-0.1.4/PointBlaster/.DS_Store` & `PointBlaster-0.1.5/PointBlaster/.DS_Store`

 * *Files 21% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 00000220: 6270 6c69 7374 3030 d601 0203 0405 0607  bplist00........
 00000230: 0807 080b 085d 5368 6f77 5374 6174 7573  .....]ShowStatus
 00000240: 4261 725b 5368 6f77 546f 6f6c 6261 725b  Bar[ShowToolbar[
 00000250: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
 00000260: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
 00000270: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
 00000280: 5368 6f77 5369 6465 6261 7208 0908 095f  ShowSidebar...._
-00000290: 1019 7b7b 3134 3931 2c20 3637 347d 2c20  ..{{1491, 674}, 
+00000290: 1019 7b7b 3134 3930 2c20 3637 357d 2c20  ..{{1490, 675}, 
 000002a0: 7b39 3230 2c20 3433 367d 7d09 0815 232f  {920, 436}}...#/
 000002b0: 3b52 5f6b 6c6d 6e6f 8b00 0000 0000 0001  ;R_klmno........
 000002c0: 0100 0000 0000 0000 0d00 0000 0000 0000  ................
 000002d0: 0000 0000 0000 0000 8c00 0000 0200 6400  ..............d.
 000002e0: 626c 6731 5363 6f6d 7000 0000 0000 0000  blg1Scomp.......
 000002f0: 0000 0000 0200 6400 626d 6f44 4462 6c6f  ......d.bmoDDblo
 00000300: 6200 0000 0810 3730 2d07 24c5 4100 0000  b.....70-.$.A...
```

### Comparing `PointBlaster-0.1.4/PointBlaster/PointBlaster.py` & `PointBlaster-0.1.5/PointBlaster/PointBlaster.py`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/.DS_Store` & `PointBlaster-0.1.5/PointBlaster/db/.DS_Store`

 * *Files 15% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 00000230: 626c 6f62 0000 00b9 6270 6c69 7374 3030  blob....bplist00
 00000240: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
 00000250: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00000260: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
 00000270: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
 00000280: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
 00000290: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-000002a0: 6261 7208 0908 095f 1019 7b7b 3134 3931  bar...._..{{1491
-000002b0: 2c20 3637 347d 2c20 7b39 3230 2c20 3433  , 674}, {920, 43
+000002a0: 6261 7208 0908 095f 1019 7b7b 3134 3930  bar...._..{{1490
+000002b0: 2c20 3637 357d 2c20 7b39 3230 2c20 3433  , 675}, {920, 43
 000002c0: 367d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  6}}...#/;R_klmno
 000002d0: 8b00 0000 0000 0001 0100 0000 0000 0000  ................
 000002e0: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
 000002f0: 8c00 0000 0e00 7000 6f00 6900 6e00 7400  ......p.o.i.n.t.
 00000300: 5f00 6d00 7500 7400 6100 7400 6900 6f00  _.m.u.t.a.t.i.o.
 00000310: 6e6c 6731 5363 6f6d 7000 0000 0000 0000  nlg1Scomp.......
 00000320: 0000 0000 0e00 7000 6f00 6900 6e00 7400  ......p.o.i.n.t.
```

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/23S.fsa` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/23S.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/acrB.fsa` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/acrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/gyrA.fsa` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/gyrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/gyrB.fsa` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/gyrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/parC.fsa` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/parC.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/parE.fsa` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/parE.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/phenotypes.txt` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/phenotypes.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/pmrA.fsa` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/pmrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/pmrB.fsa` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/pmrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/salmonella.fsa` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b` & `PointBlaster-0.1.5/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/PointBlaster.egg-info/PKG-INFO` & `PointBlaster-0.1.5/PointBlaster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PointBlaster
-Version: 0.1.4
+Version: 0.1.5
 Summary: find point mutation in assembled genomes
 Home-page: https://github.com/hbucqp/PointBlaster
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,wgs,blastn,pointmutation
 Platform: any
```

### Comparing `PointBlaster-0.1.4/PointBlaster.egg-info/SOURCES.txt` & `PointBlaster-0.1.5/PointBlaster.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 PointBlaster.egg-info/SOURCES.txt
 PointBlaster.egg-info/dependency_links.txt
 PointBlaster.egg-info/entry_points.txt
 PointBlaster.egg-info/requires.txt
 PointBlaster.egg-info/top_level.txt
 PointBlaster/db/.DS_Store
 PointBlaster/db/point_mutation/.DS_Store
+PointBlaster/db/point_mutation/campylobacter/.DS_Store
 PointBlaster/db/point_mutation/campylobacter/23S.fsa
 PointBlaster/db/point_mutation/campylobacter/RNA_genes.txt
 PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b
 PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa
+PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa.original
 PointBlaster/db/point_mutation/campylobacter/campylobacter.length.b
 PointBlaster/db/point_mutation/campylobacter/campylobacter.name
 PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b
 PointBlaster/db/point_mutation/campylobacter/genes.txt
 PointBlaster/db/point_mutation/campylobacter/gyrA.fsa
 PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa
 PointBlaster/db/point_mutation/campylobacter/phenotypes.txt
@@ -37,10 +39,14 @@
 PointBlaster/db/point_mutation/salmonella/parE.fsa
 PointBlaster/db/point_mutation/salmonella/phenotypes.txt
 PointBlaster/db/point_mutation/salmonella/pmrA.fsa
 PointBlaster/db/point_mutation/salmonella/pmrB.fsa
 PointBlaster/db/point_mutation/salmonella/resistens-overview.txt
 PointBlaster/db/point_mutation/salmonella/salmonella.comp.b
 PointBlaster/db/point_mutation/salmonella/salmonella.fsa
+PointBlaster/db/point_mutation/salmonella/salmonella.fsa.original
 PointBlaster/db/point_mutation/salmonella/salmonella.length.b
 PointBlaster/db/point_mutation/salmonella/salmonella.name
-PointBlaster/db/point_mutation/salmonella/salmonella.seq.b
+PointBlaster/db/point_mutation/salmonella/salmonella.seq.b
+dist/.DS_Store
+dist/PointBlaster-0.1.4-py3-none-any.whl
+dist/PointBlaster-0.1.4.tar.gz
```

### Comparing `PointBlaster-0.1.4/README.md` & `PointBlaster-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.4/setup.py` & `PointBlaster-0.1.5/setup.py`

 * *Files identical despite different names*

