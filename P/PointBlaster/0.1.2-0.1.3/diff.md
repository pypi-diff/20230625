# Comparing `tmp/PointBlaster-0.1.2.tar.gz` & `tmp/PointBlaster-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PointBlaster-0.1.2.tar", last modified: Sun Jun 25 06:35:50 2023, max compression
+gzip compressed data, was "PointBlaster-0.1.3.tar", last modified: Sun Jun 25 06:38:21 2023, max compression
```

## Comparing `PointBlaster-0.1.2.tar` & `PointBlaster-0.1.3.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:35:50.008856 PointBlaster-0.1.2/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 06:35:00.000000 PointBlaster-0.1.2/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       61 2023-06-25 06:30:58.000000 PointBlaster-0.1.2/MANIFEST.in
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-25 06:35:50.008726 PointBlaster-0.1.2/PKG-INFO
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:35:49.990161 PointBlaster-0.1.2/PointBlaster/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 05:55:52.000000 PointBlaster-0.1.2/PointBlaster/.DS_Store
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    21412 2023-06-25 06:11:03.000000 PointBlaster-0.1.2/PointBlaster/PointBlaster.py
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      303 2023-06-25 06:35:08.000000 PointBlaster-0.1.2/PointBlaster/__init__.py
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:35:49.991135 PointBlaster-0.1.2/PointBlaster/db/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 05:56:01.000000 PointBlaster-0.1.2/PointBlaster/db/.DS_Store
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:35:49.991372 PointBlaster-0.1.2/PointBlaster/db/point_mutation/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     8196 2023-06-25 05:56:06.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/.DS_Store
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:35:49.999923 PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2972 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/23S.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        4 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/RNA_genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)  4259822 2023-06-19 06:54:12.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     8657 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:54:12.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.length.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      149 2023-06-19 06:54:12.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.name
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     4936 2023-06-19 06:54:12.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       14 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     5272 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2613 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2523 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1961 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      412 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/rpsL.fsa
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:35:50.006582 PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1593 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/RNA_genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     3214 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/acrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/genes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2694 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/gyrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2469 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/gyrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2311 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/parC.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1940 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/parE.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     7137 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/phenotypes.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      698 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/pmrA.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1106 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/pmrB.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     5030 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)  4318510 2023-06-19 06:54:12.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)    16025 2023-06-19 06:40:55.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/salmonella.fsa
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       72 2023-06-19 06:54:12.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/salmonella.length.b
--rw-r--r--   0 cuiqingpo   (501) staff       (20)      296 2023-06-19 06:54:12.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/salmonella.name
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     7888 2023-06-19 06:54:12.000000 PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:35:49.991022 PointBlaster-0.1.2/PointBlaster.egg-info/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-25 06:35:49.000000 PointBlaster-0.1.2/PointBlaster.egg-info/PKG-INFO
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2214 2023-06-25 06:35:49.000000 PointBlaster-0.1.2/PointBlaster.egg-info/SOURCES.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2023-06-25 06:35:49.000000 PointBlaster-0.1.2/PointBlaster.egg-info/dependency_links.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       65 2023-06-25 06:35:49.000000 PointBlaster-0.1.2/PointBlaster.egg-info/entry_points.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2023-06-25 06:35:49.000000 PointBlaster-0.1.2/PointBlaster.egg-info/requires.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       13 2023-06-25 06:35:49.000000 PointBlaster-0.1.2/PointBlaster.egg-info/top_level.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     1611 2023-06-25 06:11:36.000000 PointBlaster-0.1.2/README.md
-drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:35:50.008390 PointBlaster-0.1.2/dist/
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     7930 2023-06-25 06:29:43.000000 PointBlaster-0.1.2/dist/PointBlaster-0.1.1-py3-none-any.whl
--rw-r--r--   0 cuiqingpo   (501) staff       (20)   242561 2023-06-25 06:29:43.000000 PointBlaster-0.1.2/dist/PointBlaster-0.1.1.tar.gz
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       57 2023-06-25 05:58:37.000000 PointBlaster-0.1.2/requirements.txt
--rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2023-06-25 06:35:50.008899 PointBlaster-0.1.2/setup.cfg
--rw-r--r--   0 cuiqingpo   (501) staff       (20)     2161 2023-06-25 06:34:44.000000 PointBlaster-0.1.2/setup.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:38:21.086372 PointBlaster-0.1.3/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 06:35:00.000000 PointBlaster-0.1.3/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       61 2023-06-25 06:30:58.000000 PointBlaster-0.1.3/MANIFEST.in
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-25 06:38:21.086209 PointBlaster-0.1.3/PKG-INFO
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:38:21.065768 PointBlaster-0.1.3/PointBlaster/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 05:55:52.000000 PointBlaster-0.1.3/PointBlaster/.DS_Store
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    21412 2023-06-25 06:11:03.000000 PointBlaster-0.1.3/PointBlaster/PointBlaster.py
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      303 2023-06-25 06:37:26.000000 PointBlaster-0.1.3/PointBlaster/__init__.py
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:38:21.066723 PointBlaster-0.1.3/PointBlaster/db/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     6148 2023-06-25 05:56:01.000000 PointBlaster-0.1.3/PointBlaster/db/.DS_Store
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:38:21.067059 PointBlaster-0.1.3/PointBlaster/db/point_mutation/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     8196 2023-06-25 05:56:06.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/.DS_Store
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:38:21.074835 PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2972 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/23S.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        4 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/RNA_genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)  4259822 2023-06-19 06:54:12.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     8657 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:54:12.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/campylobacter.length.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      149 2023-06-19 06:54:12.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/campylobacter.name
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     4936 2023-06-19 06:54:12.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       14 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     5272 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2613 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2523 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1961 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      412 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/rpsL.fsa
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:38:21.082618 PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1593 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        9 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/RNA_genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     3214 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/acrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       44 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/genes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2694 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/gyrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2469 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/gyrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2311 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/parC.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1940 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/parE.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     7137 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/phenotypes.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      698 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/pmrA.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1106 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/pmrB.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     5030 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)  4318510 2023-06-19 06:54:12.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)    16025 2023-06-19 06:40:55.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/salmonella.fsa
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       72 2023-06-19 06:54:12.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/salmonella.length.b
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)      296 2023-06-19 06:54:12.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/salmonella.name
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     7888 2023-06-19 06:54:12.000000 PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:38:21.066582 PointBlaster-0.1.3/PointBlaster.egg-info/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2376 2023-06-25 06:38:20.000000 PointBlaster-0.1.3/PointBlaster.egg-info/PKG-INFO
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2286 2023-06-25 06:38:20.000000 PointBlaster-0.1.3/PointBlaster.egg-info/SOURCES.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)        1 2023-06-25 06:38:20.000000 PointBlaster-0.1.3/PointBlaster.egg-info/dependency_links.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       65 2023-06-25 06:38:20.000000 PointBlaster-0.1.3/PointBlaster.egg-info/entry_points.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       39 2023-06-25 06:38:20.000000 PointBlaster-0.1.3/PointBlaster.egg-info/requires.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       13 2023-06-25 06:38:20.000000 PointBlaster-0.1.3/PointBlaster.egg-info/top_level.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     1611 2023-06-25 06:11:36.000000 PointBlaster-0.1.3/README.md
+drwxr-xr-x   0 cuiqingpo   (501) staff       (20)        0 2023-06-25 06:38:21.085706 PointBlaster-0.1.3/dist/
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     7930 2023-06-25 06:29:43.000000 PointBlaster-0.1.3/dist/PointBlaster-0.1.1-py3-none-any.whl
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)   242561 2023-06-25 06:29:43.000000 PointBlaster-0.1.3/dist/PointBlaster-0.1.1.tar.gz
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     8195 2023-06-25 06:35:50.000000 PointBlaster-0.1.3/dist/PointBlaster-0.1.2-py3-none-any.whl
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)   493249 2023-06-25 06:35:50.000000 PointBlaster-0.1.3/dist/PointBlaster-0.1.2.tar.gz
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       57 2023-06-25 05:58:37.000000 PointBlaster-0.1.3/requirements.txt
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)       38 2023-06-25 06:38:21.086418 PointBlaster-0.1.3/setup.cfg
+-rw-r--r--   0 cuiqingpo   (501) staff       (20)     2161 2023-06-25 06:37:13.000000 PointBlaster-0.1.3/setup.py
```

### Comparing `PointBlaster-0.1.2/.DS_Store` & `PointBlaster-0.1.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PKG-INFO` & `PointBlaster-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PointBlaster
-Version: 0.1.2
+Version: 0.1.3
 Summary: find point mutation in assembled genomes
 Home-page: https://github.com/hbucqp/PointBlaster
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,wgs,blastn,pointmutation
 Platform: any
