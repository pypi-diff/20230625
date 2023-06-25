# Comparing `tmp/ontolocy-0.1.3.tar.gz` & `tmp/ontolocy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontolocy-0.1.3.tar", last modified: Thu Feb  9 18:27:44 2023, max compression
+gzip compressed data, was "ontolocy-0.3.0.tar", last modified: Sun Jun 25 12:03:12 2023, max compression
```

## Comparing `ontolocy-0.1.3.tar` & `ontolocy-0.3.0.tar`

### file list

```diff
@@ -1,54 +1,58 @@
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-02-09 18:27:44.168707 ontolocy-0.1.3/
--rw-r--r--   0 mike      (1000) mike      (1000)     1065 2022-07-26 13:43:01.000000 ontolocy-0.1.3/LICENSE
--rw-r--r--   0 mike      (1000) mike      (1000)      640 2023-02-09 18:27:44.168707 ontolocy-0.1.3/PKG-INFO
--rw-r--r--   0 mike      (1000) mike      (1000)      202 2022-12-31 17:32:12.000000 ontolocy-0.1.3/README.md
--rw-r--r--   0 mike      (1000) mike      (1000)      747 2022-10-30 07:18:42.000000 ontolocy-0.1.3/pyproject.toml
--rw-r--r--   0 mike      (1000) mike      (1000)      663 2023-02-09 18:27:44.168707 ontolocy-0.1.3/setup.cfg
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-02-09 18:27:44.158707 ontolocy-0.1.3/src/
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-02-09 18:27:44.158707 ontolocy-0.1.3/src/ontolocy/
--rw-r--r--   0 mike      (1000) mike      (1000)     5918 2023-02-09 18:26:48.000000 ontolocy-0.1.3/src/ontolocy/__init__.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1068 2022-08-17 14:57:48.000000 ontolocy-0.1.3/src/ontolocy/dataorigin.py
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-02-09 18:27:44.168707 ontolocy-0.1.3/src/ontolocy/models/
--rw-r--r--   0 mike      (1000) mike      (1000)        0 2022-07-26 13:44:48.000000 ontolocy-0.1.3/src/ontolocy/models/__init__.py
--rw-r--r--   0 mike      (1000) mike      (1000)      340 2022-09-24 16:51:04.000000 ontolocy-0.1.3/src/ontolocy/models/actortype.py
--rw-r--r--   0 mike      (1000) mike      (1000)      655 2022-08-16 10:59:35.000000 ontolocy-0.1.3/src/ontolocy/models/asn.py
--rw-r--r--   0 mike      (1000) mike      (1000)      514 2022-10-28 18:07:41.000000 ontolocy-0.1.3/src/ontolocy/models/banner.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1893 2022-10-28 18:07:41.000000 ontolocy-0.1.3/src/ontolocy/models/campaign.py
--rw-r--r--   0 mike      (1000) mike      (1000)      917 2022-12-31 16:34:16.000000 ontolocy-0.1.3/src/ontolocy/models/capecpattern.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1536 2022-10-28 18:07:41.000000 ontolocy-0.1.3/src/ontolocy/models/cobaltstrikebeacon.py
--rw-r--r--   0 mike      (1000) mike      (1000)      234 2022-08-10 13:58:53.000000 ontolocy-0.1.3/src/ontolocy/models/cobaltstrikewatermark.py
--rw-r--r--   0 mike      (1000) mike      (1000)     6861 2022-09-02 17:33:06.000000 ontolocy-0.1.3/src/ontolocy/models/country.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2876 2022-12-31 16:47:42.000000 ontolocy-0.1.3/src/ontolocy/models/cpe.py
--rw-r--r--   0 mike      (1000) mike      (1000)      813 2022-12-31 16:34:16.000000 ontolocy-0.1.3/src/ontolocy/models/cve.py
--rw-r--r--   0 mike      (1000) mike      (1000)      311 2022-12-31 16:34:16.000000 ontolocy-0.1.3/src/ontolocy/models/cwe.py
--rw-r--r--   0 mike      (1000) mike      (1000)      359 2022-09-25 08:30:29.000000 ontolocy-0.1.3/src/ontolocy/models/cyberharm.py
--rw-r--r--   0 mike      (1000) mike      (1000)      778 2022-10-28 18:07:41.000000 ontolocy-0.1.3/src/ontolocy/models/dnsrecord.py
--rw-r--r--   0 mike      (1000) mike      (1000)      568 2022-10-28 18:07:41.000000 ontolocy-0.1.3/src/ontolocy/models/domainname.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1076 2023-01-05 20:25:55.000000 ontolocy-0.1.3/src/ontolocy/models/exploit.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1942 2022-12-31 16:34:16.000000 ontolocy-0.1.3/src/ontolocy/models/intrusionset.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2862 2023-01-06 18:40:04.000000 ontolocy-0.1.3/src/ontolocy/models/ip.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1278 2022-08-16 16:32:20.000000 ontolocy-0.1.3/src/ontolocy/models/jarmhash.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2566 2022-11-13 13:53:28.000000 ontolocy-0.1.3/src/ontolocy/models/listeningsocket.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1687 2022-12-31 16:34:16.000000 ontolocy-0.1.3/src/ontolocy/models/mitreattackcampaign.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1085 2022-12-31 16:34:16.000000 ontolocy-0.1.3/src/ontolocy/models/mitreattacksoftware.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1150 2022-12-31 16:34:16.000000 ontolocy-0.1.3/src/ontolocy/models/mitreattacktactic.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1141 2022-11-12 10:51:41.000000 ontolocy-0.1.3/src/ontolocy/models/mitreattacktechnique.py
--rw-r--r--   0 mike      (1000) mike      (1000)      545 2022-10-28 18:07:41.000000 ontolocy-0.1.3/src/ontolocy/models/networkservice.py
--rw-r--r--   0 mike      (1000) mike      (1000)      889 2022-12-31 16:34:16.000000 ontolocy-0.1.3/src/ontolocy/models/organisation.py
--rw-r--r--   0 mike      (1000) mike      (1000)      854 2022-10-28 18:07:41.000000 ontolocy-0.1.3/src/ontolocy/models/port.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3328 2022-12-31 16:34:16.000000 ontolocy-0.1.3/src/ontolocy/models/report.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4780 2022-10-28 18:07:41.000000 ontolocy-0.1.3/src/ontolocy/models/sector.py
--rw-r--r--   0 mike      (1000) mike      (1000)      919 2022-10-28 18:07:41.000000 ontolocy-0.1.3/src/ontolocy/models/threatactor.py
--rw-r--r--   0 mike      (1000) mike      (1000)      434 2022-08-18 14:24:07.000000 ontolocy-0.1.3/src/ontolocy/models/url.py
--rw-r--r--   0 mike      (1000) mike      (1000)      822 2022-10-28 18:07:41.000000 ontolocy-0.1.3/src/ontolocy/models/x509certificate.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1117 2023-02-09 18:26:48.000000 ontolocy-0.1.3/src/ontolocy/node.py
--rw-r--r--   0 mike      (1000) mike      (1000)      991 2022-11-25 12:07:22.000000 ontolocy-0.1.3/src/ontolocy/relationship.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1607 2022-08-04 15:46:26.000000 ontolocy-0.1.3/src/ontolocy/utils.py
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-02-09 18:27:44.168707 ontolocy-0.1.3/src/ontolocy.egg-info/
--rw-r--r--   0 mike      (1000) mike      (1000)      640 2023-02-09 18:27:44.000000 ontolocy-0.1.3/src/ontolocy.egg-info/PKG-INFO
--rw-r--r--   0 mike      (1000) mike      (1000)     1451 2023-02-09 18:27:44.000000 ontolocy-0.1.3/src/ontolocy.egg-info/SOURCES.txt
--rw-r--r--   0 mike      (1000) mike      (1000)        1 2023-02-09 18:27:44.000000 ontolocy-0.1.3/src/ontolocy.egg-info/dependency_links.txt
--rw-r--r--   0 mike      (1000) mike      (1000)       33 2023-02-09 18:27:44.000000 ontolocy-0.1.3/src/ontolocy.egg-info/requires.txt
--rw-r--r--   0 mike      (1000) mike      (1000)        9 2023-02-09 18:27:44.000000 ontolocy-0.1.3/src/ontolocy.egg-info/top_level.txt
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-02-09 18:27:44.168707 ontolocy-0.1.3/tests/
--rw-r--r--   0 mike      (1000) mike      (1000)      900 2023-02-09 18:26:48.000000 ontolocy-0.1.3/tests/test_node.py
+drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-06-25 12:03:12.846553 ontolocy-0.3.0/
+-rw-r--r--   0 mike      (1000) mike      (1000)     1065 2022-07-26 13:43:01.000000 ontolocy-0.3.0/LICENSE
+-rw-r--r--   0 mike      (1000) mike      (1000)      751 2023-06-25 12:03:12.846553 ontolocy-0.3.0/PKG-INFO
+-rw-r--r--   0 mike      (1000) mike      (1000)      313 2023-06-25 12:02:02.000000 ontolocy-0.3.0/README.md
+-rw-r--r--   0 mike      (1000) mike      (1000)      747 2022-10-30 07:18:42.000000 ontolocy-0.3.0/pyproject.toml
+-rw-r--r--   0 mike      (1000) mike      (1000)      663 2023-06-25 12:03:12.846553 ontolocy-0.3.0/setup.cfg
+drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-06-25 12:03:12.826553 ontolocy-0.3.0/src/
+drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-06-25 12:03:12.836553 ontolocy-0.3.0/src/ontolocy/
+-rw-r--r--   0 mike      (1000) mike      (1000)     7101 2023-06-25 12:02:02.000000 ontolocy-0.3.0/src/ontolocy/__init__.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1068 2022-08-17 14:57:48.000000 ontolocy-0.3.0/src/ontolocy/dataorigin.py
+drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-06-25 12:03:12.846553 ontolocy-0.3.0/src/ontolocy/models/
+-rw-r--r--   0 mike      (1000) mike      (1000)        0 2022-07-26 13:44:48.000000 ontolocy-0.3.0/src/ontolocy/models/__init__.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1301 2023-06-25 12:02:02.000000 ontolocy-0.3.0/src/ontolocy/models/actortype.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      723 2023-06-25 12:02:02.000000 ontolocy-0.3.0/src/ontolocy/models/asn.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      514 2022-10-28 18:07:41.000000 ontolocy-0.3.0/src/ontolocy/models/banner.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1893 2022-10-28 18:07:41.000000 ontolocy-0.3.0/src/ontolocy/models/campaign.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      917 2022-12-31 16:34:16.000000 ontolocy-0.3.0/src/ontolocy/models/capecpattern.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1536 2022-10-28 18:07:41.000000 ontolocy-0.3.0/src/ontolocy/models/cobaltstrikebeacon.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      234 2022-08-10 13:58:53.000000 ontolocy-0.3.0/src/ontolocy/models/cobaltstrikewatermark.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1536 2023-06-25 12:02:02.000000 ontolocy-0.3.0/src/ontolocy/models/control.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     6861 2022-09-02 17:33:06.000000 ontolocy-0.3.0/src/ontolocy/models/country.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2876 2022-12-31 16:47:42.000000 ontolocy-0.3.0/src/ontolocy/models/cpe.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      843 2023-06-25 12:02:02.000000 ontolocy-0.3.0/src/ontolocy/models/cve.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      311 2022-12-31 16:34:16.000000 ontolocy-0.3.0/src/ontolocy/models/cwe.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      359 2022-09-25 08:30:29.000000 ontolocy-0.3.0/src/ontolocy/models/cyberharm.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1720 2023-06-25 12:02:02.000000 ontolocy-0.3.0/src/ontolocy/models/dnsrecord.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      945 2023-06-25 12:02:02.000000 ontolocy-0.3.0/src/ontolocy/models/domainname.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1076 2023-01-05 20:25:55.000000 ontolocy-0.3.0/src/ontolocy/models/exploit.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1122 2023-06-25 12:02:02.000000 ontolocy-0.3.0/src/ontolocy/models/host.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1911 2023-06-25 12:02:02.000000 ontolocy-0.3.0/src/ontolocy/models/intrusionset.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3440 2023-06-25 12:02:02.000000 ontolocy-0.3.0/src/ontolocy/models/ip.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1278 2022-08-16 16:32:20.000000 ontolocy-0.3.0/src/ontolocy/models/jarmhash.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2659 2023-06-25 12:02:02.000000 ontolocy-0.3.0/src/ontolocy/models/listeningsocket.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      871 2023-06-25 12:02:02.000000 ontolocy-0.3.0/src/ontolocy/models/macaddress.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1687 2022-12-31 16:34:16.000000 ontolocy-0.3.0/src/ontolocy/models/mitreattackcampaign.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1085 2022-12-31 16:34:16.000000 ontolocy-0.3.0/src/ontolocy/models/mitreattacksoftware.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1150 2022-12-31 16:34:16.000000 ontolocy-0.3.0/src/ontolocy/models/mitreattacktactic.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1141 2022-11-12 10:51:41.000000 ontolocy-0.3.0/src/ontolocy/models/mitreattacktechnique.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      545 2022-10-28 18:07:41.000000 ontolocy-0.3.0/src/ontolocy/models/networkservice.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1843 2023-06-25 12:02:02.000000 ontolocy-0.3.0/src/ontolocy/models/organisation.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      854 2022-10-28 18:07:41.000000 ontolocy-0.3.0/src/ontolocy/models/port.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3542 2023-06-25 12:02:02.000000 ontolocy-0.3.0/src/ontolocy/models/report.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4780 2022-10-28 18:07:41.000000 ontolocy-0.3.0/src/ontolocy/models/sector.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1173 2023-06-25 12:02:02.000000 ontolocy-0.3.0/src/ontolocy/models/threatactor.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      434 2022-08-18 14:24:07.000000 ontolocy-0.3.0/src/ontolocy/models/url.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1362 2023-06-25 12:02:02.000000 ontolocy-0.3.0/src/ontolocy/models/useraccount.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      822 2022-10-28 18:07:41.000000 ontolocy-0.3.0/src/ontolocy/models/x509certificate.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1209 2023-06-25 12:02:02.000000 ontolocy-0.3.0/src/ontolocy/node.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      991 2022-11-25 12:07:22.000000 ontolocy-0.3.0/src/ontolocy/relationship.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1607 2022-08-04 15:46:26.000000 ontolocy-0.3.0/src/ontolocy/utils.py
+drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-06-25 12:03:12.836553 ontolocy-0.3.0/src/ontolocy.egg-info/
+-rw-r--r--   0 mike      (1000) mike      (1000)      751 2023-06-25 12:03:12.000000 ontolocy-0.3.0/src/ontolocy.egg-info/PKG-INFO
+-rw-r--r--   0 mike      (1000) mike      (1000)     1579 2023-06-25 12:03:12.000000 ontolocy-0.3.0/src/ontolocy.egg-info/SOURCES.txt
+-rw-r--r--   0 mike      (1000) mike      (1000)        1 2023-06-25 12:03:12.000000 ontolocy-0.3.0/src/ontolocy.egg-info/dependency_links.txt
+-rw-r--r--   0 mike      (1000) mike      (1000)       33 2023-06-25 12:03:12.000000 ontolocy-0.3.0/src/ontolocy.egg-info/requires.txt
+-rw-r--r--   0 mike      (1000) mike      (1000)        9 2023-06-25 12:03:12.000000 ontolocy-0.3.0/src/ontolocy.egg-info/top_level.txt
+drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-06-25 12:03:12.846553 ontolocy-0.3.0/tests/
+-rw-r--r--   0 mike      (1000) mike      (1000)      900 2023-02-09 18:26:48.000000 ontolocy-0.3.0/tests/test_node.py
```

### Comparing `ontolocy-0.1.3/LICENSE` & `ontolocy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ontolocy-0.1.3/PKG-INFO` & `ontolocy-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontolocy
-Version: 0.1.3
+Version: 0.3.0
 Summary: A Python package for modeling cybersecurity data in a Neo4j graph database.
 Home-page: https://github.com/ontolocy/ontolocy-lib
 Author: Ontolocy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -14,7 +14,11 @@
 # Ontolocy
 
 An open source cyber security graph ontology.
 
 Use Python and Neo4j to explore cyber security data as a graph.
 
 Currently in alpha/proof-of-concept stage - the ontology is likely to change.
+
+> "All models are wrong, but some are useful" - George Box
+
+Read the [docs](https://ontolocy.readthedocs.io/)
```

### Comparing `ontolocy-0.1.3/pyproject.toml` & `ontolocy-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ontolocy-0.1.3/setup.cfg` & `ontolocy-0.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ontolocy
-version = 0.1.3
+version = 0.3.0
 author = Ontolocy
 description = A Python package for modeling cybersecurity data in a Neo4j graph database.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ontolocy/ontolocy-lib
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `ontolocy-0.1.3/src/ontolocy/__init__.py` & `ontolocy-0.3.0/src/ontolocy/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,46 +18,62 @@
 )
 from ontolocy.models.cobaltstrikebeacon import (
     CobaltStikeBeaconCollectedFrom,
     CobaltStikeBeaconHasWatermark,
     CobaltStrikeBeacon,
 )
 from ontolocy.models.cobaltstrikewatermark import CobaltStrikeWatermark
+from ontolocy.models.control import (
+    Control,
+    ControlMitigatesAttackTechnique,
+    ControlRelatedToControl,
+)
 from ontolocy.models.country import Country
 from ontolocy.models.cpe import CPE
 from ontolocy.models.cve import CVE, CVERelatesToCPE, CVERelatesToCWE
 from ontolocy.models.cwe import CWE
 from ontolocy.models.cyberharm import CyberHarm
+from ontolocy.models.dnsrecord import (
+    DNSRecord,
+    DNSRecordForDomain,
+    DNSRecordPointsToDomainName,
+    DNSRecordPointsToIPAddress,
+)
+from ontolocy.models.domainname import DomainName, DomainNameHasDNSRecord
 from ontolocy.models.exploit import Exploit, ExploitExploitsVulnerability
+from ontolocy.models.host import Host
 from ontolocy.models.intrusionset import (
     IntrusionSet,
     IntrusionSetAttributedToNation,
     IntrusionSetIsOfType,
     IntrusionSetLinkedToIntrusionSet,
     IntrusionSetLinkedToThreatActor,
     IntrusionSetUsesSoftware,
     IntrusionSetUsesTechnique,
 )
 from ontolocy.models.ip import (
     IPAddressBelongsToASN,
     IPAddressHasOpenPort,
     IPAddressIdentifiedAsPlatform,
     IPAddressLocatedInCountry,
+    IPAddressMapsToMACAddress,
     IPAddressNode,
+    IPAddressObservedWithHostname,
 )
 from ontolocy.models.jarmhash import JarmHash
 from ontolocy.models.listeningsocket import (
     ListeningSocket,
     ListeningSocketUsesPort,
     OpenPortHasJarmHash,
     OpenPortPresentsBanner,
     OpenPortPresentsX509Certificate,
     ServiceHostsURL,
     ServiceIdentifiedAsPlatform,
 )
+from ontolocy.models.macaddress import MACAddress, MACAddressAssignedToHost
 from ontolocy.models.mitreattackcampaign import (
     MitreAttackCampaign,
     MitreCampaignAttributedTo,
     MitreCampaignUsesSoftware,
     MitreCampaignUsesTechnique,
 )
 from ontolocy.models.mitreattacksoftware import (
@@ -71,15 +87,17 @@
 from ontolocy.models.mitreattacktechnique import (
     MitreAttackTechnique,
     MitreSubtechniqueOf,
 )
 from ontolocy.models.networkservice import NetworkService, NetworkServiceRunsOnPort
 from ontolocy.models.organisation import (
     Organisation,
-    OrganisationAssignedAssignedCVSSToCVE,
+    OrganisationAssignedCVSSToCVE,
+    OrganisationPublishedThreatReport,
+    OrganisationReportedExploitationOfCVE,
 )
 from ontolocy.models.port import Port
 from ontolocy.models.report import (
     Report,
     ReportIdentifiesCampaign,
     ReportIdentifiesCVE,
     ReportIdentifiesCyberHarm,
@@ -99,14 +117,15 @@
 from ontolocy.models.sector import Sector
 from ontolocy.models.threatactor import (
     ThreatActor,
     ThreatActorAttributedToNation,
     ThreatActorIsOfType,
 )
 from ontolocy.models.url import URLNode, UrlRedirectsToUrl
+from ontolocy.models.useraccount import UserAccount, UserAccountAuthorizedOnHost
 from ontolocy.models.x509certificate import X509Certificate
 from ontolocy.node import OntolocyNode
 from ontolocy.relationship import OntolocyRelationship
 from ontolocy.utils import init_ontolocy
 
 __all__ = [
     "DataOrigin",
@@ -129,39 +148,53 @@
     "CAPECPattern",
     "CAPECPatternMapsToAttackTechnique",
     "CAPECPatternRelatesToCWE",
     "CobaltStrikeBeacon",
     "CobaltStikeBeaconCollectedFrom",
     "CobaltStikeBeaconHasWatermark",
     "CobaltStrikeWatermark",
+    "Control",
+    "ControlMitigatesAttackTechnique",
+    "ControlRelatedToControl",
     "Country",
     "CPE",
     "CVE",
     "CVERelatesToCPE",
     "CVERelatesToCWE",
     "CWE",
     "CyberHarm",
+    "DNSRecord",
+    "DNSRecordForDomain",
+    "DNSRecordPointsToDomainName",
+    "DNSRecordPointsToIPAddress",
+    "DomainName",
+    "DomainNameHasDNSRecord",
     "Exploit",
     "ExploitExploitsVulnerability",
+    "Host",
     "IntrusionSet",
     "IntrusionSetAttributedToNation",
     "IntrusionSetLinkedToIntrusionSet",
     "IntrusionSetIsOfType",
     "IntrusionSetLinkedToThreatActor",
     "IntrusionSetUsesSoftware",
     "IntrusionSetUsesTechnique",
     "IPAddressNode",
     "IPAddressBelongsToASN",
     "IPAddressHasOpenPort",
     "IPAddressIdentifiedAsPlatform",
     "IPAddressLocatedInCountry",
+    "IPAddressMapsToMACAddress",
+    "IPAddressObservedWithHostname",
     "JarmHash",
     "ListeningSocket",
     "ListeningSocketUsesPort",
     "ServiceIdentifiedAsPlatform",
+    "MACAddress",
+    "MACAddressAssignedToHost",
     "MitreAttackTactic",
     "MitreTacticIncludesTechnique",
     "MitreAttackTechnique",
     "MitreSubtechniqueOf",
     "MitreAttackCampaign",
     "MitreCampaignUsesSoftware",
     "MitreCampaignUsesTechnique",
@@ -170,15 +203,17 @@
     "MitreCampaignAttributedTo",
     "NetworkService",
     "NetworkServiceRunsOnPort",
     "OpenPortHasJarmHash",
     "OpenPortPresentsBanner",
     "OpenPortPresentsX509Certificate",
     "Organisation",
-    "OrganisationAssignedAssignedCVSSToCVE",
+    "OrganisationAssignedCVSSToCVE",
+    "OrganisationPublishedThreatReport",
+    "OrganisationReportedExploitationOfCVE",
     "Port",
     "Report",
     "ReportMentionsCountry",
     "ReportMentionsCVE",
     "ReportMentionsIntrusionSet",
     "ReportMentionsIP",
     "ReportMentionsSector",
@@ -196,8 +231,10 @@
     "ServiceHostsURL",
     "ThreatActor",
     "ThreatActorAttributedToNation",
     "ThreatActorIsOfType",
     "X509Certificate",
     "URLNode",
     "UrlRedirectsToUrl",
+    "UserAccount",
+    "UserAccountAuthorizedOnHost",
 ]
```

### Comparing `ontolocy-0.1.3/src/ontolocy/dataorigin.py` & `ontolocy-0.3.0/src/ontolocy/dataorigin.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.1.3/src/ontolocy/models/asn.py` & `ontolocy-0.3.0/src/ontolocy/models/asn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from typing import ClassVar, Optional
 
 from pydantic import IPvAnyNetwork
 
 from ..node import OntolocyNode
 from ..relationship import OntolocyRelationship
-from .organisation import Organisation
 
 
 class ASN(OntolocyNode):
-
     __primaryproperty__: ClassVar[str] = "number"
     __primarylabel__: ClassVar[Optional[str]] = "ASN"
 
     number: int
     network_name: str
     description: str
     cidr: IPvAnyNetwork
@@ -22,12 +20,16 @@
 
 #
 # OUTGOING RELATIONSHIPS
 #
 
 
 class ASNHasWhoIsRegisteredContact(OntolocyRelationship):
-
     __relationshiptype__: ClassVar[str] = "ASN_HAS_REGISTERED_CONTACT"
 
     source: ASN
-    target: Organisation
+    target: "Organisation"
+
+
+from .organisation import Organisation  # noqa: E402
+
+ASNHasWhoIsRegisteredContact.update_forward_refs()
```

### Comparing `ontolocy-0.1.3/src/ontolocy/models/banner.py` & `ontolocy-0.3.0/src/ontolocy/models/banner.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.1.3/src/ontolocy/models/campaign.py` & `ontolocy-0.3.0/src/ontolocy/models/campaign.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.1.3/src/ontolocy/models/capecpattern.py` & `ontolocy-0.3.0/src/ontolocy/models/capecpattern.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.1.3/src/ontolocy/models/cobaltstrikebeacon.py` & `ontolocy-0.3.0/src/ontolocy/models/cobaltstrikebeacon.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.1.3/src/ontolocy/models/country.py` & `ontolocy-0.3.0/src/ontolocy/models/country.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.1.3/src/ontolocy/models/cpe.py` & `ontolocy-0.3.0/src/ontolocy/models/cpe.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.1.3/src/ontolocy/models/cve.py` & `ontolocy-0.3.0/src/ontolocy/models/cve.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from ..node import OntolocyNode
 from ..relationship import OntolocyRelationship
 from .cpe import CPE
 from .cwe import CWE
 
 
 class CVE(OntolocyNode):
-
     __primaryproperty__: ClassVar[str] = "cve_id"
     __primarylabel__: ClassVar[Optional[str]] = "CVE"
 
     cve_id: constr(to_upper=True, regex=r"CVE-\d{4}-\d{4,8}")  # noqa: F722
     published_date: Optional[datetime]
     assigner: Optional[str]
+    description: Optional[str]
 
 
 #
 # OUTGOING RELATIONSHIPS
 #
```

### Comparing `ontolocy-0.1.3/src/ontolocy/models/dnsrecord.py` & `ontolocy-0.3.0/src/ontolocy/models/port.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,39 @@
+from enum import Enum
 from typing import Any, ClassVar, Dict, Optional
 from uuid import UUID
 
 from pydantic import validator
 
 from ..node import OntolocyNode
 from ..utils import generate_deterministic_uuid
 
 
-class DNSRecord(OntolocyNode):
+class PortProtocolEnum(str, Enum):
+    tcp = "tcp"
+    udp = "udp"
+    sctp = "sctp"
 
+
+class Port(OntolocyNode):
+
+    __primarylabel__: ClassVar[str] = "Port"
     __primaryproperty__: ClassVar[str] = "unique_id"
-    __primarylabel__: ClassVar[Optional[str]] = "DNSRecord"
 
-    type: str
-    name: str
-    content: str
+    port_number: int
+    protocol: PortProtocolEnum
 
-    unique_id: Optional[UUID]
+    unique_id: Optional[UUID] = None
 
     @validator("unique_id", always=True)
-    def generate_dnsrecord_uuid(cls, v: Optional[UUID], values: Dict[str, Any]) -> UUID:
+    def generate_socket_uuid(cls, v: Optional[UUID], values: Dict[str, Any]) -> UUID:
 
         if v is None:
 
             key_values = [
-                values["type"],
-                values["name"],
-                values["content"],
+                values["port_number"],
+                values["protocol"],
             ]
 
             v = generate_deterministic_uuid(key_values)
 
         return v
```

### Comparing `ontolocy-0.1.3/src/ontolocy/models/exploit.py` & `ontolocy-0.3.0/src/ontolocy/models/exploit.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.1.3/src/ontolocy/models/intrusionset.py` & `ontolocy-0.3.0/src/ontolocy/models/intrusionset.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,21 +8,19 @@
 from .country import Country
 from .mitreattacksoftware import MitreAttackSoftware
 from .mitreattacktechnique import MitreAttackTechnique
 from .threatactor import ThreatActor
 
 
 class IntrusionSet(OntolocyNode):
-
     __primaryproperty__: ClassVar[str] = "unique_id"
     __primarylabel__: ClassVar[Optional[str]] = "IntrusionSet"
 
     name: str
     unique_id: str
-    name_giver: Optional[str]
     description: Optional[str]
     url_reference: Optional[HttpUrl]
 
 
 #
 # OUTGOING RELATIONSHIPS
 #
```

### Comparing `ontolocy-0.1.3/src/ontolocy/models/ip.py` & `ontolocy-0.3.0/src/ontolocy/models/ip.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,42 +8,44 @@
 from ..node import OntolocyNode
 from ..relationship import OntolocyRelationship
 from ..utils import generate_deterministic_uuid
 from .asn import ASN
 from .country import Country
 from .cpe import CPE
 from .listeningsocket import ListeningSocket
+from .macaddress import MACAddress
 
 
 class IPVersionEnum(str, Enum):
     ipv4 = "ipv4"
     ipv6 = "ipv6"
 
 
 class IPAddressNode(OntolocyNode):
-
     __primaryproperty__: ClassVar[str] = "unique_id"
     __primarylabel__: ClassVar[str] = "IPAddress"
 
     ip_address: IPvAnyAddress
     ip_version: Optional[IPVersionEnum]
     private: Optional[bool] = None
     namespace: Optional[str] = None
 
     unique_id: Optional[UUID] = None
 
+    def get_identifier(self) -> str:
+        return str(self.ip_address)
+
     @validator("ip_address", pre=True)
     def refang_ip(cls, v: str):
         """Some reports will 'de-fang' an IP with square brackets.
         Remove them for consistency"""
         return v.replace("[", "").replace("]", "")
 
     @validator("ip_version", always=True)
     def mark_ip_version(cls, v, values: Dict[str, Any]):
-
         versions = {4: IPVersionEnum.ipv4, 6: IPVersionEnum.ipv6}
         if v is None and "ip_address" in values:
             return versions[ip_address(values["ip_address"]).version]
         else:
             return v
 
     @validator("private", always=True)
@@ -62,47 +64,60 @@
             return str(uuid4())
 
         else:
             return v
 
     @validator("unique_id", always=True)
     def generate_instance_id(cls, v: Optional[UUID], values: Dict[str, Any]) -> UUID:
-
         if v is None:
-
             key_values = [values["ip_address"], values["namespace"]]
 
             v = generate_deterministic_uuid(key_values)
 
         return v
 
 
 class IPAddressHasOpenPort(OntolocyRelationship):
-
     __relationshiptype__: ClassVar[str] = "IP_ADDRESS_HAS_OPEN_PORT"
 
     source: IPAddressNode
     target: ListeningSocket
 
 
 class IPAddressBelongsToASN(OntolocyRelationship):
-
     __relationshiptype__: ClassVar[str] = "IP_ADDRESS_BELONGS_TO_ASN"
 
     source: IPAddressNode
     target: ASN
 
 
 class IPAddressLocatedInCountry(OntolocyRelationship):
-
     __relationshiptype__: ClassVar[str] = "IP_ADDRESS_LOCATED_IN_COUNTRY"
 
     source: IPAddressNode
     target: Country
 
 
 class IPAddressIdentifiedAsPlatform(OntolocyRelationship):
-
     __relationshiptype__: ClassVar[str] = "IP_ADDRESS_IDENTIFIED_AS_PLATFORM"
 
     source: IPAddressNode
     target: CPE
+
+
+class IPAddressMapsToMACAddress(OntolocyRelationship):
+    __relationshiptype__: ClassVar[str] = "IP_ADDRESS_MAPS_TO_MAC_ADDRESS"
+
+    source: IPAddressNode
+    target: MACAddress
+
+
+class IPAddressObservedWithHostname(OntolocyRelationship):
+    __relationshiptype__: ClassVar[str] = "IP_ADDRESS_OBSERVED_WITH_HOSTNAME"
+
+    source: IPAddressNode
+    target: "DomainName"
+
+
+from .domainname import DomainName  # noqa: E402
+
+IPAddressObservedWithHostname.update_forward_refs()
```

### Comparing `ontolocy-0.1.3/src/ontolocy/models/jarmhash.py` & `ontolocy-0.3.0/src/ontolocy/models/jarmhash.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.1.3/src/ontolocy/models/listeningsocket.py` & `ontolocy-0.3.0/src/ontolocy/models/listeningsocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,17 @@
     ip_address: IPvAnyAddress
     ip_address_unique_id: Optional[
         UUID
     ] = None  # for private IPs, uniquely identify the IP to avoid collisions
 
     unique_id: Optional[UUID] = None
 
+    def get_identifier(self) -> str:
+        return f"{self.ip_address}:{self.port_number}"
+
     @validator("unique_id", always=True)
     def generate_socket_uuid(cls, v: Optional[UUID], values: Dict[str, Any]) -> UUID:
 
         if v is None:
 
             key_values = [
                 values["protocol"],
```

### Comparing `ontolocy-0.1.3/src/ontolocy/models/mitreattackcampaign.py` & `ontolocy-0.3.0/src/ontolocy/models/mitreattackcampaign.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.1.3/src/ontolocy/models/mitreattacksoftware.py` & `ontolocy-0.3.0/src/ontolocy/models/mitreattacksoftware.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.1.3/src/ontolocy/models/mitreattacktactic.py` & `ontolocy-0.3.0/src/ontolocy/models/mitreattacktactic.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.1.3/src/ontolocy/models/mitreattacktechnique.py` & `ontolocy-0.3.0/src/ontolocy/models/mitreattacktechnique.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.1.3/src/ontolocy/models/networkservice.py` & `ontolocy-0.3.0/src/ontolocy/models/networkservice.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.1.3/src/ontolocy/models/report.py` & `ontolocy-0.3.0/src/ontolocy/models/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from .cve import CVE
 from .cyberharm import CyberHarm
 from .intrusionset import IntrusionSet
 from .ip import IPAddressNode
 from .mitreattacksoftware import MitreAttackSoftware
 from .mitreattacktechnique import MitreAttackTechnique
 from .sector import Sector
+from .threatactor import ThreatActor
 
 
 class Report(OntolocyNode):
-
     __primaryproperty__: ClassVar[str] = "url_reference"
     __primarylabel__: ClassVar[Optional[str]] = "Report"
 
     title: str
     author: str
     url_reference: HttpUrl
     published_date: date
@@ -78,14 +78,21 @@
 class ReportIdentifiesIntrusionSet(OntolocyRelationship):
     source: Report
     target: IntrusionSet
 
     __relationshiptype__: ClassVar[str] = "REPORT_IDENTIFIES_INTRUSION_SET"
 
 
+class ReportIdentifiesThreatActor(OntolocyRelationship):
+    source: Report
+    target: ThreatActor
+
+    __relationshiptype__: ClassVar[str] = "REPORT_IDENTIFIES_THREAT_ACTOR"
+
+
 class ReportIdentifiesTechnique(OntolocyRelationship):
     source: Report
     target: MitreAttackTechnique
 
     __relationshiptype__: ClassVar[str] = "REPORT_IDENTIFIES_TECHNIQUE"
```

### Comparing `ontolocy-0.1.3/src/ontolocy/models/sector.py` & `ontolocy-0.3.0/src/ontolocy/models/sector.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.1.3/src/ontolocy/models/threatactor.py` & `ontolocy-0.3.0/src/ontolocy/models/threatactor.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from ..node import OntolocyNode
 from ..relationship import OntolocyRelationship
 from .actortype import ActorType
 from .country import Country
 
 
 class ThreatActor(OntolocyNode):
-
     __primaryproperty__: ClassVar[str] = "unique_id"
     __primarylabel__: ClassVar[Optional[str]] = "ThreatActor"
 
     name: str
     unique_id: str
     description: Optional[str]
     url_reference: Optional[HttpUrl]
@@ -34,7 +33,16 @@
 
 class ThreatActorIsOfType(OntolocyRelationship):
     source: ThreatActor
     target: ActorType
     url_reference: Optional[HttpUrl]
 
     __relationshiptype__: ClassVar[str] = "THREAT_ACTOR_IS_OF_TYPE"
+
+
+class ThreatActorLinkedToThreatActor(OntolocyRelationship):
+    source: ThreatActor
+    target: ThreatActor
+    url_reference: Optional[HttpUrl]
+    context: Optional[str]
+
+    __relationshiptype__: ClassVar[str] = "THREAT_ACTOR_LINKED_TO_THREAT_ACTOR"
```

### Comparing `ontolocy-0.1.3/src/ontolocy/models/x509certificate.py` & `ontolocy-0.3.0/src/ontolocy/models/x509certificate.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.1.3/src/ontolocy/node.py` & `ontolocy-0.3.0/src/ontolocy/node.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,7 +40,10 @@
         # if a data_origin is specified, merge that and then creat the OriginGenerated relationship
         if data_origin is not None:
             data_origin.merge()
 
             rel = OriginGenerated(source=data_origin, target=self)
 
             rel.merge()
+
+    def get_identifier(self) -> str:
+        return str(self.get_primary_property_value())
```

### Comparing `ontolocy-0.1.3/src/ontolocy/relationship.py` & `ontolocy-0.3.0/src/ontolocy/relationship.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.1.3/src/ontolocy/utils.py` & `ontolocy-0.3.0/src/ontolocy/utils.py`

 * *Files identical despite different names*

### Comparing `ontolocy-0.1.3/src/ontolocy.egg-info/PKG-INFO` & `ontolocy-0.3.0/src/ontolocy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontolocy
-Version: 0.1.3
+Version: 0.3.0
 Summary: A Python package for modeling cybersecurity data in a Neo4j graph database.
 Home-page: https://github.com/ontolocy/ontolocy-lib
 Author: Ontolocy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -14,7 +14,11 @@
 # Ontolocy
 
 An open source cyber security graph ontology.
 
 Use Python and Neo4j to explore cyber security data as a graph.
 
 Currently in alpha/proof-of-concept stage - the ontology is likely to change.
+
+> "All models are wrong, but some are useful" - George Box
+
+Read the [docs](https://ontolocy.readthedocs.io/)
```

### Comparing `ontolocy-0.1.3/src/ontolocy.egg-info/SOURCES.txt` & `ontolocy-0.3.0/src/ontolocy.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,32 +16,36 @@
 src/ontolocy/models/actortype.py
 src/ontolocy/models/asn.py
 src/ontolocy/models/banner.py
 src/ontolocy/models/campaign.py
 src/ontolocy/models/capecpattern.py
 src/ontolocy/models/cobaltstrikebeacon.py
 src/ontolocy/models/cobaltstrikewatermark.py
+src/ontolocy/models/control.py
 src/ontolocy/models/country.py
 src/ontolocy/models/cpe.py
 src/ontolocy/models/cve.py
 src/ontolocy/models/cwe.py
 src/ontolocy/models/cyberharm.py
 src/ontolocy/models/dnsrecord.py
 src/ontolocy/models/domainname.py
 src/ontolocy/models/exploit.py
+src/ontolocy/models/host.py
 src/ontolocy/models/intrusionset.py
 src/ontolocy/models/ip.py
 src/ontolocy/models/jarmhash.py
 src/ontolocy/models/listeningsocket.py
+src/ontolocy/models/macaddress.py
 src/ontolocy/models/mitreattackcampaign.py
 src/ontolocy/models/mitreattacksoftware.py
 src/ontolocy/models/mitreattacktactic.py
 src/ontolocy/models/mitreattacktechnique.py
 src/ontolocy/models/networkservice.py
 src/ontolocy/models/organisation.py
 src/ontolocy/models/port.py
 src/ontolocy/models/report.py
 src/ontolocy/models/sector.py
 src/ontolocy/models/threatactor.py
 src/ontolocy/models/url.py
+src/ontolocy/models/useraccount.py
 src/ontolocy/models/x509certificate.py
 tests/test_node.py
```

### Comparing `ontolocy-0.1.3/tests/test_node.py` & `ontolocy-0.3.0/tests/test_node.py`

 * *Files identical despite different names*