```

### Comparing `PointBlaster-0.1.2/PointBlaster/.DS_Store` & `PointBlaster-0.1.3/PointBlaster/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/PointBlaster.py` & `PointBlaster-0.1.3/PointBlaster/PointBlaster.py`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/.DS_Store` & `PointBlaster-0.1.3/PointBlaster/db/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/.DS_Store` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/.DS_Store`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/23S.fsa` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/23S.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/campylobacter.comp.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/campylobacter.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/campylobacter.seq.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/gyrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/gyrA_2.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/phenotypes.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/campylobacter/resistens-overview.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/16S-rrsD.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/acrB.fsa` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/acrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/gyrA.fsa` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/gyrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/gyrB.fsa` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/gyrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/parC.fsa` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/parC.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/parE.fsa` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/parE.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/phenotypes.txt` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/phenotypes.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/pmrA.fsa` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/pmrA.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/pmrB.fsa` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/pmrB.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/resistens-overview.txt`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/salmonella.comp.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/salmonella.fsa` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/salmonella.fsa`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b` & `PointBlaster-0.1.3/PointBlaster/db/point_mutation/salmonella/salmonella.seq.b`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/PointBlaster.egg-info/PKG-INFO` & `PointBlaster-0.1.3/PointBlaster.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PointBlaster
-Version: 0.1.2
+Version: 0.1.3
 Summary: find point mutation in assembled genomes
 Home-page: https://github.com/hbucqp/PointBlaster
 Author: Qingpo Cui
 Author-email: cqp@cau.edu.cn
 License: MIT Licence
 Keywords: pip,wgs,blastn,pointmutation
 Platform: any
```

### Comparing `PointBlaster-0.1.2/PointBlaster.egg-info/SOURCES.txt` & `PointBlaster-0.1.3/PointBlaster.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,8 +41,10 @@
 PointBlaster/db/point_mutation/salmonella/resistens-overview.txt
 PointBlaster/db/point_mutation/salmonella/salmonella.comp.b
 PointBlaster/db/point_mutation/salmonella/salmonella.fsa
 PointBlaster/db/point_mutation/salmonella/salmonella.length.b
 PointBlaster/db/point_mutation/salmonella/salmonella.name
 PointBlaster/db/point_mutation/salmonella/salmonella.seq.b
 dist/PointBlaster-0.1.1-py3-none-any.whl
-dist/PointBlaster-0.1.1.tar.gz
+dist/PointBlaster-0.1.1.tar.gz
+dist/PointBlaster-0.1.2-py3-none-any.whl
+dist/PointBlaster-0.1.2.tar.gz
```

### Comparing `PointBlaster-0.1.2/README.md` & `PointBlaster-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/dist/PointBlaster-0.1.1-py3-none-any.whl` & `PointBlaster-0.1.3/dist/PointBlaster-0.1.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/dist/PointBlaster-0.1.1.tar.gz` & `PointBlaster-0.1.3/dist/PointBlaster-0.1.1.tar.gz`

 * *Files identical despite different names*

### Comparing `PointBlaster-0.1.2/setup.py` & `PointBlaster-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 try:
     from setuptools import setup, find_packages
 except ImportError:
     from distutils.core import setup
 
 
 requirements = [
-    'Bio', 'pandas', 'numpy', 'cvmblaster' 'setuptools'
+    'Bio', 'pandas', 'numpy', 'cvmblaster','setuptools'
 ]
 
 about = {}
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, 'PointBlaster', '__init__.py'), 'r', encoding='utf-8') as f:
     exec(f.read(), about)
```

